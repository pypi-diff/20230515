# Comparing `tmp/djaodjin-survey-0.9.7.tar.gz` & `tmp/djaodjin-survey-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djaodjin-survey-0.9.7.tar", last modified: Fri May  5 18:13:48 2023, max compression
+gzip compressed data, was "djaodjin-survey-0.9.8.tar", last modified: Mon May 15 19:01:01 2023, max compression
```

## Comparing `djaodjin-survey-0.9.7.tar` & `djaodjin-survey-0.9.8.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.669855 djaodjin-survey-0.9.7/
--rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/LICENSE.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/MANIFEST.in
--rw-r--r--   0 smirolo    (501) staff       (20)     1932 2023-05-05 18:13:48.669922 djaodjin-survey-0.9.7/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     1173 2023-05-05 18:12:15.000000 djaodjin-survey-0.9.7/README.md
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.651610 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/
--rw-r--r--   0 smirolo    (501) staff       (20)     1932 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/PKG-INFO
--rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/SOURCES.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/dependency_links.txt
--rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/requires.txt
--rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-05-05 18:13:48.000000 djaodjin-survey-0.9.7/djaodjin_survey.egg-info/top_level.txt
--rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.7/pyproject.toml
--rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-05-05 18:13:48.670123 djaodjin-survey-0.9.7/setup.cfg
--rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.7/setup.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.655850 djaodjin-survey-0.9.7/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-05-05 18:11:51.000000 djaodjin-survey-0.9.7/survey/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/admin.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.659905 djaodjin-survey-0.9.7/survey/api/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.7/survey/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)    45858 2023-05-05 17:40:52.000000 djaodjin-survey-0.9.7/survey/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.7/survey/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)    26832 2023-05-05 17:25:00.000000 djaodjin-survey-0.9.7/survey/api/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    58251 2023-05-05 17:22:48.000000 djaodjin-survey-0.9.7/survey/api/sample.py
--rw-r--r--   0 smirolo    (501) staff       (20)    24572 2023-05-05 17:16:15.000000 djaodjin-survey-0.9.7/survey/api/serializers.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.7/survey/api/serializers_overrides.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.7/survey/api/units.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.7/survey/compat.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/docs.py
--rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.7/survey/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/forms.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.7/survey/helpers.py
--rw-r--r--   0 smirolo    (501) staff       (20)    14735 2023-05-04 19:49:21.000000 djaodjin-survey-0.9.7/survey/mixins.py
--rw-r--r--   0 smirolo    (501) staff       (20)    39897 2023-05-02 16:54:48.000000 djaodjin-survey-0.9.7/survey/models.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.7/survey/pagination.py
--rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.7/survey/queries.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.7/survey/settings.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.7/survey/signals.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.649420 djaodjin-survey-0.9.7/survey/static/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.660166 djaodjin-survey-0.9.7/survey/static/css/
--rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/css/matrix-chart.css
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.662171 djaodjin-survey-0.9.7/survey/static/js/
--rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-categorize.js
--rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-matrix.js
--rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-resources-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-set.js
--rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey-vue.js
--rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey.js
--rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/static/js/matrix-chart.js
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.649535 djaodjin-survey-0.9.7/survey/templates/
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.663943 djaodjin-survey-0.9.7/survey/templates/survey/
--rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/answer_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/campaign_form.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664077 djaodjin-survey-0.9.7/survey/templates/survey/campaigns/
--rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/campaigns/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/categorize.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664664 djaodjin-survey-0.9.7/survey/templates/survey/matrix/
--rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/compare.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/index.html
--rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/matrix/matrix.html
--rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/portfolios.html
--rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/question_form.html
--rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/question_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/respondent_list.html
--rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/result.html
--rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.7/survey/templates/survey/result_quizz.html
--rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/sample_create.html
--rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/sample_update.html
--rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templates/survey/send.html
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.664893 djaodjin-survey-0.9.7/survey/templatetags/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/templatetags/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.7/survey/templatetags/survey_tags.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.665095 djaodjin-survey-0.9.7/survey/urls/
--rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.7/survey/urls/__init__.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.666601 djaodjin-survey-0.9.7/survey/urls/api/
--rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.7/survey/urls/api/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.7/survey/urls/api/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.7/survey/urls/api/filters.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.7/survey/urls/api/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.7/survey/urls/api/metrics.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.7/survey/urls/api/noauth.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.7/survey/urls/api/portfolios.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.667163 djaodjin-survey-0.9.7/survey/urls/api/sample/
--rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/reset.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.7/survey/urls/api/sample/update.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.668301 djaodjin-survey-0.9.7/survey/urls/views/
--rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.7/survey/urls/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.7/survey/urls/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.7/survey/urls/views/matrices.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.7/survey/urls/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.7/survey/urls/views/samples.py
--rw-r--r--   0 smirolo    (501) staff       (20)     9471 2023-04-20 22:32:58.000000 djaodjin-survey-0.9.7/survey/utils.py
-drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-05 18:13:48.669602 djaodjin-survey-0.9.7/survey/views/
--rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/__init__.py
--rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.7/survey/views/campaigns.py
--rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/createquestion.py
--rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.7/survey/views/edit.py
--rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.7/survey/views/matrix.py
--rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.7/survey/views/portfolios.py
--rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.7/survey/views/sample.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.355826 djaodjin-survey-0.9.8/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1318 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/LICENSE.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       35 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/MANIFEST.in
+-rw-r--r--   0 smirolo    (501) staff       (20)     1855 2023-05-15 19:01:01.355911 djaodjin-survey-0.9.8/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     1096 2023-05-15 18:59:57.000000 djaodjin-survey-0.9.8/README.md
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.337917 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1855 2023-05-15 19:01:01.000000 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/PKG-INFO
+-rw-r--r--   0 smirolo    (501) staff       (20)     2399 2023-05-15 19:01:01.000000 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/SOURCES.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        1 2023-05-15 19:01:01.000000 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/dependency_links.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)       73 2023-05-15 19:01:01.000000 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/requires.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)        7 2023-05-15 19:01:01.000000 djaodjin-survey-0.9.8/djaodjin_survey.egg-info/top_level.txt
+-rw-r--r--   0 smirolo    (501) staff       (20)     1358 2023-04-18 19:54:04.000000 djaodjin-survey-0.9.8/pyproject.toml
+-rw-r--r--   0 smirolo    (501) staff       (20)       79 2023-05-15 19:01:01.356130 djaodjin-survey-0.9.8/setup.cfg
+-rw-r--r--   0 smirolo    (501) staff       (20)     1381 2023-04-18 16:17:24.000000 djaodjin-survey-0.9.8/setup.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.341437 djaodjin-survey-0.9.8/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1435 2023-05-15 18:56:32.000000 djaodjin-survey-0.9.8/survey/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1842 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/admin.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.344940 djaodjin-survey-0.9.8/survey/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     7333 2022-09-14 00:28:06.000000 djaodjin-survey-0.9.8/survey/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    45858 2023-05-05 17:40:52.000000 djaodjin-survey-0.9.8/survey/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    12575 2023-01-27 18:26:55.000000 djaodjin-survey-0.9.8/survey/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    26832 2023-05-05 17:25:00.000000 djaodjin-survey-0.9.8/survey/api/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    58251 2023-05-15 18:55:58.000000 djaodjin-survey-0.9.8/survey/api/sample.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    24572 2023-05-05 17:16:15.000000 djaodjin-survey-0.9.8/survey/api/serializers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2929 2023-03-10 17:42:57.000000 djaodjin-survey-0.9.8/survey/api/serializers_overrides.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5569 2023-04-13 17:06:50.000000 djaodjin-survey-0.9.8/survey/api/units.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4094 2022-09-26 17:15:24.000000 djaodjin-survey-0.9.8/survey/compat.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2316 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/docs.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    17450 2023-04-07 16:40:09.000000 djaodjin-survey-0.9.8/survey/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8639 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/forms.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6173 2023-04-05 16:25:51.000000 djaodjin-survey-0.9.8/survey/helpers.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    14735 2023-05-04 19:49:21.000000 djaodjin-survey-0.9.8/survey/mixins.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    39970 2023-05-15 18:53:49.000000 djaodjin-survey-0.9.8/survey/models.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4007 2023-04-05 18:59:23.000000 djaodjin-survey-0.9.8/survey/pagination.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    13064 2023-04-05 17:26:46.000000 djaodjin-survey-0.9.8/survey/queries.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4395 2023-03-21 20:59:50.000000 djaodjin-survey-0.9.8/survey/settings.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1955 2022-10-04 20:48:04.000000 djaodjin-survey-0.9.8/survey/signals.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.335682 djaodjin-survey-0.9.8/survey/static/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.345613 djaodjin-survey-0.9.8/survey/static/css/
+-rw-r--r--   0 smirolo    (501) staff       (20)      296 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/css/matrix-chart.css
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.347964 djaodjin-survey-0.9.8/survey/static/js/
+-rw-r--r--   0 smirolo    (501) staff       (20)    12547 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-categorize.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    15443 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-matrix.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    51604 2023-04-14 15:55:35.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-resources-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)     5462 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-set.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    17193 2023-04-14 16:37:55.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-survey-vue.js
+-rw-r--r--   0 smirolo    (501) staff       (20)      544 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/js/djaodjin-survey.js
+-rw-r--r--   0 smirolo    (501) staff       (20)    12995 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/static/js/matrix-chart.js
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.335799 djaodjin-survey-0.9.8/survey/templates/
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.349831 djaodjin-survey-0.9.8/survey/templates/survey/
+-rw-r--r--   0 smirolo    (501) staff       (20)      667 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/answer_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/campaign_form.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.349961 djaodjin-survey-0.9.8/survey/templates/survey/campaigns/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1184 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/campaigns/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2529 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/categorize.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.350436 djaodjin-survey-0.9.8/survey/templates/survey/matrix/
+-rw-r--r--   0 smirolo    (501) staff       (20)       62 2023-01-19 22:34:30.000000 djaodjin-survey-0.9.8/survey/templates/survey/matrix/compare.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2087 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/matrix/index.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     4088 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/matrix/matrix.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     9287 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/portfolios.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      249 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/question_form.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     1572 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/question_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      471 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/respondent_list.html
+-rw-r--r--   0 smirolo    (501) staff       (20)     2077 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/result.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      983 2023-03-10 17:29:52.000000 djaodjin-survey-0.9.8/survey/templates/survey/result_quizz.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      562 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/sample_create.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      356 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/sample_update.html
+-rw-r--r--   0 smirolo    (501) staff       (20)      245 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templates/survey/send.html
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.350658 djaodjin-survey-0.9.8/survey/templatetags/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/templatetags/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1769 2023-02-10 21:30:25.000000 djaodjin-survey-0.9.8/survey/templatetags/survey_tags.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.350872 djaodjin-survey-0.9.8/survey/urls/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1533 2022-09-25 23:08:10.000000 djaodjin-survey-0.9.8/survey/urls/__init__.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.352497 djaodjin-survey-0.9.8/survey/urls/api/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1718 2023-03-22 18:00:00.000000 djaodjin-survey-0.9.8/survey/urls/api/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1653 2022-09-26 00:12:56.000000 djaodjin-survey-0.9.8/survey/urls/api/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2772 2022-09-26 02:10:24.000000 djaodjin-survey-0.9.8/survey/urls/api/filters.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2125 2023-04-07 17:48:09.000000 djaodjin-survey-0.9.8/survey/urls/api/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1717 2022-09-26 00:13:35.000000 djaodjin-survey-0.9.8/survey/urls/api/metrics.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1622 2022-09-26 00:12:26.000000 djaodjin-survey-0.9.8/survey/urls/api/noauth.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2390 2023-03-07 21:45:05.000000 djaodjin-survey-0.9.8/survey/urls/api/portfolios.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.353095 djaodjin-survey-0.9.8/survey/urls/api/sample/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1512 2022-09-26 00:09:27.000000 djaodjin-survey-0.9.8/survey/urls/api/sample/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1722 2023-02-21 21:54:31.000000 djaodjin-survey-0.9.8/survey/urls/api/sample/reset.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2830 2023-04-07 17:59:33.000000 djaodjin-survey-0.9.8/survey/urls/api/sample/update.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.354184 djaodjin-survey-0.9.8/survey/urls/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)     1714 2023-03-22 18:07:23.000000 djaodjin-survey-0.9.8/survey/urls/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2942 2022-09-26 00:06:32.000000 djaodjin-survey-0.9.8/survey/urls/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2105 2023-01-19 22:50:22.000000 djaodjin-survey-0.9.8/survey/urls/views/matrices.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1894 2023-01-25 23:37:48.000000 djaodjin-survey-0.9.8/survey/urls/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     2180 2022-09-26 00:14:39.000000 djaodjin-survey-0.9.8/survey/urls/views/samples.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     9471 2023-04-20 22:32:58.000000 djaodjin-survey-0.9.8/survey/utils.py
+drwxr-xr-x   0 smirolo    (501) staff       (20)        0 2023-05-15 19:01:01.355581 djaodjin-survey-0.9.8/survey/views/
+-rw-r--r--   0 smirolo    (501) staff       (20)        0 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/views/__init__.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     8457 2023-03-21 21:02:40.000000 djaodjin-survey-0.9.8/survey/views/campaigns.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     5626 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/views/createquestion.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     1898 2022-07-26 19:09:35.000000 djaodjin-survey-0.9.8/survey/views/edit.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     6155 2023-04-07 17:48:37.000000 djaodjin-survey-0.9.8/survey/views/matrix.py
+-rw-r--r--   0 smirolo    (501) staff       (20)     4391 2023-03-21 21:10:13.000000 djaodjin-survey-0.9.8/survey/views/portfolios.py
+-rw-r--r--   0 smirolo    (501) staff       (20)    11685 2023-03-21 20:44:41.000000 djaodjin-survey-0.9.8/survey/views/sample.py
```

### Comparing `djaodjin-survey-0.9.7/LICENSE.txt` & `djaodjin-survey-0.9.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/PKG-INFO` & `djaodjin-survey-0.9.8/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.7
+Version: 0.9.8
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -47,16 +47,15 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.7
+0.9.8
 
-  * prevents extra data to leak through API under unexpected conditions
-  * uses prefix to filter questions in benchmarks API
+  * insures Portfolio.ends_at is not set to NULL
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.7/djaodjin_survey.egg-info/PKG-INFO` & `djaodjin-survey-0.9.8/djaodjin_survey.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djaodjin-survey
-Version: 0.9.7
+Version: 0.9.8
 Summary: Django app for qualitative and quantitative surveys
 Author-email: The DjaoDjin Team <help@djaodjin.com>
 Maintainer-email: The DjaoDjin Team <help@djaodjin.com>
 License: BSD-2-Clause
 Project-URL: repository, https://github.com/djaodjin/djaodjin-survey
 Project-URL: documentation, https://djaodjin-survey.readthedocs.io/
 Project-URL: changelog, https://github.com/djaodjin/djaodjin-survey/changelog
@@ -47,16 +47,15 @@
 
 Tested with
 
 - **Python:** 3.7, **Django:** 3.2 ([LTS](https://www.djangoproject.com/download/))
 - **Python:** 3.10, **Django:** 4.2 (latest)
 - **Python:** 2.7, **Django:** 1.11 (legacy) - use testsite/requirements-legacy.txt
 
-0.9.7
+0.9.8
 
-  * prevents extra data to leak through API under unexpected conditions
-  * uses prefix to filter questions in benchmarks API
+  * insures Portfolio.ends_at is not set to NULL
 
 [previous release notes](changelog)
 
 
 Models have been completely re-designed between version 0.1.7 and 0.2.0
```

### Comparing `djaodjin-survey-0.9.7/djaodjin_survey.egg-info/SOURCES.txt` & `djaodjin-survey-0.9.8/djaodjin_survey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/pyproject.toml` & `djaodjin-survey-0.9.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/setup.py` & `djaodjin-survey-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/__init__.py` & `djaodjin-survey-0.9.8/survey/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF
 # ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """
 PEP 386-compliant version number for the survey django app.
 """
 
-__version__ = '0.9.7'
+__version__ = '0.9.8'
```

### Comparing `djaodjin-survey-0.9.7/survey/admin.py` & `djaodjin-survey-0.9.8/survey/admin.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/campaigns.py` & `djaodjin-survey-0.9.8/survey/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/matrix.py` & `djaodjin-survey-0.9.8/survey/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/metrics.py` & `djaodjin-survey-0.9.8/survey/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/portfolios.py` & `djaodjin-survey-0.9.8/survey/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/sample.py` & `djaodjin-survey-0.9.8/survey/api/sample.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/serializers.py` & `djaodjin-survey-0.9.8/survey/api/serializers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/serializers_overrides.py` & `djaodjin-survey-0.9.8/survey/api/serializers_overrides.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/api/units.py` & `djaodjin-survey-0.9.8/survey/api/units.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/compat.py` & `djaodjin-survey-0.9.8/survey/compat.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/docs.py` & `djaodjin-survey-0.9.8/survey/docs.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/filters.py` & `djaodjin-survey-0.9.8/survey/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/forms.py` & `djaodjin-survey-0.9.8/survey/forms.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/helpers.py` & `djaodjin-survey-0.9.8/survey/helpers.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/mixins.py` & `djaodjin-survey-0.9.8/survey/mixins.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/models.py` & `djaodjin-survey-0.9.8/survey/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -957,20 +957,22 @@
     invoice_key = models.CharField(max_length=40, null=True)
 
     def __str__(self):
         return "<PortfolioDoubleOptIn(grantee='%s', account='%s', "\
             "campaign='%s', ends_at='%s')>" % (self.grantee_id,
             self.account_id, self.campaign_id, self.ends_at)
 
-    def create_portfolios(self):
+    def create_portfolios(self, at_time=None):
+        if not at_time:
+            at_time = datetime_or_now()
         with transaction.atomic():
             Portfolio.objects.update_or_create(
                 grantee=self.grantee, account=self.account,
                 campaign=self.campaign,
-                defaults={'ends_at': self.ends_at})
+                defaults={'ends_at': at_time})
 
     @staticmethod
     def generate_key(account):
         random_key = str(random.random()).encode('utf-8')
         salt = hashlib.sha1(random_key).hexdigest()[:5]
         verification_key = hashlib.sha1(
             (salt+str(account)).encode('utf-8')).hexdigest()
```

### Comparing `djaodjin-survey-0.9.7/survey/pagination.py` & `djaodjin-survey-0.9.8/survey/pagination.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/queries.py` & `djaodjin-survey-0.9.8/survey/queries.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/settings.py` & `djaodjin-survey-0.9.8/survey/settings.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/signals.py` & `djaodjin-survey-0.9.8/survey/signals.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-categorize.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-categorize.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-matrix.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-matrix.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-resources-vue.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-resources-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-set.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-set.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey-vue.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-survey-vue.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/djaodjin-survey.js` & `djaodjin-survey-0.9.8/survey/static/js/djaodjin-survey.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/static/js/matrix-chart.js` & `djaodjin-survey-0.9.8/survey/static/js/matrix-chart.js`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/answer_form.html` & `djaodjin-survey-0.9.8/survey/templates/survey/answer_form.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/campaigns/index.html` & `djaodjin-survey-0.9.8/survey/templates/survey/campaigns/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/categorize.html` & `djaodjin-survey-0.9.8/survey/templates/survey/categorize.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/matrix/index.html` & `djaodjin-survey-0.9.8/survey/templates/survey/matrix/index.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/matrix/matrix.html` & `djaodjin-survey-0.9.8/survey/templates/survey/matrix/matrix.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/portfolios.html` & `djaodjin-survey-0.9.8/survey/templates/survey/portfolios.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/question_list.html` & `djaodjin-survey-0.9.8/survey/templates/survey/question_list.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/result.html` & `djaodjin-survey-0.9.8/survey/templates/survey/result.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/result_quizz.html` & `djaodjin-survey-0.9.8/survey/templates/survey/result_quizz.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templates/survey/sample_create.html` & `djaodjin-survey-0.9.8/survey/templates/survey/sample_create.html`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/templatetags/survey_tags.py` & `djaodjin-survey-0.9.8/survey/templatetags/survey_tags.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/__init__.py` & `djaodjin-survey-0.9.8/survey/urls/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/__init__.py` & `djaodjin-survey-0.9.8/survey/urls/api/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/campaigns.py` & `djaodjin-survey-0.9.8/survey/urls/api/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/filters.py` & `djaodjin-survey-0.9.8/survey/urls/api/filters.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/matrix.py` & `djaodjin-survey-0.9.8/survey/urls/api/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/metrics.py` & `djaodjin-survey-0.9.8/survey/urls/api/metrics.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/noauth.py` & `djaodjin-survey-0.9.8/survey/urls/api/noauth.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/portfolios.py` & `djaodjin-survey-0.9.8/survey/urls/api/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/sample/__init__.py` & `djaodjin-survey-0.9.8/survey/urls/api/sample/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/sample/reset.py` & `djaodjin-survey-0.9.8/survey/urls/api/sample/reset.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/api/sample/update.py` & `djaodjin-survey-0.9.8/survey/urls/api/sample/update.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/views/__init__.py` & `djaodjin-survey-0.9.8/survey/urls/views/__init__.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/views/campaigns.py` & `djaodjin-survey-0.9.8/survey/urls/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/views/matrices.py` & `djaodjin-survey-0.9.8/survey/urls/views/matrices.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/views/portfolios.py` & `djaodjin-survey-0.9.8/survey/urls/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/urls/views/samples.py` & `djaodjin-survey-0.9.8/survey/urls/views/samples.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/utils.py` & `djaodjin-survey-0.9.8/survey/utils.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/campaigns.py` & `djaodjin-survey-0.9.8/survey/views/campaigns.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/createquestion.py` & `djaodjin-survey-0.9.8/survey/views/createquestion.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/edit.py` & `djaodjin-survey-0.9.8/survey/views/edit.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/matrix.py` & `djaodjin-survey-0.9.8/survey/views/matrix.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/portfolios.py` & `djaodjin-survey-0.9.8/survey/views/portfolios.py`

 * *Files identical despite different names*

### Comparing `djaodjin-survey-0.9.7/survey/views/sample.py` & `djaodjin-survey-0.9.8/survey/views/sample.py`

 * *Files identical despite different names*

