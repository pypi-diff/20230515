# Comparing `tmp/cloup-2.0.0.post1.tar.gz` & `tmp/cloup-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cloup/cloup/dist/tmpuhbq1aqr/cloup-2.0.0.post1.tar", last modified: Sun Nov 13 21:29:31 2022, max compression
+gzip compressed data, was "/home/runner/work/cloup/cloup/dist/.tmp-hidybb66/cloup-2.1.0.tar", last modified: Mon May 15 01:54:24 2023, max compression
```

## Comparing `cloup-2.0.0.post1.tar` & `cloup-2.1.0.tar`

### file list

```diff
@@ -1,135 +1,135 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      552 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/enhancement.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/release.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2311 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1291 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)    20337 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1834 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/CREDITS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1525 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3382 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6716 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup/
--rw-r--r--   0 runner    (1001) docker     (121)     2029 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28378 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)    10625 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_context.py
--rw-r--r--   0 runner    (1001) docker     (121)    14130 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     1614 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     2856 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_params.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    10174 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_sections.py
--rw-r--r--   0 runner    (1001) docker     (121)     4510 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3013 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/_conditional.py
--rw-r--r--   0 runner    (1001) docker     (121)    21214 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/_core.py
--rw-r--r--   0 runner    (1001) docker     (121)     8059 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/common.py
--rw-r--r--   0 runner    (1001) docker     (121)     9420 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/constraints/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup/formatting/
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17233 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/formatting/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)      793 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/formatting/_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     8416 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/formatting/sep.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     6293 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/styling.py
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/types.py
--rw-r--r--   0 runner    (1001) docker     (121)      801 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)      490 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/cloup/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7105 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2692 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/cloup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      299 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      606 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/_autoapi_templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/_autoapi_templates/python/
--rw-r--r--   0 runner    (1001) docker     (121)     2866 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_autoapi_templates/python/module.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)    57493 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/basic-example.png
--rw-r--r--   0 runner    (1001) docker     (121)     4819 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/logo-dark-mode.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4960 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/logo-on-white.svg
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/_static/styles/
--rw-r--r--   0 runner    (1001) docker     (121)      653 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/styles/extensions-overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/styles/theme-overrides.css
--rw-r--r--   0 runner    (1001) docker     (121)    62855 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/_static/theme-elems.png
--rw-r--r--   0 runner    (1001) docker     (121)     4226 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1390 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      767 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/docs/pages/
--rw-r--r--   0 runner    (1001) docker     (121)     2814 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/aliases.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1787 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/arguments.rst
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)    20026 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/constraints.rst
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/credits.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13555 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/formatting.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/misc.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10917 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/option-groups.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4768 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/docs/pages/sections.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/arguments_with_help.py
--rw-r--r--   0 runner    (1001) docker     (121)     1015 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/default_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1133 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/flat_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     2896 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/git_sections.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/examples/manim/
--rw-r--r--   0 runner    (1001) docker     (121)      769 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/manim/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/manim/main.py
--rw-r--r--   0 runner    (1001) docker     (121)     4880 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/manim/render.py
--rw-r--r--   0 runner    (1001) docker     (121)     1827 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/examples/option_groups.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/dev.in
--rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (121)     1988 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/requirements/test.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/scripts/browser.py
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/scripts/copytree.py
--rw-r--r--   0 runner    (1001) docker     (121)     5553 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/scripts/generate_git_example.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/scripts/make-help.py
--rw-r--r--   0 runner    (1001) docker     (121)     1094 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/scripts/remove.py
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1822 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:31.000000 cloup-2.0.0.post1/tests/constraints/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1434 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2241 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/test_common.py
--rw-r--r--   0 runner    (1001) docker     (121)    14069 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/test_conditional_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)    14507 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (121)     7103 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/constraints/test_support.py
--rw-r--r--   0 runner    (1001) docker     (121)     6097 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/example_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     3539 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/example_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     5024 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_aliases.py
--rw-r--r--   0 runner    (1001) docker     (121)     3666 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1963 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_context.py
--rw-r--r--   0 runner    (1001) docker     (121)     8402 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_formatting.py
--rw-r--r--   0 runner    (1001) docker     (121)     8564 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_option_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)     4722 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_sections.py
--rw-r--r--   0 runner    (1001) docker     (121)     2518 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_sep.py
--rw-r--r--   0 runner    (1001) docker     (121)     1555 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_styling.py
--rw-r--r--   0 runner    (1001) docker     (121)      492 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1403 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1933 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-13 21:29:13.000000 cloup-2.0.0.post1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-15 01:54:09.000000 cloup-2.1.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-15 01:54:09.000000 cloup-2.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/enhancement.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/release.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-15 01:54:09.000000 cloup-2.1.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-15 01:54:09.000000 cloup-2.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-15 01:54:09.000000 cloup-2.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    20337 2023-05-15 01:54:09.000000 cloup-2.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-05-15 01:54:09.000000 cloup-2.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-15 01:54:09.000000 cloup-2.1.0/CREDITS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-15 01:54:09.000000 cloup-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-15 01:54:09.000000 cloup-2.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-15 01:54:24.000000 cloup-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-15 01:54:09.000000 cloup-2.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29113 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14135 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_params.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10194 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4524 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21196 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/constraints/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup/formatting/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17356 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8312 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/formatting/sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-15 01:54:09.000000 cloup-2.1.0/cloup/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2692 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-15 01:54:24.000000 cloup-2.1.0/cloup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-15 01:54:09.000000 cloup-2.1.0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_autoapi_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_autoapi_templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_autoapi_templates/python/module.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    57493 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/basic-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo-dark-mode.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo-on-white.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/_static/styles/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/styles/extensions-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5519 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/styles/theme-overrides.css
+-rw-r--r--   0 runner    (1001) docker     (123)    62855 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/_static/theme-elems.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/docs/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/aliases.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/arguments.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    20026 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/constraints.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/credits.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13553 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/formatting.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/misc.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/option-groups.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-15 01:54:09.000000 cloup-2.1.0/docs/pages/sections.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/arguments_with_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/default_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/flat_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/git_sections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/examples/manim/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/manim/render.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-15 01:54:09.000000 cloup-2.1.0/examples/option_groups.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/dev.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-15 01:54:09.000000 cloup-2.1.0/requirements/test.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/browser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/copytree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5561 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/generate_git_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/make-help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-15 01:54:09.000000 cloup-2.1.0/scripts/remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-15 01:54:24.000000 cloup-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-15 01:54:09.000000 cloup-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:24.000000 cloup-2.1.0/tests/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14069 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_conditional_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14505 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/constraints/test_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/example_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/example_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8563 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_option_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_sep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_styling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-15 01:54:09.000000 cloup-2.1.0/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-15 01:54:09.000000 cloup-2.1.0/tox.ini
```

### Comparing `cloup-2.0.0.post1/.github/ISSUE_TEMPLATE/bug_report.md` & `cloup-2.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/.github/workflows/tests.yaml` & `cloup-2.1.0/.github/workflows/tests.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -36,20 +36,20 @@
           python-version: ${{ matrix.python }}
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           pip install -U wheel
           pip install -U setuptools
-          pip install tox
+          pip install "tox < 4"
 
       - name: Run tox -e ${{ matrix.tox }}
         run: tox -e ${{ matrix.tox }}
 
-      - name: Install and run codecov (py38-click7 only)
+      - name: Install and run codecov (py38-click8 only)
         if: ${{ matrix.tox == 'py38-click8' }}
         run: |
           pip install codecov
           codecov
 
   publish:   # only if tests passed and this is a tagged commit.
     name: Publish package to PyPI
```

### Comparing `cloup-2.0.0.post1/.gitignore` & `cloup-2.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/CHANGELOG.rst` & `cloup-2.1.0/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/CONTRIBUTING.rst` & `cloup-2.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/CREDITS.rst` & `cloup-2.1.0/CREDITS.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/LICENSE` & `cloup-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/Makefile` & `cloup-2.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/PKG-INFO` & `cloup-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.0.0.post1
+Version: 2.1.0
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 .. |tests-status| image:: https://github.com/janLuke/cloup/workflows/Tests/badge.svg
     :alt: Tests status
     :target: https://github.com/janLuke/cloup/actions?query=workflow%3ATests
 
 .. |coverage| image:: https://codecov.io/github/janLuke/cloup/coverage.svg?branch=master
     :alt: Coverage Status
-    :target: https://codecov.io/github/janLuke/cloup?branch=master
+    :target: https://app.codecov.io/github/janluke/cloup/tree/master
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/cloup.svg
     :alt: Supported versions
     :target: https://pypi.org/project/cloup
 
 .. |dev-docs| image:: https://readthedocs.org/projects/cloup/badge/?version=latest
     :alt: Documentation Status (master branch)
@@ -66,15 +66,15 @@
 - **option groups** and an (optional) help section for positional arguments
 
 - **constraints**, like ``mutually_exclusive``, that can be applied to option groups
   or to any group of parameters, even *conditionally*
 
 - **subcommand aliases**
 
-- **subcommands sections**, i.e. the possibility to organize the subcommands of a
+- **subcommands sections**, i.e. the possibility of organizing the subcommands of a
   ``Group`` in multiple help sections
 
 - a **themeable HelpFormatter**  that:
 
   - has more parameters for adjusting widths and spacing, which can be provided
     at the context and command level
   - use a different layout when the terminal width is below a certain threshold
@@ -82,16 +82,16 @@
 
 - suggestions like "did you mean <subcommand>?" when you mistype a subcommand.
 
 Moreover, Cloup improves on **IDE support** providing decorators with *detailed*
 type hints and adding the static methods ``Context.settings()`` and
 ``HelpFormatter.settings()`` for creating dictionaries of settings.
 
-Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested** 
-against multiple versions of Python with nearly 100% coverage. 
+Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested**
+against multiple versions of Python with nearly 100% coverage.
 
 
 A simple example
 ================
 
 .. code-block:: python
```

### Comparing `cloup-2.0.0.post1/README.rst` & `cloup-2.1.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 .. |tests-status| image:: https://github.com/janLuke/cloup/workflows/Tests/badge.svg
     :alt: Tests status
     :target: https://github.com/janLuke/cloup/actions?query=workflow%3ATests
 
 .. |coverage| image:: https://codecov.io/github/janLuke/cloup/coverage.svg?branch=master
     :alt: Coverage Status
-    :target: https://codecov.io/github/janLuke/cloup?branch=master
+    :target: https://app.codecov.io/github/janluke/cloup/tree/master
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/cloup.svg
     :alt: Supported versions
     :target: https://pypi.org/project/cloup
 
 .. |dev-docs| image:: https://readthedocs.org/projects/cloup/badge/?version=latest
     :alt: Documentation Status (master branch)
@@ -65,15 +65,15 @@
 - **option groups** and an (optional) help section for positional arguments
 
 - **constraints**, like ``mutually_exclusive``, that can be applied to option groups
   or to any group of parameters, even *conditionally*
 
 - **subcommand aliases**
 
-- **subcommands sections**, i.e. the possibility to organize the subcommands of a
+- **subcommands sections**, i.e. the possibility of organizing the subcommands of a
   ``Group`` in multiple help sections
 
 - a **themeable HelpFormatter**  that:
 
   - has more parameters for adjusting widths and spacing, which can be provided
     at the context and command level
   - use a different layout when the terminal width is below a certain threshold
@@ -81,16 +81,16 @@
 
 - suggestions like "did you mean <subcommand>?" when you mistype a subcommand.
 
 Moreover, Cloup improves on **IDE support** providing decorators with *detailed*
 type hints and adding the static methods ``Context.settings()`` and
 ``HelpFormatter.settings()`` for creating dictionaries of settings.
 
-Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested** 
-against multiple versions of Python with nearly 100% coverage. 
+Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested**
+against multiple versions of Python with nearly 100% coverage.
 
 
 A simple example
 ================
 
 .. code-block:: python
```

### Comparing `cloup-2.0.0.post1/cloup/__init__.py` & `cloup-2.1.0/cloup/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/cloup/_commands.py` & `cloup-2.1.0/cloup/_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 - in the other signature, there's ``cls: ClickCommand`` without a default, where
   ``ClickCommand`` is a type variable.
 
 When and if the MyPy issue is resolved, the overloads will be removed.
 """
 import inspect
 from typing import (
-    Any, Callable, Dict, Iterable, List, NamedTuple, Optional, Tuple, Type,
-    TypeVar, Union, cast, overload,
+    Any, Callable, Dict, Iterable, List, NamedTuple, Optional, Sequence, Tuple,
+    Type, TypeVar, Union, cast, overload,
 )
 
 import click
 
 import cloup
 from ._context import Context
 from ._option_groups import OptionGroupMixin
 from ._sections import Section, SectionMixin
 from ._util import click_version_ge_8_1, first_bool, reindent
 from .constraints import ConstraintMixin
+from .styling import DEFAULT_THEME
 from .typing import AnyCallable
 
 ClickCommand = TypeVar('ClickCommand', bound=click.Command)
 ClickGroup = TypeVar('ClickGroup', bound=click.Group)
 
 
 class Command(ConstraintMixin, OptionGroupMixin, click.Command):
@@ -159,15 +160,15 @@
         super().add_command(cmd, name, section, fallback_to_default_section)
         name = cast(str, cmd.name) if name is None else name
         aliases = getattr(cmd, 'aliases', [])
         for alias in aliases:
             self.alias2name[alias] = name
 
     def resolve_command_name(self, ctx: click.Context, name: str) -> Optional[str]:
-        """Maps a string supposed to be a command name or an alias to a normalized
+        """Map a string supposed to be a command name or an alias to a normalized
         command name. If no match is found, it returns ``None``."""
         if ctx.token_normalize_func:
             name = ctx.token_normalize_func(name)
         if name in self.commands:
             return name
         return self.alias2name.get(name)
 
@@ -223,18 +224,34 @@
         )
 
     def format_subcommand_name(
         self, ctx: click.Context, name: str, cmd: click.Command
     ) -> str:
         aliases = getattr(cmd, 'aliases', None)
         if aliases and self.must_show_subcommand_aliases(ctx):
-            alias_list = ', '.join(aliases)
-            return f"{name} ({alias_list})"
+            assert isinstance(ctx, cloup.Context)
+            theme = cast(
+                cloup.HelpTheme, ctx.formatter_settings.get("theme", DEFAULT_THEME)
+            )
+            alias_list = self.format_subcommand_aliases(aliases, theme)
+            return f"{name} {alias_list}"
         return name
 
+    @staticmethod
+    def format_subcommand_aliases(aliases: Sequence[str], theme: cloup.HelpTheme) -> str:
+        secondary_style = theme.alias_secondary
+        if secondary_style is None or secondary_style == theme.alias:
+            return theme.alias(f"({', '.join(aliases)})")
+        else:
+            return (
+                secondary_style("(")
+                + secondary_style(", ").join(theme.alias(alias) for alias in aliases)
+                + secondary_style(")")
+            )
+
     # MyPy complains because "Signature of "group" incompatible with supertype".
     # The supertype signature is (*args, **kwargs), which is compatible with
     # this provided that you pass all arguments (expect "name") as keyword arg.
     @overload  # type: ignore
     def command(  # Why overloading? Refer to module docstring.
         self, name: Optional[str] = None,
         *,
@@ -281,15 +298,15 @@
     def command(
         self, name: Optional[str] = None, *,
         aliases: Optional[Iterable[str]] = None,
         cls: Optional[Type[ClickCommand]] = None,
         section: Optional[Section] = None,
         **kwargs: Any
     ) -> Callable[[AnyCallable], Union[Command, ClickCommand]]:
-        """Returns a decorator that creates a new subcommand of this ``Group``
+        """Return a decorator that creates a new subcommand of this ``Group``
         using the decorated function as callback.
 
         It takes the same arguments of :func:`command` plus:
 
         ``section``: ``Optional[Section]``
             if provided, put the subcommand in this section.
 
@@ -360,15 +377,15 @@
         self, name: Optional[None] = None,
         *,
         cls: Optional[Type[ClickGroup]] = None,
         aliases: Optional[Iterable[str]] = None,
         section: Optional[Section] = None,
         **kwargs: Any
     ) -> Callable[[AnyCallable], Union["Group", ClickGroup]]:
-        """Returns a decorator that creates a new subcommand of this ``Group``
+        """Return a decorator that creates a new subcommand of this ``Group``
         using the decorated function as callback.
 
         It takes the same argument of :func:`group` plus:
 
         ``section``: ``Optional[Section]``
             if provided, put the subcommand in this section.
 
@@ -434,15 +451,15 @@
 def command(
     name: Optional[str] = None, *,
     aliases: Optional[Iterable[str]] = None,
     cls: Optional[Type[ClickCommand]] = None,
     **kwargs: Any
 ) -> Callable[[AnyCallable], Union[Command, ClickCommand]]:
     """
-    Returns a decorator that creates a new command using the decorated function
+    Return a decorator that creates a new command using the decorated function
     as callback.
 
     The only differences with respect to ``click.command`` are:
 
     - the default command class is :class:`cloup.Command`
     - supports constraints, provided that ``cls`` inherits from ``ConstraintMixin``
       like ``cloup.Command`` (the default)
@@ -593,15 +610,15 @@
     ...
 
 
 def group(
     name: Optional[str] = None, *, cls: Optional[Type[ClickGroup]] = None, **kwargs: Any
 ) -> Callable[[AnyCallable], click.Group]:
     """
-    Returns a decorator that instantiates a ``Group`` (or a subclass of it)
+    Return a decorator that instantiates a ``Group`` (or a subclass of it)
     using the decorated function as callback.
 
     .. versionchanged:: 0.10.0
         the ``cls`` argument can now be any ``click.Group`` (previously had to
         be a ``cloup.Group``) and the type of the instantiated command matches
         it (previously, the type was ``cloup.Group`` even if ``cls`` was a subclass
         of it).
@@ -694,15 +711,15 @@
     ]
 }
 
 
 def _process_unexpected_kwarg_error(
     error: TypeError, args_info: Dict[str, _ArgInfo], cls: Type[Command]
 ) -> TypeError:
-    """Checks if the developer tried to pass a Cloup-specific argument to a ``cls``
+    """Check if the developer tried to pass a Cloup-specific argument to a ``cls``
     that doesn't support it and if that's the case, augments the error message
     to provide useful more info about the error."""
     import re
 
     message = str(error)
     match = re.search('|'.join(arg_name for arg_name in args_info), message)
     if match is None:
```

### Comparing `cloup-2.0.0.post1/cloup/_context.py` & `cloup-2.1.0/cloup/_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
     def make_formatter(self) -> HelpFormatter:
         opts = self.get_formatter_settings()
         return self.formatter_class(**opts)
 
     @staticmethod
     def settings(
-        *, auto_envvar_prefix: Possibly[bool] = MISSING,
+        *, auto_envvar_prefix: Possibly[str] = MISSING,
         default_map: Possibly[Dict[str, Any]] = MISSING,
         terminal_width: Possibly[int] = MISSING,
         max_content_width: Possibly[int] = MISSING,
         resilient_parsing: Possibly[bool] = MISSING,
         allow_extra_args: Possibly[bool] = MISSING,
         allow_interspersed_args: Possibly[bool] = MISSING,
         ignore_unknown_options: Possibly[bool] = MISSING,
```

### Comparing `cloup-2.0.0.post1/cloup/_option_groups.py` & `cloup-2.1.0/cloup/_option_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 def get_option_group_of(param: click.Option) -> Optional[OptionGroup]:
     return getattr(param, 'group', None)
 
 
 # noinspection PyMethodMayBeStatic
 class OptionGroupMixin:
-    """Implements support to:
+    """Implements support for:
 
      - option groups
      - the "Positional arguments" help section; this section is shown only if
        at least one of your arguments has non-empty ``help``.
 
     .. important::
         In order to check the constraints defined on the option groups,
@@ -170,15 +170,15 @@
         option_groups = list(options_by_group.keys())
         for group, options in options_by_group.items():
             group.options = options
 
         return arguments, option_groups, ungrouped_options
 
     def get_ungrouped_options(self, ctx: click.Context) -> Sequence[click.Option]:
-        """Returns options not explicitly assigned to an option group
+        """Return options not explicitly assigned to an option group
         (eventually including the ``--help`` option), i.e. options that will be
         part of the "default option group"."""
         help_option = ctx.command.get_help_option(ctx)
         if help_option is not None:
             return self.ungrouped_options + [help_option]
         else:
             return self.ungrouped_options
@@ -194,21 +194,21 @@
         args_with_help = (arg for arg in self.arguments if getattr(arg, "help", None))
         if not any(args_with_help):
             return None
         return HelpSection(
             heading="Positional arguments",
             definitions=[
                 self.get_argument_help_record(arg, ctx) for arg in self.arguments
-            ]
+            ],
         )
 
     def make_option_group_help_section(
         self, group: OptionGroup, ctx: click.Context
     ) -> HelpSection:
-        """Returns a HelpSection for an OptionGroup, i.e. an object containing
+        """Return a ``HelpSection`` for an ``OptionGroup``, i.e. an object containing
         the title, the optional description and the options' definitions for
         this option group.
 
         .. versionadded:: 0.8.0
         """
         return HelpSection(
             heading=group.title,
@@ -217,30 +217,30 @@
             constraint=group.constraint.help(ctx) if group.constraint else None
         )
 
     def must_align_option_groups(
         self, ctx: Optional[click.Context], default: bool = True
     ) -> bool:
         """
-        Returns ``True`` if the help sections of all options groups should have
+        Return ``True`` if the help sections of all options groups should have
         their columns aligned.
 
         .. versionadded:: 0.8.0
         """
         return first_bool(
             self.align_option_groups,
             getattr(ctx, 'align_option_groups', None),
             default,
         )
 
     def get_default_option_group(
         self, ctx: click.Context, is_the_only_visible_option_group: bool = False
     ) -> OptionGroup:
         """
-        Returns an ``OptionGroup`` instance for the options not explicitly
+        Return an ``OptionGroup`` instance for the options not explicitly
         assigned to an option group, eventually including the ``--help`` option.
 
         .. versionadded:: 0.8.0
         """
         default_group = OptionGroup(
             "Options" if is_the_only_visible_option_group else "Other options")
         default_group.options = self.get_ungrouped_options(ctx)
@@ -300,15 +300,15 @@
 ) -> Callable[[F], F]:
     ...
 
 
 # noinspection PyIncorrectDocstring
 def option_group(title: str, *args: Any, **kwargs: Any) -> Callable[[F], F]:
     """
-    Returns a decorator that annotates a function with an option group.
+    Return a decorator that annotates a function with an option group.
 
     The ``help`` argument is an optional description and can be provided either
     as keyword argument or as 2nd positional argument after the ``name`` of
     the group::
 
         # help as keyword argument
         @option_group(name, *options, help=None, ...)
```

### Comparing `cloup-2.0.0.post1/cloup/_params.py` & `cloup-2.1.0/cloup/_params.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 import click
 from click.decorators import _param_memo
 
 
 class Argument(click.Argument):
+    """A :class:`click.Argument` with help text."""
+
     def __init__(self, *args, help=None, **attrs):
         super().__init__(*args, **attrs)
         self.help = help
 
     def get_help_record(self, ctx):
         return self.make_metavar(), self.help or ""
 
 
 class Option(click.Option):
-    """A click.Option with an extra field ``group`` of type ``OptionGroup``."""
+    """A :class:`click.Option` with an extra field ``group`` of type ``OptionGroup``."""
 
     def __init__(self, *args, group=None, **attrs):
         super().__init__(*args, **attrs)
         self.group = group
 
 
 GroupedOption = Option
@@ -30,15 +32,15 @@
         _param_memo(f, ArgumentClass(param_decls, **attrs))
         return f
 
     return decorator
 
 
 def option(*param_decls, cls=None, group=None, **attrs):
-    """Attaches an ``Option`` to the command.
+    """Attach an ``Option`` to the command.
     Refer to :class:`click.Option` and :class:`click.Parameter` for more info
     about the accepted parameters.
 
     In your IDE, you won't see arguments relating to shell completion,
     because they are different in Click 7 and 8 (both supported by Cloup):
 
     - in Click 7, it's ``autocompletion``
```

### Comparing `cloup-2.0.0.post1/cloup/_params.pyi` & `cloup-2.1.0/cloup/_params.pyi`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/cloup/_sections.py` & `cloup-2.1.0/cloup/_sections.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,16 @@
 
     def __repr__(self) -> str:
         return 'Section({}, is_sorted={})'.format(self.title, self.is_sorted)
 
 
 class SectionMixin:
     """
-    Adds to a click.MultiCommand the possibility to organize its subcommands
-    in multiple help sections.
+    Adds to a :class:`click.MultiCommand` the possibility of organizing its subcommands
+    into multiple help sections.
 
     Sections can be specified in the following ways:
 
     #. passing a list of :class:`Section` objects to the constructor setting
        the argument ``sections``
     #. using :meth:`add_section` to add a single section
     #. using :meth:`add_command` with the argument `section` set
@@ -131,49 +131,49 @@
             self.add_section(section)
 
     def _add_command_to_section(
         self, cmd: click.Command,
         name: Optional[str] = None,
         section: Optional[Section] = None
     ) -> None:
-        """Adds a command to the section (if specified) or to the default section."""
+        """Add a command to the section (if specified) or to the default section."""
         name = name or cmd.name
         if section is None:
             section = self._default_section
         section.add_command(cmd, name)
         if section not in self._section_set:
             self._user_sections.append(section)
             self._section_set.add(section)
 
     def add_section(self, section: Section) -> None:
-        """ Adds a :class:`Section` to this group. You can add the same
-        section object a single time. """
+        """Add a :class:`Section` to this group. You can add the same
+        section object a single time."""
         if section in self._section_set:
             raise ValueError(f'section "{section}" was already added')
         self._user_sections.append(section)
         self._section_set.add(section)
         for name, cmd in section.commands.items():
             # It's important to call self.add_command() and not super().add_command() here
             # otherwise subclasses' add_command() is not called.
             self.add_command(cmd, name, fallback_to_default_section=False)
 
     def section(self, title: str, *commands: click.Command, **attrs: Any) -> Section:
-        """ Creates a new :class:`Section`, adds it to this group and returns it."""
+        """Create a new :class:`Section`, adds it to this group and returns it."""
         section = Section(title, commands, **attrs)
         self.add_section(section)
         return section
 
     def add_command(
         self, cmd: click.Command,
         name: Optional[str] = None,
         section: Optional[Section] = None,
         fallback_to_default_section: bool = True,
     ) -> None:
         """
-        Adds a subcommand to this ``Group``.
+        Add a subcommand to this ``Group``.
 
         **Implementation note:** ``fallback_to_default_section`` looks not very
         clean but, even if it's not immediate to see (it wasn't for me), I chose
         it over apparently cleaner options.
 
         :param cmd:
         :param name:
@@ -189,17 +189,20 @@
         super().add_command(cmd, name)  # type: ignore
         if section or fallback_to_default_section:
             self._add_command_to_section(cmd, name, section)
 
     def list_sections(
         self, ctx: click.Context, include_default_section: bool = True
     ) -> List[Section]:
-        """ Returns the list of all sections in the "correct order".
-         if ``include_default_section=True`` and the default section is non-empty,
-         it will be included at the end of the list. """
+        """
+        Return the list of all sections in the "correct order".
+
+        If ``include_default_section=True`` and the default section is non-empty,
+        it will be included at the end of the list.
+        """
         section_list = list(self._user_sections)
         if include_default_section and len(self._default_section) > 0:
             default_section = Section.sorted(
                 title='Other commands' if len(self._user_sections) > 0 else 'Commands',
                 commands=self._default_section.commands)
             section_list.append(default_section)
         return section_list
```

### Comparing `cloup-2.0.0.post1/cloup/_util.py` & `cloup-2.1.0/cloup/_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,21 @@
         return zero
     if count == 1 and one:
         return one
     return many.format(count=count)
 
 
 def coalesce(*values: Optional[T]) -> Optional[T]:
-    """Returns the first value that is not None (or None if no such value exists)."""
+    """Return the first value that is not ``None``
+    (or ``None`` if no such value exists)."""
     return next((val for val in values if val is not None), None)
 
 
 def first_bool(*values: Any) -> bool:
-    """Returns the first bool (or raises StopIteration if no bool is found)."""
+    """Return the first bool (or raises ``StopIteration`` if no bool is found)."""
     return next(val for val in values if isinstance(val, bool))
 
 
 def pick_not_none(iterable: Iterable[Optional[T]]) -> List[T]:
     return [x for x in iterable if x is not None]
```

### Comparing `cloup-2.0.0.post1/cloup/constraints/__init__.py` & `cloup-2.1.0/cloup/constraints/__init__.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/cloup/constraints/_conditional.py` & `cloup-2.1.0/cloup/constraints/_conditional.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This modules contains classes to create conditional constraints.
+This modules contains classes for creating conditional constraints.
 """
 from typing import Optional, Sequence, Union
 
 from click import Context, Parameter
 
 from ._core import Constraint
 from .conditions import AllSet, IsSet, Predicate
@@ -15,51 +15,53 @@
     if isinstance(arg, str):
         return IsSet(arg)
     elif isinstance(arg, Predicate):
         return arg
     elif isinstance(arg, Sequence):
         return AllSet(*arg)
     else:
-        raise TypeError('`arg` should be a string, a list of strings or a `Predicate`')
+        raise TypeError("`arg` should be a string, a list of strings or a `Predicate`")
 
 
 class If(Constraint):
+    """
+    Checks one constraint or another depending on the truth value of the condition.
+
+    .. versionadded:: 0.8.0
+        you can now pass a sequence of parameter names as condition, which
+        corresponds to the predicate ``AllSet(*param_names)``.
+
+    :param condition:
+        can be either an instance of ``Predicate`` or (more often) the name of a
+        parameter or a list/tuple of parameters that must be all set for the
+        condition to be true.
+    :param then:
+        a constraint checked if the condition is true.
+    :param else_:
+        an (optional) constraint checked if the condition is false.
+    """
+
     def __init__(
-        self, condition: Union[str, Sequence[str], Predicate],
+        self,
+        condition: Union[str, Sequence[str], Predicate],
         then: Constraint,
-        else_: Optional[Constraint] = None
+        else_: Optional[Constraint] = None,
     ):
-        """
-        Checks one constraint or another depending on the truth value of the condition.
-
-        .. versionadded:: 0.8.0
-            you can now pass a sequence of parameter names as condition, which
-            corresponds to the predicate ``AllSet(*param_names)``.
-
-        :param condition:
-            can be either an instance of ``Predicate`` or (more often) the name of a
-            parameter or a list/tuple of parameters that must be all set for the
-            condition to be true.
-        :param then:
-            a constraint checked if the condition is true.
-        :param else_:
-            an (optional) constraint checked if the condition is false.
-        """
         self._condition = as_predicate(condition)
         self._then = then
         self._else = else_
 
     def help(self, ctx: Context) -> str:
         condition = self._condition.description(ctx)
         then_help = self._then.help(ctx)
         else_help = self._else.help(ctx) if self._else else None
         if not self._else:
-            return f'{then_help} if {condition}'
+            return f"{then_help} if {condition}"
         else:
-            return f'{then_help} if {condition}, otherwise {else_help}'
+            return f"{then_help} if {condition}, otherwise {else_help}"
 
     def check_consistency(self, params: Sequence[Parameter]) -> None:
         self._then.check_consistency(params)
         if self._else:
             self._else.check_consistency(params)
 
     def check_values(self, params: Sequence[Parameter], ctx: Context) -> None:
@@ -67,16 +69,20 @@
         condition_is_true = condition(ctx)
         branch = self._then if condition_is_true else self._else
         if branch is None:
             return
         try:
             branch.check_values(params, ctx=ctx)
         except ConstraintViolated as err:
-            desc = (condition.description(ctx) if condition_is_true
-                    else condition.negated_description(ctx))
+            desc = (
+                condition.description(ctx)
+                if condition_is_true
+                else condition.negated_description(ctx)
+            )
             raise ConstraintViolated(
-                f"when {desc}, {err}", ctx=ctx, constraint=self, params=params)
+                f"when {desc}, {err}", ctx=ctx, constraint=self, params=params
+            )
 
     def __repr__(self) -> str:
         if self._else:
             return make_repr(self, self._condition, then=self._then, else_=self._else)
         return make_repr(self, self._condition, then=self._then)
```

### Comparing `cloup-2.0.0.post1/cloup/constraints/_core.py` & `cloup-2.1.0/cloup/constraints/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         calling a constraint, previously equivalent to :meth:`~Constraint.check`,
         is now equivalent to calling :func:`cloup.constrained_params` with this
         constraint as first argument.
     """
 
     @staticmethod
     def must_check_consistency(ctx: click.Context) -> bool:
-        """Returns True if consistency checks are enabled.
+        """Return ``True`` if consistency checks are enabled.
 
         .. versionchanged:: 0.9.0
             this method now a static method and takes a ``click.Context`` in input.
         """
         return first_bool(
             getattr(ctx, 'check_constraints_consistency', True),
             True,
@@ -61,15 +61,15 @@
 
     @abc.abstractmethod
     def help(self, ctx: click.Context) -> str:
         """A description of the constraint. """
 
     def check_consistency(self, params: Sequence[click.Parameter]) -> None:
         """
-        Performs some sanity checks that detect inconsistencies between these
+        Perform some sanity checks that detect inconsistencies between these
         constraints and the properties of the input parameters (e.g. required).
 
         For example, a constraint that requires the parameters to be mutually
         exclusive is not consistent with a group of parameters with multiple
         required options.
 
         These sanity checks are meant to catch developer's mistakes and don't
@@ -84,15 +84,15 @@
                  if the constraint cannot be satisfied independently from the values
                  provided by the user
         """
 
     @abc.abstractmethod
     def check_values(self, params: Sequence[click.Parameter], ctx: click.Context) -> None:
         """
-        Checks that the constraint is satisfied by the input parameters in the
+        Check that the constraint is satisfied by the input parameters in the
         given context, which (among other things) contains the values assigned
         to the parameters in ``ctx.params``.
 
         You probably don't want to call this method directly.
         Use :meth:`check` instead.
 
         :param params: list of :class:`click.Parameter` instances
@@ -112,15 +112,15 @@
         ...
 
     def check(
         self, params: Union[Sequence[click.Parameter], Sequence[str]],
         ctx: Optional[click.Context] = None
     ) -> None:
         """
-        Raises an exception if the constraint is not satisfied by the input
+        Raise an exception if the constraint is not satisfied by the input
         parameters in the given (or current) context.
 
         This method calls both :meth:`check_consistency` (if enabled) and
         :meth:`check_values`.
 
         .. tip::
             By default :meth:`check_consistency` is called since it shouldn't
@@ -158,15 +158,15 @@
 
     def rephrased(
         self,
         help: Union[None, str, HelpRephraser] = None,
         error: Union[None, str, ErrorRephraser] = None,
     ) -> 'Rephraser':
         """
-        Overrides the help string and/or the error message of this constraint
+        Override the help string and/or the error message of this constraint
         wrapping it with a :class:`Rephraser`.
 
         :param help:
             if provided, overrides the help string of this constraint. It can be
             a string or a function ``(ctx: click.Context, constr: Constraint) -> str``.
             If you want to hide this constraint from the help, pass ``help=""``.
         :param error:
@@ -180,15 +180,15 @@
               a :class:`ConstraintViolated` error has fields for ``ctx``,
               ``constraint`` and ``params``, so it's a complete description
               of what happened.
         """
         return Rephraser(self, help=help, error=error)
 
     def hidden(self) -> 'Rephraser':
-        """Hides this constraint from the command help."""
+        """Hide this constraint from the command help."""
         return Rephraser(self, help='')
 
     def __call__(self, *param_adders: Decorator) -> Callable[[F], F]:
         """Equivalent to calling :func:`cloup.constrained_params` with this
         constraint as first argument.
 
         .. versionchanged:: 0.9.0
@@ -297,15 +297,15 @@
     append or prepend some extra info to the original error message."""
 
     param_list = '{param_list}'
     """Replaced by a 2-space indented list of the constrained parameters."""
 
 
 class Rephraser(Constraint):
-    """A Constraint decorator that can override the help and/or the error
+    """A constraint decorator that can override the help and/or the error
     message of the wrapped constraint.
 
     You'll rarely (if ever) use this class directly. In most cases, you'll use
     the method :meth:`Constraint.rephrased`. Refer to it for more info.
 
     .. seealso::
 
@@ -317,15 +317,15 @@
 
     def __init__(
         self, constraint: Constraint,
         help: Union[None, str, HelpRephraser] = None,
         error: Union[None, str, ErrorRephraser] = None,
     ):
         if help is None and error is None:
-            raise ValueError('at least one between [help] and [error] must not be None')
+            raise ValueError('`help` and `error` cannot both be `None`')
         self.constraint = constraint
         self._help = help
         self._error = error
 
     def help(self, ctx: click.Context) -> str:
         if self._help is None:
             return self.constraint.help(ctx)
```

### Comparing `cloup-2.0.0.post1/cloup/constraints/_support.py` & `cloup-2.1.0/cloup/constraints/_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ) -> None:
     if not hasattr(f, '__cloup_constraints__'):
         f.__cloup_constraints__ = []
     f.__cloup_constraints__.append(constr)
 
 
 def constraint(constr: Constraint, params: Iterable[str]) -> Callable[[F], F]:
-    """Registers a constraint on a list of parameters specified by (destination) name
+    """Register a constraint on a list of parameters specified by (destination) name
     (e.g. the default name of ``--input-file`` is ``input_file``)."""
     spec = BoundConstraintSpec(constr, tuple(params))
 
     def decorator(f: F) -> F:
         _constraint_memo(f, spec)
         return f
 
@@ -48,15 +48,15 @@
 
 
 def constrained_params(
     constr: Constraint,
     *param_adders: Decorator,
 ) -> Callable[[F], F]:
     """
-    Returns a decorator that adds the given parameters and applies a constraint
+    Return a decorator that adds the given parameters and applies a constraint
     to them. Equivalent to::
 
         @param_adders[0]
         ...
         @param_adders[-1]
         @constraint(constr, <param names>)
 
@@ -115,15 +115,15 @@
         if not constr_help:
             return None
         param_list = '{%s}' % join_param_labels(self.params)
         return param_list, constr_help
 
 
 class ConstraintMixin:
-    """Provides support to constraints."""
+    """Provides support for constraints."""
 
     def __init__(
         self, *args: Any,
         constraints: Sequence[Union[BoundConstraintSpec, BoundConstraint]] = (),
         show_constraints: Optional[bool] = None,
         **kwargs: Any,
     ):
```

### Comparing `cloup-2.0.0.post1/cloup/constraints/common.py` & `cloup-2.1.0/cloup/constraints/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from typing import Any, Dict, Iterable, List, Sequence
 
 from click import Argument, Context, Option, Parameter
 
 
 def param_value_is_set(param: Parameter, value: Any) -> bool:
-    """Defines what it means for a parameter of a specific kind to be "set".
+    """Define what it means for a parameter of a specific kind to be "set".
 
     All cases are obvious besides that of boolean options:
     - (common rule) if the value is ``None``, the parameter is unset;
     - a parameter that takes multiple values is set if at least one argument is provided;
     - a boolean **flag** is set only if True;
     - a boolean option is set if not None, even if it's False.
     """
@@ -23,15 +23,15 @@
         return bool(value)
     elif param.nargs != 1 or param.multiple:
         return len(value) > 0
     return True
 
 
 def get_param_name(param: Parameter) -> str:
-    """Returns the name of a parameter casted to ``str``.
+    """Return the name of a parameter casted to ``str``.
     Use this function to avoid typing errors in places where you expect a parameter
     having a name.
     """
     if param.name is None:
         raise TypeError(
             '`param.name` is required to be a string in this context.\n'
             'Hint: `param.name` is None only when `parameter.expose_value` is False, '
@@ -39,15 +39,15 @@
         )
     return param.name
 
 
 def get_params_whose_value_is_set(
     params: Iterable[Parameter], values: Dict[str, Any]
 ) -> List[Parameter]:
-    """Filters ``params`` returning only the parameters that have a value.
+    """Filter ``params``, returning only the parameters that have a value.
     Boolean flags are considered "set" if their value is ``True``."""
     return [p for p in params
             if param_value_is_set(p, values[get_param_name(p)])]
 
 
 def get_required_params(params: Iterable[Parameter]) -> List[Parameter]:
     return [p for p in params if p.required]
```

### Comparing `cloup-2.0.0.post1/cloup/constraints/conditions.py` & `cloup-2.1.0/cloup/constraints/conditions.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/cloup/constraints/exceptions.py` & `cloup-2.1.0/cloup/constraints/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         return ConstraintViolated(
             default_constraint_error(params, desc),
             ctx=ctx, constraint=constraint, params=params,
         )
 
 
 class UnsatisfiableConstraint(Exception):
-    """ Raised if a constraint cannot be satisfied by a group of parameters
-    independently from their values at runtime; e.g. mutually_exclusive cannot
-    be satisfied if multiple of the parameters are required. """
+    """Raised if a constraint cannot be satisfied by a group of parameters
+    independently from their values at runtime; e.g. ``mutually_exclusive`` cannot
+    be satisfied if multiple of the parameters are required."""
 
     def __init__(
         self, constraint: 'Constraint', params: Iterable[Parameter], reason: str
     ):
         self.constraint = constraint
         self.params = params
         self.reason = reason
```

### Comparing `cloup-2.0.0.post1/cloup/formatting/_formatter.py` & `cloup-2.1.0/cloup/formatting/_formatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,15 +181,17 @@
         self.write(f" {alias_list}\n")
 
     def write_command_help_text(self, cmd: click.Command) -> None:
         help_text = cmd.help or ""
         if help_text and click_version_ge_8_1:
             help_text = inspect.cleandoc(help_text)
         if cmd.deprecated:
-            help_text = "(DEPRECATED) " + help_text
+            # Use the same label as Click:
+            # https://github.com/pallets/click/blob/b0538df/src/click/core.py#L1331
+            help_text = "(Deprecated) " + help_text
         if help_text:
             self.write_paragraph()
             with self.indentation():
                 self.write_text(help_text, style=self.theme.command_help)
 
     def write_heading(self, heading: str, newline: bool = True) -> None:
         if self.current_indent:
@@ -204,15 +206,15 @@
     ) -> None:
         if aligned:
             return self.write_aligned_sections(sections)
         for s in sections:
             self.write_section(s)
 
     def write_aligned_sections(self, sections: Sequence[HelpSection]) -> None:
-        """Writes multiple aligned definition lists."""
+        """Write multiple aligned definition lists."""
         all_rows = chain.from_iterable(dl.definitions for dl in sections)
         col1_width = self.compute_col1_width(all_rows, self.col1_max_width)
         for s in sections:
             self.write_section(s, col1_width=col1_width)
 
     def write_section(self, s: HelpSection, col1_width: Optional[int] = None) -> None:
         theme = self.theme
@@ -251,15 +253,15 @@
 
     def write_dl(
         self, rows: Sequence[Definition],
         col_max: Optional[int] = None,  # default changed to None wrt parent class
         col_spacing: Optional[int] = None,  # default changed to None wrt parent class
         col1_width: Optional[int] = None,
     ) -> None:
-        """Writes a definition list into the buffer. This is how options
+        """Write a definition list into the buffer. This is how options
         and commands are usually formatted.
 
         If there's enough space, definition lists are rendered as a 2-column
         pseudo-table: if the first column text of a row doesn't fit in the
         provided/computed ``col1_width``, the 2nd column is printed on the
         following line.
 
@@ -318,15 +320,15 @@
         else:
             raise TypeError('row_sep')
 
     def write_tabular_dl(
         self, rows: Sequence[Definition],
         col1_width: int, col_spacing: int, col2_width: int,
     ) -> None:
-        """Formats a definition list as a 2-column "pseudo-table". If the first
+        """Format a definition list as a 2-column "pseudo-table". If the first
         column of a row exceeds ``col1_width``, the 2nd column is written on
         the subsequent line. This is the standard way of formatting definition
         lists and it's the default if there's enough space."""
 
         col1_plus_spacing = col1_width + col_spacing
         col2_indentation = " " * (
             self.current_indent + max(self.indent_increment, col1_plus_spacing)
@@ -363,15 +365,15 @@
         write_row(text_rows[0])
         for row in text_rows[1:]:
             if row_sep is not None:
                 self.write(indentation, row_sep, "\n")
             write_row(row)
 
     def write_linear_dl(self, dl: Sequence[Definition]) -> None:
-        """Formats a definition list as a "linear list". This is the default when
+        """Format a definition list as a "linear list". This is the default when
         the available width for the definitions (2nd column) is below
         ``self.col2_min_width``."""
         help_extra_indent = max(3, self.indent_increment)
         help_total_indent = self.current_indent + help_extra_indent
         help_max_width = self.width - help_total_indent
         current_indentation = " " * self.current_indent
```

### Comparing `cloup-2.0.0.post1/cloup/formatting/_util.py` & `cloup-2.1.0/cloup/formatting/_util.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import click
 
 if TYPE_CHECKING:
     import cloup
 
 FORMATTER_TYPE_ERROR = """
-since cloup v0.8.0, this class relies on cloup.HelpFormatter to align help
-sections. So, you need to make sure your command class uses cloup.HelpFormatter
+since Cloup v0.8, this class relies on `cloup.HelpFormatter` to align help
+sections. So, you need to make sure your command class uses `cloup.HelpFormatter`
 as formatter class.
 
-If you have your own custom HelpFormatter, know that cloup.HelpFormatter is
+If you have your own custom `HelpFormatter`, know that `cloup.HelpFormatter` is
 more easily customizable then Click's one, so consider extending it instead
-of extending click.HelpFormatter.
+of extending `click.HelpFormatter`.
 """
 
 
 def ensure_is_cloup_formatter(formatter: click.HelpFormatter) -> 'cloup.HelpFormatter':
     from cloup import HelpFormatter
     if isinstance(formatter, HelpFormatter):
         return formatter
```

### Comparing `cloup-2.0.0.post1/cloup/formatting/sep.py` & `cloup-2.1.0/cloup/formatting/sep.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 else:  # pragma: no cover
     from typing_extensions import Protocol
 
 SepType = Union[str, 'SepGenerator']
 
 
 class SepGenerator(Protocol):
-    """Generates a separator given a width. When used as ``row_sep``, this ``width`
+    """Generate a separator given a width. When used as ``row_sep``, this ``width``
     corresponds to ``HelpFormatter.available_width``, i.e. the line width excluding
     the current indentation width.
 
     Note: the length of the returned separator may differ from ``width``.
     """
 
     def __call__(self, width: int) -> str:
@@ -50,55 +50,56 @@
 
     @abc.abstractmethod
     def __call__(  # noqa E704
         self, rows: Sequence[Sequence[str]],
         col_widths: Sequence[int],
         col_spacing: int,
     ) -> Optional[str]:
-        """Decides which row separator to use (eventually none) in the given
+        """Decide which row separator to use (eventually none) in the given
         definition list."""
 
 
 class RowSepCondition(Protocol):
     """Determines when a definition list should use a row separator."""
 
     # Ignore error due to flake8 issue: "multiple statements on one line (def)"
     def __call__(  # noqa E704
         self, rows: Sequence[Sequence[str]],
         col_widths: Sequence[int],
         col_spacing: int,
     ) -> bool:
-        """Returns ``True`` if the input definition list should use a row
+        """Return ``True`` if the input definition list should use a row
         separator (in addition to the usual ``\\n``)."""
 
 
 class RowSepIf(RowSepPolicy):
+    """
+    Inserts a row separator between the rows of a definition list only if a
+    condition is satisfied. This class implements the ``RowSepPolicy``
+    protocol and does two things:
+
+    - enforces the use of a single row separator for all rows of a
+        definition lists and for all definition lists; note that
+        ``RowSepPolicy`` doesn't for implementation reasons but it's probably
+        what you want;
+    - allows you to implement different conditions (see type
+        :data:`RowSepCondition`) without worrying about the generation part,
+        which is always the same.
+
+    :param condition:
+        a :class:`RowSepCondition` that determines when to add the (extra)
+        row separator.
+    :param sep:
+        either a string or a ``SepGenerator``,
+        i.e. a function ``(width: int) -> str`` (e.g. :class:`Hline`).
+        The empty string corresponds to an empty line separator.
+    """
+
     def __init__(self, condition: RowSepCondition,
                  sep: Union[str, SepGenerator] = ''):
-        """
-        Inserts a row separator between the rows of a definition list only if a
-        condition is satisfied. This class implements the ``RowSepPolicy``
-        protocol and does two things:
-
-        - enforces the use of a single row separator for all rows of a
-          definition lists and for all definition lists; note that
-          ``RowSepPolicy`` doesn't for implementation reasons but it's probably
-          what you want;
-        - allows you to implement different conditions (see type
-          :data:`RowSepCondition`) without worrying about the generation part,
-          which is always the same.
-
-        :param condition:
-            a :class:`RowSepCondition` that determines when to add the (extra)
-            row separator.
-        :param sep:
-            either a string or a ``SepGenerator``,
-            i.e. a function ``(width: int) -> str`` (e.g. :class:`Hline`).
-            The empty string corresponds to an empty line separator.
-        """
         if isinstance(sep, str) and sep.endswith('\n'):
             raise ValueError(
                 "sep must not end with '\\n'. The formatter writes  a '\\n' after it; "
                 "no other newline is allowed.")
         self.condition = condition
         self.sep = sep
 
@@ -113,15 +114,15 @@
         return None
 
 
 # ==========================================
 #  Conditions & related utils
 
 def get_total_width(col_widths: Sequence[int], col_spacing: int) -> int:
-    """Returns the total width of a definition list (or, more generally, a table).
+    """Return the total width of a definition list (or, more generally, a table).
     Useful when implementing a RowSepStrategy."""
     return sum(col_widths) + col_spacing * (len(col_widths) - 1)
 
 
 def count_multiline_rows(rows: Sequence[Sequence[str]], col_widths: Sequence[int]) -> int:
     # Note: I'm using zip_longest on purpose so that a TypeError will be raised
     # if len(row) != len(col_widths). An explicit check is not worth it since
@@ -133,15 +134,15 @@
     )
 
 
 def multiline_rows_are_at_least(
     count_or_percentage: Union[int, float]
 ) -> RowSepCondition:
     """
-    Returns a ``RowSepStrategy`` that returns a row separator between all rows
+    Return a ``RowSepStrategy`` that returns a row separator between all rows
     of a definition list, only if the number of rows taking multiple lines is
     greater than or equal to a certain threshold.
 
     :param count_or_percentage:
         a threshold for multiline rows above which the returned strategy will
         insert a row separator. It can be either an absolute count (`int`) or a
         percentage relative to the total number of rows expressed as a `float`
@@ -179,45 +180,46 @@
     else:
         raise TypeError('count_or_percentage must be an int or a float')
 
     return condition
 
 
 class Hline(SepGenerator):
+    """Returns a function that generates an horizontal line of a given length.
+
+    This class has different static members for different line styles
+    like ``Hline.solid``, ``Hline.dashed``, ``Hline.densely_dashed``
+    and  ``Hline.dotted``.
+
+    :param pattern:
+        a string (usually a single character) that is repeated to generate
+        the line.
+    """
+
     # Workaround: PyCharm auto-completion doesn't work without these declarations
     solid: 'Hline'
     dashed: 'Hline'
     densely_dashed: 'Hline'
     dotted: 'Hline'
 
     def __init__(self, pattern: str):
-        """Returns a function that generates an horizontal line of a given length.
-
-        This class has different static members for different line styles
-        like ``Hline.solid``, ``Hline.dashed``, ``Hline.densely_dashed``
-        and  ``Hline.dotted``.
-
-        :param pattern:
-            a string (usually a single character) that is repeated to generate
-            the line.
-        """
         self.pattern = pattern
 
     def __call__(self, width: int) -> str:
         pattern = self.pattern
         if len(pattern) == 1:
             return pattern * width
         reps, rest = width // len(pattern), width % len(pattern)
         return pattern * reps + pattern[:rest]
 
 
 Hline.solid = Hline("─")
-"""Returns a line like ``────────``."""
+"""Return a line like ``────────``."""
 
 Hline.dashed = Hline('-')
-"""Returns a line like ``--------``."""
+"""Return a line like ``--------``."""
 
 Hline.densely_dashed = Hline('╌')
-"""Returns a line like ``╌╌╌╌╌╌╌╌``."""
+"""Return a line like ``╌╌╌╌╌╌╌╌``."""
 
 Hline.dotted = Hline("┄")
-"""Returns a line like ``┄┄┄┄┄┄┄┄``."""
+"""Return a line like ``┄┄┄┄┄┄┄┄``."""
```

### Comparing `cloup-2.0.0.post1/cloup/styling.py` & `cloup-2.1.0/cloup/styling.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 """
 import dataclasses as dc
 from typing import Any, Callable, Dict, NamedTuple, Optional
 
 import click
 
 from cloup._util import FrozenSpace, click_version_tuple, delete_keys, identity
+from cloup.typing import MISSING, Possibly
 
 IStyle = Callable[[str], str]
 """A callable that takes a string and returns a styled version of it."""
 
 
 # noinspection PyUnresolvedReferences
 class HelpTheme(NamedTuple):
@@ -35,14 +36,19 @@
         Style of the help text of a section (the optional paragraph below the heading).
     :param col1:
         Style of the first column of a definition list (options and command names).
     :param col2:
         Style of the second column of a definition list (help text).
     :param epilog:
         Style of the epilog.
+    :param alias:
+        Style of subcommand aliases in a definition lists.
+    :param alias_secondary:
+        Style of separator and eventual parenthesis/brackets in subcommand alias lists.
+        If not provided, the ``alias`` style will be used.
     """
 
     invoked_command: IStyle = identity
     """Style of the invoked command name (in Usage)."""
 
     command_help: IStyle = identity
     """Style of the invoked command description (below Usage)."""
@@ -58,41 +64,54 @@
 
     col1: IStyle = identity
     """Style of the first column of a definition list (options and command names)."""
 
     col2: IStyle = identity
     """Style of the second column of a definition list (help text)."""
 
+    alias: IStyle = identity
+    """Style of subcommand aliases in a definition lists."""
+
+    alias_secondary: Optional[IStyle] = None
+    """Style of separator and eventual parenthesis/brackets in subcommand alias lists.
+    If not provided, the ``alias`` style will be used."""
+
     epilog: IStyle = identity
     """Style of the epilog."""
 
     def with_(
         self, invoked_command: Optional[IStyle] = None,
         command_help: Optional[IStyle] = None,
         heading: Optional[IStyle] = None,
         constraint: Optional[IStyle] = None,
         section_help: Optional[IStyle] = None,
         col1: Optional[IStyle] = None,
         col2: Optional[IStyle] = None,
+        alias: Optional[IStyle] = None,
+        alias_secondary: Possibly[Optional[IStyle]] = MISSING,
         epilog: Optional[IStyle] = None,
     ) -> 'HelpTheme':
         kwargs = {key: val for key, val in locals().items() if val is not None}
+        if alias_secondary is MISSING:
+            del kwargs["alias_secondary"]
         kwargs.pop('self')
         if kwargs:
             return self._replace(**kwargs)
         return self
 
     @staticmethod
     def dark() -> "HelpTheme":
         """A theme assuming a dark terminal background color."""
         return HelpTheme(
             invoked_command=Style(fg='bright_yellow'),
             heading=Style(fg='bright_white', bold=True),
             constraint=Style(fg='magenta'),
             col1=Style(fg='bright_yellow'),
+            alias=Style(fg='yellow'),
+            alias_secondary=Style(fg='white'),
         )
 
     @staticmethod
     def light() -> "HelpTheme":
         """A theme assuming a light terminal background color."""
         return HelpTheme(
             invoked_command=Style(fg='yellow'),
@@ -180,7 +199,10 @@
     bright_red = "bright_red"
     bright_green = "bright_green"
     bright_yellow = "bright_yellow"
     bright_blue = "bright_blue"
     bright_magenta = "bright_magenta"
     bright_cyan = "bright_cyan"
     bright_white = "bright_white"
+
+
+DEFAULT_THEME = HelpTheme()
```

### Comparing `cloup-2.0.0.post1/cloup/types.py` & `cloup-2.1.0/cloup/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Parameter types and "shortcuts" to create commonly used types.
+Parameter types and "shortcuts" for creating commonly used types.
 """
 import pathlib
 
 import click
 
 
 def path(
```

### Comparing `cloup-2.0.0.post1/cloup/typing.py` & `cloup-2.1.0/cloup/typing.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/cloup.egg-info/PKG-INFO` & `cloup-2.1.0/cloup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloup
-Version: 2.0.0.post1
+Version: 2.1.0
 Summary: Adds features to Click: option groups, constraints, subcommand sections and help themes.
 Home-page: https://github.com/janLuke/cloup
 Author: Gianluca Gippetto
 Author-email: gianluca.gippetto@gmail.com
 License: BSD 3-Clause
 Keywords: CLI,click,argument groups,option groups,constraints,help colors,help themes,help styles
 Classifier: Intended Audience :: Developers
@@ -28,15 +28,15 @@
 
 .. |tests-status| image:: https://github.com/janLuke/cloup/workflows/Tests/badge.svg
     :alt: Tests status
     :target: https://github.com/janLuke/cloup/actions?query=workflow%3ATests
 
 .. |coverage| image:: https://codecov.io/github/janLuke/cloup/coverage.svg?branch=master
     :alt: Coverage Status
-    :target: https://codecov.io/github/janLuke/cloup?branch=master
+    :target: https://app.codecov.io/github/janluke/cloup/tree/master
 
 .. |python-versions| image:: https://img.shields.io/pypi/pyversions/cloup.svg
     :alt: Supported versions
     :target: https://pypi.org/project/cloup
 
 .. |dev-docs| image:: https://readthedocs.org/projects/cloup/badge/?version=latest
     :alt: Documentation Status (master branch)
@@ -66,15 +66,15 @@
 - **option groups** and an (optional) help section for positional arguments
 
 - **constraints**, like ``mutually_exclusive``, that can be applied to option groups
   or to any group of parameters, even *conditionally*
 
 - **subcommand aliases**
 
-- **subcommands sections**, i.e. the possibility to organize the subcommands of a
+- **subcommands sections**, i.e. the possibility of organizing the subcommands of a
   ``Group`` in multiple help sections
 
 - a **themeable HelpFormatter**  that:
 
   - has more parameters for adjusting widths and spacing, which can be provided
     at the context and command level
   - use a different layout when the terminal width is below a certain threshold
@@ -82,16 +82,16 @@
 
 - suggestions like "did you mean <subcommand>?" when you mistype a subcommand.
 
 Moreover, Cloup improves on **IDE support** providing decorators with *detailed*
 type hints and adding the static methods ``Context.settings()`` and
 ``HelpFormatter.settings()`` for creating dictionaries of settings.
 
-Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested** 
-against multiple versions of Python with nearly 100% coverage. 
+Cloup is **statically type-checked** with MyPy in strict mode and extensively **tested**
+against multiple versions of Python with nearly 100% coverage.
 
 
 A simple example
 ================
 
 .. code-block:: python
```

### Comparing `cloup-2.0.0.post1/cloup.egg-info/SOURCES.txt` & `cloup-2.1.0/cloup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/Makefile` & `cloup-2.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_autoapi_templates/python/module.rst` & `cloup-2.1.0/docs/_autoapi_templates/python/module.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/basic-example.png` & `cloup-2.1.0/docs/_static/basic-example.png`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/logo-dark-mode.svg` & `cloup-2.1.0/docs/_static/logo-dark-mode.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/logo-on-white.svg` & `cloup-2.1.0/docs/_static/logo-on-white.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/logo.svg` & `cloup-2.1.0/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/styles/extensions-overrides.css` & `cloup-2.1.0/docs/_static/styles/extensions-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/styles/theme-overrides.css` & `cloup-2.1.0/docs/_static/styles/theme-overrides.css`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/_static/theme-elems.png` & `cloup-2.1.0/docs/_static/theme-elems.png`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/conf.py` & `cloup-2.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/index.rst` & `cloup-2.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/make.bat` & `cloup-2.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/pages/aliases.rst` & `cloup-2.1.0/docs/pages/aliases.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/pages/arguments.rst` & `cloup-2.1.0/docs/pages/arguments.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/pages/constraints.rst` & `cloup-2.1.0/docs/pages/constraints.rst`

 * *Files 0% similar despite different names*

```diff
@@ -218,16 +218,16 @@
 
     @option_group(
         ...
         constraint=RequireAtLeast(1).hidden(),
     )
 
 
-The @constraint decorator
-~~~~~~~~~~~~~~~~~~~~~~~~~
+The ``@constraint`` decorator
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Using the :func:`cloup.constraint` decorator, you can apply a constraint to any
 group of parameters (arguments and options) providing their **destination names**,
 i.e. the names of the function arguments they are mapped to (by Click).
 For example:
 
 =============================================== ===================
 Declaration                                     Name
@@ -312,15 +312,15 @@
 
 .. admonition:: Syntax limitation in Python < 3.9
     :name: attention-python-decorators
     :class: attention
 
     In Python < 3.9, the expression on the right of the operator ``@``
     is required to be a "dotted name, optionally followed by a single call"
-    (see `PEP 614 <https://www.python.org/dev/peps/pep-0614/#motivation>`_).
+    (see `PEP 614 <https://peps.python.org/pep-0614/#motivation>`_).
     This means that you can't instantiate a parametric constraint on the right
     of ``@``, because the resultant expressions would make two calls, e.g.:
 
     .. code-block:: python
 
         # This is a syntax error in Python < 3.9
         @RequireExactly(2)(  # 1st call to instantiate the constraint
```

### Comparing `cloup-2.0.0.post1/docs/pages/formatting.rst` & `cloup-2.1.0/docs/pages/formatting.rst`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 An example
 ~~~~~~~~~~
 
 .. tip::
     In Cloup, you can use the static methods :meth:`Context.settings` and
     :meth:`HelpFormatter.settings` to create dictionaries without leaving your
-    IDE (to check the docs).
+    IDE to check the docs.
 
 .. code-block:: python
 
     from cloup import Context, command, group, HelpFormatter, HelpTheme
 
     CONTEXT_SETTINGS = Context.settings(
         # parameters of Command:
```

### Comparing `cloup-2.0.0.post1/docs/pages/installation.rst` & `cloup-2.1.0/docs/pages/installation.rst`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/docs/pages/option-groups.rst` & `cloup-2.1.0/docs/pages/option-groups.rst`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
             option("--six", help="3rd output option"),
             constraint=RequireAtLeast(1),
         )
         # The following will be shown (with --help) under "Other options"
         @option("--seven", help="1st uncategorized option")
         @option("--height", help="2nd uncategorized option")
         def cli(**kwargs):
-            """ A CLI that does nothing. """
+            """A CLI that does nothing."""
             print(kwargs)
 
         cli()
 
 .. tabbed:: Generated help
 
     .. code-block:: none
@@ -218,15 +218,15 @@
 
     @cloup.command()
     @input_grp.option('--one')
     @input_grp.option('--two')
     @output_grp.option('--three')
     @output_grp.option('--four')
     def cli_flat(one, two, three, four):
-        """ A CLI that does nothing. """
+        """A CLI that does nothing."""
         print(kwargs)
 
 The above notation is just syntax sugar on top of ``@cloup.option``:
 
 .. code-block:: python
 
     @input_grp.option('--one')
```

### Comparing `cloup-2.0.0.post1/docs/pages/sections.rst` & `cloup-2.1.0/docs/pages/sections.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 .. highlight:: none
 
 Subcommand sections
 ===================
 
-Cloup allows to organize the subcommand of a ``Group`` (or, more in general, of
+Cloup allows you to organize the subcommand of a ``Group`` (or, more in general, of
 a ``MultiCommand``) in multiple help sections. Each such help section is
 represented by a :class:`~cloup.Section` instance, which is just a titled
 container for commands.
 
 A ``Section`` can be:
 
 - **sorted** -- it lists the commands in alphabetical order
```

### Comparing `cloup-2.0.0.post1/examples/arguments_with_help.py` & `cloup-2.1.0/examples/arguments_with_help.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/examples/default_command.py` & `cloup-2.1.0/examples/default_command.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/examples/flat_option_groups.py` & `cloup-2.1.0/examples/flat_option_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,13 +28,13 @@
 @_output.option('--five', help='2nd output option')
 @_output.option('--six', help='3rd output option')
 # Other options
 @option('--seven', help='first uncategorized option',
         type=click.Choice('yes no ask'.split()))
 @option('--height', help='second uncategorized option')
 def main(**kwargs):
-    """ A CLI that does nothing. """
+    """A CLI that does nothing."""
     print(kwargs)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `cloup-2.0.0.post1/examples/git_sections.py` & `cloup-2.1.0/examples/git_sections.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
-This example shows how to use cloup.Section to organize the subcommands of
-a multi-command in many --help sections.
+This example shows how to use ``cloup.Section`` to organize the subcommands of
+a multi-command in many ``--help`` sections.
 
-The code was generated by parsing "git --help" and taking
-- the first 3 sections
+The code was generated by parsing ``git --help`` and taking
+- the first 3 sections;
 - for each section, the first 3 commands after shuffling them.
 """
 # flake8: noqa E128
 import cloup
 
 
 def f(**kwargs):
-    """ Dummy command callback """
+    """Dummy command callback."""
     print(**kwargs)
 
 
 # In a real big application, you would import the following commands from separate modules =========
 git_clone = cloup.command('clone', help='Clone a repository into a new directory')(f)
 git_init = cloup.command('init', help='Create an empty Git repository or reinitialize an existing one')(f)
```

### Comparing `cloup-2.0.0.post1/examples/manim/config.py` & `cloup-2.1.0/examples/manim/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,33 +5,30 @@
 
 @cloup.group(
     'config', aliases=['conf', 'cfg'],
     invoke_without_command=True,
     no_args_is_help=True,
 )
 def config():
-    """Manages Manim configuration files."""
-    pass
+    """Manage Manim configuration files."""
 
 
 @config.command(no_args_is_help=True)
 @cloup.option(
     "-l", "--level",
     type=cloup.Choice(["user", "cwd"], case_sensitive=False), default="cwd",
     help="Specify if this config is for user or the working directory.",
 )
 @cloup.option("-o", "--open", "openfile", is_flag=True)
 def write(level: str, openfile: bool) -> None:
-    """Writes configurations."""
-    pass
+    """Write configurations."""
 
 
 @config.command()
 def show():
-    """Shows current configuration."""
-    pass
+    """Show current configuration."""
 
 
 @config.command()
 @cloup.option("-d", "--directory", default=os.getcwd())
 def export(directory):
     pass
```

### Comparing `cloup-2.0.0.post1/examples/manim/main.py` & `cloup-2.1.0/examples/manim/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,29 +37,30 @@
             # command_help=Style(...),
             # heading=Style(...),
             # constraint=Style(fg='red'),
             # section_help=Style(...),
             # col1=Style(...),
             col2=Style(dim=True),
             epilog=Style(fg=Color.bright_white, italic=True),
+            alias=Style(fg=Color.yellow),
+            alias_secondary=Style(fg=Color.white),
         ),
     ),
 )
 
 
 @cloup.group(
     name='Manim',
     no_args_is_help=True,
     context_settings=CONTEXT_SETTINGS,
     epilog="Made with <3 by Manim Community developers.",
 )
 @cloup.version_option(version=VERSION)
 def main():
     """Animation engine for explanatory math videos."""
-    pass
 
 
 main.add_command(render)
 main.add_command(config)
 
 if __name__ == "__main__":
     main(prog_name='manim')
```

### Comparing `cloup-2.0.0.post1/examples/manim/render.py` & `cloup-2.1.0/examples/manim/render.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/examples/option_groups.py` & `cloup-2.1.0/examples/option_groups.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/requirements/dev.txt` & `cloup-2.1.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/requirements/docs.txt` & `cloup-2.1.0/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/requirements/test.txt` & `cloup-2.1.0/requirements/test.txt`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/scripts/generate_git_example.py` & `cloup-2.1.0/scripts/generate_git_example.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,16 @@
    reset             Reset current HEAD to the specified state
    switch            Switch branches
    tag               Create, list, delete or verify a tag object signed with GPG
 """.strip()
 
 CODE_TEMPLATE = """
 \"\"\"
-This example shows how to use cloup.Section to organize the subcommands of
-a multi-command in many --help sections.
+This example shows how to use ``cloup.Section`` to organize the subcommands of
+a multi-command in many ``--help`` sections.
 
 The code was generated by parsing "git --help" and taking
 - the first {max_section_count} sections
 - for each section, the first {max_commands_per_section} commands after shuffling them.
 \"\"\"
 import cloup
```

### Comparing `cloup-2.0.0.post1/scripts/remove.py` & `cloup-2.1.0/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/setup.py` & `cloup-2.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/conftest.py` & `cloup-2.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/constraints/conftest.py` & `cloup-2.1.0/tests/constraints/conftest.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/constraints/test_common.py` & `cloup-2.1.0/tests/constraints/test_common.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/constraints/test_conditional_constraints.py` & `cloup-2.1.0/tests/constraints/test_conditional_constraints.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/constraints/test_constraints.py` & `cloup-2.1.0/tests/constraints/test_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from cloup.constraints.exceptions import ConstraintViolated, UnsatisfiableConstraint
 from tests.util import (
     make_context, make_fake_context, make_options, parametrize, should_raise
 )
 
 
 class FakeConstraint(Constraint):
-    """Sometimes it's useful to use::
+    """Sometimes it's useful to use
 
         Mock(wraps=FakeConstraint(...))
 
     to create a test double with characteristics of both a mock and a fake."""
 
     def __init__(self, satisfied=True, consistent=True, help='help',
                  error='error', inconsistency_reason='consistency_error'):
```

### Comparing `cloup-2.0.0.post1/tests/constraints/test_support.py` & `cloup-2.1.0/tests/constraints/test_support.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/example_command.py` & `cloup-2.1.0/tests/example_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         constraint=If('three', then=RequireAtLeast(1))
     )
     @option('--seven', help='First uncategorized option.',
             type=click.Choice('yes no ask'.split()))
     @option('--height', help='Second uncategorized option.')
     @option('--nine', help='Third uncategorized option.', hidden=True)
     def cmd(**kwargs):
-        """ A CLI that does nothing. """
+        """A CLI that does nothing."""
         print(kwargs)
 
     if tabular_help:
         expected_help = (_TABULAR_ALIGNED_HELP if align_option_groups
                          else _TABULAR_NON_ALIGNED_HELP)
     else:
         expected_help = _LINEAR_HELP
```

### Comparing `cloup-2.0.0.post1/tests/example_group.py` & `cloup-2.1.0/tests/example_group.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/test_aliases.py` & `cloup-2.1.0/tests/test_aliases.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,24 @@
+from typing import Optional
+
 import click
 import pytest
 
 import cloup
-from cloup import Group
-from cloup._util import first_bool, reindent
+from cloup import Color, Group, HelpTheme, Style
+from cloup._util import first_bool, identity, reindent
+from cloup.styling import IStyle
 from cloup.typing import MISSING
 
 
 @pytest.fixture()
 def cli() -> cloup.Group:
     @cloup.group()
     def cli():
         """A package installer."""
-        pass
 
     @cloup.command(aliases=['i', 'add'])
     @cloup.argument('pkg')
     def install(pkg: str):
         """Install a package."""
         print('install', pkg)
 
@@ -165,7 +167,32 @@
 
           Manage the configuration.
 
         Options:
           --help  Show this message and exit.
     """)
     assert res.output == expected
+
+
+def test_alias_are_correctly_styled(runner):
+    red = Style(fg=Color.red)
+    green = Style(fg=Color.green)
+
+    def fmt(alias: IStyle = identity, alias_secondary: Optional[IStyle] = None):
+        theme = HelpTheme(alias=alias, alias_secondary=alias_secondary)
+        return Group.format_subcommand_aliases(["i", "add"], theme)
+
+    # No styles (default theme)
+    assert fmt() == "(i, add)"
+
+    # Only theme.alias
+    assert fmt(alias=green) == f"{green('(i, add)')}"
+
+    # Only theme.alias_secondary
+    assert fmt(alias_secondary=green) == (
+        green("(") + "i" + green(", ") + "add" + green(")")
+    )
+
+    # Both
+    assert fmt(alias=red, alias_secondary=green) == (
+        green("(") + red("i") + green(", ") + red("add") + green(")")
+    )
```

### Comparing `cloup-2.0.0.post1/tests/test_commands.py` & `cloup-2.1.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/test_context.py` & `cloup-2.1.0/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/test_formatting.py` & `cloup-2.1.0/tests/test_formatting.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 from textwrap import dedent
 from typing import Optional
 
 import click
 import pytest
 
 from cloup import HelpFormatter
-from cloup.typing import Possibly
 from cloup.formatting import HelpSection, unstyled_len
 from cloup.formatting.sep import (
     Hline, RowSepIf, RowSepPolicy, multiline_rows_are_at_least
 )
 from cloup.styling import HelpTheme, Style
+from cloup.typing import Possibly
 from tests.util import parametrize
 
 LOREM = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor."
 ROWS = [
     ('-l, --long-option-name TEXT', LOREM),
     ('--another-option INT', LOREM),
     ('--short', LOREM),
```

### Comparing `cloup-2.0.0.post1/tests/test_option_groups.py` & `cloup-2.1.0/tests/test_option_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tests for the "option groups" feature/module."""
+"""Test for the "option groups" feature/module."""
 from textwrap import dedent
 from typing import cast
 
 import click
 import pytest
 from click import pass_context
```

### Comparing `cloup-2.0.0.post1/tests/test_sections.py` & `cloup-2.1.0/tests/test_sections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Tests for the "subcommand sections" feature/module."""
+"""Test for the "subcommand sections" feature/module."""
 import click
 import pytest
 from click import pass_context
 
 import cloup
 from cloup import Section
 from cloup._util import pick_non_missing, reindent
```

### Comparing `cloup-2.0.0.post1/tests/test_sep.py` & `cloup-2.1.0/tests/test_sep.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/test_styling.py` & `cloup-2.1.0/tests/test_styling.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/test_util.py` & `cloup-2.1.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `cloup-2.0.0.post1/tests/util.py` & `cloup-2.1.0/tests/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 def make_fake_context(
     params: Iterable[click.Parameter],
     command_cls=cloup.Command,
     cls=Context,
     **ctx_kwargs
 ) -> Context:
-    """Creates a simple instance of Command with the specified parameters,
+    """Create a simple instance of Command with the specified parameters,
     then create a fake context without actually invoking the command."""
     return cls(
         command_cls('fake', params=params, callback=new_dummy_func()), **ctx_kwargs
     )
 
 
 def make_options(names: Iterable[str], **common_kwargs) -> List[click.Option]:
```

### Comparing `cloup-2.0.0.post1/tox.ini` & `cloup-2.1.0/tox.ini`

 * *Files identical despite different names*

