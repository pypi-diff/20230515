# Comparing `tmp/render_engine-2023.5.1a2.tar.gz` & `tmp/render_engine-2023.5.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "render_engine-2023.5.1a2.tar", last modified: Tue May  9 00:00:37 2023, max compression
+gzip compressed data, was "render_engine-2023.5.2a1.tar", last modified: Mon May 15 21:44:14 2023, max compression
```

## Comparing `render_engine-2023.5.1a2.tar` & `render_engine-2023.5.2a1.tar`

### file list

```diff
@@ -1,125 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.chglog/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.chglog/CHANGELOG.tpl.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.chglog/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.devcontainer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.devcontainer/devcontainer.json
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.devcontainer/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/CONTRIBUTION.md
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/Contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     9640 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/changelog.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.258398 render_engine-2023.5.1a2/docs/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/archive.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.262398 render_engine-2023.5.1a2/docs/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/assets/create-app-help.png
--rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/assets/render-engine-init-help.png
--rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/assets/render-engine-init.png
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/cli.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/collection.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.262398 render_engine-2023.5.1a2/docs/docs/contributing/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/contributing/pages.md
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/custom_collections.md
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/feeds.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.262398 render_engine-2023.5.1a2/docs/docs/getting-started/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/building-your-site.md
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/creating-a-collection.md
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/creating-a-page.md
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/creating-your-app.md
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/installation.md
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/getting-started/layout.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/hookspecs.md
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/page.md
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/parsers.md
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/site.md
--rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/docs/templates.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.262398 render_engine-2023.5.1a2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/.DS_Store
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.266398 render_engine-2023.5.1a2/src/render_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/blog.py
--rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/hookspecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/links.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.266398 render_engine-2023.5.1a2/src/render_engine/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/.DS_Store
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/README_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/base_parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.266398 render_engine-2023.5.1a2/src/render_engine/parsers/markdown/
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/markdown/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/parsers/markdown/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.266398 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/base_collection_path.md
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/content.html
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/create_app_py.txt
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/rss2.0.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/rss2.0_items.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/sitemap.xml
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/render_engine_templates/sitemap_item.xml
--rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/src/render_engine/site.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.266398 render_engine-2023.5.1a2/src/render_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-09 00:00:37.000000 render_engine-2023.5.1a2/src/render_engine.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/create_app_check_file.txt
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/create_app_check_file_no_site_vars.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/tests/site_test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/tests/site_test/blog/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/site_test/blog/test_blog_content.md
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/site_test/build.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 00:00:37.270398 render_engine-2023.5.1a2/tests/site_test/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/site_test/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_base_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_base_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_blog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_create_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_feeds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_parser_markdown_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-09 00:00:22.000000 render_engine-2023.5.1a2/tests/test_site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.chglog/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1142 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.chglog/CHANGELOG.tpl.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      330 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.chglog/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/devcontainer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.devcontainer/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/CONTRIBUTION.md
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/PULL_REQUEST_TEMPLATE/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/Contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12647 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.169125 render_engine-2023.5.2a1/docs/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/archive.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   273561 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/create-app-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)   288201 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/render-engine-init-help.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90538 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/assets/render-engine-init.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/collection.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/contributing/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/contributing/pages.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/custom_collections.md
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/feeds.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/docs/docs/getting-started/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/building-your-site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-collection.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-page.md
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/creating-your-app.md
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/getting-started/layout.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/hookspecs.md
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/page.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/parsers.md
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/site.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/docs/templates.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.173126 render_engine-2023.5.2a1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/.DS_Store
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6271 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/hookspecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/.DS_Store
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/README_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/base_parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/parsers/markdown/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/base_collection_path.md
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/content.html
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/create_app_py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      180 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/sitemap.xml
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/render_engine_templates/sitemap_item.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     7549 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/src/render_engine/site.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.177126 render_engine-2023.5.2a1/src/render_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-15 21:44:14.000000 render_engine-2023.5.2a1/src/render_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/create_app_check_file.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/create_app_check_file_no_site_vars.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/blog/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/blog/test_blog_content.md
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 21:44:14.181126 render_engine-2023.5.2a1/tests/site_test/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/site_test/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_base_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_base_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_blog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_create_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_feeds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_parser_markdown_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-15 21:43:57.000000 render_engine-2023.5.2a1/tests/test_site.py
```

### Comparing `render_engine-2023.5.1a2/.chglog/CHANGELOG.tpl.md` & `render_engine-2023.5.2a1/.chglog/CHANGELOG.tpl.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.devcontainer/devcontainer.json` & `render_engine-2023.5.2a1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/CODE_OF_CONDUCT.md` & `render_engine-2023.5.2a1/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/CONTRIBUTION.md` & `render_engine-2023.5.2a1/.github/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/FUNDING.yml` & `render_engine-2023.5.2a1/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/LICENSE` & `render_engine-2023.5.2a1/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/dependabot.yml` & `render_engine-2023.5.2a1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.github/workflows/publish.yml` & `render_engine-2023.5.2a1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/.gitignore` & `render_engine-2023.5.2a1/.gitignore`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/PKG-INFO` & `render_engine-2023.5.2a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render_engine
-Version: 2023.5.1a2
+Version: 2023.5.2a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.1a2/README.md` & `render_engine-2023.5.2a1/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/changelog.md` & `render_engine-2023.5.2a1/changelog.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,44 @@
 <a name="unreleased"></a>
 ## [Unreleased]
 
 
+<a name="2023.5.1"></a>
+## [2023.5.1] - 2023-05-08
+
+<a name="2023.5.1a2"></a>
+## [2023.5.1a2] - 2023-05-08
+
+<a name="2023.5.1a1"></a>
+## [2023.5.1a1] - 2023-05-08
+
+<a name="v-2023.5.1a1"></a>
+## [v-2023.5.1a1] - 2023-05-08
+### Pull Requests
+- Merge pull request [#187](https://github.com/kjaymiller/render_engine/issues/187) from kjaymiller:dependabot/pip/platformdirs-3.5.0
+- Merge pull request [#189](https://github.com/kjaymiller/render_engine/issues/189) from kjaymiller:dependabot/pip/ruff-0.0.265
+- Merge pull request [#188](https://github.com/kjaymiller/render_engine/issues/188) from kjaymiller:dependabot/pip/urllib3-2.0.2
+- Merge pull request [#190](https://github.com/kjaymiller/render_engine/issues/190) from kjaymiller:dependabot/pip/rich-13.3.5
+- Merge pull request [#191](https://github.com/kjaymiller/render_engine/issues/191) from kjaymiller:dependabot/pip/mkdocs-1.4.3
+- Merge pull request [#185](https://github.com/kjaymiller/render_engine/issues/185) from kjaymiller/kjaymiller/issue146
+- Merge pull request [#184](https://github.com/kjaymiller/render_engine/issues/184) from kjaymiller:kjaymiller/issue174
+- Merge pull request [#183](https://github.com/kjaymiller/render_engine/issues/183) from kjaymiller:renames-gs-getting-started-to-installation
+- Merge pull request [#158](https://github.com/kjaymiller/render_engine/issues/158) from kjaymiller/dependabot/pip/pymdown-extensions-9.11
+- Merge pull request [#160](https://github.com/kjaymiller/render_engine/issues/160) from kjaymiller/dependabot/pip/griffe-0.27.1
+- Merge pull request [#162](https://github.com/kjaymiller/render_engine/issues/162) from kjaymiller/dependabot/pip/attrs-23.1.0
+- Merge pull request [#165](https://github.com/kjaymiller/render_engine/issues/165) from kjaymiller/dependabot/pip/ruff-0.0.263
+- Merge pull request [#163](https://github.com/kjaymiller/render_engine/issues/163) from kjaymiller/dependabot/pip/pygments-2.15.1
+- Merge pull request [#181](https://github.com/kjaymiller/render_engine/issues/181) from kjaymiller/kjaymiller/issue84
+- Merge pull request [#179](https://github.com/kjaymiller/render_engine/issues/179) from kjaymiller/kjaymiller/issue87
+- Merge pull request [#178](https://github.com/kjaymiller/render_engine/issues/178) from kjaymiller/kjaymiller/issue142
+- Merge pull request [#177](https://github.com/kjaymiller/render_engine/issues/177) from kjaymiller:kjaymiller/issue168
+- Merge pull request [#176](https://github.com/kjaymiller/render_engine/issues/176) from kjaymiller/corrects-docs-for-createapp
+- Merge pull request [#175](https://github.com/kjaymiller/render_engine/issues/175) from jefftriplett/small-typos
+
+
 <a name="2023.4.2a1"></a>
 ## [2023.4.2a1] - 2023-04-16
 ### Reverts
 - Bump markdown from 3.3.7 to 3.4.3
 
 ### Pull Requests
 - Merge pull request [#156](https://github.com/kjaymiller/render_engine/issues/156) from kjaymiller:adds-changelog-from-chglog
@@ -118,15 +151,19 @@
 - Merge pull request [#54](https://github.com/kjaymiller/render_engine/issues/54) from jonafato/fix-docs-requirements
 - Merge pull request [#53](https://github.com/kjaymiller/render_engine/issues/53) from jonafato/missing-pages-broken-links
 - Merge pull request [#50](https://github.com/kjaymiller/render_engine/issues/50) from kjaymiller/adds-tox
 - Merge pull request [#41](https://github.com/kjaymiller/render_engine/issues/41) from jonafato/fix-tests
 - Merge pull request [#40](https://github.com/kjaymiller/render_engine/issues/40) from jonafato/test-in-ci
 
 
-[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.4.2a1...HEAD
+[Unreleased]: https://github.com/kjaymiller/render_engine/compare/2023.5.1...HEAD
+[2023.5.1]: https://github.com/kjaymiller/render_engine/compare/2023.5.1a2...2023.5.1
+[2023.5.1a2]: https://github.com/kjaymiller/render_engine/compare/2023.5.1a1...2023.5.1a2
+[2023.5.1a1]: https://github.com/kjaymiller/render_engine/compare/v-2023.5.1a1...2023.5.1a1
+[v-2023.5.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.4.2a1...v-2023.5.1a1
 [2023.4.2a1]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a5...2023.4.2a1
 [2023.4.1a5]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a4...2023.4.1a5
 [2023.4.1a4]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a3...2023.4.1a4
 [2023.4.1a3]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a2...2023.4.1a3
 [2023.4.1a2]: https://github.com/kjaymiller/render_engine/compare/2023.4.1a1...2023.4.1a2
 [2023.4.1a1]: https://github.com/kjaymiller/render_engine/compare/2023.3.1b13...2023.4.1a1
 [2023.3.1b13]: https://github.com/kjaymiller/render_engine/compare/2023.3.1b14...2023.3.1b13
```

### Comparing `render_engine-2023.5.1a2/docs/docs/archive.md` & `render_engine-2023.5.2a1/docs/docs/archive.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/assets/create-app-help.png` & `render_engine-2023.5.2a1/docs/docs/assets/create-app-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/assets/render-engine-init-help.png` & `render_engine-2023.5.2a1/docs/docs/assets/render-engine-init-help.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/assets/render-engine-init.png` & `render_engine-2023.5.2a1/docs/docs/assets/render-engine-init.png`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/cli.md` & `render_engine-2023.5.2a1/docs/docs/cli.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/contributing/pages.md` & `render_engine-2023.5.2a1/docs/docs/contributing/pages.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/custom_collections.md` & `render_engine-2023.5.2a1/docs/docs/custom_collections.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/getting-started/building-your-site.md` & `render_engine-2023.5.2a1/docs/docs/getting-started/building-your-site.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/getting-started/creating-a-collection.md` & `render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-collection.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/getting-started/creating-a-page.md` & `render_engine-2023.5.2a1/docs/docs/getting-started/creating-a-page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/getting-started/installation.md` & `render_engine-2023.5.2a1/docs/docs/getting-started/installation.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/getting-started/layout.md` & `render_engine-2023.5.2a1/docs/docs/getting-started/layout.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/index.md` & `render_engine-2023.5.2a1/docs/docs/index.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/page.md` & `render_engine-2023.5.2a1/docs/docs/page.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/parsers.md` & `render_engine-2023.5.2a1/docs/docs/parsers.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/docs/templates.md` & `render_engine-2023.5.2a1/docs/docs/templates.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/docs/mkdocs.yml` & `render_engine-2023.5.2a1/docs/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/pyproject.toml` & `render_engine-2023.5.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/.DS_Store` & `render_engine-2023.5.2a1/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/.DS_Store` & `render_engine-2023.5.2a1/src/render_engine/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/_base_object.py` & `render_engine-2023.5.2a1/src/render_engine/_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/archive.py` & `render_engine-2023.5.2a1/src/render_engine/archive.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/blog.py` & `render_engine-2023.5.2a1/src/render_engine/blog.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/cli.py` & `render_engine-2023.5.2a1/src/render_engine/cli.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/collection.py` & `render_engine-2023.5.2a1/src/render_engine/collection.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/engine.py` & `render_engine-2023.5.2a1/src/render_engine/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import urllib.parse
+
 from datetime import datetime
 from email import utils
 
 from jinja2 import (
     ChoiceLoader,
     Environment,
     FileSystemLoader,
@@ -30,22 +32,30 @@
 def to_pub_date(value: datetime):
     """
     Parse information from the given class object.
     """
     return utils.format_datetime(value)
 engine.filters["to_pub_date"] = to_pub_date
 
+
 @pass_environment
 def format_datetime(env: Environment, value: str) -> str:
     """
     Parse information from the given class object.
     """
     return datetime.strftime(value, env.globals.get("DATETIME_FORMAT", "%d %b %Y %H:%M %Z"))
 engine.filters["format_datetime"] = format_datetime
 
+
+@pass_environment
+def to_absolute(env: Environment, url:str) -> str:
+    return urllib.parse.urljoin(env.globals.get('SITE_URL'), url)
+engine.filters["to_absolute"] = to_absolute
+
+
 @pass_environment
 def url_for(env: Environment, value: str, page: int=0) -> str:
     """Look for the route in the route_list and return the url for the page."""
     routes = env.globals.get("routes")
     route = value.split(".", maxsplit=1)
 
     if len(route) == 2 and type(route) == list:
```

### Comparing `render_engine-2023.5.1a2/src/render_engine/feeds.py` & `render_engine-2023.5.2a1/src/render_engine/feeds.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/hookspecs.py` & `render_engine-2023.5.2a1/src/render_engine/hookspecs.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/links.py` & `render_engine-2023.5.2a1/src/render_engine/links.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/page.py` & `render_engine-2023.5.2a1/src/render_engine/page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/parsers/.DS_Store` & `render_engine-2023.5.2a1/src/render_engine/parsers/.DS_Store`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/parsers/README_TEMPLATE.md` & `render_engine-2023.5.2a1/src/render_engine/parsers/README_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/parsers/base_parsers.py` & `render_engine-2023.5.2a1/src/render_engine/parsers/base_parsers.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/parsers/markdown/README.md` & `render_engine-2023.5.2a1/src/render_engine/parsers/markdown/README.md`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/plugins.py` & `render_engine-2023.5.2a1/src/render_engine/plugins.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/render_engine_templates/create_app_py.txt` & `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/create_app_py.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/render_engine_templates/index.html` & `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/index.html`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/render_engine_templates/rss2.0.xml` & `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0.xml`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

 * *Files 4% similar despite different names*

#### Comparing `render_engine-2023.5.1a2/src/render_engine/render_engine_templates/rss2.0_items.xml` & `render_engine-2023.5.2a1/src/render_engine/render_engine_templates/rss2.0_items.xml`

```diff
@@ -15,20 +15,22 @@
 {% if item.category is defined and category %}
   {% if item.category is defined and category['domain'] %}
   <category domain="{{item.category['domain']}}">{{item.category}}</category>
   {% else %}
   <category>{{item.category}}</category>
   {% endif %}
 {% endif %}
-  <link>{{SITE_URL}}{{item.url_for()}}</link>
+  <link>{{item.url_for() | to_absolute }}</link>
   {% if item.date is defined %}
   <pubDate>{{item.date | to_pub_date }}</pubDate>
   {% endif %}
-{% if item.guid is defined and guid %}
+{% if item.guid is defined %}
   <guid isPermaLink="false">{{item.guid}}</guid>
+  {% else %}
+  <guid isPermaLink="true">{{item.url_for() | to_absolute }}</guid>
   {% endif %}
 {% if item.author is defined and author %}{{item.author}}{% endif %}
 {% if item.comments is defined and comments %}{{item.comments}}{% endif %}
 {% if item.source is defined and source %}
   <source url="{{item.source.url}}">{{item.source}}</source>
   {% endif %}
 </item>
```

### Comparing `render_engine-2023.5.1a2/src/render_engine/site.py` & `render_engine-2023.5.2a1/src/render_engine/site.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/src/render_engine.egg-info/PKG-INFO` & `render_engine-2023.5.2a1/src/render_engine.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: render-engine
-Version: 2023.5.1a2
+Version: 2023.5.2a1
 Summary: A Flexible Static Site Generator for Python
 Project-URL: homepage, https://github.com/kjaymiller/render_engine/
 Project-URL: repository, https://github.com/kjaymiller/render_engine/
 Project-URL: documentation, https://render-engine.readthedocs.io/en/latest/
 Description-Content-Type: text/markdown
 Provides-Extra: dev
```

### Comparing `render_engine-2023.5.1a2/src/render_engine.egg-info/SOURCES.txt` & `render_engine-2023.5.2a1/src/render_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/create_app_check_file.txt` & `render_engine-2023.5.2a1/tests/create_app_check_file.txt`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_base_object.py` & `render_engine-2023.5.2a1/tests/test_base_object.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_base_parser.py` & `render_engine-2023.5.2a1/tests/test_base_parser.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_collections.py` & `render_engine-2023.5.2a1/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_create_app.py` & `render_engine-2023.5.2a1/tests/test_create_app.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_feeds.py` & `render_engine-2023.5.2a1/tests/test_feeds.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import datetime
 
 import pluggy
+import pytest
 from jinja2 import StrictUndefined
 
 from render_engine.collection import Collection
-from render_engine.engine import engine, to_pub_date
 from render_engine.feeds import RSSFeed
 from render_engine.page import Page
 
 pm = pluggy.PluginManager("fake_test")
 
 
 def test_can_manually_set_slug():
@@ -50,30 +50,27 @@
         archive_template = None
         Feed = RSSFeed
 
     collection = BasicCollection()
 
     assert collection._feed.title == "BasicCollection"
 
-def test_rss_feed_item_url(tmp_path):
+
+def test_rss_feed_item_url(site):
     """Test that the feed item url is set correctly"""
-    tmp_dir = tmp_path / "content"
-    tmp_dir.mkdir()
-    file = tmp_dir / "#"
-    file.write_text("test")
+    assert "<link>http://localhost:8000/page.html</link>" in site._route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
-    class TestCollection(Collection):
-        pages = [Page(content_path=file)]
-        Feed = RSSFeed
 
-    collection = TestCollection()
-    print(collection._feed.template)
-    assert "http://localhost:8000//page.html" in collection._feed._render_content(engine=engine)
+
+def test_rss_feed_item_has_guid(site):
+    """Test that the feed item url is set correctly"""
+    assert '<guid isPermaLink="true">http://localhost:8000/page.html</guid>' in site._route_list['testcollection']._feed._render_content(engine=site.engine, SITE_URL="http://localhost:8000")
 
 
+@pytest.mark.skip("Invalid Test")
 def test_rss_feed_template_with_strictundefined(engine, tmp_path):
     """Test that the RSS feed template works with the StrictUndefined undefined handler."""
     tmp_dir = tmp_path / "content"
     tmp_dir.mkdir()
     file = tmp_dir / "#"
     file.write_text("test")
 
@@ -101,16 +98,14 @@
         date = datetime.datetime(2023, 4, 15, 0, 0, 0, tzinfo=datetime.timezone.utc)   # noqa: UP017
     class TestCollection(Collection):
         Feed = RSSFeed
         pages = [TestPage()]
 
     collection = TestCollection()
 
-    engine.filters["to_pub_date"] = to_pub_date
-
     rendered_content = collection._feed._render_content(
         engine=engine,
         SITE_TITLE="Test Site Title",
         SITE_URL="http://localhost:8000",
         title="Test Feed Title",
         description="Test Feed Description",
     )
```

### Comparing `render_engine-2023.5.1a2/tests/test_page.py` & `render_engine-2023.5.2a1/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `render_engine-2023.5.1a2/tests/test_site.py` & `render_engine-2023.5.2a1/tests/test_site.py`

 * *Files identical despite different names*

