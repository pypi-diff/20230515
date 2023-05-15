# Comparing `tmp/aa_freight-1.8.0.tar.gz` & `tmp/aa_freight-1.9.0.tar.gz`

## Comparing `aa_freight-1.8.0.tar` & `aa_freight-1.9.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/__init__.py
--rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/admin.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/app_settings.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/apps.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/auth_hooks.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/constants.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/forms.py
--rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/helpers.py
--rw-r--r--   0        0        0    18034 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/managers.py
--rw-r--r--   0        0        0    48444 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/models.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/providers.py
--rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/swagger.json
--rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tasks.py
--rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/urls.py
--rw-r--r--   0        0        0    20324 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/views.py
--rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/django.pot
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/migrations/0001_squashed.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/migrations/0002_alter_contracthandler_last_error.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/migrations/__init__.py
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/css/calculator.css
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/css/contracts.css
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/css/kalkoken.css
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/css/statistics.css
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/js/contracts.js
--rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/static/freight/vendor/datatables/datetime.js
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/add_location.html
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/base.html
--rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/calculator.html
--rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/contracts_all.html
--rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/contracts_user.html
--rw-r--r--   0        0        0    14434 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/statistics.html
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/partials/contract_table.html
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/partials/contracts_js_includes.html
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/partials/contracts_legend.html
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/partials/global_js.html
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templates/freight/partials/menu.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templatetags/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/templatetags/freight_filters.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/__init__.py
--rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_admin.py
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_helpers.py
--rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_integration.py
--rw-r--r--   0        0        0    35000 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_managers.py
--rw-r--r--   0        0        0    60667 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_models.py
--rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_tasks.py
--rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_templatetags.py
--rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/test_views.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/__init__.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/characters.json
--rw-r--r--   0        0        0    13440 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/contracts.json
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/factories.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/factories_2.py
--rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/generate_contracts.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/generate_contracts_2.py
--rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/helpers.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_freight-1.8.0/freight/tests/testdata/universe_structures.json
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_freight-1.8.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_freight-1.8.0/LICENSE
--rw-r--r--   0        0        0    15772 2020-02-02 00:00:00.000000 aa_freight-1.8.0/README.md
--rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 aa_freight-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    16881 2020-02-02 00:00:00.000000 aa_freight-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/__init__.py
+-rw-r--r--   0        0        0     6954 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/admin.py
+-rw-r--r--   0        0        0     3123 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/app_settings.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/apps.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/auth_hooks.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/constants.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/forms.py
+-rw-r--r--   0        0        0     1369 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/helpers.py
+-rw-r--r--   0        0        0    18347 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/managers.py
+-rw-r--r--   0        0        0    48444 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/models.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/providers.py
+-rw-r--r--   0        0        0   887006 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/swagger.json
+-rw-r--r--   0        0        0     2364 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tasks.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/urls.py
+-rw-r--r--   0        0        0    20324 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/views.py
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/django.pot
+-rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8073 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8026 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8217 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8304 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     8066 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/migrations/0001_squashed.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/migrations/0002_alter_contracthandler_last_error.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/migrations/__init__.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/css/calculator.css
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/css/contracts.css
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/css/kalkoken.css
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/css/statistics.css
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/js/contracts.js
+-rw-r--r--   0        0        0     3250 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/static/freight/vendor/datatables/datetime.js
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/add_location.html
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/base.html
+-rw-r--r--   0        0        0    13875 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/calculator.html
+-rw-r--r--   0        0        0     2131 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/contracts_all.html
+-rw-r--r--   0        0        0     1577 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/contracts_user.html
+-rw-r--r--   0        0        0    14434 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/statistics.html
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/partials/contract_table.html
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/partials/contracts_js_includes.html
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/partials/contracts_legend.html
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/partials/global_js.html
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templates/freight/partials/menu.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templatetags/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/templatetags/freight_filters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/__init__.py
+-rw-r--r--   0        0        0     3138 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_admin.py
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_helpers.py
+-rw-r--r--   0        0        0     5514 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_integration.py
+-rw-r--r--   0        0        0    39345 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_managers.py
+-rw-r--r--   0        0        0    60667 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_models.py
+-rw-r--r--   0        0        0     4428 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_tasks.py
+-rw-r--r--   0        0        0      993 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_templatetags.py
+-rw-r--r--   0        0        0    20751 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/test_views.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/__init__.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/characters.json
+-rw-r--r--   0        0        0    13440 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/contracts.json
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/factories.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/factories_2.py
+-rw-r--r--   0        0        0     3213 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/generate_contracts.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/generate_contracts_2.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/helpers.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 aa_freight-1.9.0/freight/tests/testdata/universe_structures.json
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 aa_freight-1.9.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 aa_freight-1.9.0/LICENSE
+-rw-r--r--   0        0        0    16026 2020-02-02 00:00:00.000000 aa_freight-1.9.0/README.md
+-rw-r--r--   0        0        0     1774 2020-02-02 00:00:00.000000 aa_freight-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    17135 2020-02-02 00:00:00.000000 aa_freight-1.9.0/PKG-INFO
```

### Comparing `aa_freight-1.8.0/freight/admin.py` & `aa_freight-1.9.0/freight/admin.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/app_settings.py` & `aa_freight-1.9.0/freight/app_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 FREIGHT_APP_NAME = clean_setting("FREIGHT_APP_NAME", "Freight", required_type=str)
 
 # Sets the number minutes until a delayed sync will be recognized as error
 FREIGHT_CONTRACT_SYNC_GRACE_MINUTES = clean_setting(
     "FREIGHT_CONTRACT_SYNC_GRACE_MINUTES", 30
 )
 
-
 # Webhook URL used for notifications if defined
 FREIGHT_DISCORD_WEBHOOK_URL = clean_setting(
     "FREIGHT_DISCORD_WEBHOOK_URL", None, required_type=str
 )
 
 # Will be shown as "user name" instead of what is configured as app name
 # for notifications if defined
@@ -73,7 +72,10 @@
 )
 
 # whether to use Discord Proxy for sending DMs
 FREIGHT_DISCORDPROXY_ENABLED = clean_setting("FREIGHT_DISCORDPROXY_ENABLED", False)
 
 # Discordproxy port for GRPC
 FREIGHT_DISCORDPROXY_PORT = clean_setting("FREIGHT_DISCORDPROXY_PORT", 50051)
+
+# Send discord notifications about every contract, even if no pricing defined
+FREIGHT_NOTIFY_ALL_CONTRACTS = clean_setting("FREIGHT_NOTIFY_ALL_CONTRACTS", False)
```

### Comparing `aa_freight-1.8.0/freight/auth_hooks.py` & `aa_freight-1.9.0/freight/auth_hooks.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/forms.py` & `aa_freight-1.9.0/freight/forms.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/helpers.py` & `aa_freight-1.9.0/freight/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/managers.py` & `aa_freight-1.9.0/freight/managers.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from app_utils.logging import LoggerAddTag
 
 from . import __title__, constants
 from .app_settings import (
     FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL,
     FREIGHT_DISCORD_WEBHOOK_URL,
     FREIGHT_DISCORDPROXY_ENABLED,
+    FREIGHT_NOTIFY_ALL_CONTRACTS,
 )
 from .providers import esi
 
 logger = LoggerAddTag(get_extension_logger(__name__), __title__)
 
 
 class PricingManager(models.Manager):
@@ -393,28 +394,30 @@
         """Send notifications for outstanding contracts that have pricing"""
         from .models import Pricing
 
         if (
             self.count() > 0
             and Pricing.objects.exists()
             and not self.filter(pricing__isnull=False).exists()
+            and not FREIGHT_NOTIFY_ALL_CONTRACTS
         ):
             logger.info(
                 "There are no notifications to send, "
-                "because none of the existing contracts have a valid pricing."
+                "because none of the existing contracts have a valid pricing"
+                "and FREIGHT_NOTIFY_ALL_CONTRACTS option is set to False."
             )
             return
         self._sent_pilot_notifications(force_sent, rate_limited)
         self._sent_customer_notifications(force_sent, rate_limited)
 
     def _sent_pilot_notifications(self, force_sent: bool, rate_limited: bool) -> None:
         if FREIGHT_DISCORD_WEBHOOK_URL:
-            contracts_qs = self.filter(
-                status__exact=self.model.Status.OUTSTANDING
-            ).exclude(pricing__exact=None)
+            contracts_qs = self.filter(status__exact=self.model.Status.OUTSTANDING)
+            if not FREIGHT_NOTIFY_ALL_CONTRACTS:
+                contracts_qs = contracts_qs.exclude(pricing__exact=None)
             if not force_sent:
                 contracts_qs = contracts_qs.filter(date_notified__exact=None)
             contracts_qs = contracts_qs.select_related()
             if contracts_qs.count() > 0:
                 contracts_qs.sent_pilot_notifications(rate_limited)
             else:
                 logger.debug("No new pilot notifications.")
@@ -423,15 +426,17 @@
 
     def _sent_customer_notifications(
         self, force_sent: bool, rate_limited: bool
     ) -> None:
         if FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL or FREIGHT_DISCORDPROXY_ENABLED:
             contracts_qs = self.filter(
                 status__in=self.model.Status.for_customer_notification
-            ).exclude(pricing__exact=None)
+            )
+            if not FREIGHT_NOTIFY_ALL_CONTRACTS:
+                contracts_qs = contracts_qs.exclude(pricing__exact=None)
             contracts_qs = contracts_qs.select_related()
             if contracts_qs.count() > 0:
                 contracts_qs.sent_customer_notifications(
                     rate_limited=rate_limited, force_sent=force_sent
                 )
             else:
                 logger.debug("No new customer notifications.")
```

### Comparing `aa_freight-1.8.0/freight/models.py` & `aa_freight-1.9.0/freight/models.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/swagger.json` & `aa_freight-1.9.0/freight/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tasks.py` & `aa_freight-1.9.0/freight/tasks.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/urls.py` & `aa_freight-1.9.0/freight/urls.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/views.py` & `aa_freight-1.9.0/freight/views.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/django.pot` & `aa_freight-1.9.0/freight/locale/django.pot`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/de/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/en/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/es/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/fr_FR/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/it_IT/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/ja/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/ko_KR/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/ru/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/uk/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_freight-1.9.0/freight/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/migrations/0001_squashed.py` & `aa_freight-1.9.0/freight/migrations/0001_squashed.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/migrations/0002_alter_contracthandler_last_error.py` & `aa_freight-1.9.0/freight/migrations/0002_alter_contracthandler_last_error.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/static/freight/css/kalkoken.css` & `aa_freight-1.9.0/freight/static/freight/css/kalkoken.css`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/static/freight/css/statistics.css` & `aa_freight-1.9.0/freight/static/freight/css/statistics.css`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/static/freight/js/contracts.js` & `aa_freight-1.9.0/freight/static/freight/js/contracts.js`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/static/freight/vendor/datatables/datetime.js` & `aa_freight-1.9.0/freight/static/freight/vendor/datatables/datetime.js`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/add_location.html` & `aa_freight-1.9.0/freight/templates/freight/add_location.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/calculator.html` & `aa_freight-1.9.0/freight/templates/freight/calculator.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/contracts_all.html` & `aa_freight-1.9.0/freight/templates/freight/contracts_all.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/contracts_user.html` & `aa_freight-1.9.0/freight/templates/freight/contracts_user.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/statistics.html` & `aa_freight-1.9.0/freight/templates/freight/statistics.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/partials/contract_table.html` & `aa_freight-1.9.0/freight/templates/freight/partials/contract_table.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/partials/contracts_legend.html` & `aa_freight-1.9.0/freight/templates/freight/partials/contracts_legend.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/partials/global_js.html` & `aa_freight-1.9.0/freight/templates/freight/partials/global_js.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/templates/freight/partials/menu.html` & `aa_freight-1.9.0/freight/templates/freight/partials/menu.html`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_admin.py` & `aa_freight-1.9.0/freight/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_helpers.py` & `aa_freight-1.9.0/freight/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_integration.py` & `aa_freight-1.9.0/freight/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_managers.py` & `aa_freight-1.9.0/freight/tests/test_managers.py`

 * *Files 10% similar despite different names*

```diff
@@ -714,23 +714,59 @@
             create_pricing(
                 start_location=jita, end_location=amamake, price_base=500000000
             )
             Contract.objects.update_pricing()
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_send_pilot_notifications_normal(self, mock_webhook_execute):
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 8)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", True)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
+        def test_send_pilot_notifications_if_invalid_route_set_but_global_option_enabled(
+            self, mock_webhook_execute
+        ):
+            x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
+            Contract.objects.all().exclude(pk=x.pk).delete()
+            x.end_location_id = 60008494
+            x.save()
+            Contract.objects.update_pricing()
+            Contract.objects.send_notifications(rate_limited=False)
+            self.assertEqual(mock_webhook_execute.call_count, 1)
+
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
+        def test_send_pilot_notifications_if_invalid_route_set_and_global_option_disabled(
+            self, mock_webhook_execute
+        ):
+            x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
+            Contract.objects.all().exclude(pk=x.pk).delete()
+            x.end_location_id = 60008494
+            x.save()
+            Contract.objects.update_pricing()
+            Contract.objects.send_notifications(rate_limited=False)
+            self.assertEqual(mock_webhook_execute.call_count, 0)
+
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_dont_send_pilot_notifications_for_expired_contracts(
             self, mock_webhook_execute
         ):
             x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
@@ -738,14 +774,15 @@
             x.date_expired = now() - timedelta(hours=1)
             x.save()
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 0)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_send_pilot_notifications_only_once(self, mock_webhook_execute):
             x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
             Contract.objects.all().exclude(pk=x.pk).delete()
 
@@ -755,35 +792,38 @@
 
             # round #2
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 1)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_dont_send_any_notifications_when_no_url_if_set(
             self, mock_webhook_execute
         ):
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 0)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_send_customer_notifications_normal(self, mock_webhook_execute):
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 12)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_dont_send_customer_notifications_for_expired_contracts(
             self, mock_webhook_execute
         ):
             x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
@@ -791,14 +831,15 @@
             x.date_expired = now() - timedelta(hours=1)
             x.save()
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 0)
 
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", None)
         @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", "url")
         @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
         def test_send_customer_notifications_only_once_per_state(
             self, mock_webhook_execute
         ):
             x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
@@ -808,14 +849,48 @@
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 1)
 
             # round #2
             Contract.objects.send_notifications(rate_limited=False)
             self.assertEqual(mock_webhook_execute.call_count, 1)
 
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", True)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
+        def test_send_customer_notification_if_invalid_route_set_but_global_option_enabled(
+            self, mock_webhook_execute
+        ):
+            x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
+            Contract.objects.all().exclude(pk=x.pk).delete()
+            x.end_location_id = 60008494
+            x.save()
+            Contract.objects.update_pricing()
+            Contract.objects.send_notifications(rate_limited=False)
+            self.assertEqual(mock_webhook_execute.call_count, 1)
+
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MANAGERS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MANAGERS_PATH + ".FREIGHT_NOTIFY_ALL_CONTRACTS", False)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_WEBHOOK_URL", "url")
+        @patch(MODELS_PATH + ".FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL", None)
+        @patch(MODELS_PATH + ".FREIGHT_DISCORDPROXY_ENABLED", False)
+        def test_send_customer_notification_if_invalid_route_set_and_global_option_disabled(
+            self, mock_webhook_execute
+        ):
+            x = Contract.objects.filter(status=Contract.Status.OUTSTANDING).first()
+            Contract.objects.all().exclude(pk=x.pk).delete()
+            x.end_location_id = 60008494
+            x.save()
+            Contract.objects.update_pricing()
+            Contract.objects.send_notifications(rate_limited=False)
+            self.assertEqual(mock_webhook_execute.call_count, 0)
+
 
 class TestPricingManager(NoSocketsTestCase):
     @classmethod
     def setUpClass(cls):
         super().setUpClass()
         cls.jita, cls.amamake, cls.amarr = create_locations()
         cls.p1 = create_pricing(
```

### Comparing `aa_freight-1.8.0/freight/tests/test_models.py` & `aa_freight-1.9.0/freight/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_tasks.py` & `aa_freight-1.9.0/freight/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_templatetags.py` & `aa_freight-1.9.0/freight/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/test_views.py` & `aa_freight-1.9.0/freight/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/characters.json` & `aa_freight-1.9.0/freight/tests/testdata/characters.json`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/contracts.json` & `aa_freight-1.9.0/freight/tests/testdata/contracts.json`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/factories.py` & `aa_freight-1.9.0/freight/tests/testdata/factories.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/factories_2.py` & `aa_freight-1.9.0/freight/tests/testdata/factories_2.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/generate_contracts.py` & `aa_freight-1.9.0/freight/tests/testdata/generate_contracts.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/generate_contracts_2.py` & `aa_freight-1.9.0/freight/tests/testdata/generate_contracts_2.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/helpers.py` & `aa_freight-1.9.0/freight/tests/testdata/helpers.py`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/freight/tests/testdata/universe_structures.json` & `aa_freight-1.9.0/freight/tests/testdata/universe_structures.json`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/LICENSE` & `aa_freight-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/README.md` & `aa_freight-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 `FREIGHT_DISCORD_MENTIONS`| Optional mention string put in front of every notification to create pings: Typical values are: `@here` or `@everyone`. You can also mention roles, however you will need to add the role ID for that. The format is: `<@&role_id>` and you can get the role ID by entering `_<@role_name>` in a channel on Discord. See [this link](https://www.reddit.com/r/discordapp/comments/580qib/how_do_i_mention_a_role_with_webhooks/) for details. | `''`
 `FREIGHT_DISCORD_WEBHOOK_URL`| Webhook URL for the Discord channel where contract notifications for pilots should appear. | `None`
 `FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL`| Webhook URL for the Discord channel where contract notifications for customers should appear. | `None`
 `FREIGHT_FULL_ROUTE_NAMES`| Show full name of locations in route, e.g on calculator drop down  | `False`
 `FREIGHT_HOURS_UNTIL_STALE_STATUS`| Defines after how many hours the status of a contract is considered to be stale. Customer notifications will not be sent for a contract status that has become stale. This settings also prevents the app from sending out customer notifications for old contracts. | `24`
 `FREIGHT_OPERATION_MODE`| See section [Operation Mode](#operation-mode) for details.<br> Note that switching operation modes requires you to remove the existing contract handler with all its contracts and then setup a new contract handler | `'my_alliance'`
 `FREIGHT_STATISTICS_MAX_DAYS`| Sets the number of days that are considered for creating the statistics  | `90`
+`FREIGHT_NOTIFY_ALL_CONTRACTS`| Sends all contracts notifications, even if they do not have corresponding pricing | `False`
 
 ## Operation Mode
 
 The operation mode defines which contracts are processed by the Freight. For example you can define that only contracts assigned to your alliance are processed. Any courier contract that is  not in scope of the configured operation mode will be ignored by the freight app and e.g. not show up in the contract list or generate notifications.
 
 The following operation modes are available:
 
@@ -249,15 +250,15 @@
 Days to complete | Recommended days for contract completion | Info
 Details | Text with additional instructions for using this pricing | Info
 
 > **How to add new locations**:<br>If you are creating a pricing for a new route you may need to first add the locations (stations and/or structures).<br>The easiest way is to create a courier contract between those locations in game and then run contract sync. Those locations will then be added automatically.<br>Alternatively you can use the "Add Location" feature on the main page of the app. This will require you to provide the respective station or structure eve ID.
 
 ## Contract Check
 
-The app will automatically check if a newly issued contract complies with the pricing parameters for the respective route.
+The app will automatically check if a newly issued contract complies with the pricing parameters for the respective route. If you want to be notified about all contracts, even without correct pricing, set `FREIGHT_NOTIFY_ALL_CONTRACTS` option to `True`
 
 Compliant contracts will have a green checkmark (✓) in the "Contract Check" column on the contract list. Related notifications on Discord will be colored in green.
 
 Non-compliant contracts will have a red warning sign in the "Contract Check" column on the contract list. And related notifications on Discord will be colored in red. In addition the first customer notification will inform the customer about the issues and ask him to correct the issues.
 
 The following parameters will be checked (if they have been defined):
```

### Comparing `aa_freight-1.8.0/pyproject.toml` & `aa_freight-1.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aa_freight-1.8.0/PKG-INFO` & `aa_freight-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aa-freight
-Version: 1.8.0
+Version: 1.9.0
 Summary: Freight is an Alliance Auth app for running a freight service
 Project-URL: Homepage, https://gitlab.com/ErikKalkoken/aa-freight
 Author-email: Erik Kalkoken <kaloken87@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -214,14 +214,15 @@
 `FREIGHT_DISCORD_MENTIONS`| Optional mention string put in front of every notification to create pings: Typical values are: `@here` or `@everyone`. You can also mention roles, however you will need to add the role ID for that. The format is: `<@&role_id>` and you can get the role ID by entering `_<@role_name>` in a channel on Discord. See [this link](https://www.reddit.com/r/discordapp/comments/580qib/how_do_i_mention_a_role_with_webhooks/) for details. | `''`
 `FREIGHT_DISCORD_WEBHOOK_URL`| Webhook URL for the Discord channel where contract notifications for pilots should appear. | `None`
 `FREIGHT_DISCORD_CUSTOMERS_WEBHOOK_URL`| Webhook URL for the Discord channel where contract notifications for customers should appear. | `None`
 `FREIGHT_FULL_ROUTE_NAMES`| Show full name of locations in route, e.g on calculator drop down  | `False`
 `FREIGHT_HOURS_UNTIL_STALE_STATUS`| Defines after how many hours the status of a contract is considered to be stale. Customer notifications will not be sent for a contract status that has become stale. This settings also prevents the app from sending out customer notifications for old contracts. | `24`
 `FREIGHT_OPERATION_MODE`| See section [Operation Mode](#operation-mode) for details.<br> Note that switching operation modes requires you to remove the existing contract handler with all its contracts and then setup a new contract handler | `'my_alliance'`
 `FREIGHT_STATISTICS_MAX_DAYS`| Sets the number of days that are considered for creating the statistics  | `90`
+`FREIGHT_NOTIFY_ALL_CONTRACTS`| Sends all contracts notifications, even if they do not have corresponding pricing | `False`
 
 ## Operation Mode
 
 The operation mode defines which contracts are processed by the Freight. For example you can define that only contracts assigned to your alliance are processed. Any courier contract that is  not in scope of the configured operation mode will be ignored by the freight app and e.g. not show up in the contract list or generate notifications.
 
 The following operation modes are available:
 
@@ -277,15 +278,15 @@
 Days to complete | Recommended days for contract completion | Info
 Details | Text with additional instructions for using this pricing | Info
 
 > **How to add new locations**:<br>If you are creating a pricing for a new route you may need to first add the locations (stations and/or structures).<br>The easiest way is to create a courier contract between those locations in game and then run contract sync. Those locations will then be added automatically.<br>Alternatively you can use the "Add Location" feature on the main page of the app. This will require you to provide the respective station or structure eve ID.
 
 ## Contract Check
 
-The app will automatically check if a newly issued contract complies with the pricing parameters for the respective route.
+The app will automatically check if a newly issued contract complies with the pricing parameters for the respective route. If you want to be notified about all contracts, even without correct pricing, set `FREIGHT_NOTIFY_ALL_CONTRACTS` option to `True`
 
 Compliant contracts will have a green checkmark (✓) in the "Contract Check" column on the contract list. Related notifications on Discord will be colored in green.
 
 Non-compliant contracts will have a red warning sign in the "Contract Check" column on the contract list. And related notifications on Discord will be colored in red. In addition the first customer notification will inform the customer about the issues and ask him to correct the issues.
 
 The following parameters will be checked (if they have been defined):
```

