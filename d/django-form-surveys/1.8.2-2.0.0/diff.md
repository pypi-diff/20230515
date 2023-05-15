# Comparing `tmp/django-form-surveys-1.8.2.tar.gz` & `tmp/django-form-surveys-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-form-surveys-1.8.2.tar", last modified: Wed Apr 26 01:47:36 2023, max compression
+gzip compressed data, was "django-form-surveys-2.0.0.tar", last modified: Mon May 15 09:18:06 2023, max compression
```

## Comparing `django-form-surveys-1.8.2.tar` & `django-form-surveys-2.0.0.tar`

### file list

```diff
@@ -1,111 +1,129 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/MANIFEST.in
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5144 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.936463 django-form-surveys-1.8.2/django_form_surveys.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6392 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/not-zip-safe
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-04-26 01:47:36.000000 django-form-surveys-1.8.2/django_form_surveys.egg-info/top_level.txt
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.944463 django-form-surveys-1.8.2/djf_surveys/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-04-26 01:44:42.000000 django-form-surveys-1.8.2/djf_surveys/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admin.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.944463 django-form-surveys-1.8.2/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admins/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1298 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/admins/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8146 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/admins/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/app_settings.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/apps.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      228 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/context_processors.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/forms.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.948463 django-form-surveys-1.8.2/djf_surveys/migrations/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0001_initial.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0002_auto_20220330_1033.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0003_auto_20220330_1036.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0004_auto_20220330_1112.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0005_auto_20220404_1518.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0006_survey_private_response.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0007_auto_20220525_1126.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0008_auto_20220721_0935.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0009_auto_20220803_0927.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0010_model_translation.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-1.8.2/djf_surveys/migrations/0011_alter_question_key.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/migrations/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/mixin.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-1.8.2/djf_surveys/models.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.948463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/rating.css
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   356448 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   455935 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.952463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-border.png
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-fill.png
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.952463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   198463 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      121 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.968463 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   270873 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   783041 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12217 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50339 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   425275 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1151819 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   539120 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1929935 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7170 2022-12-26 04:13:44.000000 django-form-surveys-1.8.2/djf_surveys/summary.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.928463 django-form-surveys-1.8.2/djf_surveys/templates/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.976462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.976462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6956 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form_preview.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1020 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/question_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/summary.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/survey_list.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4237 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/answer_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.980462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/add_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/delete_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/edit_button.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/buttons/share_button.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/empty_state.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/header_nav.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3074 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5379 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/pagination.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      938 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/search_form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      542 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/section_welcome.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_border.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_fill.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      889 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/detail_result.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2014 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/form.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      792 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/master.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/survey_list.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-04-26 01:44:17.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/datepicker.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/djf_surveys/templatetags/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/templatetags/__init__.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/templatetags/djf_survey_tags.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/tests.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-1.8.2/djf_surveys/urls.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2277 2023-03-15 09:08:50.000000 django-form-surveys-1.8.2/djf_surveys/utils.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      550 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/djf_surveys/validators.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-1.8.2/djf_surveys/views.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      477 2022-10-24 00:52:04.000000 django-form-surveys-1.8.2/djf_surveys/widgets.py
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-04-26 01:47:36.984462 django-form-surveys-1.8.2/setup.cfg
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-1.8.2/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1059 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      158 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/MANIFEST.in
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6504 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5256 2023-05-15 04:57:18.000000 django-form-surveys-2.0.0/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.238770 django-form-surveys-2.0.0/django_form_surveys.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6504 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4870 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4287 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/dependency_links.txt.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2022-12-03 04:02:38.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/not-zip-safe
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       17 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/requires.txt.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-15 09:18:06.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-12 07:36:56.000000 django-form-surveys-2.0.0/django_form_surveys.egg-info/top_level.txt.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       81 2023-05-15 04:59:14.000000 django-form-surveys-2.0.0/djf_surveys/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      977 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/admin.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/admins/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1378 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/admins/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8232 2023-05-12 08:29:19.000000 django-form-surveys-2.0.0/djf_surveys/admins/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1650 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/app_settings.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      194 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/apps.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      315 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/context_processors.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6449 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/forms.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/en/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.242770 django-form-surveys-2.0.0/djf_surveys/locale/en/LC_MESSAGES/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5632 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/en/LC_MESSAGES/django.mo
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/fr/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.246770 django-form-surveys-2.0.0/djf_surveys/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6132 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/fr/LC_MESSAGES/django.mo
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/locale/id/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.246770 django-form-surveys-2.0.0/djf_surveys/locale/id/LC_MESSAGES/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5908 2023-05-15 09:18:04.000000 django-form-surveys-2.0.0/djf_surveys/locale/id/LC_MESSAGES/django.mo
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.250770 django-form-surveys-2.0.0/djf_surveys/migrations/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3775 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0001_initial.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      860 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0002_auto_20220330_1033.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      553 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0003_auto_20220330_1036.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      850 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0004_auto_20220330_1112.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      377 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0005_auto_20220404_1518.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      451 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0006_survey_private_response.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      895 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0007_auto_20220525_1126.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0008_auto_20220721_0935.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      784 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0009_auto_20220803_0927.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8956 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0010_model_translation.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      662 2022-12-26 04:31:54.000000 django-form-surveys-2.0.0/djf_surveys/migrations/0011_alter_question_key.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/migrations/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      611 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/mixin.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7182 2023-04-17 04:11:38.000000 django-form-surveys-2.0.0/djf_surveys/models.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.250770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      321 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/rating.css
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   356448 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   455935 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.254770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2962 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-border.png
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2729 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-fill.png
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.230770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.254770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   198463 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      121 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css.map
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.270770 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   270873 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   783041 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    12217 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)    50339 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   425275 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1151819 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)   539120 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)  1929935 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7140 2023-05-12 08:30:24.000000 django-form-surveys-2.0.0/djf_surveys/summary.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.234770 django-form-surveys-2.0.0/djf_surveys/templates/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.278770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.282770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1761 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     7165 2023-05-12 07:25:35.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form_preview.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1132 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      702 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       45 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form_v2.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1790 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/summary.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1490 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/survey_list.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     4237 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/answer_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.282770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      292 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/add_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      343 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/delete_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      309 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/edit_button.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      457 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/buttons/share_button.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.286770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1638 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      326 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2955 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2779 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      347 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/empty_state.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3324 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/header_nav.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3622 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3073 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      777 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3552 2023-05-12 07:21:46.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/pagination.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      968 2023-05-12 07:05:05.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/search_form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      570 2023-05-12 07:05:05.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/section_welcome.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      557 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_border.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_fill.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      889 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/detail_result.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2014 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/form.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      792 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/master.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1189 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/survey_list.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.286770 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      247 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      538 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      364 2023-04-26 01:44:17.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/datepicker.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     5069 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/inline_choices.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      520 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1767 2023-03-15 09:08:50.000000 django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/djf_surveys/templatetags/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        0 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/templatetags/__init__.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      509 2023-03-15 09:08:50.000000 django-form-surveys-2.0.0/djf_surveys/templatetags/djf_survey_tags.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      396 2022-10-24 00:52:04.000000 django-form-surveys-2.0.0/djf_surveys/tests.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      799 2022-12-02 18:18:26.000000 django-form-surveys-2.0.0/djf_surveys/urls.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3722 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/utils.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      514 2023-05-12 08:31:40.000000 django-form-surveys-2.0.0/djf_surveys/validators.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     8190 2022-12-26 03:50:09.000000 django-form-surveys-2.0.0/djf_surveys/views.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     1096 2023-05-12 03:45:22.000000 django-form-surveys-2.0.0/djf_surveys/widgets.py
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2023-05-15 09:18:06.290770 django-form-surveys-2.0.0/setup.cfg
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3085 2022-12-01 07:58:14.000000 django-form-surveys-2.0.0/setup.py
```

### Comparing `django-form-surveys-1.8.2/LICENSE` & `django-form-surveys-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/PKG-INFO` & `django-form-surveys-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.2
+Version: 2.0.0
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -88,14 +88,15 @@
 - Option config survey:
     - `editable`: this option allows the user to edit the answer
     - `deletable`: this option allows the user to delete the answer
     - `duplicate entry`: this option allows users to submit more than once
     - `private reponse`: this option makes the answer list only visible to admin
     - `can anonymous user`: This option allows users without authentication to submit
 - Support many question type (type field): Available field types include:
+![image](https://user-images.githubusercontent.com/11069520/237864026-9f933369-4cf0-4292-a394-ac398eb1be9b.png)
     - Text 
     - Number
     - Radio 
     - Select 
     - Multi Select 
     - Text Area 
     - URL
```

### Comparing `django-form-surveys-1.8.2/README.md` & `django-form-surveys-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 - Option config survey:
     - `editable`: this option allows the user to edit the answer
     - `deletable`: this option allows the user to delete the answer
     - `duplicate entry`: this option allows users to submit more than once
     - `private reponse`: this option makes the answer list only visible to admin
     - `can anonymous user`: This option allows users without authentication to submit
 - Support many question type (type field): Available field types include:
+![image](https://user-images.githubusercontent.com/11069520/237864026-9f933369-4cf0-4292-a394-ac398eb1be9b.png)
     - Text 
     - Number
     - Radio 
     - Select 
     - Multi Select 
     - Text Area 
     - URL
```

### Comparing `django-form-surveys-1.8.2/django_form_surveys.egg-info/PKG-INFO` & `django-form-surveys-2.0.0/django_form_surveys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-form-surveys
-Version: 1.8.2
+Version: 2.0.0
 Summary: A simple Django app to conduct Web-based survey
 Home-page: https://irfanpule.github.io/django-form-surveys
 Author: irfanpule
 Author-email: irfan.pule2@gmail.com
 License: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -88,14 +88,15 @@
 - Option config survey:
     - `editable`: this option allows the user to edit the answer
     - `deletable`: this option allows the user to delete the answer
     - `duplicate entry`: this option allows users to submit more than once
     - `private reponse`: this option makes the answer list only visible to admin
     - `can anonymous user`: This option allows users without authentication to submit
 - Support many question type (type field): Available field types include:
+![image](https://user-images.githubusercontent.com/11069520/237864026-9f933369-4cf0-4292-a394-ac398eb1be9b.png)
     - Text 
     - Number
     - Radio 
     - Select 
     - Multi Select 
     - Text Area 
     - URL
```

### Comparing `django-form-surveys-1.8.2/django_form_surveys.egg-info/SOURCES.txt` & `django-form-surveys-2.0.0/django_form_surveys.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 django_form_surveys.egg-info/PKG-INFO
 django_form_surveys.egg-info/SOURCES.txt
+django_form_surveys.egg-info/SOURCES.txt.py
 django_form_surveys.egg-info/dependency_links.txt
+django_form_surveys.egg-info/dependency_links.txt.py
 django_form_surveys.egg-info/not-zip-safe
 django_form_surveys.egg-info/requires.txt
+django_form_surveys.egg-info/requires.txt.py
 django_form_surveys.egg-info/top_level.txt
+django_form_surveys.egg-info/top_level.txt.py
 djf_surveys/__init__.py
 djf_surveys/admin.py
 djf_surveys/app_settings.py
 djf_surveys/apps.py
 djf_surveys/context_processors.py
 djf_surveys/forms.py
 djf_surveys/mixin.py
@@ -22,14 +26,17 @@
 djf_surveys/utils.py
 djf_surveys/validators.py
 djf_surveys/views.py
 djf_surveys/widgets.py
 djf_surveys/admins/__init__.py
 djf_surveys/admins/urls.py
 djf_surveys/admins/views.py
+djf_surveys/locale/en/LC_MESSAGES/django.mo
+djf_surveys/locale/fr/LC_MESSAGES/django.mo
+djf_surveys/locale/id/LC_MESSAGES/django.mo
 djf_surveys/migrations/0001_initial.py
 djf_surveys/migrations/0002_auto_20220330_1033.py
 djf_surveys/migrations/0003_auto_20220330_1036.py
 djf_surveys/migrations/0004_auto_20220330_1112.py
 djf_surveys/migrations/0005_auto_20220404_1518.py
 djf_surveys/migrations/0006_survey_private_response.py
 djf_surveys/migrations/0007_auto_20220525_1126.py
@@ -58,33 +65,37 @@
 djf_surveys/templates/djf_surveys/form.html
 djf_surveys/templates/djf_surveys/master.html
 djf_surveys/templates/djf_surveys/survey_list.html
 djf_surveys/templates/djf_surveys/admins/form.html
 djf_surveys/templates/djf_surveys/admins/form_preview.html
 djf_surveys/templates/djf_surveys/admins/master.html
 djf_surveys/templates/djf_surveys/admins/question_form.html
+djf_surveys/templates/djf_surveys/admins/question_form_v2.html
 djf_surveys/templates/djf_surveys/admins/summary.html
 djf_surveys/templates/djf_surveys/admins/survey_list.html
 djf_surveys/templates/djf_surveys/buttons/add_button.html
 djf_surveys/templates/djf_surveys/buttons/delete_button.html
 djf_surveys/templates/djf_surveys/buttons/edit_button.html
 djf_surveys/templates/djf_surveys/buttons/share_button.html
 djf_surveys/templates/djf_surveys/components/alert.html
 djf_surveys/templates/djf_surveys/components/alert_js.html
 djf_surveys/templates/djf_surveys/components/card_list_answer.html
 djf_surveys/templates/djf_surveys/components/card_list_survey.html
 djf_surveys/templates/djf_surveys/components/empty_state.html
 djf_surveys/templates/djf_surveys/components/header_nav.html
+djf_surveys/templates/djf_surveys/components/modal_choice_field_type.html
 djf_surveys/templates/djf_surveys/components/modal_delete.html
 djf_surveys/templates/djf_surveys/components/modal_delete_js.html
 djf_surveys/templates/djf_surveys/components/pagination.html
 djf_surveys/templates/djf_surveys/components/search_form.html
 djf_surveys/templates/djf_surveys/components/section_welcome.html
 djf_surveys/templates/djf_surveys/components/share_link_button_js.html
 djf_surveys/templates/djf_surveys/components/star_border.html
 djf_surveys/templates/djf_surveys/components/star_fill.html
+djf_surveys/templates/djf_surveys/widgets/attrs_exclude_id.html
 djf_surveys/templates/djf_surveys/widgets/checkbox_option.html
 djf_surveys/templates/djf_surveys/widgets/datepicker.html
+djf_surveys/templates/djf_surveys/widgets/inline_choices.html
 djf_surveys/templates/djf_surveys/widgets/radio_option.html
 djf_surveys/templates/djf_surveys/widgets/star_rating.html
 djf_surveys/templatetags/__init__.py
 djf_surveys/templatetags/djf_survey_tags.py
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/admin.py` & `django-form-surveys-2.0.0/djf_surveys/admin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/admins/urls.py` & `django-form-surveys-2.0.0/djf_surveys/admins/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from django.urls import path
 from djf_surveys.admins import views as admin_views
+from djf_surveys.admins.v2 import views as admin_views_v2
 
 
 urlpatterns = [
     path('', admin_views.AdminSurveyListView.as_view(), name='admin_survey'),
     path('create/survey/', admin_views.AdminCrateSurveyView.as_view(), name='admin_create_survey'),
     path('edit/survey/<str:slug>/', admin_views.AdminEditSurveyView.as_view(), name='admin_edit_survey'),
     path('delete/survey/<str:slug>/', admin_views.AdminDeleteSurveyView.as_view(), name='admin_delete_survey'),
     path('forms/<str:slug>/', admin_views.AdminSurveyFormView.as_view(), name='admin_forms_survey'),
-    path('question/add/<int:pk>/', admin_views.AdminCreateQuestionView.as_view(), name='admin_create_question'),
-    path('question/edit/<int:pk>/', admin_views.AdminUpdateQuestionView.as_view(), name='admin_edit_question'),
+    path('question/add/<int:pk>/<int:type_field>', admin_views_v2.AdminCreateQuestionView.as_view(), name='admin_create_question'),
+    path('question/edit/<int:pk>/', admin_views_v2.AdminUpdateQuestionView.as_view(), name='admin_edit_question'),
     path('question/delete/<int:pk>/', admin_views.AdminDeleteQuestionView.as_view(), name='admin_delete_question'),
     path('question/ordering/', admin_views.AdminChangeOrderQuestionView.as_view(), name='admin_change_order_question'),
     path('download/survey/<str:slug>/', admin_views.DownloadResponseSurveyView.as_view(), name='admin_download_survey'),
     path('summary/survey/<str:slug>/', admin_views.SummaryResponseSurveyView.as_view(), name='admin_summary_survey'),
 ]
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/admins/views.py` & `django-form-surveys-2.0.0/djf_surveys/admins/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,20 +84,23 @@
 @method_decorator(staff_member_required, name='dispatch')
 class AdminDeleteSurveyView(DetailView):
     model = Survey
 
     def get(self, request, *args, **kwargs):
         survey = self.get_object()
         survey.delete()
-        messages.success(request, gettext("Survey %(name)s succesfully deleted.") % dict(name=survey.name))
+        messages.success(request, gettext("Survey %ss succesfully deleted.") % survey.name)
         return redirect("djf_surveys:admin_survey")
 
 
 @method_decorator(staff_member_required, name='dispatch')
 class AdminCreateQuestionView(ContextTitleMixin, CreateView):
+    """
+    Note: This class already has version 2
+    """
     model = Question
     template_name = 'djf_surveys/admins/question_form.html'
     success_url = reverse_lazy("djf_surveys:")
     fields = ['label', 'key', 'type_field', 'choices', 'help_text', 'required']
     title_page = _("Add Question")
     survey = None
 
@@ -118,14 +121,17 @@
 
     def get_success_url(self):
         return reverse("djf_surveys:admin_forms_survey", args=[self.survey.slug])
 
 
 @method_decorator(staff_member_required, name='dispatch')
 class AdminUpdateQuestionView(ContextTitleMixin, UpdateView):
+    """
+    Note: This class already has version 2
+    """
     model = Question
     template_name = 'djf_surveys/admins/question_form.html'
     success_url = SURVEYS_ADMIN_BASE_PATH
     fields = ['label', 'key', 'type_field', 'choices', 'help_text', 'required']
     title_page = _("Add Question")
     survey = None
 
@@ -147,15 +153,15 @@
         question = self.get_object()
         self.survey = question.survey
         return super().dispatch(request, *args, **kwargs)
 
     def get(self, request, *args, **kwargs):
         question = self.get_object()
         question.delete()
-        messages.success(request, gettext("Question %(name)s succesfully deleted.") % dict(name=question.label))
+        messages.success(request, gettext("Question %ss succesfully deleted.") % question.label)
         return redirect("djf_surveys:admin_forms_survey", slug=self.survey.slug)
 
 
 @method_decorator(staff_member_required, name='dispatch')
 class AdminChangeOrderQuestionView(View):
     def post(self, request, *args, **kwargs):
         ordering = request.POST['order_question'].split(",")
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/app_settings.py` & `django-form-surveys-2.0.0/djf_surveys/app_settings.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/forms.py` & `django-form-surveys-2.0.0/djf_surveys/forms.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0001_initial.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0002_auto_20220330_1033.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0002_auto_20220330_1033.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0003_auto_20220330_1036.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0003_auto_20220330_1036.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0004_auto_20220330_1112.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0004_auto_20220330_1112.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0007_auto_20220525_1126.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0007_auto_20220525_1126.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0008_auto_20220721_0935.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0008_auto_20220721_0935.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0009_auto_20220803_0927.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0009_auto_20220803_0927.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0010_model_translation.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0010_model_translation.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/migrations/0011_alter_question_key.py` & `django-form-surveys-2.0.0/djf_surveys/migrations/0011_alter_question_key.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/mixin.py` & `django-form-surveys-2.0.0/djf_surveys/mixin.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/models.py` & `django-form-surveys-2.0.0/djf_surveys/models.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/css/tailwindcss-plugin-3.3.1.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-border.png` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-border.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/images/star-fill.png` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/images/star-fill.png`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/css/tw-elements.min.css`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chart.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/chartjs-plugin-datalabels.es.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.es.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map` & `django-form-surveys-2.0.0/djf_surveys/static/djf_surveys/te-starter/js/tw-elements.umd.min.js.map`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/summary.py` & `django-form-surveys-2.0.0/djf_surveys/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -236,10 +236,10 @@
             input_types = ', '.join(str(x[1]) for x in models.Question.TYPE_FIELD if
                       x[0] in (models.TYPE_FIELD.radio, models.TYPE_FIELD.select, models.TYPE_FIELD.multi_select, models.TYPE_FIELD.rating))
             return """
 <div class="bg-yellow-100 space-y-1 py-5 rounded-md border border-yellow-200 text-center shadow-xs mb-2">
     <h1 class="text-2xl font-semibold">{}</h1>
     <h5 class="mb-0 mt-1 text-sm p-2">{}</h5>
 </div>
-""".format(gettext("No summary"), gettext("Summary is available only for input type: %(input_types)s") % dict(input_types=input_types))
+""".format(gettext("No summary"), gettext("Summary is available only for input type: %ss") % input_types)
 
         return " ".join(html_str)
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/form_preview.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/form_preview.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 {% extends 'djf_surveys/admins/master.html' %}
-{% load djf_survey_tags static %}
+{% load djf_survey_tags static i18n %}
 
 {% block extra_css %}
     <link rel="stylesheet" href="{% static 'djf_surveys/css/rating.css' %}"/>
 {% endblock %}
 
 {% block content %}
     <div class="flex py-1 fixed bottom-10 right-10">
-        <a href="{% url 'djf_surveys:admin_create_question' object.id %}"
-           class="z-20 block p-4 text-blue-100 transition-all bg-blue-700 border-2 border-white rounded-full active:bg-purple-50 hover:scale-110 focus:outline-none focus:ring"
-           type="button">
+        <button
+            class="z-20 block p-4 text-blue-100 transition-all bg-blue-700 border-2 border-white rounded-full active:bg-purple-50 hover:scale-110 focus:outline-none focus:ring"
+            data-te-toggle="modal"
+            data-te-target="#addQuestion"
+            data-te-ripple-init
+            data-te-ripple-color="light"
+            type="button">
             {% include "djf_surveys/buttons/add_button.html" with size=6 %}
-            <span class="items-center float-right"> Question </span>
-        </a>
+            <span class="items-center float-right"> {% trans 'Question' %} </span>
+        </button>
     </div>
 
     <div class="max-w-screen-xl px-4 py-16 mx-auto sm:px-6 lg:px-8">
         <div class="max-w-lg mx-auto">
             <div class="flex -space-x-4 hover:space-x-1 py-1 float-right">
                 <a href="{% url 'djf_surveys:admin_edit_survey' object.slug %}"
                    class="z-20 block p-4 text-blue-700 transition-all bg-blue-100 border-2 border-white rounded-full active:bg-blue-50 hover:scale-110 focus:outline-none focus:ring"
@@ -42,15 +46,15 @@
             </p>
 
             <form method="post" class="mx-auto mt-12" id="sortable">
                 {% csrf_token %}
                 {% for field in form %}
                     <div class="ui-state-default" id="{{ field|get_id_field }}">
                         <div class="flex -space-x-4 hover:space-x-1 py-1">
-                            <a href="{% url 'djf_surveys:admin_edit_question' field|get_id_field %}"
+                            <a href="{% url 'djf_surveys:admin_edit_question' field|get_id_field  %}"
                                class="z-20 block p-4 text-blue-700 transition-all bg-blue-100 border-2 border-white rounded-full active:bg-blue-50 hover:scale-110 focus:outline-none focus:ring"
                                type="button">
                                 {% include "djf_surveys/buttons/edit_button.html" %}
                             </a>
 
                             <a class="button-delete z-30 block p-4 text-red-700 transition-all bg-red-100 border-2 border-white rounded-full hover:scale-110 focus:outline-none focus:ring active:bg-red-50"
                                data-te-toggle="modal"
@@ -84,14 +88,15 @@
                     </div>
 
                 {% endfor %}
             </form>
         </div>
 
         {% include 'djf_surveys/components/modal_delete.html' %}
+        {% include 'djf_surveys/components/modal_choice_field_type.html' %}
     </div>
 
 {% endblock %}
 
 {% block extra_js %}
     <script src="https://code.jquery.com/jquery-3.6.1.js"></script>
     <script src="https://code.jquery.com/ui/1.13.2/jquery-ui.js"></script>
@@ -110,15 +115,15 @@
                             'order_question': order.toString(),
                         },
                         dataType: 'json',
                         success: function (data) {
                             console.log(data.message);
                         },
                         error: function (data) {
-                            alert("An error occured!");
+                            alert("{% trans 'An error occured!' %}");
                         }
                     });
                 }
             });
         });
     </script>
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/master.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/master.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,25 @@
-{% load static %}
 <!doctype html>
+{% load i18n static %}
 <html>
 <head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
-    <title>Survey - {{ title }}</title>
-    <link rel="stylesheet" href="{% static 'djf_surveys/te-starter/css/tw-elements.min.css' %}">
+    <title>{% trans "Survey" %} - {{ title }}</title>
     <script src="{% static 'djf_surveys/css/tailwindcss-3.3.1.js' %}"></script>
     <script src="{% static 'djf_surveys/css/tailwindcss-plugin-3.3.1.js' %}"></script>
     {% block extra_css %}{% endblock %}
 </head>
 <body>
     {% if messages %}
         {% for message in messages %}
             {% include 'djf_surveys/components/alert.html' %}
         {% endfor %}
     {% endif %}
-    {% include 'djf_surveys/components/header_nav.html' %}
     <div class="container mx-auto">
         {% block content %} {% endblock %}
     </div>
-    <script src="{% static 'djf_surveys/te-starter/js/tw-elements.umd.min.js' %}"></script>
+
     {% include 'djf_surveys/components/alert_js.html' %}
     {% block extra_js %}{% endblock %}
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,8 @@
-{% load static %}
+ {% load i18n static %}
 
  {% block extra_css %}{% endblock %}
 {% if messages %} {% for message in messages %} {% include 'djf_surveys/
-components/alert.html' %} {% endfor %} {% endif %} {% include 'djf_surveys/
-components/header_nav.html' %}
+components/alert.html' %} {% endfor %} {% endif %}
 {% block content %} {% endblock %}
- {% include 'djf_surveys/components/alert_js.html' %} {% block extra_js %}{%
+{% include 'djf_surveys/components/alert_js.html' %} {% block extra_js %}{%
 endblock %}
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/question_form.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/question_form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/summary.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/summary.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/admins/survey_list.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/admins/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/answer_list.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/answer_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/alert.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/alert.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_answer.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_answer.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/card_list_survey.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/card_list_survey.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/header_nav.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/header_nav.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete.html`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         class="flex flex-shrink-0 flex-wrap items-center justify-end rounded-b-md border-t-2 border-neutral-100 border-opacity-100 p-4 dark:border-opacity-50">
         <button
           type="button"
           class="inline-block px-6 py-2.5 bg-red-400 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-red-700 hover:shadow-lg focus:outline-none focus:ring-0 transition duration-150 ease-in-out"
           data-te-modal-dismiss
           data-te-ripple-init
           data-te-ripple-color="light">
-          {% trans "Cancel" %}
+          {% trans "Close" %}
         </button>
         <a
           id="confirmDeleteButton"
           class="inline-block px-6 py-2.5 bg-blue-500 text-white font-medium text-xs leading-tight uppercase rounded shadow-md hover:bg-blue-700 focus:bg-blue-700 focus:shadow-lg focus:outline-none focus:ring-0 active:bg-blue-800 transition duration-150 ease-in-out ml-1"
           data-te-ripple-init
           data-te-ripple-color="light">
           {% trans "Yes" %}
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/modal_delete_js.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/modal_delete_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/search_form.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/search_form.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+{% load i18n %}
 <div class="flex space-x-4 mb-5">
       <form class="">
         <div class="relative">
           <input
             class="h-10 pr-10 text-sm placeholder-gray-300 border-gray-200 rounded-lg focus:z-10"
-            placeholder="Search..."
+            placeholder="{% trans 'Search...' %}"
             type="text",
             name="q"
           />
 
           <button
             class="absolute inset-y-0 right-0 p-2 mr-px text-gray-600 rounded-r-lg"
             type="submit"
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/share_link_button_js.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/share_link_button_js.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/components/star_border.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/components/star_border.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/detail_result.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/detail_result.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/form.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/form.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/survey_list.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/survey_list.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/checkbox_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/radio_option.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/radio_option.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/templates/djf_surveys/widgets/star_rating.html` & `django-form-surveys-2.0.0/djf_surveys/templates/djf_surveys/widgets/star_rating.html`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/urls.py` & `django-form-surveys-2.0.0/djf_surveys/urls.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/djf_surveys/validators.py` & `django-form-surveys-2.0.0/djf_surveys/validators.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 
 def validate_rating(value):
     try:
         rating = int(value)
     except (TypeError, ValueError):
         raise ValidationError(
-            _('%(value)s is not a number.'),
-            params={'value': value},
+            _('%ss is not a number.' % value)
         )
 
     if rating > 5:
         raise ValidationError(
             _('Value cannot be greater than 5.')
         )
```

### Comparing `django-form-surveys-1.8.2/djf_surveys/views.py` & `django-form-surveys-2.0.0/djf_surveys/views.py`

 * *Files identical despite different names*

### Comparing `django-form-surveys-1.8.2/setup.py` & `django-form-surveys-2.0.0/setup.py`

 * *Files identical despite different names*

