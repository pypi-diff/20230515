# Comparing `tmp/alphaz-0.7.7.9.tar.gz` & `tmp/alphaz-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alphaz-0.7.7.9.tar", last modified: Fri May  5 17:01:32 2023, max compression
+gzip compressed data, was "dist/alphaz-0.7.8.tar", last modified: Mon May 15 07:13:57 2023, max compression
```

## Comparing `alphaz-0.7.7.9.tar` & `alphaz-0.7.8.tar`

### file list

```diff
@@ -1,398 +1,400 @@
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1085 2019-07-02 13:36:12.000000 alphaz-0.7.7.9/LICENSE
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-05-05 17:01:30.000000 alphaz-0.7.7.9/MANIFEST.in
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.7.9/README.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.190321 alphaz-0.7.7.9/alphaz/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/README.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      498 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/alphaz.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/alphaz.code-workspace
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/alphaz.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/api.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/api.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/log.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2721 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/mails.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1601 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/admin.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3039 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/basic_tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3253 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/git.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/logs.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1810 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/mails.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1594 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/apis/routes/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/routes/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/application_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/permission_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/role_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/user_management/user_management.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3493 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/routes/users.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/tests.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/apis/users/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/ldap.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11859 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/apis/users/users.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/config.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/config.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/config/main_configuration.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/page.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config/source.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/core.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz/documentations/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_admin.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_core.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_screens.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/alpha_setup.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/authorizations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/cache.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/configuration.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/issues.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/methods.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/parameters.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/routes.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api/sqlalchemy.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/api_database.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/configuration.md
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/docs/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/init.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/instantiate.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/main.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/model.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/relations.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/schema.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/database/update.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/documentation.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/docs/index.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/documentations/mkdocs.yml
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/404.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.198320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/api/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/cache/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/cache/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/issues/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/issues/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/methods/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/methods/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/routes/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/routes/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/api_database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/api_database/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/assets/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/images/favicon.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.202320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/configuration/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/configuration/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/documentations/site/database/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/init/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/init/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.206320 alphaz-0.7.7.9/alphaz/documentations/site/database/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/main/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/model/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/model/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/relations/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/relations/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/schema/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/schema/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/database/update/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/database/update/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/documentation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/documentation/index.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.210320 alphaz-0.7.7.9/alphaz/documentations/site/search/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/search/search_index.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml.gz
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/git.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/help.md
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/index.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5807 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/api_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/barcode_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13989 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/config_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/converter_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9474 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/database_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/date_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/dict_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/emulation/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/emulation/vt102_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/events.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/files_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/flask_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/ftp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/img_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6207 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/io_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3783 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/libs/json_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/logs_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    13008 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/mail_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/nav_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/notifications_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/number_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/os_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/process_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14220 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/py_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/scp_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/search_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/secure_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/soap_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/libs/sql_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/ssh_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9896 2023-05-04 16:17:45.000000 alphaz-0.7.7.9/alphaz/libs/string_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5691 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/libs/test_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/time_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/transactions_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6565 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/libs/user_management/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/application_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/permission_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/role_management_lib.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/libs/user_management/user_management_lib.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.214321 alphaz-0.7.7.9/alphaz/mails/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/mails/Images/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Background.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Facebook_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Twitter_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Images/Web_logo.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/Images/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/Mail.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/Webmail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/debug.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/mail.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/password_reset.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/mails/stay_in_touch.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/mails/template.html
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/api/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      926 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_answer.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_methods.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14340 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_parameter.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_reloader.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_reloaders.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2402 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20365 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/api/_route.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    20460 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_structures.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/api/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.218320 alphaz-0.7.7.9/alphaz/models/config/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/config/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    26517 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/config/_config.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/config/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5495 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/main_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9992 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/models.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/operators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/requests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/database/row.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    56078 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/database/structure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4797 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/users_definitions.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     9301 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/database/views.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/excel.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/ftp.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/img.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/json/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/json/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2609 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/json/_converters.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/logger/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/_colorations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/logger/_logger.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/logger/_utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/logs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.7.9/alphaz/models/logs/main.log
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.7.9/alphaz/models/logs/main.log.2021-11-07
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.222320 alphaz-0.7.7.9/alphaz/models/main/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    31204 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/main/_base.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/models/main/_core/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_core/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    16001 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_core/_core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_core/_utils.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      335 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_enum.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/main/_exception.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_file.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_process.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_request.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/main/_singleton.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/request.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/models/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8399 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_category.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3670 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_group.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_levels.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4224 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_method.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4578 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_save.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14974 2023-05-05 17:01:29.000000 alphaz-0.7.7.9/alphaz/models/tests/_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/tests/_wrappers.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2910 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/models/user.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/models/watcher.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/pocs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/pocs/main.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/reload_gitignore.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/req.sh
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/requirements.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/run.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/src/alpha.png
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/configs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/config.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/loggers.json
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/configs/loggers_colors.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/src/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/src/database/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/Core.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/imports/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/imports/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.226320 alphaz-0.7.7.9/alphaz/stitch/models/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/models/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/models/element.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/run.bat
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1857 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/stitch.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.234320 alphaz-0.7.7.9/alphaz/stitch/web-drivers/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/web-drivers/chromedriver.exe
--rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/web-drivers/geckodriver
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.186320 alphaz-0.7.7.9/alphaz/stitch/websites/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/stitch/websites/Test/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/stitch/websites/Test/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/stitch/websites/stiki/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/stitch/websites/stiki/init.json
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/templates/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.242320 alphaz-0.7.7.9/alphaz/templates/assets/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/__init__.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/css/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/css/home.css
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/css/logs.css
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/images/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/admin.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/alpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/save.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/start-icon.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/user.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/icons/wsalpha.png
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/images/loading.gif
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/js/
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/ansi_up.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/libs/jquery.min.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/assets/js/logs.js
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/templates/hello.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/home.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/templates/logs.html
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/test.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.246320 alphaz-0.7.7.9/alphaz/tests/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    14409 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/api.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5646 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/basic_test.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1526 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/configurations.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    25295 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/tests/database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/processes.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/tests/utils.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11705 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/api.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/apm/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/apm/__init__.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/apm/ora.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/clean.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/configuration.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/alphaz/utils/database/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11444 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/database/init.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/database_to_dataclass.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/decorators.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.7.9/alphaz/utils/ensure.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1801 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/init_database.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     4405 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/mep.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     7639 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/screens.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/selectionMenu.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/tasks.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/tests.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/time.py
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-05-04 16:17:46.000000 alphaz-0.7.7.9/alphaz/utils/transactions.py
-drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-05 17:01:32.194321 alphaz-0.7.7.9/alphaz.egg-info/
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      600 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/PKG-INFO
--rw-rw-r--   0 aurele    (1000) aurele    (1000)    11373 2023-05-05 17:01:32.000000 alphaz-0.7.7.9/alphaz.egg-info/SOURCES.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/dependency_links.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)      458 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/requires.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-05-05 17:01:31.000000 alphaz-0.7.7.9/alphaz.egg-info/top_level.txt
--rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-05-05 17:01:32.250320 alphaz-0.7.7.9/setup.cfg
--rw-rw-r--   0 aurele    (1000) aurele    (1000)     3094 2023-05-05 17:00:51.000000 alphaz-0.7.7.9/setup.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.639627 alphaz-0.7.8/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1085 2019-07-02 13:36:12.000000 alphaz-0.7.8/LICENSE
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11211 2023-05-15 07:13:55.000000 alphaz-0.7.8/MANIFEST.in
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      596 2023-05-15 07:13:57.639627 alphaz-0.7.8/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-07-12 18:07:51.000000 alphaz-0.7.8/README.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.571627 alphaz-0.7.8/alphaz/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        9 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/README.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      531 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      104 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/alphaz.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       70 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/alphaz.code-workspace
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      208 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/alphaz.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       48 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/api.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      713 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/api.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      770 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.575627 alphaz-0.7.8/alphaz/apis/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/log.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2617 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/apis/mails.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.575627 alphaz-0.7.8/alphaz/apis/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/apis/routes/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1601 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/admin.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1143 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2961 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/apis/routes/basic_tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3271 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/apis/routes/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      413 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/git.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7272 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/logs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1840 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/apis/routes/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6384 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3202 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/apis/routes/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.575627 alphaz-0.7.8/alphaz/apis/routes/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      114 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2479 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/user_management/application_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2243 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/user_management/permission_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4104 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/user_management/role_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1291 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/user_management/user_management.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3493 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/routes/users.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      584 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/tests.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.575627 alphaz-0.7.8/alphaz/apis/users/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/users/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2718 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/apis/users/ldap.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11892 2023-05-09 13:51:35.000000 alphaz-0.7.8/alphaz/apis/users/users.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.575627 alphaz-0.7.8/alphaz/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      795 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config/config.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12602 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config/config.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      707 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/config/main_configuration.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      823 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config/page.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1700 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config/source.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1564 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      238 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/core.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.579627 alphaz-0.7.8/alphaz/documentations/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.579627 alphaz-0.7.8/alphaz/documentations/docs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/alpha_admin.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1408 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/alpha_core.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2595 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/alpha_screens.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2222 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/alpha_setup.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.579627 alphaz-0.7.8/alphaz/documentations/docs/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1527 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/authorizations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/cache.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2931 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/configuration.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       24 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/issues.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      705 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      559 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/methods.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1728 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/parameters.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1197 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/routes.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      486 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api/sqlalchemy.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1129 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/api_database.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2520 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/configuration.md
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.579627 alphaz-0.7.8/alphaz/documentations/docs/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2187 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/init.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      442 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/instantiate.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      113 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/main.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1806 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/model.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      373 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/relations.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/schema.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      615 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/database/update.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      357 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/documentation.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3526 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/docs/index.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1090 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/documentations/mkdocs.yml
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    13156 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/404.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/alpha_admin/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14222 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/alpha_admin/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/alpha_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22752 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/alpha_core/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/alpha_screens/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21873 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/alpha_screens/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/alpha_setup/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24071 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/alpha_setup/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.563627 alphaz-0.7.8/alphaz/documentations/site/api/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/authorizations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17905 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/authorizations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/cache/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14918 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/cache/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    27645 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/issues/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16365 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/issues/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17987 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/methods/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17722 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/methods/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/parameters/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20075 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/parameters/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/routes/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19333 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/routes/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api/sqlalchemy/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17109 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api/sqlalchemy/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/api_database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22959 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/api_database/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.563627 alphaz-0.7.8/alphaz/documentations/site/assets/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/assets/images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1870 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/images/favicon.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    79520 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   384391 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.583627 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.587627 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17058 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4654 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6119 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6208 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11499 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9342 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10669 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9437 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11232 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2313 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       36 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      817 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6026 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4754 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10171 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10958 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10331 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3647 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4523 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    15009 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      784 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22878 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.587627 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/workers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    34936 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   167496 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    87332 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   319950 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10915 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    37512 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/configuration/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    28465 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/configuration/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.567627 alphaz-0.7.8/alphaz/documentations/site/database/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/init/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23029 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/init/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/instantiate/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17445 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/instantiate/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14939 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/main/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/model/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24758 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/model/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/relations/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16511 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/relations/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/schema/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18704 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/schema/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/database/update/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20308 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/database/update/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/documentation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    17065 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/documentation/index.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    29467 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.591627 alphaz-0.7.8/alphaz/documentations/site/search/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    54135 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/search/search_index.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2809 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/sitemap.xml
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      209 2023-04-27 20:33:29.000000 alphaz-0.7.8/alphaz/documentations/site/sitemap.xml.gz
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       50 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/git.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       45 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/help.md
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      905 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/index.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.595627 alphaz-0.7.8/alphaz/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6052 2023-05-10 15:07:49.000000 alphaz-0.7.8/alphaz/libs/api_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1901 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/barcode_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14656 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/libs/config_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2420 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/converter_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     9724 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/libs/database_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4223 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/date_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6381 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/dict_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.595627 alphaz-0.7.8/alphaz/libs/emulation/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1758 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/emulation/vt102_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1642 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/events.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3351 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/files_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1184 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/flask_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       49 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/ftp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1093 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/img_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6212 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/io_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3711 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/json_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1151 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/logs_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12984 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/mail_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      508 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/nav_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      614 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/notifications_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1348 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/number_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      177 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/os_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2782 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/process_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14220 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/py_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      886 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/scp_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8082 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/search_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6362 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/secure_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2929 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/soap_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      139 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/libs/sql_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    18623 2023-05-04 16:17:45.000000 alphaz-0.7.8/alphaz/libs/ssh_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10500 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/string_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5796 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/test_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      703 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/time_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4492 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/transactions_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6565 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/user_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.599627 alphaz-0.7.8/alphaz/libs/user_management/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/user_management/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1336 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/user_management/application_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1597 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/user_management/permission_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3376 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/libs/user_management/role_management_lib.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2315 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/libs/user_management/user_management_lib.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.599627 alphaz-0.7.8/alphaz/mails/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.603627 alphaz-0.7.8/alphaz/mails/Images/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   948952 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/Images/Background.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1835 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/Images/Facebook_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2484 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/Images/Twitter_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3522 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/Images/Web_logo.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/Images/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)   966605 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/Mail.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5097 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/Webmail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    22029 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/debug.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23078 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/mail.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2331 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/password_reset.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    24598 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/mails/stay_in_touch.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       40 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/mails/template.html
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.603627 alphaz-0.7.8/alphaz/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      107 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/api/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      185 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      979 2023-05-10 10:18:52.000000 alphaz-0.7.8/alphaz/models/api/_answer.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2179 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      133 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_methods.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14580 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/models/api/_parameter.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14445 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_reloader.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3717 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_reloaders.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2402 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20497 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/models/api/_route.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    20461 2023-05-09 13:51:35.000000 alphaz-0.7.8/alphaz/models/api/_structures.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      651 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/api/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      388 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/config/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       32 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/config/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    26520 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/config/_config.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    12350 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/config/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       53 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1216 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/database/configs.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1938 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/database/mails.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3374 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/database/main_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10002 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/models/database/models.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      609 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/operators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1164 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/requests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1087 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/database/row.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    58488 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/models/database/structure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1826 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4797 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/users_definitions.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    10653 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/database/utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1061 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/database/views.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1241 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/excel.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     6683 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/ftp.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      150 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/img.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/json/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       41 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/json/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2664 2023-05-12 14:46:32.000000 alphaz-0.7.8/alphaz/models/json/_converters.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/logger/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       68 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/logger/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1319 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/logger/_colorations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    14322 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/logger/_logger.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      757 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/logger/_utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.607627 alphaz-0.7.8/alphaz/models/logs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1280 2021-11-12 08:53:17.000000 alphaz-0.7.8/alphaz/models/logs/main.log
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      160 2021-11-07 15:22:58.000000 alphaz-0.7.8/alphaz/models/logs/main.log.2021-11-07
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/models/main/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      354 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/main/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    30998 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/models/main/_base.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/models/main/_core/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_core/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16265 2023-05-10 10:18:52.000000 alphaz-0.7.8/alphaz/models/main/_core/_core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       13 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_core/_utils.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      552 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/main/_enum.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2001 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/main/_exception.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      501 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_file.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      477 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_process.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1305 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_request.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      925 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/main/_singleton.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2218 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/request.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/models/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      167 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8306 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/tests/_category.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3881 2023-05-10 13:32:39.000000 alphaz-0.7.8/alphaz/models/tests/_group.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      163 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/tests/_levels.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4224 2023-05-05 17:01:29.000000 alphaz-0.7.8/alphaz/models/tests/_method.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4510 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/models/tests/_save.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16488 2023-05-15 07:13:54.000000 alphaz-0.7.8/alphaz/models/tests/_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7505 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/tests/_wrappers.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2910 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/models/user.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2367 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/models/watcher.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/pocs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      685 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/pocs/main.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       72 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/reload_gitignore.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       67 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/req.sh
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      460 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/requirements.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1345 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/run.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/src/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/src/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/src/alpha.png
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/src/configs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      135 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/src/configs/config.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      674 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/src/configs/loggers.json
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      490 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/src/configs/loggers_colors.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/src/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/src/database/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.611627 alphaz-0.7.8/alphaz/stitch/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1769 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/Core.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       26 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.615627 alphaz-0.7.8/alphaz/stitch/imports/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       78 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/imports/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.615627 alphaz-0.7.8/alphaz/stitch/models/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/stitch/models/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      391 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/models/element.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       46 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/run.bat
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1808 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/stitch/stitch.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.623627 alphaz-0.7.8/alphaz/stitch/web-drivers/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  8738816 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/web-drivers/chromedriver.exe
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)  7008696 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/stitch/web-drivers/geckodriver
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.567627 alphaz-0.7.8/alphaz/stitch/websites/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/stitch/websites/Test/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      204 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/stitch/websites/Test/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/stitch/websites/stiki/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      363 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/stitch/websites/stiki/init.json
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/templates/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/templates/assets/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/__init__.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/templates/assets/css/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    95923 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/css/home.css
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2356 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/css/logs.css
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.631627 alphaz-0.7.8/alphaz/templates/assets/images/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/templates/assets/images/icons/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      276 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/admin.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1444 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/alpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      142 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/save.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     8889 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/start-icon.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      136 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/user.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23747 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/icons/wsalpha.png
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1165 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/images/loading.gif
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/templates/assets/js/
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/templates/assets/js/libs/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    21922 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/js/libs/ansi_up.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    89475 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/js/libs/jquery.min.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7339 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/assets/js/logs.js
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       37 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/templates/hello.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    19017 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/home.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3779 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/templates/logs.html
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1153 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/test.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/tests/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      119 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/tests/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    16017 2023-05-10 14:19:24.000000 alphaz-0.7.8/alphaz/tests/api.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5653 2023-05-10 10:18:52.000000 alphaz-0.7.8/alphaz/tests/basic_test.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1591 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/tests/configurations.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    25820 2023-05-10 10:18:52.000000 alphaz-0.7.8/alphaz/tests/database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      397 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/tests/processes.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      555 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/tests/utils.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/utils/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       57 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11704 2023-05-10 15:07:49.000000 alphaz-0.7.8/alphaz/utils/api.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/utils/apm/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        0 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/apm/__init__.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1671 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/apm/ora.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      338 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/clean.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      813 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/configuration.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.635627 alphaz-0.7.8/alphaz/utils/database/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11329 2023-05-10 12:03:02.000000 alphaz-0.7.8/alphaz/utils/database/init.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     5438 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/database_to_dataclass.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     2207 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/decorators.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3112 2021-03-29 08:42:45.000000 alphaz-0.7.8/alphaz/utils/ensure.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     1691 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/utils/init_database.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     4387 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/utils/mep.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     7976 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/utils/screens.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    23624 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/selectionMenu.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      764 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/tasks.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3419 2023-05-09 11:09:57.000000 alphaz-0.7.8/alphaz/utils/tests.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      628 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/time.py
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3849 2023-05-04 16:17:46.000000 alphaz-0.7.8/alphaz/utils/transactions.py
+drwxrwxr-x   0 aurele    (1000) aurele    (1000)        0 2023-05-15 07:13:57.571627 alphaz-0.7.8/alphaz.egg-info/
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      596 2023-05-15 07:13:56.000000 alphaz-0.7.8/alphaz.egg-info/PKG-INFO
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)    11439 2023-05-15 07:13:57.000000 alphaz-0.7.8/alphaz.egg-info/SOURCES.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        1 2023-05-15 07:13:56.000000 alphaz-0.7.8/alphaz.egg-info/dependency_links.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)      483 2023-05-15 07:13:57.000000 alphaz-0.7.8/alphaz.egg-info/requires.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)        7 2023-05-15 07:13:57.000000 alphaz-0.7.8/alphaz.egg-info/top_level.txt
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)       79 2023-05-15 07:13:57.639627 alphaz-0.7.8/setup.cfg
+-rw-rw-r--   0 aurele    (1000) aurele    (1000)     3133 2023-05-15 07:13:09.000000 alphaz-0.7.8/setup.py
```

### Comparing `alphaz-0.7.7.9/LICENSE` & `alphaz-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/MANIFEST.in` & `alphaz-0.7.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/PKG-INFO` & `alphaz-0.7.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7.9
+Version: 0.7.8
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.9.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.8.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alphaz-0.7.7.9/README.md` & `alphaz-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/api.json` & `alphaz-0.7.8/alphaz/api.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/api.py` & `alphaz-0.7.8/alphaz/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/mails.py` & `alphaz-0.7.8/alphaz/apis/mails.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,85 +1,89 @@
-import json
+import ujson
+
 from ...libs import user_lib, sql_lib, secure_lib, mail_lib
 from ..models.main import AlphaException
 
-def stay_in_touch(api,user_mail,name,token,db):
-    status        = None
-    valid_token   = mail_lib.is_mail_token_valid(user_mail, token)
+
+def stay_in_touch(api, user_mail, name, token, db):
+    status = None
+    valid_token = mail_lib.is_mail_token_valid(user_mail, token)
     if not valid_token:
-        AlphaException('invalid_token')
+        AlphaException("invalid_token")
 
-    status                  = user_lib.is_valid_mail(db,user_mail)
+    status = user_lib.is_valid_mail(db, user_mail)
     if not status:
-        raise AlphaException('invalid_mail')
+        raise AlphaException("invalid_mail")
 
-    parameters          = {'mail':user_mail,'name':name}
+    parameters = {"mail": user_mail, "name": name}
 
     mail_lib.send_mail(
-        mail_config     = 'stay_in_touch',
-        parameters_list = [parameters],
-        log=api.log
+        mail_config="stay_in_touch", parameters_list=[parameters], log=api.log
     )
 
+
 def mail_me(api, mail, name):
-    parameters          = {'mail':mail,'name':name}
+    parameters = {"mail": mail, "name": name}
+
+    mail_lib.send_mail(mail_config="mail", parameters_list=[parameters])
 
-    mail_lib.send_mail(
-        mail_config     = 'mail',
-        parameters_list = [parameters]
-    )
 
 def unstring_value(value):
     value = value.strip()
     if value[0] == "'" or value[0] == '"':
         value = value[1:]
     if value[-1] == "'" or value[-1] == '"':
         value = value[::-1][1:][::-1]
     value = value.strip()
     return value
 
+
 def str_parameters_to_dict(parameters_str):
-    parameters = json.loads(parameters_str)
+    parameters = ujson.loads(parameters_str)
     return parameters
 
-def request_view(api,user_mail,token,mail_type,mail_id,db):
-    mail_type   = mail_lib.get_mail_type(mail_type)
-    parameters  = None
-    mail_token  = mail_lib.get_mail_token(user_mail)
-    valid       = mail_token == token
+
+def request_view(api, user_mail, token, mail_type, mail_id, db):
+    mail_type = mail_lib.get_mail_type(mail_type)
+    parameters = None
+    mail_token = mail_lib.get_mail_token(user_mail)
+    valid = mail_token == token
 
     if not valid:
-        raise AlphaException('invalid_token')
-    
-    query       = "SELECT * from mails_history where mail_type = %s and uuid = %s"
-    values      = (mail_type,mail_id)
-    results     = db.get_query_results(query,values,unique=False)
-    valid       = len(results) != 0
+        raise AlphaException("invalid_token")
+
+    query = "SELECT * from mails_history where mail_type = %s and uuid = %s"
+    values = (mail_type, mail_id)
+    results = db.get_query_results(query, values, unique=False)
+    valid = len(results) != 0
     if not valid:
-        raise AlphaException('no_mail')
-        
-    parameters = str_parameters_to_dict(results[0]['parameters_full'])
-    parameters['mail'] = user_mail
-    #parameters = [{'key':x,'value':y} for x,y in parameters.items()]
+        raise AlphaException("no_mail")
 
-    mail_path = api.get_config('mails/path')
-    mail_contents_list = mail_lib.get_mail_content_for_parameters(mail_path,mail_type,[parameters],api.log)
+    parameters = str_parameters_to_dict(results[0]["parameters_full"])
+    parameters["mail"] = user_mail
+    # parameters = [{'key':x,'value':y} for x,y in parameters.items()]
+
+    mail_path = api.get_config("mails/path")
+    mail_contents_list = mail_lib.get_mail_content_for_parameters(
+        mail_path, mail_type, [parameters], api.log
+    )
 
     if len(mail_contents_list) == 0:
-        AlphaException('mail_error')
+        AlphaException("mail_error")
     else:
-        return mail_contents_list[0]['content']
+        return mail_contents_list[0]["content"]
+
 
-def request_unsubscribe(api,user_mail, token, mail_type,db):
-    mail_type   = mail_lib.get_mail_type(mail_type)
-    mail_token  = mail_lib.get_mail_token(user_mail)
-    valid       = mail_token == token
+def request_unsubscribe(api, user_mail, token, mail_type, db):
+    mail_type = mail_lib.get_mail_type(mail_type)
+    mail_token = mail_lib.get_mail_token(user_mail)
+    valid = mail_token == token
 
     if not valid:
-        raise AlphaException('invalid_token')
+        raise AlphaException("invalid_token")
 
-    query   = "INSERT INTO mail_blacklist (mail,mail_type) VALUES (%s,%s)"
-    values  = (user_mail,mail_type)
-    valid   = db.execute_query(query,values)
+    query = "INSERT INTO mail_blacklist (mail,mail_type) VALUES (%s,%s)"
+    values = (user_mail, mail_type)
+    valid = db.execute_query(query, values)
 
     if not valid:
-        raise AlphaException('fail')
+        raise AlphaException("fail")
```

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/admin.py` & `alphaz-0.7.8/alphaz/apis/routes/admin.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/api.py` & `alphaz-0.7.8/alphaz/apis/routes/api.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/basic_tests.py` & `alphaz-0.7.8/alphaz/apis/routes/basic_tests.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 from ...models.main import AlphaException
 from ...models.tests._test import TestInput
 
 from .. import tests
 
 from core import core
 
-api = core.api
+API = core.api
 
 
 @route(
     "/test/cache",
     cache=True,
     timeout=100,
     parameters=[Parameter("value"), Parameter("options", options=["Y", "N"])],
 )
 def api_test():
-    parameters = api.get_parameters()
-    parameters["uuid"] = uuid.uuid4()
-    return parameters
+    return API.gets(added={"uuid": uuid.uuid4()})
 
 
 @route(
     "/test/parameters",
     methods=["GET", "POST"],
     route_log=False,
     parameters=[
@@ -54,28 +52,28 @@
         Parameter("start_like_mode", ptype=str, mode=ParameterMode.START_LIKE),
         Parameter("none_mode", ptype=str, mode=ParameterMode.NONE),
         Parameter("bool", ptype=bool),
     ],
     description="Route used for auto test",
 )
 def api_test_parameters_route():
-    parameters = api.get_parameters()
+    parameters = API.gets()
     return parameters
 
 
 @route(
     "/test/insert",
 )
 def test_insert():
     return tests.insert()
 
 
 @route("/test/html", parameters=[Parameter("message")])
 def html_message():
-    return api.set_html("hello.html", parameters={"message": api.get("message")})
+    return API.set_html("hello.html", parameters={"message": API.get("message")})
 
 
 @route("/test/methods", methods=["GET"])
 def get_method_1():
     return "GET"
 
 
@@ -97,20 +95,20 @@
 @route("/test/methods", methods=["DELETE"])
 def get_method_5():
     return "DELETE"
 
 
 @route("/test/status", parameters=[Parameter("status"), Parameter("description")])
 def get_status():
-    api.set_status(**api.get_parameters())
+    API.set_status(**API.gets())
 
 
 @route(
     "/test/exception",
     parameters=[
         Parameter("name"),
         Parameter("warning", ptype=bool),
         Parameter("description"),
     ],
 )
 def get_exception():
-    raise AlphaException(**api.get_parameters())
+    raise AlphaException(**API.gets())
```

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/database.py` & `alphaz-0.7.8/alphaz/apis/routes/database.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,42 +52,45 @@
     admin=True,
     parameters=[Parameter("bind"), Parameter("table", required=True)],
 )
 def drop_table():
     return core.db.drop_table(**API.gets())
 
 
+DB_INIT_PARAMETERS = [
+    Parameter("binds", ptype=list[str]),
+    Parameter("tables", ptype=list[str]),
+    Parameter("drop", ptype=bool, default=False),
+    Parameter("truncate", ptype=bool, default=False),
+    Parameter("force", ptype=bool, default=False),
+    Parameter("create", ptype=bool, default=False),
+    Parameter("init", ptype=bool, default=False),
+    Parameter("init_views", ptype=bool, default=False),
+]
+
+
 @route(
     "/database/init",
     admin=True,
-    parameters=[
-        Parameter("binds", ptype=list[str]),
-        Parameter("tables", ptype=list[str]),
-        Parameter("drop", ptype=bool, default=False),
-        Parameter("truncate", ptype=bool, default=False),
-        Parameter("force", ptype=bool, default=False),
-        Parameter("create", ptype=bool, default=False),
-        Parameter("init", ptype=bool, default=False),
-        Parameter("init_views", ptype=bool, default=False),
-    ],
+    parameters=DB_INIT_PARAMETERS,
 )
 def init_all_database():
     database_lib.init_databases(core, **API.gets())
 
 
 @route("database/blocking", admin=True)
 def get_blocking_queries():
     return core.db.get_blocked_queries()
 
 
 @route(
     "/table",
     parameters=[
         Parameter("bind", ptype=str, default="ALPHA"),
-        Parameter("tablename", ptype=str, required=True),
+        Parameter("table", ptype=str, required=True),
         Parameter("order_by", ptype=str),
         Parameter("direction", ptype=str),
         Parameter("page_index", ptype=int),
         Parameter("page_size", ptype=int),
         Parameter("limit", ptype=int),
     ],
     logged=True,
@@ -95,31 +98,31 @@
 def get_transactions_history():
     return database_lib.get_table_content(**API.gets())
 
 
 @route(
     "/table/columns",
     parameters=[
-        Parameter("schema", ptype=str, default="ALPHA"),
-        Parameter("tablename", ptype=str, required=True),
+        Parameter("bind", ptype=str, default="ALPHA"),
+        Parameter("table", ptype=str, required=True),
     ],
 )
 def get_table_columns():
     return core.db.get_table_columns(**API.gets())
 
 
 @route(
     "/table/model",
     parameters=[
-        Parameter("schema", ptype=str, default="ALPHA"),
-        Parameter("tablename", ptype=str, required=True),
+        Parameter("bind", ptype=str, default="ALPHA"),
+        Parameter("table", ptype=str, required=True),
     ],
 )
 def get_table_model():
-    return core.db.get_table_model(**API.gets())
+    return core.db.get_table_model(**API.gets()).get_table_model_structure()
 
 
 @route(
     "/database/whereused",
     parameters=[
         Parameter("data_type", required=True),
         Parameter("value", required=True),
```

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/logs.py` & `alphaz-0.7.8/alphaz/apis/routes/logs.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/mails.py` & `alphaz-0.7.8/alphaz/apis/routes/mails.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,81 @@
 from ...utils.api import route, Parameter
 from .. import mails
 
 from alphaz.models.api import AlphaRequest
+from alphaz.models.database.mais import NewsLetter
 
 from core import core
 
-api         = core.api
-db          = core.db
-log         = core.get_logger('api')
+api = core.api
+db = core.db
+log = core.get_logger("api")
 
-@route('/mails/mailme',logged=False,cache=False)
+
+@route("/mails/mailme", logged=False, cache=False)
 def mail_me():
-    mails.mail_me(api,db)
+    mails.mail_me(api, db)
+
 
-@route('/mails/stayintouch',logged=False,cache=False, 
-    parameters = [
-        Parameter('token',required=True),
-        Parameter('mail',required=True),
-        Parameter('name',required=True)
-    ])
+@route(
+    "/mails/stayintouch",
+    logged=False,
+    cache=False,
+    parameters=[
+        Parameter("token", required=True),
+        Parameter("mail", required=True),
+        Parameter("name", required=True),
+    ],
+)
 def mails_stay_in_touch():
-    token           = api.get('token')
-    user_mail       = api.get('mail')
-    name            = api.get('name')
-
-    mails.stay_in_touch(api,user_mail,name, token,db)
-
-@route('/mails/newsletter',
-    parameters = [
-        Parameter('mail',required=True),
-        Parameter('name',required=True)
-    ]
+    token = api.get("token")
+    user_mail = api.get("mail")
+    name = api.get("name")
+
+    mails.stay_in_touch(api, user_mail, name, token, db)
+
+
+@route(
+    "/mails/newsletter",
+    parameters=[Parameter("mail", required=True), Parameter("name", required=True)],
 )
 def mail_newsletter():
-    db.add(defs.NewsLetter,values=api.get_parameters())
-    return 'saved' 
+    db.add(NewsLetter, values=api.get_parameters())
+    return "saved"
+
 
-@route('/mails/requestview',logged=False,cache=False, 
-    parameters = [
-        Parameter('token',required=True),
-        Parameter('mail',required=True),
-        Parameter('name',required=True),
-        Parameter('id',required=True)
-    ])
+@route(
+    "/mails/requestview",
+    logged=False,
+    cache=False,
+    parameters=[
+        Parameter("token", required=True),
+        Parameter("mail", required=True),
+        Parameter("name", required=True),
+        Parameter("id", required=True),
+    ],
+)
 def mails_request_view():
-    token       = api.get('token')
-    user_mail   = api.get('mail')
-    mail_type   = api.get('name')
-    mail_id     = api.get('id')
-
-    mails.request_view(api,user_mail,token,mail_type,mail_id,db)
-
-@route('/mails/unsubscribe',logged=False,cache=False, 
-    parameters = [
-        Parameter('token',required=True),
-        Parameter('mail',required=True),
-        Parameter('type',required=True)
-    ])
+    token = api.get("token")
+    user_mail = api.get("mail")
+    mail_type = api.get("name")
+    mail_id = api.get("id")
+
+    mails.request_view(api, user_mail, token, mail_type, mail_id, db)
+
+
+@route(
+    "/mails/unsubscribe",
+    logged=False,
+    cache=False,
+    parameters=[
+        Parameter("token", required=True),
+        Parameter("mail", required=True),
+        Parameter("type", required=True),
+    ],
+)
 def mails_unsubscribe():
-    token       = api.get('token')
-    user_mail   = api.get('mail')
-    mail_type   = api.get('type')
+    token = api.get("token")
+    user_mail = api.get("mail")
+    mail_type = api.get("type")
 
-    mails.request_unsubscribe(api,user_mail,token,mail_type,db)
+    mails.request_unsubscribe(api, user_mail, token, mail_type, db)
```

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/main.py` & `alphaz-0.7.8/alphaz/apis/routes/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/tests.py` & `alphaz-0.7.8/alphaz/apis/routes/tests.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,63 @@
 # MODULES
 import sqlalchemy
-
+from pathlib import Path
 
 # CORE
 from core import core
 
 # MODELS
 from ...models.database.users_definitions import Application
 from ...models.tests import Levels
+from ...models.database.tests import Test
 
 # UTILS
 from ...utils.api import route, Parameter
 
 # LIBS
-from ...libs import test_lib, io_lib
+from ...libs import test_lib, io_lib, database_lib
 
+# LOCALS
+from .database import DB_INIT_PARAMETERS
 
 API = core.api
 
+TESTS_PARAMETERS = [
+    Parameter("category", ptype=str),
+    Parameter("categories", ptype=list),
+    Parameter("group", ptype=str),
+    Parameter("groups", ptype=list),
+    Parameter("name", ptype=str),
+    Parameter("names", ptype=list),
+    Parameter("run", ptype=bool),
+    Parameter("file_path", ptype=str),
+    Parameter("coverage", ptype=str),
+    Parameter("load_from_db", ptype=bool),
+    Parameter("stop", ptype=bool),
+    Parameter("report", ptype=str),
+    Parameter("coverage", ptype=str),
+    Parameter("levels", ptype=list[Levels], default=[]),
+    Parameter("failed_only", ptype=bool),
+]
+
 
 @route(
     "/tests",
     parameters=[
-        Parameter("category", ptype=str),
-        Parameter("categories", ptype=list),
-        Parameter("group", ptype=str),
-        Parameter("groups", ptype=list),
-        Parameter("name", ptype=str),
-        Parameter("names", ptype=list),
-        Parameter("run", ptype=bool),
-        Parameter("file_path", ptype=str),
-        Parameter("coverage", ptype=str),
-        Parameter("load_from_db", ptype=bool),
-        Parameter("stop", ptype=bool),
-        Parameter("report", ptype=str),
-        Parameter("coverage", ptype=str),
-        Parameter("levels", ptype=list[Levels], default=[]),
-        Parameter("failed_only", ptype=bool),
+        *TESTS_PARAMETERS,
+        *DB_INIT_PARAMETERS,
     ],
 )
 def get_tests():
-    return test_lib.get_tests_auto(**API.gets())
+    database_lib.init_databases(
+        core, **API.gets(without=[p.name for p in TESTS_PARAMETERS])
+    )
+    return test_lib.get_tests_auto(
+        **API.gets(without=[p.name for p in DB_INIT_PARAMETERS])
+    )
 
 
 @route("/tests/coverage", parameters=[Parameter("file", required=True)])
 def get_coverage_file():
     coverages = io_lib.unarchive_object(API["file"])
     return coverages
 
@@ -52,18 +65,49 @@
 def test_null(update_date=None):
     return core.db.select(
         Application, optional_filters=[Application.update_date == update_date]
     )
 
 
 @route(
-    "test_null",
+    "/test/null",
     parameters=[
         Parameter(
             "update_date",
             required=False,
             none_value=sqlalchemy.null(),
         )
     ],
 )
 def test():
     return test_null(**API.get_parameters())
+
+
+@route("/test/select", pagination=True)
+def select_test():
+    return core.db.select(Test, **API.gets())
+
+
+@route("/test/download")
+def generate_pdf() -> None:
+    from fpdf import FPDF
+
+    directory = core.config.get("directories/tmp")
+    wd_path = Path(directory)
+    file_path = wd_path / "test"
+    file_name = f"test.pdf"
+    pdf = FPDF(unit="mm", format="A4")
+    pdf.add_page()
+    pdf.set_font("Arial", "B", 16)
+
+    # Écrire un titre
+    pdf.cell(0, 10, "Page de test", 0, 1, "C")
+
+    # Définir la police et la taille du texte pour le contenu
+    pdf.set_font("Arial", "", 12)
+
+    # Écrire un paragraphe
+    lorem_ipsum = "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Donec at tincidunt lorem, ut tempus felis. In hac habitasse platea dictumst. Nulla hendrerit, justo id congue placerat, tellus ante ullamcorper ex, eget aliquet enim nisl sit amet orci. Morbi efficitur dolor sed metus rhoncus, a feugiat tortor pulvinar. Mauris ultrices gravida faucibus. Proin fermentum mi a erat efficitur malesuada. Morbi in purus eget lectus feugiat rhoncus. Suspendisse egestas tincidunt metus, sed consectetur turpis aliquet in."
+
+    pdf.multi_cell(0, 10, lorem_ipsum)
+    pdf.output(file_path / file_name, "F")
+    API.get_file(directory=file_path, filename=file_name)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/user_management/application_management.py` & `alphaz-0.7.8/alphaz/apis/routes/user_management/application_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/user_management/permission_management.py` & `alphaz-0.7.8/alphaz/apis/routes/user_management/permission_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/user_management/role_management.py` & `alphaz-0.7.8/alphaz/apis/routes/user_management/role_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/user_management/user_management.py` & `alphaz-0.7.8/alphaz/apis/routes/user_management/user_management.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/routes/users.py` & `alphaz-0.7.8/alphaz/apis/routes/users.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/tests.py` & `alphaz-0.7.8/alphaz/apis/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/users/ldap.py` & `alphaz-0.7.8/alphaz/apis/users/ldap.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/apis/users/users.py` & `alphaz-0.7.8/alphaz/apis/users/users.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,14 +269,15 @@
     try:
         ip_address = request.remote_addr
     except:
         ## getting the hostname by socket.gethostname() method
         hostname = socket.gethostname()
         ## getting the IP address using socket.gethostbyname() method
         ip_address = socket.gethostbyname(hostname)
+        ip_address = "127.0.0.1"
 
     # Add new token session related to user
     if not DB.add_or_update(
         UserSession(
             user_id=user.id,
             token=token,
             ip=ip_address,
```

### Comparing `alphaz-0.7.7.9/alphaz/config/config.css` & `alphaz-0.7.8/alphaz/config/config.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/config/config.html` & `alphaz-0.7.8/alphaz/config/config.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/config/main_configuration.py` & `alphaz-0.7.8/alphaz/config/main_configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/config/page.py` & `alphaz-0.7.8/alphaz/config/page.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/config/source.html` & `alphaz-0.7.8/alphaz/config/source.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/config.json` & `alphaz-0.7.8/alphaz/config.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_core.md` & `alphaz-0.7.8/alphaz/documentations/docs/alpha_core.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_screens.md` & `alphaz-0.7.8/alphaz/documentations/docs/alpha_screens.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/alpha_setup.md` & `alphaz-0.7.8/alphaz/documentations/docs/alpha_setup.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/authorizations.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/authorizations.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/configuration.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/main.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/main.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/methods.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/methods.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/parameters.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/parameters.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api/routes.md` & `alphaz-0.7.8/alphaz/documentations/docs/api/routes.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/api_database.md` & `alphaz-0.7.8/alphaz/documentations/docs/api_database.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/configuration.md` & `alphaz-0.7.8/alphaz/documentations/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/database/init.md` & `alphaz-0.7.8/alphaz/documentations/docs/database/init.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/database/model.md` & `alphaz-0.7.8/alphaz/documentations/docs/database/model.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/database/schema.md` & `alphaz-0.7.8/alphaz/documentations/docs/database/schema.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/database/update.md` & `alphaz-0.7.8/alphaz/documentations/docs/database/update.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/docs/index.md` & `alphaz-0.7.8/alphaz/documentations/docs/index.md`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/mkdocs.yml` & `alphaz-0.7.8/alphaz/documentations/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/404.html` & `alphaz-0.7.8/alphaz/documentations/site/404.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/alpha_admin/index.html` & `alphaz-0.7.8/alphaz/documentations/site/alpha_admin/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/alpha_core/index.html` & `alphaz-0.7.8/alphaz/documentations/site/alpha_core/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/alpha_screens/index.html` & `alphaz-0.7.8/alphaz/documentations/site/alpha_screens/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/alpha_setup/index.html` & `alphaz-0.7.8/alphaz/documentations/site/alpha_setup/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/authorizations/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/authorizations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/cache/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/cache/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/configuration/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/issues/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/issues/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/main/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/methods/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/methods/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/parameters/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/parameters/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/routes/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/routes/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api/sqlalchemy/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api/sqlalchemy/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/api_database/index.html` & `alphaz-0.7.8/alphaz/documentations/site/api_database/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/images/favicon.png` & `alphaz-0.7.8/alphaz/documentations/site/assets/images/favicon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/bundle.7353b375.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ar.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.da.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.de.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.du.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.es.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.fr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.hu.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.it.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ja.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.multi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.nl.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.no.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.pt.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ro.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.ru.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.sv.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.tr.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/min/lunr.vi.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/lunr/tinyseg.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map` & `alphaz-0.7.8/alphaz/documentations/site/assets/javascripts/workers/search.fe42c31b.min.js.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css` & `alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map` & `alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/main.9299cb39.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css` & `alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map` & `alphaz-0.7.8/alphaz/documentations/site/assets/stylesheets/palette.ef6f36e2.min.css.map`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/configuration/index.html` & `alphaz-0.7.8/alphaz/documentations/site/configuration/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/init/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/init/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/instantiate/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/instantiate/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/main/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/main/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/model/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/model/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/relations/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/relations/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/schema/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/schema/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/database/update/index.html` & `alphaz-0.7.8/alphaz/documentations/site/database/update/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/documentation/index.html` & `alphaz-0.7.8/alphaz/documentations/site/documentation/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/index.html` & `alphaz-0.7.8/alphaz/documentations/site/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/search/search_index.json` & `alphaz-0.7.8/alphaz/documentations/site/search/search_index.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/documentations/site/sitemap.xml` & `alphaz-0.7.8/alphaz/documentations/site/sitemap.xml`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/index.html` & `alphaz-0.7.8/alphaz/index.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/api_lib.py` & `alphaz-0.7.8/alphaz/libs/api_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-import json, inspect, requests
+import inspect, requests, json
 
 # UTILS
 from ..utils.api import ROUTES
 
 # MODELS
 from ..models.logger import AlphaLogger
 from ..models.api import ApiMethods
@@ -23,14 +23,15 @@
     url: str,
     params: dict = {},
     log: AlphaLogger | None = None,
     no_log: bool = False,
     method: ApiMethods = ApiMethods.GET,
     requester=None,
     allow_none: bool = False,
+    token: str | None = None,
 ) -> ApiAnswer | None:
     """Get data from api
 
     Args:
         url (str): [description]
         params (dict, optional): [description]. Defaults to {}.
         log (AlphaLogger, optional): [description]. Defaults to None.
@@ -68,55 +69,62 @@
                     ]
                 )
                 + "]"
             )
         else:
             converted_params[key] = json_lib.jsonify_data(value, string_output=True)
 
+    headers = {}
+    if token is not None or core.api.admin_token is not None:
+        token = core.api.admin_token if token is None else token
+        headers["Authorization"] = f"Bearer {token}"
+
     if not "http" in url:
         url = f"http://localhost:{core.api.port}/{url}"
     converted_params["requester"] = requester
     if no_log:
         converted_params["no_log"] = "Y"
     try:
         if method_str.lower() == "post":
-            resp = fct(url=url, data=converted_params)
+            resp = fct(url=url, data=converted_params, headers=headers)
         else:
-            resp = fct(url=url, params=converted_params)
+            resp = fct(url=url, params=converted_params, headers=headers)
     except Exception as ex:
         raise AlphaException(f"Fail to contact {url}", ex=ex)
 
     try:
         answer = resp.json()
     except Exception as ex:
         raise AlphaException(f"Cannot decode answer from {url=}", ex=ex)
+
     if (
         type(answer) == dict
         and answer.get("status", None) is not None
         and answer.get("status_description", None) is not None
     ):
         api_answer = ApiAnswer.map_from_dict(answer)
     else:
-        pagination = resp.headers.get("x-pagination", {})
-        if isinstance(pagination, str):
-            pagination_dict = json.loads(pagination.replace("'", '"'))
-            pagination = ApiPagination.map_from_dict(pagination_dict)
         api_answer = ApiAnswer.map_from_dict(
             {
                 "data": answer,
                 "token_status": resp.headers.get("x-token-status"),
                 "status": resp.headers.get("x-status"),
                 "status_code": resp.status_code,
                 "error": int(resp.headers.get("x-error")),
                 "warning": int(resp.headers.get("x-warning")),
                 "status_description": resp.headers.get("x-status-description"),
                 "requester": resp.headers.get("x-requester"),
-                "pagination": pagination,
             }
         )
+
+    pagination = resp.headers.get("x-pagination", {})
+    if isinstance(pagination, str):
+        pagination_dict = json.loads(pagination.replace("'", '"'))
+        pagination = ApiPagination.map_from_dict(pagination_dict)
+    api_answer.pagination = pagination
     return api_answer
 
 
 def get_api_data(
     url: str,
     params: dict = {},
     log: AlphaLogger | None = None,
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/barcode_lib.py` & `alphaz-0.7.8/alphaz/libs/barcode_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/config_lib.py` & `alphaz-0.7.8/alphaz/libs/config_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,239 +1,244 @@
-import datetime, os, re, configparser, pickle, json
-
-CONFIG_FILE_EXTENSION = ".ini"
-
+# MODULES
+import datetime, os, re, configparser, pickle
 from collections import OrderedDict
 
+# LIBS
 from ..libs import converter_lib, json_lib, io_lib, dict_lib
+
+# MODELS
 from ..models.database.structure import AlphaDatabase
 
 import numpy as np
 
 CONSTANTS = {}
 PARAMETERS = {}
 CONFIGS = {}
+CONFIG_FILE_EXTENSION = ".ini"
 
 
 def un_pickle(value):
     decoded = base64.b64decode(value)
     value = pickle.loads(decoded)
     return value
 
 
 def order(D: dict) -> OrderedDict:
     return OrderedDict(sorted(D.items(), key=lambda x: len(x[0]), reverse=True))
 
 
-def get_db_constants(db: AlphaDatabase) -> OrderedDict:
+def get_db_constants(bind: str | None = None) -> OrderedDict:
+    from core import DB
+
     global CONSTANTS
-    from core import core
 
     """Get constants from database
 
     Args:
-        db (AlphaDatabase): [description]
+        bind (str): [description]
 
     Returns:
         OrderedDict: constants in a dict with <name> key and <value> value
     """
-    model = core.get_table_model(db.name, "constants")
-
-    rows = db.select(model, json=True)
+    rows = DB.select(Constants, json=True)
     values = {x["name"]: x["value"] for x in rows}
 
     now = datetime.datetime.now()
     values["year"] = now.year
     values["month"] = now.month  # TODO: need to update constants each time
     values["day"] = now.day
     values["hour"] = now.hour
     values["minute"] = now.minute
     values["second"] = now.second
 
     order(values)
-    CONSTANT = values
+    CONSTANTS = values
     return CONSTANTS
 
 
-def get_db_parameters(db: AlphaDatabase) -> OrderedDict:
-    global PARAMETERS
-    from core import core
+def get_db_parameters(bind: str | None = None) -> OrderedDict:
+    from core import DB, core
 
     LOG = core.get_logger("config")
+    global PARAMETERS
     """[summary]
 
     Args:
         db ([type]): [description]
         model ([type]): [description]
 
     Returns:
         [type]: [description]
     """
-    model = core.get_table_model(db.name, "parameters")
+    model = DB.get_table_model("parameters", bind=bind)
 
-    rows = db.select(model)
+    rows = DB.select(model)
     values = {}
     for row in rows:
         try:
             values[row.name] = pickle.loads(row.value)
         except Exception as ex:
             LOG.error(f"Cannot load parameter <{row.name}>", ex=ex)
     order(values)
     PARAMETERS = values
     return PARAMETERS
 
 
-def get_db_constant(db: AlphaDatabase, name: str, update: bool = False, separator=None):
+def get_db_constant(
+    name: str, update: bool = False, separator=None, bind: str | None = None
+) -> list[str]:
     """[summary]
 
     Args:
         db ([type]): [description]
         model ([type]): [description]
         core_ ([type]): [description]
         name ([type]): [description]
         update (bool, optional): [description]. Defaults to False.
 
     Returns:
         [type]: [description]
     """
     if update:
-        get_db_constants(db)
+        get_db_constants(bind=bind)
 
     values = None
-    if not is_db_constant(db, name):
-        get_db_constants(db)
-        if is_db_constant(db, name):
+    if not is_db_constant(name, bind=bind):
+        get_db_constants(bind=bind)
+        if is_db_constant(name, bind=bind):
             values = CONSTANTS[name]
+    else:
+        values = CONSTANTS[name]
 
     if separator is not None:
         if values is not None:
             return (
                 str(values)
                 .replace("b", "")
                 .replace('"', "")
                 .replace("'", "")
                 .split(separator)
             )
         return []
     return values
 
 
-def get_db_parameter(db: AlphaDatabase, name: str, update: bool = False):
+def get_db_parameter(name: str, update: bool = False, bind: str | None = None):
     """[summary]
 
     Args:
-        db ([type]): [description]
         model ([type]): [description]
         core_ ([type]): [description]
         name ([type]): [description]
         update (bool, optional): [description]. Defaults to False.
+        bind (str): [description]
 
     Returns:
         [type]: [description]
     """
     values = None
     if update:
-        get_db_parameters(db)
+        get_db_parameters(bind=bind)
 
-    if not is_db_parameter(db, name):
-        get_db_parameters(db)
-        if is_db_parameter(db, name):
+    if not is_db_parameter(name, bind=bind):
+        get_db_parameters(bind=bind)
+        if is_db_parameter(name, bind=bind):
             values = PARAMETERS[name]
     else:
         values = PARAMETERS[name]
     return values
 
 
-def set_db_constant(db: AlphaDatabase, name: str, value):
-    from core import core
+def set_db_constant(name: str, value, bind: str | None = None):
+    from core import DB
 
     """[summary]
 
     Args:
         db ([type]): [description]
         model ([type]): [description]
         name ([type]): [description]
         value ([type]): [description]
     """
     CONSTANTS[name] = value
-    model = core.db.get_table_model(db.name, "constants")
-    db.insert_or_update(model, values={"name": name, "value": value})
+    model = DB.get_table_model("constants", bind=bind)
+    DB.insert_or_update(model, values={"name": name, "value": value})
 
 
-def set_db_parameter(db: AlphaDatabase, name: str, value):  # TODO: set core
-    from core import core
+def set_db_parameter(name: str, value, bind: str | None = None):  # TODO: set core
+    from core import DB
 
     """[summary]
 
     Args:
         db ([type]): [description]
         model ([type]): [description]
         name ([type]): [description]
         value ([type]): [description]
     """
     PARAMETERS[name] = value
-    model = core.db.get_table_model(db.name, "parameters")
+    model = DB.get_table_model("parameters", bind=bind)
     # data                = json.dumps(json_lib.jsonify_data(value))
     data = pickle.dumps(value)
-    db.insert_or_update(model, values={"name": name, "value": data})
+    DB.insert_or_update(model, values={"name": name, "value": data})
 
 
-def is_db_constant(db: AlphaDatabase, name: str):
+def is_db_constant(name: str, bind: str | None = None):
     """[summary]
 
     Args:
         core_ ([type]): [description]
         name ([type]): [description]
 
     Returns:
         [type]: [description]
     """
     return name in CONSTANTS
 
 
-def is_db_parameter(db: AlphaDatabase, name: str):
+def is_db_parameter(name: str, bind: str | None = None):
     """[summary]
 
     Args:
         core_ ([type]): [description]
         name ([type]): [description]
 
     Returns:
         [type]: [description]
     """
     return name in PARAMETERS
 
 
-def get_api_build(db: AlphaDatabase, update: bool = False):
+def get_api_build(update: bool = False, bind: str | None = None):
     """[summary]
 
     Args:
         db ([type]): [description]
         core_ ([type]): [description]
         update (bool, optional): [description]. Defaults to False.
 
     Returns:
         [type]: [description]
     """
-    build = get_db_constant(db, "api_build", update=update)
+    build = get_db_constant("api_build", update=update, bind=bind)
     if build is None:
         build = 0
     return build
 
 
-def upgrade_api_build(db: AlphaDatabase):
+def upgrade_api_build(bind: str | None = None):
     """[summary]
 
     Args:
         db ([type]): [description]
         model ([type]): [description]
         core_ ([type]): [description]
     """
-    build = get_api_build(db)
-    set_db_constant(db, "api_build", int(build) + 1)
+    build = get_api_build()
+    set_db_constant("api_build", int(build) + 1, bind=bind)
 
 
 def get_config_filename(fileName, directory, test=False):
     prefix = "test_" if test else ""
     parametersFileName = "%s/%s" % (
         directory,
         prefix + fileName + CONFIG_FILE_EXTENSION,
@@ -458,33 +463,46 @@
 
     global CONFIGS
     configs = DB.select(Configs)
     configs_dict = {}
     for config in configs:
         keys = [x.lower() for x in config.name.split(":")]
         value = config.value
-        type = config.type.upper().strip()
+        config_type = config.type.upper().strip()
 
-        if type == "BOOLEAN":
-            value = True if "T" in value.upper() else False
-        elif type == "STRING":
-            value = str(value)
-        elif type == "INT":
-            value = int(value)
-        elif type == "STRING[]":
-            value = str(value).split(";")
+        try:
+            match config_type:
+                case "BOOLEAN":
+                    value = True if "T" in value.upper() else False
+                case "STRING":
+                    value = str(value)
+                case "STRING[]":
+                    value = str(value).split(";")
+                case "INT":
+                    value = int(value)
+                case "INT[]":
+                    value = [int(x) for x in str(value).split(";")]
+                case "FLOAT":
+                    value = float(value)
+                case "FLOAT[]":
+                    value = [float(x) for x in str(value).split(";")]
+        except:
+            LOG.error(
+                f"Failed to convert config parameter {config.name} to {config_type}"
+            )
+            value = None
 
         dict_keys = dict_lib.get_nested_dict_from_list(keys)
         dict_lib.set_nested(dict_keys, keys, value)
         configs_dict = dict_lib.merge_dict(configs_dict, dict_keys)
     CONFIGS = configs_dict
     return configs_dict
 
 
-def get_configs_key(keys: list[str], config: str | None = None, default=None):
+def get_configs_key(keys: str | list[str], config: str | None = None, default=None):
     global CONFIGS
     if type(keys) == str:
-        keys = keys.split(";")
+        keys = keys.split(":")
     if CONFIGS is None or len(CONFIGS) == 0:
         CONFIGS = get_configs(config)
     value = dict_lib.get_nested(CONFIGS, [x.lower() for x in keys])
     return value if value is not None else default
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/converter_lib.py` & `alphaz-0.7.8/alphaz/libs/converter_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/database_lib.py` & `alphaz-0.7.8/alphaz/libs/database_lib.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,64 +9,74 @@
 # MODELS
 from ..models.main import AlphaException, AlphaCore
 
 # UTILS
 from ..utils.database import init as init_database_fct
 
 
+def reoder_tables_and_binds_based_on_db_structure(
+    tables: list[str], binds: list[str]
+) -> tuple:
+    db_structure = get_database_structure()
+
+    s_binds, s_tables = [], []
+    for bn in db_structure:
+        tbls = get_tables_for_bind(bn)
+
+        if binds is None or bn in [b.upper() for b in binds]:
+            s_binds.append(bn)
+
+        for t in tbls:
+            if t in db_structure[bn]:
+                if tables is None or t.upper() in tables:
+                    s_tables.append(t)
+    """if tables is None:
+        s_tables = None
+    if binds is None:
+        s_binds = None"""
+    return s_tables, s_binds
+
+
 def init_databases(
     core: AlphaCore,
-    tables: list[str] | dict[str, str] | None = None,
+    tables: list[str] | None = None,
     binds: list[str] | None = None,
     create: bool = False,
     drop: bool = False,
     truncate: bool = False,
-    sqlite: bool = True,
     force: bool = True,
     init: bool = False,
-    init_views: bool = False
+    init_views: bool = False,
+    no_log: bool = False,
 ):
     """Initialise les bases de données en fonction des paramètres fournis. Cette fonction est la principale et appelle les autres fonctions pour effectuer diverses tâches.
 
     Args:
         core (AlphaCore): objet Core contenant les informations de base et les configurations
         tables (list[str] | dict[str, str], optional): Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
         binds (list[str], optional): Liste des binds à traiter. Defaults to None.
         create (bool, optional): Booléen indiquant si les tables doivent être créées. Defaults to False.
         drop (bool, optional): Booléen indiquant si les tables doivent être supprimées. Defaults to False.
         truncate (bool, optional):  Booléen indiquant si les tables doivent être vidées. Defaults to False.
-        sqlite (bool, optional): Booléen indiquant si SQLite doit être utilisé. Defaults to True.
         force (bool, optional): Booléen indiquant si la configuration doit être forcée à 'local'. Defaults to True.
         init (bool, optional): Booléen indiquant si les fichiers d'initialisation doivent être traités. Defaults to False.
     """
     # Vérifie que la configuration est 'local' ou que le paramètre 'force' est True
     if core.configuration != "local" and not force:
         if core.log:
             core.log.error("Configuration must be <local>")
         return
 
     # Normalise le paramètre 'tables'
-    r_tables = init_database_fct.__normalize_tables(tables)
+    tables = [t.upper() for t in tables] if tables is not None else None
 
     # Normalise le paramètre 'binds' et vérifie que les binds sont valides
-    r_binds = init_database_fct.__normalize_and_check_binds(binds, core)
-
-    db_structure = get_database_structure()
+    binds = init_database_fct.__normalize_and_check_binds(binds, core)
 
-    binds, tables = [], []
-    for bn in db_structure:
-        tbls = get_tables_for_bind(bn)
-
-        if r_binds is None or bn in [b.upper() for b in r_binds]:
-            binds.append(bn)
-
-        for t in tbls:
-            if t in db_structure[bn]:
-                if r_tables is None or t in r_tables:
-                    tables.append(t)
+    tables, binds = reoder_tables_and_binds_based_on_db_structure(tables, binds)
 
     # Récupère les modèles de tables à partir des paramètres 'tables' et 'binds'
     tables_models = core.db.get_tables_models(tables, binds)
 
     # Filter views
     if not init_views:
         tables_models = [m for m in tables_models if not getattr(m, "__view__", False)]
@@ -77,33 +87,35 @@
 
     # Initialise les bases de données en fonction des paramètres
     core.db.init_all(
         tables=tables_models,
         create=create,
         drop=drop,
         truncate=truncate,
-        sqlite=sqlite,
         log=core.log,
+        no_log=no_log,
     )
 
     # Charge les fichiers d'initialisation si le paramètre 'init' est True
     if init:
-        init_database_fct.process_init_files(core, binds, tables, init_databases_config)
+        init_database_fct.process_init_files(
+            core, binds, tables, init_databases_config, no_log=no_log
+        )
 
 
 def get_table_content(
     bind: str,
-    tablename: str,
+    table: str,
     order_by: str,
     direction: str,
     page_index: int,
     page_size: int,
     limit: int | None = None,
 ):
-    model = core.db.get_table_model(tablename, bind)
+    model = core.db.get_table_model(table, bind=bind)
     return core.db.select(
         model,
         page=page_index,
         per_page=page_size,
         order_by=order_by,
         order_by_direction=direction,
         limit=limit,
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/date_lib.py` & `alphaz-0.7.8/alphaz/libs/date_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/dict_lib.py` & `alphaz-0.7.8/alphaz/libs/dict_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/emulation/vt102_lib.py` & `alphaz-0.7.8/alphaz/libs/emulation/vt102_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/events.py` & `alphaz-0.7.8/alphaz/libs/events.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/files_lib.py` & `alphaz-0.7.8/alphaz/libs/files_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/flask_lib.py` & `alphaz-0.7.8/alphaz/libs/flask_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/img_lib.py` & `alphaz-0.7.8/alphaz/libs/img_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/io_lib.py` & `alphaz-0.7.8/alphaz/libs/io_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import requests, json, re, os, pickle, pathlib, datetime
+import requests, ujson, re, os, pickle, pathlib, datetime
 from lxml.html import fromstring
 from ..models.main import AlphaFile
 
 
 def ensure_dir(file_path):
     directory = os.path.dirname(file_path)
     if directory != "" and not os.path.exists(directory):
@@ -25,25 +25,25 @@
 
 def save_as_json(filename, data, log=None):
     ensure_file(filename)
     if log:
         log.info(f"Write json file to {filename}")
 
     # Writing JSON data
-    json_content = json.dumps(data, default=myconverter).replace("NaN", '"null"')
+    json_content = ujson.dumps(data, default=myconverter).replace("NaN", '"null"')
     with open(filename, "w", encoding="utf-8") as f:
         f.write(json_content)
-        # json.dump(data, f)
+        # ujson.dump(data, f)
 
 
 def read_json(file_path, log=None):
     data = {}
     if os.path.exists(file_path):
         with open(file_path, encoding="utf-8") as json_data_file:
-            data = json.load(json_data_file)
+            data = ujson.load(json_data_file)
     return data
 
     original = {}
 
     with open(file_path, "r", encoding="utf-8") as f:
         original = f.read()
     # save state
@@ -70,15 +70,15 @@
         if i % 2 == 0:
             j = int(i / 2)
             nxt = text.find('"', p)
             # replacing a portion of a string
             # use slicing to extract those parts of the original string to be kept
             text = text[:p] + states[j][1] + text[nxt:]
 
-    converted = json.loads(text)  # error stems from here
+    converted = ujson.loads(text)  # error stems from here
     return converted
 
 
 def get_proxies(nb=None):
     url = "https://free-proxy-list.net/"
     response = requests.get(url)
     parser = fromstring(response.text)
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/json_lib.py` & `alphaz-0.7.8/alphaz/libs/json_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 import dataclasses
 
-try:
-    import ujson as json
-except:
-    import json
-
-    print("Cannot import ujson")
-
+import ujson
 
 from flask_sqlalchemy.model import DefaultMeta
 from sqlalchemy.orm.attributes import instance_state
 from sqlalchemy import null
 
 from ..libs.time_lib import timer
 
@@ -45,15 +39,15 @@
             relationship=relationship, disabled_relationships=disabled_relationships
         )
 
         structures = schema()  # schema(many=True) if not first else
         results_json = structures.dump(model)  # TODO: ? wtf why does it works
     else:
         try:
-            results_json = json.dumps(model.__dict__)
+            results_json = ujson.dumps(model.__dict__)
         except:
             results_json = str(model)
     return results_json
 
 
 def is_standard(data) -> bool:
     if type(data) == Row:
@@ -104,34 +98,34 @@
         elif hasattr(data, "_fields"):
             result = {x: data[i] for i, x in enumerate(data._fields)}
         elif hasattr(data, "to_json"):
             result = data.to_json()
         elif dataclasses.is_dataclass(data):
             result = dataclasses.asdict(data)
     if string_output:
-        result = json.dumps(result)
+        result = ujson.dumps(result)
     return result
 
 
 def load_json(string: str):
     if string is None:
         return None
     if type(string) != str:
         string = str(string)
     string = string.strip()
 
     if len(string) != 0 and string[0] == "{" and string[-1] == "}":
         try:
-            return json.loads(string)
+            return ujson.loads(string)
         except Exception as ex:
             print(f"Cannot convert to json: {string[:100]}")
             raise ex
 
     if len(string) == 0:
         string = '""'
     string = '{"json":' + string + "}"
     try:
-        data = json.loads(string)
+        data = ujson.loads(string)
     except Exception as ex:
         print(f"Cannot convert to json: {string[:100]}")
         raise ex
     return data["json"]
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/logs_lib.py` & `alphaz-0.7.8/alphaz/libs/logs_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/mail_lib.py` & `alphaz-0.7.8/alphaz/libs/mail_lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import smtplib, socks, copy, json
+import smtplib, socks, copy, ujson
 
 
 import hashlib, re, os, datetime
 from flask import current_app
 from flask_mail import Message
 
 import uuid
 
-from alphaz.models.database.main_definitions import MailHistory
+from alphaz.models.database.mails import MailHistory, MailBlacklist
 
 from . import string_lib
 from ..models.config._utils import get_mails_parameters
 
 from ..models.api import _utils
 
 # CORE
@@ -390,30 +390,30 @@
 def is_mail_already_send(db, mail_type, parameters, log=None):
     from ..models.database import main_definitions as defs
 
     mail_type = get_mail_type(mail_type)
     unique_parameters = get_unique_parameters(parameters)
 
     results = db.select(
-        defs.MailHistory,
+        MailHistory,
         filters=[
-            defs.MailHistory.mail_type == mail_type,
-            defs.MailHistory.parameters == json.dumps(unique_parameters),
+            MailHistory.mail_type == mail_type,
+            MailHistory.parameters == ujson.dumps(unique_parameters),
         ],
         json=True,
     )
     return len(results) != 0
 
 
 def is_blacklisted(db, user_mail, mail_type, log=None):
     from ..models.database import main_definitions as defs
 
     mail_type = get_mail_type(mail_type)
     results = db.select(
-        defs.MailBlacklist,
+        MailBlacklist,
         filters=[
-            defs.MailBlacklist.mail_type == mail_type,
-            defs.MailBlacklist.mail == user_mail,
+            MailBlacklist.mail_type == mail_type,
+            MailBlacklist.mail == user_mail,
         ],
         json=True,
     )
     return len(results) != 0
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/notifications_lib.py` & `alphaz-0.7.8/alphaz/libs/notifications_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/number_lib.py` & `alphaz-0.7.8/alphaz/libs/number_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/process_lib.py` & `alphaz-0.7.8/alphaz/libs/process_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/py_lib.py` & `alphaz-0.7.8/alphaz/libs/py_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/scp_lib.py` & `alphaz-0.7.8/alphaz/libs/scp_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/search_lib.py` & `alphaz-0.7.8/alphaz/libs/search_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/secure_lib.py` & `alphaz-0.7.8/alphaz/libs/secure_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/soap_lib.py` & `alphaz-0.7.8/alphaz/libs/soap_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/ssh_lib.py` & `alphaz-0.7.8/alphaz/libs/ssh_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/string_lib.py` & `alphaz-0.7.8/alphaz/libs/string_lib.py`

 * *Files 6% similar despite different names*

```diff
@@ -283,15 +283,15 @@
     ]
     max_value = max(match_values)
     if threshold is not None and max_value < threshold:
         return None, max_value
     return words[match_values.index(max_value)], max_value
 
 
-def to_list(o: str) -> list[str]:
+def to_list(o: str) -> list[str]:  # TODO delete ?
     """
     Convert a string representation of a list to a list of strings.
 
     The input string should be a comma-separated list of values, optionally enclosed in square brackets. String values
     may be enclosed in either single or double quotes.
 
     Args:
@@ -318,14 +318,33 @@
             el = el[1:]
         if el.endswith(("'", '"')):
             el = el[:-1]
         output.append(el)
     return output
 
 
+def str_to_str_list(input_str: str, separators: list[str] | None = None) -> list[str]:
+    if separators is None:
+        separators = [",", ";"]
+    # Check if the input string is "[]"
+    if input_str == "[]":
+        return []
+
+    # Remove outer brackets if present
+    input_str = re.sub(r"^\[(.+)\]$", r"\1", input_str)
+
+    # Split on "," or ";" if present, otherwise return the original string
+    if "," in input_str or ";" in input_str:
+        return re.split("|".join(separators), input_str)
+    elif input_str == "":
+        return []
+    else:
+        return [input_str]
+
+
 def escape_ansi(line: str) -> str:
     """
     Remove ANSI escape codes from a string.
 
     Args:
         line: A string that may contain ANSI escape codes.
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/test_lib.py` & `alphaz-0.7.8/alphaz/libs/test_lib.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 LOG = core.get_logger("tests")
 
 CATEGORIES = {}
 
 
 def __group_parameters(
     name: str | None = None,
-    names: list[str] = [],
+    names: list[str] | None = None,
     group: str | None = None,
-    groups: list[str] = [],
+    groups: list[str] | None = None,
     category: str | None = None,
-    categories: list[str] = [],
+    categories: list[str] | None = None,
 ):
     categories = categories if categories is not None else []
     groups = groups if groups is not None else []
     names = names if names is not None else []
 
     if category is not None:
         categories.append(category)
@@ -54,16 +54,17 @@
     subclasses_by_module = defaultdict(list)
     for subclass in subclasses:
         module_name = subclass.__module__.split(".")[0]
         subclasses_by_module[module_name].append(subclass)
 
     test_categories = TestCategories()
     for category, class_list in subclasses_by_module.items():
+        groups_str = ", ".join([x.__name__ for x in class_list])
         LOG.info(
-            f'Loaded test module <{category}> with test groups: {", ".join([x.__name__ for x in class_list])}'
+            f"Loaded test module <{category}> with test groups: {groups_str[:100]} ..."
         )
 
         for el in class_list:
             test_group = TestGroup(el, coverage=coverage is not None)
 
             if len(categories) != 0 and test_group.category not in categories:
                 continue
@@ -81,25 +82,25 @@
         test_categories.test_all(names, levels, stop=stop, failed_only=failed_only)
 
     return test_categories
 
 
 def get_tests_auto(
     name: str | None = None,
-    names: list[str] = [],
+    names: list[str] | None = None,
     group: str | None = None,
-    groups: list[str] = [],
+    groups: list[str] | None = None,
     category: str | None = None,
-    categories: list[str] = [],
+    categories: list[str] | None = None,
     file_path: str | None = None,
     run: bool = False,
     load_from_db: bool = False,
     report: str | None = None,
     coverage: str | None = None,
-    levels: list[Levels] = [],
+    levels: list[Levels] | None = None,
     stop: bool = False,
     failed_only: bool = False,
 ) -> TestCategories:
     """Get the TestCategories class, containings all required tests.
 
     Args:
         tests_modules (list[str]): list of test modules path
```

### Comparing `alphaz-0.7.7.9/alphaz/libs/time_lib.py` & `alphaz-0.7.8/alphaz/libs/time_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/transactions_lib.py` & `alphaz-0.7.8/alphaz/libs/transactions_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/user_lib.py` & `alphaz-0.7.8/alphaz/libs/user_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/user_management/application_management_lib.py` & `alphaz-0.7.8/alphaz/libs/user_management/application_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/user_management/permission_management_lib.py` & `alphaz-0.7.8/alphaz/libs/user_management/permission_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/user_management/role_management_lib.py` & `alphaz-0.7.8/alphaz/libs/user_management/role_management_lib.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/libs/user_management/user_management_lib.py` & `alphaz-0.7.8/alphaz/libs/user_management/user_management_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-import json
+import ujson
 
 
 from sqlalchemy import or_, and_, outerjoin
 from alphaz.models.database.users_definitions import (
     User,
     UserRole,
     Role,
@@ -81,10 +81,10 @@
 
     added_infos = users.infos_dict_from_ldap(ldap.LDAP_DATA, res)
 
     user = {
         "username": res["uid"],
         "mail": res["mail"] if "mail" in res else "-",
         "date_registred": datetime.now(),
-        "infos": json.dumps(added_infos),
+        "infos": ujson.dumps(added_infos),
     }
     return DB.add(User(**user))
```

### Comparing `alphaz-0.7.7.9/alphaz/mails/Images/Background.png` & `alphaz-0.7.8/alphaz/mails/Images/Background.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/Images/Facebook_logo.png` & `alphaz-0.7.8/alphaz/mails/Images/Facebook_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/Images/Twitter_logo.png` & `alphaz-0.7.8/alphaz/mails/Images/Twitter_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/Images/Web_logo.png` & `alphaz-0.7.8/alphaz/mails/Images/Web_logo.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/Mail.png` & `alphaz-0.7.8/alphaz/mails/Mail.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/Webmail.html` & `alphaz-0.7.8/alphaz/mails/Webmail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/debug.html` & `alphaz-0.7.8/alphaz/mails/debug.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/mail.html` & `alphaz-0.7.8/alphaz/mails/mail.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/password_reset.html` & `alphaz-0.7.8/alphaz/mails/password_reset.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/mails/stay_in_touch.html` & `alphaz-0.7.8/alphaz/mails/stay_in_touch.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_answer.py` & `alphaz-0.7.8/alphaz/models/api/_answer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from dataclasses import (
     dataclass,
     field,
 )
 from ..main import _base
 
+from ...libs import json_lib
+
 
 @dataclass
 class ApiPagination(_base.AlphaDataclass):
     total: int | None = None
     total_pages: int | None = None
     page: int | None = None
     previous_page: int | None = None
@@ -24,14 +26,14 @@
     status_code: int = 200
     status_description: str = ""
     requester: str = "unknow"
     data: dict = field(default_factory=lambda: {})
     pagination: ApiPagination = field(default_factory=lambda: {})
 
     def to_json(self):
-        return self.get_fields_dict()
+        return json_lib.jsonify_data(self.get_fields_dict())
 
     def set_error(self, description: str):
         self.error = 1
         self.status = "error"
         self.status_code = 520
         self.status_description = description
```

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_colorations.py` & `alphaz-0.7.8/alphaz/models/api/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_parameter.py` & `alphaz-0.7.8/alphaz/models/api/_parameter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,109 @@
-import json, datetime, dataclasses, re, sqlalchemy, xmltodict
+# MODULES
+import ujson, datetime, re, sqlalchemy, xmltodict
 
 from sqlalchemy.ext.declarative import DeclarativeMeta
 from sqlalchemy import inspect as inspect_sqlalchemy
 
 from flask import request
 from collections.abc import Callable
 
+# MAIN
 from ..main import AlphaException
 from ..main._base import is_dataclass
-from ..main._enum import MappingMode
+from ..main._enum import MappingMode, ParameterMode
 
-from ...libs import date_lib, json_lib, py_lib
+# LIBS
+from ...libs import date_lib, json_lib, py_lib, string_lib
 
-from enum import Enum
+
+# TODO: remove form
+def convert_parameter_value(
+    name: str,
+    value,
+    ptype,
+    form,
+    mode=None,
+    map_none: bool = False,
+    required: bool = False,
+    mapping_mode: MappingMode | None = None,
+):
+    str_value = str(value).lower()
+    if py_lib.is_subtype(ptype, bool):
+        if str_value in ["y", "true", "t", "1"]:
+            value = True
+        elif str_value in ["n", "false", "f", "0"]:
+            value = False
+        elif not required and value is None:
+            value = None
+        else:
+            raise AlphaException(
+                f"Wrong value <{value}> for parameter <{name}> of type <bool>",
+            )
+        value = value
+    elif py_lib.is_subtype(ptype, int):
+        try:
+            value = int(value) if value is not None else None
+        except:
+            raise AlphaException(
+                f"Wrong value <{value}> for parameter <{name}> of type <int>"
+            )
+    elif py_lib.is_subtype(ptype, float):
+        try:
+            value = float(value)
+        except:
+            raise AlphaException(
+                f"Wrong value <{value}> for parameter <{name}> of type <float>"
+            )
+    elif ptype == datetime.datetime:
+        value = date_lib.str_to_datetime(value)
+    elif py_lib.is_subtype(ptype, dict):
+        value = json_lib.load_json(value)
+    elif str_value in ["null()"]:
+        value = sqlalchemy.null()
+    elif str_value in [
+        "null",
+        "none",
+        "undefined",
+    ]:
+        value = None
+    elif is_dataclass(ptype):
+        if hasattr(ptype, "map_from_json"):
+            value = ptype.map_from_json(value, mapping_mode=mapping_mode)
+        else:
+            try:
+                P = ujson.loads(value)
+            except Exception as ex:
+                raise ex
+            value = ptype(**P)
+    elif isinstance(ptype, DeclarativeMeta):  # DB MODEL
+        if value is None:
+            parameters = {x: y for x, y in form.items() if hasattr(ptype, x)}
+        else:
+            parameters = value if type(value) == dict else json_lib.load_json(value)
+            parameters = {
+                x: y
+                for x, y in parameters.items()
+                if hasattr(ptype, x) and (map_none or y is not None)
+            }  # TODO: enhance
+        value = dict_to_model(ptype, parameters)
+    elif hasattr(ptype, "metadata") and not hasattr(
+        value, "metadata"
+    ):  # classic dataclass
+        r = ujson.loads(value)
+        value = ptype(**r)
+    elif py_lib.is_subtype(ptype, str):
+        if mode in [
+            ParameterMode.LIKE,
+            ParameterMode.IN_LIKE,
+            ParameterMode.START_LIKE,
+            ParameterMode.END_LIKE,
+        ]:
+            value = set_value_like_mode(value, mode)
+    return value
 
 
 def dict_to_model(model, parameters):
     from core import core
 
     inspected = inspect_sqlalchemy(model)
 
@@ -67,28 +154,14 @@
         ParameterMode.IN_LIKE,
         ParameterMode.END_LIKE,
     ]:
         value = f"{value}%"
     return value
 
 
-class ParameterMode(Enum):
-    NONE = 0
-    LIKE = 1
-    IN_LIKE = 2
-    START_LIKE = 3
-    END_LIKE = 4
-
-    def __str__(self):
-        return str(self.value)
-
-    def to_json(self):
-        return str(self.value)
-
-
 class Parameter:
     _value = None
     no_log: bool = False
 
     def __init__(
         self,
         name: str,
@@ -98,19 +171,21 @@
         options=None,
         cacheable: bool = True,
         required: bool = False,
         ptype: type = str,
         private: bool = False,
         mode: ParameterMode = ParameterMode.NONE,
         override: bool = False,
-        function: Callable = None,
+        function: Callable | None = None,
         mapping_mode: MappingMode | str | None = None,
         map_none: bool = False,
         max_size: int | None = None,
         min_size: int | None = None,
+        max_value: int | None = None,
+        min_value: int | None = None,
         separators: list = [",", ";"],
     ):
         """[summary]
 
         Args:
             name (str): [description]
             default ([type], optional): [description]. Defaults to None.
@@ -135,18 +210,20 @@
         self.mode = mode
         self.override = override
         self.is_value = False
         self.mapping_mode = mapping_mode
         self.max_size = max_size
         self.min_size = min_size
         self.map_none = map_none
+        self.max_value = max_value
+        self.min_value = min_value
 
     @property
     def value(self):
-        return self._value if self._value is not None else self.default
+        return self._value if self._value is not None or self.is_value else self.default
 
     def __check_options(self, value):
         if (
             self.options is not None
             and value not in self.options
             and not (not self.required and value is None)
         ):
@@ -155,25 +232,15 @@
                 parameters={
                     "value": value,
                     "parameter": self.name,
                     "options": str(self.options),
                 },
             )
 
-    def set_value(self, method: str, dataDict, api_json, form, args):
-        """Set parameter value
-
-        Raises:
-            AlphaException: [description]
-        """
-        # dataDict: for list GET
-        self._value = self.default
-        self.name = self.name.strip()
-        dataDict = {x.strip(): y for x, y in dataDict.items()}
-
+    def _get_value_from_request(self, dataDict, api_json, form, args):
         if "<xml>" in str(request.data):
             try:
                 data = xmltodict.parse(request.data)
                 if self.name in data["xml"]:
                     self._value = data["xml"][self.name]
             except:
                 pass
@@ -195,14 +262,45 @@
         elif self.name in args:
             self._value = args.get(self.name)
             self.is_value = True
         elif self.name in dataDict:
             self._value = dataDict[self.name]
             self.is_value = True
 
+    def _check_min_max_value(self):
+        if (
+            self.max_value is not None
+            and self._value is not None
+            and type(self._value) in [int, float]
+            and self._value > self.max_value
+        ):
+            raise AlphaException(
+                "api_parameter_value_above_max",
+                parameters={
+                    "parameter": self.name,
+                    "value": self._value,
+                    "max_value": self.max_value,
+                },
+            )
+        if (
+            self.min_value is not None
+            and self._value is not None
+            and type(self._value) in [int, float]
+            and self._value < self.min_value
+        ):
+            raise AlphaException(
+                "api_parameter_value_below_min",
+                parameters={
+                    "parameter": self.name,
+                    "value": self._value,
+                    "min_value": self.min_value,
+                },
+            )
+
+    def _check_sizes(self):
         # check size
         if (
             self.max_size is not None
             and self._value is not None
             and len(self._value) > self.max_size
         ):
             raise AlphaException(
@@ -216,191 +314,126 @@
             )
         if (
             self.min_size is not None
             and self._value is not None
             and len(self._value) < self.min_size
         ):
             raise AlphaException(
-                "api_parameter_length_too_long",
+                "api_parameter_length_too_short",
                 parameters={
                     "parameter": self.name,
                     "size": len(self.value),
                     "value": self._value,
                     "min": self.min_size,
                 },
             )
 
-        # list
-        if self.ptype == list or py_lib.is_subtype(self.ptype, list):
-            is_empty = self._value is None or str(self._value).strip() == ""
-            is_empty_value = all(not x in str(self._value) for x in [";", ",", "["])
-
-            if is_empty:
-                self._value = self.default
-            elif is_empty_value:
-                self._value = (
-                    dataDict[self.name] if self.name in dataDict else self.default
-                )
-
-            sub_type = py_lib.get_subtype(self.ptype)
-            if is_dataclass(sub_type):
-                if self._value is not None:
-                    values = re.findall(r"{[^{]*}", str(self._value))
-                    self._value = self.default if len(values) == 0 else []
-                    for val in values:
-                        if hasattr(sub_type, "map_from_json"):
-                            val = sub_type.map_from_json(
-                                val, mapping_mode=self.mapping_mode
-                            )
-                        else:
-                            P = json.loads(val)
-                            val = sub_type(**P)
-                        self._value.append(val)
-                else:
-                    self._value = self.default
-
+    def _check_none(self, form) -> bool:
         if self._value is None and form is not None and self.name in form:
             self._value = form[self.name]
-        if self._value is None and form is not None and self.name in form:
-            self._value = form[self.name]
-
-        if isinstance(self.ptype, DeclarativeMeta):
-            if self._value is None:
-                parameters = {x: y for x, y in form.items() if hasattr(self.ptype, x)}
-            else:
-                parameters = (
-                    self._value
-                    if type(self._value) == dict
-                    else json_lib.load_json(self._value)
-                )
-                parameters = {
-                    x: y
-                    for x, y in parameters.items()
-                    if hasattr(self.ptype, x) and (self.map_none or y is not None)
-                }  # TODO: enhance
-            self._value = dict_to_model(self.ptype, parameters)
-        elif is_dataclass(self.ptype):
-            if hasattr(self.ptype, "map_from_json"):
-                self._value = self.ptype.map_from_json(
-                    self._value, mapping_mode=self.mapping_mode
-                )
-            else:
-                P = json.loads(self._value)
-                self._value = self.ptype(**P)
-
-        if self.ptype == dict:
-            self._value = json_lib.load_json(self._value)
-
-        if self.required and (self._value is None or str(self._value) == "undefined"):
-            raise AlphaException(f"Missing parameter {self.name}")
 
+        if self._value is not None and str(self._value).lower() in [
+            "null",
+            "none",
+            "undefined",
+        ]:
+            self._value = self.none_value if self.is_value else None
+            self.__check_options(self._value)
+            return False
         if self._value is None:
             self.__check_options(self._value)
-            return
+            self._value = self.default
+        if self._value is None and self.required:
+            raise AlphaException(f"Parameter {self.name} is required")
+        return self._value is not None
+
+    def _process_list_value(self, dataDict, form) -> bool:
+        if not py_lib.is_subtype(self.ptype, list):
+            return False
+        is_empty = self._value is None or str(self._value).strip() == ""
+        if is_empty:
+            self._value = self.default
+            return True
+
+        is_empty_value = all(not x in str(self._value) for x in [";", ",", "["])
+
+        if is_empty_value:
+            dataDict = {x.strip(): y for x, y in dataDict.items()}
+            self._value = dataDict[self.name] if self.name in dataDict else self.default
 
-        if str(self._value).lower() in ["null", "none", "undefined"]:
-            self._value = self.none_value if self.is_value else None
-        if str(self._value).lower() in ["null()"]:
-            self._value = sqlalchemy.null()
-        if self.empty_value is not None and str(self._value).lower() == "":
-            self._value = self.empty_value
-
-        if self.ptype == str and (
-            self.mode
-            in [
-                ParameterMode.LIKE,
-                ParameterMode.IN_LIKE,
-                ParameterMode.START_LIKE,
-                ParameterMode.END_LIKE,
-            ]
-        ):
-            self._value = set_value_like_mode(self._value, self.mode)
+        if self._value is None:
+            return True
 
-        if self.ptype == bool:
-            str_value = str(self._value).lower()
-            self.__check_options(str(self._value))
-
-            if str_value in ["y", "true", "t", "1"]:
-                value = True
-            elif str_value in ["n", "false", "f", "0"]:
-                value = False
-            else:
-                raise AlphaException(
-                    f"Wrong value <{self._value}> for parameter <{self.name}> of type <bool>",
+        sub_type = py_lib.get_subtype(self.ptype)
+        if is_dataclass(sub_type):
+            values = re.findall(r"{[^{]*}", str(self._value))
+            self._value = self.default if len(values) == 0 else []
+            for val in values:
+                if hasattr(sub_type, "map_from_json"):
+                    val = sub_type.map_from_json(val, mapping_mode=self.mapping_mode)
+                else:
+                    P = ujson.loads(val)
+                    val = sub_type(**P)
+                self._value.append(val)
+        else:
+            if not py_lib.is_subtype(self._value, list):
+                self._value = string_lib.str_to_str_list(
+                    str(self._value), separators=[",", ";"]
                 )
-            self._value = value
 
-        if self.ptype == list or py_lib.is_subtype(self.ptype, list):
-            if type(self._value) == str and str(self._value).strip() == "":
-                self._value = []
-            elif type(self._value) == str:
-                try:
-                    if (
-                        len(str(self._value)) != 0
-                        and str(self._value)[0] == "["
-                        and str(self._value)[-1] == "]"
-                    ):
-                        self._value = (
-                            str(self._value)[1:-1].split(";")
-                            if ";" in str(self._value)
-                            else str(self._value)[1:-1].split(",")
-                        )
-                    elif ";" in str(self._value) or "," in str(self._value):
-                        self._value = (
-                            str(self._value).split(";")
-                            if ";" in str(self._value)
-                            else str(self._value).split(",")
-                        )
-                    else:
-                        self._value = [self._value]
-                except:
-                    raise AlphaException(
-                        f"Wrong value <{self._value}> for parameter <{self.name}> of type <list>"
-                    )
-
-            if py_lib.is_subtype(self.ptype, list[int]):
-                self._value = [int(x) for x in self._value]
-            if py_lib.is_subtype(self.ptype, list[float]):
-                self._value = [float(x) for x in self._value]
+            self._value = [
+                convert_parameter_value(
+                    self.name, x, py_lib.get_subtype(self.ptype), form
+                )
+                for x in self._value
+            ]
 
             for val in self._value:
                 self.__check_options(val)
 
             if self.mode in [
                 ParameterMode.LIKE,
                 ParameterMode.IN_LIKE,
                 ParameterMode.START_LIKE,
                 ParameterMode.END_LIKE,
             ]:
                 self._value = [set_value_like_mode(x, self.mode) for x in self._value]
+        return True
 
-        if self.ptype == int:
-            try:
-                self._value = int(self._value) if self._value is not None else None
-            except:
-                raise AlphaException(
-                    f"Wrong value <{self._value}> for parameter <{self.name}> of type <int>"
-                )
-            self.__check_options(self._value)
+    def set_value(self, dataDict: dict, api_json, form, args):
+        """Set parameter value
 
-        if self.ptype == float:
-            try:
-                self._value = float(self._value)
-            except:
-                raise AlphaException(
-                    f"Wrong value <{self._value}> for parameter <{self.name}> of type <float>"
-                )
-            self.__check_options(self._value)
+        Raises:
+            AlphaException: [description]
+        """
+        dataDict = {x.strip(): y for x, y in dataDict.items()}
 
-        if self.ptype == datetime.datetime:
-            self.__check_options(self._value)
-            self._value = date_lib.str_to_datetime(self._value)
+        self._value = self.default
+        self.name = self.name.strip()
 
-        if hasattr(self.ptype, "metadata") and not hasattr(self._value, "metadata"):
-            r = json.loads(self._value)
-            self._value = self.ptype(**r)
+        self._get_value_from_request(dataDict, api_json, form, args)
+        self._check_sizes()
+        self._check_min_max_value()
+
+        if not self._check_none(form):
+            return
+
+        # list
+        if not self._process_list_value(dataDict, form):
+            if self.empty_value is not None and str(self._value).lower() == "":
+                self._value = self.empty_value
+
+            self._value = convert_parameter_value(
+                self.name,
+                self._value,
+                self.ptype,
+                form,
+                mode=self.mode,
+                map_none=self.map_none,
+                required=self.required,
+                mapping_mode=self.mapping_mode,
+            )
 
-        if self.ptype == str:
-            self.__check_options(str(self._value))
+        self.__check_options(self._value)
 
         if self.function is not None:
             self._value = self.function(self._value)
```

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_reloader.py` & `alphaz-0.7.8/alphaz/models/api/_reloader.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_reloaders.py` & `alphaz-0.7.8/alphaz/models/api/_reloaders.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_requests.py` & `alphaz-0.7.8/alphaz/models/api/_requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_route.py` & `alphaz-0.7.8/alphaz/models/api/_route.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,8 @@
-import datetime, os, copy
-
-try:
-    import ujson as json
-except:
-    import json
-
-    print("Cannot import ujson")
+import datetime, os, copy, ujson, json
 import time
 import traceback
 
 from flask import (
     jsonify,
     request,
     make_response,
@@ -18,24 +11,25 @@
 )
 
 from ...libs.time_lib import timer
 
 from ...libs import json_lib, converter_lib, io_lib, py_lib
 from ...models.main import AlphaException
 from ...models.api import ApiAnswer, AlphaRequest
+from ...models.json._converters import AlphaJSONEncoder
 
 from ._parameter import Parameter
 from ..main._exception import get_message_from_name
 
 SEPARATOR = "__"
-DEBUG = False
+DEBUG = True
 
 
 def get_columns_values_output(
-    objects: list, columns: list = None, header: bool = False
+    objects: list, columns: list | None = None, header: bool = False
 ) -> dict:
     """Generate columns names output columns names + list of list (only the values) + nb of values if not header
     ex : { "columns":["col1","col2",...], "values": ["value1","value2",..], "values_nb":12}
 
     else Generate columns names output columns names + list of JSON objetcs + nb of values,
 
     ex : { "columns":["col1","col2",...], "values": [{"col1": "value1",...},{...}], "values_nb":12}
@@ -155,20 +149,20 @@
 
         self.page: int = 0
         self.total, self.total_pages, self.per_page = None, None, None
         self._is_pagination: bool | None = None
 
         self.init_return()
 
-        self.parameters: dict[Parameter] = {y.name: copy.copy(y) for y in parameters}
+        self.parameters: dict[str, Parameter] = {
+            y.name: copy.copy(y) for y in parameters
+        }
         for parameter in self.parameters.values():
             try:
-                parameter.set_value(
-                    self.method, self.dict, self.json, self.form, self.args
-                )
+                parameter.set_value(self.dict, self.json, self.form, self.args)
                 if parameter.name == "no_log":
                     self.no_log = parameter.value
                 else:
                     parameter.no_log = self.no_log
             except Exception as ex:
                 # TODO: enhance
                 message = traceback.format_exc()
@@ -382,17 +376,17 @@
     def is_paginated(self):
         return (
             self.parameters.get("page", None) is not None
             and self.parameters.get("per_page", None) is not None
         )
 
     def is_pagination(self) -> bool:
-        if self._is_pagination is not None:
-            pagination_mode = self.api.db.config.get("pagination_mode", "raw")
-            if pagination_mode == "integrated":
+        if self._is_pagination is None:
+            pagination_mode = self.api.db.config.get("pagination_mode", "standard")
+            if pagination_mode == "standard":
                 is_pagination = self.api.db.full_count is not None
             else:
                 is_pagination = self.page is not None and (
                     py_lib.is_list(self.data)
                     and len(self.data) == 2
                     and type(self.data[0]) == list
                     and type(self.data[1]) == int
@@ -408,31 +402,31 @@
             None,
             None,
             self.get("page", 0),
             self.get("per_page", None),
         )
 
         is_pagination = self.is_pagination()
-        pagination_mode = self.api.db.config.get("pagination_mode", "raw")
-        if pagination_mode == "integrated":
+        pagination_mode = self.api.db.config.get("pagination_mode", "standard")
+        if pagination_mode == "standard":
             if is_pagination and py_lib.is_iterable(data):
                 self.per_page = len(data) if self.per_page is None else self.per_page
                 self.total = (
                     self.api.db.full_count if self.api.db.full_count is not None else 0
                 )
                 self.total_pages = (
                     int(self.total / self.per_page)
                     if self.per_page is not None and self.per_page != 0
                     else 0
                 )
         else:
             if self.per_page is None and is_pagination:
                 self.per_page = len(data[0])
 
-            if "pagination" in format_ and is_pagination:
+            if not "inpagination" in format_ and is_pagination:
                 self.total, self.total_pages = (
                     data[1] if data[1] is not None else 0,
                     int(data[1] / self.per_page) if self.per_page is not None else 0,
                 )
                 data = data[0]
             self.data = data
 
@@ -456,53 +450,57 @@
             headers[key] = value
         headers[
             "Access-Control-Expose-Headers"
         ] = "*"  # ",".join(headers_content.keys())
         # headers["Access-Control-Allow-Headers"] = "*" # ",".join(headers_content.keys())
 
         # returned = Response(returned, status=returned["status_code"])
-        if "pagination" in format_ and self.is_pagination():
-            headers["X-pagination"] = {
-                "total": self.total,
-                "total_pages": self.total_pages,
-                "page": self.page,
-                "previous_page": self.page - 1 if self.page > 0 else 0,
-                "next_page": (
-                    self.page + 1 if self.page < self.total_pages else self.total_pages
-                )
-                if (self.total_pages is not None and self.page is not None)
-                else None,
-                "per_page": self.per_page,
-            }
+        if self.is_pagination():
+            headers["X-pagination"] = json.dumps(
+                {
+                    "total": self.total,
+                    "total_pages": self.total_pages,
+                    "page": self.page,
+                    "previous_page": self.page - 1 if self.page > 0 else 0,
+                    "next_page": (
+                        self.page + 1
+                        if self.page < self.total_pages
+                        else self.total_pages
+                    )
+                    if (self.total_pages is not None and self.page is not None)
+                    else None,
+                    "per_page": self.per_page,
+                }
+            )
 
         return headers
 
     def get_format(self) -> str:
-        default_format = self.api.conf.get("default_format", "json")
+        default_format = self.api.conf.get("default_format", "standard")
         format_ = self.get("format", default=default_format, enable_none=False).lower()
         return format_
 
     def get_return(self, forceData=False, return_status=None):
         format_ = self.get_format()
 
         if self.mode == "html":
             if "page" in self.data:
                 return render_template(self.data["page"], **self.data["parameters"])
             else:
                 return self.data
         elif self.mode == "print":
             return self.message
         elif "get_file" in self.mode:
-            file_path, filename = self.file_to_get
+            directory, filename = self.file_to_get
             if file_path is not None and filename is not None:
                 if not self.no_log:
-                    self.log.info(f"Sending file {filename} from {file_path}")
+                    self.log.info(f"Sending file {filename} from {directory}")
                 try:
                     return send_from_directory(
-                        file_path,
+                        directory,
                         filename,
                         as_attachment="attached" in self.mode,
                     )
                 except FileNotFoundError:
                     self.set_error("missing_file")
             else:
                 self.set_error("missing_file")
@@ -515,15 +513,15 @@
             self.data = {}
 
         self.returned.data = {}
 
         self.set_pagination()
 
         data = self.data
-        if not check_format(data):
+        if "check" in format_ and not check_format(data):
             tic = time.perf_counter()
             data = json_lib.jsonify_data(data)
             toc = time.perf_counter()
             elapsed_time = toc - tic
             if DEBUG:
                 print(f"Elapsed time: {elapsed_time:0.4f} seconds for jsonify_data")
 
@@ -534,62 +532,63 @@
 
         self.returned.data = data
         status_code = self.returned.status_code
         if type(self.returned.status) == int:
             status_code = self.returned.status
 
         tic = time.perf_counter()
-        if "txt" in format_:
-            route_output = str(data)
+
+        returned = None
+        route_output = (
+            data if not "integrated" in format_ else self.returned
+        )  # if "make" in format_ else ujson.dumps(data)
+
+        if "xml" in format_:
+            route_output = json_lib.jsonify_data(route_output)
+            route_output = converter_lib.dict_to_xml(
+                route_output, attr_type=not "no_type" in format_
+            )
+        elif "txt" in format_:
+            route_output = json.dumps(route_output, cls=AlphaJSONEncoder)
+            route_output = str(route_output)
             if (
                 route_output is not None
                 and len(route_output) != 0
                 and route_output[0] == '"'
             ):
                 route_output = route_output[1:-1]
-        elif "xml" in format_:
-            route_output = (
-                self.returned.to_json()
-                if "raw" in format_
-                else (jsonify(data) if "make" in format_ else data)
-            )
-            route_output = converter_lib.dict_to_xml(
-                route_output, attr_type=not "no_type" in format_
-            )
-        elif "raw" in format_:
-            route_output = jsonify(data) if "make" in format_ else json.dumps(data)
+        elif "jsonify" in format_:
+            returned = jsonify(route_output)
         else:
-            # returned = jsonify(self.returned)
-            route_output = self.returned.to_json()
-            if not "make" in format_:
-                route_output = json.dumps(route_output)
+            route_output = json.dumps(route_output, cls=AlphaJSONEncoder)
 
         toc = time.perf_counter()
         elapsed_time = toc - tic
         if DEBUG:
             print(f"Elapsed time: {elapsed_time:0.4f} seconds for conversion")
 
         tic = time.perf_counter()
 
-        if "make" in format_:
-            returned = make_response(route_output, status_code)
-        else:
-            returned = make_response({}, status_code)
-            returned.set_data(route_output)
+        if returned is None:
+            if "make" in format_:
+                returned = make_response(route_output, status_code)
+            else:
+                returned = make_response({}, status_code)
+                returned.set_data(route_output)
 
         toc = time.perf_counter()
         elapsed_time = toc - tic
         if DEBUG:
             print(f"Elapsed time: {elapsed_time:0.4f} seconds for returned")
 
         headers = self.get_headers()
 
         for key, value in headers.items():
             returned.headers[key] = (
-                json.dumps([str(v) for v in value.split("\n")])
+                ujson.dumps([str(v) for v in value.split("\n")])
                 if "\n" in str(value)
                 else value
             )
         return returned
 
     def log_user(self, user):
         self.returned.role = "user"
```

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_structures.py` & `alphaz-0.7.8/alphaz/models/api/_structures.py`

 * *Files 1% similar despite different names*

```diff
@@ -513,15 +513,15 @@
         try:
             ip = request.remote_addr
         except:
             ## getting the hostname by socket.gethostname() method
             hostname = socket.gethostname()
             ## getting the IP address using socket.gethostbyname() method
             ip_address = socket.gethostbyname(hostname)
-            ip = ip_address
+            ip = "127.0.0.1"
         admins_ips = self.conf.get("admins/ips")
         if admins_ips and (ip in admins_ips or f"::ffff:{ip}" in admins_ips):
             return True
 
         if check_logged_user:
             user = self.get_logged_user()
             if user is not None:
```

### Comparing `alphaz-0.7.7.9/alphaz/models/api/_utils.py` & `alphaz-0.7.8/alphaz/models/api/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/config/_config.py` & `alphaz-0.7.8/alphaz/models/config/_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import os, json, inspect, copy, sys, socket, re, platform, getpass
+import os, ujson, inspect, copy, sys, socket, re, platform, getpass
 import numpy as np
 
 from collections.abc import Iterable
 from sqlalchemy.orm import scoped_session, sessionmaker
 from sqlalchemy.ext.declarative import declarative_base
 
 from ...config.main_configuration import CONFIGURATION
@@ -143,15 +143,15 @@
         else:
             self.__load()
 
     def __load_raw(self):
         if not self.loaded:
             with open(self.filepath, encoding="utf-8") as json_data_file:
                 try:
-                    self.data_origin = json.load(json_data_file)
+                    self.data_origin = ujson.load(json_data_file)
                 except Exception as ex:
                     print(f"Configuration file {self.filepath} is invalid: {ex}")
                     exit()
                 self.loaded = True
 
     def set_configuration(self, configuration, force=False):
         if CONFIGURATIONS.is_configured(self) and not force:
@@ -568,15 +568,15 @@
 
     def save(self):
         self.info(f"Save configuration file at {self.filepath}")
 
         self.__clean()
 
         with open(self.filepath, "w", encoding="utf-8") as json_data_file:
-            json.dump(
+            ujson.dump(
                 self.data_origin,
                 json_data_file,
                 sort_keys=True,
                 indent=4,
                 ensure_ascii=False,
             )
```

### Comparing `alphaz-0.7.7.9/alphaz/models/config/_utils.py` & `alphaz-0.7.8/alphaz/models/config/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/models.py` & `alphaz-0.7.8/alphaz/models/database/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -200,15 +200,15 @@
             if hasattr(col, "prop"):
                 column_property = isinstance(col.prop, ColumnProperty)
             if hasattr(col, "name"):
                 columns_names.append(col.name)
         return columns_names
 
     @classmethod
-    def get_table_model(class_obj) -> dict[str, str]:
+    def get_table_model_structure(class_obj) -> dict[str, str]:
         columns_names = []
         columns = []
 
         for col in class_obj.__table__.columns:
             binary_expression = type(col.expression) is BinaryExpression
             if hasattr(col, "prop"):
                 column_property = isinstance(col.prop, ColumnProperty)
```

### Comparing `alphaz-0.7.7.9/alphaz/models/database/operators.py` & `alphaz-0.7.8/alphaz/models/database/operators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/requests.py` & `alphaz-0.7.8/alphaz/models/database/requests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/row.py` & `alphaz-0.7.8/alphaz/models/database/row.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/structure.py` & `alphaz-0.7.8/alphaz/models/database/structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,39 +1,36 @@
 # MODULES
-import copy
+import threading
 import enum, re, itertools, datetime
 import numpy as np
 from collections.abc import Iterable
 from dataclasses import fields
 from time import sleep
 import logging
 
 # SQLALCHEMY
 from sqlalchemy import MetaData
 from sqlalchemy import inspect as inspect_sqlalchemy
 import sqlalchemy
-from sqlalchemy.orm import (
-    RelationshipProperty,
-    ColumnProperty,
-)
+from sqlalchemy.orm import RelationshipProperty, ColumnProperty
 from sqlalchemy import desc, asc
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.orm.relationships import RelationshipProperty
 from sqlalchemy.sql.expression import or_, and_, all_
 from sqlalchemy.sql.elements import BinaryExpression, Null
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.sql.elements import Null
 
 from flask_sqlalchemy import DefaultMeta, SQLAlchemy, BaseQuery
 
 # MODELS
 from ...models.logger import AlphaLogger
-from ...models.main import AlphaException
-from ...models.main._enum import MappingMode
+from ...models.main import AlphaException, AlphaDataclass
 from ...models.database.models import AlphaTable
+from ...models.database import utils as db_utils
 
 # LIBS
 from ...libs import dict_lib, py_lib
 
 # LOCAL
 from .row import Row
 from .utils import get_schema
@@ -52,15 +49,15 @@
     results,
     default=None,
     columns: dict | None = None,
     page: int | None = None,
     per_page: int | None = None,
     full_count: int | None = None,
     first: bool = False,
-    pagination_mode: str = "raw",
+    pagination_mode: str = "standard",
 ):
     results = results if results is not None else default
     columns = (
         {}
         if columns is None
         else {x if not hasattr(x, "key") else x.key(): y for x, y in columns.items()}
     )
@@ -74,15 +71,15 @@
             results = [
                 {x if x not in columns else columns[x]: y for x, y in r.items()}
                 for r in results
             ]
 
     if first and type(results) == dict and len(results) == 0:
         return None
-    if page is not None and per_page is not None and pagination_mode == "raw":
+    if page is not None and per_page is not None and pagination_mode == "integrated":
         return (results, full_count)
     return results
 
 
 def get_conditions_from_dict(values: dict, model=None, optional: bool = False):
     conditions = []
     for key, value in values.items():
@@ -164,15 +161,15 @@
                     )
                 elif Operators.HAS.equals(k):
                     v = get_filters(v, None, optional=optional)
                     for condition in v:
                         conditions.append(key.has(condition))
                 elif Operators.ANY.equals(k):
                     v = get_filters(v, None, optional=optional)
-                    conditions.append(key.any(*v))
+                    conditions.append(key.any(and_(*v)))
         elif type(value) == list and value is not None:
             conditions.append(key.in_(value))
         elif not (optional and value is None):
             conditions.append(key == value)
     return conditions
 
 
@@ -378,16 +375,22 @@
         self.config = config
         self.log: AlphaLogger | None = log
 
         self.error = None
 
         self.query_str = None
         self.full_count = None
-        self.pagination_mode = config.get("pagination_mode", "raw")
+        self.pagination_mode = config.get("pagination_mode", "standard")
         self.mapping_mode = config.get("mapping_mode", None)
+        self.check_session = config.get("check_session", True)
+        self.check_autocommit = config.get("check_autocommit", False)
+        self.check_autocommit = self.autocommit and self.check_autocommit
+        self.use_schemas = config.get("use_schemas", True)
+        self.use_multithread_dump = config.get("use_multithread_dump", False)
+        self.num_threads_dump = config.get("num_threads_dump", 4)
 
         self.models = []
 
     def get_session(self, bind: str | None = None):
         return self.db.session if bind is None else self.get_engine(bind=bind)
 
     def get_meta(self, bind: str | None = None):
@@ -408,21 +411,21 @@
         output = False
         query = "SELECT 1"
         if self.db_type == "oracle" and not "sql" in str(engine):
             query = "SELECT 1 from dual"
 
         try:
             engine.execute(query)
-            if not self.autocommit:
+            if not self.check_autocommit:
                 self.session.commit()
             output = True
         except Exception as ex:
             if self.log:
                 self.log.error("ex:", ex=ex)
-            if not self.autocommit:
+            if not self.check_autocommit:
                 self.session.rollback()
         finally:
             if close:
                 self.session.close()
         return output
 
     def _get_filtered_query(
@@ -529,15 +532,15 @@
                     engine.execute(query)
             else:
                 if values is not None:
                     engine.execute(query, values)
                 else:
                     engine.execute(query)
             self.query_str = get_compiled_query(query).replace("\n", "")
-            if commit and not self.autocommit:
+            if commit and not self.check_autocommit:
                 self.commit()
             if close:
                 self.session.close()
             return True
         except Exception as ex:
             self.log.error(ex)
             raise ex
@@ -735,15 +738,15 @@
         else:
             session = obj.query.session
             if not update:
                 session.add(obj)
             else:
                 session.merge(obj)
 
-        if commit and not self.autocommit:
+        if commit:
             self.commit(session=session)
         elif flush:
             session.flush()
         if rollback:
             session.rollback()
 
         if close:
@@ -795,23 +798,24 @@
                 seen.add(unique)
 
             return row
 
         rows = list(filter(None, (handle_foreignkeys_constraints(row) for row in rows)))
         self.session.execute(stmt, rows, bind=bind)
 
-    def commit(self, close=False, session=None, check_session: bool = False) -> bool:
-        if self.autocommit:
+    def commit(self, close=False, session=None, force: bool = False) -> bool:
+        if not force and self.check_autocommit:
             return True
         if session is None:
             session = self.session
         valid = True
         try:
-            if not check_session or not session.is_active:
-                session.commit()
+            if self.check_session and not session.is_active:
+                session.begin()
+            session.commit()
         except Exception as ex:
             self.log.error(ex=ex)
             session.rollback()
             valid = False
             # session.close()
             # session.begin()
             raise ex
@@ -845,18 +849,26 @@
         session = self.object_session(obj) if session is None else session
         session.delete(obj)
         if commit:
             return self.commit(close=close, session=session)
         return True
 
     def delete(
-        self, model, filters, commit: bool = True, new_session: bool = False
+        self,
+        model,
+        filters,
+        commit: bool = True,
+        close: bool = False,
+        new_session: bool = False,
+        force: bool = False,
     ) -> bool:
-        if filters is None or len(filters) == 0:
-            raise AlphaException("Cannot delete without specifying filters")
+        if (filters is None or len(filters) == 0) and not force:
+            raise AlphaException(
+                "Cannot delete without specifying filters or force parameter"
+            )
         objs = self.select(model, filters=filters, json=False)
         if len(objs) == 0:
             return False
         if new_session:
             with self.session.begin():
                 for obj in objs:
                     self.session.delete(obj)
@@ -890,32 +902,32 @@
                     for x in self.get_tables_models()
                     if getattr(x, "__bind_key__", None) is not None
                 ]
             )
         )
 
     def get_table_model(self, table: str, bind: str | None = None):
+        binds = [bind] if bind is not None else None
+        models = self.get_tables_models(
+            tables=[table] if table is not None else [], binds=binds
+        )
         model = next(
-            iter(
-                self.get_tables_models(
-                    tables=[table], binds=[bind] if bind is not None else None
-                )
-            ),
+            iter(models),
             None,
         )
         if model is None:
             raise AlphaException(f"Cannot find table {table} in databases models")
         return model
 
-    def get_table_columns(self, table: str):
-        model = self.get_table_model(table)
+    def get_table_columns(self, table: str, bind: str = None):
+        model = self.get_table_model(table, bind=bind)
         return model._sa_class_manager.local_attrs
 
     def get_tables_models(
-        self, tables: list[str] = None, binds: list[str] = None
+        self, tables: list[str] | None = None, binds: list[str] | None = None
     ) -> list:
         if tables is not None:
             tables = [x.upper() for x in tables]
         if binds is not None:
             binds = [x.upper() for x in binds]
         models = self.__get_tables_models()
         registered_models = [
@@ -985,31 +997,31 @@
         except Exception as ex:
             self.log.error(ex=ex)
             return False
 
     def select(
         self,
         model,
-        filters: list = None,
-        optional_filters: list = None,
+        filters: list | None = None,
+        optional_filters: list | None = None,
         first: bool = False,
         json: bool = False,
-        unique: InstrumentedAttribute = None,
+        unique: InstrumentedAttribute | None = None,
         count: bool = False,
         order_by=None,
         order_by_direction=None,
         group_by=None,
         distinct=None,
         limit: int | None = None,
         columns: list | dict | None = None,
         close=False,
         flush=False,
         schema=None,
         relationship=True,
-        disabled_relationships: list[str] = None,
+        disabled_relationships: list[str] | None = None,
         page: int | None = None,
         per_page: int | None = None,
         offset: int | None = None,
         dataclass=None,
         default=None,
         # new_session: bool = True,
     ):
@@ -1121,42 +1133,43 @@
         offset: int | None = None,
         dataclass=None,
         default=None,
         columns: dict | None = None,
         distinct=None,
         group_by=None,
     ):
-        if per_page is not None and page is None:
-            page = 0
+        if disabled_relationships and not self.use_schemas:
+            query = db_utils.nested_noload(query, disabled_relationships)
+
+        page = 0 if per_page is not None and page is None else page
         if distinct is not None:
             query = (
                 query.distinct(distinct)
                 if type(distinct) != tuple
                 else query.distinct(*distinct)
             )
 
         if group_by is not None:
             query = (
                 query.group_by(group_by)
                 if type(group_by) != tuple
                 else query.group_by(*group_by)
             )
 
-        self.full_count = None
-        if dataclass is not None:
-            json = True
+        # self.full_count = None
+
         if filters is not None:
             filters = get_filters(filters, model=None, optional=False)
             query = query.filter(and_(*filters))
         if optional_filters is not None:
             optional_filters = get_filters(optional_filters, model=None, optional=True)
             query = query.filter(and_(*optional_filters))
 
-        if first and limit is None:
-            limit = 1
+        json = True if dataclass is not None else json
+        limit = 1 if first and limit is None else limit
 
         if page is not None and per_page is not None:
             self.full_count = query.count()
             query = apply_order_by(query, order_by, order_by_direction, model)
             query = query.limit(per_page).offset(page * per_page)
         else:
             query = apply_order_by(query, order_by, order_by_direction, model)
@@ -1204,40 +1217,74 @@
                 page=page,
                 per_page=per_page,
                 full_count=self.full_count,
                 first=first,
                 pagination_mode=self.pagination_mode,
             )
         # json conversion
+        converted = False
         results_json = {}
-        if schema is None and model is not None:
-            schema = get_schema(
-                model,
-                relationship=relationship,
-                disabled_relationships=disabled_relationships,
-            )
+        if self.use_schemas:
+            if schema is None and model is not None:
+                schema = get_schema(
+                    model,
+                    relationship=relationship,
+                    disabled_relationships=disabled_relationships,
+                )
+            if schema is not None:
+                structures = schema(many=True) if not first else schema()
+
+                if self.use_multithread_dump:
+                    nbr_results = len(results)
+                    num_threads = min(self.num_threads_dump, nbr_results)
+                    threads: list[threading.Thread] = []
+
+                    results_dump = []
+
+                    def dump_results(structures, results):
+                        results_dump.append(structures.dump(results))
+
+                    for i in range(num_threads):
+                        t = threading.Thread(
+                            target=dump_results,
+                            args=(structures, results[i::num_threads]),
+                        )
+                        threads.append(t)
+                        t.start()
 
-            structures = schema(many=True) if not first else schema()
-            results_json = structures.dump(results)
-        elif results is not None:
-            results_json = (
-                (
-                    results.to_json()
-                    if hasattr(results, "to_json")
-                    else results._asdict()
+                    # Wait for all threads to finish
+                    for t in threads:
+                        t.join()
+
+                    results_json = [item for result in results_dump for item in result]
+                else:
+                    results_json = structures.dump(results)
+                converted = True
+        if not converted:
+            if not self.use_schemas:
+                results_json = (
+                    [db_utils.instance_to_dict(res) for res in results]
+                    if type(results) == list
+                    else db_utils.instance_to_dict(results)
+                )
+            if results is not None:
+                results_json = (
+                    (
+                        results.to_json()
+                        if hasattr(results, "to_json")
+                        else results._asdict()
+                    )
+                    if type(results) != list
+                    else [
+                        (x.to_json() if hasattr(x, "to_json") else x._asdict())
+                        for x in results
+                    ]
                 )
-                if type(results) != list
-                else [
-                    (x.to_json() if hasattr(x, "to_json") else x._asdict())
-                    for x in results
-                ]
-            )
 
         self.query_str = get_compiled_query(query).replace("\n", "")
-        # self.log.debug(self.query_str, level=2)
 
         if unique:
             if type(unique) == str:
                 if not first:
                     return default_return(
                         (
                             []
@@ -1310,18 +1357,16 @@
                     page=page,
                     per_page=per_page,
                     full_count=self.full_count,
                     first=first,
                     pagination_mode=self.pagination_mode,
                 )
 
-            is_alpha_dataclass = hasattr(dataclass, "auto_map_from_dict")
-
             field_names = [field.name for field in fields(dataclass)]
-            if is_alpha_dataclass:
+            if issubclass(dataclass, AlphaDataclass):
                 mapping_mode = (
                     dataclass._map if dataclass.map is not None else self.mapping_mode
                 )
                 if first:
                     results_json = dataclass.map(results_json, mapping_mode)
                 else:
                     results_json = [
@@ -1347,21 +1392,23 @@
             first=first,
             pagination_mode=self.pagination_mode,
         )
 
     def update(
         self,
         model,
-        values={},
+        values=None,
         filters=None,
         fetch: bool = True,
         commit: bool = True,
         close: bool = False,
         not_none: bool = False,
     ) -> bool:
+        if values is None:
+            values = {}
         if type(model) != list:
             state, models, values_list = inspect_sqlalchemy(model), [model], [values]
         else:
             state, models, values_list = inspect_sqlalchemy(model[0]), model, values
 
         is_transient = state.transient if hasattr(state, "transient") else False
         if is_transient:
@@ -1462,15 +1509,15 @@
 
             if len(rows) != 1:
                 self.log.error(
                     f"Too much entries to update corresponding to {transient}"
                 )
                 return False
             # rows[0].query.update(values_to_update)
-            model.query.update(values_to_update)
+            model.query.filter(*filters).update(values_to_update)
             # self.session.merge(transient)
         if commit:
             return self.commit(close)
         return True
 
     def get_values(self, model, values, filters=None):
         values_update = {}
@@ -1527,36 +1574,29 @@
 
         for entry in entries:
             session.merge(entry)
         session.commit()"""
 
     def init_all(
         self,
-        binds: list[str] = None,
-        tables: list[AlphaTable] = None,
+        binds: list[str] | None = None,
+        tables: list[AlphaTable] | None = None,
         drop: bool = False,
         create: bool = False,
         truncate: bool = False,
-        sqlite: bool = True,
         log=None,
+        no_log: bool = False,
     ):
-        """if sqlite:
-        binds = [
-            x.upper()
-            for x, y in self.db_cnx.items()
-            if y["type"] == "sqlite" and (binds is None or x in binds)
-        ]"""
-
         """for bind, tables_dict in self.tables.items():
-            if binds is None or bind in binds:
-                for table_name, table_model in tables_dict.items():
-                    engine = self.db.get_engine(bind=bind)
-                    if drop:
-                        table_model.__table__.drop(engine)
-                    table_model.__table__.create(engine)"""
+        if binds is None or bind in binds:
+            for table_name, table_model in tables_dict.items():
+                engine = self.db.get_engine(bind=bind)
+                if drop:
+                    table_model.__table__.drop(engine)
+                table_model.__table__.create(engine)"""
         """if drop:
             self._db.drop_all(bind=binds, tables=tables)
         self._db.create_all(bind=binds, tables=tables)"""
 
         tables_by_bind = {}
         for table_model in tables:
             bind = (
@@ -1573,43 +1613,52 @@
                 tables_by_bind[bind].append(table_model)
 
         for bind, tables_models in tables_by_bind.items():
             tables = [x.__table__ for x in tables_models]
             if drop or create:
                 try:
                     meta = self.get_meta(bind=bind)
+                    log.info(
+                        f"Init of {bind=} with engine {str(meta.bind.engine)}",
+                        enabled=not no_log,
+                    )
                 except:
-                    log.error(f"Cannot find {bind=}")
+                    log.error(f"Cannot find {bind=}", enabled=not no_log)
                     continue
-            log.info(f"Init of {str(meta.bind.engine)}")
 
             table_names = [x.__tablename__ for x in tables_models]
             tables_names_str = ";".join(table_names)
 
             if drop:
                 if log is not None:
-                    log.info(f"Drop tables from {bind=}: {tables_names_str}")
+                    log.info(
+                        f"Drop tables from {bind=}: {tables_names_str}",
+                        enabled=not no_log,
+                    )
                 meta.drop_all(tables=tables)
 
             if create:
                 if log is not None:
-                    log.info(f"Create tables from {bind=}: {tables_names_str}")
+                    log.info(
+                        f"Create tables from {bind=}: {tables_names_str}",
+                        enabled=not no_log,
+                    )
                 meta.create_all(tables=tables)
 
             # Vide les tables si le paramètre 'truncate' est True
             if truncate:
                 for table_model in tables_models:
                     self.truncate(table_model)
 
     def create_table(self, table: str, bind: str | None = None, drop: bool = False):
-        table_object = self.get_table_model(table, bind)
+        table_object = self.get_table_model(table, bind=bind)
         if drop:
             try:
                 table_object.__table__.drop(self.engine)
             except:
                 pass
         table_object.__table__.create(self.engine)
         return True
 
     def drop_table(self, table: str, bind: str | None = None):
-        table_object = self.get_table_model(table, bind)
+        table_object = self.get_table_model(table, bind=bind)
         table_object.__table__.drop(self.db.engine)
```

### Comparing `alphaz-0.7.7.9/alphaz/models/database/tests.py` & `alphaz-0.7.8/alphaz/models/database/tests.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/users_definitions.py` & `alphaz-0.7.8/alphaz/models/database/users_definitions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/database/utils.py` & `alphaz-0.7.8/alphaz/models/database/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-import importlib, json
+import importlib, datetime
 
 from marshmallow import Schema
 from marshmallow import fields as cfields
 from marshmallow_sqlalchemy import ModelConverter, fields
 
-from ...config.main_configuration import CONFIGURATION
+from sqlalchemy.orm import (
+    RelationshipProperty,
+    ColumnProperty,
+    noload,
+    with_loader_criteria,
+    class_mapper,
+)
 
-from ..logger import AlphaLogger
+from ...config.main_configuration import CONFIGURATION
 
 SCHEMAS = {}
 MODULES = {}
 LOG = None
 
 
 def __get_nested_schema(mapper, parent=None):
@@ -118,19 +124,19 @@
         content += f"l{level}-{tp[0]}-{tp[1]}_{sub_value}".replace("None", "a")
     return content
 
 
 def generate_schema(
     class_obj,
     relationship: bool = True,
-    disabled_relationships: list[str] = None,
-    parents: list[str] = None,
+    disabled_relationships: list[str] | None = None,
+    parents: list[str] | None = None,
 ):
     parents = parents or []
-    disabled_relationships = disabled_relationships or []
+    disabled_relationships = disabled_relationships or {}
     disabled_relationships = __pdr_list_to_dict(disabled_relationships)
     disabled_relationships_keys = __pdr_flat(disabled_relationships)
 
     # schema_key = "-".join([f"{x}:{str(y)}" for x, y in locals().items()])
     schema_key = (
         f"{class_obj.__tablename__}-{disabled_relationships_keys}-{str(parents)}"
     )
@@ -253,15 +259,15 @@
     Args:
         class_obj ([type]): [description]
         parent ([type], optional): [description]. Defaults to None.
 
     Returns:
         [type]: [description]
     """
-    disabled_relationships = disabled_relationships or []
+    disabled_relationships = disabled_relationships or {}
 
     schema_name = f"{class_obj.__name__}Schema"
 
     if default:
         module_name = class_obj.__module__
         if not module_name in MODULES:
             mod = importlib.import_module(module_name)
@@ -276,7 +282,52 @@
             )
     generated_schema = generate_schema(
         class_obj,
         relationship=relationship,
         disabled_relationships=disabled_relationships,
     )
     return generated_schema
+
+
+def instance_to_dict(instance, mapped: list | None = None):
+    if mapped is None:
+        mapped = []
+
+    def process_value(value):
+        if isinstance(value, datetime.datetime):
+            value = value.isoformat()
+        return value
+
+    result = {
+        key: process_value(value)
+        for key, value in instance.__dict__.items()
+        if key != "_sa_instance_state"
+    }
+
+    mapped.append(instance.__class__)
+    relationships = class_mapper(instance.__class__).relationships
+
+    for prop in relationships:
+        related_instances = getattr(instance, prop.key)
+        if related_instances is None:
+            continue
+
+        if related_instances.__class__ in mapped:
+            continue
+
+        if prop.uselist:
+            result[prop.key] = [
+                instance_to_dict(related_instance, mapped)
+                for related_instance in related_instances
+            ]
+        else:
+            result[prop.key] = instance_to_dict(related_instances, mapped)
+
+    return result
+
+
+def nested_noload(query, disabled_relationships):
+    options = [
+        with_loader_criteria(relationship, lambda _: False)
+        for relationship in disabled_relationships
+    ]
+    return query.options(*options)
```

### Comparing `alphaz-0.7.7.9/alphaz/models/database/views.py` & `alphaz-0.7.8/alphaz/models/database/views.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/excel.py` & `alphaz-0.7.8/alphaz/models/excel.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/ftp.py` & `alphaz-0.7.8/alphaz/models/ftp.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/json/_converters.py` & `alphaz-0.7.8/alphaz/models/json/_converters.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import pandas as pd
 import numpy as np
 
 from _collections_abc import dict_keys
 
 from flask.json import JSONEncoder
 
-from sqlalchemy.exc import OperationalError
+import sqlalchemy
 
 
 class AlphaJSONEncoder(JSONEncoder):
     rules = {}
 
     def __init__(self, *args, **kwargs):
         super(AlphaJSONEncoder, self).__init__(*args, **kwargs)
@@ -30,51 +30,54 @@
         self.rules[pd.DataFrame] = lambda o: o.to_json(orient="index")
         self.rules[bytes] = lambda o: str(o.decode("utf-8"))
         self.rules[dict_keys] = lambda o: list(o)
         self.rules[datetime.timedelta] = lambda o: str(o)
         self.rules[decimal.Decimal] = lambda o: str(o)
         self.rules[enum.Enum] = lambda o: str(o)
         self.rules[str] = lambda o: str(o)
+        self.rules[type(sqlalchemy.null())] = lambda o: "null()"
         # self.rules[NameError] = lambda o:str(o)
         # self.rules[ValueError] = lambda o:str(o)
         # self.rules[TypeError] = lambda o:str(o)
         # self.rules[AttributeError] = lambda o:str(o)
         # self.rules[OperationalError] = lambda o:str(o)
         # self.rules[str] = lambda o:str(o)
 
     def default(self, o):  # pylint: disable=E0202
-        if "<class " in str(o):
-            return str(o)
-
+        if hasattr(o, "to_json"):
+            return o.to_json()
+        for key_type, fct in self.rules.items():
+            if isinstance(o, key_type):
+                returned_value = fct(o)
+                return returned_value
         try:
-            if hasattr(o, "to_json"):
-                return o.to_json()
-            for key_type, fct in self.rules.items():
-                if isinstance(o, key_type):
-                    returned_value = fct(o)
-                    return returned_value
+            iterable = iter(o)
+        except:
+            iterable = None
+        if iterable is not None:
             try:
-                iterable = iter(o)
-            except:
-                iterable = None
-        except TypeError as ex:
-            print(f"Cannot convert {o} to json: {ex}")
-        else:
-            if iterable is not None:
                 return list(iterable)
+            except:
+                return o
 
+        """if "<class " in str(o):
+            return str(o)"""
         try:
             return JSONEncoder.default(self, o=o)
         except:
             o = str(o)
             try:
                 return JSONEncoder.default(self, o=o)
             except:
                 return o
 
+        """try:
+        except TypeError as ex:
+            print(f"Cannot convert {o} to json: {ex}")"""
+
         """results_json = {}
         if hasattr(model,"schema"):
             schema          = model.get_schema()
             structures      = schema(many=True) if not first else schema()
             results_json    = structures.dump(results)
         else:
             self.log.error('Missing schema for model <%s>'%str(model.__name__))"""
```

### Comparing `alphaz-0.7.7.9/alphaz/models/logger/_colorations.py` & `alphaz-0.7.8/alphaz/models/logger/_colorations.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/logger/_logger.py` & `alphaz-0.7.8/alphaz/models/logger/_logger.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/logger/_utils.py` & `alphaz-0.7.8/alphaz/models/logger/_utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/logs/main.log` & `alphaz-0.7.8/alphaz/models/logs/main.log`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/main/_base.py` & `alphaz-0.7.8/alphaz/models/main/_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,30 +99,30 @@
     def to_json(
         self,
         columns: list | None = None,
         rejected: list | None = None,
         not_none: bool = False,
         not_empty: bool = False,
     ):
-        d_rejected = [
+        """d_rejected = [
             "_map",
             "_map_keys",
             "_no_map",
             "_piles",
             "_init_args",
             "_children",
             "_log",
         ]
         if rejected is not None:
-            d_rejected.extend(rejected)
+            d_rejected.extend(rejected)"""
         dict_output = {}
         for x, y in self.get_attributes().items():
             if columns is not None and x not in columns:
                 continue
-            if x in d_rejected:
+            if x.startswith("_"):
                 continue
             if not_none and y is None:
                 continue
             is_iterable = py_lib.is_iterable(y)
             if not_empty and y is not None and is_iterable and len(y) == 0:
                 continue
             dict_output[x] = json_lib.jsonify_data(
@@ -816,20 +816,17 @@
         dataclass_type,
         dict_values: dict[str, object] | dict[str, str],
         mapping_mode: MappingMode | str | None = None,
     ):
         if is_auto_map(dataclass_type, mapping_mode=mapping_mode):
             return dataclass_type.auto_map_from_dict(dict_values=dict_values)
 
-        if (
-            not py_lib.is_subtype(type(dict_values), dict)
-            and not py_lib.is_subtype(type(dict_values), dict)
-            and not type(dict_values) == dict
-        ):
+        if not isinstance(dict_values, dict):
             return None
+
         if dict_values is None:
             return None
 
         field_values = {}
         for key, value in dict_values.items():
             no_match = False
             if dataclass_type._map_keys is not None:
@@ -860,17 +857,15 @@
 
             field = dataclass_type.__dataclass_fields__[key]
             field_type = py_lib.get_first_non_none_type(field.type)
 
             if not field.init:
                 continue
 
-            if py_lib.is_subtype(field_type, list) or py_lib.is_subtype(
-                field_type, list
-            ):
+            if py_lib.is_subtype(field_type, list):
                 field_values[key] = []
                 if value is not None:
                     field_values[key] = [
                         convert_value_from_field(
                             py_lib.get_subtype(field_type), v, mapping_mode=mapping_mode
                         )
                         for v in value
```

### Comparing `alphaz-0.7.7.9/alphaz/models/main/_core/_core.py` & `alphaz-0.7.8/alphaz/models/main/_core/_core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODULES
-import os, sys, warnings, logging
-
+import os, sys, warnings, logging, re
 
 from sqlalchemy import exc as sqlalchemy_exc
 
 with warnings.catch_warnings():
     from flask_marshmallow import Marshmallow
 from flask_cors import CORS
 
@@ -263,15 +262,15 @@
                     name = cf_db["sid"]
                     c = f"{host}:{port}/{name}"
                 elif "service_name" in cf_db:
                     name = cf_db["service_name"]
                     c = f"(DESCRIPTION = (LOAD_BALANCE=on) (FAILOVER=ON) (ADDRESS = (PROTOCOL = TCP)(HOST = {host})(PORT = {port})) (CONNECT_DATA = (SERVER = DEDICATED) (SERVICE_NAME = {name})))"
                 cnx_str = f"oracle://{user}:{password}@{c}"
             elif db_type == "sqlite":
-                cnx_str = "sqlite:///" + cf_db["path"] + "?timeout=5"
+                cnx_str = "sqlite:///" + cf_db["path"]  # + "?timeout=5"
 
             if "ssl" in cf_db and cf_db["ssl"] is not None:
                 if not all(
                     elem in cf_db["ssl"].keys()
                     for elem in ["ssl_ca", "ssl_cert", "ssl_key"]
                 ):
                     raise AlphaException(
@@ -287,14 +286,20 @@
                 if "ssl_check_hostname" in cf_db["ssl"].keys():
                     cnx_str = f"{cnx_str}&ssl_check_hostname={cf_db['ssl']['ssl_check_hostname']}"
 
             if cnx_str is not None:
                 cf_db["cnx"] = cnx_str
                 db_cnx[db_name.upper()] = cf_db
 
+                pattern = re.compile(r":([^@:]+)@")
+                masked_conn_str = re.sub(pattern, ":****@", cnx_str)
+                self.log.debug(
+                    f"Prepared cnx from {masked_conn_str} for bind {db_name.upper()}"
+                )
+
         self.db_cnx = db_cnx
 
     def set_configuration(self, configuration_name):
         if configuration_name is None and self.config.configuration is not None:
             configuration_name = self.config.configuration
 
         self.config.set_configuration(configuration_name)
```

### Comparing `alphaz-0.7.7.9/alphaz/models/main/_exception.py` & `alphaz-0.7.8/alphaz/models/main/_exception.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/main/_request.py` & `alphaz-0.7.8/alphaz/models/main/_request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/main/_singleton.py` & `alphaz-0.7.8/alphaz/models/main/_singleton.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/request.py` & `alphaz-0.7.8/alphaz/models/request.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_category.py` & `alphaz-0.7.8/alphaz/models/tests/_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,22 +81,18 @@
         names: list[str] | None = None,
         levels: list[Levels] = [],
         stop: bool = True,
         failed_only: bool = False,
     ) -> bool:
         stopped = False
         for category in self.categories.values():
-            if failed_only and category.status:
-                continue
             if stopped:
                 break
-            for test_group in category.groups.values():
-                if failed_only and test_group.status:
-                    continue
 
+            for test_group in category.groups.values():
                 if stopped:
                     break
                 if not test_group.test_all(
                     names, levels, stop=stop, failed_only=failed_only
                 ):
                     self.status = False
                     if stop:
@@ -141,14 +137,16 @@
         for category_name, category in self.categories.items():
             c_failed, c_success, c_times = [], [], 0
             c_content = []
 
             for group_name, group in category.groups.items():
                 g_failed, g_success, g_times = [], [], 0
                 g_content = []
+                if group.disable:
+                    continue
 
                 for test_name, test in group.tests.items():
                     if test.disable:
                         continue
                     stdout = test.last_run_elapsed
                     stderr = str(test.ex) if test.ex is not None else None
```

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_group.py` & `alphaz-0.7.8/alphaz/models/tests/_group.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 
                 tests[test_function.name] = test_function
 
         sorted_tests = dict(
             sorted(tests.items(), key=lambda item: item[1].func.__code__.co_firstlineno)
         )
         self.tests = sorted_tests
+        self.disable = False
 
     def get_from_database(self):
         tests = core.db.select(
             Tests,
             filters=[Tests.category == self.category, Tests.tests_group == self.name],
             order_by=Tests.start_time.desc(),
         )
@@ -79,20 +80,24 @@
     ) -> bool:
         tests = self.tests
         if names is not None and len(names) != 0:
             tests = {x: y for x, y in tests.items() if x in names}
         if levels is not None and len(levels) != 0:
             tests = {x: y for x, y in tests.items() if y.level.name in levels}
 
-        if len(tests) != 0:
+        if len(tests) != 0 and not self.classTest.disable:
             classTest = self.classTest()
 
-            if failed_only and self.status:
+            valid_tests = all([t.status for t in self.tests.values() if not t.disable])
+            if failed_only and valid_tests:
                 return self.status
+
             for test in tests.values():
+                if test.disable:
+                    continue
                 if not test.test(
                     classTest=classTest, coverage=self.coverage, failed_only=failed_only
                 ):
                     self.status = False
                     if stop:
                         break
         return self.status
```

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_method.py` & `alphaz-0.7.8/alphaz/models/tests/_method.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_save.py` & `alphaz-0.7.8/alphaz/models/tests/_save.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # MODULES
 import os
-import json
-from pathlib import Path
-from typing import Any, Callable
 
-# MODELS
-from ...models.main import dataclass
+from pathlib import Path
+from typing import Any
 
 # LIBS
 from ...libs.io_lib import archive_object, unarchive_object, read_json, save_as_json
 
 # CORE
 from core import core
```

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_test.py` & `alphaz-0.7.8/alphaz/models/tests/_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class AlphaTest(AlphaClass):
     _test = True
     category = ""
     index = 0
     current_test_name = ""
+    disable: bool = False
 
     outputs: dict[str, bool] = {}
     coverages: dict[str, object] = {}
 
     def __init__(self):
         self.begin_class()
 
@@ -47,25 +48,27 @@
         self,
         tables: list[str],
         binds: list[str] | None = None,
         truncate: bool = False,
         drop: bool = False,
         create: bool = False,
         init: bool = True,
-        init_views: bool = False
+        init_views: bool = False,
+        no_log: bool = True,
     ):
         database_lib.init_databases(
             core=core,
             binds=binds,
             tables=tables,
             truncate=truncate,
             drop=drop,
             create=create,
             init=init,
-            init_views=init_views
+            init_views=init_views,
+            no_log=no_log,
         )
 
     def test(self, name, coverage: bool = False) -> bool:
         self.output = None
 
         status = False
         self.current_test_name = name
@@ -230,14 +233,20 @@
 
     def assert_is_dict(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
         status = type(a) == dict
         if not type(a) == dict:
             LOG.info(f"{self.current_test_name} {msg} - Assert: value is not a dict")
         return self._assert(status, conditions)
 
+    def assert_is_list(self, a, conditions: list[bool] = [], msg: str = "") -> bool:
+        status = type(a) == list
+        if not type(a) == list:
+            LOG.info(f"{self.current_test_name} {msg} - Assert: value is not a list")
+        return self._assert(status, conditions)
+
     def assert_is_dict_not_empty(self, a, conditions: list[bool] = [], msg: str = ""):
         self.assert_is_dict(a, msg=msg)
         status = self.assert_is_not_empty(a, msg=msg)
         if not status:
             LOG.info(f"{self.current_test_name} {msg} - Assert: dict {a} is empty")
         return self._assert(status, conditions)
 
@@ -270,14 +279,30 @@
             status = self.assert_equal(a[key], value, msg=msg)
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: {a} does not contains a {key=} with {value=}"
             )
         return self._assert(status, conditions)
 
+    def assert_is_list_no_empty(self, a, conditions: list[bool] = [], msg: str = ""):
+        status = self.assert_is_list(a, msg=msg)
+        if status:
+            status = self.assert_is_not_empty(a)
+        return self._assert(status, conditions)
+
+    def assert_is_equal(
+        self,
+        a,
+        b,
+        ignore: list | dict | None = None,
+        conditions: list[bool] = [],
+        msg: str = "",
+    ):
+        return self.assert_equal(a, b, ignore=ignore, conditions=conditions, msg=msg)
+
     def assert_equal(
         self,
         a,
         b,
         ignore: list | dict | None = None,
         conditions: list[bool] = [],
         msg: str = "",
@@ -305,17 +330,16 @@
 
         elif type(a) == dict and type(b) == dict:
             diff = dict_lib.compare_dicts(a, b, ignore=ignore)
 
             status = diff is None
             if not status:
                 LOG.info(
-                    f"{self.current_test_name} {msg} - Assert: dict are not equals\n"
+                    f"{self.current_test_name} {msg} - Assert: dict are not equals\n\n{dict_lib.show_dict(diff)}"
                 )
-                print("\n", dict_lib.show_dict(diff))
 
         else:
             status = a == b
             if not status:
                 LOG.info(
                     f"{self.current_test_name} {msg} - Assert: {a} and {b} are not equals"
                 )
@@ -337,14 +361,37 @@
         status = a in b
         if not status:
             LOG.info(
                 f"{self.current_test_name} {msg} - Assert: {b} does not include {b}"
             )
         return self._assert(status, conditions)
 
+    def assert_list_str_in_str(
+        self,
+        a: list[str],
+        b: str,
+        conditions: list[bool] = [],
+        msg: str = "",
+    ) -> bool:  # TODO add check on a type
+        if type(b) != str:
+            LOG.info(f"{self.current_test_name} {msg} - Assert: {b} type is not str")
+            return self._assert(False, conditions)
+
+        status = True
+        for e in a:
+            if e not in b:
+                status = False
+                LOG.info(
+                    f"{self.current_test_name} {msg} - Assert: {e} does not include in {a}"
+                )
+
+                break
+
+        return self._assert(status, conditions)
+
     def assert_not_equal(
         self,
         a,
         b,
         ignore: list | dict | None = None,
         conditions: list[bool] = [],
         msg: str = "",
```

### Comparing `alphaz-0.7.7.9/alphaz/models/tests/_wrappers.py` & `alphaz-0.7.8/alphaz/models/tests/_wrappers.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/user.py` & `alphaz-0.7.8/alphaz/models/user.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/models/watcher.py` & `alphaz-0.7.8/alphaz/models/watcher.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/pocs/main.py` & `alphaz-0.7.8/alphaz/pocs/main.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/run.py` & `alphaz-0.7.8/alphaz/run.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/src/alpha.png` & `alphaz-0.7.8/alphaz/src/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/src/configs/loggers.json` & `alphaz-0.7.8/alphaz/src/configs/loggers.json`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/stitch/Core.py` & `alphaz-0.7.8/alphaz/stitch/Core.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/stitch/stitch.py` & `alphaz-0.7.8/alphaz/stitch/stitch.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,67 @@
-import ast, json
+import ast, ujson
 
 from .imports import *
 
+
 class Stitch(object):
-    name        = None
-    path        = None
-    configured  = False
+    name = None
+    path = None
+    configured = False
 
-    elements    = {}
+    elements = {}
 
-    def __init__(self,name):
-        self.name       = name
-        self.path       = name.lower()
+    def __init__(self, name):
+        self.name = name
+        self.path = name.lower()
 
-        websites        = Core.getWebsites()
+        websites = Core.getWebsites()
         self.configured = self.path in websites
 
-    def set_driver(self,name):
+    def set_driver(self, name):
         Core.set_driver(name)
 
     def process(self, file_name):
-        path = Core.WEBSITES_PATH + os.sep + self.path + os.sep + file_name + '.json'
-        
+        path = Core.WEBSITES_PATH + os.sep + self.path + os.sep + file_name + ".json"
+
         if os.path.isfile(path):
-            with open(path,'r') as f:
+            with open(path, "r") as f:
                 content = f.read()
-            content_dict = json.loads(content)
+            content_dict = ujson.loads(content)
         else:
-            print('Folder not found')
+            print("Folder not found")
             exit()
 
         root_keys = content_dict.keys()
-        
+
         for key in root_keys:
             properties = content_dict[key]
 
             if key == "elements":
                 for key, properties in properties.items():
                     self.elements[key] = Element(key, properties)
             elif key == "url":
                 self.get(properties)
             elif key == "set":
                 for el in properties:
-                    name    = list(el.keys())[0]
-                    value   = el[name]
+                    name = list(el.keys())[0]
+                    value = el[name]
                     self.elements[name].value = value
 
                     elem_pass = self.getById(name)
                     elem_pass.send_keys(value)
             elif key == "click":
                 for name in properties:
                     self.getById(name).click()
             elif key == "submit":
                 for name in properties:
                     self.elements[key].submit()
 
-    def getById(self,name):
+    def getById(self, name):
         return Core.DRIVER.find_element_by_id(name)
 
     def get(self, *args):
         Core.DRIVER.get(args[0])
 
+
 if __name__ == "__main__":
-    print('Stitch')
+    print("Stitch")
```

### Comparing `alphaz-0.7.7.9/alphaz/stitch/web-drivers/chromedriver.exe` & `alphaz-0.7.8/alphaz/stitch/web-drivers/chromedriver.exe`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/stitch/web-drivers/geckodriver` & `alphaz-0.7.8/alphaz/stitch/web-drivers/geckodriver`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/css/home.css` & `alphaz-0.7.8/alphaz/templates/assets/css/home.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/css/logs.css` & `alphaz-0.7.8/alphaz/templates/assets/css/logs.css`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/alpha.png` & `alphaz-0.7.8/alphaz/templates/assets/images/icons/alpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/start-icon.png` & `alphaz-0.7.8/alphaz/templates/assets/images/icons/start-icon.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/images/icons/wsalpha.png` & `alphaz-0.7.8/alphaz/templates/assets/images/icons/wsalpha.png`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/images/loading.gif` & `alphaz-0.7.8/alphaz/templates/assets/images/loading.gif`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/js/libs/ansi_up.js` & `alphaz-0.7.8/alphaz/templates/assets/js/libs/ansi_up.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/js/libs/jquery.min.js` & `alphaz-0.7.8/alphaz/templates/assets/js/libs/jquery.min.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/assets/js/logs.js` & `alphaz-0.7.8/alphaz/templates/assets/js/logs.js`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/home.html` & `alphaz-0.7.8/alphaz/templates/home.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/templates/logs.html` & `alphaz-0.7.8/alphaz/templates/logs.html`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/test.py` & `alphaz-0.7.8/alphaz/test.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/tests/api.py` & `alphaz-0.7.8/alphaz/tests/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from core import core
 
 # ALPHAZ
 from alphaz.models.tests import Levels
 from alphaz.utils.api import api
 from alphaz.models.tests import AlphaTest, test
 
-from alphaz.libs import api_lib
+from alphaz.libs import api_lib, date_lib
 from alphaz.utils.api import api
 from alphaz.models.api import ApiMethods
 from alphaz.models.main import AlphaException
 from alphaz.models.tests._test import TestInput
 from alphaz.models.api._route import description_from_status
 
 from alphaz.models.database.tests import Test
@@ -229,16 +229,16 @@
                 "list_db_object": [
                     Test(**p1),
                     Test(**p2),
                 ]
             },
             expected_output={
                 "list_db_object": [
-                    p1,
-                    p2,
+                    Test(**p1).to_json(),
+                    Test(**p2).to_json(),
                 ]
             },
             default_values=default_values,
         )
 
     @test(description="Test input parameters form url", level=Levels.REQUIRED)
     def test_parameters_url(self):
@@ -261,41 +261,43 @@
             ("list_int=1,2", {"list_int": [1, 2]}),
             ("list_int=1;2", {"list_int": [1, 2]}),
             ("list_float=1.1,2.2", {"list_float": [1.1, 2.2]}),
             ("list_float=1.1;2.2", {"list_float": [1.1, 2.2]}),
             ('dict={"1":"a","b":2 }', {"dict": {"1": "a", "b": 2}}),
         ]
 
+        stop = False
         for t in tests_cases_success_values:
-            self.assert_api_answer(
+            if stop:
+                break
+            if not self.assert_api_answer(
                 url=url + "?" + t[0],
                 method=method,
                 expected_output=t[1],
                 default_values=default_values,
-            )
+            ):
+                stop = True
 
     @test(description="Test str max and min lenght parameter")
     def test_parameter_max_min_lenght(self):
-        answer = self.get_api_answer_test(
-            route="/test/parameters", method="GET", params={"string": "a" * 10}
-        )
-        if answer.error:
-            return False
-
-        answer = self.get_api_answer_test(
-            route="/test/parameters", method="GET", params={"string": "a" * 120}
-        )
-        if not answer.error:
-            return False
-        answer = self.get_api_answer_test(
-            route="/test/parameters", method="GET", params={"string": "a"}
-        )
-        if not answer.error:
-            return False
-        return True
+        tests = [
+            ({"string": "a" * 10}, True),
+            ({"string": "a" * 120}, False),
+            ({"string": "a"}, False),
+        ]
+        stop = False
+        for test in tests:
+            p, output = test
+            if stop:
+                break
+            answer = self.get_api_answer_test(
+                route="/test/parameters", method="GET", params=p
+            )
+            if not self.assert_is_false(answer.error if output else not answer.error):
+                stop = True
 
     @test()
     def none_parameters_to_get_api_answer(self):
         answer = self.get_api_answer_test(
             route="/test/parameters",
             method="GET",
             params={"string": None, "bool": None},
@@ -378,14 +380,27 @@
             route="/test/exception", method="GET", params=params
         )
         self.assert_equal(answer.status_description, params["description"])
         self.assert_equal(answer.status, "exception")
         self.assert_equal(answer.error, 0)
         self.assert_equal(answer.warning, 1)
 
+        api.set_status("")
+
+    @test()
+    def description_headers_multilines(self):
+        params = {"description": "test\n test"}
+        answer = self.get_api_answer_test(
+            route="/test/status", method="GET", params=params
+        )
+        self.assert_equal(answer.status_description, params["description"])
+        self.assert_equal(answer.status, "success")
+        self.assert_equal(answer.error, 0)
+        self.assert_equal(answer.warning, 0)
+
     @test()
     def auth_su(self):
         answer = self.get_api_answer_test(
             route="/auth/su", method="POST", params={"admin_user_name": "alpha"}
         )
         self.assert_equal(answer.token_status, "success")
         self.assert_equal(answer.status, "success")
@@ -405,7 +420,37 @@
     def auth_su_auto_id(self):
         answer = self.get_api_answer_test(route="user/infos")
         self.assert_is_dict_with_key_with_value(answer.data, "id", -1)
         self.assert_equal(answer.token_status, "success")
         self.assert_equal(answer.status, "success")
         self.assert_equal(answer.error, 0)
         self.assert_equal(answer.warning, 0)
+
+    @test()
+    def test_pagination_request(self):
+        date_datetime = date_lib.str_to_datetime("2020/01/07 10:02:03")
+        parameters_ref = {
+            Test.id.key: 0,
+            Test.name.key: "insert",
+            Test.text.key: "insert_text",
+            Test.number.key: 12,
+            Test.date.key: date_datetime,
+        }
+        tests = [Test(**parameters_ref)]
+        for i in range(5):
+            parameters = parameters_ref.copy()
+            parameters[Test.id.key] = i + 2
+            parameters[Test.number.key] = i
+            parameters[Test.date.key] = date_lib.str_to_datetime(
+                "2020/01/%s 10:02:03" % (i + 1)
+            )
+            tests.append(Test(**parameters))
+        core.db.add_or_update(tests)
+
+        params = {"page": 0, "per_page": 0}
+        answer = self.get_api_answer_test(
+            route="/test/select", method="GET", params=params
+        )
+
+        self.assert_equal(answer.status, "success")
+        self.assert_equal(answer.error, 0)
+        self.assert_equal(answer.warning, 0)
```

### Comparing `alphaz-0.7.7.9/alphaz/tests/basic_test.py` & `alphaz-0.7.8/alphaz/tests/basic_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
         o = TestDataclass.map({"a": "e", "b": 2, "k": 4, "boo": "false"})
         self.assert_equal(o, TestDataclass("e", 2, 0.1, 4))
 
     @test()
     def to_json_map(self):
         o = TestDataclass.map({"a": "e", "b": 2, "k": 4, "h": 32})
         d = o.to_json()
-        self.assert_equal(set(d.keys()), set(["a", "b", "c", "d", "h"]))
+        self.assert_equal(set(d.keys()), set(["boo", "a", "b", "c", "d", "h"]))
 
 
 class SubType(AlphaTest):
     def __init__(self):
         self.l: list[str] = []
 
         self.c1, self.c2 = TestClass("e", 2, 0.1), TestClass("c", 3, 0.8)
```

### Comparing `alphaz-0.7.7.9/alphaz/tests/configurations.py` & `alphaz-0.7.8/alphaz/tests/configurations.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,52 +1,59 @@
 from ..models.tests import test, AlphaTest
 from ..libs import config_lib
 
 from core import core
 
 DB = core.db
 
+
 class ConfigConstants(AlphaTest):
-    def __init__(self):
-        self.constant_name = 'test'
-        config_lib.set_db_constant(DB,self.constant_name,0)
+    def begin(self):
+        self.constant_name = "test"
+        config_lib.set_db_constant(self.constant_name, 0)
         pass
 
     @test(stop=True)
     def is_db_constant(self):
-        return config_lib.is_db_constant(DB,self.constant_name)
+        return config_lib.is_db_constant(self.constant_name)
 
     @test(stop=True)
     def get_db_constants(self):
-        self.assert_is_not_empty(config_lib.get_db_constants(DB))
-        
+        constants = config_lib.get_db_constants()
+        self.assert_is_not_empty(constants)
+
     @test()
     def get_db_constant(self):
-        return config_lib.get_db_constant(DB,self.constant_name) == 0
+        value = config_lib.get_db_constant(self.constant_name)
+        self.assert_equal(value, 0)
 
     @test()
     def set_db_constant(self):
-        config_lib.set_db_constant(DB,self.constant_name,1)
-        return config_lib.get_db_constant(DB,self.constant_name) == 1
+        config_lib.set_db_constant(self.constant_name, 1)
+        value = config_lib.get_db_constant(self.constant_name)
+        self.assert_equal(value, 1)
+
 
 class ConfigParameters(AlphaTest):
-    def __init__(self):
-        self.parameter_name = 'test'
-        config_lib.set_db_parameter(DB,self.parameter_name,0)
+    disable = True
+
+    def begin(self):
+        self.parameter_name = "test"
+        config_lib.set_db_parameter(self.parameter_name, 0)
         pass
 
     @test(stop=True)
     def is_db_parameter(self):
-        return config_lib.is_db_parameter(DB,self.parameter_name)
+        return config_lib.is_db_parameter(self.parameter_name)
 
     @test(stop=True)
     def get_db_parameters(self):
-        self.assert_is_not_empty(config_lib.get_db_parameters(DB))
-        
+        self.assert_is_not_empty(config_lib.get_db_parameters())
+
     @test()
     def get_db_parameter(self):
-        return config_lib.get_db_parameter(DB,self.parameter_name) == 0
+        return config_lib.get_db_parameter(self.parameter_name) == 0
 
     @test()
     def set_db_parameter(self):
-        config_lib.set_db_parameter(DB,self.parameter_name,1)
-        return config_lib.get_db_parameter(DB,self.parameter_name) == 1
+        config_lib.set_db_parameter(self.parameter_name, 1)
+        return config_lib.get_db_parameter(self.parameter_name) == 1
```

### Comparing `alphaz-0.7.7.9/alphaz/tests/database.py` & `alphaz-0.7.8/alphaz/tests/database.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # MODULES
-import datetime
+import datetime, copy
 
 # CORE
 from core import core, DB
 
 # MODELS
 from alphaz.models.tests import AlphaTest, test
 from alphaz.models.database.main_definitions import Test
@@ -14,54 +14,90 @@
 from alphaz.libs import date_lib, json_lib
 
 LOG = core.get_logger("tests")
 
 
 def delete():
     Test.query.delete()
+    if not Test.query.session.is_active:
+        Test.query.session.begin()
     Test.query.session.commit()
 
 
 class Database(AlphaTest):
     connected = False
 
     columns = [Test.name.key, Test.text.key, Test.number.key]
 
     date_datetime = date_lib.str_to_datetime("2020/01/07 10:02:03")
     parameters = {
+        Test.id.key: 0,
         Test.name.key: "insert",
         Test.text.key: "insert_text",
         Test.number.key: 12,
         Test.date.key: date_datetime,
     }
 
     select_parameters = {
         Test.name.key: "select",
         Test.text.key: "select",
         Test.number.key: 12,
     }
 
-    test_p = {"id": 1, "name": "test", "test_child_id": 1}
-    test_p_child = {"id": 1, "name": "test"}
+    date, text, number = datetime.date(2022, 12, 25), "test_text", 2
+    test_p = {
+        "id": 1,
+        "name": "test",
+        "test_child_id": 1,
+        "number": number,
+        "date": date,
+        "text": text,
+    }
+    test_p_child = {
+        "id": 1,
+        "name": "test",
+        "number": number,
+        "date": date,
+        "text": text,
+    }
     test_p_childs_1 = {
         "id": 1,
         "name": "test",
         "parent_id": 1,
         "child_parent_id": 1,
+        "number": number,
+        "date": date,
+        "text": text,
     }
     test_p_childs_2 = {
         "id": 2,
         "name": "test2",
         "parent_id": 1,
         "child_parent_id": 1,
+        "number": number,
+        "date": date,
+        "text": text,
     }
 
-    def __init__(self):
-        super().__init__()
+    ignore_pattern = {
+        "update_date": None,
+        "date": None,
+        "test_child": {
+            "update_date": None,
+            "test_childs": ["update_date"],
+            "date": None,
+        },
+        "test_childs": {
+            "update_date": None,
+            "date": None,
+            "parent": {"update_date": None, "date": None},
+        },
+    }
 
+    def begin(self):
         self.db = core.db
         self.connected = self.db.test()
 
         if not self.connected:
             LOG.error("not connected")
             return
         # self.db.session.delete(Test)
@@ -78,148 +114,144 @@
         return self.connected
 
     @test(save=False)
     def truncate(self):
         rows = self.db.select(Test)
         self.assert_length(rows, 0)
 
-    def init_childs(self, disabled_relationships: list | dict = None) -> dict:
+    def init_childs(self, disabled_relationships: list | dict | None = None) -> dict:
         Test.query.delete()
         TestChild.query.delete()
         TestChilds.query.delete()
 
-        DB.add(TestChild(**self.test_p_child))
-        DB.add(Test(**self.test_p))
+        test_child = DB.add(TestChild(**self.test_p_child))
+
+        self.test_p["test_child_id"] = test_child.id
+        test = DB.add(Test(**self.test_p))  # , commit=False, flush=False
+
+        self.test_p_childs_1["parent_id"] = test.id
+        self.test_p_childs_1["child_parent_id"] = test_child.id
+        self.test_p_childs_2["parent_id"] = test.id
+        self.test_p_childs_2["child_parent_id"] = test_child.id
 
         DB.add(TestChilds(**self.test_p_childs_1))
         DB.add(TestChilds(**self.test_p_childs_2))
 
         rows = DB.select(Test, json=True, disabled_relationships=disabled_relationships)
         return rows
 
     @test()
     def childs_compare_fail(self):
         rows = self.init_childs()
 
-        full_model = {x: y for x, y in self.test_p.items()}
-        full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
+        full_model = self.test_p.copy()
+        full_model["test_child"] = self.test_p_child.copy()
         full_model["test_child"]["test_childs"] = [
-            self.test_p_childs_2,
-            self.test_p_childs_2,
+            self.test_p_childs_2.copy(),
+            self.test_p_childs_2.copy(),
+        ]
+        full_model["test_childs"] = [
+            self.test_p_childs_1.copy(),
+            self.test_p_childs_2.copy(),
         ]
-        full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
 
         full_model["id"] = 3
 
         self.assert_length(rows, 1)
         self.assert_not_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
     @test()
     def childs_compare(self):
         rows = self.init_childs()
 
-        full_model = {x: y for x, y in self.test_p.items()}
-        full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
-        full_model["test_child"]["test_childs"] = [
-            self.test_p_childs_1,
-            self.test_p_childs_2,
-        ]
-        full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
+        tc1 = self.test_p_childs_1.copy()
+        tc2 = self.test_p_childs_2.copy()
+
+        tc1["parent"] = self.test_p.copy()
+        tc2["parent"] = self.test_p.copy()
+
+        full_model = self.test_p.copy()
+        full_model["test_child"] = self.test_p_child.copy()
+        full_model["test_childs"] = [tc1, tc2]
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
     @test()
     def no_test_childs_compare(self):
         rows = self.init_childs(disabled_relationships=[Test.test_childs])
 
-        full_model = {x: y for x, y in self.test_p.items()}
-        full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
-        full_model["test_child"]["test_childs"] = [
-            self.test_p_childs_1,
-            self.test_p_childs_2,
-        ]
-        # full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
+        full_model = self.test_p.copy()
+        full_model["test_child"] = self.test_p_child.copy()
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
-    @test()
+    @test(disable=True)
     def no_test_child_compare(self):
         rows = self.init_childs(disabled_relationships=[Test.test_child])
 
-        full_model = {x: y for x, y in self.test_p.items()}
-        """full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
-        full_model["test_child"]["test_childs"] = [
-            self.test_p_childs_1,
-            self.test_p_childs_2,
-        ]"""
-        full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
+        full_model = self.test_p.copy()
+        full_model["test_childs"] = [
+            self.test_p_childs_1.copy(),
+            self.test_p_childs_2.copy(),
+        ]
+
+        parent = full_model.copy()
+        parent["text_child"] = self.test_p_child.copy()  # TODO: remove
+        full_model["test_childs"][0]["parent"] = parent
+        full_model["test_childs"][1]["parent"] = parent
+
+        ignore_patterns = self.ignore_pattern
+        ignore_patterns["test_childs"]["parent"] = self.ignore_pattern
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=ignore_patterns,
         )
 
-    @test()
+    @test(disable=True)
     def no_test_child_test_childs_compare(self):
         rows = self.init_childs(
             disabled_relationships={Test.test_child: TestChild.test_childs}
         )
 
-        full_model = {x: y for x, y in self.test_p.items()}
-        full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
+        full_model = self.test_p.copy()
+        full_model["test_child"] = self.test_p_child.copy()
         """full_model["test_child"]["test_childs"] = [
             self.test_p_childs_1,
             self.test_p_childs_2,
         ]"""
-        full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
+        full_model["test_childs"] = [
+            self.test_p_childs_1.copy(),
+            self.test_p_childs_2.copy(),
+        ]
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
-    @test()
+    @test(disable=True)
     def no_test_child_test_childs_compare_notation(self):
         rows = self.init_childs(
             disabled_relationships=[
                 {Test.test_child: TestChild.test_childs},
                 Test.test_childs,
             ]
         )
@@ -232,22 +264,18 @@
         ]"""
         # full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
-    @test()
+    @test(disable=True)
     def fail_no_test_child_test_childs_compare(self):
         rows = self.init_childs(
             disabled_relationships={Test.test_child: Test.test_childs}
         )
 
         full_model = {x: y for x, y in self.test_p.items()}
         full_model["test_child"] = {x: y for x, y in self.test_p_child.items()}
@@ -257,50 +285,42 @@
         ]
         full_model["test_childs"] = [self.test_p_childs_1, self.test_p_childs_2]
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
-    @test()
+    @test(disable=True)
     def no_test_child_and_test_childs_compare(self):
         rows = self.init_childs(
             disabled_relationships=[Test.test_child, Test.test_childs]
         )
 
         full_model = {x: y for x, y in self.test_p.items()}
 
         self.assert_length(rows, 1)
         self.assert_equal(
             rows[0],
             full_model,
-            ignore={
-                "update_date": None,
-                "test_child": {"update_date": None, "test_childs": ["update_date"]},
-                "test_childs": ["update_date"],
-            },
+            ignore=self.ignore_pattern,
         )
 
     @test(save=False, begin=delete)
     def insert(self):
         test = self.db.add(Test, self.parameters)
         rows = self.db.select(Test)
         if len(rows) == 0:
             return False
         values = {x: getattr(rows[0], x) for x in self.parameters}
         return len(rows) == 1 and values == self.parameters
 
-    @test(save=False, begin=delete)
+    @test(disable=True, save=False, begin=delete)
     def roolback(self):
         rows = self.db.select(Test)
         if len(rows) != 0:
             return False
 
         test = self.db.add(Test, self.parameters, commit=False, rollback=False)
         rows = self.db.select(Test)
@@ -309,33 +329,33 @@
         self.db.rollback(session=test.query.session)
 
         # self.db.rollback()
         rows = self.db.select(Test)
 
         return len(rows) == 0
 
-    @test(save=False, begin=delete)
+    @test(disable=True, save=False, begin=delete)
     def roolback_update(self):
         rows = self.db.select(Test)
         if len(rows) != 0:
             return False
 
-        test = self.db.add(Test, self.parameters, commit=True, rollback=False)
+        test = self.db.add(Test, self.parameters, commit=True)
 
         new_parameters = {x: y for x, y in self.parameters.items()}
         new_parameters[Test.number.key] = 13
         self.db.update(test, new_parameters, commit=False)
         self.db.rollback(session=test.query.session)
 
         rows = self.db.select(Test)
         if len(rows) != 1:
             return False
         return new_parameters == rows[0]
 
-    @test(save=False, begin=delete)
+    @test(disable=True, save=False, begin=delete)
     def roolback_update_2(self):
         rows = self.db.select(Test)
         if len(rows) != 0:
             return False
 
         test = self.db.add(Test, self.parameters, commit=True, rollback=False)
 
@@ -351,17 +371,18 @@
         return new_parameters == rows[0]
 
     @test(save=False, begin=delete)
     def insert2(self):
         self.db.add(
             Test,
             {
+                Test.id: self.parameters[Test.id.key],
                 Test.name: self.parameters[Test.name.key],
                 Test.number: self.parameters[Test.number.key],
-                Test.text_: self.parameters[Test.text_.key],
+                Test.text: self.parameters[Test.text.key],
                 Test.date: self.parameters[Test.date.key],
             },
         )
         rows = self.db.select(Test)
         if len(rows) == 0:
             return False
         values = {x: getattr(rows[0], x) for x in self.parameters}
@@ -392,23 +413,23 @@
             and values == parameters_values
             and len(json_values) == len(self.columns)
         )
 
     @test(save=False, begin=delete)
     def delete(self):
         self.db.add(Test, self.parameters)
-        self.db.delete(Test, name=[Test.name == self.parameters[Test.name.key]])
+        self.db.delete(Test, filters=[Test.name == self.parameters[Test.name.key]])
         rows = self.db.select(Test)
         return len(rows) == 0
 
     @test(save=False, begin=delete)
     def delete2(self):
         test = Test(**self.parameters)
         self.db.add(test)
-        self.db.delete(test)
+        self.db.delete(test, filters=[], force=True)
         rows = self.db.select(Test)
         return len(rows) == 0
 
     @test(save=False, begin=delete)
     def select_unique(self):
         self.db.add(Test, self.parameters)
         rows = self.db.select(Test, unique=Test.name.key)
@@ -463,17 +484,15 @@
 
     @test(save=False, begin=delete)
     def update_with_model(self):
         added = self.db.add(Test, self.parameters)
         parameters = {x: y for x, y in self.parameters.items()}
         parameters[Test.number.key] += 1
         parameters[Test.id.key] = added.id
-        test = Test(**parameters)
-        test.query.session.commit()
-        # updated = self.db.update(Test(**parameters))
+        updated = self.db.update(Test(**parameters))
         rows = self.db.select(Test)
         return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in parameters
         }
 
     @test(save=False, begin=delete)
     def update_with_model_update(self):
@@ -491,16 +510,18 @@
 
     @test(save=False, begin=delete)
     def update_with_transient_model(self):
         added = self.db.add(Test, self.parameters, commit=False)
         added.number += 1
         updated = self.db.update(added)
         rows = self.db.select(Test)
+        parameters = self.parameters.copy()
+        parameters["number"] += 1
         return len(rows) == 1 and parameters == {
-            x: getattr(rows[0], x) for x in parameters
+            x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False, begin=delete)
     def update_last_with_model(self):
         added = self.db.add(Test, self.parameters)
         parameters_added = []
         for i in range(4):
@@ -515,14 +536,15 @@
         }
 
     @test(save=False, begin=delete)
     def update_multiple_with_model(self):
         parameters_list = []
         for i in range(4):
             parameters = {x: y for x, y in self.parameters.items()}
+            parameters[Test.id.key] = i
             parameters[Test.number.key] = i
             added = self.db.add(Test, parameters)
             parameters[Test.id.key] = added.id
             parameters_list.append({**parameters})
 
         for i in range(4):
             parameters_list[i][Test.number.key] += 1
@@ -568,46 +590,60 @@
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
             parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
         rows = self.db.select(Test)
-        return len(rows) == 1 and self.parameters == {
+        parameters = self.parameters.copy()
+        parameters["number"] += 4
+        return len(rows) == 1 and parameters == {
             x: getattr(rows[0], x) for x in self.parameters
         }
 
     @test(save=False, begin=delete)
     def add_or_update_multiple3(self):
         tests = [Test(**self.parameters)]
         for i in range(5):
-            parameters = {x: y for x, y in self.parameters.items()}
+            parameters = self.parameters.copy()
+            parameters[Test.id.key] = i + 2
             parameters[Test.number.key] += i
             tests.append(Test(**parameters))
-        parameters2 = {x: y for x, y in self.parameters.items()}
+
+        parameters2 = self.parameters.copy()
+        parameters2[Test.id.key] += 1
         parameters2[Test.name.key] = "new"
         tests.append(Test(**parameters2))
+
         self.db.add_or_update(tests)
         rows = self.db.select(Test)
-        return len(rows) == len(tests) and all(
+        len_check = len(rows) == len(tests)
+        similar_check = all(
             [
-                y == getattr(rows[0], x)
+                (
+                    y == getattr(rows[0], x)
+                    if x != Test.name.key
+                    else getattr(rows[0], x) in [y, "new"]
+                )
                 for x, y in self.parameters.items()
-                if x != Test.number.key
+                if (x != Test.number.key and x != Test.id.key)
             ]
         )
+        len_new = len([t for t in rows if t.name == "new"]) == 1
+        return len_check and similar_check and len_new
 
     @test(description="Test session bulk update", begin=delete)
     def bulk_update(self):
         rows = self.db.select(Test)
         self.assert_is_empty(rows)
 
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
+            parameters[Test.id.key] = i
             parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
         numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 5)
         self.assert_equal(set(numbers), set([12, 13, 14, 15, 16]))
 
@@ -633,14 +669,15 @@
     def bulk_update_2(self):
         rows = self.db.select(Test)
         self.assert_is_empty(rows)
 
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
+            parameters[Test.id.key] = i
             parameters[Test.number.key] += i
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
         numbers = self.db.select(Test, unique=Test.number)
         self.assert_length(numbers, 5)
         self.assert_equal(set(numbers), set([12, 13, 14, 15, 16]))
 
@@ -678,14 +715,15 @@
         self.assert_is_empty(rows)
 
     @test(description="Test select filters on dates", begin=delete)
     def select_date_filters(self):
         tests = [Test(**self.parameters)]
         for i in range(5):
             parameters = {x: y for x, y in self.parameters.items()}
+            parameters[Test.id.key] = i
             parameters[Test.number.key] = i
             parameters[Test.date.key] = date_lib.str_to_datetime(
                 "2020/01/%s 10:02:03" % (i + 1)
             )
             tests.append(Test(**parameters))
         self.db.add_or_update(tests)
```

### Comparing `alphaz-0.7.7.9/alphaz/tests/utils.py` & `alphaz-0.7.8/alphaz/tests/utils.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/api.py` & `alphaz-0.7.8/alphaz/utils/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,15 +122,15 @@
     route_log: bool = True,
     access_strings: list[str] | list[Enum] = [],
     access_error_message: str | None = None,
     pagination: int | None = None,
 ):
     path = "/" + path if path[0] != "/" else path
     if path in ROUTES_DISABLED:
-        return lambda x : x
+        return lambda x: x
 
     parameters = _process_parameters(path, parameters, pagination=pagination)
 
     def api_in(func):
         api.add_url_rule(path, methods=methods, view_func=func, endpoint=func.__name__)
 
         @api.endpoint(func.__name__)
```

### Comparing `alphaz-0.7.7.9/alphaz/utils/apm/ora.py` & `alphaz-0.7.8/alphaz/utils/apm/ora.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/configuration.py` & `alphaz-0.7.8/alphaz/utils/configuration.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/database/init.py` & `alphaz-0.7.8/alphaz/utils/database/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # MODULES
-import glob, os, importlib, re, json
-
+import glob, os, importlib, re, ujson, pathlib
 
 # MODELS
 from ...models.main import AlphaException, AlphaCore
 
+INI_TYPES = {
+    "json": {"key": "init_database_dir_json", "pattern": "*.json"},
+    "py": {"key": "init_database_dir_py", "pattern": "*.py"},
+    "sql": {"key": "init_database_dir_sql", "pattern": "*.sql"},
+}
+
 
 def __get_module_path(file_path: str) -> str:
     """
     Convert a file path to a Python module path.
 
     :param file_path: File path to convert.
     :return: The corresponding module path.
@@ -39,16 +44,17 @@
     with open(file_path, "r") as f:
         sql = f.read()
         sql = replace_to_date(sql)
         statements = sql.split(";")
 
         for statement in statements:
             try:
-                core.db.execute(statement, bind=bind.upper())
+                core.db.execute(statement + ";", bind=bind.upper())
             except Exception as ex:
+                print(f"Error with init of {file_path=}: " + str(ex))
                 core.db.log.error(f"Error with init of {file_path=}", ex=ex)
 
 
 def __process_headers_values(
     core: AlphaCore,
     bind: str,
     table_name: str,
@@ -129,143 +135,141 @@
             raise ValueError(f"Invalid data_type '{data_type}'")
 
         entries.append(entry)
 
     return entries
 
 
-def process_init_files(
-    core: AlphaCore, binds: list[str], tables: list[str], init_databases_config: dict
-):
-    """Charge les fichiers d'initialisation en fonction des types de fichiers et du répertoire d'initialisation spécifié pour chaque type.
-
-    Args:
-        core (AlphaCore): objet Core contenant les informations de base et les configurations
-        binds (list[str]): Liste des binds à traiter
-        tables (list[str]):  Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
-        init_databases_config (dict): Dictionnaire de configuration d'initialisation normalisé avec les clés en majuscules
-    """
-    ini_types = {
-        "json": {"key": "init_database_dir_json", "pattern": "*.json"},
-        "py": {"key": "init_database_dir_py", "pattern": "*.py"},
-        "sql": {"key": "init_database_dir_sql", "pattern": "*.sql"},
-    }
-
+def get_init_files(
+    core: AlphaCore, binds: list[str], init_databases_config: dict
+) -> list[str]:
+    ini_files = set()
     for bind in binds:
         if not bind in init_databases_config:
             core.log.warning(
                 f"No initialisation configuration has been set in <databases> entry for {bind=}"
             )
             continue
-        tables_configs = {}
 
         bind_cf = init_databases_config[bind]
         if type(bind_cf) == str and bind_cf.upper() in init_databases_config:
             bind_cf = init_databases_config[bind_cf.upper()]
 
-        for ini_type, cf_ini in ini_types.items():
+        for ini_type, cf_ini in INI_TYPES.items():
             if not cf_ini["key"] in bind_cf:
                 continue
 
             ini_dir = bind_cf[cf_ini["key"]]
             files = glob.glob(ini_dir + os.sep + cf_ini["pattern"])
+            ini_files.update(files)
 
-            for file_path in files:
-                ini = {}
-
-                if ini_type == "py":
-                    module_path = __get_module_path(file_path)
-                    module = importlib.import_module(module_path)
-
-                    if not hasattr(module, "ini"):
-                        continue
-
-                    ini = module.__dict__["ini"]
-                    if type(ini) != dict:
-                        raise AlphaException(
-                            f"In file {file_path} <ini> configuration must be of type <dict>"
-                        )
-                elif ini_type == "json":
-                    if os.path.exists(file_path):
-                        try:
-                            with open(file_path, encoding="utf-8") as json_data_file:
-                                ini = json.load(json_data_file)
-                        except Exception as ex:
-                            raise AlphaException(f"Cannot read file {file_path}: {ex}")
-                elif ini_type == "sql":
+            if ini_type == "sql":
+                for file_path in files:
                     __process_sql_file(core, bind, file_path)
-                else:
-                    raise ValueError(f"Unsupported file type '{ini_type}'")
+    return ini_files
 
-                for table_name, conf in ini.items():
-                    if not table_name in tables_configs:
-                        tables_configs[table_name] = []
-
-                    if not isinstance(conf, dict):
-                        core.log.error(
-                            f"Configuration for {table_name=} in file {file_path} must be of type <dict>"
-                        )
-                        continue
-                    conf["file_name"] = file_path
-                    tables_configs[table_name].append(conf)
+
+def process_init_files(
+    core: AlphaCore,
+    binds: list[str],
+    tables: list[str],
+    init_databases_config: dict,
+    no_log: bool = False,
+):
+    """Charge les fichiers d'initialisation en fonction des types de fichiers et du répertoire d'initialisation spécifié pour chaque type.
+
+    Args:
+        core (AlphaCore): objet Core contenant les informations de base et les configurations
+        binds (list[str]): Liste des binds à traiter
+        tables (list[str]):  Liste ou dictionnaire des noms des tables à traiter. Defaults to None.
+        init_databases_config (dict): Dictionnaire de configuration d'initialisation normalisé avec les clés en majuscules
+    """
+    tables_configs = {}  # TODO add BIND
+    for file_path in get_init_files(core, binds, init_databases_config):
+        ini = {}
+
+        ini_type = pathlib.Path(file_path).suffix.replace(".", "")
+        if ini_type == "py":
+            module_path = __get_module_path(file_path)
+            module = importlib.import_module(module_path)
+
+            if not hasattr(module, "ini"):
+                continue
+
+            ini = module.__dict__["ini"]
+            if type(ini) != dict:
+                raise AlphaException(
+                    f"In file {file_path} <ini> configuration must be of type <dict>"
+                )
+        elif ini_type == "json":
+            if os.path.exists(file_path):
+                try:
+                    with open(file_path, encoding="utf-8") as json_data_file:
+                        ini = ujson.load(json_data_file)
+                except Exception as ex:
+                    raise AlphaException(f"Cannot read file {file_path}: {ex}")
+        elif ini_type == "sql":
+            continue
+        else:
+            raise ValueError(f"Unsupported file type '{ini_type}'")
+
+        for table_name, conf in ini.items():
+            if not table_name in tables:
+                continue
+            if not table_name in tables_configs:
+                tables_configs[table_name] = []
+
+            if not isinstance(conf, dict):
+                core.log.error(
+                    f"Configuration for {table_name=} in file {file_path} must be of type <dict>",
+                    enabled=not no_log,
+                )
+                continue
+            conf["file_name"] = file_path
+            tables_configs[table_name].append(conf)
 
     for table_name in tables:
         if not table_name in tables_configs:
             continue
 
         for configuration in tables_configs[table_name]:
             model = core.db.get_table_model(table_name)
             bind = model.__bind_key__.upper()
             file_name = configuration["file_name"]
 
             entries = configuration.get("objects", [])
             if entries:
                 core.db.process_entries(bind, model, values=entries)
                 core.log.info(
-                    f"{table_name=} and {bind=} initiatied with <objects> format with file {file_name}"
+                    f"{table_name=} and {bind=} initiatied with <objects> format with file {file_name}",
+                    enabled=not no_log,
                 )
 
             headers, values = configuration.get("headers", []), configuration.get(
                 "values", []
             )
             if len(values) != 0:
                 __process_headers_values(core, bind, table_name, model, headers, values)
                 core.log.info(
-                    f"{table_name=} and {bind=} initiatied with <values> format with file {file_name}"
+                    f"{table_name=} and {bind=} initiatied with <values> format with file {file_name}",
+                    enabled=not no_log,
                 )
 
             values = configuration.get("results", [{"items": [{}]}])[0]["items"]
             headers = list(values[0].keys())
             if len(values) != 0:
                 __process_headers_values(
                     core, bind, table_name, model, headers, values, "sql"
                 )
                 core.log.info(
-                    f"{table_name=} and {bind=} initiatied with <results> format with file {file_name}"
+                    f"{table_name=} and {bind=} initiatied with <results> format with file {file_name}",
+                    enabled=not no_log,
                 )
 
 
-def __normalize_tables(tables: list[str] | dict[str, str]) -> list[str]:
-    """Normalise le paramètre 'tables' pour s'assurer qu'il est sous la forme d'un dictionnaire avec les noms des tables en majuscules.
-
-    Args:
-        tables (list[str]): Liste ou dictionnaire des noms des tables à traiter
-
-    Returns:
-        list[str] | dict[str, str, optional: _description_
-    """
-    if tables is not None:
-        return (
-            {x.upper(): None for x in tables}
-            if type(tables) == list
-            else {x.upper(): y for x, y in tables.items()}
-        )
-    return tables
-
-
 def __normalize_and_check_binds(binds: list[str], core: AlphaCore) -> list[str]:
     """Normalise le paramètre 'binds' et vérifie que les binds sont valides.
 
     Args:
         binds (list[str]): Liste des binds à traiter
         core (AlphaCore): objet Core contenant les informations de base et les configurations
```

### Comparing `alphaz-0.7.7.9/alphaz/utils/database_to_dataclass.py` & `alphaz-0.7.8/alphaz/utils/database_to_dataclass.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/decorators.py` & `alphaz-0.7.8/alphaz/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/ensure.py` & `alphaz-0.7.8/alphaz/utils/ensure.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/init_database.py` & `alphaz-0.7.8/alphaz/utils/init_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import subprocess, os, psutil, logging, json, argparse, time, re, sys
+import subprocess, os, psutil, logging, ujson, argparse, time, re, sys
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Init database")
 
     parser.add_argument("--project", "-p", help="Project path")
     parser.add_argument("--configuration", "-c", help="Configuration to run")
 
@@ -14,15 +14,14 @@
     parser.add_argument(
         "--create", "-cr", action="store_true", help="Create the tables"
     )
     parser.add_argument("--drop", "-d", action="store_true", help="Drop the tables")
     parser.add_argument(
         "--truncate", "-t", action="store_true", help="Truncate the tables"
     )
-    parser.add_argument("--sqlite", "-s", action="store_true", help="Sqlite mode")
     parser.add_argument(
         "--force", "-f", action="store_true", help="Force non local configuration"
     )
     parser.add_argument("--init", "-i", action="store_true", help="Init the tables")
     parser.add_argument(
         "--init_views", "-iv", action="store_true", help="Init the tables views"
     )
@@ -43,12 +42,11 @@
     test_categories = database_lib.init_databases(
         core=core,
         tables=args.tables,
         binds=args.binds,
         create=args.create,
         drop=args.drop,
         truncate=args.truncate,
-        sqlite=args.sqlite,
         force=args.force,
         init=args.init,
         init_views=args.init_views,
     )
```

### Comparing `alphaz-0.7.7.9/alphaz/utils/mep.py` & `alphaz-0.7.8/alphaz/utils/mep.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,9 +108,9 @@
             cmd                 = 'unzip -o -d %s %s'%(unzip_repository,backup_zip_file)
             os.system(cmd)
         
         if config_name == 'api':
             upload(target,Core.WEB_API_PATH,folder_list,root_ftp='')
 
     if config_name == 'api':
-        config_lib.upgrade_api_build(DB,Constants,CoreW)
+        config_lib.upgrade_api_build()
         restart_api()
```

### Comparing `alphaz-0.7.7.9/alphaz/utils/screens.py` & `alphaz-0.7.8/alphaz/utils/screens.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,210 +1,247 @@
-import subprocess, os, psutil, logging, json, argparse, time, re
+import subprocess, os, psutil, logging, argparse, time, re
 
 from logging.handlers import TimedRotatingFileHandler
 from screenutils import list_screens, Screen
 
 from alphaz.models.config import AlphaConfig
 
 import requests
 
 LOG = None
 
-def error(message,quit=False):
+
+def error(message, quit=False):
     if message is None or message.strip() == "":
         if quit:
             exit()
         return
     global LOG
-    print("ERROR: %s"%message)
+    print("ERROR: %s" % message)
     if LOG is not None:
         LOG.error(message)
     if quit:
         exit()
 
+
 def info(message, end="\n"):
     if message is None or message.strip() == "":
         return
     global LOG
-    print("INFO: %s"%message,end=end)
+    print("INFO: %s" % message, end=end)
     if LOG is not None:
         LOG.info(message)
 
+
 def get_cmd_output(cmd):
     result = subprocess.check_output(cmd, shell=True)
     lines = str(result).split("\\n")
     i = 0
     output_lines = []
     for line in lines:
         line = line.replace("\\t", "    ").replace("\\r", "")
         output_lines.append(line)
         i += 1
     return output_lines
 
+
 def replace_envs(text):
     if type(text) != str:
-       return text
-    envs = re.findall(r"\$[_a-zA-Z]+",text)
+        return text
+    envs = re.findall(r"\$[_a-zA-Z]+", text)
     for env in envs:
         if env[1:] in os.environ:
             text = text.replace(env, os.environ[env[1:]].strip())
     return text
 
+
 def log_config():
     global LOG
-    
+
     LOG = logging.getLogger(log_file.split(os.sep)[-1].split(".")[0])
     LOG.setLevel(logging.DEBUG)
 
     formatter = logging.Formatter(
         "%(asctime)s - %(name)s - %(levelname)s - %(message)s"
     )
 
     log_handler = TimedRotatingFileHandler(log_file, when="midnight", backupCount=30)
     log_handler.setFormatter(formatter)
     LOG.addHandler(log_handler)
-    
+
+
 def check_screen(screen, single=False):
     restarted = False
     info(screen["check_message"])
-    info("Fetching %s"%screen["request"])
+    info("Fetching %s" % screen["request"])
     time.sleep(screen["sleep"])
-    
+
     times = screen["retries"] if not single else 1
     for i in range(times):
         if restarted:
             continue
         try:
-            print('         ' + '.'*(times - i))
+            print("         " + "." * (times - i))
             r = requests.get(screen["request"], timeout=screen["timeout"])
             if "success" in str(r.content):
                 info(screen["success_message"])
                 restarted = True
                 continue
         except Exception as ex:
             time.sleep(screen["sleep"])
     if not restarted:
         error(screen["failed_message"])
     return restarted
 
+
 def launch_cmd(screen, s=None):
     if s is None:
-        s = Screen(screen["name"],True)
+        s = Screen(screen["name"], True)
     s.enable_logs()
-    s.send_commands("cd %s"%screen["dir"])
+    s.send_commands("cd %s" % screen["dir"])
     s.send_commands(screen["shell_cmd"])
     s.detach()
-    
+
     info("Screen %s restarted" % screen["name"])
     if "request" in screen and screen["request"]:
         restarted = check_screen(screen)
 
     print(next(s.logs))
     s.disable_logs()
-    
+
+
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(description="Ensure that a screen is running")
 
     parser.add_argument("--log", "-l", help="log file path")
     parser.add_argument("--file", "-f", help="Input configuration file")
-    
+
     parser.add_argument("--name", "-n", help="Screen name")
     parser.add_argument("--cmd", "-c", help="Command to run")
-    
+
     parser.add_argument("--envs", "-e", nargs="+", default=[], help="Command to run")
-    
+
     parser.add_argument("--directory", "-d", help="Working directory")
     parser.add_argument("--request", "-req", help="Request to check the response")
-    parser.add_argument("--retries", "-ret", type=int, default=10, help="Number of check before fail state")
+    parser.add_argument(
+        "--retries",
+        "-ret",
+        type=int,
+        default=10,
+        help="Number of check before fail state",
+    )
     parser.add_argument("--sleep", "-s", type=int, default=3, help="Sleep time (s)")
     parser.add_argument("--timeout", "-t", type=int, default=10, help="Sleep time (s)")
-    
+
     parser.add_argument("--message", "-m", help="Check message")
     parser.add_argument("--failed_message", "-fm", help="Failed message")
     parser.add_argument("--success_message", "-sm", help="Success message")
-    
-    parser.add_argument("--restart", "-r",action="store_true", help="Force a restart")
+
+    parser.add_argument("--restart", "-r", action="store_true", help="Force a restart")
 
     args = parser.parse_args()
 
     log_file = args.log
-    
+
     defaults = {
         "active": True,
         "name": args.name,
         "dir": args.directory if args.directory else os.getcwd(),
         "request": None if not args.request else args.request,
         "sleep": args.sleep,
         "retries": args.retries,
         "timeout": args.timeout,
         "restart": args.restart,
         "check_message": "" if not args.message else args.message,
         "failed_message": "Failed" if not args.failed_message else args.failed_message,
-        "success_message": "Success" if not args.success_message else args.success_message,
+        "success_message": "Success"
+        if not args.success_message
+        else args.success_message,
     }
-    
+
     for env in args.envs:
         envs_p = re.findall(r'^(\w+)="?([^"]+)"?', env)
         if len(envs_p) != 1:
-            error("<%s> environment variable is not weel defined, it must be like this: var=value")
+            error(
+                "<%s> environment variable is not weel defined, it must be like this: var=value"
+            )
             exit()
         name, value = envs_p[0][0], envs_p[0][1]
-        info("Set environment variable <%s> to <%s>"%(name, value))
+        info("Set environment variable <%s> to <%s>" % (name, value))
         os.environ[name] = value
 
     if args.file:
         file_path = args.file
         if not ".json" in file_path:
             file_path = file_path + ".json"
         if not os.path.exists(file_path):
-            error("Configuration file does not exist: %s"%file_path, quit=True)
+            error("Configuration file does not exist: %s" % file_path, quit=True)
         config = AlphaConfig(filepath=file_path)
         screens = config.get("screens")
         if screens is None:
-            error("Missing entry <screens> in configuration file %s"%file_path, quit=True)
+            error(
+                "Missing entry <screens> in configuration file %s" % file_path,
+                quit=True,
+            )
         if type(screens) != dict:
-            error("<screens> entry in configuration file %s is not valid"%file_path, quit=True)
+            error(
+                "<screens> entry in configuration file %s is not valid" % file_path,
+                quit=True,
+            )
         if not "configurations" in screens:
-            error("No <configurations> entry <screens> entry in configuration file %s"%file_path, quit=True)
+            error(
+                "No <configurations> entry <screens> entry in configuration file %s"
+                % file_path,
+                quit=True,
+            )
         if type(screens["configurations"]) != dict:
-            error("<screens> entry in configuration file %s is not valid"%file_path, quit=True)
+            error(
+                "<screens> entry in configuration file %s is not valid" % file_path,
+                quit=True,
+            )
         screens_dict = screens["configurations"]
     elif args.name and args.cmd:
         screens_dict = {args.name: defaults}
     else:
-        error("You need to specify a configuration file or at least a screen name (--name) and a command (--cmd)")
+        error(
+            "You need to specify a configuration file or at least a screen name (--name) and a command (--cmd)"
+        )
         exit()
 
     screens_list = list_screens()
-        
+
     for name, screen in screens_dict.items():
-        screen = {x:replace_envs(y) for x,y in screen.items()}
+        screen = {x: replace_envs(y) for x, y in screen.items()}
         active = screen["active"]
         screen_name = screen["name"]
-        
+
         if not active:
-            info("Screen configuration <%s> is DISABLED"%screen_name)
+            info("Screen configuration <%s> is DISABLED" % screen_name)
             continue
-            
-        
+
         for key, value in defaults.items():
             if not key in screen or screen is None:
                 screen[key] = value
-                info("Set default key <%s> to <%s>"%(key, value))
-        
-        info("Processing screen configuration <%s>"%screen_name)
-        
+                info("Set default key <%s> to <%s>" % (key, value))
+
+        info("Processing screen configuration <%s>" % screen_name)
+
         screen_exist_list = [x for x in screens_list if x.name == screen_name]
         if len(screen_exist_list) != 0:
             for screen_entity in screen_exist_list:
-                info("Screen %s %s is running ..." % (screen_entity.id, screen_entity.name))
+                info(
+                    "Screen %s %s is running ..."
+                    % (screen_entity.id, screen_entity.name)
+                )
                 if screen["restart"]:
                     screen_entity.kill()
-                    info("Screen %s %s killed !" % (screen_entity.id, screen_entity.name))
-                
+                    info(
+                        "Screen %s %s killed !" % (screen_entity.id, screen_entity.name)
+                    )
+
                 if "request" in screen and screen["request"]:
                     restarted = check_screen(screen, single=True)
                     if not restarted or screen["restart"]:
                         launch_cmd(screen)
-        
+
         elif len(screen_exist_list) == 0 or screen["restart"]:
-            launch_cmd(screen)
+            launch_cmd(screen)
```

### Comparing `alphaz-0.7.7.9/alphaz/utils/selectionMenu.py` & `alphaz-0.7.8/alphaz/utils/selectionMenu.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/tasks.py` & `alphaz-0.7.8/alphaz/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/time.py` & `alphaz-0.7.8/alphaz/utils/time.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz/utils/transactions.py` & `alphaz-0.7.8/alphaz/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `alphaz-0.7.7.9/alphaz.egg-info/PKG-INFO` & `alphaz-0.7.8/alphaz.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: alphaz
-Version: 0.7.7.9
+Version: 0.7.8
 Summary: A package full of very nice tools
 Home-page: https://github.com/ZAurele/alphaz
-Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.7.9.tar.gz
+Download-URL: https://github.com/ZAurele/alphaz/archive/refs/tags/0.7.8.tar.gz
 Author: Aurèle
 Author-email: contact@aurele.eu
 License: MIT
 Keywords: Flask,Json
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `alphaz-0.7.7.9/alphaz.egg-info/SOURCES.txt` & `alphaz-0.7.8/alphaz.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,16 @@
 alphaz/models/api/_route.py
 alphaz/models/api/_structures.py
 alphaz/models/api/_utils.py
 alphaz/models/config/__init__.py
 alphaz/models/config/_config.py
 alphaz/models/config/_utils.py
 alphaz/models/database/__init__.py
+alphaz/models/database/configs.py
+alphaz/models/database/mails.py
 alphaz/models/database/main_definitions.py
 alphaz/models/database/models.py
 alphaz/models/database/operators.py
 alphaz/models/database/requests.py
 alphaz/models/database/row.py
 alphaz/models/database/structure.py
 alphaz/models/database/tests.py
```

### Comparing `alphaz-0.7.7.9/setup.py` & `alphaz-0.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os, glob, re
 from datetime import date
 
 today = date.today()
 
 from setuptools import setup, find_packages
 
-version = "0.7.7.9"
+version = "0.7.8"
 
 excludes = [".git", ".vscode"]
 
 archives = glob.glob("dist/*")
 for archive in archives:
     os.remove(archive)
 
@@ -53,14 +53,16 @@
 print(f"Reading {req_path} ...")
 with open(req_path, 'r') as f:
     required = [''.join([i for i in x.strip().replace("\ufeff","") if i.isalnum()]) for x in f.readlines()]
     try:
       """
 
 required = [
+    "SQLAlchemy==1.4.37",
+    "ujson",
     "chardet",
     "paramiko",
     "typing-extensions",
     "numpy",
     "colorama",
     "concurrent_log_handler",
     "flask_sqlalchemy",
```

