# Comparing `tmp/translate-toolkit-3.8.6.tar.gz` & `tmp/translate-toolkit-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "translate-toolkit-3.8.6.tar", last modified: Tue Mar  7 12:41:27 2023, max compression
+gzip compressed data, was "translate-toolkit-3.9.0.tar", last modified: Mon May 15 15:14:10 2023, max compression
```

## Comparing `translate-toolkit-3.8.6.tar` & `translate-toolkit-3.9.0.tar`

### file list

```diff
@@ -1,991 +1,1001 @@
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.526634 translate-toolkit-3.8.6/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      140 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.deepsource.toml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.430634 translate-toolkit-3.8.6/.github/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      349 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/dependabot.yml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.430634 translate-toolkit-3.8.6/.github/matchers/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/matchers/flake8.json
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/.github/workflows/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      802 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/docs.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1894 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/linux.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1361 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/osx.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1764 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/pre-commit.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1761 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/setup.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1145 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.github/workflows/win.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      724 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.gitignore
--rw-r--r--   0 nijel     (1000) nijel     (1000)      102 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.gitmodules
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1098 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.pre-commit-config.yaml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      569 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/.readthedocs.yml
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17992 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/COPYING
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1768 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/CREDITS
--rw-r--r--   0 nijel     (1000) nijel     (1000)      171 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/LICENSES
--rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/MANIFEST.in
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2925 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/Makefile
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-03-07 12:41:27.526634 translate-toolkit-3.8.6/PKG-INFO
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8810 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/README.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)       15 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/codecov.yml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5743 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/Makefile
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_ext/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/_ext/translate_docs.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_static/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       55 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/_static/README.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_themes/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      703 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/README.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/globaltoc.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2628 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/layout.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      227 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/localtoc.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      304 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/relations.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1085 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/search.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/searchbox.html
--rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/sourcelink.html
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10518 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css
--rw-r--r--   0 nijel     (1000) nijel     (1000)      374 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.css_t
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1727 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js
--rw-r--r--   0 nijel     (1000) nijel     (1000)    97055 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap.css
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22323 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap.js
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.434634 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    38708 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)   130151 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    68476 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    41752 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff
--rw-r--r--   0 nijel     (1000) nijel     (1000)    93436 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/jquery.js
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.438634 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14766 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4514 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/theme.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8431 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/variables.less
--rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-03-07 12:40:40.000000 translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/theme.conf
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.438634 translate-toolkit-3.8.6/docs/api/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5427 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/convert.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/filters.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      912 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/lang.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      964 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/misc.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      364 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/search.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      177 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/services.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6573 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/storage.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1680 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/api/tools.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.442634 translate-toolkit-3.8.6/docs/commands/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5021 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/csv2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3362 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/csv2tbx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5091 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/flatxml2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2063 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/general_usage.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5138 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/html2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4287 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/ical2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6234 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5482 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/ini2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4106 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/json2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      259 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/junitmsgfmt.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2631 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/levenshtein_distance.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4456 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/moz-l10n-builder.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7496 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/moz2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9695 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/mozilla_l10n_scripts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3699 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/odf2xliff.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7685 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/oo2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1157 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_accelerator.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2411 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_duplicates.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1704 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_errorlevel.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      599 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_filteraction.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      613 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_multifile.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1562 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_personality.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2719 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_progress.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4073 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/option_rewrite.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4377 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/phase.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4172 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/php2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3396 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/po2tmx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1659 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/po2wordfast.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1804 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poclean.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      968 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pocommentclean.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3485 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pocompendium.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1847 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pocompile.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3790 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poconflicts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5658 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pocount.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7176 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/podebug.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pofilter.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25812 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pofilter_tests.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3789 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pogrep.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4091 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pomerge.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pomigrate2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1746 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/popuretext.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1367 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poreencode.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2046 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/porestructure.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3586 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/posegment.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      848 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/posplit.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3354 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poswap.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4111 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pot2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16451 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poterminology.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8052 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/poterminology_stopword_file.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3214 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/pretranslate.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7629 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/prop2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4925 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/rc2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4019 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/resx2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3908 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/sub2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5754 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/symb2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1638 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/tbx2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2375 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/tiki2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/tmserver.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3864 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/ts2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7056 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/txt2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3727 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/web2py2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3213 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/xliff2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4357 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/commands/yaml2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6573 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/conf.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1028 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/contents.rst.inc
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.442634 translate-toolkit-3.8.6/docs/developers/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1299 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/building.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3679 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/contributing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2146 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/deprecation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9692 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/developers.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11047 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/releasing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3174 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/reporting_bugs.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19038 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/styleguide.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9434 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/developers/testing.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2499 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/features.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.446634 translate-toolkit-3.8.6/docs/formats/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      736 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/android.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7698 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/base_classes.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2041 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/catkeys.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      707 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/conformance.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1973 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/csv.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1006 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/dtd.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3043 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/flatxml.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      451 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/flex.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      493 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/gsi.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1160 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/html.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/ical.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7893 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      769 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/ini.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      923 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/json.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      998 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/mo.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/mozilla_lang.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1549 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/odf.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      962 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/omegat_glossary.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7761 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/php.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1210 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1579 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/properties.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      888 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/qm.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1233 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/qt_phrase_book.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2078 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/quoting_and_escaping.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1281 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/rc.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1412 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/resx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/strings.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1360 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/subtitles.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2026 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/tbx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      800 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/text.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      810 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/tmx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1964 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/ts.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1216 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/utx.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/wiki.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      316 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/wml.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/wordfast.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2160 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/xliff.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      495 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/formats/yaml.rst
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.450634 translate-toolkit-3.8.6/docs/guides/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6603 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/checking_for_inconsistencies.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1736 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/cleanup_translator_comments.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7490 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2161 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/creating_mozilla_pot_files.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1960 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/document_translation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1297 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6258 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/migrating_translations.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1524 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/running_the_tools_on_microsoft_windows.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7596 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/using_csv2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/using_oo2po.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7736 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/guides/using_pofilter.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4864 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/history.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      237 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5263 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/installation.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      233 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/license.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5116 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/make.bat
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.454634 translate-toolkit-3.8.6/docs/releases/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      225 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.10.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2200 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.10.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1170 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.11.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      220 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.7.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.8.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.9.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.9.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4422 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/0.9.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      655 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.0.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6959 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4071 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      680 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.1.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4368 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.10.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4975 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.11.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5431 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.12.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4151 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.13.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2206 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.2.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      273 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      713 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      961 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.4.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.5.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.5.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      589 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.6.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      218 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.7.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.8.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3162 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.8.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/1.9.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8012 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.0.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1621 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1310 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      376 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      384 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1018 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      557 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.2.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2341 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.3.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2357 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1465 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1416 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/2.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1563 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.0.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1211 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.1.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      378 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.1.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      639 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.2.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1490 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      604 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      692 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      438 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      490 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.3.6.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      563 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.4.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      573 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.4.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      481 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.5.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      367 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.5.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      482 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.5.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      394 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.5.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      765 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.6.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      533 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.6.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      508 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.6.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      869 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.7.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      477 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.7.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      387 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.7.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      602 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.7.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      536 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.7.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      701 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.0.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      529 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.1.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      348 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.2.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      398 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.3.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      403 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.4.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      347 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.5.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      447 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/3.8.6.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1246 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/README.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1666 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/docs/releases/index.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)      118 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/pyproject.toml
--rw-r--r--   0 nijel     (1000) nijel     (1000)       41 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/pytest.ini
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.454634 translate-toolkit-3.8.6/requirements/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       36 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/dev.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/dist.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       18 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/lint.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)      735 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/optional.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       71 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/required.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       68 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/requirements/test.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6398 2023-03-07 12:41:27.526634 translate-toolkit-3.8.6/setup.cfg
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2385 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/setup.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.430634 translate-toolkit-3.8.6/tests/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.458634 translate-toolkit-3.8.6/tests/cli/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.430634 translate-toolkit-3.8.6/tests/cli/data/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.458634 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      460 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      813 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.458634 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongkey/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongkey/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      212 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongkey/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongns/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongns/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongns/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongroot/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongroot/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongroot/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongvalue/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongvalue/one.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      210 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po_wrongvalue/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2csv/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2csv/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       88 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2csv/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       61 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      118 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml/out.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_params/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_params/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      318 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_params/out.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_preserve/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       89 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_preserve/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_preserve/out.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      264 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_preserve/two.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_template/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_template/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      270 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_template/out.xml
--rw-r--r--   0 nijel     (1000) nijel     (1000)      115 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2flatxml_template/two.xml
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2html/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2html/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       79 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2html/out.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       78 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2html/template.html
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.462634 translate-toolkit-3.8.6/tests/cli/data/test_po2json_files_removeuntranslated/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       42 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2json_files_removeuntranslated/out.json
--rw-r--r--   0 nijel     (1000) nijel     (1000)       83 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2json_files_removeuntranslated/template.json
--rw-r--r--   0 nijel     (1000) nijel     (1000)      161 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2json_files_removeuntranslated/translations.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_po2prop_mozilla_files/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      145 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2prop_mozilla_files/out.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      141 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2prop_mozilla_files/template.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2prop_mozilla_files/translations.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_po2ts/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2ts/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      362 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2ts/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_po2txt/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2txt/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       32 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2txt/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_po2txt_threshold/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2txt_threshold/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_po2txt_threshold/out.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      206 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_help/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      686 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_help/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_mutually_exclusive/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_mutually_exclusive/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_nonexistant/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       74 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_nonexistant/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_csv/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_csv/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      302 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_csv/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_file/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_file/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      430 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_file/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_fuzzy/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      121 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_fuzzy/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      492 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_fuzzy/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_plurals/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      101 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_plurals/plural.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_po_plurals/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_no/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1505 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_no/states.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_no/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_yes/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_yes/states.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)      504 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_yes/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pofilter_listfilters/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3337 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pofilter_listfilters/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.466634 translate-toolkit-3.8.6/tests/cli/data/test_pofilter_manpage/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3421 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_pofilter_manpage/stdout.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_posegment/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      370 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_posegment/one.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      388 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_posegment/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_poswap_comments/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_comments/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      130 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_comments/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_comments/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af_reverse/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af_reverse/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af_reverse/fr_af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_fr_af_reverse/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_poswap_missing_units/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       52 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_missing_units/af.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       54 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_missing_units/fr.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       49 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_poswap_missing_units/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      322 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/one/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/one/a.properties
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/out/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      498 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/out/a.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      144 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_dirs/stderr.txt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files/one.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      506 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files/out.po
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files_templates/
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files_templates/one.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)      574 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files_templates/out.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)       11 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files_templates/two.properties
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.470634 translate-toolkit-3.8.6/tests/cli/data/test_rc2po/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3564 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_rc2po/one.rc
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1882 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/data/test_rc2po/out.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)      727 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/example_test.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      226 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/run_tests.sh
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4775 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test.inc.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_flatxml2po.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_flatxml2po_wrongkey.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_flatxml2po_wrongns.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      142 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_flatxml2po_wrongroot.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      143 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_flatxml2po_wrongvalue.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2csv.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2flatxml.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      252 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2flatxml_params.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2flatxml_preserve.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      266 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2flatxml_template.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      137 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2html.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      167 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2json_files_removeuntranslated.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      168 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2prop_mozilla_files.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2ts.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2txt.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      194 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_po2txt_threshold.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      135 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_help.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_mutually_exclusive.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      109 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_nonexistant.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      109 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_po_csv.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_po_file.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_po_fuzzy.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_xliff_states_no.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pocount_xliff_states_yes.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      113 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pofilter_listfilters.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      182 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_pofilter_manpage.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      126 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_posegment.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_poswap_comments.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_poswap_fr_af.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      160 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_poswap_fr_af_reverse.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_poswap_missing_units.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)       98 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_prop2po.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      108 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_prop2po_dirs.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      124 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_prop2po_files.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      132 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_prop2po_files_templates.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      128 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/cli/test_rc2po.sh
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.474634 translate-toolkit-3.8.6/tests/odf_xliff/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3085 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)   133081 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/odf_xliff/test_2.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1864 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7300 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/odf_xliff/test_inline.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5467 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/odf_xliff/test_odf_xliff.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.474634 translate-toolkit-3.8.6/tests/xliff_conformance/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    36103 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/xliff_conformance/af-pootle.po
--rw-r--r--   0 nijel     (1000) nijel     (1000)    30075 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/xliff_conformance/en-US.sdf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2152 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/xliff_conformance/test_xliff_conformance.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    96911 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tests/xliff_conformance/xliff-core-1.1.xsd
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.474634 translate-toolkit-3.8.6/tools/
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1903 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/junitmsgfmt
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.474634 translate-toolkit-3.8.6/tools/mozilla/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7012 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/README.firefox_build_instructions.rst
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4102 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/Vagrantfile
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3429 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/accesskey_checker
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2546 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/accesskey_checker_PO
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12855 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/build_firefox.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7178 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/build_tb3_langs.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9666 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/buildxpi.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      158 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/compare-locales.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4496 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/get_moz_enUS.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11342 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/moz-l10n-builder
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    23576 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/moz_l10n_builder.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2258 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/mozcronbuild.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1487 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/mozilla-l10n.patch
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12089 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/mozzy.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3208 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/postinstall.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      497 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/mozilla/setup_mozilla.sh
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18996 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/phase
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      626 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/phaselist2goals
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1041 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/pocommentclean
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4683 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/pocompendium
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5288 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/pomigrate2
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1852 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/popuretext
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1121 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/poreencode
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1526 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/tools/posplit
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.474634 translate-toolkit-3.8.6/translate/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1816 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1406 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/__version__.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.490634 translate-toolkit-3.8.6/translate/convert/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      790 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8226 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/accesskey.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    20604 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/convert.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    10172 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/csv2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3325 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/csv2tbx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13191 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/dtd2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7542 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/factory.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3663 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/flatxml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5523 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/html2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4527 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/ical2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1902 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/idml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5078 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/ini2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5181 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/json2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2358 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/moz2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4922 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/mozfunny2prop.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3952 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/mozlang2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3839 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/odf2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      357 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/odfxml
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7937 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/oo2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7287 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/oo2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4536 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/php2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3950 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2csv.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8688 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2dtd.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5083 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2flatxml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6792 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2html.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3617 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2ical.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6806 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2idml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4107 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2ini.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3682 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2json.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3490 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2moz.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3702 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2mozlang.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11234 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2oo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3375 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2php.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12941 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2prop.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13214 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2rc.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3195 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2resx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2821 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2sub.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4085 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2symb.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3227 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2tiki.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5569 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2tmx.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3228 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2ts.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5171 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2txt.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2559 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2web2py.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4185 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2wordfast.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4287 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2xliff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3949 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/po2yaml.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12222 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/pot2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6230 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/prop2mozfunny.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18819 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/prop2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5942 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/rc2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6039 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/resx2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1730 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/roundtrip-OOo
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1629 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/roundtrip-gaia
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1589 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/roundtrip-mozilla
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4777 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/sub2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4101 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/symb2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2352 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/tbx2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   189411 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test.idml
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11608 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test.odt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_accesskey.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5373 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_convert.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6225 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_csv2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19205 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_dtd2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4744 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_flatxml2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27945 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_html2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12076 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_ical2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      449 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_idml2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4544 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_ini2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2472 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_json2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      414 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_moz2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2179 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_mozfunny2prop.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4733 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_mozlang2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      446 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_ods2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13063 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_oo2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2989 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_oo2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11579 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_php2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5969 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2csv.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22148 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4617 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11889 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10814 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2ical.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      826 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2idml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8118 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3853 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2json.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      494 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2moz.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5024 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2mozlang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9663 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10874 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2php.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17564 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2prop.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9085 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18992 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2152 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2sub.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2097 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6522 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4373 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5238 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1967 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2web2py.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10413 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6837 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_po2yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27471 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_pot2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2201 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_prop2mozfunny.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14486 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_prop2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4828 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_rc2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10049 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_resx2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2362 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_tiki2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4628 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_ts2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8333 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_txt2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1823 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_web2py2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      942 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_xliff2odf.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12996 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_xliff2po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5143 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/test_yaml2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3144 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/tiki2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3774 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/ts2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4682 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/txt2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2757 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/web2py2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5947 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/xliff2odf.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11231 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/xliff2oo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4049 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/xliff2po.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4458 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/convert/yaml2po.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.490634 translate-toolkit-3.8.6/translate/filters/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      766 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2440 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/autocorrect.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   101820 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/checks.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10481 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/decoration.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1940 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/decorators.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2796 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/helpers.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13302 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/pofilter.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6133 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/prefilters.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2131 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/spelling.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2531 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/test_autocorrect.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)   108937 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/test_checks.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4060 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/test_decoration.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13635 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/test_pofilter.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1065 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/filters/test_prefilters.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.498634 translate-toolkit-3.8.6/translate/lang/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3869 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/af.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      925 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ak.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/am.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/az.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2096 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/bn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/bo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1458 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/code_as.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1551 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/code_or.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13175 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/common.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1081 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/da.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    27414 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/data.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/de.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/dz.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1949 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/el.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1782 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/es.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3632 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/fa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2489 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      985 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/fi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2849 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/fr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/gd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/gu.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/he.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/hi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/hy.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4934 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/identify.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1699 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ja.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1977 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/km.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/kn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ko.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/kw.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/lo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      986 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/mr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ms.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1042 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/my.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1637 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ne.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4894 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ngram.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1413 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/nqo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/nso.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1614 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/pa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1079 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/pl.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5968 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/poedit.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1100 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/pt_BR.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2828 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ro.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5382 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/scn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      992 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/si.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      963 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/son.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      940 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/st.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/su.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1080 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/sv.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      978 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ta.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/te.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    21017 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/team.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)      707 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test-language-teams.sh
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1690 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_af.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1119 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_am.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1388 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_ar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5162 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_common.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4131 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_data.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1417 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_el.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1273 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_es.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2815 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_fa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1918 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3107 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_fr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1448 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_hy.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6481 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_identify.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1116 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_ja.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1829 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_km.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1094 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_ko.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2963 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_ne.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1751 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_nqo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1639 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_or.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      705 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_poedit.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1737 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_ro.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1869 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_scn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      775 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_team.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      632 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_th.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      405 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_tr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      328 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_uk.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1426 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_vi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1008 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/test_zh.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1181 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/th.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1025 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/tr.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1091 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ug.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1186 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ur.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/ve.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1532 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/vi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1655 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/wo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2367 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/zh.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/zh_cn.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/zh_hk.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/lang/zh_tw.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.502634 translate-toolkit-3.8.6/translate/misc/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      838 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1610 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/deprecation.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2733 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/dictutils.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2580 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/file_discovery.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3010 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/multistring.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    33419 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/optrecurse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10454 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/ourdom.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/progressbar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17756 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/quote.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17682 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/selector.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      465 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_deprecation.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      234 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_dictutils.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3052 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_multistring.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1133 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_optrecurse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      419 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_progressbar.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7634 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_quote.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1209 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/test_xml_helpers.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1424 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/wStringIO.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1138 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/wsgi.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6870 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/misc/xml_helpers.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.502634 translate-toolkit-3.8.6/translate/search/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      772 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6056 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/lshtein.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15948 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/match.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1754 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1866 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/test_lshtein.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5705 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/test_match.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      307 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/search/test_terminology.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.502634 translate-toolkit-3.8.6/translate/services/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      833 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/services/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1855 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/services/test_tmserver.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8293 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/services/tmserver.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.502634 translate-toolkit-3.8.6/translate/share/
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.510634 translate-toolkit-3.8.6/translate/share/langmodels/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1449 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Ndebele.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1481 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/NorthernSotho.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1071 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/README
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Sotho.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Swati.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1447 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Tsonga.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1475 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Tswana.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1457 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Venda.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1421 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Xhosa.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1464 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/Zulu.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3387 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/afrikaans.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/albanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/arabic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3243 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/basque.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2195 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/belarus.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/bosnian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3287 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/breton.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3223 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/catalan.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2089 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/chinese_simplified.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1991 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/chinese_traditional.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3428 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/croatian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3369 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/czech.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3375 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/danish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3384 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/dutch.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/english.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3427 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/esperanto.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3315 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/estonian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3425 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/finnish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3687 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/fpdb.conf
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/french.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3443 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/frisian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3444 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/german.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4266 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/greek.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4187 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/hebrew.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3353 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/hungarian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3475 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/icelandic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3359 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/indonesian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3178 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/irish_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3426 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/italian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2309 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/japanese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3324 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/latin.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3500 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/latvian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3350 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/lithuanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3597 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/malay.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3462 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/manx_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3408 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/norwegian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3416 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/polish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3467 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/portuguese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3205 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/quechua.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/romanian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3117 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/romansh.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4146 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/russian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/scots.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3323 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/scots_gaelic.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3420 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/serbian_ascii.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/slovak_ascii.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3152 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/slovenian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3417 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/spanish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3314 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/swahili.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3484 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/swedish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3261 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/tagalog.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3539 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/turkish.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2172 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/ukrainian.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3689 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/vietnamese.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3535 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/langmodels/welsh.lm
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8740 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/share/stoplist-en
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.518634 translate-toolkit-3.8.6/translate/storage/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1325 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/_factory_classes.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    23089 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/aresource.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    34025 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7514 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/benchmark.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10411 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/bundleprojstore.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10971 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/catkeys.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    37642 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/cpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11481 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/csvl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      338 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/debug.properties
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2383 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/directory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    24353 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8763 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8204 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6909 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/fluent.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    19720 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/fpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17148 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4973 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/ical.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2847 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/idml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4516 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25065 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/jsonl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13083 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10983 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/mo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5500 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/mozilla_lang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1165 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/odf_io.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5390 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/odf_shared.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6140 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/omegat.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15689 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18547 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/php.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.522634 translate-toolkit-3.8.6/translate/storage/placeables/
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2005 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2963 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13902 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/general.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1241 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/interfaces.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7196 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3269 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/parse.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    35646 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/strelem.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3298 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8107 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/test_base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10622 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/test_general.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6121 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/test_lisa.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1990 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/test_terminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3992 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/placeables/xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1694 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7093 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/pocommon.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16277 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/poheader.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13216 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/poparser.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    12926 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/poxliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9144 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/project.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14696 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/projstore.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      753 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/properties.java
--rw-r--r--   0 nijel     (1000) nijel     (1000)    43633 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/properties.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    37284 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8560 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/qm.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5127 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/qph.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    16053 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1649 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/resourcedictionary.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8538 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7568 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/statistics.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6662 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/stringsdict.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7653 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/subtitles.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2235 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/symbian.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4496 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/tbx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    30223 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_aresource.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14725 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_base.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2492 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_catkeys.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9087 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_cpo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5570 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_csvl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2798 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_directory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    21418 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_dtd.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6704 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_factory.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3869 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_flatxml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7927 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_fluent.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9820 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_html.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      483 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_ini.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    28695 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_jsonl10n.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8420 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_mo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1296 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_monolingual.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10207 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_mozilla_lang.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      472 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_omegat.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6658 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_oo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    44427 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_php.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    38517 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_po.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      675 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_pocommon.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11275 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_poheader.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4443 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_poxliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    64202 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_properties.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    22936 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1198 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_qm.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3240 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_qph.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    18737 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_rc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1928 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_resourcedictionary.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5022 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_resx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6114 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_stringsdict.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      743 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_subtitles.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2413 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_tbx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3146 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3916 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      883 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_trados.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      211 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13669 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_ts2.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2002 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_utx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2818 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_wordfast.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    25248 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_xliff.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15664 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2697 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/test_zip.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6986 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/tiki.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    13005 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/tmdb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5845 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/tmx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6410 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/trados.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     6935 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/ts.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    17855 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/ts2.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4995 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/txt.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     9488 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/utx.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    15188 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/wordfast.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8786 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/workflow.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    33544 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xliff.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.522634 translate-toolkit-3.8.6/translate/storage/xml_extract/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      716 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/__init__.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14635 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/extract.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11240 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/generate.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2825 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/misc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2167 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/test_misc.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2956 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/test_unit_tree.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1205 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/test_xpath_breadcrumb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     4854 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/unit_tree.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_extract/xpath_breadcrumb.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2677 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/xml_name.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     7211 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/yaml.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     2276 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/storage/zip.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.526634 translate-toolkit-3.8.6/translate/tools/
--rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/__init__.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3351 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/build_tmdb.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3415 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/phppo2pypo.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2364 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/poclean.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3408 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pocompile.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8679 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/poconflicts.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18858 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pocount.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    16414 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/podebug.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    14678 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pogrep.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5292 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pomerge.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5643 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/porestructure.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4954 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/posegment.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3720 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/poswap.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    25252 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/poterminology.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9214 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pretranslate.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12660 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pydiff.py
--rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3384 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/pypo2phppo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1710 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_phppo2pypo.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     5131 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_pocount.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    11913 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_podebug.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     8182 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_pogrep.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    23743 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_pomerge.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3529 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_posegment.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)      946 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_poterminology.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)    14618 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_pretranslate.py
--rw-r--r--   0 nijel     (1000) nijel     (1000)     1709 2023-03-07 12:34:33.000000 translate-toolkit-3.8.6/translate/tools/test_pypo2phppo.py
-drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-03-07 12:41:27.526634 translate-toolkit-3.8.6/translate_toolkit.egg-info/
--rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 nijel     (1000) nijel     (1000)    28595 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)     3150 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/not-zip-safe
--rw-r--r--   0 nijel     (1000) nijel     (1000)      629 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/requires.txt
--rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-03-07 12:41:27.000000 translate-toolkit-3.8.6/translate_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      135 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.deepsource.toml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      349 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/dependabot.yml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/matchers/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/matchers/flake8.json
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/.github/workflows/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      815 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1905 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/linux.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1361 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/osx.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1764 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1774 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/setup.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1145 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.github/workflows/win.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      724 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.gitignore
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      102 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.gitmodules
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1265 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.pre-commit-config.yaml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      569 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/.readthedocs.yml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/COPYING
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1768 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/CREDITS
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/LICENSES
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/MANIFEST.in
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/Makefile
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/PKG-INFO
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8810 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/README.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       15 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/codecov.yml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/docs/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5743 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/Makefile
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.481689 translate-toolkit-3.9.0/docs/_ext/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/_ext/translate_docs.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_static/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       55 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/_static/README.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      703 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/README.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/globaltoc.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2628 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/layout.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      227 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/localtoc.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      304 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/relations.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1085 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/search.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      305 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/searchbox.html
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/sourcelink.html
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10518 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      374 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.css_t
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1727 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    97055 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.css
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22323 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.js
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    38708 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)   130151 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    68476 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    41752 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    93436 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/jquery.js
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14766 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4514 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/theme.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8431 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/variables.less
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:13:17.000000 translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/theme.conf
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.485689 translate-toolkit-3.9.0/docs/api/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/convert.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/filters.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      912 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/lang.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      964 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/misc.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      364 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/search.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      177 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/services.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6573 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/storage.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1680 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/api/tools.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.493689 translate-toolkit-3.9.0/docs/commands/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5021 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/csv2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/csv2tbx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/flatxml2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2063 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/general_usage.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5138 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/html2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ical2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5482 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ini2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4106 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/json2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      356 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/junitmsgfmt.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2631 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/levenshtein_distance.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4456 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/moz-l10n-builder.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7496 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/moz2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9695 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/mozilla_l10n_scripts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3699 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/odf2xliff.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7685 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/oo2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1157 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_accelerator.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2411 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_duplicates.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1704 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_errorlevel.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      599 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_filteraction.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      613 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_multifile.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1562 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_personality.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2719 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_progress.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4073 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/option_rewrite.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4377 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/phase.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4172 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/php2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3396 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/po2tmx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1659 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/po2wordfast.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1804 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poclean.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      968 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocommentclean.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3485 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocompendium.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1847 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocompile.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3790 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poconflicts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5658 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pocount.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7176 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/podebug.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pofilter.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25812 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pofilter_tests.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3789 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pogrep.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pomerge.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pomigrate2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1746 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/popuretext.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poreencode.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2046 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/porestructure.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3586 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/posegment.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      848 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/posplit.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3354 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poswap.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4111 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pot2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16451 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poterminology.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8052 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/poterminology_stopword_file.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3214 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/pretranslate.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7629 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/prop2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/rc2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4019 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/resx2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3908 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/sub2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5754 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/symb2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1638 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tbx2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2375 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tiki2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2544 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/tmserver.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/ts2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7056 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/txt2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3727 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/web2py2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3213 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/xliff2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/commands/yaml2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6572 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/conf.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1028 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/contents.rst.inc
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.497689 translate-toolkit-3.9.0/docs/developers/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1299 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/building.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3679 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/contributing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/deprecation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9692 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/developers.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11047 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/releasing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3174 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/reporting_bugs.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19038 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/styleguide.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9434 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/developers/testing.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2499 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/features.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.501689 translate-toolkit-3.9.0/docs/formats/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/android.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7698 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/base_classes.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2041 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/catkeys.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      707 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/conformance.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/csv.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1006 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/dtd.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3043 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/flatxml.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      451 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/flex.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      493 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/gsi.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/html.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ical.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7893 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      769 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ini.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      923 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/json.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      998 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/mo.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/mozilla_lang.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1549 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/odf.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      962 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/omegat_glossary.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7761 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/php.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1210 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1579 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/properties.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      888 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/qm.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/qt_phrase_book.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2078 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/quoting_and_escaping.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1281 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/rc.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1412 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/resx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/strings.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1360 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/subtitles.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2026 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/tbx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      800 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/text.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      810 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/tmx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1964 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/ts.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1216 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/utx.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wiki.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      316 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wml.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/wordfast.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/xliff.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      495 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/formats/yaml.rst
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.501689 translate-toolkit-3.9.0/docs/guides/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6603 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/checking_for_inconsistencies.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/cleanup_translator_comments.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2161 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/creating_mozilla_pot_files.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1960 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/document_translation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6258 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/migrating_translations.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1524 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/running_the_tools_on_microsoft_windows.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7596 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_csv2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_oo2po.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7736 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/guides/using_pofilter.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/history.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      237 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5263 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/installation.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/license.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5116 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/make.bat
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.509689 translate-toolkit-3.9.0/docs/releases/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.10.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2200 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.10.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1170 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.11.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      220 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.7.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.8.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      219 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4422 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/0.9.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.0.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6959 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4071 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      680 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.1.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4368 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.10.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4975 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.11.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5431 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.12.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.13.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2206 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.2.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      273 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      713 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      961 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.4.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.5.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      589 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.6.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      218 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.7.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      221 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.8.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3162 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.8.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/1.9.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8012 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.0.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1621 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1310 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      376 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      384 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1018 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      557 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.2.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2341 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.3.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1465 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1416 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/2.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1563 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.0.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1211 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.1.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      378 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.1.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      639 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.2.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      604 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      692 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      438 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      452 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.3.6.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      563 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.4.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      573 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.4.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      482 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      394 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.5.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      765 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      533 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      508 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.6.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      477 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      387 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      602 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      536 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.7.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      701 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      529 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.1.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      348 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.2.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      398 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.3.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      403 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.4.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      347 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.5.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      447 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.8.6.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      776 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/3.9.0.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1246 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/README.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/docs/releases/index.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      306 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/pyproject.toml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       41 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/pytest.ini
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.509689 translate-toolkit-3.9.0/requirements/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       47 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/dev.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/dist.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       18 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/lint.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      735 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/optional.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       71 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/required.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/requirements/test.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5951 2023-05-15 15:14:10.633689 translate-toolkit-3.9.0/setup.cfg
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2385 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/setup.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.473689 translate-toolkit-3.9.0/tests/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.517689 translate-toolkit-3.9.0/tests/cli/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.473689 translate-toolkit-3.9.0/tests/cli/data/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.517689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      460 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      813 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      212 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongkey/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      200 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongns/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongroot/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       57 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/one.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      210 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po_wrongvalue/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      846 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_failure/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      808 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       88 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2csv/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       61 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      118 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml/out.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.521689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      318 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_params/out.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       89 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      292 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/out.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      264 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_preserve/two.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       82 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      270 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/out.xml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      115 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2flatxml_template/two.xml
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2html/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       79 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/out.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       78 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2html/template.html
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       42 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/out.json
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       83 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/template.json
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      161 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2json_files_removeuntranslated/translations.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      145 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/out.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/template.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2prop_mozilla_files/translations.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.525689 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       85 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2ts/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       32 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_po2txt_threshold/out.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      206 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_mutually_exclusive/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_mutually_exclusive/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_nonexistant/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       74 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_nonexistant/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_csv/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_csv/one.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       43 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      430 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_file/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      492 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_fuzzy/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      101 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/plural.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_po_plurals/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1505 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/states.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      503 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.529689 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/states.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      504 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3337 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3421 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/stdout.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_posegment/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      370 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_posegment/one.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      388 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_posegment/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      130 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_comments/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       86 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/fr_af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       81 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_fr_af_reverse/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       52 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/af.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       54 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/fr.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       49 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_poswap_missing_units/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      322 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.533689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/one/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/one/a.properties
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/out/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      498 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/out/a.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      144 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_dirs/stderr.txt
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/one.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      506 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files/out.po
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/one.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      574 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/out.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       11 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/two.properties
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3564 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/one.rc
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1882 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/data/test_rc2po/out.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      727 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/example_test.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      226 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/run_tests.sh
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4775 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test.inc.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongkey.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongns.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      142 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongroot.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_flatxml2po_wrongvalue.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_junitmsgfmt_failure.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_junitmsgfmt_untranslated.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2csv.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      252 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_params.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      141 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_preserve.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      266 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2flatxml_template.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      137 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2html.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      167 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2json_files_removeuntranslated.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      168 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2prop_mozilla_files.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      122 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2ts.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      123 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2txt.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      194 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_po2txt_threshold.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      135 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_mutually_exclusive.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      109 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_nonexistant.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_po_file.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_po_fuzzy.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_xliff_states_no.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pocount_xliff_states_yes.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      113 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pofilter_listfilters.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      182 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_pofilter_manpage.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      126 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_posegment.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_comments.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_fr_af.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      160 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_fr_af_reverse.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_poswap_missing_units.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)       98 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      108 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_dirs.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      124 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_files.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      132 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_prop2po_files_templates.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      128 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/cli/test_rc2po.sh
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.537689 translate-toolkit-3.9.0/tests/odf_xliff/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3085 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   133081 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_2.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1864 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7300 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_inline.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5466 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/odf_xliff/test_odf_xliff.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.541689 translate-toolkit-3.9.0/tests/xliff_conformance/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    36103 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/af-pootle.po
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    30075 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/en-US.sdf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2257 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/test_xliff_conformance.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    96911 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tests/xliff_conformance/xliff-core-1.1.xsd
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.541689 translate-toolkit-3.9.0/tools/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.545689 translate-toolkit-3.9.0/tools/mozilla/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7012 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/README.firefox_build_instructions.rst
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4102 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/Vagrantfile
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3429 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/accesskey_checker
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2546 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/accesskey_checker_PO
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12855 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/build_firefox.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7178 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/build_tb3_langs.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9665 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/buildxpi.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      158 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/compare-locales.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4495 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/get_moz_enUS.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11342 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/moz-l10n-builder
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    23575 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/moz_l10n_builder.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2257 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozcronbuild.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1487 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozilla-l10n.patch
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12089 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/mozzy.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3208 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/postinstall.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      497 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/mozilla/setup_mozilla.sh
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18996 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/phase
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      626 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/phaselist2goals
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1041 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pocommentclean
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4683 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pocompendium
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5288 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/pomigrate2
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1852 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/popuretext
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/poreencode
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1526 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/tools/posplit
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.545689 translate-toolkit-3.9.0/translate/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1816 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1406 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/__version__.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.565689 translate-toolkit-3.9.0/translate/convert/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      790 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/accesskey.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    20603 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/convert.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    10171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/csv2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/csv2tbx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13191 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/dtd2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7541 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/factory.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3663 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/flatxml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5523 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/html2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4527 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ical2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1902 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/idml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5078 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ini2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5180 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/json2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2358 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/moz2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4922 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/mozfunny2prop.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3981 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/mozlang2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3839 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/odf2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      357 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/odfxml
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7936 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/oo2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     7286 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/oo2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4536 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/php2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3950 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2csv.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8688 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2dtd.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5083 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2flatxml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6792 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2html.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3617 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ical.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6806 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2idml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ini.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3682 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2json.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3490 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2moz.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3702 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2mozlang.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11233 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2oo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3374 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2php.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2prop.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13213 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2rc.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2resx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2sub.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4085 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2symb.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3227 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2tiki.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5569 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2tmx.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3228 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2ts.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5171 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2txt.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2559 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2web2py.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4185 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2wordfast.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2xliff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3949 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/po2yaml.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12222 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/pot2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/prop2mozfunny.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    18818 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/prop2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5941 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/rc2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     6038 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/resx2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1730 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-OOo
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1629 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-gaia
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     1589 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/roundtrip-mozilla
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4776 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/sub2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4101 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/symb2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2352 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/tbx2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   189411 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test.idml
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11608 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test.odt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_accesskey.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5372 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_convert.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6225 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_csv2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19205 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_dtd2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4744 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_flatxml2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27945 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_html2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12076 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ical2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      449 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_idml2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4543 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ini2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2472 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_json2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      414 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_moz2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2179 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_mozfunny2prop.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4733 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_mozlang2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      446 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ods2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13063 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_oo2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2989 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_oo2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11579 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_php2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2csv.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22148 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4617 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11889 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10814 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ical.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      826 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2idml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3853 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2json.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      494 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2moz.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5024 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2mozlang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9663 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10874 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2php.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17564 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2prop.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9084 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    18992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2151 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2sub.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2097 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6522 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4373 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5238 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2web2py.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6837 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_po2yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27471 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_pot2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2201 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_prop2mozfunny.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14486 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_prop2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4827 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_rc2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10049 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_resx2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2362 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_tiki2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4628 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_ts2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8333 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_txt2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1823 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_web2py2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      942 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_xliff2odf.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12996 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_xliff2po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/test_yaml2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3144 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/tiki2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3774 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/ts2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4682 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/txt2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2757 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/web2py2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5947 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2odf.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    11230 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2oo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4049 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/xliff2po.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4458 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/convert/yaml2po.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.569689 translate-toolkit-3.9.0/translate/filters/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      766 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2440 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/autocorrect.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   101819 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/checks.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/decoration.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/decorators.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2796 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/helpers.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    13302 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/pofilter.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/prefilters.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2153 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/spelling.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2531 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_autocorrect.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)   108937 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_checks.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4060 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_decoration.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13635 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_pofilter.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1065 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/filters/test_prefilters.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.585689 translate-toolkit-3.9.0/translate/lang/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3868 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/af.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      925 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ak.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1513 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/am.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2090 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/az.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2096 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/bn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/bo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1458 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/code_as.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1551 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/code_or.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13174 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/common.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1081 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/da.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    27413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/data.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/de.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      976 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/dz.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1949 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/el.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1782 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/es.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2488 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      985 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2849 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/fr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      969 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/gd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/gu.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      983 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/he.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      974 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/hi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1821 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/hy.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4934 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/identify.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1699 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ja.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1977 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/km.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/kn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ko.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      973 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/kw.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/lo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      986 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      980 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/mr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      967 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ms.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1042 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/my.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1637 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ne.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4893 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ngram.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1413 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/nqo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/nso.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1614 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1079 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pl.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5968 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/poedit.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1100 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/pt_BR.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2828 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ro.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5382 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/scn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      992 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/si.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      963 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/son.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      940 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/st.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      979 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/su.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1080 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/sv.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      978 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ta.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      971 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/te.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    21016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/team.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)      707 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test-language-teams.sh
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1690 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_af.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1119 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_am.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1388 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5162 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_common.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_data.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1417 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_el.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1273 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_es.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2815 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_fa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1918 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_fr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1448 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_hy.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6480 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_identify.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1116 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ja.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1829 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_km.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1094 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ko.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2963 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ne.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1751 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_nqo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1639 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_or.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      705 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_poedit.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1737 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_ro.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_scn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      775 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_team.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_th.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      405 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_tr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      328 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_uk.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1426 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_vi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1008 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/test_zh.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1181 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/th.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1025 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/tr.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1091 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ug.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1186 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ur.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      952 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/ve.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1532 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/vi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/wo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2367 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1016 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_cn.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_hk.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/lang/zh_tw.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/misc/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      838 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1610 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/deprecation.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2733 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/dictutils.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2580 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/file_discovery.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3010 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/multistring.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    33419 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/optrecurse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10453 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/ourdom.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4655 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/progressbar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17756 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/quote.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17681 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/selector.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      465 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_deprecation.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_dictutils.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3052 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_multistring.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1133 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_optrecurse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      419 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_progressbar.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7634 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_quote.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1209 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/test_xml_helpers.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1424 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/wStringIO.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1138 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/wsgi.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/misc/xml_helpers.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/search/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      772 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6056 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/lshtein.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15948 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/match.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1754 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1866 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_lshtein.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5705 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_match.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      307 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/search/test_terminology.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/services/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      833 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1855 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/test_tmserver.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8293 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/services/tmserver.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.589689 translate-toolkit-3.9.0/translate/share/
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.601689 translate-toolkit-3.9.0/translate/share/langmodels/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1449 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Ndebele.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/NorthernSotho.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1071 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/README
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Sotho.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1463 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Swati.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1447 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Tsonga.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1475 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Tswana.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1457 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Venda.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1421 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Xhosa.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1464 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/Zulu.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3387 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/afrikaans.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/albanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2325 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/arabic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3243 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/basque.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/belarus.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/bosnian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3287 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/breton.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3223 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/catalan.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2089 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/chinese_simplified.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1991 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/chinese_traditional.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3428 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/croatian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3369 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/czech.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3375 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/danish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3384 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/dutch.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3317 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/english.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/esperanto.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3315 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/estonian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3425 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/finnish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3687 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/fpdb.conf
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3355 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/french.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3443 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/frisian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3444 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/german.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4266 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/greek.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4187 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/hebrew.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3353 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/hungarian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3475 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/icelandic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3359 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/indonesian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3178 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/irish_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3426 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/italian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2309 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/japanese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3324 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/latin.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3500 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/latvian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3350 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/lithuanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3597 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/malay.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3462 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/manx_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3408 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/norwegian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3416 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/polish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3467 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/portuguese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3205 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/quechua.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/romanian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3117 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/romansh.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/russian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3131 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/scots.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3323 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/scots_gaelic.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/serbian_ascii.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/slovak_ascii.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3152 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/slovenian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3417 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/spanish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3314 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/swahili.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3484 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/swedish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3261 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/tagalog.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3539 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/turkish.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2172 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/ukrainian.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3689 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/vietnamese.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3535 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/langmodels/welsh.lm
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8740 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/share/stoplist-en
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.621689 translate-toolkit-3.9.0/translate/storage/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      786 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1324 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/_factory_classes.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    22457 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/aresource.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    34064 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7514 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/benchmark.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10410 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/bundleprojstore.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10970 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/catkeys.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    37641 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/cpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11481 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/csvl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      338 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/debug.properties
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2383 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/directory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    24352 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8762 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8204 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    24555 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/fluent.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    19719 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/fpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17147 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4972 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ical.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2846 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/idml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4515 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25065 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/jsonl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13083 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10982 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/mo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5500 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/mozilla_lang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1165 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/odf_io.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5390 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/odf_shared.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6139 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/omegat.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15688 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    18547 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/php.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.621689 translate-toolkit-3.9.0/translate/storage/placeables/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2004 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2962 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13901 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/general.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1241 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/interfaces.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7195 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3269 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/parse.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    35646 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/strelem.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3297 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8107 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10622 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_general.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6121 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_lisa.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2029 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/test_terminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3991 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/placeables/xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1693 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7092 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/pocommon.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16276 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poheader.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13215 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poparser.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    12932 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/poxliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9143 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/project.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14695 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/projstore.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      753 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/properties.java
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    43632 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/properties.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    37283 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8559 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/qm.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5127 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/qph.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    16053 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1649 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/resourcedictionary.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8538 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7567 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/statistics.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6662 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/stringsdict.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7652 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/subtitles.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2234 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/symbian.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4531 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tbx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    30744 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_aresource.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14765 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_base.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2492 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_catkeys.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9086 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_cpo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5570 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_csvl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2798 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_directory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    21418 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_dtd.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6704 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_factory.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3869 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_flatxml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    71615 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_fluent.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9820 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_html.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      483 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ini.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    28694 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_jsonl10n.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8420 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_mo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1296 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_monolingual.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_mozilla_lang.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      501 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_omegat.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6658 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_oo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    44427 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_php.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    38517 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_po.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      675 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_pocommon.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11275 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_poheader.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5392 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_poxliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    64201 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_properties.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    22936 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1198 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_qm.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3239 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_qph.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    18737 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_rc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1928 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_resourcedictionary.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5022 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_resx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6114 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_stringsdict.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      743 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_subtitles.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3558 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tbx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3146 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3916 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      882 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_trados.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      211 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13697 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_ts2.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2002 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      207 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_utx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2847 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_wordfast.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    25248 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_xliff.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15664 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2697 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/test_zip.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6986 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tiki.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    13004 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tmdb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5845 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/tmx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6409 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/trados.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     6935 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ts.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    17854 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/ts2.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4994 2023-05-15 15:11:37.000000 translate-toolkit-3.9.0/translate/storage/txt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     9488 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/utx.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    15187 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/wordfast.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8786 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/workflow.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    33543 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xliff.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.625689 translate-toolkit-3.9.0/translate/storage/xml_extract/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      716 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/__init__.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14635 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/extract.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11240 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/generate.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2825 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/misc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2166 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_misc.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2955 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_unit_tree.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1205 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/test_xpath_breadcrumb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     4854 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/unit_tree.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2230 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_extract/xpath_breadcrumb.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2677 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/xml_name.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     7211 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/yaml.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     2276 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/storage/zip.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate/tools/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      777 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__init__.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate/tools/__snapshots__/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1871 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__snapshots__/test_junitmsgfmt.ambr
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10626 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/__snapshots__/test_pocount.ambr
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      301 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/_test_utils.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3350 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/build_tmdb.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2844 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/junitmsgfmt.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3415 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/phppo2pypo.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     2363 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poclean.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3408 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pocompile.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     8679 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poconflicts.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    19130 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pocount.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    16454 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/podebug.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    14678 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pogrep.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5292 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pomerge.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     5643 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/porestructure.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     4954 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/posegment.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3720 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poswap.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    25251 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/poterminology.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     9213 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pretranslate.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)    12659 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pydiff.py
+-rwxr-xr-x   0 nijel     (1000) nijel     (1000)     3384 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/pypo2phppo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      714 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_help.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      548 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_junitmsgfmt.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1710 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_phppo2pypo.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     5751 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pocount.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    11912 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_podebug.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     8182 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pogrep.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    23743 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pomerge.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3529 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_posegment.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      945 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_poterminology.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    14618 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pretranslate.py
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     1709 2023-05-15 15:11:38.000000 translate-toolkit-3.9.0/translate/tools/test_pypo2phppo.py
+drwxr-xr-x   0 nijel     (1000) nijel     (1000)        0 2023-05-15 15:14:10.629689 translate-toolkit-3.9.0/translate_toolkit.egg-info/
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    10835 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 nijel     (1000) nijel     (1000)    28961 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)     3197 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)        1 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 nijel     (1000) nijel     (1000)      629 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/requires.txt
+-rw-r--r--   0 nijel     (1000) nijel     (1000)       10 2023-05-15 15:14:10.000000 translate-toolkit-3.9.0/translate_toolkit.egg-info/top_level.txt
```

### Comparing `translate-toolkit-3.8.6/.github/workflows/docs.yml` & `translate-toolkit-3.9.0/.github/workflows/docs.yml`

 * *Files 23% similar despite different names*

```diff
@@ -21,17 +21,19 @@
         submodules: recursive
     - name: Setup Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.11'
         cache: pip
         cache-dependency-path: requirements/*.txt
+    - name: Configure Fast APT Mirror
+      uses: vegardit/fast-apt-mirror.sh@v1
     - name: Install apt dependencies
       run: |
-        sudo apt-get --option="APT::Acquire::Retries=3 update
-        sudo apt-get --option="APT::Acquire::Retries=3 install -y libgettextpo-dev
+        sudo apt-get update
+        sudo apt-get install -y libgettextpo-dev
     - name: Install dependencies
       run: |
         pip install --upgrade pip wheel
         pip install -r requirements/dev.txt
     - name: Build docs
       run: make docs
```

### Comparing `translate-toolkit-3.8.6/.github/workflows/linux.yml` & `translate-toolkit-3.9.0/.github/workflows/linux.yml`

 * *Files 15% similar despite different names*

```diff
@@ -35,18 +35,20 @@
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
         cache: pip
         cache-dependency-path: requirements/*.txt
+    - name: Configure Fast APT Mirror
+      uses: vegardit/fast-apt-mirror.sh@v1
     - name: Install apt dependencies
       run: |
-        sudo apt-get --option="APT::Acquire::Retries=3" update
-        sudo apt-get --option="APT::Acquire::Retries=3" install -y libgettextpo-dev libxml2-dev libxmlsec1-dev gettext hunspell-af
+        sudo apt-get update
+        sudo apt-get install -y libgettextpo-dev libxml2-dev libxmlsec1-dev gettext hunspell-af
     - name: Update pip
       run: pip install --upgrade pip wheel
     - name: Install pip dependencies
       run: pip install -r requirements/test.txt
     - name: Install pip dependencies
       if: matrix.requirements == 'minimal'
       run: |
```

### Comparing `translate-toolkit-3.8.6/.github/workflows/osx.yml` & `translate-toolkit-3.9.0/.github/workflows/osx.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/.github/workflows/pre-commit.yml` & `translate-toolkit-3.9.0/.github/workflows/pre-commit.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/.github/workflows/setup.yml` & `translate-toolkit-3.9.0/.github/workflows/setup.yml`

 * *Files 20% similar despite different names*

```diff
@@ -21,18 +21,20 @@
         submodules: recursive
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.11'
         cache: pip
         cache-dependency-path: requirements/*.txt
+    - name: Configure Fast APT Mirror
+      uses: vegardit/fast-apt-mirror.sh@v1
     - name: Install apt dependencies
       run: |
-        sudo apt-get --option="APT::Acquire::Retries=3 update
-        sudo apt-get --option="APT::Acquire::Retries=3 install -y libgettextpo-dev
+        sudo apt-get update
+        sudo apt-get install -y libgettextpo-dev
     - name: Update pip
       run: pip install --upgrade pip wheel
     - name: Install pip dependencies
       run: |
         pip install -r requirements/dev.txt
     - name: Build sdist
       run: make build
```

### Comparing `translate-toolkit-3.8.6/.github/workflows/win.yml` & `translate-toolkit-3.9.0/.github/workflows/win.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/.gitignore` & `translate-toolkit-3.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/.pre-commit-config.yaml` & `translate-toolkit-3.9.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -3,32 +3,38 @@
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
   hooks:
   - id: check-yaml
   - id: check-merge-conflict
   - id: check-json
+  - id: check-toml
   - id: requirements-txt-fixer
   - id: fix-encoding-pragma
     args: [--remove]
+- repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
+  rev: v2.8.0
+  hooks:
+  - id: pretty-format-toml
+    args: [--autofix]
 - repo: meta
   hooks:
   - id: check-hooks-apply
   - id: check-useless-excludes
 - repo: https://github.com/pycqa/isort
   rev: 5.12.0
   hooks:
   - id: isort
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
+  rev: v3.4.0
   hooks:
   - id: pyupgrade
     args: [--py36-plus]
 - repo: https://github.com/psf/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/PyCQA/flake8
   rev: 6.0.0
   hooks:
   - id: flake8
     additional_dependencies:
@@ -36,11 +42,11 @@
     - flake8-mutable
     - flake8-polyfill
 - repo: https://github.com/PyCQA/pydocstyle
   rev: 6.3.0
   hooks:
   - id: pydocstyle
 - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-  rev: v2.7.0
+  rev: v2.8.0
   hooks:
   - id: pretty-format-yaml
     args: [--autofix, --indent, '2']
```

### Comparing `translate-toolkit-3.8.6/.readthedocs.yml` & `translate-toolkit-3.9.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/COPYING` & `translate-toolkit-3.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/CREDITS` & `translate-toolkit-3.9.0/CREDITS`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/Makefile` & `translate-toolkit-3.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/PKG-INFO` & `translate-toolkit-3.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-toolkit
-Version: 3.8.6
+Version: 3.9.0
 Summary: Tools and API for translation and localization engineering.
 Home-page: https://toolkit.translatehouse.org/
 Download-URL: https://github.com/translate/translate/releases/
 Author: Translate
 Author-email: translate-devel@lists.sourceforge.net
 License: GPL-2.0-or-later
 Project-URL: Issue Tracker, https://github.com/translate/translate/issues
```

### Comparing `translate-toolkit-3.8.6/README.rst` & `translate-toolkit-3.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/Makefile` & `translate-toolkit-3.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_ext/translate_docs.py` & `translate-toolkit-3.9.0/docs/_ext/translate_docs.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/README.rst` & `translate-toolkit-3.9.0/docs/_themes/README.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/layout.html` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/layout.html`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/search.html` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/search.html`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-responsive.css`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap.css` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.css`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/bootstrap.js` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/bootstrap.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/font/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/jquery.js` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/jquery.js`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/font-awesome.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/theme.less` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/theme.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/_themes/sphinx-bootstrap/static/less/variables.less` & `translate-toolkit-3.9.0/docs/_themes/sphinx-bootstrap/static/less/variables.less`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/convert.rst` & `translate-toolkit-3.9.0/docs/api/convert.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/filters.rst` & `translate-toolkit-3.9.0/docs/api/filters.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/index.rst` & `translate-toolkit-3.9.0/docs/api/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/lang.rst` & `translate-toolkit-3.9.0/docs/api/lang.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/misc.rst` & `translate-toolkit-3.9.0/docs/api/misc.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/storage.rst` & `translate-toolkit-3.9.0/docs/api/storage.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/api/tools.rst` & `translate-toolkit-3.9.0/docs/api/tools.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/csv2po.rst` & `translate-toolkit-3.9.0/docs/commands/csv2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/csv2tbx.rst` & `translate-toolkit-3.9.0/docs/commands/csv2tbx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/flatxml2po.rst` & `translate-toolkit-3.9.0/docs/commands/flatxml2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/general_usage.rst` & `translate-toolkit-3.9.0/docs/commands/general_usage.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/html2po.rst` & `translate-toolkit-3.9.0/docs/commands/html2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/ical2po.rst` & `translate-toolkit-3.9.0/docs/commands/ical2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/index.rst` & `translate-toolkit-3.9.0/docs/commands/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/ini2po.rst` & `translate-toolkit-3.9.0/docs/commands/ini2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/json2po.rst` & `translate-toolkit-3.9.0/docs/commands/json2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/levenshtein_distance.rst` & `translate-toolkit-3.9.0/docs/commands/levenshtein_distance.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/moz-l10n-builder.rst` & `translate-toolkit-3.9.0/docs/commands/moz-l10n-builder.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/moz2po.rst` & `translate-toolkit-3.9.0/docs/commands/moz2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/mozilla_l10n_scripts.rst` & `translate-toolkit-3.9.0/docs/commands/mozilla_l10n_scripts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/odf2xliff.rst` & `translate-toolkit-3.9.0/docs/commands/odf2xliff.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/oo2po.rst` & `translate-toolkit-3.9.0/docs/commands/oo2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_accelerator.rst` & `translate-toolkit-3.9.0/docs/commands/option_accelerator.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_duplicates.rst` & `translate-toolkit-3.9.0/docs/commands/option_duplicates.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_errorlevel.rst` & `translate-toolkit-3.9.0/docs/commands/option_errorlevel.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_filteraction.rst` & `translate-toolkit-3.9.0/docs/commands/option_filteraction.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_multifile.rst` & `translate-toolkit-3.9.0/docs/commands/option_multifile.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_personality.rst` & `translate-toolkit-3.9.0/docs/commands/option_personality.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_progress.rst` & `translate-toolkit-3.9.0/docs/commands/option_progress.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/option_rewrite.rst` & `translate-toolkit-3.9.0/docs/commands/option_rewrite.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/phase.rst` & `translate-toolkit-3.9.0/docs/commands/phase.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/php2po.rst` & `translate-toolkit-3.9.0/docs/commands/php2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/po2tmx.rst` & `translate-toolkit-3.9.0/docs/commands/po2tmx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/po2wordfast.rst` & `translate-toolkit-3.9.0/docs/commands/po2wordfast.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poclean.rst` & `translate-toolkit-3.9.0/docs/commands/poclean.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pocommentclean.rst` & `translate-toolkit-3.9.0/docs/commands/pocommentclean.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pocompendium.rst` & `translate-toolkit-3.9.0/docs/commands/pocompendium.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pocompile.rst` & `translate-toolkit-3.9.0/docs/commands/pocompile.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poconflicts.rst` & `translate-toolkit-3.9.0/docs/commands/poconflicts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pocount.rst` & `translate-toolkit-3.9.0/docs/commands/pocount.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/podebug.rst` & `translate-toolkit-3.9.0/docs/commands/podebug.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pofilter.rst` & `translate-toolkit-3.9.0/docs/commands/pofilter.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pofilter_tests.rst` & `translate-toolkit-3.9.0/docs/commands/pofilter_tests.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pogrep.rst` & `translate-toolkit-3.9.0/docs/commands/pogrep.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pomerge.rst` & `translate-toolkit-3.9.0/docs/commands/pomerge.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pomigrate2.rst` & `translate-toolkit-3.9.0/docs/commands/pomigrate2.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/popuretext.rst` & `translate-toolkit-3.9.0/docs/commands/popuretext.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poreencode.rst` & `translate-toolkit-3.9.0/docs/commands/poreencode.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/porestructure.rst` & `translate-toolkit-3.9.0/docs/commands/porestructure.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/posegment.rst` & `translate-toolkit-3.9.0/docs/commands/posegment.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/posplit.rst` & `translate-toolkit-3.9.0/docs/commands/posplit.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poswap.rst` & `translate-toolkit-3.9.0/docs/commands/poswap.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pot2po.rst` & `translate-toolkit-3.9.0/docs/commands/pot2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poterminology.rst` & `translate-toolkit-3.9.0/docs/commands/poterminology.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/poterminology_stopword_file.rst` & `translate-toolkit-3.9.0/docs/commands/poterminology_stopword_file.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/pretranslate.rst` & `translate-toolkit-3.9.0/docs/commands/pretranslate.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/prop2po.rst` & `translate-toolkit-3.9.0/docs/commands/prop2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/rc2po.rst` & `translate-toolkit-3.9.0/docs/commands/rc2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/resx2po.rst` & `translate-toolkit-3.9.0/docs/commands/resx2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/sub2po.rst` & `translate-toolkit-3.9.0/docs/commands/sub2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/symb2po.rst` & `translate-toolkit-3.9.0/docs/commands/symb2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/tbx2po.rst` & `translate-toolkit-3.9.0/docs/commands/tbx2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/tiki2po.rst` & `translate-toolkit-3.9.0/docs/commands/tiki2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/tmserver.rst` & `translate-toolkit-3.9.0/docs/commands/tmserver.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/ts2po.rst` & `translate-toolkit-3.9.0/docs/commands/ts2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/txt2po.rst` & `translate-toolkit-3.9.0/docs/commands/txt2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/web2py2po.rst` & `translate-toolkit-3.9.0/docs/commands/web2py2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/xliff2po.rst` & `translate-toolkit-3.9.0/docs/commands/xliff2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/commands/yaml2po.rst` & `translate-toolkit-3.9.0/docs/commands/yaml2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/conf.py` & `translate-toolkit-3.9.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,26 +9,25 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-
 sys.path.insert(0, os.path.abspath("_ext"))
 sys.path.insert(0, os.path.abspath("."))
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- Project information -----------------------------------------------------
 
 project = "Translate Toolkit"
 copyright = "2002-2023, Translate"
 
 # The short X.Y version.
-version = "3.8.6"
+version = "3.9.0"
 
 # The full version, including alpha/beta/rc tags
 release = version
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
```

### Comparing `translate-toolkit-3.8.6/docs/contents.rst.inc` & `translate-toolkit-3.9.0/docs/contents.rst.inc`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/building.rst` & `translate-toolkit-3.9.0/docs/developers/building.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/contributing.rst` & `translate-toolkit-3.9.0/docs/developers/contributing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/deprecation.rst` & `translate-toolkit-3.9.0/docs/developers/deprecation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/developers.rst` & `translate-toolkit-3.9.0/docs/developers/developers.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/releasing.rst` & `translate-toolkit-3.9.0/docs/developers/releasing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/reporting_bugs.rst` & `translate-toolkit-3.9.0/docs/developers/reporting_bugs.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/styleguide.rst` & `translate-toolkit-3.9.0/docs/developers/styleguide.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/developers/testing.rst` & `translate-toolkit-3.9.0/docs/developers/testing.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/features.rst` & `translate-toolkit-3.9.0/docs/features.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/android.rst` & `translate-toolkit-3.9.0/docs/formats/android.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/base_classes.rst` & `translate-toolkit-3.9.0/docs/formats/base_classes.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/catkeys.rst` & `translate-toolkit-3.9.0/docs/formats/catkeys.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/conformance.rst` & `translate-toolkit-3.9.0/docs/formats/conformance.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/csv.rst` & `translate-toolkit-3.9.0/docs/formats/csv.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/dtd.rst` & `translate-toolkit-3.9.0/docs/formats/dtd.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/flatxml.rst` & `translate-toolkit-3.9.0/docs/formats/flatxml.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/html.rst` & `translate-toolkit-3.9.0/docs/formats/html.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/ical.rst` & `translate-toolkit-3.9.0/docs/formats/ical.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/index.rst` & `translate-toolkit-3.9.0/docs/formats/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/ini.rst` & `translate-toolkit-3.9.0/docs/formats/ini.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/json.rst` & `translate-toolkit-3.9.0/docs/formats/json.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/mo.rst` & `translate-toolkit-3.9.0/docs/formats/mo.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/odf.rst` & `translate-toolkit-3.9.0/docs/formats/odf.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/omegat_glossary.rst` & `translate-toolkit-3.9.0/docs/formats/omegat_glossary.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/php.rst` & `translate-toolkit-3.9.0/docs/formats/php.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/po.rst` & `translate-toolkit-3.9.0/docs/formats/po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/properties.rst` & `translate-toolkit-3.9.0/docs/formats/properties.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/qm.rst` & `translate-toolkit-3.9.0/docs/formats/qm.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/qt_phrase_book.rst` & `translate-toolkit-3.9.0/docs/formats/qt_phrase_book.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/quoting_and_escaping.rst` & `translate-toolkit-3.9.0/docs/formats/quoting_and_escaping.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/rc.rst` & `translate-toolkit-3.9.0/docs/formats/rc.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/resx.rst` & `translate-toolkit-3.9.0/docs/formats/resx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/strings.rst` & `translate-toolkit-3.9.0/docs/formats/strings.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/subtitles.rst` & `translate-toolkit-3.9.0/docs/formats/subtitles.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/tbx.rst` & `translate-toolkit-3.9.0/docs/formats/tbx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/text.rst` & `translate-toolkit-3.9.0/docs/formats/text.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/tmx.rst` & `translate-toolkit-3.9.0/docs/formats/tmx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/ts.rst` & `translate-toolkit-3.9.0/docs/formats/ts.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/utx.rst` & `translate-toolkit-3.9.0/docs/formats/utx.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/wiki.rst` & `translate-toolkit-3.9.0/docs/formats/wiki.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/wordfast.rst` & `translate-toolkit-3.9.0/docs/formats/wordfast.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/formats/xliff.rst` & `translate-toolkit-3.9.0/docs/formats/xliff.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/checking_for_inconsistencies.rst` & `translate-toolkit-3.9.0/docs/guides/checking_for_inconsistencies.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/cleanup_translator_comments.rst` & `translate-toolkit-3.9.0/docs/guides/cleanup_translator_comments.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst` & `translate-toolkit-3.9.0/docs/guides/creating_a_terminology_list_from_your_existing_translations.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/creating_mozilla_pot_files.rst` & `translate-toolkit-3.9.0/docs/guides/creating_mozilla_pot_files.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/document_translation.rst` & `translate-toolkit-3.9.0/docs/guides/document_translation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/index.rst` & `translate-toolkit-3.9.0/docs/guides/index.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/migrating_translations.rst` & `translate-toolkit-3.9.0/docs/guides/migrating_translations.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/running_the_tools_on_microsoft_windows.rst` & `translate-toolkit-3.9.0/docs/guides/running_the_tools_on_microsoft_windows.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/using_csv2po.rst` & `translate-toolkit-3.9.0/docs/guides/using_csv2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/using_oo2po.rst` & `translate-toolkit-3.9.0/docs/guides/using_oo2po.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/guides/using_pofilter.rst` & `translate-toolkit-3.9.0/docs/guides/using_pofilter.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/history.rst` & `translate-toolkit-3.9.0/docs/history.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/installation.rst` & `translate-toolkit-3.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/make.bat` & `translate-toolkit-3.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/0.10.rst` & `translate-toolkit-3.9.0/docs/releases/0.10.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/0.11.rst` & `translate-toolkit-3.9.0/docs/releases/0.11.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/0.9.rst` & `translate-toolkit-3.9.0/docs/releases/0.9.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.0.1.rst` & `translate-toolkit-3.9.0/docs/releases/1.0.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.1.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.1.1.rst` & `translate-toolkit-3.9.0/docs/releases/1.1.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.10.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.10.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.11.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.11.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.12.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.12.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.13.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.13.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.2.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.4.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.4.1.rst` & `translate-toolkit-3.9.0/docs/releases/1.4.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.6.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.6.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.8.1.rst` & `translate-toolkit-3.9.0/docs/releases/1.8.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/1.9.0.rst` & `translate-toolkit-3.9.0/docs/releases/1.9.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.0.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.0.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.1.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.2.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.2.1.rst` & `translate-toolkit-3.9.0/docs/releases/2.2.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.2.4.rst` & `translate-toolkit-3.9.0/docs/releases/2.2.4.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.2.5.rst` & `translate-toolkit-3.9.0/docs/releases/2.2.5.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.3.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.3.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.3.1.rst` & `translate-toolkit-3.9.0/docs/releases/2.3.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.4.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.5.0.rst` & `translate-toolkit-3.9.0/docs/releases/2.5.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/2.5.1.rst` & `translate-toolkit-3.9.0/docs/releases/2.5.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.0.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.0.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.1.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.1.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.2.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.2.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.3.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.3.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.3.2.rst` & `translate-toolkit-3.9.0/docs/releases/3.3.2.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.3.3.rst` & `translate-toolkit-3.9.0/docs/releases/3.3.3.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.4.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.4.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.4.1.rst` & `translate-toolkit-3.9.0/docs/releases/3.4.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.6.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.6.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.6.1.rst` & `translate-toolkit-3.9.0/docs/releases/3.6.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.7.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.7.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.7.3.rst` & `translate-toolkit-3.9.0/docs/releases/3.7.3.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.7.4.rst` & `translate-toolkit-3.9.0/docs/releases/3.7.4.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.8.0.rst` & `translate-toolkit-3.9.0/docs/releases/3.8.0.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/3.8.1.rst` & `translate-toolkit-3.9.0/docs/releases/3.8.1.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/README.rst` & `translate-toolkit-3.9.0/docs/releases/README.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/docs/releases/index.rst` & `translate-toolkit-3.9.0/docs/releases/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 Final releases
 ==============
 
 .. toctree::
    :maxdepth: 1
 
+   3.9.0 <3.9.0>
    3.8.6 <3.8.6>
    3.8.5 <3.8.5>
    3.8.4 <3.8.4>
    3.8.3 <3.8.3>
    3.8.2 <3.8.2>
    3.8.1 <3.8.1>
    3.8.0 <3.8.0>
```

### Comparing `translate-toolkit-3.8.6/requirements/optional.txt` & `translate-toolkit-3.9.0/requirements/optional.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 # Format support
 BeautifulSoup4>=4.3  # Trados
 # Encoding detection
 charset-normalizer==3.1.0   # chardet
 # Tmserver backend
 cheroot==9.0.0       # tmserver
 # Format support
-fluent.syntax==0.18.1 # Fluent
+fluent.syntax==0.19.0 # Fluent
 # Format support
 iniparse==0.5        # INI
 # Format support
 phply==1.2.6         # PHP
 # To provide translations for language names without need for OS package.
 pycountry==22.3.5          # Languages
 pyenchant==3.2.2     # spellcheck
 # Windows Resources (rc2po and po2rc)
 pyparsing==3.0.9     # RC
 # Faster matching in e.g. pot2po
 python-Levenshtein>=0.12    # Levenshtein
 # Format support
-ruamel.yaml==0.17.21 # YAML
+ruamel.yaml==0.17.26 # YAML
 # Format support
 vobject==0.9.6.1     # iCal
```

### Comparing `translate-toolkit-3.8.6/setup.cfg` & `translate-toolkit-3.9.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 
 [options]
 packages = find_namespace:
 python_requires = >=3.7
 include_package_data = 1
 zip_safe = 0
 scripts = 
-	tools/junitmsgfmt
 	tools/mozilla/build_firefox.sh
 	tools/mozilla/buildxpi.py
 	tools/mozilla/get_moz_enUS.py
 	tools/pocommentclean
 	tools/pocompendium
 	tools/pomigrate2
 	tools/popuretext
@@ -65,14 +64,15 @@
 	dtd2po = translate.convert.dtd2po:main
 	flatxml2po = translate.convert.flatxml2po:main
 	html2po = translate.convert.html2po:main
 	ical2po = translate.convert.ical2po:main
 	idml2po = translate.convert.idml2po:main
 	ini2po = translate.convert.ini2po:main
 	json2po = translate.convert.json2po:main
+	junitmsgfmt = translate.tools.junitmsgfmt:main
 	mozfunny2prop = translate.convert.mozfunny2prop:main
 	mozlang2po = translate.convert.mozlang2po:main
 	moz2po = translate.convert.moz2po:main
 	odf2xliff = translate.convert.odf2xliff:main
 	oo2po = translate.convert.oo2po:main
 	oo2xliff = translate.convert.oo2xliff:main
 	php2po = translate.convert.php2po:main
@@ -154,27 +154,11 @@
 ignore = E203,E129,E226,E402,E731,W503,N,E265,E501,E266,E741,W504
 statistics = True
 per-file-ignores = 
 	translate/storage/placeables/__init__.py:F401,F403
 	translate/storage/po.py:F401,F403
 	translate/storage/wordfast.py:E262
 
-[isort]
-multi_line_output = 3
-include_trailing_comma = True
-force_grid_wrap = 0
-use_parentheses = True
-ensure_newline_before_comments = True
-line_length = 88
-known_standard_library = 
-known_third_party = iniparse,lxml,vobject,sphinx,pytest,cheroot,phply,bs4,ruamel,pyparsing,setuptools
-known_first_party = translate
-default_section = FIRSTPARTY
-sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
-order_by_type = True
-combine_as_imports = True
-lines_after_imports = 2
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `translate-toolkit-3.8.6/setup.py` & `translate-toolkit-3.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_flatxml2po/out.po` & `translate-toolkit-3.9.0/tests/cli/data/test_flatxml2po/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_no/states.xlf` & `translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_no/states.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_pocount_xliff_states_yes/states.xlf` & `translate-toolkit-3.9.0/tests/cli/data/test_pocount_xliff_states_yes/states.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_pofilter_listfilters/stdout.txt` & `translate-toolkit-3.9.0/tests/cli/data/test_pofilter_listfilters/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_pofilter_manpage/stdout.txt` & `translate-toolkit-3.9.0/tests/cli/data/test_pofilter_manpage/stdout.txt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_prop2po_files_templates/out.po` & `translate-toolkit-3.9.0/tests/cli/data/test_prop2po_files_templates/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_rc2po/one.rc` & `translate-toolkit-3.9.0/tests/cli/data/test_rc2po/one.rc`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/data/test_rc2po/out.po` & `translate-toolkit-3.9.0/tests/cli/data/test_rc2po/out.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/example_test.sh` & `translate-toolkit-3.9.0/tests/cli/example_test.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/cli/test.inc.sh` & `translate-toolkit-3.9.0/tests/cli/test.inc.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf` & `translate-toolkit-3.9.0/tests/odf_xliff/test_2-test_odf2xliff-reference.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/odf_xliff/test_2.odt` & `translate-toolkit-3.9.0/tests/odf_xliff/test_2.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf` & `translate-toolkit-3.9.0/tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/odf_xliff/test_inline.odt` & `translate-toolkit-3.9.0/tests/odf_xliff/test_inline.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/odf_xliff/test_odf_xliff.py` & `translate-toolkit-3.9.0/tests/odf_xliff/test_odf_xliff.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import os
 import os.path as path
 import sys
 import zipfile
 
 from lxml import etree
 
-
 # get directory of this test
 dir = os.path.dirname(os.path.abspath(__file__))
 # get top-level directory (moral equivalent of ../..)
 dir = os.path.dirname(os.path.dirname(dir))
 # load python modules from top-level
 sys.path.insert(0, dir)
```

### Comparing `translate-toolkit-3.8.6/tests/xliff_conformance/af-pootle.po` & `translate-toolkit-3.9.0/tests/xliff_conformance/af-pootle.po`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/xliff_conformance/en-US.sdf` & `translate-toolkit-3.9.0/tests/xliff_conformance/en-US.sdf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tests/xliff_conformance/test_xliff_conformance.py` & `translate-toolkit-3.9.0/tests/xliff_conformance/test_xliff_conformance.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,61 +11,57 @@
 # translate is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
-
 import os
 import os.path as path
 from subprocess import call
 
+import pytest
 from lxml import etree
 
 
-schema = None
-
-
-def xmllint(fullpath):
-    return schema.validate(etree.parse(fullpath))
+@pytest.fixture(autouse=True, scope="module")
+def change_test_dir(request):
+    os.chdir(request.fspath.dirname)
+    yield
+    os.chdir(request.config.invocation_params.dir)
 
 
-def setup_module(module):
-    global schema
-    os.chdir(path.dirname(__file__))
+@pytest.fixture(scope="module")
+def xmllint():
     schema = etree.XMLSchema(etree.parse("xliff-core-1.1.xsd"))
+    return lambda fullpath: schema.validate(etree.parse(fullpath))
 
 
 def find_files(base, check_ext):
     for dirpath, _dirnames, filenames in os.walk(base):
         for filename in filenames:
             fullpath = path.join(dirpath, filename)
             _namepath, ext = path.splitext(fullpath)
             if check_ext == ext:
                 yield fullpath
 
 
-def test_open_office_to_xliff():
+def test_open_office_to_xliff(xmllint):
     assert call(["oo2xliff", "en-US.sdf", "-l", "fr", "fr"]) == 0
     for filepath in find_files("fr", ".xlf"):
         assert xmllint(filepath)
     cleardir("fr")
 
 
-def test_po_to_xliff():
+def test_po_to_xliff(xmllint):
     OUTPUT = "af-pootle.xlf"
     assert call(["po2xliff", "af-pootle.po", OUTPUT]) == 0
     assert xmllint(OUTPUT)
 
 
-def teardown_module(module):
-    pass
-
-
 def cleardir(testdir):
     """removes the test directory"""
     if os.path.exists(testdir):
         for dirpath, subdirs, filenames in os.walk(testdir, topdown=False):
             for name in filenames:
                 os.remove(os.path.join(dirpath, name))
             for name in subdirs:
```

### Comparing `translate-toolkit-3.8.6/tests/xliff_conformance/xliff-core-1.1.xsd` & `translate-toolkit-3.9.0/tests/xliff_conformance/xliff-core-1.1.xsd`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/README.firefox_build_instructions.rst` & `translate-toolkit-3.9.0/tools/mozilla/README.firefox_build_instructions.rst`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/Vagrantfile` & `translate-toolkit-3.9.0/tools/mozilla/Vagrantfile`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/accesskey_checker` & `translate-toolkit-3.9.0/tools/mozilla/accesskey_checker`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/accesskey_checker_PO` & `translate-toolkit-3.9.0/tools/mozilla/accesskey_checker_PO`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/build_firefox.sh` & `translate-toolkit-3.9.0/tools/mozilla/build_firefox.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/build_tb3_langs.sh` & `translate-toolkit-3.9.0/tools/mozilla/build_tb3_langs.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/buildxpi.py` & `translate-toolkit-3.9.0/tools/mozilla/buildxpi.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
 import os
 import re
 from glob import glob
 from shutil import move, rmtree
 from subprocess import PIPE, CalledProcessError, Popen
 from tempfile import mkdtemp
 
-
 logger = logging.getLogger(__name__)
 
 
 class RunProcessError(CalledProcessError):
     """Subclass of CalledProcessError exception with custom message strings"""
 
     _default_message = "Command '%s' returned exit status %d"
```

### Comparing `translate-toolkit-3.8.6/tools/mozilla/get_moz_enUS.py` & `translate-toolkit-3.9.0/tools/mozilla/get_moz_enUS.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import os
 import shutil
 from configparser import ConfigParser, NoSectionError
 
-
 srccheckout = "mozilla"
 l10ncheckout = "l10n"
 product = "browser"
 verbose = False
 
 
 def path_neutral(path):
```

### Comparing `translate-toolkit-3.8.6/tools/mozilla/moz-l10n-builder` & `translate-toolkit-3.9.0/tools/mozilla/moz-l10n-builder`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/moz_l10n_builder.py` & `translate-toolkit-3.9.0/tools/mozilla/moz_l10n_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import os
 import shutil
 import sys
 import tempfile
 import time
 from subprocess import PIPE, Popen
 
-
 join = os.path.join
 
 try:
     # Make sure that all convertion tools are available
     from translate.convert import moz2po, po2moz, po2prop, txt2po  # noqa: F401
 except ImportError:
     raise Exception(
```

### Comparing `translate-toolkit-3.8.6/tools/mozilla/mozcronbuild.py` & `translate-toolkit-3.9.0/tools/mozilla/mozcronbuild.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 from tools.mozilla import moz_l10n_builder
 
-
 MOZDIR = os.path.join(os.path.expanduser("~"), "mozbuild")
 
 
 def build_langs(langs, verbose):
     olddir = os.getcwd()
     os.chdir(MOZDIR)
```

### Comparing `translate-toolkit-3.8.6/tools/mozilla/mozilla-l10n.patch` & `translate-toolkit-3.9.0/tools/mozilla/mozilla-l10n.patch`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/mozzy.sh` & `translate-toolkit-3.9.0/tools/mozilla/mozzy.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/mozilla/postinstall.sh` & `translate-toolkit-3.9.0/tools/mozilla/postinstall.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/phase` & `translate-toolkit-3.9.0/tools/phase`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/phaselist2goals` & `translate-toolkit-3.9.0/tools/phaselist2goals`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/pocommentclean` & `translate-toolkit-3.9.0/tools/pocommentclean`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/pocompendium` & `translate-toolkit-3.9.0/tools/pocompendium`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/pomigrate2` & `translate-toolkit-3.9.0/tools/pomigrate2`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/popuretext` & `translate-toolkit-3.9.0/tools/popuretext`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/poreencode` & `translate-toolkit-3.9.0/tools/poreencode`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/tools/posplit` & `translate-toolkit-3.9.0/tools/posplit`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/__init__.py` & `translate-toolkit-3.9.0/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/__version__.py` & `translate-toolkit-3.9.0/translate/__version__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """This file contains the version of the Translate Toolkit."""
 
-ver = (3, 8, 6)
+ver = (3, 9, 0)
 """Machine readable version number. Used by tools that need to adjust code
 paths based on a Translate Toolkit release number."""
 
 build = ver[0] * 10000 + ver[1] * 100 + ver[2]
 """The build number is used by external users of the Translate Toolkit to
 trigger refreshes.  Thus increase the build number whenever changes are made to
 code touching stats or quality checks.  An increased build number will force a
```

### Comparing `translate-toolkit-3.8.6/translate/convert/__init__.py` & `translate-toolkit-3.9.0/translate/convert/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/accesskey.py` & `translate-toolkit-3.9.0/translate/convert/accesskey.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """functions used to manipulate access keys in strings"""
 
 
 from translate.storage.placeables.general import XMLEntityPlaceable
 
-
 DEFAULT_ACCESSKEY_MARKER = "&"
 
 
 class UnitMixer:
     """Helper to mix separately defined labels and accesskeys into one unit."""
 
     def __init__(self, labelsuffixes, accesskeysuffixes):
```

### Comparing `translate-toolkit-3.8.6/translate/convert/convert.py` & `translate-toolkit-3.9.0/translate/convert/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 """
 
 import os.path
 from io import BytesIO
 
 from translate.misc import optrecurse
 
-
 # Don't import optparse ourselves, get the version from optrecurse.
 optparse = optrecurse.optparse
 
 
 class ConvertOptionParser(optrecurse.RecursiveOptionParser):
     """A specialized Option Parser for convertor tools..."""
```

### Comparing `translate-toolkit-3.8.6/translate/convert/csv2po.py` & `translate-toolkit-3.9.0/translate/convert/csv2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import csvl10n, po
 
-
 logger = logging.getLogger(__name__)
 
 
 def replacestrings(source, *pairs):
     r"""Use ``pairs`` of ``(original, replacement)`` to replace text found in
     ``source``.
```

### Comparing `translate-toolkit-3.8.6/translate/convert/csv2tbx.py` & `translate-toolkit-3.9.0/translate/convert/csv2tbx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/dtd2po.py` & `translate-toolkit-3.9.0/translate/convert/dtd2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/factory.py` & `translate-toolkit-3.9.0/translate/convert/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """Factory methods to convert supported input files to supported translatable files."""
 
 import os
 
-
 # from translate.convert import prop2po, po2prop, odf2xliff, xliff2odf
 
 
 __all__ = ("converters", "UnknownExtensionError", "UnsupportedConversionError")
 
 # Turn into property to support lazy loading of things?
 converters = {}
```

### Comparing `translate-toolkit-3.8.6/translate/convert/flatxml2po.py` & `translate-toolkit-3.9.0/translate/convert/flatxml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/html2po.py` & `translate-toolkit-3.9.0/translate/convert/html2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/ical2po.py` & `translate-toolkit-3.9.0/translate/convert/ical2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/idml2po.py` & `translate-toolkit-3.9.0/translate/convert/idml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/ini2po.py` & `translate-toolkit-3.9.0/translate/convert/ini2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/json2po.py` & `translate-toolkit-3.9.0/translate/convert/json2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import po
 
-
 logger = logging.getLogger(__name__)
 
 
 class json2po:
     """Convert a JSON file to a PO file"""
 
     def convert_store(self, input_store, duplicatestyle="msgctxt"):
```

### Comparing `translate-toolkit-3.8.6/translate/convert/moz2po.py` & `translate-toolkit-3.9.0/translate/convert/moz2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/mozfunny2prop.py` & `translate-toolkit-3.9.0/translate/convert/mozfunny2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/mozlang2po.py` & `translate-toolkit-3.9.0/translate/convert/mozlang2po.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 # Original Author: Dan Schafer <dschafer@mozilla.com>
 # Date: 10 Jun 2008
 
 """Convert Mozilla .lang files to Gettext PO localization files.
 """
 
 from translate.convert import convert
-from translate.storage import mozilla_lang as lang, po
+from translate.storage import mozilla_lang as lang
+from translate.storage import po
 
 
 class lang2po:
     """Convert one Mozilla .lang file to a single PO file."""
 
     SourceStoreClass = lang.LangStore
     TargetStoreClass = po.pofile
```

### Comparing `translate-toolkit-3.8.6/translate/convert/odf2xliff.py` & `translate-toolkit-3.9.0/translate/convert/odf2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/oo2po.py` & `translate-toolkit-3.9.0/translate/convert/oo2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 """
 
 import logging
 from urllib import parse
 
 from translate.storage import oo, po
 
-
 # TODO: support using one GSI file as template, another as input (for when English is in one and translation in another)
 
 logger = logging.getLogger(__name__)
 
 
 class oo2po:
     def __init__(
```

### Comparing `translate-toolkit-3.8.6/translate/convert/oo2xliff.py` & `translate-toolkit-3.9.0/translate/convert/oo2xliff.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import oo, xliff
 
-
 # TODO: support using one GSI file as template, another as input (for when English is in one and translation in another)
 
 logger = logging.getLogger(__name__)
 
 
 class oo2xliff:
     def __init__(
```

### Comparing `translate-toolkit-3.8.6/translate/convert/php2po.py` & `translate-toolkit-3.9.0/translate/convert/php2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2csv.py` & `translate-toolkit-3.9.0/translate/convert/po2csv.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2dtd.py` & `translate-toolkit-3.9.0/translate/convert/po2dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2flatxml.py` & `translate-toolkit-3.9.0/translate/convert/po2flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2html.py` & `translate-toolkit-3.9.0/translate/convert/po2html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2ical.py` & `translate-toolkit-3.9.0/translate/convert/po2ical.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2idml.py` & `translate-toolkit-3.9.0/translate/convert/po2idml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2ini.py` & `translate-toolkit-3.9.0/translate/convert/po2ini.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2json.py` & `translate-toolkit-3.9.0/translate/convert/po2json.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2moz.py` & `translate-toolkit-3.9.0/translate/convert/po2moz.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2mozlang.py` & `translate-toolkit-3.9.0/translate/convert/po2mozlang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2oo.py` & `translate-toolkit-3.9.0/translate/convert/po2oo.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 import os
 import time
 
 from translate.convert import convert
 from translate.filters import autocorrect, checks, pofilter
 from translate.storage import factory, oo
 
-
 logger = logging.getLogger(__name__)
 
 
 class reoo:
     def __init__(
         self,
         templatefile,
```

### Comparing `translate-toolkit-3.8.6/translate/convert/po2php.py` & `translate-toolkit-3.9.0/translate/convert/po2php.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 See: http://docs.translatehouse.org/projects/translate-toolkit/en/latest/commands/php2po.html
 for examples and usage instructions.
 """
 
 from translate.convert import convert
 from translate.storage import php, po
 
-
 eol = "\n"
 
 
 class rephp:
     def __init__(self, templatefile, inputstore):
         self.outputstore = php.phpfile(templatefile)
         self.inputstore = inputstore
```

### Comparing `translate-toolkit-3.8.6/translate/convert/po2prop.py` & `translate-toolkit-3.9.0/translate/convert/po2prop.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 
 import warnings
 
 from translate.convert import accesskey, convert
 from translate.misc import quote
 from translate.storage import po, properties
 
-
 eol = "\n"
 
 
 def applytranslation(key, propunit, inunit, mixedkeys):
     """applies the translation for key in the po unit to the prop unit"""
     # this converts the po-style string to a prop-style string
     value = inunit.target
```

### Comparing `translate-toolkit-3.8.6/translate/convert/po2rc.py` & `translate-toolkit-3.9.0/translate/convert/po2rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 from translate.storage import po, rc
 from translate.storage.rc import (
     generate_menu_pre_name,
     generate_popup_caption_name,
     generate_popup_pre_name,
 )
 
-
 NL = "\r\n"
 BLOCK_START = "BEGIN"
 BLOCK_END = "END"
 
 EMPTY_LOCATION = ""
```

### Comparing `translate-toolkit-3.8.6/translate/convert/po2resx.py` & `translate-toolkit-3.9.0/translate/convert/po2resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2sub.py` & `translate-toolkit-3.9.0/translate/convert/po2sub.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2symb.py` & `translate-toolkit-3.9.0/translate/convert/po2symb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2tiki.py` & `translate-toolkit-3.9.0/translate/convert/po2tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2tmx.py` & `translate-toolkit-3.9.0/translate/convert/po2tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2ts.py` & `translate-toolkit-3.9.0/translate/convert/po2ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2txt.py` & `translate-toolkit-3.9.0/translate/convert/po2txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2web2py.py` & `translate-toolkit-3.9.0/translate/convert/po2web2py.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2wordfast.py` & `translate-toolkit-3.9.0/translate/convert/po2wordfast.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2xliff.py` & `translate-toolkit-3.9.0/translate/convert/po2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/po2yaml.py` & `translate-toolkit-3.9.0/translate/convert/po2yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/pot2po.py` & `translate-toolkit-3.9.0/translate/convert/pot2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/prop2mozfunny.py` & `translate-toolkit-3.9.0/translate/convert/prop2mozfunny.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/prop2po.py` & `translate-toolkit-3.9.0/translate/convert/prop2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 """
 
 import logging
 
 from translate.convert.accesskey import UnitMixer
 from translate.storage import po, properties
 
-
 logger = logging.getLogger(__name__)
 
 
 class DiscardUnit(ValueError):
     pass
```

### Comparing `translate-toolkit-3.8.6/translate/convert/rc2po.py` & `translate-toolkit-3.9.0/translate/convert/rc2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import po, rc
 
-
 logger = logging.getLogger(__name__)
 
 
 class rc2po:
     """Convert a .rc file to a .po file for handling the translation."""
 
     def convert_store(self, input_store, duplicatestyle="msgctxt"):
```

### Comparing `translate-toolkit-3.8.6/translate/convert/resx2po.py` & `translate-toolkit-3.9.0/translate/convert/resx2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import po
 
-
 logger = logging.getLogger(__name__)
 
 
 class resx2po:
     """Convert a RESX file to a PO file for handling translation"""
 
     def convert_store(self, input_store, duplicatestyle="msgctxt"):
```

### Comparing `translate-toolkit-3.8.6/translate/convert/roundtrip-OOo` & `translate-toolkit-3.9.0/translate/convert/roundtrip-OOo`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/roundtrip-gaia` & `translate-toolkit-3.9.0/translate/convert/roundtrip-gaia`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/roundtrip-mozilla` & `translate-toolkit-3.9.0/translate/convert/roundtrip-mozilla`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/sub2po.py` & `translate-toolkit-3.9.0/translate/convert/sub2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 for examples and usage instructions.
 """
 
 import logging
 
 from translate.storage import po
 
-
 logger = logging.getLogger(__name__)
 
 
 def convert_store(input_store, duplicatestyle="msgctxt"):
     """converts a subtitle file to a .po file..."""
     output_store = po.pofile()
     output_header = output_store.header()
```

### Comparing `translate-toolkit-3.8.6/translate/convert/symb2po.py` & `translate-toolkit-3.9.0/translate/convert/symb2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/tbx2po.py` & `translate-toolkit-3.9.0/translate/convert/tbx2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test.idml` & `translate-toolkit-3.9.0/translate/convert/test.idml`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test.odt` & `translate-toolkit-3.9.0/translate/convert/test.odt`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_accesskey.py` & `translate-toolkit-3.9.0/translate/convert/test_accesskey.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_convert.py` & `translate-toolkit-3.9.0/translate/convert/test_convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import re
 from itertools import chain
 
 import pytest
 
 from translate.convert import convert
 
-
 OPTION_RE = re.compile(r"^\s*-")
 
 
 class TestConvertCommand:
     """Tests running actual commands on files"""
 
     convertmodule = convert
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_csv2po.py` & `translate-toolkit-3.9.0/translate/convert/test_csv2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_dtd2po.py` & `translate-toolkit-3.9.0/translate/convert/test_dtd2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_flatxml2po.py` & `translate-toolkit-3.9.0/translate/convert/test_flatxml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_html2po.py` & `translate-toolkit-3.9.0/translate/convert/test_html2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_ical2po.py` & `translate-toolkit-3.9.0/translate/convert/test_ical2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_ini2po.py` & `translate-toolkit-3.9.0/translate/convert/test_ini2po.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from io import BytesIO
 
 from pytest import importorskip
 
 from translate.convert import ini2po, test_convert
 
-
 importorskip("iniparse")
 
 
 class TestIni2PO:
     ConverterClass = ini2po.ini2po
 
     def _convert(
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_json2po.py` & `translate-toolkit-3.9.0/translate/convert/test_json2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_mozfunny2prop.py` & `translate-toolkit-3.9.0/translate/convert/test_mozfunny2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_mozlang2po.py` & `translate-toolkit-3.9.0/translate/convert/test_mozlang2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_oo2po.py` & `translate-toolkit-3.9.0/translate/convert/test_oo2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_oo2xliff.py` & `translate-toolkit-3.9.0/translate/convert/test_oo2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_php2po.py` & `translate-toolkit-3.9.0/translate/convert/test_php2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2csv.py` & `translate-toolkit-3.9.0/translate/convert/test_po2csv.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2dtd.py` & `translate-toolkit-3.9.0/translate/convert/test_po2dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2flatxml.py` & `translate-toolkit-3.9.0/translate/convert/test_po2flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2html.py` & `translate-toolkit-3.9.0/translate/convert/test_po2html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2ical.py` & `translate-toolkit-3.9.0/translate/convert/test_po2ical.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2idml.py` & `translate-toolkit-3.9.0/translate/convert/test_po2idml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2ini.py` & `translate-toolkit-3.9.0/translate/convert/test_po2ini.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from io import BytesIO
 
 from pytest import importorskip, raises
 
 from translate.convert import po2ini, test_convert
 
-
 importorskip("iniparse")
 
 
 class TestPO2Ini:
     ConverterClass = po2ini.po2ini
 
     def _convert(
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2json.py` & `translate-toolkit-3.9.0/translate/convert/test_po2json.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2mozlang.py` & `translate-toolkit-3.9.0/translate/convert/test_po2mozlang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2oo.py` & `translate-toolkit-3.9.0/translate/convert/test_po2oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2php.py` & `translate-toolkit-3.9.0/translate/convert/test_po2php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2prop.py` & `translate-toolkit-3.9.0/translate/convert/test_po2prop.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2rc.py` & `translate-toolkit-3.9.0/translate/convert/test_po2rc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from translate.convert import po2rc, test_convert
 from translate.storage.rc import rcfile
 
-
 RC_SOURCE = r"""
 #include "other_file.h" // This must be ignored
 
 LANGUAGE LANG_ENGLISH, SUBLANG_DEFAULT
 
 /////////////////////////////////////////////////////////////////////////////
 //
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2resx.py` & `translate-toolkit-3.9.0/translate/convert/test_po2resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2sub.py` & `translate-toolkit-3.9.0/translate/convert/test_po2sub.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
 
 from pytest import importorskip
 
 from translate.convert import po2sub, test_convert
 from translate.storage import po
 
-
 # Technically subtitles can also use an older gaupol
 importorskip("aeidon")
 
 
 class TestPO2Sub:
     @staticmethod
     def po2sub(posource):
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2tiki.py` & `translate-toolkit-3.9.0/translate/convert/test_po2tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2tmx.py` & `translate-toolkit-3.9.0/translate/convert/test_po2tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2ts.py` & `translate-toolkit-3.9.0/translate/convert/test_po2ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2txt.py` & `translate-toolkit-3.9.0/translate/convert/test_po2txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2web2py.py` & `translate-toolkit-3.9.0/translate/convert/test_po2web2py.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2xliff.py` & `translate-toolkit-3.9.0/translate/convert/test_po2xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_po2yaml.py` & `translate-toolkit-3.9.0/translate/convert/test_po2yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_pot2po.py` & `translate-toolkit-3.9.0/translate/convert/test_pot2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_prop2mozfunny.py` & `translate-toolkit-3.9.0/translate/convert/test_prop2mozfunny.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_prop2po.py` & `translate-toolkit-3.9.0/translate/convert/test_prop2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_rc2po.py` & `translate-toolkit-3.9.0/translate/convert/test_rc2po.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from translate.convert import rc2po, test_convert
 from translate.storage.po import pofile
 
-
 RC_SOURCE = r"""
 #include "other_file.h" // This must be ignored
 
 LANGUAGE LANG_ENGLISH, SUBLANG_DEFAULT
 
 /////////////////////////////////////////////////////////////////////////////
 //
```

### Comparing `translate-toolkit-3.8.6/translate/convert/test_resx2po.py` & `translate-toolkit-3.9.0/translate/convert/test_resx2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_tiki2po.py` & `translate-toolkit-3.9.0/translate/convert/test_tiki2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_ts2po.py` & `translate-toolkit-3.9.0/translate/convert/test_ts2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_txt2po.py` & `translate-toolkit-3.9.0/translate/convert/test_txt2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_web2py2po.py` & `translate-toolkit-3.9.0/translate/convert/test_web2py2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_xliff2odf.py` & `translate-toolkit-3.9.0/translate/convert/test_xliff2odf.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_xliff2po.py` & `translate-toolkit-3.9.0/translate/convert/test_xliff2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/test_yaml2po.py` & `translate-toolkit-3.9.0/translate/convert/test_yaml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/tiki2po.py` & `translate-toolkit-3.9.0/translate/convert/tiki2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/ts2po.py` & `translate-toolkit-3.9.0/translate/convert/ts2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/txt2po.py` & `translate-toolkit-3.9.0/translate/convert/txt2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/web2py2po.py` & `translate-toolkit-3.9.0/translate/convert/web2py2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/xliff2odf.py` & `translate-toolkit-3.9.0/translate/convert/xliff2odf.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/xliff2oo.py` & `translate-toolkit-3.9.0/translate/convert/xliff2oo.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import logging
 import os
 import time
 
 from translate.filters import autocorrect, checks, pofilter
 from translate.storage import factory, oo
 
-
 logger = logging.getLogger(__name__)
 
 
 class reoo:
     def __init__(
         self,
         templatefile,
```

### Comparing `translate-toolkit-3.8.6/translate/convert/xliff2po.py` & `translate-toolkit-3.9.0/translate/convert/xliff2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/convert/yaml2po.py` & `translate-toolkit-3.9.0/translate/convert/yaml2po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/__init__.py` & `translate-toolkit-3.9.0/translate/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/autocorrect.py` & `translate-toolkit-3.9.0/translate/filters/autocorrect.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/checks.py` & `translate-toolkit-3.9.0/translate/filters/checks.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,14 @@
 import logging
 import re
 
 from translate.filters import decoration, helpers, prefilters, spelling
 from translate.filters.decorators import cosmetic, critical, extraction, functional
 from translate.lang import data, factory
 
-
 logger = logging.getLogger(__name__)
 
 # These are some regular expressions that are compiled for use in some tests
 
 # printf syntax based on http://en.wikipedia.org/wiki/Printf which doesn't
 # cover everything we leave \w instead of specifying the exact letters as
 # this should capture printf types defined in other platforms.
```

### Comparing `translate-toolkit-3.8.6/translate/filters/decoration.py` & `translate-toolkit-3.9.0/translate/filters/decoration.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/decorators.py` & `translate-toolkit-3.9.0/translate/filters/decorators.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/helpers.py` & `translate-toolkit-3.9.0/translate/filters/helpers.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/pofilter.py` & `translate-toolkit-3.9.0/translate/filters/pofilter.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/prefilters.py` & `translate-toolkit-3.9.0/translate/filters/prefilters.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/spelling.py` & `translate-toolkit-3.9.0/translate/filters/spelling.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """An API to provide spell checking for use in checks or elsewhere."""
 
 import logging
 from functools import lru_cache
 
-
 logger = logging.getLogger(__name__)
 
 available = False
 
 try:
     # Enchant
-    from enchant import Error as EnchantError, checker
+    from enchant import Error as EnchantError
+    from enchant import checker
 
     available = True
     checkers = {}
 
     def _get_checker(lang):
         if lang not in checkers:
             try:
```

### Comparing `translate-toolkit-3.8.6/translate/filters/test_autocorrect.py` & `translate-toolkit-3.9.0/translate/filters/test_autocorrect.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/test_checks.py` & `translate-toolkit-3.9.0/translate/filters/test_checks.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/test_decoration.py` & `translate-toolkit-3.9.0/translate/filters/test_decoration.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/test_pofilter.py` & `translate-toolkit-3.9.0/translate/filters/test_pofilter.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/filters/test_prefilters.py` & `translate-toolkit-3.9.0/translate/filters/test_prefilters.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/__init__.py` & `translate-toolkit-3.9.0/translate/lang/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/af.py` & `translate-toolkit-3.9.0/translate/lang/af.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 """
 
 
 import re
 
 from translate.lang import common
 
-
 articlere = re.compile(r"'n\b")
 
 
 class af(common.Common):
     """This class represents Afrikaans."""
 
     validdoublewords = [""]
```

### Comparing `translate-toolkit-3.8.6/translate/lang/ak.py` & `translate-toolkit-3.9.0/translate/lang/ak.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/am.py` & `translate-toolkit-3.9.0/translate/lang/am.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ar.py` & `translate-toolkit-3.9.0/translate/lang/ar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/az.py` & `translate-toolkit-3.9.0/translate/lang/az.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/bn.py` & `translate-toolkit-3.9.0/translate/lang/bn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/bo.py` & `translate-toolkit-3.9.0/translate/lang/bo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/code_as.py` & `translate-toolkit-3.9.0/translate/lang/code_as.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/code_or.py` & `translate-toolkit-3.9.0/translate/lang/code_or.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/common.py` & `translate-toolkit-3.9.0/translate/lang/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
 
 import logging
 import re
 
 from translate.lang import data
 
-
 logger = logging.getLogger(__name__)
 
 
 class Common:
     """This class is the common parent class for all language classes."""
 
     code = ""
```

### Comparing `translate-toolkit-3.8.6/translate/lang/da.py` & `translate-toolkit-3.9.0/translate/lang/da.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/data.py` & `translate-toolkit-3.9.0/translate/lang/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 import gettext
 import locale
 import os
 import re
 import unicodedata
 
-
 try:
     import pycountry
 except ImportError:
     pycountry = None
 
 
 languages = {
```

### Comparing `translate-toolkit-3.8.6/translate/lang/de.py` & `translate-toolkit-3.9.0/translate/lang/de.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/dz.py` & `translate-toolkit-3.9.0/translate/lang/dz.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/el.py` & `translate-toolkit-3.9.0/translate/lang/el.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/es.py` & `translate-toolkit-3.9.0/translate/lang/es.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/fa.py` & `translate-toolkit-3.9.0/translate/lang/fa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/factory.py` & `translate-toolkit-3.9.0/translate/lang/factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import pkgutil
 from functools import lru_cache
 from importlib import import_module
 
 from translate.lang import common, data
 
-
 prefix = "code_"
 
 
 @lru_cache(maxsize=128)
 def getlanguage(code):
     """This returns a language class.
```

### Comparing `translate-toolkit-3.8.6/translate/lang/fi.py` & `translate-toolkit-3.9.0/translate/lang/fi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/fr.py` & `translate-toolkit-3.9.0/translate/lang/fr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/gd.py` & `translate-toolkit-3.9.0/translate/lang/gd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/gu.py` & `translate-toolkit-3.9.0/translate/lang/gu.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/he.py` & `translate-toolkit-3.9.0/translate/lang/he.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/hi.py` & `translate-toolkit-3.9.0/translate/lang/hi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/hy.py` & `translate-toolkit-3.9.0/translate/lang/hy.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/identify.py` & `translate-toolkit-3.9.0/translate/lang/identify.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ja.py` & `translate-toolkit-3.9.0/translate/lang/ja.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/km.py` & `translate-toolkit-3.9.0/translate/lang/km.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/kn.py` & `translate-toolkit-3.9.0/translate/lang/kn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ko.py` & `translate-toolkit-3.9.0/translate/lang/ko.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/kw.py` & `translate-toolkit-3.9.0/translate/lang/kw.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/lo.py` & `translate-toolkit-3.9.0/translate/lang/lo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ml.py` & `translate-toolkit-3.9.0/translate/lang/ml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/mr.py` & `translate-toolkit-3.9.0/translate/lang/mr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ms.py` & `translate-toolkit-3.9.0/translate/lang/ms.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/my.py` & `translate-toolkit-3.9.0/translate/lang/my.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ne.py` & `translate-toolkit-3.9.0/translate/lang/ne.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ngram.py` & `translate-toolkit-3.9.0/translate/lang/ngram.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 """
 
 import glob
 import re
 import sys
 from os import path
 
-
 nb_ngrams = 400
 white_space_re = re.compile(r"\s+")
 
 
 class _NGram:
     def __init__(self, arg=None):
         if isinstance(arg, str):
```

### Comparing `translate-toolkit-3.8.6/translate/lang/nqo.py` & `translate-toolkit-3.9.0/translate/lang/nqo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/nso.py` & `translate-toolkit-3.9.0/translate/lang/nso.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/pa.py` & `translate-toolkit-3.9.0/translate/lang/pa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/pl.py` & `translate-toolkit-3.9.0/translate/lang/pl.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/poedit.py` & `translate-toolkit-3.9.0/translate/lang/poedit.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/pt_BR.py` & `translate-toolkit-3.9.0/translate/lang/pt_BR.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ro.py` & `translate-toolkit-3.9.0/translate/lang/ro.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/scn.py` & `translate-toolkit-3.9.0/translate/lang/scn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/si.py` & `translate-toolkit-3.9.0/translate/lang/si.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/son.py` & `translate-toolkit-3.9.0/translate/lang/son.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/st.py` & `translate-toolkit-3.9.0/translate/lang/st.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/su.py` & `translate-toolkit-3.9.0/translate/lang/su.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/sv.py` & `translate-toolkit-3.9.0/translate/lang/sv.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ta.py` & `translate-toolkit-3.9.0/translate/lang/ta.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/te.py` & `translate-toolkit-3.9.0/translate/lang/te.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/team.py` & `translate-toolkit-3.9.0/translate/lang/team.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 """Module to guess the language ISO code based on the 'Language-Team' entry in
 the header of a Gettext PO file.
 """
 
 import re
 
-
 __all__ = ("LANG_TEAM_CONTACT_SNIPPETS", "guess_language")
 
 LANG_TEAM_REGEX = (
     ("@li.org", "([a-z_A-Z]{2,})@li.org", ["LL", "XX", "TEAM"]),
     ("translation-team", "translation-team-([a-z_A-Z]+)@lists.sourceforge.net", None),
     ("fedora-trans", "fedora-trans-([a-z_A-Z]+)@redhat.com", ["list"]),
     ("ubuntu-l10n", "ubuntu-l10n-([a-z_A-Z]+)@lists.ubuntu.com", None),
```

### Comparing `translate-toolkit-3.8.6/translate/lang/test-language-teams.sh` & `translate-toolkit-3.9.0/translate/lang/test-language-teams.sh`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_af.py` & `translate-toolkit-3.9.0/translate/lang/test_af.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_am.py` & `translate-toolkit-3.9.0/translate/lang/test_am.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_ar.py` & `translate-toolkit-3.9.0/translate/lang/test_ar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_common.py` & `translate-toolkit-3.9.0/translate/lang/test_common.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_data.py` & `translate-toolkit-3.9.0/translate/lang/test_data.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_el.py` & `translate-toolkit-3.9.0/translate/lang/test_el.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_es.py` & `translate-toolkit-3.9.0/translate/lang/test_es.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_fa.py` & `translate-toolkit-3.9.0/translate/lang/test_fa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_factory.py` & `translate-toolkit-3.9.0/translate/lang/test_factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_fr.py` & `translate-toolkit-3.9.0/translate/lang/test_fr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_hy.py` & `translate-toolkit-3.9.0/translate/lang/test_hy.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_identify.py` & `translate-toolkit-3.9.0/translate/lang/test_identify.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from pytest import raises
 
 from translate.lang.identify import LanguageIdentifier
 from translate.storage.base import TranslationUnit
 
-
 TEXT = """
 Ästhetik des "Erhabenen" herangezogen.
 kostete (hinzu kommen über 6 630 tote
    O3 steht für Ozon; es wird in der
 NO2 sind wesentlich am "sauren Regen"
 Ethik hängt eng mit einer Dauerkrise der
 Serumwerk GmbH Dresden, Postfach
```

### Comparing `translate-toolkit-3.8.6/translate/lang/test_ja.py` & `translate-toolkit-3.9.0/translate/lang/test_ja.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_km.py` & `translate-toolkit-3.9.0/translate/lang/test_km.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_ko.py` & `translate-toolkit-3.9.0/translate/lang/test_ko.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_ne.py` & `translate-toolkit-3.9.0/translate/lang/test_ne.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_nqo.py` & `translate-toolkit-3.9.0/translate/lang/test_nqo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_or.py` & `translate-toolkit-3.9.0/translate/lang/test_or.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_poedit.py` & `translate-toolkit-3.9.0/translate/lang/test_poedit.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_ro.py` & `translate-toolkit-3.9.0/translate/lang/test_ro.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_scn.py` & `translate-toolkit-3.9.0/translate/lang/test_scn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_team.py` & `translate-toolkit-3.9.0/translate/lang/test_team.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_th.py` & `translate-toolkit-3.9.0/translate/lang/test_th.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_vi.py` & `translate-toolkit-3.9.0/translate/lang/test_vi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/test_zh.py` & `translate-toolkit-3.9.0/translate/lang/test_zh.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/th.py` & `translate-toolkit-3.9.0/translate/lang/th.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/tr.py` & `translate-toolkit-3.9.0/translate/lang/tr.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ug.py` & `translate-toolkit-3.9.0/translate/lang/ug.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ur.py` & `translate-toolkit-3.9.0/translate/lang/ur.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/ve.py` & `translate-toolkit-3.9.0/translate/lang/ve.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/vi.py` & `translate-toolkit-3.9.0/translate/lang/vi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/wo.py` & `translate-toolkit-3.9.0/translate/lang/wo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/zh.py` & `translate-toolkit-3.9.0/translate/lang/zh.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/zh_cn.py` & `translate-toolkit-3.9.0/translate/lang/zh_cn.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/zh_hk.py` & `translate-toolkit-3.9.0/translate/lang/zh_hk.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/lang/zh_tw.py` & `translate-toolkit-3.9.0/translate/lang/zh_tw.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/__init__.py` & `translate-toolkit-3.9.0/translate/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/deprecation.py` & `translate-toolkit-3.9.0/translate/misc/deprecation.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/dictutils.py` & `translate-toolkit-3.9.0/translate/misc/dictutils.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/file_discovery.py` & `translate-toolkit-3.9.0/translate/misc/file_discovery.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/multistring.py` & `translate-toolkit-3.9.0/translate/misc/multistring.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/optrecurse.py` & `translate-toolkit-3.9.0/translate/misc/optrecurse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/ourdom.py` & `translate-toolkit-3.9.0/translate/misc/ourdom.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 directly from minidom, like minidom.Element, minidom.Document or methods such
 as minidom.parseString, since the functionality provided here will not be in
 those objects.
 """
 
 from xml.dom import expatbuilder, minidom
 
-
 # helper functions we use to do xml the way we want, used by modified
 # classes below
 
 
 def writexml_helper(self, writer, indent="", addindent="", newl=""):
     """A replacement for writexml that formats it like typical XML files.
     Nodes are intendented but text nodes, where whitespace can be significant,
```

### Comparing `translate-toolkit-3.8.6/translate/misc/progressbar.py` & `translate-toolkit-3.9.0/translate/misc/progressbar.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/quote.py` & `translate-toolkit-3.9.0/translate/misc/quote.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/selector.py` & `translate-toolkit-3.9.0/translate/misc/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 
 """
 
 import re
 from itertools import starmap
 from wsgiref.util import shift_path_info
 
-
 try:
     from resolver import resolve
 except ImportError:
     # resolver not essential for basic featurs
     # FIXME: this library is overkill, simplify
     pass
```

### Comparing `translate-toolkit-3.8.6/translate/misc/test_multistring.py` & `translate-toolkit-3.9.0/translate/misc/test_multistring.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/test_optrecurse.py` & `translate-toolkit-3.9.0/translate/misc/test_optrecurse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/test_quote.py` & `translate-toolkit-3.9.0/translate/misc/test_quote.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/test_xml_helpers.py` & `translate-toolkit-3.9.0/translate/misc/test_xml_helpers.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/wStringIO.py` & `translate-toolkit-3.9.0/translate/misc/wStringIO.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/wsgi.py` & `translate-toolkit-3.9.0/translate/misc/wsgi.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/misc/xml_helpers.py` & `translate-toolkit-3.9.0/translate/misc/xml_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 """Helper functions for working with XML."""
 
 import re
 from typing import List, Optional
 
 from lxml import etree
 
-
 # some useful xpath expressions
 xml_preserve_ancestors = etree.XPath(
     "ancestor-or-self::*[attribute::xml:space='preserve']"
 )
 """All ancestors with xml:space='preserve'"""
 
 xml_space_ancestors = etree.XPath("ancestor-or-self::*/attribute::xml:space")
```

### Comparing `translate-toolkit-3.8.6/translate/search/__init__.py` & `translate-toolkit-3.9.0/translate/search/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/search/lshtein.py` & `translate-toolkit-3.9.0/translate/search/lshtein.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/search/match.py` & `translate-toolkit-3.9.0/translate/search/match.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/search/terminology.py` & `translate-toolkit-3.9.0/translate/search/terminology.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/search/test_lshtein.py` & `translate-toolkit-3.9.0/translate/search/test_lshtein.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/search/test_match.py` & `translate-toolkit-3.9.0/translate/search/test_match.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/services/__init__.py` & `translate-toolkit-3.9.0/translate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/services/test_tmserver.py` & `translate-toolkit-3.9.0/translate/services/test_tmserver.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/services/tmserver.py` & `translate-toolkit-3.9.0/translate/services/tmserver.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Ndebele.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Ndebele.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/NorthernSotho.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/NorthernSotho.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/README` & `translate-toolkit-3.9.0/translate/share/langmodels/README`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Sotho.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Sotho.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Swati.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Swati.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Tsonga.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Tsonga.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Tswana.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Tswana.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Venda.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Venda.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Xhosa.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Xhosa.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/Zulu.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/Zulu.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/afrikaans.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/afrikaans.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/albanian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/albanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/arabic.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/arabic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/basque.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/basque.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/belarus.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/belarus.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/bosnian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/bosnian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/breton.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/breton.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/catalan.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/catalan.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/chinese_simplified.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/chinese_simplified.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/chinese_traditional.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/chinese_traditional.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/croatian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/croatian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/czech.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/czech.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/danish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/danish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/dutch.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/dutch.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/english.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/english.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/esperanto.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/esperanto.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/estonian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/estonian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/finnish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/finnish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/fpdb.conf` & `translate-toolkit-3.9.0/translate/share/langmodels/fpdb.conf`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/french.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/french.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/frisian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/frisian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/german.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/german.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/greek.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/greek.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/hebrew.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/hebrew.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/hungarian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/hungarian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/icelandic.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/icelandic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/indonesian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/indonesian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/irish_gaelic.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/irish_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/italian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/italian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/japanese.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/japanese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/latin.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/latin.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/latvian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/latvian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/lithuanian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/lithuanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/malay.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/malay.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/manx_gaelic.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/manx_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/norwegian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/norwegian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/polish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/polish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/portuguese.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/portuguese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/quechua.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/quechua.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/romanian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/romanian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/romansh.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/romansh.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/russian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/russian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/scots.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/scots.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/scots_gaelic.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/scots_gaelic.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/serbian_ascii.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/serbian_ascii.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/slovak_ascii.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/slovak_ascii.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/slovenian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/slovenian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/spanish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/spanish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/swahili.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/swahili.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/swedish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/swedish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/tagalog.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/tagalog.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/turkish.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/turkish.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/ukrainian.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/ukrainian.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/vietnamese.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/vietnamese.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/langmodels/welsh.lm` & `translate-toolkit-3.9.0/translate/share/langmodels/welsh.lm`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/share/stoplist-en` & `translate-toolkit-3.9.0/translate/share/stoplist-en`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/__init__.py` & `translate-toolkit-3.9.0/translate/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/_factory_classes.py` & `translate-toolkit-3.9.0/translate/storage/_factory_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     tmx,
     ts2,
     utx,
     wordfast,
     xliff,
 )
 
-
 try:
     from . import trados
 except ImportError:
     pass
 
 __all__ = [
     "catkeys",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/aresource.py` & `translate-toolkit-3.9.0/translate/storage/aresource.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from lxml import etree
 
 from translate.lang import data
 from translate.misc.multistring import multistring
 from translate.storage import base, lisa
 
-
 EOF = None
 WHITESPACE = " \n\t"  # Whitespace that we collapse.
 MULTIWHITESPACE = re.compile("[ \n\t]{2}(?!\\\\n)")
 
 
 class AndroidResourceUnit(base.TranslationUnit):
     """A single entry in the Android String resource file."""
@@ -96,40 +95,29 @@
         while i < len(text):
             c = text[i]
 
             if not active_escape:
                 # Handle whitespace collapsing
                 if c is not EOF and c in WHITESPACE:
                     space_count += 1
-                elif space_count > 1:
-                    # Remove duplicate whitespace; Pay attention: We
+                elif space_count >= 1:
+                    # Remove sequential whitespace; Pay attention: We
                     # don't do this if we are currently inside a quote,
                     # except for one special case: If we have unbalanced
                     # quotes, e.g. we reach eof while a quote is still
                     # open, we *do* collapse that trailing part; this is
                     # how Android does it, for some reason.
                     if not active_quote or c is EOF:
                         # Replace by a single space, will get rid of
                         # non-significant newlines/tabs etc.
                         text[i - space_count : i] = " "
                         i -= space_count - 1
                         if strip and (i == 1 or c is EOF):
                             del text[i - 1]
                     space_count = 0
-                elif space_count == 1:
-                    # At this point we have a single whitespace character,
-                    # but it might be a newline or tab. If we write this
-                    # kind of insignificant whitespace into the .po file,
-                    # it will be considered significant on import. So,
-                    # make sure that this kind of whitespace is always a
-                    # standard space.
-                    text[i - 1] = " "
-                    if strip and not active_quote and (i == 1 or c is EOF):
-                        del text[i - 1]
-                    space_count = 0
                 else:
                     space_count = 0
 
             # Handle quotes
             if c == '"' and not active_escape:
                 active_quote = not active_quote
                 del text[i]
```

### Comparing `translate-toolkit-3.8.6/translate/storage/base.py` & `translate-toolkit-3.9.0/translate/storage/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 import codecs
 import logging
 import pickle
 from io import BytesIO
 from typing import List, Optional, Tuple
 
 from translate.misc.multistring import multistring
-from translate.storage.placeables import StringElem, parse as rich_parse
+from translate.storage.placeables import StringElem
+from translate.storage.placeables import parse as rich_parse
 from translate.storage.workflow import StateEnum as states
 
-
 # Simple BOM based encoding detection
 ENCODING_BOMS = (
     (codecs.BOM_UTF8, "utf-8-sig"),
     (codecs.BOM_UTF16, "utf-16"),
     (codecs.BOM_UTF16_BE, "utf-16-be"),
     (codecs.BOM_UTF16_LE, "utf-16-le"),
     (codecs.BOM_UTF32, "utf-32"),
```

### Comparing `translate-toolkit-3.8.6/translate/storage/benchmark.py` & `translate-toolkit-3.9.0/translate/storage/benchmark.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/bundleprojstore.py` & `translate-toolkit-3.9.0/translate/storage/bundleprojstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 import os
 import shutil
 import tempfile
 from zipfile import ZipFile
 
 from translate.storage.projstore import FileNotInProjectError, ProjectStore
 
-
 __all__ = ("BundleProjectStore", "InvalidBundleError")
 
 
 class InvalidBundleError(Exception):
     pass
```

### Comparing `translate-toolkit-3.8.6/translate/storage/catkeys.py` & `translate-toolkit-3.9.0/translate/storage/catkeys.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 """
 
 import csv
 
 from translate.lang import data
 from translate.storage import base
 
-
 FIELDNAMES_HEADER = ["version", "language", "mimetype", "checksum"]
 """Field names for the catkeys header"""
 
 FIELDNAMES = ["source", "context", "comment", "target"]
 """Field names for a catkeys TU"""
 
 FIELDNAMES_HEADER_DEFAULTS = {
```

### Comparing `translate-toolkit-3.8.6/translate/storage/cpo.py` & `translate-toolkit-3.9.0/translate/storage/cpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     c_uint,
     cdll,
 )
 
 from translate.misc.multistring import multistring
 from translate.storage import base, pocommon, pypo
 
-
 logger = logging.getLogger(__name__)
 
 lsep = " "
 """Separator for #: entries"""
 
 STRING = c_char_p
```

### Comparing `translate-toolkit-3.8.6/translate/storage/csvl10n.py` & `translate-toolkit-3.9.0/translate/storage/csvl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/directory.py` & `translate-toolkit-3.9.0/translate/storage/directory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/dtd.py` & `translate-toolkit-3.9.0/translate/storage/dtd.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,14 @@
 from io import BytesIO
 
 from lxml import etree
 
 from translate.misc import quote
 from translate.storage import base
 
-
 labelsuffixes = (".label", ".title")
 """Label suffixes: entries with this suffix are able to be comibed with accesskeys
 found in in entries ending with :attr:`.accesskeysuffixes`"""
 accesskeysuffixes = (".accesskey", ".accessKey", ".akey")
 """Accesskey Suffixes: entries with this suffix may be combined with labels
 ending in :attr:`.labelsuffixes` into accelerator notation"""
```

### Comparing `translate-toolkit-3.8.6/translate/storage/factory.py` & `translate-toolkit-3.9.0/translate/storage/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 import os
 from functools import lru_cache
 from importlib import import_module
 
 from translate.storage.base import TranslationStore
 from translate.storage.directory import Directory
 
-
 # TODO: Monolingual formats (with template?)
 
 decompressclass = {
     "gz": ("gzip", "GzipFile"),
     "bz2": ("bz2", "BZ2File"),
 }
```

### Comparing `translate-toolkit-3.8.6/translate/storage/flatxml.py` & `translate-toolkit-3.9.0/translate/storage/flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/fpo.py` & `translate-toolkit-3.9.0/translate/storage/fpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 import copy
 import logging
 import re
 
 from translate.misc.multistring import multistring
 from translate.storage import base, cpo, pocommon
 
-
 logger = logging.getLogger(__name__)
 
 
 lsep = " "
 """Separator for #: entries"""
 
 basic_header = r"""msgid ""
```

### Comparing `translate-toolkit-3.8.6/translate/storage/html.py` & `translate-toolkit-3.9.0/translate/storage/html.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 import html.parser
 import re
 from html.entities import html5
 
 from translate.storage import base
 from translate.storage.base import ParseError
 
-
 # Override the piclose tag from simple > to ?> otherwise we consume HTML
 # within the processing instructions
 html.parser.piclose = re.compile(r"\?>")
 
 
 class htmlunit(base.TranslationUnit):
     """A unit of translatable/localisable HTML content"""
```

### Comparing `translate-toolkit-3.8.6/translate/storage/ical.py` & `translate-toolkit-3.9.0/translate/storage/ical.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,14 @@
 import re
 from io import BytesIO
 
 import vobject
 
 from translate.storage import base
 
-
 ICAL_UNIT_LOCATION_RE = re.compile("\\[(?P<uid>.+)\\](?P<property>.+)")
 
 
 class icalunit(base.TranslationUnit):
     """An ical entry that is translatable"""
 
     def __init__(self, source=None, **kwargs):
```

### Comparing `translate-toolkit-3.8.6/translate/storage/idml.py` & `translate-toolkit-3.9.0/translate/storage/idml.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import zipfile
 
-
 # Tags to be extracted as placeables (tags that are within translatable texts).
 INLINE_ELEMENTS = [
     ("", "CharacterStyleRange"),
     ("", "Content"),
     # ('', 'Br'),
 ]
```

### Comparing `translate-toolkit-3.8.6/translate/storage/ini.py` & `translate-toolkit-3.9.0/translate/storage/ini.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 
 import re
 import uuid
 from io import StringIO
 
 from translate.storage import base
 
-
 try:
     from iniparse import INIConfig
 except ImportError:
     raise ImportError("Missing iniparse library.")
 
 
 dialects = {}
```

### Comparing `translate-toolkit-3.8.6/translate/storage/jsonl10n.py` & `translate-toolkit-3.9.0/translate/storage/jsonl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/lisa.py` & `translate-toolkit-3.9.0/translate/storage/lisa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/mo.py` & `translate-toolkit-3.9.0/translate/storage/mo.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
 import array
 import re
 import struct
 
 from translate.misc.multistring import multistring
 from translate.storage import base, poheader
 
-
 MO_MAGIC_NUMBER = 0x950412DE
 POT_HEADER = re.compile(r"^POT-Creation-Date:.*(\n|$)", re.IGNORECASE | re.MULTILINE)
 
 
 def mounpack(filename="messages.mo"):
     """Helper to unpack Gettext MO files into a Python string"""
     with open(filename, "rb") as fh:
```

### Comparing `translate-toolkit-3.8.6/translate/storage/mozilla_lang.py` & `translate-toolkit-3.9.0/translate/storage/mozilla_lang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/odf_io.py` & `translate-toolkit-3.9.0/translate/storage/odf_io.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/odf_shared.py` & `translate-toolkit-3.9.0/translate/storage/odf_shared.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/omegat.py` & `translate-toolkit-3.9.0/translate/storage/omegat.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 """
 
 import csv
 import locale
 
 from translate.storage import base
 
-
 OMEGAT_FIELDNAMES = ["source", "target", "comment"]
 """Field names for an OmegaT glossary unit"""
 
 
 class OmegaTDialect(csv.Dialect):
     """Describe the properties of an OmegaT generated TAB-delimited glossary
     file.
```

### Comparing `translate-toolkit-3.8.6/translate/storage/oo.py` & `translate-toolkit-3.9.0/translate/storage/oo.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 import os
 import re
 import warnings
 from io import BytesIO
 
 from translate.misc import quote, wStringIO
 
-
 # File normalisation
 
 normalfilenamechars = (
     b"/#.0123456789abcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ"
 )
```

### Comparing `translate-toolkit-3.8.6/translate/storage/php.py` & `translate-toolkit-3.9.0/translate/storage/php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/__init__.py` & `translate-toolkit-3.9.0/translate/storage/placeables/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
 from . import base, general, interfaces, xliff
 from .base import *
 from .base import __all__ as all_your_base
 from .parse import parse
 from .strelem import StringElem
 
-
 __all__ = (
     "base",
     "interfaces",
     "general",
     "parse",
     "StringElem",
     "xliff",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/base.py` & `translate-toolkit-3.9.0/translate/storage/placeables/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     MaskingPlaceable,
     PairedDelimiter,
     ReplacementPlaceable,
     SubflowPlaceable,
 )
 from translate.storage.placeables.strelem import StringElem
 
-
 __all__ = ("Bpt", "Ept", "Ph", "It", "G", "Bx", "Ex", "X", "Sub", "to_base_placeables")
 
 
 # Basic placeable types.
 class Bpt(MaskingPlaceable, PairedDelimiter):
     has_content = True
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/general.py` & `translate-toolkit-3.9.0/translate/storage/placeables/general.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 fit into any other sub-category.
 """
 
 import re
 
 from translate.storage.placeables.base import G, Ph, StringElem
 
-
 __all__ = (
     "AltAttrPlaceable",
     "XMLEntityPlaceable",
     "XMLTagPlaceable",
     "parsers",
     "to_general_placeables",
 )
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/interfaces.py` & `translate-toolkit-3.9.0/translate/storage/placeables/interfaces.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/lisa.py` & `translate-toolkit-3.9.0/translate/storage/placeables/lisa.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from lxml import etree
 
 from translate.misc.xml_helpers import normalize_xml_space
 from translate.storage.placeables import StringElem, base, xliff
 from translate.storage.xml_extract import misc
 
-
 __all__ = ("xml_to_strelem", "strelem_to_xml")
 # Use the above functions as entry points into this module. The rest are
 # used by these functions.
 
 
 def make_empty_replacement_placeable(klass, node, xml_space="preserve"):
     try:
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/parse.py` & `translate-toolkit-3.9.0/translate/storage/placeables/parse.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/strelem.py` & `translate-toolkit-3.9.0/translate/storage/placeables/strelem.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/terminology.py` & `translate-toolkit-3.9.0/translate/storage/placeables/terminology.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 """
 Contains the placeable that represents a terminology term.
 """
 
 from translate.storage.placeables import StringElem, base
 
-
 __all__ = ("TerminologyPlaceable", "parsers")
 
 
 class TerminologyPlaceable(base.Ph):
     """Terminology distinguished from the rest of a string by being
     a placeable.
     """
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/test_base.py` & `translate-toolkit-3.9.0/translate/storage/placeables/test_base.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/test_general.py` & `translate-toolkit-3.9.0/translate/storage/placeables/test_general.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/test_lisa.py` & `translate-toolkit-3.9.0/translate/storage/placeables/test_lisa.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/test_terminology.py` & `translate-toolkit-3.9.0/translate/storage/placeables/test_terminology.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 from io import BytesIO
 
 from translate.search.match import terminologymatcher
 from translate.storage.placeables import general, parse
-from translate.storage.placeables.terminology import (
-    TerminologyPlaceable,
-    parsers as term_parsers,
-)
+from translate.storage.placeables.terminology import TerminologyPlaceable
+from translate.storage.placeables.terminology import parsers as term_parsers
 from translate.storage.pypo import pofile
 
 
 class TestTerminologyPlaceable:
     TERMINOLOGY = """
 msgid "name"
 msgstr "naam"
```

### Comparing `translate-toolkit-3.8.6/translate/storage/placeables/xliff.py` & `translate-toolkit-3.9.0/translate/storage/placeables/xliff.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """Contains XLIFF-specific placeables."""
 
 from translate.storage.placeables import base
 from translate.storage.placeables.strelem import StringElem
 
-
 __all__ = (
     "Bpt",
     "Ept",
     "X",
     "Bx",
     "Ex",
     "G",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/po.py` & `translate-toolkit-3.9.0/translate/storage/po.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 tested).
 """
 
 import logging
 import os
 import platform
 
-
 usecpo = os.getenv("USECPO")
 
 if platform.python_implementation() == "CPython":
     if usecpo == "1":
         from translate.storage.cpo import *  # pylint: disable=W0401,W0614
     elif usecpo == "2":
         from translate.storage.fpo import *  # pylint: disable=W0401,W0614
```

### Comparing `translate-toolkit-3.8.6/translate/storage/pocommon.py` & `translate-toolkit-3.9.0/translate/storage/pocommon.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 import re
 from urllib import parse
 
 from translate.storage import base, poheader
 from translate.storage.workflow import StateEnum as state
 
-
 msgid_comment_re = re.compile("_: (.*?)\n")
 
 
 def extract_msgid_comment(text):
     """The one definitive way to extract a msgid comment out of an unescaped
     unicode string that might contain it.
```

### Comparing `translate-toolkit-3.8.6/translate/storage/poheader.py` & `translate-toolkit-3.9.0/translate/storage/poheader.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import re
 import time
 
 from translate import __version__
 from translate.misc.dictutils import cidict
 
-
 author_re = re.compile(r".*<\S+@\S+>.*\d{4,4}")
 
 default_header = {
     "Project-Id-Version": "PACKAGE VERSION",
     "PO-Revision-Date": "YEAR-MO-DA HO:MI+ZONE",
     "Last-Translator": "FULL NAME <EMAIL@ADDRESS>",
     "Language-Team": "LANGUAGE <LL@li.org>",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/poparser.py` & `translate-toolkit-3.9.0/translate/storage/poparser.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
      msgctxt CONTEXT                   (Gettext 0.15)
      msgid UNTRANSLATED-STRING
      msgstr TRANSLATED-STRING
 """
 
 import re
 
-
 SINGLE_BYTE_ENCODING = "iso-8859-1"
 isspace = str.isspace
 find = str.find
 rfind = str.rfind
 startswith = str.startswith
 append = list.append
 decode = bytes.decode
```

### Comparing `translate-toolkit-3.8.6/translate/storage/poxliff.py` & `translate-toolkit-3.9.0/translate/storage/poxliff.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     rich_to_multistring = base.TranslationUnit.rich_to_multistring
 
     rich_source = base.TranslationUnit.rich_source
     rich_target = base.TranslationUnit.rich_target
 
     def gettarget(self, lang=None):
         if self.hasplural():
-            strings = [unit.target for unit in self.units]
+            strings = [unit.target or "" for unit in self.units]
             if strings:
                 return multistring(strings)
             else:
                 return None
         else:
             return super().gettarget(lang)
```

### Comparing `translate-toolkit-3.8.6/translate/storage/project.py` & `translate-toolkit-3.9.0/translate/storage/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 from translate.convert import factory as convert_factory
 from translate.storage.projstore import ProjectStore
 
-
 __all__ = ("Project",)
 
 
 def split_extensions(filename):
     """Split the given filename into a name and extensions part.  The
     extensions part is defined by any sequence of extensions, where an
     extension is a 3-letter, .-separated string or one of "po" or "properties".
```

### Comparing `translate-toolkit-3.8.6/translate/storage/projstore.py` & `translate-toolkit-3.9.0/translate/storage/projstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import os
 
 from lxml import etree
 
-
 __all__ = ("FileExistsInProjectError", "FileNotInProjectError", "ProjectStore")
 
 
 class FileExistsInProjectError(Exception):
     pass
```

### Comparing `translate-toolkit-3.8.6/translate/storage/properties.java` & `translate-toolkit-3.9.0/translate/storage/properties.java`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/properties.py` & `translate-toolkit-3.9.0/translate/storage/properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -134,15 +134,14 @@
 from lxml import etree
 
 from translate.lang import data
 from translate.misc import quote
 from translate.misc.multistring import multistring
 from translate.storage import base
 
-
 labelsuffixes = (".label", ".title")
 """Label suffixes: entries with this suffix are able to be comibed with accesskeys
 found in in entries ending with :attr:`.accesskeysuffixes`"""
 accesskeysuffixes = (".accesskey", ".accessKey", ".akey")
 """Accesskey Suffixes: entries with this suffix may be combined with labels
 ending in :attr:`.labelsuffixes` into accelerator notation"""
```

### Comparing `translate-toolkit-3.8.6/translate/storage/pypo.py` & `translate-toolkit-3.9.0/translate/storage/pypo.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 import unicodedata
 from typing import List, Tuple
 
 from translate.misc import quote
 from translate.misc.multistring import multistring
 from translate.storage import pocommon, poparser
 
-
 logger = logging.getLogger(__name__)
 
 
 lsep = "\n#: "
 """Separator for #: entries"""
 
 # general functions for quoting / unquoting po strings
```

### Comparing `translate-toolkit-3.8.6/translate/storage/qm.py` & `translate-toolkit-3.9.0/translate/storage/qm.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,14 @@
 import codecs
 import logging
 import struct
 
 from translate.misc.multistring import multistring
 from translate.storage import base
 
-
 logger = logging.getLogger(__name__)
 
 QM_MAGIC_NUMBER = (0x3CB86418, 0xCAEF9C95, 0xCD211CBF, 0x60A1BDDD)
 
 
 def qmunpack(file_="messages.qm"):
     """Helper to unpack Qt .qm files into a Python string"""
```

### Comparing `translate-toolkit-3.8.6/translate/storage/qph.py` & `translate-toolkit-3.9.0/translate/storage/qph.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/rc.py` & `translate-toolkit-3.9.0/translate/storage/rc.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/resourcedictionary.py` & `translate-toolkit-3.9.0/translate/storage/resourcedictionary.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/resx.py` & `translate-toolkit-3.9.0/translate/storage/resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/statistics.py` & `translate-toolkit-3.9.0/translate/storage/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 """Module to provide statistics and related functionality.
 
 """
 
 
 from translate.lang import factory
 
-
 # calling classifyunits() in the constructor is probably not ideal.
 # idea: have a property for .classification that calls it if necessary
 
 # If we add units or change translations, statistics are out of date
 # Compare with modules/Status.py in pootling that uses a bitmask to
 # filter units
```

### Comparing `translate-toolkit-3.8.6/translate/storage/stringsdict.py` & `translate-toolkit-3.9.0/translate/storage/stringsdict.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/subtitles.py` & `translate-toolkit-3.9.0/translate/storage/subtitles.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,14 @@
 
 import os
 from io import StringIO
 from tempfile import NamedTemporaryFile
 
 from translate.storage import base
 
-
 try:
     from aeidon import Subtitle, documents, newlines
     from aeidon.encodings import detect
     from aeidon.files import AdvSubStationAlpha, MicroDVD, SubRip, SubStationAlpha, new
     from aeidon.util import detect_format as determine
 except ImportError:
     try:
```

### Comparing `translate-toolkit-3.8.6/translate/storage/symbian.py` & `translate-toolkit-3.9.0/translate/storage/symbian.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 import re
 
-
 charset_re = re.compile("CHARACTER_SET[ ]+(?P<charset>.*)")
 header_item_or_end_re = re.compile(
     "(((?P<key>[^ ]+)(?P<space>[ ]*:[ ]*)(?P<value>.*))|(?P<end_comment>[*]/))"
 )
 header_item_re = re.compile("(?P<key>[^ ]+)(?P<space>[ ]*:[ ]*)(?P<value>.*)")
 string_entry_re = re.compile(
     "(?P<start>rls_string[ ]+)(?P<id>[^ ]+)(?P<space>[ ]+)(?P<str>.*)"
```

### Comparing `translate-toolkit-3.8.6/translate/storage/tbx.py` & `translate-toolkit-3.9.0/translate/storage/tbx.py`

 * *Files 9% similar despite different names*

```diff
@@ -47,49 +47,50 @@
     def getid(self):
         # The id attribute is optional
         return self.xmlelement.get("id") or self.source
 
     def setid(self, value):
         return self.xmlelement.set("id", value)
 
+    def _get_origin_element(self, origin: str):
+        if origin == "pos":
+            return self.namespaced("termNote")
+        elif origin == "definition":
+            return self.namespaced("descrip")
+        return self.namespaced("note")
+
     def removenotes(self, origin=None):
         """Remove all the translator notes."""
-        notes = self.xmlelement.iterdescendants(self.namespaced("note"))
+        notes = self.xmlelement.iterdescendants(self._get_origin_element(origin))
         for note in notes:
             self.xmlelement.remove(note)
 
     def addnote(self, text, origin=None, position="append"):
         """Add a note specifically in a "note" tag"""
         if position != "append":
             self.removenotes(origin=origin)
 
         if text:
             text = text.strip()
         if not text:
             return
-        note = etree.SubElement(self.xmlelement, self.namespaced("note"))
+        note = etree.SubElement(self.xmlelement, self._get_origin_element(origin))
         note.text = text
-        if origin:
+        if origin and origin not in ("pos", "definition"):
             note.set("from", origin)
 
     def _getnotelist(self, origin=None):
         """Returns the text from notes matching ``origin`` or all notes.
 
         :param origin: The origin of the note (or note type)
         :type origin: String
         :return: The text from notes matching ``origin``
         :rtype: List
         """
-        note_nodes = []
-        if origin == "pos":
-            note_nodes = self.xmlelement.iterdescendants(self.namespaced("termNote"))
-        elif origin == "definition":
-            note_nodes = self.xmlelement.iterdescendants(self.namespaced("descrip"))
-        else:
-            note_nodes = self.xmlelement.iterdescendants(self.namespaced("note"))
+        note_nodes = self.xmlelement.iterdescendants(self._get_origin_element(origin))
         # TODO: consider using xpath to construct initial_list directly
         # or to simply get the correct text from the outset (just remember to
         # check for duplication.
         initial_list = [
             lisa.getText(note, getXMLspace(self.xmlelement, self._default_xml_space))
             for note in note_nodes
         ]
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_aresource.py` & `translate-toolkit-3.9.0/translate/storage/test_aresource.py`

 * *Files 1% similar despite different names*

```diff
@@ -270,15 +270,15 @@
     def test_parse_leading_space(self):
         string = " leading space"
         xml = '<string name="teststring">" leading space"</string>\n'
         self.__check_parse(string, xml)
 
     def test_parse_quoted_newlines(self):
         self.__check_parse(
-            "\n\nstring with newlines",
+            "\n\n\n\nstring with newlines",
             r"""<string name="teststring">"
 \n
 \nstring with newlines"</string>
 """,
         )
 
     def test_parse_xml_entities(self):
@@ -465,14 +465,29 @@
         self.__check_parse(string, xml)
 
     def test_parse_unicode(self):
         with pytest.raises(ValueError):
             self.__check_parse("", r'<string name="test">\utest</string>')
         self.__check_parse("\u0230", r'<string name="test">\u0230</string>')
 
+    def test_single_unescaped(self):
+        string = "a b c d"
+        xml = '<string name="teststring">a\nb\tc d</string>'
+        self.__check_parse(string, xml)
+
+    def test_single_escaped_alone(self):
+        string = "a\nb\tc d"
+        xml = '<string name="teststring">a"\n"b"\t"c" "d</string>'
+        self.__check_parse(string, xml)
+
+    def test_single_escaped_full(self):
+        string = "a\nb\tc d"
+        xml = '<string name="teststring">"a\nb\tc d"</string>'
+        self.__check_parse(string, xml)
+
 
 class TestAndroidResourceFile(test_monolingual.TestMonolingualStore):
     StoreClass = aresource.AndroidResourceFile
 
     def test_targetlanguage_default_handlings(self):
         store = self.StoreClass()
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_base.py` & `translate-toolkit-3.9.0/translate/storage/test_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,16 @@
 
 
 import os
 from io import BytesIO
 
 from translate.misc.multistring import multistring
 from translate.storage import base, factory
-from translate.storage.placeables import general, parse as rich_parse
+from translate.storage.placeables import general
+from translate.storage.placeables import parse as rich_parse
 
 
 def headerless_len(units):
     """return count of translatable (non header) units"""
     return len(list(filter(lambda x: not x.isheader(), units)))
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_catkeys.py` & `translate-toolkit-3.9.0/translate/storage/test_catkeys.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_cpo.py` & `translate-toolkit-3.9.0/translate/storage/test_cpo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from io import BytesIO
 
 from pytest import importorskip, mark, raises
 
 from translate.misc.multistring import multistring
 from translate.storage import test_po
 
-
 pytestmark = mark.skipif(
     not sys.platform.startswith("linux"), reason="cpo is only available on Linux"
 )
 
 
 cpo = importorskip("translate.storage.cpo")
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_csvl10n.py` & `translate-toolkit-3.9.0/translate/storage/test_csvl10n.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_directory.py` & `translate-toolkit-3.9.0/translate/storage/test_directory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_dtd.py` & `translate-toolkit-3.9.0/translate/storage/test_dtd.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_factory.py` & `translate-toolkit-3.9.0/translate/storage/test_factory.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_flatxml.py` & `translate-toolkit-3.9.0/translate/storage/test_flatxml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_html.py` & `translate-toolkit-3.9.0/translate/storage/test_html.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_jsonl10n.py` & `translate-toolkit-3.9.0/translate/storage/test_jsonl10n.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
 
 from pytest import raises
 
 from translate.misc.multistring import multistring
 from translate.storage import base, jsonl10n, test_monolingual
 
-
 JSON_I18NEXT = """{
     "key": "value",
     "keyDeep": {
         "inner": "value"
     },
     "keyPluralSimple": "the singular",
     "keyPluralSimple_plural": "the plural",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_mo.py` & `translate-toolkit-3.9.0/translate/storage/test_mo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_monolingual.py` & `translate-toolkit-3.9.0/translate/storage/test_monolingual.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_mozilla_lang.py` & `translate-toolkit-3.9.0/translate/storage/test_mozilla_lang.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_oo.py` & `translate-toolkit-3.9.0/translate/storage/test_oo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_php.py` & `translate-toolkit-3.9.0/translate/storage/test_php.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_po.py` & `translate-toolkit-3.9.0/translate/storage/test_po.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_pocommon.py` & `translate-toolkit-3.9.0/translate/storage/test_pocommon.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_poheader.py` & `translate-toolkit-3.9.0/translate/storage/test_poheader.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_poxliff.py` & `translate-toolkit-3.9.0/translate/storage/test_poxliff.py`

 * *Files 16% similar despite different names*

```diff
@@ -118,7 +118,30 @@
             == "Zulu translation of program ABC\nazoozoo come back!"
         )
         assert xlifffile.units[0].getnotes("developer") == "azoozoo come back!"
         assert (
             xlifffile.units[0].getnotes("po-translator")
             == "Zulu translation of program ABC"
         )
+
+    def test_plural(self):
+        minixlf = (
+            self.xliffskeleton
+            % """
+        <group id="1238108068" restype="x-gettext-plurals">
+                <trans-unit id="1238108068[0]" xml:space="preserve">
+                        <source>This field must contain at least {0,number} character</source>
+                </trans-unit>
+                <trans-unit id="1238108068[1]" xml:space="preserve">
+                        <source>This field must contain at least {0,number} characters</source>
+                </trans-unit>
+        </group>
+            """
+        )
+        xlifffile = self.StoreClass.parsestring(minixlf)
+        assert len(xlifffile.units) == 1
+        unit = xlifffile.units[0]
+        assert unit.source.strings == [
+            "This field must contain at least {0,number} character",
+            "This field must contain at least {0,number} characters",
+        ]
+        assert unit.target == ["", ""]
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_properties.py` & `translate-toolkit-3.9.0/translate/storage/test_properties.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from io import BytesIO
 
 from pytest import mark, raises
 
 from translate.misc.multistring import multistring
 from translate.storage import properties, test_monolingual
 
-
 # Note that DialectJava delimitors are ["=", ":", " "]
 
 
 def test_find_delimiter_pos_simple():
     """Simple tests to find the various delimiters"""
     assert properties.DialectJava.find_delimiter("key=value") == ("=", 3)
     assert properties.DialectJava.find_delimiter("key:value") == (":", 3)
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_pypo.py` & `translate-toolkit-3.9.0/translate/storage/test_pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_qm.py` & `translate-toolkit-3.9.0/translate/storage/test_qm.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_qph.py` & `translate-toolkit-3.9.0/translate/storage/test_qph.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 
 """Tests for Qt Linguist phase book storage class"""
 
 from translate.storage import qph, test_base
 from translate.storage.placeables import parse, xliff
 
-
 xliffparsers = []
 for attrname in dir(xliff):
     attr = getattr(xliff, attrname)
     if (
         type(attr) is type
         and attrname not in ("XLIFFPlaceable")
         and hasattr(attr, "parse")
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_rc.py` & `translate-toolkit-3.9.0/translate/storage/test_rc.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_resourcedictionary.py` & `translate-toolkit-3.9.0/translate/storage/test_resourcedictionary.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_resx.py` & `translate-toolkit-3.9.0/translate/storage/test_resx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_stringsdict.py` & `translate-toolkit-3.9.0/translate/storage/test_stringsdict.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_subtitles.py` & `translate-toolkit-3.9.0/translate/storage/test_subtitles.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_tiki.py` & `translate-toolkit-3.9.0/translate/storage/test_tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_tmx.py` & `translate-toolkit-3.9.0/translate/storage/test_tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_trados.py` & `translate-toolkit-3.9.0/translate/storage/test_trados.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from pytest import importorskip
 
-
 trados = importorskip("translate.storage.trados")
 
 
 def test_unescape():
     # NBSP
     assert trados.unescape("Ordre du jour\\~:") == "Ordre du jour\u00a0:"
     assert (
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_ts2.py` & `translate-toolkit-3.9.0/translate/storage/test_ts2.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,18 +18,18 @@
 
 """Tests for Qt Linguist storage class
 
 Reference implementation & tests:
 http://code.qt.io/cgit/qt/qttools.git/tree/tests/auto/linguist/lconvert/data
 """
 
-from translate.storage import test_base, ts2 as ts
+from translate.storage import test_base
+from translate.storage import ts2 as ts
 from translate.storage.placeables import parse, xliff
 
-
 TS_NUMERUS = """<?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1">
 <context>
     <name>Dialog2</name>
     <message numerus="yes">
         <location filename="../tools/qtconfig/mainwindow.cpp" line="+202"/>
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_txt.py` & `translate-toolkit-3.9.0/translate/storage/test_txt.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_wordfast.py` & `translate-toolkit-3.9.0/translate/storage/test_wordfast.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from translate.storage import test_base, wordfast as wf
+from translate.storage import test_base
+from translate.storage import wordfast as wf
 
 
 class TestWFTime:
     @staticmethod
     def test_timestring():
         """Setting and getting times set using a timestring"""
         wftime = wf.WordfastTime()
```

### Comparing `translate-toolkit-3.8.6/translate/storage/test_xliff.py` & `translate-toolkit-3.9.0/translate/storage/test_xliff.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_yaml.py` & `translate-toolkit-3.9.0/translate/storage/test_yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/test_zip.py` & `translate-toolkit-3.9.0/translate/storage/test_zip.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/tiki.py` & `translate-toolkit-3.9.0/translate/storage/tiki.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/tmdb.py` & `translate-toolkit-3.9.0/translate/storage/tmdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import threading
 import time
 from sqlite3 import dbapi2
 
 from translate.lang import data
 from translate.search.lshtein import LevenshteinComparer
 
-
 STRIP_REGEXP = re.compile(r"\W", re.UNICODE)
 
 
 class LanguageError(Exception):
     def __init__(self, value):
         self.value = value
```

### Comparing `translate-toolkit-3.8.6/translate/storage/tmx.py` & `translate-toolkit-3.9.0/translate/storage/tmx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/trados.py` & `translate-toolkit-3.9.0/translate/storage/trados.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,14 @@
 """
 
 import re
 import time
 
 from translate.storage import base
 
-
 try:
     # FIXME see if we can't use lxml
     from bs4 import BeautifulSoup
 except ImportError:
     raise ImportError(
         "BeautifulSoup 4 is not installed. Support for Trados txt is disabled."
     )
```

### Comparing `translate-toolkit-3.8.6/translate/storage/ts.py` & `translate-toolkit-3.9.0/translate/storage/ts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/ts2.py` & `translate-toolkit-3.9.0/translate/storage/ts2.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
 
 from translate.lang import data
 from translate.misc.multistring import multistring
 from translate.storage import lisa
 from translate.storage.placeables import general
 from translate.storage.workflow import StateEnum as state
 
-
 # TODO: handle translation types
 
 
 class tsunit(lisa.LISAunit):
     """A single term in the TS file."""
 
     rootNode = "message"
```

### Comparing `translate-toolkit-3.8.6/translate/storage/txt.py` & `translate-toolkit-3.9.0/translate/storage/txt.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,14 @@
   - MediaWiki
 """
 
 import re
 
 from translate.storage import base
 
-
 dokuwiki = [
     (
         "Dokuwiki heading",
         re.compile(r"( ?={2,6}[\s]*)(.+)"),
         re.compile(r"([\s]*={2,6}[\s]*)$"),
     ),
     ("Dokuwiki bullet", re.compile(r"([\s]{2,}\*[\s]*)(.+)"), re.compile(r"[\s]+$")),
```

### Comparing `translate-toolkit-3.8.6/translate/storage/utx.py` & `translate-toolkit-3.9.0/translate/storage/utx.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/wordfast.py` & `translate-toolkit-3.9.0/translate/storage/wordfast.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 """
 
 import csv
 import time
 
 from translate.storage import base
 
-
 WF_TIMEFORMAT = "%Y%m%d~%H%M%S"
 """Time format used by Wordfast"""
 
 WF_FIELDNAMES_HEADER = [
     "date",
     "userlist",
     "tucount",
```

### Comparing `translate-toolkit-3.8.6/translate/storage/workflow.py` & `translate-toolkit-3.9.0/translate/storage/workflow.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xliff.py` & `translate-toolkit-3.9.0/translate/storage/xliff.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     setXMLlang,
     setXMLspace,
 )
 from translate.storage import base, lisa
 from translate.storage.placeables.lisa import strelem_to_xml, xml_to_strelem
 from translate.storage.workflow import StateEnum as state
 
-
 # TODO: handle translation types
 
 ID_SEPARATOR = "\04"
 # ID_SEPARATOR is commonly used through toolkit to generate compound
 # unit ids (for instance to concatenate msgctxt and msgid in po), but
 # \04 is an illegal char in XML 1.0, ID_SEPARATOR_SAFE will be used
 # instead when converting between xliff and other toolkit supported
```

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/__init__.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/extract.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/extract.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/generate.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/generate.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/misc.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/misc.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/test_misc.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/test_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 #
 
 from translate.storage.xml_extract import misc
 
-
 # reduce_tree
 
 test_tree_1 = (
     "a",
     [("b", []), ("c", [("d", []), ("e", [])]), ("f", [("g", [("h", [])])])],
 )
```

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/test_unit_tree.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/test_unit_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program; if not, see <http://www.gnu.org/licenses/>.
 #
 
 from translate.storage.xml_extract import unit_tree
 
-
 # _split_xpath_component
 
 
 def test__split_xpath_component():
     assert ("some-tag", 0) == unit_tree._split_xpath_component("some-tag[0]")
```

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/test_xpath_breadcrumb.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/test_xpath_breadcrumb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/unit_tree.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/unit_tree.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_extract/xpath_breadcrumb.py` & `translate-toolkit-3.9.0/translate/storage/xml_extract/xpath_breadcrumb.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/xml_name.py` & `translate-toolkit-3.9.0/translate/storage/xml_name.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/yaml.py` & `translate-toolkit-3.9.0/translate/storage/yaml.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/storage/zip.py` & `translate-toolkit-3.9.0/translate/storage/zip.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/__init__.py` & `translate-toolkit-3.9.0/translate/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/build_tmdb.py` & `translate-toolkit-3.9.0/translate/tools/build_tmdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import logging
 import os
 from argparse import ArgumentParser
 
 from translate.storage import factory, tmdb
 
-
 logger = logging.getLogger(__name__)
 
 
 class Builder:
     def __init__(self, tmdbfile, source_lang, target_lang, filenames):
         self.tmdb = tmdb.TMDB(tmdbfile)
         self.source_lang = source_lang
```

### Comparing `translate-toolkit-3.8.6/translate/tools/phppo2pypo.py` & `translate-toolkit-3.9.0/translate/tools/phppo2pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/poclean.py` & `translate-toolkit-3.9.0/translate/tools/poclean.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 """
 
 import re
 
 from translate.misc.multistring import multistring
 from translate.storage import factory
 
-
 tw4winre = re.compile(r"\{0>.*?<\}\d{1,3}\{>(.*?)<0\}", re.M | re.S)
 
 
 def cleanunit(unit):
     """cleans the targets in the given unit"""
     if isinstance(unit.target, multistring):
         strings = unit.target.strings
```

### Comparing `translate-toolkit-3.8.6/translate/tools/pocompile.py` & `translate-toolkit-3.9.0/translate/tools/pocompile.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/poconflicts.py` & `translate-toolkit-3.9.0/translate/tools/poconflicts.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/pocount.py` & `translate-toolkit-3.9.0/translate/tools/pocount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# pyright: strictDictionaryInference=true
 #
 # Copyright 2003-2009 Zuza Software Foundation
 #
 # This file is part of the Translate Toolkit.
 #
 # This program is free software; you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
@@ -19,27 +20,36 @@
 """Count strings and words for supported localization files.
 
 These include: XLIFF, TMX, Gettex PO and MO, Qt .ts and .qm, Wordfast TM, etc
 
 See: http://docs.translatehouse.org/projects/translate-toolkit/en/latest/commands/pocount.html
 for examples and usage instructions.
 """
+from __future__ import annotations
 
+import csv
 import logging
 import os
 import re
 import sys
 from argparse import ArgumentParser
 from collections import defaultdict
+from dataclasses import dataclass
+from operator import itemgetter
 
 from translate.lang.common import Common
 from translate.misc.multistring import multistring
 from translate.storage import factory
 from translate.storage.workflow import StateEnum
 
+try:
+    from functools import cached_property
+except ImportError:
+    # Fix for python 3.7
+    cached_property = property
 
 extended_state_strings = {
     StateEnum.EMPTY: "empty",
     StateEnum.NEEDS_WORK: "needs-work",
     StateEnum.REJECTED: "rejected",
     StateEnum.NEEDS_REVIEW: "needs-review",
     StateEnum.UNREVIEWED: "unreviewed",
@@ -54,20 +64,14 @@
     UNTRANSLATED: "untranslated",
     FUZZY: "fuzzy",
     TRANSLATED: "translated",
 }
 
 logger = logging.getLogger(__name__)
 
-# define style constants
-style_full, style_csv, style_short_strings, style_short_words = range(4)
-
-# default output style
-default_style = style_full
-
 # kdepluralre = re.compile("^_n: ") #Restore this if you really need support for old kdeplurals
 brtagre = re.compile(r"<br\s*?/?>")
 # xmltagre is a direct copy of the from placeables/general.py
 xmltagre = re.compile(
     r"""
         <                         # start of opening tag
         ([\w.:]+)                 # tag name, possibly namespaced
@@ -143,37 +147,34 @@
         targetstrings = [unit.target or ""]
     for s in targetstrings:
         targetwords += wordcount(s)
     return sourcewords, targetwords
 
 
 def calcstats(filename):
-    """This is the previous implementation of calcstats() and is left for
-    comparison and debuging purposes.
-    """
     # ignore totally blank or header units
     try:
         store = factory.getobject(filename)
     except ValueError as e:
         logger.warning(e)
         return {}
 
-    units = [unit for unit in store.units if unit.istranslatable()]
+    units = [unit for unit in store.units if unit.istranslatable()]  # type: ignore
     translated = translatedmessages(units)
     fuzzy = fuzzymessages(units)
     review = [unit for unit in units if unit.isreview()]
     untranslated = untranslatedmessages(units)
     wordcounts = {id(unit): wordsinunit(unit) for unit in units}
     sourcewords = lambda elementlist: sum(
         wordcounts[id(unit)][0] for unit in elementlist
     )
     targetwords = lambda elementlist: sum(
         wordcounts[id(unit)][1] for unit in elementlist
     )
-    stats = {}
+    stats = {"filename": filename}
 
     # units
     stats["translated"] = len(translated)
     stats["fuzzy"] = len(fuzzy)
     stats["untranslated"] = len(untranslated)
     stats["review"] = len(review)
     stats["total"] = stats["translated"] + stats["fuzzy"] + stats["untranslated"]
@@ -222,117 +223,59 @@
         state_stats["targetwords"] += wordcounts[id(unit)][1]
 
         stats[extended_state] = state_stats
 
     return stats
 
 
-def summarize(title, stats, style=style_full, indent=8, incomplete_only=False):
-    """Print summary for a .po file in specified format.
-
-    :param title: name of .po file
-    :param stats: array with translation statistics for the file specified
-    :param indent: indentation of the 2nd column (length of longest filename)
-    :param incomplete_only: omit fully translated files
-    :type incomplete_only: Boolean
-    :rtype: Boolean
-    :return: 1 if counting incomplete files (incomplete_only=True) and the
-             file is completely translated, 0 otherwise
-    """
-
-    def percent(denominator, devisor):
-        if devisor == 0:
-            return 0
-        else:
-            return denominator * 100 / devisor
+@dataclass
+class Renderer:
+    stats: StatCollector
+
+    def header(self):
+        pass
+
+    def entry(self, title: str, stats: dict):
+        pass
+
+    def footer(self):
+        pass
+
+
+@dataclass
+class CsvRenderer(Renderer):
+    def __post_init__(self):
+        self._fields = {
+            "title": "Filename",
+            "translated": "Translated Messages",
+            "translatedsourcewords": "Translated Source Words",
+            "translatedtargetwords": "Translated Target Words",
+            "fuzzy": "Fuzzy Messages",
+            "fuzzysourcewords": "Fuzzy Source Words",
+            "untranslated": "Untranslated Messages",
+            "untranslatedsourcewords": "Untranslated Source Words",
+            "total": "Total Message",
+            "totalsourcewords": "Total Source Words",
+            "review": "Review Messages",
+            "reviewsourcewords": "Review Source Words",
+        }
+        self._writer = csv.DictWriter(sys.stdout, self._fields.values())
+
+    def header(self):
+        self._writer.writeheader()
+
+    def entry(self, title, stats):
+        data = stats.copy()
+        data.update(title=title)
+        row = {v: data[k] for k, v in self._fields.items()}
+        self._writer.writerow(row)
 
-    if incomplete_only and (stats["total"] == stats["translated"]):
-        return 1
 
-    if style == style_csv:
-        print("%s, " % title, end=" ")
-        print(
-            "%d, %d, %d,"
-            % (
-                stats["translated"],
-                stats["translatedsourcewords"],
-                stats["translatedtargetwords"],
-            ),
-            end=" ",
-        )
-        print("%d, %d," % (stats["fuzzy"], stats["fuzzysourcewords"]), end=" ")
-        print(
-            "%d, %d," % (stats["untranslated"], stats["untranslatedsourcewords"]),
-            end=" ",
-        )
-        print("%d, %d" % (stats["total"], stats["totalsourcewords"]), end=" ")
-        if stats["review"] > 0:
-            print(", %d, %d" % (stats["review"], stats["reviewsourdcewords"]), end=" ")
-        print()
-    elif style == style_short_strings:
-        spaces = " " * (indent - len(title))
-        print(
-            "%s%s strings: total: %d\t| %st\t%sf\t%su\t| %st\t%sf\t%su"
-            % (
-                ConsoleColor.HEADER() + title + ConsoleColor.ENDC(),
-                spaces,
-                stats["total"],
-                ConsoleColor.OKGREEN() + str(stats["translated"]) + ConsoleColor.ENDC(),
-                ConsoleColor.WARNING() + str(stats["fuzzy"]) + ConsoleColor.ENDC(),
-                ConsoleColor.FAIL() + str(stats["untranslated"]) + ConsoleColor.ENDC(),
-                ConsoleColor.OKGREEN()
-                + str(percent(stats["translated"], stats["total"]))
-                + "%"
-                + ConsoleColor.ENDC(),
-                ConsoleColor.WARNING()
-                + str(percent(stats["fuzzy"], stats["total"]))
-                + "%"
-                + ConsoleColor.ENDC(),
-                ConsoleColor.FAIL()
-                + str(percent(stats["untranslated"], stats["total"]))
-                + "%"
-                + ConsoleColor.ENDC(),
-            )
-        )
-    elif style == style_short_words:
-        spaces = " " * (indent - len(title))
-        print(
-            "%s%s source words: total: %d\t| %st\t%sf\t%su\t| %st\t%sf\t%su"
-            % (
-                ConsoleColor.HEADER() + title + ConsoleColor.ENDC(),
-                spaces,
-                stats["totalsourcewords"],
-                ConsoleColor.OKGREEN()
-                + str(stats["translatedsourcewords"])
-                + ConsoleColor.ENDC(),
-                ConsoleColor.WARNING()
-                + str(stats["fuzzysourcewords"])
-                + ConsoleColor.ENDC(),
-                ConsoleColor.FAIL()
-                + str(stats["untranslatedsourcewords"])
-                + ConsoleColor.ENDC(),
-                ConsoleColor.OKGREEN()
-                + str(
-                    percent(stats["translatedsourcewords"], stats["totalsourcewords"])
-                )
-                + "%"
-                + ConsoleColor.ENDC(),
-                ConsoleColor.WARNING()
-                + str(percent(stats["fuzzysourcewords"], stats["totalsourcewords"]))
-                + "%"
-                + ConsoleColor.ENDC(),
-                ConsoleColor.FAIL()
-                + str(
-                    percent(stats["untranslatedsourcewords"], stats["totalsourcewords"])
-                )
-                + "%"
-                + ConsoleColor.ENDC(),
-            )
-        )
-    else:  # style == style_full
+class FullRenderer(Renderer):
+    def entry(self, title, stats):
         print(
             "Processing file : " + ConsoleColor.HEADER() + title + ConsoleColor.ENDC()
         )
         print("Type               Strings      Words (source)    Words (translation)")
         print(
             ConsoleColor.OKGREEN()
             + "Translated:   %5d (%3d%%) %10d (%3d%%) %15d"
@@ -392,15 +335,112 @@
 
         if stats["review"] > 0:
             print(
                 "review:          %5d %17d                    n/a"
                 % (stats["review"], stats["reviewsourcewords"])
             )
         print()
-    return 0
+
+    def footer(self):
+        stats = self.stats
+        if stats.file_count > 1:
+            if stats.incomplete_only:
+                self.entry("TOTAL (incomplete only):", stats.totals)
+                print("File count (incomplete):   %5d" % len(stats.results))
+            else:
+                self.entry("TOTAL:", stats.totals)
+            print("File count:   %5d" % (stats.file_count))
+            print()
+
+
+@dataclass
+class ShortStringsRenderer(Renderer):
+    """
+    :param indent: indentation of the 2nd column (length of longest filename)
+    """
+
+    indent: int = 8
+
+    def entry(self, title, stats):
+        spaces = " " * (self.indent - len(title))
+        print(
+            "%s%s strings: total: %d\t| %st\t%sf\t%su\t| %st\t%sf\t%su"
+            % (
+                ConsoleColor.HEADER() + title + ConsoleColor.ENDC(),
+                spaces,
+                stats["total"],
+                ConsoleColor.OKGREEN() + str(stats["translated"]) + ConsoleColor.ENDC(),
+                ConsoleColor.WARNING() + str(stats["fuzzy"]) + ConsoleColor.ENDC(),
+                ConsoleColor.FAIL() + str(stats["untranslated"]) + ConsoleColor.ENDC(),
+                ConsoleColor.OKGREEN()
+                + str(percent(stats["translated"], stats["total"]))
+                + "%"
+                + ConsoleColor.ENDC(),
+                ConsoleColor.WARNING()
+                + str(percent(stats["fuzzy"], stats["total"]))
+                + "%"
+                + ConsoleColor.ENDC(),
+                ConsoleColor.FAIL()
+                + str(percent(stats["untranslated"], stats["total"]))
+                + "%"
+                + ConsoleColor.ENDC(),
+            )
+        )
+
+
+@dataclass
+class ShortWordsRenderer(Renderer):
+    """
+    :param indent: indentation of the 2nd column (length of longest filename)
+    """
+
+    indent: int = 8
+
+    def entry(self, title, stats):
+        spaces = " " * (self.indent - len(title))
+        print(
+            "%s%s source words: total: %d\t| %st\t%sf\t%su\t| %st\t%sf\t%su"
+            % (
+                ConsoleColor.HEADER() + title + ConsoleColor.ENDC(),
+                spaces,
+                stats["totalsourcewords"],
+                ConsoleColor.OKGREEN()
+                + str(stats["translatedsourcewords"])
+                + ConsoleColor.ENDC(),
+                ConsoleColor.WARNING()
+                + str(stats["fuzzysourcewords"])
+                + ConsoleColor.ENDC(),
+                ConsoleColor.FAIL()
+                + str(stats["untranslatedsourcewords"])
+                + ConsoleColor.ENDC(),
+                ConsoleColor.OKGREEN()
+                + str(
+                    percent(stats["translatedsourcewords"], stats["totalsourcewords"])
+                )
+                + "%"
+                + ConsoleColor.ENDC(),
+                ConsoleColor.WARNING()
+                + str(percent(stats["fuzzysourcewords"], stats["totalsourcewords"]))
+                + "%"
+                + ConsoleColor.ENDC(),
+                ConsoleColor.FAIL()
+                + str(
+                    percent(stats["untranslatedsourcewords"], stats["totalsourcewords"])
+                )
+                + "%"
+                + ConsoleColor.ENDC(),
+            )
+        )
+
+
+def percent(denominator, devisor):
+    if devisor == 0:
+        return 0
+    else:
+        return denominator * 100 / devisor
 
 
 def fuzzymessages(units):
     return [unit for unit in units if unit.isfuzzy() and unit.target]
 
 
 def translatedmessages(units):
@@ -411,147 +451,148 @@
     return [
         unit
         for unit in units
         if not (unit.istranslated() or unit.isfuzzy()) and unit.source
     ]
 
 
-class summarizer:
-    def __init__(self, filenames, style=default_style, incomplete_only=False):
-        self.totals = {}
-        self.filecount = 0
-        self.longestfilename = 0
-        self.style = style
+class StatCollector:
+    def __init__(self, items: list[str], incomplete_only=False):
         self.incomplete_only = incomplete_only
-        self.complete_count = 0
+        self._results: list[dict] = []
+        self._handle_items(items)
 
-        if self.style == style_csv:
-            print(
-                """Filename, Translated Messages, Translated Source Words, \
-Translated Target Words, Fuzzy Messages, Fuzzy Source Words, Untranslated Messages, \
-Untranslated Source Words, Total Message, Total Source Words, \
-Review Messages, Review Source Words"""
-            )
-        if self.style in (style_short_strings, style_short_words):
-            for filename in filenames:  # find longest filename
-                if len(filename) > self.longestfilename:
-                    self.longestfilename = len(filename)
-        for filename in filenames:
-            if not os.path.exists(filename):
-                logger.error("cannot process %s: does not exist", filename)
-                continue
-            elif os.path.isdir(filename):
-                self.handledir(filename)
-            else:
-                self.handlefile(filename)
-        if self.filecount > 1 and (self.style == style_full):
-            if self.incomplete_only:
-                summarize("TOTAL (incomplete only):", self.totals, incomplete_only=True)
-                print(
-                    "File count (incomplete):   %5d"
-                    % (self.filecount - self.complete_count)
-                )
-            else:
-                summarize("TOTAL:", self.totals, incomplete_only=False)
-            print("File count:   %5d" % (self.filecount))
-            print()
+    def render(self, renderer_class: type[Renderer]):
+        if renderer_class in (ShortWordsRenderer, ShortStringsRenderer):
+            renderer = renderer_class(self, indent=self.longest_filename)
+        else:
+            renderer = renderer_class(self)
 
-    def updatetotals(self, stats):
-        """Update self.totals with the statistics in stats."""
-        for key in stats.keys():
-            if key == "extended":
-                # FIXME: calculate extended totals
+        renderer.header()
+        for entry in self.results:
+            renderer.entry(entry["filename"], entry)
+        renderer.footer()
+
+    @cached_property
+    def results(self):
+        if self.incomplete_only:
+            return [s for s in self._results if s["total"] != s["translated"]]
+        else:
+            return self._results
+
+    def _handle_items(self, items: list[str]):
+        for item in items:
+            if not os.path.exists(item):
+                logger.error("cannot process %s: does not exist", item)
                 continue
-            if key not in self.totals:
-                self.totals[key] = 0
-            self.totals[key] += stats[key]
+            elif os.path.isdir(item):
+                self._handle_dir(item)
+            else:
+                self._handle_single_file(item)
 
-    def handlefile(self, filename):
-        try:
-            stats = calcstats(filename)
-            self.updatetotals(stats)
-            self.complete_count += summarize(
-                filename, stats, self.style, self.longestfilename, self.incomplete_only
-            )
-            self.filecount += 1
-        except Exception:  # This happens if we have a broken file.
-            logger.error(sys.exc_info()[1])
+    def _handle_dir(self, dirname):
+        _, name = os.path.split(dirname)
+        if name in ["CVS", ".svn", "_darcs", ".git", ".hg", ".bzr"]:
+            return
+        entries = os.listdir(dirname)
+        self._handle_multiple_files(dirname, entries)
 
-    def handlefiles(self, dirname, filenames):
+    def _handle_multiple_files(self, dirname, filenames):
         for filename in filenames:
             pathname = os.path.join(dirname, filename)
             if os.path.isdir(pathname):
-                self.handledir(pathname)
+                self._handle_dir(pathname)
             else:
-                self.handlefile(pathname)
+                self._handle_single_file(pathname)
 
-    def handledir(self, dirname):
-        path, name = os.path.split(dirname)
-        if name in ["CVS", ".svn", "_darcs", ".git", ".hg", ".bzr"]:
-            return
-        entries = os.listdir(dirname)
-        self.handlefiles(dirname, entries)
+    def _handle_single_file(self, filename):
+        try:
+            stats = calcstats(filename)
+            self._results.append(stats)
+        except Exception:  # This happens if we have a broken file.
+            logger.error(sys.exc_info()[1])
+
+    @property
+    def longest_filename(self):
+        filenames = list(map(itemgetter("filename"), self.results)) or [""]
+        return max(len(f) for f in filenames)
+
+    @property
+    def file_count(self):
+        return len(self._results)
+
+    @cached_property
+    def totals(self) -> dict:
+        """Total stats"""
+        totals = defaultdict(int)
+        for stats in self._results:
+            for key, value in stats.items():
+                if key in ["extended", "filename"]:
+                    # FIXME: calculate extended totals
+                    continue
+                totals[key] += value
+        return totals
 
 
-def main():
+def main(arguments=None):
     parser = ArgumentParser()
     parser.add_argument(
         "--incomplete",
         action="store_true",
         default=False,
         dest="incomplete_only",
         help="skip 100%% translated files.",
     )
     output_group = parser.add_argument_group("Output format")
     megroup = output_group.add_mutually_exclusive_group()
     megroup.add_argument(
         "--full",
         action="store_const",
-        const=style_full,
+        const=FullRenderer,
         dest="style",
-        default=style_full,
+        default=FullRenderer,
         help="(default) statistics in full, verbose format",
     )
     megroup.add_argument(
         "--csv",
         action="store_const",
-        const=style_csv,
+        const=CsvRenderer,
         dest="style",
         help="statistics in CSV format",
     )
     megroup.add_argument(
         "--short",
         action="store_const",
-        const=style_short_strings,
+        const=ShortStringsRenderer,
         dest="style",
         help="same as --short-strings",
     )
     megroup.add_argument(
         "--short-strings",
         action="store_const",
-        const=style_short_strings,
+        const=ShortStringsRenderer,
         dest="style",
         help="statistics of strings in short format - one line per file",
     )
     megroup.add_argument(
         "--short-words",
         action="store_const",
-        const=style_short_words,
+        const=ShortWordsRenderer,
         dest="style",
         help="statistics of words in short format - one line per file",
     )
     output_group.add_argument(
         "--no-color", action="store_true", help="show output without color"
     )
 
     parser.add_argument("files", nargs="+")
 
-    args = parser.parse_args()
+    args = parser.parse_args(arguments)
 
     logging.basicConfig(format="%(name)s: %(levelname)s: %(message)s")
     ConsoleColor.color_mode = not args.no_color
 
-    summarizer(args.files, args.style, args.incomplete_only)
+    StatCollector(args.files, args.incomplete_only).render(args.style)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `translate-toolkit-3.8.6/translate/tools/podebug.py` & `translate-toolkit-3.9.0/translate/tools/podebug.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,16 @@
 
 import os
 import re
 from hashlib import md5
 
 from translate.convert import dtd2po
 from translate.storage import factory
-from translate.storage.placeables import StringElem, general, parse as rich_parse
+from translate.storage.placeables import StringElem, general
+from translate.storage.placeables import parse as rich_parse
 
 
 def add_prefix(prefix, stringelems):
     for stringelem in stringelems:
         for string in stringelem.flatten():
             if len(string.sub) > 0:
                 string.sub[0] = prefix + string.sub[0]
```

### Comparing `translate-toolkit-3.8.6/translate/tools/pogrep.py` & `translate-toolkit-3.9.0/translate/tools/pogrep.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/pomerge.py` & `translate-toolkit-3.9.0/translate/tools/pomerge.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/porestructure.py` & `translate-toolkit-3.9.0/translate/tools/porestructure.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/posegment.py` & `translate-toolkit-3.9.0/translate/tools/posegment.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/poswap.py` & `translate-toolkit-3.9.0/translate/tools/poswap.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/poterminology.py` & `translate-toolkit-3.9.0/translate/tools/poterminology.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 import sys
 from operator import itemgetter
 
 from translate.lang import factory as lang_factory
 from translate.misc import file_discovery, optrecurse
 from translate.storage import factory, po
 
-
 logger = logging.getLogger(__name__)
 
 
 def create_termunit(
     term, unit, targets, locations, sourcenotes, transnotes, filecounts
 ):
     termunit = po.pounit(term)
```

### Comparing `translate-toolkit-3.8.6/translate/tools/pretranslate.py` & `translate-toolkit-3.9.0/translate/tools/pretranslate.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 See: http://docs.translatehouse.org/projects/translate-toolkit/en/latest/commands/pretranslate.html
 for examples and usage instructions.
 """
 
 from translate.search import match
 from translate.storage import factory
 
-
 # We don't want to reinitialise the TM each time, so let's store it here.
 tmmatcher = None
 
 
 def memory(tmfiles, max_candidates=1, min_similarity=75, max_length=1000):
     """Returns the TM store to use. Only initialises on first call."""
     global tmmatcher
```

### Comparing `translate-toolkit-3.8.6/translate/tools/pydiff.py` & `translate-toolkit-3.9.0/translate/tools/pydiff.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,14 @@
 import difflib
 import fnmatch
 import os
 import sys
 import time
 from argparse import ArgumentParser
 
-
 lineterm = "\n"
 
 
 def main():
     """main program for pydiff"""
     parser = ArgumentParser()
     # GNU diff like options
```

### Comparing `translate-toolkit-3.8.6/translate/tools/pypo2phppo.py` & `translate-toolkit-3.9.0/translate/tools/pypo2phppo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_phppo2pypo.py` & `translate-toolkit-3.9.0/translate/tools/test_phppo2pypo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_pocount.py` & `translate-toolkit-3.9.0/translate/tools/test_pocount.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from io import BytesIO
 
 from pytest import mark
 
 from translate.storage import po
 from translate.tools import pocount
 
+from ._test_utils import requires_py38_mark, test_po_files
+
 
 class TestCount:
     @staticmethod
     def count(source, expectedsource, target=None, expectedtarget=None):
         """simple helper to check the respective word counts"""
         poelement = po.pounit(source)
         if target is not None:
@@ -158,7 +160,24 @@
         stats = pocount.calcstats(pofile)
         assert stats["untranslatedsourcewords"] == 2
 
     def test_totalsourcewords(self):
         pofile = BytesIO(self.inputdata)
         stats = pocount.calcstats(pofile)
         assert stats["totalsourcewords"] == 6
+
+
+@requires_py38_mark
+@mark.parametrize("style", ["csv", "full", "short-strings", "short-words"])
+@mark.parametrize("incomplete", [True, False], ids=lambda v: f"incomplete={v}")
+@mark.parametrize("no_color", [True, False], ids=lambda v: f"no-color={v}")
+def test_output(style, incomplete, no_color, capsys, snapshot):
+    opts = [f"--{style}"]
+    if incomplete:
+        opts.append("--incomplete")
+    if no_color:
+        opts.append("--no-color")
+
+    pocount.main([*opts, *test_po_files])
+    stdout = capsys.readouterr()[0]
+
+    assert stdout == snapshot
```

### Comparing `translate-toolkit-3.8.6/translate/tools/test_podebug.py` & `translate-toolkit-3.9.0/translate/tools/test_podebug.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 from translate.storage import base, po, xliff
 from translate.tools import podebug
 
-
 PO_DOC = """
 msgid "This is a %s test, hooray."
 msgstr ""
 """
 
 XLIFF_DOC = """<?xml version="1.0" encoding="utf-8"?>
 <xliff xmlns="urn:oasis:names:tc:xliff:document:1.1" version="1.1">
```

### Comparing `translate-toolkit-3.8.6/translate/tools/test_pogrep.py` & `translate-toolkit-3.9.0/translate/tools/test_pogrep.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_pomerge.py` & `translate-toolkit-3.9.0/translate/tools/test_pomerge.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_posegment.py` & `translate-toolkit-3.9.0/translate/tools/test_posegment.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_poterminology.py` & `translate-toolkit-3.9.0/translate/tools/test_poterminology.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import os
 
 from translate.storage import factory
 from translate.tools import poterminology
 
-
 base_dir = os.path.dirname(os.path.dirname(os.path.dirname(__file__)))
 sample_po_file = os.path.join(base_dir, "tests", "xliff_conformance", "af-pootle.po")
 
 
 class TestPOTerminology:
     @staticmethod
     def test_term_extraction():
```

### Comparing `translate-toolkit-3.8.6/translate/tools/test_pretranslate.py` & `translate-toolkit-3.9.0/translate/tools/test_pretranslate.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate/tools/test_pypo2phppo.py` & `translate-toolkit-3.9.0/translate/tools/test_pypo2phppo.py`

 * *Files identical despite different names*

### Comparing `translate-toolkit-3.8.6/translate_toolkit.egg-info/PKG-INFO` & `translate-toolkit-3.9.0/translate_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: translate-toolkit
-Version: 3.8.6
+Version: 3.9.0
 Summary: Tools and API for translation and localization engineering.
 Home-page: https://toolkit.translatehouse.org/
 Download-URL: https://github.com/translate/translate/releases/
 Author: Translate
 Author-email: translate-devel@lists.sourceforge.net
 License: GPL-2.0-or-later
 Project-URL: Issue Tracker, https://github.com/translate/translate/issues
```

### Comparing `translate-toolkit-3.8.6/translate_toolkit.egg-info/SOURCES.txt` & `translate-toolkit-3.9.0/translate_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -255,14 +255,15 @@
 docs/releases/3.8.0.rst
 docs/releases/3.8.1.rst
 docs/releases/3.8.2.rst
 docs/releases/3.8.3.rst
 docs/releases/3.8.4.rst
 docs/releases/3.8.5.rst
 docs/releases/3.8.6.rst
+docs/releases/3.9.0.rst
 docs/releases/README.rst
 docs/releases/index.rst
 requirements/dev.txt
 requirements/dist.txt
 requirements/lint.txt
 requirements/optional.txt
 requirements/required.txt
@@ -271,30 +272,30 @@
 tests/cli/run_tests.sh
 tests/cli/test.inc.sh
 tests/cli/test_flatxml2po.sh
 tests/cli/test_flatxml2po_wrongkey.sh
 tests/cli/test_flatxml2po_wrongns.sh
 tests/cli/test_flatxml2po_wrongroot.sh
 tests/cli/test_flatxml2po_wrongvalue.sh
+tests/cli/test_junitmsgfmt_failure.sh
+tests/cli/test_junitmsgfmt_untranslated.sh
 tests/cli/test_po2csv.sh
 tests/cli/test_po2flatxml.sh
 tests/cli/test_po2flatxml_params.sh
 tests/cli/test_po2flatxml_preserve.sh
 tests/cli/test_po2flatxml_template.sh
 tests/cli/test_po2html.sh
 tests/cli/test_po2json_files_removeuntranslated.sh
 tests/cli/test_po2prop_mozilla_files.sh
 tests/cli/test_po2ts.sh
 tests/cli/test_po2txt.sh
 tests/cli/test_po2txt_threshold.sh
 tests/cli/test_pocount.sh
-tests/cli/test_pocount_help.sh
 tests/cli/test_pocount_mutually_exclusive.sh
 tests/cli/test_pocount_nonexistant.sh
-tests/cli/test_pocount_po_csv.sh
 tests/cli/test_pocount_po_file.sh
 tests/cli/test_pocount_po_fuzzy.sh
 tests/cli/test_pocount_xliff_states_no.sh
 tests/cli/test_pocount_xliff_states_yes.sh
 tests/cli/test_pofilter_listfilters.sh
 tests/cli/test_pofilter_manpage.sh
 tests/cli/test_posegment.sh
@@ -313,14 +314,18 @@
 tests/cli/data/test_flatxml2po_wrongkey/stderr.txt
 tests/cli/data/test_flatxml2po_wrongns/one.xml
 tests/cli/data/test_flatxml2po_wrongns/stderr.txt
 tests/cli/data/test_flatxml2po_wrongroot/one.xml
 tests/cli/data/test_flatxml2po_wrongroot/stderr.txt
 tests/cli/data/test_flatxml2po_wrongvalue/one.xml
 tests/cli/data/test_flatxml2po_wrongvalue/stderr.txt
+tests/cli/data/test_junitmsgfmt_failure/one.po
+tests/cli/data/test_junitmsgfmt_failure/stdout.txt
+tests/cli/data/test_junitmsgfmt_untranslated/one.po
+tests/cli/data/test_junitmsgfmt_untranslated/stdout.txt
 tests/cli/data/test_po2csv/one.po
 tests/cli/data/test_po2csv/out.txt
 tests/cli/data/test_po2flatxml/one.po
 tests/cli/data/test_po2flatxml/out.xml
 tests/cli/data/test_po2flatxml_params/one.po
 tests/cli/data/test_po2flatxml_params/out.xml
 tests/cli/data/test_po2flatxml_preserve/one.po
@@ -341,19 +346,17 @@
 tests/cli/data/test_po2ts/one.po
 tests/cli/data/test_po2ts/out.txt
 tests/cli/data/test_po2txt/one.po
 tests/cli/data/test_po2txt/out.txt
 tests/cli/data/test_po2txt_threshold/one.po
 tests/cli/data/test_po2txt_threshold/out.txt
 tests/cli/data/test_pocount/stderr.txt
-tests/cli/data/test_pocount_help/stdout.txt
 tests/cli/data/test_pocount_mutually_exclusive/stderr.txt
 tests/cli/data/test_pocount_nonexistant/stderr.txt
 tests/cli/data/test_pocount_po_csv/one.po
-tests/cli/data/test_pocount_po_csv/stdout.txt
 tests/cli/data/test_pocount_po_file/one.po
 tests/cli/data/test_pocount_po_file/stdout.txt
 tests/cli/data/test_pocount_po_fuzzy/one.po
 tests/cli/data/test_pocount_po_fuzzy/stdout.txt
 tests/cli/data/test_pocount_po_plurals/plural.po
 tests/cli/data/test_pocount_po_plurals/stdout.txt
 tests/cli/data/test_pocount_xliff_states_no/states.xlf
@@ -392,15 +395,14 @@
 tests/odf_xliff/test_inline-test_odf2xliff_inline-reference.xlf
 tests/odf_xliff/test_inline.odt
 tests/odf_xliff/test_odf_xliff.py
 tests/xliff_conformance/af-pootle.po
 tests/xliff_conformance/en-US.sdf
 tests/xliff_conformance/test_xliff_conformance.py
 tests/xliff_conformance/xliff-core-1.1.xsd
-tools/junitmsgfmt
 tools/phase
 tools/phaselist2goals
 tools/pocommentclean
 tools/pocompendium
 tools/pomigrate2
 tools/popuretext
 tools/poreencode
@@ -872,15 +874,17 @@
 translate/storage/xml_extract/misc.py
 translate/storage/xml_extract/test_misc.py
 translate/storage/xml_extract/test_unit_tree.py
 translate/storage/xml_extract/test_xpath_breadcrumb.py
 translate/storage/xml_extract/unit_tree.py
 translate/storage/xml_extract/xpath_breadcrumb.py
 translate/tools/__init__.py
+translate/tools/_test_utils.py
 translate/tools/build_tmdb.py
+translate/tools/junitmsgfmt.py
 translate/tools/phppo2pypo.py
 translate/tools/poclean.py
 translate/tools/pocompile.py
 translate/tools/poconflicts.py
 translate/tools/pocount.py
 translate/tools/podebug.py
 translate/tools/pogrep.py
@@ -888,23 +892,27 @@
 translate/tools/porestructure.py
 translate/tools/posegment.py
 translate/tools/poswap.py
 translate/tools/poterminology.py
 translate/tools/pretranslate.py
 translate/tools/pydiff.py
 translate/tools/pypo2phppo.py
+translate/tools/test_help.py
+translate/tools/test_junitmsgfmt.py
 translate/tools/test_phppo2pypo.py
 translate/tools/test_pocount.py
 translate/tools/test_podebug.py
 translate/tools/test_pogrep.py
 translate/tools/test_pomerge.py
 translate/tools/test_posegment.py
 translate/tools/test_poterminology.py
 translate/tools/test_pretranslate.py
 translate/tools/test_pypo2phppo.py
+translate/tools/__snapshots__/test_junitmsgfmt.ambr
+translate/tools/__snapshots__/test_pocount.ambr
 translate_toolkit.egg-info/PKG-INFO
 translate_toolkit.egg-info/SOURCES.txt
 translate_toolkit.egg-info/dependency_links.txt
 translate_toolkit.egg-info/entry_points.txt
 translate_toolkit.egg-info/not-zip-safe
 translate_toolkit.egg-info/requires.txt
 translate_toolkit.egg-info/top_level.txt
```

### Comparing `translate-toolkit-3.8.6/translate_toolkit.egg-info/entry_points.txt` & `translate-toolkit-3.9.0/translate_toolkit.egg-info/entry_points.txt`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 dtd2po = translate.convert.dtd2po:main
 flatxml2po = translate.convert.flatxml2po:main
 html2po = translate.convert.html2po:main
 ical2po = translate.convert.ical2po:main
 idml2po = translate.convert.idml2po:main
 ini2po = translate.convert.ini2po:main
 json2po = translate.convert.json2po:main
+junitmsgfmt = translate.tools.junitmsgfmt:main
 moz2po = translate.convert.moz2po:main
 mozfunny2prop = translate.convert.mozfunny2prop:main
 mozlang2po = translate.convert.mozlang2po:main
 odf2xliff = translate.convert.odf2xliff:main
 oo2po = translate.convert.oo2po:main
 oo2xliff = translate.convert.oo2xliff:main
 php2po = translate.convert.php2po:main
```

### Comparing `translate-toolkit-3.8.6/translate_toolkit.egg-info/requires.txt` & `translate-toolkit-3.9.0/translate_toolkit.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 lxml>=4.6.3
 
 [Fluent]
-fluent.syntax==0.18.1
+fluent.syntax==0.19.0
 
 [INI]
 iniparse==0.5
 
 [Languages]
 pycountry==22.3.5
 
@@ -21,29 +21,29 @@
 [Subtitles]
 aeidon==1.12
 
 [Trados]
 BeautifulSoup4>=4.3
 
 [YAML]
-ruamel.yaml==0.17.21
+ruamel.yaml==0.17.26
 
 [all]
 aeidon==1.12
 BeautifulSoup4>=4.3
 charset-normalizer==3.1.0
 cheroot==9.0.0
-fluent.syntax==0.18.1
+fluent.syntax==0.19.0
 iniparse==0.5
 phply==1.2.6
 pycountry==22.3.5
 pyenchant==3.2.2
 pyparsing==3.0.9
 python-Levenshtein>=0.12
-ruamel.yaml==0.17.21
+ruamel.yaml==0.17.26
 vobject==0.9.6.1
 
 [chardet]
 charset-normalizer==3.1.0
 
 [iCal]
 vobject==0.9.6.1
```

