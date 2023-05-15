# Comparing `tmp/browserist-1.4.5.tar.gz` & `tmp/browserist-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserist-1.4.5.tar", last modified: Mon Apr 24 17:22:11 2023, max compression
+gzip compressed data, was "browserist-1.4.6.tar", last modified: Mon May 15 15:41:06 2023, max compression
```

## Comparing `browserist-1.4.5.tar` & `browserist-1.4.6.tar`

### file list

```diff
@@ -1,313 +1,313 @@
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.758074 browserist-1.4.5/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2102 2023-04-24 17:20:50.000000 browserist-1.4.5/INSTALLATION.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    11343 2023-01-25 13:58:31.000000 browserist-1.4.5/LICENSE.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 09:20:52.000000 browserist-1.4.5/MANIFEST.in
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24590 2023-04-24 17:22:11.758236 browserist-1.4.5/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    10161 2023-04-24 17:20:50.000000 browserist-1.4.5/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      141 2023-02-03 11:49:45.000000 browserist-1.4.5/pyproject.toml
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1823 2023-04-24 17:22:11.758642 browserist-1.4.5/setup.cfg
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.715509 browserist-1.4.5/src/
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.720178 browserist-1.4.5/src/browserist/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1016 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.721598 browserist-1.4.5/src/browserist/browser/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4622 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.723763 browserist-1.4.5/src/browserist/browser/check_if/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3008 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      447 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/contains_any_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/contains_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      400 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/does_exist.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      506 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_clickable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      299 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_disabled.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      427 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_displayed.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      423 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_enabled.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_image_loaded.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      999 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/check_if/is_in_viewport.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.724430 browserist-1.4.5/src/browserist/browser/click/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/click/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1017 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/click/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      721 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/click/button.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1094 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/click/button_if_contains_text.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.725122 browserist-1.4.5/src/browserist/browser/combo/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/combo/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1815 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/combo/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1619 2023-02-01 06:40:37.000000 browserist-1.4.5/src/browserist/browser/combo/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3071 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/combo/log_in.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1440 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/combo/search.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.726248 browserist-1.4.5/src/browserist/browser/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3275 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.726882 browserist-1.4.5/src/browserist/browser/get/attribute/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/attribute/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1414 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/attribute/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      505 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/attribute/value.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/attribute/values.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      639 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/dimensions.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      732 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      749 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/elements.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/elements_by_tag.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      199 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/page_title.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      491 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/texts.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.728255 browserist-1.4.5/src/browserist/browser/get/url/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2690 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/browser/get/url/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      207 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/current.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      270 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/browser/get/url/current_domain.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      683 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/from_image.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/from_images.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      685 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/from_link.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/get/url/from_links.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.728738 browserist-1.4.5/src/browserist/browser/iframe/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/iframe/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      858 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/iframe/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      533 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/iframe/switch_to.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      224 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/iframe/switch_to_original_page.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.729432 browserist-1.4.5/src/browserist/browser/input/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/input/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/input/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      495 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/input/clear.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      461 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/input/select.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      588 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/input/value.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.729803 browserist-1.4.5/src/browserist/browser/mouse/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/mouse/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/mouse/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      642 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/mouse/hover.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.730295 browserist-1.4.5/src/browserist/browser/open/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/open/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1229 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/open/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      253 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/open/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      986 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/open/url_if_not_current.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.730916 browserist-1.4.5/src/browserist/browser/prompt/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/prompt/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1092 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/prompt/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      474 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/prompt/input_value.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      647 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/prompt/proceed_yes_or_no.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.731740 browserist-1.4.5/src/browserist/browser/screenshot/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3403 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/screenshot/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1116 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/browser/screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      992 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/browser/screenshot/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      796 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/browser/screenshot/visible_portion.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.733046 browserist-1.4.5/src/browserist/browser/scroll/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     4040 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      373 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.733566 browserist-1.4.5/src/browserist/browser/scroll/check_if/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/check_if/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      872 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/check_if/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      725 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/check_if/is_end_of_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/check_if/is_top_of_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      238 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/down_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.734062 browserist-1.4.5/src/browserist/browser/scroll/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      825 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/get/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      545 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/get/total_height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/into_view.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      483 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/into_view_if_not_visible.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/left_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.734881 browserist-1.4.5/src/browserist/browser/scroll/page/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1559 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      384 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/down.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1354 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/to_end.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      251 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/to_top.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      385 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/page/up.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/right_by.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/to_position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      237 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/scroll/up_by.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.735489 browserist-1.4.5/src/browserist/browser/tool/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/tool/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1472 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/tool/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      454 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/tool/count_elements.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/tool/execute_script.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      216 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/tool/is_input_valid.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.735751 browserist-1.4.5/src/browserist/browser/viewport/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/__main__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.736342 browserist-1.4.5/src/browserist/browser/viewport/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1061 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      248 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/get/height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      330 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/get/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      246 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/get/width.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.736880 browserist-1.4.5/src/browserist/browser/viewport/set/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/set/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1312 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/set/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      982 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/set/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      318 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/viewport/set/size_by_device.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.737491 browserist-1.4.5/src/browserist/browser/wait/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1513 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1667 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/for_element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      158 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/random_seconds.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/seconds.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.738380 browserist-1.4.5/src/browserist/browser/wait/until/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2791 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      467 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/contains_any_text.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      446 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/element_disappears.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      829 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/images_have_loaded.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      438 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/is_clickable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1231 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/number_of_window_handles_is.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.739007 browserist-1.4.5/src/browserist/browser/wait/until/page_title/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/page_title/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1658 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/page_title/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/page_title/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1200 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/until/page_title/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1156 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/until/page_title/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.739630 browserist-1.4.5/src/browserist/browser/wait/until/text/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/text/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1570 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/text/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      722 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/text/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/text/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      742 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/text/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.740421 browserist-1.4.5/src/browserist/browser/wait/until/url/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/url/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/url/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/wait/until/url/changes.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1121 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/until/url/contains.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1137 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/browser/wait/until/url/equals.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.741480 browserist-1.4.5/src/browserist/browser/window/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2857 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      479 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/close.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      210 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/fullscreen.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.742244 browserist-1.4.5/src/browserist/browser/window/get/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1456 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/height.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      327 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      320 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      232 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/get/width.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.742840 browserist-1.4.5/src/browserist/browser/window/handle/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/handle/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1617 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/handle/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      449 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/handle/all.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      403 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/handle/count.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      227 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/handle/current.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/maximize.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/minimize.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.743299 browserist-1.4.5/src/browserist/browser/window/open/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/open/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1599 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/open/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1307 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/open/new_tab_or_window.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.743872 browserist-1.4.5/src/browserist/browser/window/set/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/set/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      793 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/set/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      235 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/set/position.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/set/size.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      573 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/browser/window/switch_to.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.744763 browserist-1.4.5/src/browserist/constant/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-01 06:40:45.000000 browserist-1.4.5/src/browserist/constant/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/constant/directory.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       60 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/constant/interval.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       48 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/constant/screenshot.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      249 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/constant/timeout.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.746278 browserist-1.4.5/src/browserist/exception/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1392 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/element.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      273 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/file_png.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      723 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/headless.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      437 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/retry.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      250 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/scroll.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1821 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/timeout.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      254 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1762 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/window_handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      262 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/exception/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.747196 browserist-1.4.5/src/browserist/factory/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      129 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/factory/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      646 2023-04-10 10:57:16.000000 browserist-1.4.5/src/browserist/factory/chromium.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1170 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/factory/get.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      944 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/factory/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      887 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/factory/safari.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      717 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/factory/set.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.749209 browserist-1.4.5/src/browserist/helper/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      309 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/helper/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/date_time.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/directory.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      460 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/file.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1418 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/image.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       83 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/operating_system.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/helper/regex.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      468 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/helper/terminal.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/timeout.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1591 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/helper/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      272 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper/viewport.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      626 2023-03-20 06:14:36.000000 browserist-1.4.5/src/browserist/helper/window_handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      934 2023-02-01 06:40:45.000000 browserist-1.4.5/src/browserist/helper/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.749596 browserist-1.4.5/src/browserist/helper_iteration/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       41 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper_iteration/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2796 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper_iteration/retry.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.750229 browserist-1.4.5/src/browserist/helper_screenshot/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      976 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper_screenshot/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3489 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/helper_screenshot/complete_page.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1422 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/helper_screenshot/controller.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1420 2023-03-17 10:25:47.000000 browserist-1.4.5/src/browserist/helper_screenshot/file.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.750663 browserist-1.4.5/src/browserist/model/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.751806 browserist-1.4.5/src/browserist/model/browser/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      636 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/README.md
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.752530 browserist-1.4.5/src/browserist/model/browser/base/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3329 2023-04-10 12:04:38.000000 browserist-1.4.5/src/browserist/model/browser/base/driver.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      459 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/page_load_strategy.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1854 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/settings.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.752984 browserist-1.4.5/src/browserist/model/browser/base/timeout/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/timeout/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      684 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/timeout/settings.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/timeout/strategy.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      283 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/base/type.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      973 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/chrome.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1401 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/edge.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.753634 browserist-1.4.5/src/browserist/model/browser/extension/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/extension/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      601 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/extension/__main__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      439 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/extension/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      407 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/extension/safari.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1176 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/browser/firefox.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1014 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/internet_explorer.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1001 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/opera.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1006 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/browser/safari.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.754746 browserist-1.4.5/src/browserist/model/combo_settings/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/combo_settings/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1184 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/combo_settings/cookie_banner.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      289 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/combo_settings/login_credentials.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     2770 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/combo_settings/login_form.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1105 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/combo_settings/search.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      987 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/driver_methods.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3215 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/screenshot.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.756053 browserist-1.4.5/src/browserist/model/type/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/type/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      507 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/type/callable.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      823 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/type/file_png.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/type/path.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      773 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/type/url.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      811 2023-02-01 06:40:45.000000 browserist-1.4.5/src/browserist/model/type/xpath.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.756626 browserist-1.4.5/src/browserist/model/viewport/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/viewport/__init__.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.757383 browserist-1.4.5/src/browserist/model/viewport/collection/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/viewport/collection/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     1080 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/viewport/collection/apple.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      271 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/viewport/collection/google.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/viewport/collection/microsoft.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      333 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/viewport/collection/samsung.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      285 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/viewport/common_devices.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      208 2023-02-03 11:49:45.000000 browserist-1.4.5/src/browserist/model/viewport/device.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.757933 browserist-1.4.5/src/browserist/model/window/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/window/__init__.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)     3231 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/window/controller.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/window/handle.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:58:31.000000 browserist-1.4.5/src/browserist/model/window/tab_or_window.py
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 15:16:10.000000 browserist-1.4.5/src/browserist/py.typed
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-04-24 17:20:56.000000 browserist-1.4.5/src/browserist/version.py
-drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-04-24 17:22:11.721083 browserist-1.4.5/src/browserist.egg-info/
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    24590 2023-04-24 17:22:11.000000 browserist-1.4.5/src/browserist.egg-info/PKG-INFO
--rw-r--r--   0 jakobbagterp   (501) staff       (20)    11183 2023-04-24 17:22:11.000000 browserist-1.4.5/src/browserist.egg-info/SOURCES.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-04-24 17:22:11.000000 browserist-1.4.5/src/browserist.egg-info/dependency_links.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-25 15:10:37.000000 browserist-1.4.5/src/browserist.egg-info/not-zip-safe
--rw-r--r--   0 jakobbagterp   (501) staff       (20)      169 2023-04-24 17:22:11.000000 browserist-1.4.5/src/browserist.egg-info/requires.txt
--rw-r--r--   0 jakobbagterp   (501) staff       (20)       11 2023-04-24 17:22:11.000000 browserist-1.4.5/src/browserist.egg-info/top_level.txt
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.833142 browserist-1.4.6/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2198 2023-05-15 15:36:51.000000 browserist-1.4.6/INSTALLATION.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    11343 2023-01-25 13:58:31.000000 browserist-1.4.6/LICENSE.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      217 2023-04-02 09:20:52.000000 browserist-1.4.6/MANIFEST.in
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24782 2023-05-15 15:41:06.833332 browserist-1.4.6/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    10257 2023-05-15 15:36:57.000000 browserist-1.4.6/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      141 2023-02-03 11:49:45.000000 browserist-1.4.6/pyproject.toml
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1822 2023-05-15 15:41:06.833753 browserist-1.4.6/setup.cfg
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.778807 browserist-1.4.6/src/
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.783152 browserist-1.4.6/src/browserist/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1016 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.784872 browserist-1.4.6/src/browserist/browser/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4622 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.787665 browserist-1.4.6/src/browserist/browser/check_if/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3008 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      447 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/contains_any_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/contains_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      400 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/does_exist.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      506 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      299 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_disabled.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      427 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_displayed.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      423 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_enabled.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      504 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_image_loaded.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      999 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/check_if/is_in_viewport.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.788286 browserist-1.4.6/src/browserist/browser/click/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/click/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1017 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/click/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      721 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/click/button.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1094 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/click/button_if_contains_text.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.789041 browserist-1.4.6/src/browserist/browser/combo/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/combo/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1815 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/combo/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1619 2023-02-01 06:40:37.000000 browserist-1.4.6/src/browserist/browser/combo/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3071 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/combo/log_in.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1440 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/combo/search.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.790454 browserist-1.4.6/src/browserist/browser/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3275 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.791076 browserist-1.4.6/src/browserist/browser/get/attribute/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/attribute/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1414 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/attribute/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      505 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/attribute/value.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/attribute/values.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      639 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/dimensions.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      732 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      749 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/elements.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/elements_by_tag.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      199 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/page_title.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      491 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/texts.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.792668 browserist-1.4.6/src/browserist/browser/get/url/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2690 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/browser/get/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      207 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/current.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      270 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/browser/get/url/current_domain.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      683 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/from_image.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/from_images.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      685 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/from_link.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      342 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/get/url/from_links.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.793328 browserist-1.4.6/src/browserist/browser/iframe/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/iframe/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      858 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/iframe/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      533 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/iframe/switch_to.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      224 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/iframe/switch_to_original_page.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.794016 browserist-1.4.6/src/browserist/browser/input/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/input/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/input/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      495 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/input/clear.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      461 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/input/select.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      588 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/input/value.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.794544 browserist-1.4.6/src/browserist/browser/mouse/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/mouse/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/mouse/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      642 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/mouse/hover.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.795159 browserist-1.4.6/src/browserist/browser/open/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1229 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      253 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/open/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      986 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/open/url_if_not_current.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.795865 browserist-1.4.6/src/browserist/browser/prompt/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/prompt/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1092 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/prompt/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      474 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/prompt/input_value.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      647 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/prompt/proceed_yes_or_no.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.797141 browserist-1.4.6/src/browserist/browser/screenshot/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3403 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/screenshot/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1116 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/browser/screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      992 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/browser/screenshot/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      796 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/browser/screenshot/visible_portion.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.798613 browserist-1.4.6/src/browserist/browser/scroll/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     4040 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      373 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.799140 browserist-1.4.6/src/browserist/browser/scroll/check_if/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/check_if/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      872 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/check_if/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      725 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/check_if/is_end_of_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/check_if/is_top_of_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      238 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/down_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.799700 browserist-1.4.6/src/browserist/browser/scroll/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      825 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/get/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      545 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/get/total_height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      681 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/into_view.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      483 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/into_view_if_not_visible.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/left_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.800516 browserist-1.4.6/src/browserist/browser/scroll/page/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1559 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      384 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/down.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1354 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/to_end.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      251 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/to_top.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      385 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/page/up.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      239 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/right_by.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      382 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/to_position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      237 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/scroll/up_by.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.801263 browserist-1.4.6/src/browserist/browser/tool/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/tool/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1472 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/tool/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      454 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/tool/count_elements.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      347 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/tool/execute_script.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      216 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/tool/is_input_valid.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.801518 browserist-1.4.6/src/browserist/browser/viewport/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      561 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/__main__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.802200 browserist-1.4.6/src/browserist/browser/viewport/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1061 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      248 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/get/height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      330 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/get/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      246 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/get/width.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.802843 browserist-1.4.6/src/browserist/browser/viewport/set/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1312 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      982 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/set/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      318 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/viewport/set/size_by_device.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.803546 browserist-1.4.6/src/browserist/browser/wait/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1513 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1667 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/for_element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      158 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/random_seconds.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/seconds.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.804635 browserist-1.4.6/src/browserist/browser/wait/until/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2791 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      467 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/contains_any_text.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      446 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/element_disappears.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      829 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/images_have_loaded.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      438 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/is_clickable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1231 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/number_of_window_handles_is.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.805357 browserist-1.4.6/src/browserist/browser/wait/until/page_title/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/page_title/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1658 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/page_title/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      542 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/page_title/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1200 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/until/page_title/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1156 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/until/page_title/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.806035 browserist-1.4.6/src/browserist/browser/wait/until/text/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/text/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1570 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/text/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      722 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/text/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/text/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      742 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/text/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.806840 browserist-1.4.6/src/browserist/browser/wait/until/url/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/url/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1622 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/url/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      593 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/wait/until/url/changes.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1121 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/until/url/contains.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1137 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/browser/wait/until/url/equals.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.808570 browserist-1.4.6/src/browserist/browser/window/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2857 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      479 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/close.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      210 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/fullscreen.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.810029 browserist-1.4.6/src/browserist/browser/window/get/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1456 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/height.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      327 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      320 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      232 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/get/width.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.810696 browserist-1.4.6/src/browserist/browser/window/handle/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/handle/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1617 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/handle/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      449 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/handle/all.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      403 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/handle/count.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      227 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/handle/current.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/maximize.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      206 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/minimize.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.811438 browserist-1.4.6/src/browserist/browser/window/open/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/open/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1599 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/open/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1307 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/open/new_tab_or_window.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.812267 browserist-1.4.6/src/browserist/browser/window/set/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/set/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      793 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/set/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      235 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/set/position.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      245 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/set/size.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      573 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/browser/window/switch_to.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.813067 browserist-1.4.6/src/browserist/constant/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-01 06:40:45.000000 browserist-1.4.6/src/browserist/constant/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       97 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/constant/directory.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       60 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/constant/interval.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       48 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/constant/screenshot.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      249 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/constant/timeout.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.814750 browserist-1.4.6/src/browserist/exception/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1392 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/element.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      273 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/file_png.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      723 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/headless.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      437 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/retry.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      250 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/scroll.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1821 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/timeout.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      254 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1762 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/window_handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      262 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/exception/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.816239 browserist-1.4.6/src/browserist/factory/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      129 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/factory/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      646 2023-04-10 10:57:16.000000 browserist-1.4.6/src/browserist/factory/chromium.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1170 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/factory/get.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      944 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/factory/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      887 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/factory/safari.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      717 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/factory/set.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.819271 browserist-1.4.6/src/browserist/helper/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      309 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/helper/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      416 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/date_time.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1220 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/directory.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      460 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/file.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1418 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/image.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       83 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/operating_system.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      117 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/helper/regex.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      468 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/helper/terminal.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      590 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/timeout.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1591 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/helper/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      272 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper/viewport.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      626 2023-03-20 06:14:36.000000 browserist-1.4.6/src/browserist/helper/window_handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      934 2023-02-01 06:40:45.000000 browserist-1.4.6/src/browserist/helper/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.820049 browserist-1.4.6/src/browserist/helper_iteration/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       41 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper_iteration/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2796 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper_iteration/retry.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.821849 browserist-1.4.6/src/browserist/helper_screenshot/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      976 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper_screenshot/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3489 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/helper_screenshot/complete_page.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1422 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/helper_screenshot/controller.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1420 2023-03-17 10:25:47.000000 browserist-1.4.6/src/browserist/helper_screenshot/file.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.823015 browserist-1.4.6/src/browserist/model/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.824496 browserist-1.4.6/src/browserist/model/browser/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      636 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/README.md
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.825383 browserist-1.4.6/src/browserist/model/browser/base/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3329 2023-04-10 12:04:38.000000 browserist-1.4.6/src/browserist/model/browser/base/driver.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      459 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/page_load_strategy.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1854 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/settings.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.826853 browserist-1.4.6/src/browserist/model/browser/base/timeout/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/timeout/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      684 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/timeout/settings.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/timeout/strategy.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      283 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/base/type.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      973 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/chrome.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1401 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/edge.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.827512 browserist-1.4.6/src/browserist/model/browser/extension/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/extension/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      601 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/extension/__main__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      439 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/extension/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      407 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/extension/safari.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1176 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/browser/firefox.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1014 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/internet_explorer.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1001 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/opera.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1006 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/browser/safari.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.828814 browserist-1.4.6/src/browserist/model/combo_settings/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/combo_settings/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1184 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/combo_settings/cookie_banner.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      289 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/combo_settings/login_credentials.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     2770 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/combo_settings/login_form.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1105 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/combo_settings/search.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      987 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/driver_methods.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3215 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/screenshot.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.830515 browserist-1.4.6/src/browserist/model/type/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/type/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      507 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/type/callable.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      823 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/type/file_png.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      789 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/type/path.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      773 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/type/url.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      811 2023-02-01 06:40:45.000000 browserist-1.4.6/src/browserist/model/type/xpath.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.831170 browserist-1.4.6/src/browserist/model/viewport/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/viewport/__init__.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.832267 browserist-1.4.6/src/browserist/model/viewport/collection/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/viewport/collection/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     1080 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/viewport/collection/apple.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      271 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/viewport/collection/google.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      234 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/viewport/collection/microsoft.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      333 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/viewport/collection/samsung.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      285 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/viewport/common_devices.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      208 2023-02-03 11:49:45.000000 browserist-1.4.6/src/browserist/model/viewport/device.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.832933 browserist-1.4.6/src/browserist/model/window/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       24 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/window/__init__.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)     3231 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/window/controller.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      261 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/window/handle.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      212 2023-01-25 13:58:31.000000 browserist-1.4.6/src/browserist/model/window/tab_or_window.py
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        0 2023-01-25 15:16:10.000000 browserist-1.4.6/src/browserist/py.typed
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       80 2023-05-15 15:37:02.000000 browserist-1.4.6/src/browserist/version.py
+drwxr-xr-x   0 jakobbagterp   (501) staff       (20)        0 2023-05-15 15:41:06.784445 browserist-1.4.6/src/browserist.egg-info/
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    24782 2023-05-15 15:41:06.000000 browserist-1.4.6/src/browserist.egg-info/PKG-INFO
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)    11183 2023-05-15 15:41:06.000000 browserist-1.4.6/src/browserist.egg-info/SOURCES.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-05-15 15:41:06.000000 browserist-1.4.6/src/browserist.egg-info/dependency_links.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)        1 2023-01-25 15:10:37.000000 browserist-1.4.6/src/browserist.egg-info/not-zip-safe
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)      168 2023-05-15 15:41:06.000000 browserist-1.4.6/src/browserist.egg-info/requires.txt
+-rw-r--r--   0 jakobbagterp   (501) staff       (20)       11 2023-05-15 15:41:06.000000 browserist-1.4.6/src/browserist.egg-info/top_level.txt
```

### Comparing `browserist-1.4.5/INSTALLATION.md` & `browserist-1.4.6/INSTALLATION.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
 * Relevant browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
```

### Comparing `browserist-1.4.5/LICENSE.md` & `browserist-1.4.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/PKG-INFO` & `browserist-1.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.4.5
+Version: 1.4.6
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://github.com/jakob-bagterp/browserist
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: Apache-2.0
@@ -22,19 +22,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 Browserist Extension for Selenium 👨‍💻
 > **browserist**
 > 1. The belief that web browsers account for differences in websites or web applications in all of their ability and that a particular web browser is superior to others.
 > 2. Discrimination or prejudice based on web browser.
 
 Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the Selenium web driver that makes it even easier to use different browsers for testing and automation.
@@ -209,19 +210,20 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/browserist/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/browserist/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
 * Relevant browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
```

### Comparing `browserist-1.4.5/README.md` & `browserist-1.4.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 Browserist Extension for Selenium 👨‍💻
 > **browserist**
 > 1. The belief that web browsers account for differences in websites or web applications in all of their ability and that a particular web browser is superior to others.
 > 2. Discrimination or prejudice based on web browser.
 
 Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the Selenium web driver that makes it even easier to use different browsers for testing and automation.
```

### Comparing `browserist-1.4.5/setup.cfg` & `browserist-1.4.6/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -31,32 +31,32 @@
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.10
 setup_requires = 
 	lxml ==4.9.2
 	pillow ==9.5.0
-	selenium ==4.9.0
+	selenium ==4.9.1
 install_requires = 
 	chromedriver
 	lxml ==4.9.2
 	pillow ==9.5.0
-	selenium ==4.9.0
+	selenium ==4.9.1
 zip_safe = no
 include_package_data = True
 
 [options.extras_require]
 testing = 
-	coverage ==7.2.3
+	coverage ==7.2.5
 	flake8 ==6.0.0
 	keyring ==23.13.1
-	mypy ==1.2.0
+	mypy ==1.3.0
 	pytest ==7.3.1
 	pytest-cov ==4.0.0
-	tox ==4.4.12
+	tox ==4.5.1
 
 [options.packages.find]
 where = src
 
 [options.package_data]
 browserist = py.typed
```

### Comparing `browserist-1.4.5/src/browserist/__init__.py` & `browserist-1.4.6/src/browserist/__init__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/__main__.py` & `browserist-1.4.6/src/browserist/browser/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/check_if/__main__.py` & `browserist-1.4.6/src/browserist/browser/check_if/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/check_if/contains_text.py` & `browserist-1.4.6/src/browserist/browser/check_if/contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/check_if/is_in_viewport.py` & `browserist-1.4.6/src/browserist/browser/check_if/is_in_viewport.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/click/__main__.py` & `browserist-1.4.6/src/browserist/browser/click/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/click/button.py` & `browserist-1.4.6/src/browserist/browser/click/button.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/click/button_if_contains_text.py` & `browserist-1.4.6/src/browserist/browser/click/button_if_contains_text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/combo/__main__.py` & `browserist-1.4.6/src/browserist/browser/combo/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/combo/cookie_banner.py` & `browserist-1.4.6/src/browserist/browser/combo/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/combo/log_in.py` & `browserist-1.4.6/src/browserist/browser/combo/log_in.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/combo/search.py` & `browserist-1.4.6/src/browserist/browser/combo/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/__main__.py` & `browserist-1.4.6/src/browserist/browser/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/attribute/__main__.py` & `browserist-1.4.6/src/browserist/browser/get/attribute/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/attribute/values.py` & `browserist-1.4.6/src/browserist/browser/get/attribute/values.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/dimensions.py` & `browserist-1.4.6/src/browserist/browser/get/dimensions.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/element.py` & `browserist-1.4.6/src/browserist/browser/get/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/elements.py` & `browserist-1.4.6/src/browserist/browser/get/elements.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/text.py` & `browserist-1.4.6/src/browserist/browser/get/text.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/url/__main__.py` & `browserist-1.4.6/src/browserist/browser/get/url/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/url/from_image.py` & `browserist-1.4.6/src/browserist/browser/get/url/from_image.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/get/url/from_link.py` & `browserist-1.4.6/src/browserist/browser/get/url/from_link.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/iframe/__main__.py` & `browserist-1.4.6/src/browserist/browser/iframe/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/iframe/switch_to.py` & `browserist-1.4.6/src/browserist/browser/iframe/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/input/__main__.py` & `browserist-1.4.6/src/browserist/browser/input/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/input/value.py` & `browserist-1.4.6/src/browserist/browser/input/value.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/mouse/__main__.py` & `browserist-1.4.6/src/browserist/browser/mouse/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/mouse/hover.py` & `browserist-1.4.6/src/browserist/browser/mouse/hover.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/open/__main__.py` & `browserist-1.4.6/src/browserist/browser/open/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/open/url_if_not_current.py` & `browserist-1.4.6/src/browserist/browser/open/url_if_not_current.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/prompt/__main__.py` & `browserist-1.4.6/src/browserist/browser/prompt/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/prompt/proceed_yes_or_no.py` & `browserist-1.4.6/src/browserist/browser/prompt/proceed_yes_or_no.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/screenshot/__main__.py` & `browserist-1.4.6/src/browserist/browser/screenshot/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/screenshot/complete_page.py` & `browserist-1.4.6/src/browserist/browser/screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/screenshot/element.py` & `browserist-1.4.6/src/browserist/browser/screenshot/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/screenshot/visible_portion.py` & `browserist-1.4.6/src/browserist/browser/screenshot/visible_portion.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/__main__.py` & `browserist-1.4.6/src/browserist/browser/scroll/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/check_if/__main__.py` & `browserist-1.4.6/src/browserist/browser/scroll/check_if/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/check_if/is_end_of_page.py` & `browserist-1.4.6/src/browserist/browser/scroll/check_if/is_end_of_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/get/__main__.py` & `browserist-1.4.6/src/browserist/browser/scroll/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/get/total_height.py` & `browserist-1.4.6/src/browserist/browser/scroll/get/total_height.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/into_view.py` & `browserist-1.4.6/src/browserist/browser/scroll/into_view.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/page/__main__.py` & `browserist-1.4.6/src/browserist/browser/scroll/page/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/scroll/page/to_end.py` & `browserist-1.4.6/src/browserist/browser/scroll/page/to_end.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/tool/__main__.py` & `browserist-1.4.6/src/browserist/browser/tool/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/viewport/__main__.py` & `browserist-1.4.6/src/browserist/browser/viewport/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/viewport/get/__main__.py` & `browserist-1.4.6/src/browserist/browser/viewport/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/viewport/set/__main__.py` & `browserist-1.4.6/src/browserist/browser/viewport/set/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/viewport/set/size.py` & `browserist-1.4.6/src/browserist/browser/viewport/set/size.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/__main__.py` & `browserist-1.4.6/src/browserist/browser/wait/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/for_element.py` & `browserist-1.4.6/src/browserist/browser/wait/for_element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/__main__.py` & `browserist-1.4.6/src/browserist/browser/wait/until/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/images_have_loaded.py` & `browserist-1.4.6/src/browserist/browser/wait/until/images_have_loaded.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/number_of_window_handles_is.py` & `browserist-1.4.6/src/browserist/browser/wait/until/number_of_window_handles_is.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/page_title/__main__.py` & `browserist-1.4.6/src/browserist/browser/wait/until/page_title/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/page_title/changes.py` & `browserist-1.4.6/src/browserist/browser/wait/until/page_title/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/page_title/contains.py` & `browserist-1.4.6/src/browserist/browser/wait/until/page_title/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/page_title/equals.py` & `browserist-1.4.6/src/browserist/browser/wait/until/page_title/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/text/__main__.py` & `browserist-1.4.6/src/browserist/browser/wait/until/text/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/text/changes.py` & `browserist-1.4.6/src/browserist/browser/wait/until/text/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/text/contains.py` & `browserist-1.4.6/src/browserist/browser/wait/until/text/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/text/equals.py` & `browserist-1.4.6/src/browserist/browser/wait/until/text/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/url/__main__.py` & `browserist-1.4.6/src/browserist/browser/wait/until/url/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/url/changes.py` & `browserist-1.4.6/src/browserist/browser/wait/until/url/changes.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/url/contains.py` & `browserist-1.4.6/src/browserist/browser/wait/until/url/contains.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/wait/until/url/equals.py` & `browserist-1.4.6/src/browserist/browser/wait/until/url/equals.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/__main__.py` & `browserist-1.4.6/src/browserist/browser/window/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/get/__main__.py` & `browserist-1.4.6/src/browserist/browser/window/get/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/handle/__main__.py` & `browserist-1.4.6/src/browserist/browser/window/handle/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/open/__main__.py` & `browserist-1.4.6/src/browserist/browser/window/open/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/open/new_tab_or_window.py` & `browserist-1.4.6/src/browserist/browser/window/open/new_tab_or_window.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/set/__main__.py` & `browserist-1.4.6/src/browserist/browser/window/set/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/browser/window/switch_to.py` & `browserist-1.4.6/src/browserist/browser/window/switch_to.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/exception/element.py` & `browserist-1.4.6/src/browserist/exception/element.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/exception/headless.py` & `browserist-1.4.6/src/browserist/exception/headless.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/exception/timeout.py` & `browserist-1.4.6/src/browserist/exception/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/exception/window_handle.py` & `browserist-1.4.6/src/browserist/exception/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/factory/chromium.py` & `browserist-1.4.6/src/browserist/factory/chromium.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/factory/get.py` & `browserist-1.4.6/src/browserist/factory/get.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/factory/internet_explorer.py` & `browserist-1.4.6/src/browserist/factory/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/factory/safari.py` & `browserist-1.4.6/src/browserist/factory/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/factory/set.py` & `browserist-1.4.6/src/browserist/factory/set.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/directory.py` & `browserist-1.4.6/src/browserist/helper/directory.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/image.py` & `browserist-1.4.6/src/browserist/helper/image.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/timeout.py` & `browserist-1.4.6/src/browserist/helper/timeout.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/url.py` & `browserist-1.4.6/src/browserist/helper/url.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/window_handle.py` & `browserist-1.4.6/src/browserist/helper/window_handle.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper/xpath.py` & `browserist-1.4.6/src/browserist/helper/xpath.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper_iteration/retry.py` & `browserist-1.4.6/src/browserist/helper_iteration/retry.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper_screenshot/__init__.py` & `browserist-1.4.6/src/browserist/helper_screenshot/__init__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper_screenshot/complete_page.py` & `browserist-1.4.6/src/browserist/helper_screenshot/complete_page.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper_screenshot/controller.py` & `browserist-1.4.6/src/browserist/helper_screenshot/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/helper_screenshot/file.py` & `browserist-1.4.6/src/browserist/helper_screenshot/file.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/README.md` & `browserist-1.4.6/src/browserist/model/browser/README.md`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/base/driver.py` & `browserist-1.4.6/src/browserist/model/browser/base/driver.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/base/settings.py` & `browserist-1.4.6/src/browserist/model/browser/base/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/base/timeout/settings.py` & `browserist-1.4.6/src/browserist/model/browser/base/timeout/settings.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/chrome.py` & `browserist-1.4.6/src/browserist/model/browser/chrome.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/edge.py` & `browserist-1.4.6/src/browserist/model/browser/edge.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/extension/__main__.py` & `browserist-1.4.6/src/browserist/model/browser/extension/__main__.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/firefox.py` & `browserist-1.4.6/src/browserist/model/browser/firefox.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/internet_explorer.py` & `browserist-1.4.6/src/browserist/model/browser/internet_explorer.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/opera.py` & `browserist-1.4.6/src/browserist/model/browser/opera.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/browser/safari.py` & `browserist-1.4.6/src/browserist/model/browser/safari.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/combo_settings/cookie_banner.py` & `browserist-1.4.6/src/browserist/model/combo_settings/cookie_banner.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/combo_settings/login_form.py` & `browserist-1.4.6/src/browserist/model/combo_settings/login_form.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/combo_settings/search.py` & `browserist-1.4.6/src/browserist/model/combo_settings/search.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/driver_methods.py` & `browserist-1.4.6/src/browserist/model/driver_methods.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/screenshot.py` & `browserist-1.4.6/src/browserist/model/screenshot.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/type/file_png.py` & `browserist-1.4.6/src/browserist/model/type/file_png.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/type/path.py` & `browserist-1.4.6/src/browserist/model/type/path.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/type/url.py` & `browserist-1.4.6/src/browserist/model/type/url.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/type/xpath.py` & `browserist-1.4.6/src/browserist/model/type/xpath.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/viewport/collection/apple.py` & `browserist-1.4.6/src/browserist/model/viewport/collection/apple.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist/model/window/controller.py` & `browserist-1.4.6/src/browserist/model/window/controller.py`

 * *Files identical despite different names*

### Comparing `browserist-1.4.5/src/browserist.egg-info/PKG-INFO` & `browserist-1.4.6/src/browserist.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserist
-Version: 1.4.5
+Version: 1.4.6
 Summary: Extension for the Selenium web driver that makes browser automation even easier
 Home-page: https://github.com/jakob-bagterp/browserist
 Author: Jakob Bagterp
 Author-email: jakob_bagterp@hotmail.com
 Maintainer: Jakob Bagterp
 Maintainer-email: jakob_bagterp@hotmail.com
 License: Apache-2.0
@@ -22,19 +22,20 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: testing
 License-File: LICENSE.md
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 Browserist Extension for Selenium 👨‍💻
 > **browserist**
 > 1. The belief that web browsers account for differences in websites or web applications in all of their ability and that a particular web browser is superior to others.
 > 2. Discrimination or prejudice based on web browser.
 
 Despite the [urban definition](https://www.urbandictionary.com/define.php?term=browserist), Browserist is a Python extension of the Selenium web driver that makes it even easier to use different browsers for testing and automation.
@@ -209,19 +210,20 @@
 
 ## Contribute
 If you have suggestions or changes to the module, feel free to add to the code and create a [pull request](https://github.com/jakob-bagterp/browserist/pulls).
 
 ## Report Bugs
 Report bugs and issues [here](https://github.com/jakob-bagterp/browserist/issues).
 
-[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.5&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
+[![Latest version](https://img.shields.io/static/v1?label=version&message=1.4.6&color=yellowgreen)](https://github.com/jakob-bagterp/browserist/releases/latest)
 ![Python 3.10 | 3.11 or higher](https://img.shields.io/static/v1?label=python&message=3.10%20|%203.11%2B&color=blueviolet)
 [![Apache 2.0 license](https://img.shields.io/static/v1?label=license&message=Apache%202.0&color=blue)](https://github.com/jakob-bagterp/browserist/blob/master/LICENSE.md)
 [![Codecov](https://codecov.io/gh/jakob-bagterp/browserist/branch/master/graph/badge.svg?token=1JL65T099J)](https://codecov.io/gh/jakob-bagterp/browserist)
 [![Test](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml/badge.svg)](https://github.com/jakob-bagterp/browserist/actions/workflows/test.yml)
+[![Downloads](https://static.pepy.tech/badge/browserist)](https://pepy.tech/project/browserist)
 
 # 👩‍💻 How to Install Browserist 👨‍💻
 ## Prerequisites
 * Python 3.10 or higher
 * [Selenium](https://www.selenium.dev)
 * Relevant browsers: Chrome, Firefox, Edge, Safari, Opera, Internet Explorer
```

### Comparing `browserist-1.4.5/src/browserist.egg-info/SOURCES.txt` & `browserist-1.4.6/src/browserist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

