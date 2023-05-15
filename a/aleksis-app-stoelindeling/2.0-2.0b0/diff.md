# Comparing `tmp/aleksis_app_stoelindeling-2.0.tar.gz` & `tmp/aleksis_app_stoelindeling-2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_stoelindeling-2.0.tar", max compression
+gzip compressed data, was "aleksis_app_stoelindeling-2.0b0.tar", max compression
```

## Comparing `aleksis_app_stoelindeling-2.0.tar` & `aleksis_app_stoelindeling-2.0b0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0     1712 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/LICENCE.rst
--rw-r--r--   0        0        0     1258 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/README.rst
--rw-r--r--   0        0        0      159 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__init__.py
--rw-r--r--   0        0        0      465 2023-05-15 16:37:34.126660 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      879 2023-05-15 16:37:34.666685 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0        0        0     3169 2023-05-15 16:37:35.630731 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/managers.cpython-311.pyc
--rw-r--r--   0        0        0     3789 2023-05-15 16:37:35.798739 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/model_extensions.cpython-311.pyc
--rw-r--r--   0        0        0     4460 2023-05-15 16:37:35.630731 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/models.cpython-311.pyc
--rw-r--r--   0        0        0     2470 2023-05-15 16:37:35.706735 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/rules.cpython-311.pyc
--rw-r--r--   0        0        0      398 2023-05-15 16:37:34.130660 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0        0        0      421 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/apps.py
--rw-r--r--   0        0        0     5322 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/forms.py
--rw-r--r--   0        0        0     2274 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/index.js
--rw-r--r--   0        0        0       60 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/messages/de.json
--rw-r--r--   0        0        0       63 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/messages/en.json
--rw-r--r--   0        0        0       77 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/messages/ru.json
--rw-r--r--   0        0        0       81 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/messages/uk.json
--rw-r--r--   0        0        0        0 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-05-15 16:37:36.114754 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4214 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2185 2023-05-15 16:37:36.106754 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4847 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-15 16:37:36.114754 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4130 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-15 16:37:36.098753 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4084 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-15 16:37:36.106754 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4084 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2749 2023-05-15 16:37:36.102753 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5359 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-15 16:37:36.114754 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     4084 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     2919 2023-05-15 16:37:36.102753 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     5532 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1599 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/managers.py
--rw-r--r--   0        0        0     3115 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0001_initial.py
--rw-r--r--   0        0        0     1166 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0002_seat_auto_create.py
--rw-r--r--   0        0        0      870 2023-05-15 16:35:12.011924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0003_seat_negative_x_y.py
--rw-r--r--   0        0        0      596 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0004_alter_seatingplan_subject.py
--rw-r--r--   0        0        0      680 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0005_alter_seatingplan_room.py
--rw-r--r--   0        0        0        0 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/__init__.py
--rw-r--r--   0        0        0     1856 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/model_extensions.py
--rw-r--r--   0        0        0     2317 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/models.py
--rw-r--r--   0        0        0     2430 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/rules.py
--rw-r--r--   0        0        0      160 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/settings.py
--rw-r--r--   0        0        0        0 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/static/.keepdir
--rw-r--r--   0        0        0      998 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/static/css/stoelindeling/seating_plan.css
--rw-r--r--   0        0        0     2820 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/static/js/stoelindeling/edit_seating_plan.js
--rw-r--r--   0        0        0      758 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/tables.py
--rw-r--r--   0        0        0      201 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/partials/seat.html
--rw-r--r--   0        0        0      710 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/copy.html
--rw-r--r--   0        0        0      630 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/create.html
--rw-r--r--   0        0        0     3125 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/edit.html
--rw-r--r--   0        0        0      714 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/list.html
--rw-r--r--   0        0        0      534 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/render.html
--rw-r--r--   0        0        0     1446 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/view.html
--rw-r--r--   0        0        0      831 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/urls.py
--rw-r--r--   0        0        0     3264 2023-05-15 16:37:35.706735 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/util/__pycache__/perms.cpython-311.pyc
--rw-r--r--   0        0        0     1748 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/util/perms.py
--rw-r--r--   0        0        0     6650 2023-05-15 16:35:12.015924 aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/views.py
--rw-r--r--   0        0        0     1500 2023-05-15 16:35:45.125497 aleksis_app_stoelindeling-2.0/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-05-15 16:35:12.023924 aleksis_app_stoelindeling-2.0/tox.ini
--rw-r--r--   0        0        0     3261 1970-01-01 00:00:00.000000 aleksis_app_stoelindeling-2.0/setup.py
--rw-r--r--   0        0        0     2230 1970-01-01 00:00:00.000000 aleksis_app_stoelindeling-2.0/PKG-INFO
+-rw-r--r--   0        0        0     1569 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1258 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/README.rst
+-rw-r--r--   0        0        0      159 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__init__.py
+-rw-r--r--   0        0        0      465 2023-03-01 18:53:12.407842 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      879 2023-03-01 18:53:12.895841 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/apps.cpython-311.pyc
+-rw-r--r--   0        0        0     3169 2023-03-01 18:53:13.739840 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/managers.cpython-311.pyc
+-rw-r--r--   0        0        0     3789 2023-03-01 18:53:13.827840 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/model_extensions.cpython-311.pyc
+-rw-r--r--   0        0        0     4460 2023-03-01 18:53:13.671840 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0        0        0     2470 2023-03-01 18:53:13.791840 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/rules.cpython-311.pyc
+-rw-r--r--   0        0        0      398 2023-03-01 18:53:12.411842 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0        0        0      421 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/apps.py
+-rw-r--r--   0        0        0     5322 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/forms.py
+-rw-r--r--   0        0        0     2274 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/index.js
+-rw-r--r--   0        0        0       60 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/messages/de.json
+-rw-r--r--   0        0        0       63 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/messages/en.json
+-rw-r--r--   0        0        0       77 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/messages/ru.json
+-rw-r--r--   0        0        0       81 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/messages/uk.json
+-rw-r--r--   0        0        0        0 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-03-01 18:53:14.159839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4214 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2185 2023-03-01 18:53:14.179839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4847 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-01 18:53:14.147839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4130 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 18:53:14.151839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4084 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 18:53:14.175839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4084 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2749 2023-03-01 18:53:14.175839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5359 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-01 18:53:14.163839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     4084 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     2919 2023-03-01 18:53:14.163839 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     5532 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1599 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/managers.py
+-rw-r--r--   0        0        0     3115 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1166 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0002_seat_auto_create.py
+-rw-r--r--   0        0        0      870 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0003_seat_negative_x_y.py
+-rw-r--r--   0        0        0      596 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0004_alter_seatingplan_subject.py
+-rw-r--r--   0        0        0      680 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0005_alter_seatingplan_room.py
+-rw-r--r--   0        0        0        0 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/__init__.py
+-rw-r--r--   0        0        0     1856 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/model_extensions.py
+-rw-r--r--   0        0        0     2317 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/models.py
+-rw-r--r--   0        0        0     2430 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/rules.py
+-rw-r--r--   0        0        0      160 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/settings.py
+-rw-r--r--   0        0        0        0 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/static/.keepdir
+-rw-r--r--   0        0        0      998 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/static/css/stoelindeling/seating_plan.css
+-rw-r--r--   0        0        0     2820 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/static/js/stoelindeling/edit_seating_plan.js
+-rw-r--r--   0        0        0      758 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/tables.py
+-rw-r--r--   0        0        0      201 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/partials/seat.html
+-rw-r--r--   0        0        0      710 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/copy.html
+-rw-r--r--   0        0        0      630 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/create.html
+-rw-r--r--   0        0        0     3125 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/edit.html
+-rw-r--r--   0        0        0      714 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/list.html
+-rw-r--r--   0        0        0      534 2023-03-01 18:50:07.756211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/render.html
+-rw-r--r--   0        0        0     1446 2023-03-01 18:50:07.760211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/view.html
+-rw-r--r--   0        0        0      831 2023-03-01 18:50:07.760211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/urls.py
+-rw-r--r--   0        0        0     3264 2023-03-01 18:53:13.795840 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/util/__pycache__/perms.cpython-311.pyc
+-rw-r--r--   0        0        0     1748 2023-03-01 18:50:07.760211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/util/perms.py
+-rw-r--r--   0        0        0     6650 2023-03-01 18:50:07.760211 aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/views.py
+-rw-r--r--   0        0        0     1506 2023-03-01 18:50:41.764144 aleksis_app_stoelindeling-2.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-03-01 18:50:07.776211 aleksis_app_stoelindeling-2.0b0/tox.ini
+-rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 aleksis_app_stoelindeling-2.0b0/setup.py
+-rw-r--r--   0        0        0     2236 1970-01-01 00:00:00.000000 aleksis_app_stoelindeling-2.0b0/PKG-INFO
```

### Comparing `aleksis_app_stoelindeling-2.0/CHANGELOG.rst` & `aleksis_app_stoelindeling-2.0b0/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,16 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`2.0`_ - 2023-05-15
--------------------
-
-Nothing changed.
-
-`2.0b0`_ - 2023-03-01
----------------------
+`2.0b0` - 2023-03-01
+--------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
@@ -63,8 +58,7 @@
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
 
 .. _1.0: https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling/-/tags/1.0
 .. _1.0.1: https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling/-/tags/1.0.1
 .. _1.0.2: https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling/-/tags/1.0.2
 .. _2.0b0: https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling/-/tags/2.0b0
-.. _2.0: https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling/-/tags/2.0
```

### Comparing `aleksis_app_stoelindeling-2.0/LICENCE.rst` & `aleksis_app_stoelindeling-2.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/README.rst` & `aleksis_app_stoelindeling-2.0b0/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/apps.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/apps.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 421
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/managers.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/managers.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 1599
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/model_extensions.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/model_extensions.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 1856
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 10
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/models.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/models.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 2317
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/__pycache__/rules.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/__pycache__/rules.cpython-311.pyc`

 * *Files 1% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 2430
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/forms.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/frontend/index.js` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/managers.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/managers.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0001_initial.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0002_seat_auto_create.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0002_seat_auto_create.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0003_seat_negative_x_y.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0003_seat_negative_x_y.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0004_alter_seatingplan_subject.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0004_alter_seatingplan_subject.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/migrations/0005_alter_seatingplan_room.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/migrations/0005_alter_seatingplan_room.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/model_extensions.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/model_extensions.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/models.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/rules.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/static/css/stoelindeling/seating_plan.css` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/static/css/stoelindeling/seating_plan.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/static/js/stoelindeling/edit_seating_plan.js` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/static/js/stoelindeling/edit_seating_plan.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/tables.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/copy.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/copy.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/create.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/create.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/edit.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/edit.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/list.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/render.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/render.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/view.html` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/templates/stoelindeling/seating_plan/view.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/urls.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/util/__pycache__/perms.cpython-311.pyc` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/util/__pycache__/perms.cpython-311.pyc`

 * *Files 0% similar despite different names*

#### Python bytecode

```diff
@@ -1,9 +1,9 @@
 magic:    0xa70d0d0a
-moddate:  0x405f6264 (Mon May 15 16:35:12 2023 UTC)
+moddate:  0x5f9eff63 (Wed Mar  1 18:50:07 2023 UTC)
 files sz: 1748
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 5
    flags     : 0
    code
```

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/util/perms.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/util/perms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/aleksis/apps/stoelindeling/views.py` & `aleksis_app_stoelindeling-2.0b0/aleksis/apps/stoelindeling/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/pyproject.toml` & `aleksis_app_stoelindeling-2.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Stoelindeling"
-version = "2.0"
+version = "2.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -26,16 +26,16 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0"
-aleksis-app-chronos = "^3.0"
+aleksis-core = "^3.0b0"
+aleksis-app-chronos = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 stoelindeling = "aleksis.apps.stoelindeling.apps:DefaultConfig"
```

### Comparing `aleksis_app_stoelindeling-2.0/tox.ini` & `aleksis_app_stoelindeling-2.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_stoelindeling-2.0/setup.py` & `aleksis_app_stoelindeling-2.0b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,23 +23,23 @@
                                 'static/*',
                                 'static/css/stoelindeling/*',
                                 'static/js/stoelindeling/*',
                                 'templates/stoelindeling/partials/*',
                                 'templates/stoelindeling/seating_plan/*']}
 
 install_requires = \
-['aleksis-app-chronos>=3.0,<4.0', 'aleksis-core>=3.0,<4.0']
+['aleksis-app-chronos>=3.0b0,<4.0', 'aleksis-core>=3.0b0,<4.0']
 
 entry_points = \
 {'aleksis.app': ['stoelindeling = '
                  'aleksis.apps.stoelindeling.apps:DefaultConfig']}
 
 setup_kwargs = {
     'name': 'aleksis-app-stoelindeling',
-    'version': '2.0',
+    'version': '2.0b0',
     'description': 'AlekSIS (School Information System)\u200a—\u200aApp Stoelindeling (Create and publish seating plans)',
     'long_description': 'AlekSIS (School Information System)\u200a—\u200aApp Stoelindeling (Create and publish seating plans)\n==========================================================================================\n\nAlekSIS\n-------\n\nThis is an application for use with the `AlekSIS®`_ platform.\n\nFeatures\n--------\n\n* Create and manage seating plans for different groups in different rooms.\n* Make these plans available in the class register.\n* Allow customizing plans for individual combinations of groups, subjects and rooms.\n\nLicence\n-------\n\n::\n\n  Copyright © 2022 Jonathan Weth <dev@jonathanweth.de>\n\n  Licenced under the EUPL, version 1.2 or later\n\nPlease see the LICENCE.rst file accompanying this distribution for the\nfull licence text or on the `European Union Public Licence`_ website\nhttps://joinup.ec.europa.eu/collection/eupl/guidelines-users-and-developers\n(including all other official language versions).\n\nTrademark\n---------\n\nAlekSIS® is a registered trademark of the AlekSIS open source project, represented\nby Teckids e.V. Please refer to the `trademark policy`_ for hints on using the trademark\nAlekSIS®.\n\n.. _AlekSIS®: https://edugit.org/AlekSIS/AlekSIS\n.. _European Union Public Licence: https://eupl.eu/\n.. _trademark policy: https://aleksis.org/pages/about\n',
     'author': 'Jonathan Weth',
     'author_email': 'dev@jonathanweth.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://aleksis.org',
```

### Comparing `aleksis_app_stoelindeling-2.0/PKG-INFO` & `aleksis_app_stoelindeling-2.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: aleksis-app-stoelindeling
-Version: 2.0
+Version: 2.0b0
 Summary: AlekSIS (School Information System) — App Stoelindeling (Create and publish seating plans)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Requires-Python: >=3.9,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-app-chronos (>=3.0,<4.0)
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-app-chronos (>=3.0b0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/official/AlekSIS-App-Stoelindeling
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Stoelindeling (Create and publish seating plans)
 ==========================================================================================
```

