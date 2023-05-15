# Comparing `tmp/obsidianhtml-3.5.1.tar.gz` & `tmp/obsidianhtml-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obsidianhtml-3.5.1.tar", last modified: Sat May 13 15:56:47 2023, max compression
+gzip compressed data, was "obsidianhtml-3.5.2.tar", last modified: Mon May 15 11:56:04 2023, max compression
```

## Comparing `obsidianhtml-3.5.1.tar` & `obsidianhtml-3.5.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.928703 obsidianhtml-3.5.1/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    35149 2022-02-06 13:26:34.000000 obsidianhtml-3.5.1/LICENSE
--rw-r--r--   0 dorus     (1000) dorus     (1000)       76 2022-02-06 13:26:34.000000 obsidianhtml-3.5.1/MANIFEST.in
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1558 2023-05-13 15:56:47.928703 obsidianhtml-3.5.1/PKG-INFO
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.872036 obsidianhtml-3.5.1/obsidianhtml/
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-02-06 13:26:34.000000 obsidianhtml-3.5.1/obsidianhtml/README.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)      737 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/SharedResources.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1831 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)       38 2023-02-12 21:27:12.000000 obsidianhtml-3.5.1/obsidianhtml/__main__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.875370 obsidianhtml-3.5.1/obsidianhtml/compiler/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     8991 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/compiler/HTML.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    17089 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/compiler/Templating.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:04.000000 obsidianhtml-3.5.1/obsidianhtml/compiler/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:04.000000 obsidianhtml-3.5.1/obsidianhtml/compiler/__main__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.878703 obsidianhtml-3.5.1/obsidianhtml/controller/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    23942 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/controller/ConvertVault.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3011 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/controller/Export.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    12403 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/controller/Run.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2262 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/controller/Serve.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:08.000000 obsidianhtml-3.5.1/obsidianhtml/controller/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:08.000000 obsidianhtml-3.5.1/obsidianhtml/controller/__main__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.882036 obsidianhtml-3.5.1/obsidianhtml/core/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2227 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/Actor.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    16551 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/ConfigManager.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     8086 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/CopyVault.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3331 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/ErrorHandling.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     7250 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/core/FileFinder.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    12067 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/FileObject.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     6973 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/Index.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     6357 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/core/NetworkTree.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5894 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/core/PicknickBasket.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1175 2023-02-12 21:35:22.000000 obsidianhtml-3.5.1/obsidianhtml/core/Types.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-17 19:18:31.000000 obsidianhtml-3.5.1/obsidianhtml/core/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-17 19:18:31.000000 obsidianhtml-3.5.1/obsidianhtml/core/__main__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2652 2022-12-19 20:59:29.000000 obsidianhtml-3.5.1/obsidianhtml/core/readme.md
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.885370 obsidianhtml-3.5.1/obsidianhtml/features/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    14593 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/features/CreateIndexFromDirStructure.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    10973 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/features/CreateIndexFromTags.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     8580 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/features/EmbeddedSearch.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    14966 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/features/RssFeed.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1655 2023-04-09 20:17:12.000000 obsidianhtml-3.5.1/obsidianhtml/features/Search.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4305 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/features/SidePane.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2023-02-12 12:08:54.000000 obsidianhtml-3.5.1/obsidianhtml/features/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2023-02-12 12:15:24.000000 obsidianhtml-3.5.1/obsidianhtml/features/__main__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1813 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/features/add_toc_when_missing.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2436 2023-02-12 21:35:23.000000 obsidianhtml-3.5.1/obsidianhtml/features/post_processing.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.885370 obsidianhtml-3.5.1/obsidianhtml/gui/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3425 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/Api.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      849 2023-04-09 20:17:12.000000 obsidianhtml-3.5.1/obsidianhtml/gui/ConfigChecker.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3166 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/Ledger.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3465 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/Templater.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1929 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/WindowManager.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      508 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      649 2023-02-12 21:35:23.000000 obsidianhtml-3.5.1/obsidianhtml/gui/__main__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      823 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/gui/lib.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)      351 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/gui/readme.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)     7877 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/lib.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.888703 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2628 2023-04-09 20:16:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/AdmonitionExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1321 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/BlockLinkExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     7309 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CallOutExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1839 2023-04-09 20:16:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CodeWrapperExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2511 2023-04-09 20:17:12.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CustomTableExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    13444 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CustomTocExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4487 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/DataviewExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1986 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/EmbeddedSearchExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4332 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/EraserExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    20430 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/FootnoteExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1974 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/FormattingExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3366 2023-04-09 20:16:25.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/MermaidExtension.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-07-29 10:39:28.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-07-30 10:57:29.000000 obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/__main__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.888703 obsidianhtml-3.5.1/obsidianhtml/md2html/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    20143 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/md2html/__init__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.888703 obsidianhtml-3.5.1/obsidianhtml/note2md/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1132 2023-04-09 20:21:25.000000 obsidianhtml-3.5.1/obsidianhtml/note2md/__init__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.892036 obsidianhtml-3.5.1/obsidianhtml/parser/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     8326 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/parser/HeaderTree.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3011 2023-02-12 21:35:23.000000 obsidianhtml-3.5.1/obsidianhtml/parser/MarkdownLink.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)    23606 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/parser/MarkdownPage.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:23.000000 obsidianhtml-3.5.1/obsidianhtml/parser/__init__.py
--rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:23.000000 obsidianhtml-3.5.1/obsidianhtml/parser/__main__.py
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.892036 obsidianhtml-3.5.1/obsidianhtml/src/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    15084 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/src/defaults_config.yml
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.895370 obsidianhtml-3.5.1/obsidianhtml/src/graph/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      399 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5545 2022-12-17 13:48:34.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_2d.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1866 2022-09-11 10:30:46.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_3d.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1055 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_node_graph.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1560 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)    11307 2022-11-13 16:19:09.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1152 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.svg
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4959 2023-01-14 12:12:51.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/graph_full_page.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      871 2022-07-30 17:25:48.000000 obsidianhtml-3.5.1/obsidianhtml/src/graph/graph_template.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.895370 obsidianhtml-3.5.1/obsidianhtml/src/help_texts/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      601 2022-09-07 13:16:28.000000 obsidianhtml-3.5.1/obsidianhtml/src/help_texts/export_help_text
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2138 2023-05-13 15:50:50.000000 obsidianhtml-3.5.1/obsidianhtml/src/help_texts/help_text
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.895370 obsidianhtml-3.5.1/obsidianhtml/src/html/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.898703 obsidianhtml-3.5.1/obsidianhtml/src/html/css/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3845 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/callouts.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5777 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/codehilite.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)    17987 2023-05-13 15:51:13.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/global_main.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      818 2022-08-26 16:39:36.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/global_overwrites.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)    39538 2022-09-19 12:16:07.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/master.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5429 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/mermaid.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)       36 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/css/taglist.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)    12014 2022-02-17 17:27:05.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/favicon.ico
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.898703 obsidianhtml-3.5.1/obsidianhtml/src/html/fonts/
--rw-r--r--   0 dorus     (1000) dorus     (1000)   168260 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/fonts/Roboto-Regular.ttf
--rw-r--r--   0 dorus     (1000) dorus     (1000)   192740 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/fonts/SourceCodePro-Regular.ttf
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.898703 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1878 2022-07-24 12:59:51.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_documentation.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      583 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_minimal.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5491 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_tabs.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)     7716 2023-01-14 12:12:43.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_documentation.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      769 2023-01-14 12:12:55.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_minimal.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3845 2023-02-10 12:09:14.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_tabs.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.902036 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      121 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/audio_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1148 2022-12-23 20:32:49.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/full_header.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      126 2023-02-12 13:25:42.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/image_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      230 2022-12-21 21:33:08.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/left_pane.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      993 2022-12-23 20:32:05.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/minimal_header.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      199 2022-09-03 16:06:56.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/not_created.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      236 2022-12-21 21:41:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/right_pane.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      107 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/templates/video_template.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.902036 obsidianhtml-3.5.1/obsidianhtml/src/html/themes/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      897 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/themes/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      339 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/themes/popup.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     6268 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/html/themes/theme-obsidian.css
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.905370 obsidianhtml-3.5.1/obsidianhtml/src/imported/
--rw-r--r--   0 dorus     (1000) dorus     (1000)   729969 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/imported/3d-force-graph.v1.70.10.min.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)    16183 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/imported/flexsearch.v0.7.2.bundle.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)   797631 2022-11-13 16:20:13.000000 obsidianhtml-3.5.1/obsidianhtml/src/imported/mathjax.v3.es5.tex-chtml.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)  1133121 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/imported/mermaid.9.0.1.min.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)  4257261 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/imported/mermaid.9.0.1.min.js.map
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.915370 obsidianhtml-3.5.1/obsidianhtml/src/index_from_dir_structure/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      298 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/index_from_dir_structure/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-09-03 19:36:31.000000 obsidianhtml-3.5.1/obsidianhtml/src/index_from_dir_structure/dirtree.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)      221 2022-02-20 16:31:45.000000 obsidianhtml-3.5.1/obsidianhtml/src/index_from_dir_structure/dirtree.svg
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.868703 obsidianhtml-3.5.1/obsidianhtml/src/installer/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.915370 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/
--rw-r--r--   0 dorus     (1000) dorus     (1000)    14562 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/configurations.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    13783 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/gp_installer.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    11339 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/index.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    12338 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/init.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      110 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/readme.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)    24152 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/setup_gitpages.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    13991 2022-04-30 21:45:32.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/test.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.868703 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.915370 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/components/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1977 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/components/select-entrypoint-path.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      889 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/components/select-vault-path.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.918703 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     6098 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/configurations_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     5319 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/gp_installer_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2875 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/index_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3874 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/init_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    15688 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/setup_gitpages_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      893 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/test_template.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.918703 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/js/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     4169 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/js/core.js
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.918703 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      828 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/action_components.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      448 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/error.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      625 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/flex.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      968 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/main.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)      655 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/response.css
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.918703 obsidianhtml-3.5.1/obsidianhtml/src/js/
--rw-r--r--   0 dorus     (1000) dorus     (1000)   108114 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/js/encoding.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2740 2022-12-21 21:59:01.000000 obsidianhtml-3.5.1/obsidianhtml/src/js/load_dirtree_footer.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)    18145 2023-02-12 21:57:56.000000 obsidianhtml-3.5.1/obsidianhtml/src/js/obsidian_core.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)    10057 2023-02-10 12:23:33.000000 obsidianhtml-3.5.1/obsidianhtml/src/js/obsidian_tabs_footer.js
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.918703 obsidianhtml-3.5.1/obsidianhtml/src/latex/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      297 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/latex/load_mathjax.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)      482 2022-09-04 19:38:03.000000 obsidianhtml-3.5.1/obsidianhtml/src/latex/load_mathjax_header_template.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.922036 obsidianhtml-3.5.1/obsidianhtml/src/rss/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      261 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/rss/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      530 2023-02-09 20:49:44.000000 obsidianhtml-3.5.1/obsidianhtml/src/rss/channel_template.xml
--rw-r--r--   0 dorus     (1000) dorus     (1000)      252 2022-02-17 17:26:47.000000 obsidianhtml-3.5.1/obsidianhtml/src/rss/item_template.xml
--rw-r--r--   0 dorus     (1000) dorus     (1000)      767 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/rss/rss.svg
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.922036 obsidianhtml-3.5.1/obsidianhtml/src/search/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1135 2023-01-28 17:50:13.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)   242525 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/pako.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)     3500 2023-03-02 13:48:12.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/search.css
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1782 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/search.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)    13950 2023-01-29 17:52:44.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/search.js
--rw-r--r--   0 dorus     (1000) dorus     (1000)      947 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/search/search.svg
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.928703 obsidianhtml-3.5.1/obsidianhtml/src/svgs/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/abstract.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/attention.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      479 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/bug.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/caution.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/check.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      535 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/cite.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/danger.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/done.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/error.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      474 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/example.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      534 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/external.svg
--rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/fail.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/failure.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/faq.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      247 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/fold.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      545 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/hashtag.svg
--rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/help.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      390 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/important.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      339 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/info.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/missing.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      303 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/note.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/question.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      535 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/quote.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/success.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/summary.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      390 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/tip.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/tldr.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      329 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/todo.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.1/obsidianhtml/src/svgs/warning.html
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.928703 obsidianhtml-3.5.1/obsidianhtml/src/tags_page/
--rw-r--r--   0 dorus     (1000) dorus     (1000)      252 2022-06-18 16:13:52.000000 obsidianhtml-3.5.1/obsidianhtml/src/tags_page/button_template.html
--rw-r--r--   0 dorus     (1000) dorus     (1000)        6 2023-05-13 15:56:41.000000 obsidianhtml-3.5.1/obsidianhtml/src/version
-drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-13 15:56:47.875370 obsidianhtml-3.5.1/obsidianhtml.egg-info/
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1558 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/PKG-INFO
--rw-r--r--   0 dorus     (1000) dorus     (1000)     7777 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/SOURCES.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/dependency_links.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)     1061 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/entry_points.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      132 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/requires.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)       13 2023-05-13 15:56:47.000000 obsidianhtml-3.5.1/obsidianhtml.egg-info/top_level.txt
--rw-r--r--   0 dorus     (1000) dorus     (1000)      807 2022-03-11 21:09:45.000000 obsidianhtml-3.5.1/pypi_readme.md
--rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-02-12 21:35:19.000000 obsidianhtml-3.5.1/pyproject.toml
--rw-r--r--   0 dorus     (1000) dorus     (1000)     2149 2023-05-13 15:56:47.932036 obsidianhtml-3.5.1/setup.cfg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.729824 obsidianhtml-3.5.2/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    35149 2022-02-06 13:26:34.000000 obsidianhtml-3.5.2/LICENSE
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       76 2022-02-06 13:26:34.000000 obsidianhtml-3.5.2/MANIFEST.in
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1558 2023-05-15 11:56:04.729824 obsidianhtml-3.5.2/PKG-INFO
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.656490 obsidianhtml-3.5.2/obsidianhtml/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-02-06 13:26:34.000000 obsidianhtml-3.5.2/obsidianhtml/README.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      737 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/SharedResources.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1831 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       38 2023-02-12 21:27:12.000000 obsidianhtml-3.5.2/obsidianhtml/__main__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.659824 obsidianhtml-3.5.2/obsidianhtml/compiler/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     8991 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/compiler/HTML.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    17089 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/compiler/Templating.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:04.000000 obsidianhtml-3.5.2/obsidianhtml/compiler/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:04.000000 obsidianhtml-3.5.2/obsidianhtml/compiler/__main__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.659824 obsidianhtml-3.5.2/obsidianhtml/controller/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    23953 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/controller/ConvertVault.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3011 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/controller/Export.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    12403 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/controller/Run.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2262 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/controller/Serve.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:08.000000 obsidianhtml-3.5.2/obsidianhtml/controller/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:08.000000 obsidianhtml-3.5.2/obsidianhtml/controller/__main__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.663157 obsidianhtml-3.5.2/obsidianhtml/core/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2227 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/Actor.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    16551 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/ConfigManager.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     8086 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/CopyVault.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3331 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/ErrorHandling.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     7352 2023-05-14 20:03:32.000000 obsidianhtml-3.5.2/obsidianhtml/core/FileFinder.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    12395 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/FileObject.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     6973 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/Index.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     6357 2023-05-14 10:08:44.000000 obsidianhtml-3.5.2/obsidianhtml/core/NetworkTree.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5894 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/core/PicknickBasket.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1175 2023-02-12 21:35:22.000000 obsidianhtml-3.5.2/obsidianhtml/core/Types.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-17 19:18:31.000000 obsidianhtml-3.5.2/obsidianhtml/core/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-17 19:18:31.000000 obsidianhtml-3.5.2/obsidianhtml/core/__main__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2652 2022-12-19 20:59:29.000000 obsidianhtml-3.5.2/obsidianhtml/core/readme.md
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.666490 obsidianhtml-3.5.2/obsidianhtml/features/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    14649 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/features/CreateIndexFromDirStructure.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10973 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/features/CreateIndexFromTags.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     8580 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/features/EmbeddedSearch.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    14966 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/features/RssFeed.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1655 2023-04-09 20:17:12.000000 obsidianhtml-3.5.2/obsidianhtml/features/Search.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4305 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/features/SidePane.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2023-02-12 12:08:54.000000 obsidianhtml-3.5.2/obsidianhtml/features/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2023-02-12 12:15:24.000000 obsidianhtml-3.5.2/obsidianhtml/features/__main__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1813 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/features/add_toc_when_missing.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2436 2023-02-12 21:35:23.000000 obsidianhtml-3.5.2/obsidianhtml/features/post_processing.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.669824 obsidianhtml-3.5.2/obsidianhtml/gui/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3425 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/Api.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      849 2023-04-09 20:17:12.000000 obsidianhtml-3.5.2/obsidianhtml/gui/ConfigChecker.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3166 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/Ledger.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3465 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/Templater.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1929 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/WindowManager.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      508 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      649 2023-02-12 21:35:23.000000 obsidianhtml-3.5.2/obsidianhtml/gui/__main__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      823 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/gui/lib.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      351 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/gui/readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     7877 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/lib.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.669824 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2628 2023-04-09 20:16:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/AdmonitionExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1321 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/BlockLinkExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     7309 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CallOutExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1839 2023-04-09 20:16:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CodeWrapperExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2511 2023-04-09 20:17:12.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CustomTableExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    13444 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CustomTocExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4487 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/DataviewExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1986 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/EmbeddedSearchExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4332 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/EraserExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    20430 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/FootnoteExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1974 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/FormattingExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3366 2023-04-09 20:16:25.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/MermaidExtension.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-07-29 10:39:28.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-07-30 10:57:29.000000 obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/__main__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.673157 obsidianhtml-3.5.2/obsidianhtml/md2html/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    20209 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/md2html/__init__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.673157 obsidianhtml-3.5.2/obsidianhtml/note2md/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1132 2023-04-09 20:21:25.000000 obsidianhtml-3.5.2/obsidianhtml/note2md/__init__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.673157 obsidianhtml-3.5.2/obsidianhtml/parser/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     8326 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/parser/HeaderTree.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3138 2023-05-14 08:48:40.000000 obsidianhtml-3.5.2/obsidianhtml/parser/MarkdownLink.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    23606 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/parser/MarkdownPage.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:23.000000 obsidianhtml-3.5.2/obsidianhtml/parser/__init__.py
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        0 2022-12-21 19:04:23.000000 obsidianhtml-3.5.2/obsidianhtml/parser/__main__.py
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.673157 obsidianhtml-3.5.2/obsidianhtml/src/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    15084 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/defaults_config.yml
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.676490 obsidianhtml-3.5.2/obsidianhtml/src/graph/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      399 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5545 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_2d.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1866 2022-09-11 10:30:46.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_3d.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1055 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_node_graph.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1560 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    11307 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1152 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.svg
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4959 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/graph_full_page.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      871 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/graph/graph_template.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.676490 obsidianhtml-3.5.2/obsidianhtml/src/help_texts/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      601 2022-09-07 13:16:28.000000 obsidianhtml-3.5.2/obsidianhtml/src/help_texts/export_help_text
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2138 2023-05-15 11:55:17.000000 obsidianhtml-3.5.2/obsidianhtml/src/help_texts/help_text
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.676490 obsidianhtml-3.5.2/obsidianhtml/src/html/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.679824 obsidianhtml-3.5.2/obsidianhtml/src/html/css/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3845 2023-03-02 13:48:12.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/callouts.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5777 2023-03-02 13:48:12.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/codehilite.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    17987 2023-05-13 15:51:13.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/global_main.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      818 2022-08-26 16:39:36.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/global_overwrites.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    39538 2022-09-19 12:16:07.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/master.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5429 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/mermaid.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       36 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/css/taglist.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    12014 2022-02-17 17:27:05.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/favicon.ico
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.679824 obsidianhtml-3.5.2/obsidianhtml/src/html/fonts/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   168260 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/fonts/Roboto-Regular.ttf
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   192740 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/fonts/SourceCodePro-Regular.ttf
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.683157 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1878 2022-07-24 12:59:51.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_documentation.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      583 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_minimal.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5491 2023-03-02 13:48:12.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_tabs.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     7716 2023-01-14 12:12:43.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_documentation.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      769 2023-01-14 12:12:55.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_minimal.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3845 2023-02-10 12:09:14.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_tabs.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.683157 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      121 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/audio_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1148 2022-12-23 20:32:49.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/full_header.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      126 2023-02-12 13:25:42.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/image_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      230 2022-12-21 21:33:08.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/left_pane.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      993 2022-12-23 20:32:05.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/minimal_header.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      199 2022-09-03 16:06:56.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/not_created.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      236 2022-12-21 21:41:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/right_pane.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      107 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/templates/video_template.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.683157 obsidianhtml-3.5.2/obsidianhtml/src/html/themes/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      897 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/themes/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      339 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/themes/popup.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     6268 2023-03-02 13:48:12.000000 obsidianhtml-3.5.2/obsidianhtml/src/html/themes/theme-obsidian.css
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.696490 obsidianhtml-3.5.2/obsidianhtml/src/imported/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   729969 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/imported/3d-force-graph.v1.70.10.min.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    16183 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/imported/flexsearch.v0.7.2.bundle.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   797631 2022-11-13 16:20:13.000000 obsidianhtml-3.5.2/obsidianhtml/src/imported/mathjax.v3.es5.tex-chtml.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)  1133121 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/imported/mermaid.9.0.1.min.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)  4257261 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/imported/mermaid.9.0.1.min.js.map
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.713157 obsidianhtml-3.5.2/obsidianhtml/src/index_from_dir_structure/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      298 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/index_from_dir_structure/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-09-03 19:36:31.000000 obsidianhtml-3.5.2/obsidianhtml/src/index_from_dir_structure/dirtree.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      221 2022-02-20 16:31:45.000000 obsidianhtml-3.5.2/obsidianhtml/src/index_from_dir_structure/dirtree.svg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.653157 obsidianhtml-3.5.2/obsidianhtml/src/installer/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.713157 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    14562 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/configurations.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    13783 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/gp_installer.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    11339 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/index.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    12338 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/init.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      110 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    24152 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/setup_gitpages.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    13991 2022-04-30 21:45:32.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/test.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.653157 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.716490 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/components/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1977 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/components/select-entrypoint-path.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      889 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/components/select-vault-path.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.716490 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     6098 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/configurations_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     5319 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/gp_installer_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2875 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/index_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3874 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/init_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    15688 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/setup_gitpages_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      893 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/test_template.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.716490 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/js/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     4169 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/js/core.js
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.719824 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      828 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/action_components.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      448 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/error.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      625 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/flex.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      968 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/main.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      655 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/response.css
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.719824 obsidianhtml-3.5.2/obsidianhtml/src/js/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   108114 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/js/encoding.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2740 2022-12-21 21:59:01.000000 obsidianhtml-3.5.2/obsidianhtml/src/js/load_dirtree_footer.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    18145 2023-02-12 21:57:56.000000 obsidianhtml-3.5.2/obsidianhtml/src/js/obsidian_core.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    10057 2023-02-10 12:23:33.000000 obsidianhtml-3.5.2/obsidianhtml/src/js/obsidian_tabs_footer.js
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.719824 obsidianhtml-3.5.2/obsidianhtml/src/latex/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      297 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/latex/load_mathjax.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      482 2022-09-04 19:38:03.000000 obsidianhtml-3.5.2/obsidianhtml/src/latex/load_mathjax_header_template.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.719824 obsidianhtml-3.5.2/obsidianhtml/src/rss/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      261 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/rss/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      530 2023-02-09 20:49:44.000000 obsidianhtml-3.5.2/obsidianhtml/src/rss/channel_template.xml
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      252 2022-02-17 17:26:47.000000 obsidianhtml-3.5.2/obsidianhtml/src/rss/item_template.xml
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      767 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/rss/rss.svg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.723157 obsidianhtml-3.5.2/obsidianhtml/src/search/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1135 2023-01-28 17:50:13.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)   242525 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/pako.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     3500 2023-03-02 13:48:12.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/search.css
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1782 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/search.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)    13950 2023-01-29 17:52:44.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/search.js
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      947 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/search/search.svg
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.729824 obsidianhtml-3.5.2/obsidianhtml/src/svgs/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/abstract.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/attention.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      479 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/bug.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/caution.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/check.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      535 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/cite.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/danger.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/done.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      275 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/error.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      474 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/example.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      534 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/external.svg
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/fail.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/failure.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/faq.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      247 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/fold.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      545 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/hashtag.svg
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/help.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      390 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/important.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      339 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/info.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      294 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/missing.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      303 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/note.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      348 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/question.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      535 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/quote.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      253 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/success.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/summary.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      390 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/tip.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      480 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/tldr.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      329 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/todo.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      401 2022-04-27 21:48:26.000000 obsidianhtml-3.5.2/obsidianhtml/src/svgs/warning.html
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.729824 obsidianhtml-3.5.2/obsidianhtml/src/tags_page/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      252 2022-06-18 16:13:52.000000 obsidianhtml-3.5.2/obsidianhtml/src/tags_page/button_template.html
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        6 2023-05-15 11:55:58.000000 obsidianhtml-3.5.2/obsidianhtml/src/version
+drwxr-xr-x   0 dorus     (1000) dorus     (1000)        0 2023-05-15 11:56:04.656490 obsidianhtml-3.5.2/obsidianhtml.egg-info/
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1558 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/PKG-INFO
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     7777 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/SOURCES.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)        1 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/dependency_links.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     1061 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/entry_points.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      132 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/requires.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)       13 2023-05-15 11:56:04.000000 obsidianhtml-3.5.2/obsidianhtml.egg-info/top_level.txt
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      807 2022-03-11 21:09:45.000000 obsidianhtml-3.5.2/pypi_readme.md
+-rw-r--r--   0 dorus     (1000) dorus     (1000)      438 2023-02-12 21:35:19.000000 obsidianhtml-3.5.2/pyproject.toml
+-rw-r--r--   0 dorus     (1000) dorus     (1000)     2149 2023-05-15 11:56:04.733157 obsidianhtml-3.5.2/setup.cfg
```

### Comparing `obsidianhtml-3.5.1/LICENSE` & `obsidianhtml-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/PKG-INFO` & `obsidianhtml-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsidianhtml
-Version: 3.5.1
+Version: 3.5.2
 Summary: Converts Obsidian notes into proper markdown and HTML
 Home-page: https://github.com/obsidian-html/obsidian-html
 Author: https://github.com/dwrolvink
 Author-email: dwrolvink@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: html,markdown,notes,markdown-to-html,note-taking,obsidian,html-css-javascript,notes-app,obsidian-md,obsidian-html,obsidianmd,obsidian-notes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/SharedResources.py` & `obsidianhtml-3.5.2/obsidianhtml/SharedResources.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/__init__.py` & `obsidianhtml-3.5.2/obsidianhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/compiler/HTML.py` & `obsidianhtml-3.5.2/obsidianhtml/compiler/HTML.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/compiler/Templating.py` & `obsidianhtml-3.5.2/obsidianhtml/compiler/Templating.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/controller/ConvertVault.py` & `obsidianhtml-3.5.2/obsidianhtml/controller/ConvertVault.py`

 * *Files 1% similar despite different names*

```diff
@@ -208,15 +208,15 @@
 
         # Get node_id
         m = re.search(r"(?<=\{_obsidian_html_node_id_pattern_:)(.*?)(?=\})", html)
         if m is None:
             continue
         node_id = m.group(0)
         node = pb.index.network_tree.node_lookup[node_id]
-        html = re.sub("\{_obsidian_html_node_id_pattern_:" + node_id + "}", "", html)
+        html = re.sub("\{_obsidian_html_node_id_pattern_:" + re.escape(node_id) + "}", "", html)
 
         # Get tags
         tags = md2html.get_tags(node)
 
         # Fill in side pane content
         left_pane = get_side_pane_html(pb, "left_pane", node)
         html = html.replace("{left_pane}", left_pane)
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/controller/Export.py` & `obsidianhtml-3.5.2/obsidianhtml/controller/Export.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/controller/Run.py` & `obsidianhtml-3.5.2/obsidianhtml/controller/Run.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/controller/Serve.py` & `obsidianhtml-3.5.2/obsidianhtml/controller/Serve.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/Actor.py` & `obsidianhtml-3.5.2/obsidianhtml/core/Actor.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/ConfigManager.py` & `obsidianhtml-3.5.2/obsidianhtml/core/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/CopyVault.py` & `obsidianhtml-3.5.2/obsidianhtml/core/CopyVault.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/ErrorHandling.py` & `obsidianhtml-3.5.2/obsidianhtml/core/ErrorHandling.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/FileFinder.py` & `obsidianhtml-3.5.2/obsidianhtml/core/FileFinder.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,26 +16,32 @@
         # the link will be converted to a path that is relative to the root dir.
         output = {}
         output["rtr_path_str"] = ""  # rtr=relative to root
         output["fo"] = False  # file object of type FileObject
         output["header"] = ""  # the last part in 'link#header'
         output["alias"] = ""
 
+        if link is None:
+            return output
+
         # split folder/note#chapter|alias into ('folder/note#chapter', 'alias')
         parts = link.split("|")
         link = parts[0]
         if len(parts) > 1:
             output["alias"] = parts[1]
 
         # split folder/note#chapter into ('folder/note', 'chapter')
         parts = link.split("#")
         link = parts[0]
         if len(parts) > 1:
             output["header"] = "#".join(parts[1:])
 
+        if link == "":
+            return output
+
         # Find file. Values will be False when file is not found.
         output["rtr_path_str"], output["fo"] = self._FindFile(link, html_url_prefix, force_filename_to_lowercase)
 
         if output["fo"] is False and link.startswith("/"):
             output["rtr_path_str"], output["fo"] = self._FindFile(link[1:], html_url_prefix, force_filename_to_lowercase)
 
         if output["fo"] is False and not link.startswith("/"):
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/FileObject.py` & `obsidianhtml-3.5.2/obsidianhtml/core/FileObject.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,18 +198,27 @@
 
     def get_depth(self, mode):
         return self._get_depth(self.path[mode]["file_relative_path"])
 
     def _get_depth(self, rel_path):
         return rel_path.as_posix().count("/")
 
-    def get_link(self, link_type, origin: "FileObject" = None, origin_rel_dst_path_str=None):
+    def get_link(self, link_type, origin: "FileObject" = None, origin_rel_dst_path_str=None, encode_special=True):
         link = self._get_link(link_type, origin, origin_rel_dst_path_str)
+
         if self.pb.gc("toggles/slugify_html_links", cached=True) and link_type == "html":
             return slugify_path(link)
+
+        # when doing a manual url_encode on the entire link returned by this function,
+        # be sure to set encode_special=False to avoid double encoding
+        if encode_special:
+            # escape question mark
+            if link_type == "html":
+                link = link.replace("?", "%3F")
+
         return link
 
     def _get_link(self, link_type, origin: "FileObject" = None, origin_rel_dst_path_str=None):
         # Get origin_rel_dst_path_str
         if origin_rel_dst_path_str is None:
             if origin is not None:
                 origin_rel_dst_path_str = origin.path[link_type]["file_relative_path"].as_posix()
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/Index.py` & `obsidianhtml-3.5.2/obsidianhtml/core/Index.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/NetworkTree.py` & `obsidianhtml-3.5.2/obsidianhtml/core/NetworkTree.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/PicknickBasket.py` & `obsidianhtml-3.5.2/obsidianhtml/core/PicknickBasket.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/Types.py` & `obsidianhtml-3.5.2/obsidianhtml/core/Types.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/core/readme.md` & `obsidianhtml-3.5.2/obsidianhtml/core/readme.md`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/CreateIndexFromDirStructure.py` & `obsidianhtml-3.5.2/obsidianhtml/features/CreateIndexFromDirStructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -299,14 +299,15 @@
 
             excluded_paths = self.pb.gc("toggles/features/create_index_from_dir_structure/exclude_files", cached=True)
             for f in tree["files"]:
                 if self.check_is_folder_note(Path(f["path"])):
                     continue
 
                 rel_path = f["rel_path"][1:]
+                rel_path = rel_path.replace("?", "%3F")
                 file_id = self.html_url_prefix + f["rel_path"]
                 name = set_file_name(f, tab_level)
 
                 if rel_path in excluded_paths:
                     continue
 
                 # get link adjustment code
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/CreateIndexFromTags.py` & `obsidianhtml-3.5.2/obsidianhtml/features/CreateIndexFromTags.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/EmbeddedSearch.py` & `obsidianhtml-3.5.2/obsidianhtml/features/EmbeddedSearch.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/RssFeed.py` & `obsidianhtml-3.5.2/obsidianhtml/features/RssFeed.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/Search.py` & `obsidianhtml-3.5.2/obsidianhtml/features/Search.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/SidePane.py` & `obsidianhtml-3.5.2/obsidianhtml/features/SidePane.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/add_toc_when_missing.py` & `obsidianhtml-3.5.2/obsidianhtml/features/add_toc_when_missing.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/features/post_processing.py` & `obsidianhtml-3.5.2/obsidianhtml/features/post_processing.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/Api.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/Api.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/ConfigChecker.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/ConfigChecker.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/Ledger.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/Ledger.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/Templater.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/Templater.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/WindowManager.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/WindowManager.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/__main__.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/gui/lib.py` & `obsidianhtml-3.5.2/obsidianhtml/gui/lib.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/lib.py` & `obsidianhtml-3.5.2/obsidianhtml/lib.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/AdmonitionExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/AdmonitionExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/BlockLinkExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/BlockLinkExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CallOutExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CallOutExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CodeWrapperExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CodeWrapperExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CustomTableExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CustomTableExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/CustomTocExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/CustomTocExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/DataviewExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/DataviewExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/EmbeddedSearchExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/EmbeddedSearchExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/EraserExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/EraserExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/FootnoteExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/FootnoteExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/FormattingExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/FormattingExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/markdown_extensions/MermaidExtension.py` & `obsidianhtml-3.5.2/obsidianhtml/markdown_extensions/MermaidExtension.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/md2html/__init__.py` & `obsidianhtml-3.5.2/obsidianhtml/md2html/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
             md.links.append(link.fo)
 
             # [11.1] Rewrite .md links to .html (when the link is to a file in our root folder)
             query_part = ""
             if link.query != "":
                 query_part = link.query_delimiter + link.query
-            new_link = f']({urllib.parse.quote(link.fo.get_link("html", origin=fo))}{query_part})'
+            new_link = f']({urllib.parse.quote(link.fo.get_link("html", origin=fo, encode_special=False))}{query_part})'
 
         # Update link
         safe_link = re.escape("](" + ol + ")")
         md.page = re.sub(safe_link, new_link, md.page)
 
 
     # [?] Handle local source tag-links (copy them over to output)
@@ -172,15 +172,15 @@
             continue
 
         # Copy src to dst
         if lo.path["markdown"]["file_absolute_path"].exists():
             lo.copy_file("mth")
 
         # [11.2] Adjust video link in page to new dst folder (when the link is to a file in our root folder)
-        new_link = template.replace("{link}", urllib.parse.quote(lo.get_link("html", origin=fo)))
+        new_link = template.replace("{link}", urllib.parse.quote(lo.get_link("html", origin=fo, encode_special=False)))
         safe_link = re.escape(tag)
         md.page = re.sub(safe_link, new_link, md.page)
 
     # [?] Handle local embeddable tag-links (copy them over to output)
     # ------------------------------------------------------------------
     for link in re.findall(r'(?<=<embed src=")([^"]*)', md.page):
         l = urllib.parse.unquote(link)
@@ -193,15 +193,15 @@
                 warnings.warn(f"Media {l} treated as external and not imported in html")
             continue
 
         # Copy src to dst
         lo.copy_file("mth")
 
         # [11.2] Adjust video link in page to new dst folder (when the link is to a file in our root folder)
-        new_link = '<embed src="' + urllib.parse.quote(lo.get_link("html", origin=fo)) + '"'
+        new_link = '<embed src="' + urllib.parse.quote(lo.get_link("html", origin=fo, encode_special=False)) + '"'
         safe_link = r'<embed src="' + re.escape(link) + r'"'
         md.page = re.sub(safe_link, new_link, md.page)
 
     # [?] Documentation styling: Table of Contents
     # ------------------------------------------------------------------
     if get_side_pane_id_by_content_selector(pb, "toc") or gc_add_toc_when_missing(pb, fo):
         # convert the common [[_TOC_]] into [TOC]
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/note2md/__init__.py` & `obsidianhtml-3.5.2/obsidianhtml/note2md/__init__.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/parser/HeaderTree.py` & `obsidianhtml-3.5.2/obsidianhtml/parser/HeaderTree.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/parser/MarkdownLink.py` & `obsidianhtml-3.5.2/obsidianhtml/parser/MarkdownLink.py`

 * *Files 7% similar despite different names*

```diff
@@ -66,14 +66,17 @@
 
         if len(url.split("#")) > 1:
             self.url = url.split("#")[0]
             self.query = url.split("#", 1)[1]
             self.query_delimiter = "#"
             return
         if len(url.split("?")) > 1:
+            # if url ends with .md, the ? is not a query identifier
+            if url.endswith(".md"):
+                return
             self.url = url.split("?")[0]
             self.query = url.split("?", 1)[1]
             self.query_delimiter = "?"
             return
 
     def TestisValid(self):
         if self.url == "":
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml/parser/MarkdownPage.py` & `obsidianhtml-3.5.2/obsidianhtml/parser/MarkdownPage.py`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/defaults_config.yml` & `obsidianhtml-3.5.2/obsidianhtml/src/defaults_config.yml`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_2d.js` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_2d.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_3d.js` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_3d.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/default_grapher_node_graph.html` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/default_grapher_node_graph.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.css` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.js` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/graph.svg` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/graph.svg`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/graph_full_page.html` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/graph_full_page.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/graph/graph_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/graph/graph_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/help_texts/export_help_text` & `obsidianhtml-3.5.2/obsidianhtml/src/help_texts/export_help_text`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/help_texts/help_text` & `obsidianhtml-3.5.2/obsidianhtml/src/help_texts/help_text`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/callouts.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/callouts.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/codehilite.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/codehilite.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/global_main.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/global_main.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/global_overwrites.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/global_overwrites.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/master.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/master.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/css/mermaid.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/css/mermaid.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/favicon.ico` & `obsidianhtml-3.5.2/obsidianhtml/src/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/fonts/Roboto-Regular.ttf` & `obsidianhtml-3.5.2/obsidianhtml/src/html/fonts/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/fonts/SourceCodePro-Regular.ttf` & `obsidianhtml-3.5.2/obsidianhtml/src/html/fonts/SourceCodePro-Regular.ttf`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_documentation.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_documentation.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_minimal.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_minimal.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/main_tabs.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/main_tabs.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_documentation.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_documentation.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_minimal.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_minimal.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/layouts/template_tabs.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/layouts/template_tabs.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/templates/full_header.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/templates/full_header.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/templates/minimal_header.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/templates/minimal_header.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/themes/button_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/html/themes/button_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/html/themes/theme-obsidian.css` & `obsidianhtml-3.5.2/obsidianhtml/src/html/themes/theme-obsidian.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/imported/3d-force-graph.v1.70.10.min.js` & `obsidianhtml-3.5.2/obsidianhtml/src/imported/3d-force-graph.v1.70.10.min.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/imported/flexsearch.v0.7.2.bundle.js` & `obsidianhtml-3.5.2/obsidianhtml/src/imported/flexsearch.v0.7.2.bundle.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/imported/mathjax.v3.es5.tex-chtml.js` & `obsidianhtml-3.5.2/obsidianhtml/src/imported/mathjax.v3.es5.tex-chtml.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/imported/mermaid.9.0.1.min.js` & `obsidianhtml-3.5.2/obsidianhtml/src/imported/mermaid.9.0.1.min.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/imported/mermaid.9.0.1.min.js.map` & `obsidianhtml-3.5.2/obsidianhtml/src/imported/mermaid.9.0.1.min.js.map`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/configurations.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/configurations.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/gp_installer.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/gp_installer.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/index.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/index.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/init.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/init.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/setup_gitpages.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/setup_gitpages.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/dist/test.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/dist/test.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/components/select-entrypoint-path.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/components/select-entrypoint-path.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/components/select-vault-path.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/components/select-vault-path.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/configurations_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/configurations_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/gp_installer_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/gp_installer_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/index_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/index_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/init_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/init_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/setup_gitpages_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/setup_gitpages_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/html/test_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/html/test_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/js/core.js` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/js/core.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/action_components.css` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/action_components.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/flex.css` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/flex.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/main.css` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/main.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/installer/units/style/response.css` & `obsidianhtml-3.5.2/obsidianhtml/src/installer/units/style/response.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/js/encoding.js` & `obsidianhtml-3.5.2/obsidianhtml/src/js/encoding.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/js/load_dirtree_footer.js` & `obsidianhtml-3.5.2/obsidianhtml/src/js/load_dirtree_footer.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/js/obsidian_core.js` & `obsidianhtml-3.5.2/obsidianhtml/src/js/obsidian_core.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/js/obsidian_tabs_footer.js` & `obsidianhtml-3.5.2/obsidianhtml/src/js/obsidian_tabs_footer.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/rss/channel_template.xml` & `obsidianhtml-3.5.2/obsidianhtml/src/rss/channel_template.xml`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/rss/rss.svg` & `obsidianhtml-3.5.2/obsidianhtml/src/rss/rss.svg`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/button_template.html` & `obsidianhtml-3.5.2/obsidianhtml/src/search/button_template.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/pako.js` & `obsidianhtml-3.5.2/obsidianhtml/src/search/pako.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/search.css` & `obsidianhtml-3.5.2/obsidianhtml/src/search/search.css`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/search.html` & `obsidianhtml-3.5.2/obsidianhtml/src/search/search.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/search.js` & `obsidianhtml-3.5.2/obsidianhtml/src/search/search.js`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/search/search.svg` & `obsidianhtml-3.5.2/obsidianhtml/src/search/search.svg`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/svgs/cite.html` & `obsidianhtml-3.5.2/obsidianhtml/src/svgs/cite.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/svgs/external.svg` & `obsidianhtml-3.5.2/obsidianhtml/src/svgs/external.svg`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/svgs/hashtag.svg` & `obsidianhtml-3.5.2/obsidianhtml/src/svgs/hashtag.svg`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml/src/svgs/quote.html` & `obsidianhtml-3.5.2/obsidianhtml/src/svgs/quote.html`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml.egg-info/PKG-INFO` & `obsidianhtml-3.5.2/obsidianhtml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: obsidianhtml
-Version: 3.5.1
+Version: 3.5.2
 Summary: Converts Obsidian notes into proper markdown and HTML
 Home-page: https://github.com/obsidian-html/obsidian-html
 Author: https://github.com/dwrolvink
 Author-email: dwrolvink@protonmail.com
 License: GNU General Public License v3 or later (GPLv3+)
 Keywords: html,markdown,notes,markdown-to-html,note-taking,obsidian,html-css-javascript,notes-app,obsidian-md,obsidian-html,obsidianmd,obsidian-notes
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `obsidianhtml-3.5.1/obsidianhtml.egg-info/SOURCES.txt` & `obsidianhtml-3.5.2/obsidianhtml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/obsidianhtml.egg-info/entry_points.txt` & `obsidianhtml-3.5.2/obsidianhtml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/pypi_readme.md` & `obsidianhtml-3.5.2/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `obsidianhtml-3.5.1/setup.cfg` & `obsidianhtml-3.5.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = obsidianhtml
-version = 3.5.1
+version = 3.5.2
 summary = Converts Obsidian notes into proper markdown and HTML
 long_description = file: pypi_readme.md
 home_page = https://github.com/obsidian-html/obsidian-html
 author = https://github.com/dwrolvink
 author_email = dwrolvink@protonmail.com
 license = GNU General Public License v3 or later (GPLv3+)
 classifiers =
```

