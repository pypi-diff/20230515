# Comparing `tmp/LinkChecker_GUI-10.0.0a4.tar.gz` & `tmp/LinkChecker_GUI-10.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed May  3 18:31:49 2023, max compression
+gzip compressed data, last modified: Mon May 15 18:24:11 2023, max compression
```

## Comparing `LinkChecker_GUI-10.0.0a4.tar` & `LinkChecker_GUI-10.0.0b1.tar`

### file list

```diff
@@ -1,77 +1,77 @@
--rw-r--r--   0        0        0      752 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.flake8
--rw-r--r--   0        0        0      125 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.git_archival.txt
--rw-r--r--   0        0        0       31 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.gitattributes
--rw-r--r--   0        0        0       38 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.pylintrc
--rw-r--r--   0        0        0      104 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.yamllint
--rw-r--r--   0        0        0      115 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/changelog.txt
--rw-r--r--   0        0        0      689 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/pyoxidizer.bzl
--rw-r--r--   0        0        0      700 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tox.ini
--rw-r--r--   0        0        0     3330 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/de.po
--rw-r--r--   0        0        0      214 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/linkchecker-gui.desktop
--rw-r--r--   0        0        0      127 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/po4a.conf
--rw-r--r--   0        0        0     1003 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/de/linkchecker-gui.1
--rw-r--r--   0        0        0      686 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/en/linkchecker-gui.1
--rw-r--r--   0        0        0    67271 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/favicon.icns
--rw-r--r--   0        0        0     3638 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/favicon.ico
--rw-r--r--   0        0        0      144 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/html.footer
--rw-r--r--   0        0        0      764 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/html.header
--rw-r--r--   0        0        0     6893 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/index.txt
--rw-r--r--   0        0        0      746 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/lccollection.qhcp
--rw-r--r--   0        0        0      476 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/lcdoc.qhp
--rw-r--r--   0        0        0     3224 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/pygments.css
--rw-r--r--   0        0        0     5382 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/sphinxdoc.css
--rw-r--r--   0        0        0    26618 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/128x128/linkchecker-gui.png
--rw-r--r--   0        0        0     1085 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/16x16/linkchecker-gui.png
--rw-r--r--   0        0        0     3254 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/32x32/linkchecker-gui.png
--rw-r--r--   0        0        0     6232 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/48x48/linkchecker-gui.png
--rw-r--r--   0        0        0     9761 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/doc/html/logo/64x64/linkchecker-gui.png
--rw-r--r--   0        0        0    24415 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/__init__.py
--rw-r--r--   0        0        0     2545 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/__main__.py
--rw-r--r--   0        0        0      212 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/_release.py
--rw-r--r--   0        0        0     1573 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/checker.py
--rw-r--r--   0        0        0     2545 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/configuration.py
--rw-r--r--   0        0        0     2580 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/contextmenu.py
--rw-r--r--   0        0        0     1541 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/debug.py
--rw-r--r--   0        0        0     6687 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor.py
--rw-r--r--   0        0        0     4004 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qsci.py
--rw-r--r--   0        0        0     6194 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qt.py
--rw-r--r--   0        0        0     2905 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/help.py
--rw-r--r--   0        0        0     9685 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/lineedit.py
--rw-r--r--   0        0        0    52172 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_rc.py
--rw-r--r--   0        0        0     1666 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_debug.py
--rw-r--r--   0        0        0     2717 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_editor.py
--rw-r--r--   0        0        0    56784 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_main.py
--rw-r--r--   0        0        0     8958 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_options.py
--rw-r--r--   0        0        0     2442 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/logger.py
--rw-r--r--   0        0        0     4135 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/options.py
--rw-r--r--   0        0        0     7561 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/projects.py
--rw-r--r--   0        0        0     2896 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/properties.py
--rw-r--r--   0        0        0     3333 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/recentdocs.py
--rw-r--r--   0        0        0     5746 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/settings.py
--rw-r--r--   0        0        0     2060 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/statistics.py
--rw-r--r--   0        0        0     3480 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/syntax.py
--rw-r--r--   0        0        0     3598 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/updater.py
--rw-r--r--   0        0        0     6926 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlmodel.py
--rw-r--r--   0        0        0     2754 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlsave.py
--rw-r--r--   0        0        0     1419 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/validator.py
--rw-r--r--   0        0        0    94208 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lccollection.qhc
--rw-r--r--   0        0        0    77824 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lcdoc.qch
--rw-r--r--   0        0        0        0 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/__init__.py
--rw-r--r--   0        0        0     1259 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/fileutil.py
--rw-r--r--   0        0        0     2179 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/url.py
--rw-r--r--   0        0        0        0 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/__init__.py
--rw-r--r--   0        0        0     2347 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chrome.py
--rw-r--r--   0        0        0     2550 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chromium.py
--rw-r--r--   0        0        0     1733 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/firefox.py
--rw-r--r--   0        0        0     1700 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/opera.py
--rw-r--r--   0        0        0     1428 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/safari.py
--rw-r--r--   0        0        0     1302 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/winutil.py
--rw-r--r--   0        0        0     1668 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/__init__.py
--rw-r--r--   0        0        0     1437 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/test_gui.py
--rw-r--r--   0        0        0     1079 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tests/library/test_fileutil.py
--rw-r--r--   0        0        0     4245 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/tools/hatch_build.py
--rw-r--r--   0        0        0      897 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/.gitignore
--rw-r--r--   0        0        0    35141 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/LICENSE
--rw-r--r--   0        0        0     1451 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/README.md
--rw-r--r--   0        0        0     2286 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/pyproject.toml
--rw-r--r--   0        0        0     2248 2023-05-03 18:31:49.000000 LinkChecker_GUI-10.0.0a4/PKG-INFO
+-rw-r--r--   0        0        0      752 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.flake8
+-rw-r--r--   0        0        0      125 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.git_archival.txt
+-rw-r--r--   0        0        0       31 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.gitattributes
+-rw-r--r--   0        0        0       38 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.pylintrc
+-rw-r--r--   0        0        0      104 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.yamllint
+-rw-r--r--   0        0        0      123 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/changelog.txt
+-rw-r--r--   0        0        0      689 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/pyoxidizer.bzl
+-rw-r--r--   0        0        0      700 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/tox.ini
+-rw-r--r--   0        0        0     3330 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/de.po
+-rw-r--r--   0        0        0      214 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/linkchecker-gui.desktop
+-rw-r--r--   0        0        0      127 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/po4a.conf
+-rw-r--r--   0        0        0     1003 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/de/linkchecker-gui.1
+-rw-r--r--   0        0        0      686 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/en/linkchecker-gui.1
+-rw-r--r--   0        0        0    67271 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/favicon.icns
+-rw-r--r--   0        0        0     3638 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/favicon.ico
+-rw-r--r--   0        0        0      144 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/html.footer
+-rw-r--r--   0        0        0      764 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/html.header
+-rw-r--r--   0        0        0     6893 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/index.txt
+-rw-r--r--   0        0        0      746 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/lccollection.qhcp
+-rw-r--r--   0        0        0      476 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/lcdoc.qhp
+-rw-r--r--   0        0        0     3224 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/pygments.css
+-rw-r--r--   0        0        0     5382 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/sphinxdoc.css
+-rw-r--r--   0        0        0    26618 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/logo/128x128/linkchecker-gui.png
+-rw-r--r--   0        0        0     1085 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/logo/16x16/linkchecker-gui.png
+-rw-r--r--   0        0        0     3254 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/logo/32x32/linkchecker-gui.png
+-rw-r--r--   0        0        0     6232 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/logo/48x48/linkchecker-gui.png
+-rw-r--r--   0        0        0     9761 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/doc/html/logo/64x64/linkchecker-gui.png
+-rw-r--r--   0        0        0    24858 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/__init__.py
+-rw-r--r--   0        0        0     2595 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/__main__.py
+-rw-r--r--   0        0        0      212 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/_release.py
+-rw-r--r--   0        0        0     1573 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/checker.py
+-rw-r--r--   0        0        0     2562 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/configuration.py
+-rw-r--r--   0        0        0     2580 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/contextmenu.py
+-rw-r--r--   0        0        0     1541 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/debug.py
+-rw-r--r--   0        0        0     6729 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor.py
+-rw-r--r--   0        0        0     4004 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor_qsci.py
+-rw-r--r--   0        0        0     6194 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor_qt.py
+-rw-r--r--   0        0        0     2905 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/help.py
+-rw-r--r--   0        0        0     9685 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/lineedit.py
+-rw-r--r--   0        0        0     1666 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_debug.py
+-rw-r--r--   0        0        0     2717 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_editor.py
+-rw-r--r--   0        0        0    56208 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_main.py
+-rw-r--r--   0        0        0     8958 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_options.py
+-rw-r--r--   0        0        0     2442 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/logger.py
+-rw-r--r--   0        0        0     4135 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/options.py
+-rw-r--r--   0        0        0     7561 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/projects.py
+-rw-r--r--   0        0        0     2896 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/properties.py
+-rw-r--r--   0        0        0     3333 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/recentdocs.py
+-rw-r--r--   0        0        0     5746 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/settings.py
+-rw-r--r--   0        0        0     2060 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/statistics.py
+-rw-r--r--   0        0        0     3480 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/syntax.py
+-rw-r--r--   0        0        0     6926 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/urlmodel.py
+-rw-r--r--   0        0        0     2754 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/urlsave.py
+-rw-r--r--   0        0        0     1419 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/validator.py
+-rw-r--r--   0        0        0    94208 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/data/help/lccollection.qhc
+-rw-r--r--   0        0        0    77824 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/data/help/lcdoc.qch
+-rw-r--r--   0        0        0    11482 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/data/rc/linkchecker.rcc
+-rw-r--r--   0        0        0        0 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/__init__.py
+-rw-r--r--   0        0        0     1259 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/fileutil.py
+-rw-r--r--   0        0        0     2179 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/url.py
+-rw-r--r--   0        0        0        0 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/__init__.py
+-rw-r--r--   0        0        0     2347 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/chrome.py
+-rw-r--r--   0        0        0     2550 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/chromium.py
+-rw-r--r--   0        0        0     1733 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/firefox.py
+-rw-r--r--   0        0        0     1700 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/opera.py
+-rw-r--r--   0        0        0     1428 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/safari.py
+-rw-r--r--   0        0        0     1302 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/winutil.py
+-rw-r--r--   0        0        0     1668 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/tests/__init__.py
+-rw-r--r--   0        0        0     6645 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/tests/test_gui.py
+-rw-r--r--   0        0        0     1073 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/tests/library/test_fileutil.py
+-rw-r--r--   0        0        0     4802 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/tools/hatch_build.py
+-rw-r--r--   0        0        0      897 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/.gitignore
+-rw-r--r--   0        0        0     9684 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/COPYING.icons
+-rw-r--r--   0        0        0    35141 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/LICENSE
+-rw-r--r--   0        0        0     1672 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/README.md
+-rw-r--r--   0        0        0     2285 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2496 2023-05-15 18:24:11.000000 LinkChecker_GUI-10.0.0b1/PKG-INFO
```

### Comparing `LinkChecker_GUI-10.0.0a4/.flake8` & `LinkChecker_GUI-10.0.0b1/.flake8`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/pyoxidizer.bzl` & `LinkChecker_GUI-10.0.0b1/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/tox.ini` & `LinkChecker_GUI-10.0.0b1/tox.ini`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/de.po` & `LinkChecker_GUI-10.0.0b1/doc/de.po`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/de/linkchecker-gui.1` & `LinkChecker_GUI-10.0.0b1/doc/de/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/en/linkchecker-gui.1` & `LinkChecker_GUI-10.0.0b1/doc/en/linkchecker-gui.1`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/favicon.icns` & `LinkChecker_GUI-10.0.0b1/doc/html/favicon.icns`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/favicon.ico` & `LinkChecker_GUI-10.0.0b1/doc/html/favicon.ico`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/html.header` & `LinkChecker_GUI-10.0.0b1/doc/html/html.header`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/index.txt` & `LinkChecker_GUI-10.0.0b1/doc/html/index.txt`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/lccollection.qhcp` & `LinkChecker_GUI-10.0.0b1/doc/html/lccollection.qhcp`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/pygments.css` & `LinkChecker_GUI-10.0.0b1/doc/html/pygments.css`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/sphinxdoc.css` & `LinkChecker_GUI-10.0.0b1/doc/html/sphinxdoc.css`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/logo/128x128/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0b1/doc/html/logo/128x128/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/logo/16x16/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0b1/doc/html/logo/16x16/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/logo/32x32/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0b1/doc/html/logo/32x32/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/logo/48x48/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0b1/doc/html/logo/48x48/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/doc/html/logo/64x64/linkchecker-gui.png` & `LinkChecker_GUI-10.0.0b1/doc/html/logo/64x64/linkchecker-gui.png`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/__init__.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,14 @@
 from .logger import GuiLogHandler, SignalLogger, StatusLogger
 from .options import LinkCheckerOptions
 from .projects import ProjectExt, loadproject, openproject, saveproject
 from .properties import clear_properties, set_properties
 from .recentdocs import RecentDocumentModel
 from .settings import Settings
 from .statistics import clear_statistics, set_statistics
-# XXX from .updater import UpdateDialog
 from .urlmodel import UrlItemModel
 from .urlsave import urlsave
 
 DocBaseUrl = "qthelp://linkchecker.app.linkchecker-gui/doc/"
 RegistryBase = "LinkChecker-GUI"
 Status = Enum("Status", ["idle", "checking"])
 
@@ -74,29 +73,29 @@
     log_status_signal = QtCore.pyqtSignal(int, int, int, float, int)
     log_stats_signal = QtCore.pyqtSignal(object)
     error_signal = QtCore.pyqtSignal(str)
 
     def __init__(self, parent=None, url=None, project=None):
         """Initialize UI."""
         super().__init__(parent)
+        QtCore.QResource.registerResource(self.get_rccpath())
         self.setupUi(self)
         self.setWindowFlags(
             self.windowFlags() | QtCore.Qt.WindowType.WindowContextHelpButtonHint)
         self.setWindowTitle(configuration.App)
         # app settings
         self.settings = Settings(RegistryBase, configuration.AppName)
         # init subdialogs
         self.options = LinkCheckerOptions(parent=self)
         self.debug = LinkCheckerDebug(parent=self)
         self.checker = CheckerThread(parent=self)
         self.contextmenu = ContextMenu(parent=self)
         self.editor = EditorWindow(parent=self)
         self.assistant = HelpWindow(self, self.get_qhcpath())
         self.actionHelp.setVisible(True)
-        self.actionCheckUpdates.setVisible(False)  # XXX
         self.config_error = None
         self.icon_start = get_icon(":/icons/start.png")
         self.icon_stop = get_icon(":/icons/stop.png")
         self.movie = QtGui.QMovie(":/icons/busy.gif")
         self.movie.setCacheMode(QtGui.QMovie.CacheMode.CacheAll)
         self.label_busy.setText("")
         self.label_busy.setMovie(self.movie)
@@ -171,27 +170,31 @@
         self.saveresultas = data['saveresultas']
 
     def get_qhcpath(self):
         """Helper function to search for the QHC help file in different
         locations."""
         return os.path.join(__path__[0], "data", "help", "lccollection.qhc")
 
+    def get_rccpath(self):
+        """Helper function to search for the RCC resource file in different
+        locations."""
+        return os.path.join(__path__[0], "data", "rc", "linkchecker.rcc")
+
     def connect_widgets(self):
         """Connect widget signals. Some signals use the AutoConnect feature.
         Autoconnected methods have the form on_<objectname>_<signal>.
         """
 
         def set_idle():
             """Set application status to idle."""
             self.status = Status.idle
             self.set_statusmsg(_("Check finished."))
             self.controlButton.clicked.disconnect(self.checker.cancel)
 
         self.checker.finished.connect(set_idle)
-        # XXX self.checker.terminated.connect(set_idle)
         self.log_url_signal.connect(self.model.log_url)
         self.log_stats_signal.connect(self.log_stats)
         self.error_signal.connect(self.internal_error)
         self.options.editor.saved.connect(self.read_config)
         self.log_status_signal.connect(self.log_status)
         self.prop_url.linkHovered.connect(self.hover_link)
         self.prop_parenturl.linkHovered.connect(self.hover_link)
@@ -358,23 +361,34 @@
     @QtCore.pyqtSlot()
     def on_actionQuit_triggered(self):
         """Quit application."""
         self.close()
 
     def closeEvent(self, e=None):
         """Save settings and remove registered logging handler"""
-        self.settings.save_geometry(dict(size=self.size(), pos=self.pos()))
-        self.settings.save_treeviewcols(self.get_treeviewcols())
-        self.settings.save_options(self.options.get_options())
-        self.settings.save_recent_documents(self.recent.get_documents())
-        self.settings.save_misc(dict(saveresultas=self.saveresultas))
-        self.settings.sync()
-        logconf.remove_loghandler(self.handler)
-        if e is not None:
-            e.accept()
+        try:
+            self.checker.finished.connect(
+                self.close, QtCore.Qt.ConnectionType.UniqueConnection)
+        except TypeError:
+            pass
+        if self.checker.isRunning():
+            self.checker.cancel()
+            self.cancel()
+            if e is not None:
+                e.ignore()
+        else:
+            self.settings.save_geometry(dict(size=self.size(), pos=self.pos()))
+            self.settings.save_treeviewcols(self.get_treeviewcols())
+            self.settings.save_options(self.options.get_options())
+            self.settings.save_recent_documents(self.recent.get_documents())
+            self.settings.save_misc(dict(saveresultas=self.saveresultas))
+            self.settings.sync()
+            logconf.remove_loghandler(self.handler)
+            if e is not None:
+                e.accept()
 
     @QtCore.pyqtSlot()
     def on_actionAbout_triggered(self):
         """Display about dialog."""
         modules = "<br>\n".join(configuration.get_modules_info().split())
         d = {
             "app": configuration.App,
@@ -395,14 +409,17 @@
 <p>Using LinkChecker %(linkchecker_version)s
 <p>Python: %(pyver)s<br>
 %(modules)s<br>
 <p>%(copyright)s
 <br>%(appname)s is licensed under the
 <a href="https://www.gnu.org/licenses/gpl-3.0.html">GPL</a>
 Version 3 or later.
+<p>Icons from <a href="https://develop.kde.org/frameworks/oxygen-icons/">
+Oxygen icons</a> copyright KDE<br>
+and licensed under the GNU LGPL version 3 or later.
 </center></qt>"""
             )
             % d,
         )
 
     @QtCore.pyqtSlot()
     def on_actionDebug_triggered(self):
@@ -422,21 +439,14 @@
     @QtCore.pyqtSlot()
     def on_actionSave_triggered(self):
         """Save URL results."""
         saveresultas = urlsave(self, self.config, self.model.urls)
         if saveresultas:
             self.saveresultas = saveresultas
 
-#    @QtCore.pyqtSlot()
-#    def on_actionCheckUpdates_triggered(self):
-#        """Display update check result."""
-#        dialog = UpdateDialog(self)
-#        dialog.reset()
-#        dialog.show()
-
     def start(self):
         """Start a new check."""
         if self.status == Status.idle:
             self.check()
 
     on_urlinput_returnPressed = start
 
@@ -619,23 +629,23 @@
         url = mime.urls()[0]
         if url.path().toLower().endsWith(ProjectExt):
             filename = url.toLocalFile()
             loadproject(self, filename)
         else:
             self.urlinput.setText(url.toString())
 
+    '''  # XXX
     def retranslateUi(self, Window):
         """Translate menu titles."""
         super().retranslateUi(Window)
         # self.menu_lang is created after calling retranslateUi
         # the first time, so check for its excistance
         if hasattr(self, "menu_lang"):
             self.menuLang.setTitle(_("&Language"))
 
-    '''  # XXX
     def switch_language(self, action):
         """Change UI language."""
         lang = str(action.data().toString())
         i18n.install_language(lang)
         self.retranslateUi(self)
         self.options.retranslateUi(self.options)
         self.debug.retranslateUi(self.debug)
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/__main__.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,20 +15,19 @@
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 Check HTML pages for broken links. This is the GUI client.
 """
 import signal
 import sys
 
-from linkcheck import configuration
 from linkcheck.command.linkchecker import drop_privileges
 from linkcheck.fileutil import is_readable
 from PyQt6.QtWidgets import QApplication  # pylint: disable=no-name-in-module
 
-from . import LinkCheckerMain
+from . import configuration, LinkCheckerMain
 from .projects import ProjectExt
 
 
 def excepthook(window, etype, evalue, tb):
     """Catch unhandled exceptions."""
     from io import StringIO
     from linkcheck.director.console import internal_error
@@ -43,14 +42,15 @@
     and show the main window."""
     if argv is None:
         argv = sys.argv
     app = QApplication(argv)
     app.setApplicationName(configuration.AppName)
     app.setApplicationVersion(configuration.Version)
     app.setOrganizationName(configuration.Author)
+    app.setDesktopFileName(f"{configuration.AppName.lower()}.desktop")
     args = app.arguments()
     mainkwargs = {}
     if len(args) > 1:
         fileorurl = args[1]
         if is_readable(fileorurl) and fileorurl.lower().endswith(ProjectExt):
             mainkwargs["project"] = fileorurl
         else:
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/checker.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/checker.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/configuration.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/configuration.py`

 * *Files 13% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # You should have received a copy of the GNU General Public License along
 # with this program; if not, write to the Free Software Foundation, Inc.,
 # 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301 USA.
 """
 Store metadata and options.
 """
 
-from linkcheck import fileutil
+import importlib
 
 try:
     from . import _release
 except ImportError:
     raise SystemExit('Run "hatchling build --hooks-only" first')
 
 Version = _release.__version__
@@ -53,18 +53,19 @@
 )
 
 
 def get_modules_info():
     """Return unicode string with detected module info."""
     module_infos = []
     for (mod, name, version_attr) in Modules:
-        if not fileutil.has_module(mod):
+        try:
+            module = importlib.import_module(mod)
+        except ModuleNotFoundError:
             continue
-        if version_attr and hasattr(mod, version_attr):
-            attr = getattr(mod, version_attr)
+        if version_attr and (attr := getattr(module, version_attr, None)):
             version = attr() if callable(attr) else attr
             module_infos.append(f"{name} {version}")
         else:
             # ignore attribute errors in case library developers
             # change the version information attribute
             module_infos.append(name)
     return "Modules: %s" % (", ".join(module_infos))
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/contextmenu.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/contextmenu.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/debug.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/debug.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,19 +114,20 @@
         dialog.setDefaultButton(QtWidgets.QMessageBox.StandardButton.Save)
         return dialog.exec() == QtWidgets.QMessageBox.StandardButton.Save
 
     def save(self):
         """Save editor contents to file."""
         if not self.filename:
             title = _("Save File As")
-            res = QtWidgets.QFileDialog.getSaveFileName(self, title, self.basedir)
-            if not res:
+            filename, _filter = \
+                QtWidgets.QFileDialog.getSaveFileName(self, title, self.basedir)
+            if not filename:
                 # user canceled
                 return
-            self.filename = res
+            self.filename = filename
             self.setWindowTitle(self.filename)
         else:
             if not os.path.isfile(self.filename):
                 return
             if not os.access(self.filename, os.W_OK):
                 return
         fh = None
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qsci.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor_qsci.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/editor_qt.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/editor_qt.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/help.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/help.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/lineedit.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/lineedit.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_debug.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_debug.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_editor.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_editor.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_main.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Form implementation generated from reading ui file 'ui/main.ui'
 #
-# Created by: PyQt6 UI code generator 6.4.2
+# Created by: PyQt6 UI code generator 6.5.0
 #
 # WARNING: Any manual changes made to this file will be lost when pyuic6 is
 # run again.  Do not edit this file unless you know what you are doing.
 
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
@@ -14,16 +14,15 @@
         MainWindow.setObjectName("MainWindow")
         MainWindow.resize(713, 627)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Preferred, QtWidgets.QSizePolicy.Policy.Preferred)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
         sizePolicy.setHeightForWidth(MainWindow.sizePolicy().hasHeightForWidth())
         MainWindow.setSizePolicy(sizePolicy)
-        icon = QtGui.QIcon()
-        icon.addPixmap(QtGui.QPixmap(":/icons/app.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        icon = QtGui.QIcon.fromTheme("linkchecker-gui")
         MainWindow.setWindowIcon(icon)
         MainWindow.setStatusTip("")
         self.centralwidget = QtWidgets.QWidget(parent=MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.verticalLayout = QtWidgets.QVBoxLayout(self.centralwidget)
         self.verticalLayout.setContentsMargins(4, 4, 4, 4)
         self.verticalLayout.setObjectName("verticalLayout")
@@ -43,17 +42,17 @@
         self.urlinput.setMaxLength(2048)
         self.urlinput.setObjectName("urlinput")
         self.horizontalLayout_3.addWidget(self.urlinput)
         spacerItem1 = QtWidgets.QSpacerItem(10, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem1)
         self.controlButton = QtWidgets.QPushButton(parent=self.centralwidget)
         self.controlButton.setStatusTip("")
-        icon1 = QtGui.QIcon()
-        icon1.addPixmap(QtGui.QPixmap(":/icons/start.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.controlButton.setIcon(icon1)
+        icon = QtGui.QIcon()
+        icon.addPixmap(QtGui.QPixmap(":/icons/start.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.controlButton.setIcon(icon)
         self.controlButton.setDefault(True)
         self.controlButton.setObjectName("controlButton")
         self.horizontalLayout_3.addWidget(self.controlButton)
         self.verticalLayout.addLayout(self.horizontalLayout_3)
         self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_4.setSizeConstraint(QtWidgets.QLayout.SizeConstraint.SetDefaultConstraint)
         self.horizontalLayout_4.setContentsMargins(0, 0, -1, -1)
@@ -688,75 +687,70 @@
         self.menuHelp = QtWidgets.QMenu(parent=self.menubar)
         self.menuHelp.setObjectName("menuHelp")
         MainWindow.setMenuBar(self.menubar)
         self.statusBar = QtWidgets.QStatusBar(parent=MainWindow)
         self.statusBar.setObjectName("statusBar")
         MainWindow.setStatusBar(self.statusBar)
         self.actionAbout = QtGui.QAction(parent=MainWindow)
-        icon2 = QtGui.QIcon()
-        icon2.addPixmap(QtGui.QPixmap(":/icons/about.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionAbout.setIcon(icon2)
+        icon1 = QtGui.QIcon()
+        icon1.addPixmap(QtGui.QPixmap(":/icons/about.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionAbout.setIcon(icon1)
         self.actionAbout.setObjectName("actionAbout")
         self.actionHelp = QtGui.QAction(parent=MainWindow)
-        icon3 = QtGui.QIcon()
-        icon3.addPixmap(QtGui.QPixmap(":/icons/help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionHelp.setIcon(icon3)
+        icon2 = QtGui.QIcon()
+        icon2.addPixmap(QtGui.QPixmap(":/icons/help.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionHelp.setIcon(icon2)
         self.actionHelp.setObjectName("actionHelp")
         self.actionViewOnline = QtGui.QAction(parent=MainWindow)
-        icon4 = QtGui.QIcon()
-        icon4.addPixmap(QtGui.QPixmap(":/icons/online.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionViewOnline.setIcon(icon4)
+        icon3 = QtGui.QIcon()
+        icon3.addPixmap(QtGui.QPixmap(":/icons/online.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionViewOnline.setIcon(icon3)
         self.actionViewOnline.setObjectName("actionViewOnline")
         self.actionOptions = QtGui.QAction(parent=MainWindow)
-        icon5 = QtGui.QIcon()
-        icon5.addPixmap(QtGui.QPixmap(":/icons/preferences.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionOptions.setIcon(icon5)
+        icon4 = QtGui.QIcon()
+        icon4.addPixmap(QtGui.QPixmap(":/icons/preferences.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionOptions.setIcon(icon4)
         self.actionOptions.setObjectName("actionOptions")
         self.actionCopyToClipboard = QtGui.QAction(parent=MainWindow)
-        icon6 = QtGui.QIcon()
-        icon6.addPixmap(QtGui.QPixmap(":/icons/copy.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionCopyToClipboard.setIcon(icon6)
+        icon5 = QtGui.QIcon()
+        icon5.addPixmap(QtGui.QPixmap(":/icons/copy.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionCopyToClipboard.setIcon(icon5)
         self.actionCopyToClipboard.setObjectName("actionCopyToClipboard")
         self.actionViewParentOnline = QtGui.QAction(parent=MainWindow)
-        self.actionViewParentOnline.setIcon(icon4)
+        self.actionViewParentOnline.setIcon(icon3)
         self.actionViewParentOnline.setObjectName("actionViewParentOnline")
         self.actionViewParentSource = QtGui.QAction(parent=MainWindow)
-        self.actionViewParentSource.setIcon(icon4)
+        self.actionViewParentSource.setIcon(icon3)
         self.actionViewParentSource.setObjectName("actionViewParentSource")
         self.actionDebug = QtGui.QAction(parent=MainWindow)
         self.actionDebug.setObjectName("actionDebug")
         self.actionViewProperties = QtGui.QAction(parent=MainWindow)
         self.actionViewProperties.setObjectName("actionViewProperties")
         self.actionSave = QtGui.QAction(parent=MainWindow)
-        icon7 = QtGui.QIcon()
-        icon7.addPixmap(QtGui.QPixmap(":/icons/save.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionSave.setIcon(icon7)
+        icon6 = QtGui.QIcon()
+        icon6.addPixmap(QtGui.QPixmap(":/icons/save.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionSave.setIcon(icon6)
         self.actionSave.setObjectName("actionSave")
         self.actionQuit = QtGui.QAction(parent=MainWindow)
-        icon8 = QtGui.QIcon()
-        icon8.addPixmap(QtGui.QPixmap(":/icons/exit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
-        self.actionQuit.setIcon(icon8)
+        icon7 = QtGui.QIcon()
+        icon7.addPixmap(QtGui.QPixmap(":/icons/exit.png"), QtGui.QIcon.Mode.Normal, QtGui.QIcon.State.Off)
+        self.actionQuit.setIcon(icon7)
         self.actionQuit.setObjectName("actionQuit")
-        self.actionCheckUpdates = QtGui.QAction(parent=MainWindow)
-        self.actionCheckUpdates.setObjectName("actionCheckUpdates")
-        self.actionDonate = QtGui.QAction(parent=MainWindow)
-        self.actionDonate.setObjectName("actionDonate")
         self.actionOpen_project = QtGui.QAction(parent=MainWindow)
         self.actionOpen_project.setObjectName("actionOpen_project")
         self.actionSave_project = QtGui.QAction(parent=MainWindow)
         self.actionSave_project.setObjectName("actionSave_project")
         self.menuEdit.addAction(self.actionOptions)
         self.menuFile.addAction(self.actionOpen_project)
         self.menuFile.addAction(self.actionSave_project)
         self.menuFile.addAction(self.actionSave)
         self.menuFile.addAction(self.actionQuit)
         self.menuHelp.addAction(self.actionAbout)
         self.menuHelp.addAction(self.actionHelp)
         self.menuHelp.addAction(self.actionDebug)
-        self.menuHelp.addAction(self.actionCheckUpdates)
         self.menubar.addAction(self.menuFile.menuAction())
         self.menubar.addAction(self.menuEdit.menuAction())
         self.menubar.addAction(self.menuHelp.menuAction())
         self.label.setBuddy(self.urlinput)
 
         self.retranslateUi(MainWindow)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
@@ -824,16 +818,13 @@
         self.actionViewParentSource.setToolTip(_translate("MainWindow", "View parent URL source"))
         self.actionDebug.setText(_translate("MainWindow", "Show debug"))
         self.actionViewProperties.setText(_translate("MainWindow", "View properties"))
         self.actionViewProperties.setToolTip(_translate("MainWindow", "View URL properties"))
         self.actionSave.setText(_translate("MainWindow", "Save &results..."))
         self.actionQuit.setText(_translate("MainWindow", "&Quit"))
         self.actionQuit.setShortcut(_translate("MainWindow", "Ctrl+Q"))
-        self.actionCheckUpdates.setText(_translate("MainWindow", "Check for updates"))
-        self.actionDonate.setText(_translate("MainWindow", "Donate"))
         self.actionOpen_project.setText(_translate("MainWindow", "&Open project..."))
         self.actionOpen_project.setIconText(_translate("MainWindow", "Open project"))
         self.actionOpen_project.setShortcut(_translate("MainWindow", "Ctrl+O"))
         self.actionSave_project.setText(_translate("MainWindow", "&Save project..."))
         self.actionSave_project.setShortcut(_translate("MainWindow", "Ctrl+S"))
 from .lineedit import LineEdit
-from . import linkchecker_rc
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/linkchecker_ui_options.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/linkchecker_ui_options.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/logger.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/logger.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/options.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/options.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/projects.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/projects.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/properties.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/properties.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/recentdocs.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/recentdocs.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/settings.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/settings.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/statistics.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/statistics.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/syntax.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/syntax.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlmodel.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/urlmodel.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/urlsave.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/urlsave.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/validator.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/validator.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lccollection.qhc` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/data/help/lccollection.qhc`

 * *Files 8% similar despite different names*

#### sqlite3 {} .dump

```diff
@@ -4,25 +4,25 @@
 INSERT INTO NamespaceTable VALUES(1,'linkchecker.app.linkchecker-gui','lcdoc.qch');
 CREATE TABLE FolderTable (Id INTEGER PRIMARY KEY, NamespaceId INTEGER, Name TEXT );
 INSERT INTO FolderTable VALUES(1,1,'doc');
 CREATE TABLE FilterAttributeTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterNameTable (Id INTEGER PRIMARY KEY, Name TEXT );
 CREATE TABLE FilterTable (NameId INTEGER, FilterAttributeId INTEGER );
 CREATE TABLE SettingsTable (Key TEXT PRIMARY KEY, Value BLOB );
-INSERT INTO SettingsTable VALUES('LastRegisterTime','2023-05-03T18:31:49.000');
+INSERT INTO SettingsTable VALUES('LastRegisterTime','2023-05-15T18:24:11.000');
 INSERT INTO SettingsTable VALUES('WindowTitle','LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('LastShownPages','qthelp://linkchecker.app.linkchecker-gui/doc/index.html');
 INSERT INTO SettingsTable VALUES('CacheDirectory','linkchecker/LinkChecker-GUI');
 INSERT INTO SettingsTable VALUES('CacheDirRelativeToCollection',0);
 INSERT INTO SettingsTable VALUES('EnableFilterFunctionality',0);
 INSERT INTO SettingsTable VALUES('HideFilterFunctionality',1);
 INSERT INTO SettingsTable VALUES('EnableDocumentationManager',0);
 INSERT INTO SettingsTable VALUES('EnableAddressBar',0);
 INSERT INTO SettingsTable VALUES('HideAddressBar',1);
-INSERT INTO SettingsTable VALUES('CreationTime',1683138709);
+INSERT INTO SettingsTable VALUES('CreationTime',1684175051);
 INSERT INTO SettingsTable VALUES('FullTextSearchFallback',0);
 INSERT INTO SettingsTable VALUES('ApplicationIcon',X'89504e470d0a1a0a0000000d49484452000000100000001008060000001ff3ff6100000006624b474400ff00ff00ffa0bda79300000009704859730000375c0000375c01cbc7a4b9000003af4944415438cb05c15b681c550006e0ff9c33979dd95b92cd65d324dd6ed2b4696252a4d634a285168b979712a1166c51fba214aa0f8a102df8526b0b62147c284aa95044a9a4e08bb7b41830921242adb59590d0682fc9ee26d9cbccecccececccec397e1f99fc6206aa2aa152ae92030787c8537bb7f2b3677ede5628d7f6d782c68e5cdec2ed3bb9e5c0adff162aea6aac4923a11f824a544000d2d2721194803c582c886ac5ef9899593e1b694b1ccd6c69893edab0452eef40ed6c26ccad5b81eb5fae6e981f1a6bc54aefe3bd448d4882ed1a3c4cec9223ea10bd03bb7ba6b5eed421afbd455a63b2c88754747626851c8b408b451489d151cae86116517f322a6e85324a089005b0553bfdd107b3ed035d7bc25434686a92250846fe7e688ab575078a1790dc83a2084c37ac976cd9339c9b3a0f9f093c5e6327dfb9846ddb87decd0cf5bc6ac309e6af7c2eafcdfd8a1e6e92375f1c251d1a274b7913d53a8161d598ef8741e885dd1cb00d2ffc835e987c497605394e34051b2e6785643f6e4507c8955bf7a14a0cfbba2278b6b584ed6995c4123a882cb1788b8e7447e2f58dbca9b378e7e921b92936c1a3aa54957544fb4648ac6f042f8f0d81afdfc3f1b72670fbcf058c3f9186132a585aade3e9914ee2397eb262793fb0fee1f111aa2b272c50114f28786408f264ab8ce75265bc71ee22ea7d8750d7bab070ed2a0c9780c632304a16ca25872574794a8a4615cff242d09a07d751301abd86533bbbf1f1e5ff80fee7b1b5f731d44c0b1b0d1d7a2285a46028e6eb500114cbae47635a6485f0b058b508d1cc799cdb7b01851b27706335444b5b2faa850202db81de9c056551e83290d415e238fea6697a2bf4e6663ccfa8f2bbe217f1de9e2fb9d4d8c467d37de0b111f8a601df09601b35488127ba9a15908668944a36bc7a38abb5c6f3d4bcd384bbff463f39357615633b73e49b69ce57c4313469ba08ac1ae44603d9942632299d1472267fb85a2101879064f6a92e5348f7bf7e01f9a2e81bded58ebfeedaf86afe2051fb86797794139b521151181cd3c1e2aad988e82ab8aa301af0f7a5a43e8706a774bdc407b3d98e49b7e6e1e28fca9a9f7ea51c4d3753574f20d9dd4e0ca6923c224864b730b525e1534adfceee1f3aaf690ac9f4a739dbb73b7eb4bd991c9959a8d8672e85af8535e93bdb323265bbde52a8380ae7752e372cd3df5c99b5efcd9d54d2fddf57560a3477fd5b6198040448d22307cc09cb01ff651ee7e33a3aec1ad20474871c4975060d3444505c05c422082bb40d8ebb9bff4c8500706c4ae07f702bc1c500e2ed86000000227a545874536f667477617265000078da2b2f2fd7cbcccb2e4e4e2c48d5cb2f4a070036d806581053ca5c0000000049454e44ae426082');
 CREATE TABLE FileNameTable (FolderId INTEGER, Name TEXT, FileId INTEGER PRIMARY KEY, Title TEXT);
 INSERT INTO FileNameTable VALUES(1,'index.html',1,'Check websites for broken links');
 INSERT INTO FileNameTable VALUES(1,'pygments.css',2,'pygments.css');
 INSERT INTO FileNameTable VALUES(1,'sphinxdoc.css',3,'sphinxdoc.css');
 INSERT INTO FileNameTable VALUES(1,'logo/64x64/linkchecker-gui.png',4,'linkchecker-gui.png');
@@ -31,15 +31,15 @@
 INSERT INTO ContentsTable VALUES(1,1,X'00000000000000140069006e006400650078002e00680074006d006c00000032004c0069006e006b0043006800650063006b0065007200200064006f00630075006d0065006e0074006100740069006f006e');
 CREATE TABLE FileFilterTable (FilterAttributeId INTEGER, FileId INTEGER);
 CREATE TABLE IndexFilterTable (FilterAttributeId INTEGER, IndexId INTEGER);
 CREATE TABLE ContentsFilterTable (FilterAttributeId INTEGER, ContentsId INTEGER );
 CREATE TABLE FileAttributeSetTable (NamespaceId INTEGER, FilterAttributeSetId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE OptimizedFilterTable (NamespaceId INTEGER, FilterAttributeId INTEGER);
 CREATE TABLE TimeStampTable (NamespaceId INTEGER, FolderId INTEGER, FilePath TEXT, Size INTEGER, TimeStamp TEXT);
-INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2023-05-03T18:31:49');
+INSERT INTO TimeStampTable VALUES(1,1,'lcdoc.qch',77824,'2023-05-15T18:24:11');
 CREATE TABLE VersionTable (NamespaceId INTEGER, Version TEXT);
 INSERT INTO VersionTable VALUES(1,NULL);
 CREATE TABLE Filter (FilterId INTEGER PRIMARY KEY, Name TEXT);
 CREATE TABLE ComponentTable (ComponentId INTEGER PRIMARY KEY, Name TEXT);
 INSERT INTO ComponentTable VALUES(1,'doc');
 CREATE TABLE ComponentMapping (ComponentId INTEGER, NamespaceId INTEGER);
 INSERT INTO ComponentMapping VALUES(1,1);
```

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/data/help/lcdoc.qch` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/data/help/lcdoc.qch`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/fileutil.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/fileutil.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/url.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/url.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chrome.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/chrome.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/chromium.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/chromium.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/firefox.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/firefox.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/opera.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/opera.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/safari.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/safari.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/linkcheck_gui/library/bookmarks/winutil.py` & `LinkChecker_GUI-10.0.0b1/linkcheck_gui/library/bookmarks/winutil.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/tests/__init__.py` & `LinkChecker_GUI-10.0.0b1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/tests/library/test_fileutil.py` & `LinkChecker_GUI-10.0.0b1/tests/library/test_fileutil.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,9 +22,9 @@
 
 class TestFileUtil(unittest.TestCase):
     """Test fileutil module."""
 
     def test_fileutil(self):
         fp = tempfile.NamedTemporaryFile(delete=False)
         fp.close()
-        assert fileutil.is_writable(fp.name), True
+        assert fileutil.is_writable(fp.name)
         os.remove(fp.name)
```

### Comparing `LinkChecker_GUI-10.0.0a4/tools/hatch_build.py` & `LinkChecker_GUI-10.0.0b1/tools/hatch_build.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,22 +21,45 @@
 
 from hatchling.builders.hooks.plugin.interface import BuildHookInterface
 import markdown2
 
 HELP_DIR = ("linkcheck_gui", "data", "help")
 RELEASE_PY = ("linkcheck_gui", "_release.py")
 HELP_SRC_DIR = ("doc", "html")
+RC_SRC_DIR = ("linkcheck_gui", "rc")
+RC_DIR = ("linkcheck_gui", "data", "rc")
 
 
 class CustomBuildHook(BuildHookInterface):
     def clean(self, versions):
         Path(*RELEASE_PY).unlink(missing_ok=True)
         shutil.rmtree(str(Path(*HELP_DIR)), ignore_errors=True)
 
+    def qt_tool_location(self, qt_module, exe):
+        try:
+            cp = subprocess.run(
+                ["pkg-config", "--variable=libexecdir", qt_module],
+                capture_output=True, text=True)
+            tool_exec_dir = cp.stdout.strip()
+        except FileNotFoundError:
+            self.app.display_warning("pkg-config not installed")
+            tool_exec_dir = None
+        if tool_exec_dir:
+            tool_location = Path(tool_exec_dir, exe)
+        else:
+            # Ubuntu 22.04 doesn't provide Qt6Help.pc, 22.10 does but without libexecdir
+            # qhelpgenerator found in bin on 22.04, libexec from 22.10
+            tool_location = shutil.which(
+                exe,
+                path="/usr/lib/qt6/libexec/:/usr/lib64/qt6/libexec/:"
+                     "/usr/lib/qt6/bin/:/usr/lib64/qt6/bin/")
+        return tool_location
+
     def initialize(self, version, build_data):
+        # _release.py
         cp = None
         committer_date = committer_year = "unknown"
         try:
             cp = subprocess.run(["git", "log", "-n 1", "HEAD", "--format=%cs"],
                                 capture_output=True, check=True, text=True)
         except (FileNotFoundError, subprocess.CalledProcessError):
             # support building wheel from sdist
@@ -65,37 +88,28 @@
 __version__ = "{self.metadata.version}"
 __release_date__ = "{committer_date}"
 __copyright_year__ = "{committer_year}"
 __author__ = "{self.metadata.core.authors[0]['name']}"
 __url__ = "{self.metadata.core.urls["Homepage"]}"
 """)
 
+        # Help
         index_html = (Path(*HELP_SRC_DIR, "html.header").read_text()
                       + markdown2.markdown_path(str(Path(*HELP_SRC_DIR, "index.txt")))
                       + Path(*HELP_SRC_DIR, "html.footer").read_text())
         Path(*HELP_SRC_DIR, "index.html").write_text(index_html)
 
-        try:
-            cp = subprocess.run(
-                ["pkg-config", "--variable=libexecdir", "Qt6Help"],
-                capture_output=True, text=True)
-            help_exec_dir = cp.stdout.strip()
-        except FileNotFoundError:
-            self.app.display_warning("pkg-config not installed")
-            help_exec_dir = None
-        if help_exec_dir:
-            help_generator = Path(help_exec_dir, "qhelpgenerator")
-        else:
-            # Ubuntu 22.04 doesn't provide Qt6Help.pc, 22.10 does but without libexecdir
-            # qhelpgenerator found in bin on 22.04, libexec from 22.10
-            help_generator = shutil.which(
-                "qhelpgenerator",
-                path="/usr/lib/qt6/libexec/:/usr/lib64/qt6/libexec/:"
-                     "/usr/lib/qt6/bin/:/usr/lib64/qt6/bin/")
-
+        help_generator = self.qt_tool_location("Qt6Help", "qhelpgenerator")
         cp = subprocess.run(
             [help_generator, "-c", "lccollection.qhcp", "-o", "lccollection.qhc"],
             cwd=Path(*HELP_SRC_DIR), check=True)
 
         Path(*HELP_DIR).mkdir(parents=True, exist_ok=True)
         shutil.copy(Path(*HELP_SRC_DIR, "lcdoc.qch"), Path(*HELP_DIR))
         shutil.copy(Path(*HELP_SRC_DIR, "lccollection.qhc"), Path(*HELP_DIR))
+
+        # Resources
+        rcc_generator = self.qt_tool_location("Qt6Core", "rcc")
+        Path(*RC_DIR).mkdir(parents=True, exist_ok=True)
+        cp = subprocess.run(
+            [rcc_generator, "-binary", Path(*RC_SRC_DIR, "linkchecker.qrc"),
+                "-o", Path(*RC_DIR, "linkchecker.rcc")], check=True)
```

### Comparing `LinkChecker_GUI-10.0.0a4/.gitignore` & `LinkChecker_GUI-10.0.0b1/.gitignore`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/LICENSE` & `LinkChecker_GUI-10.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `LinkChecker_GUI-10.0.0a4/README.md` & `LinkChecker_GUI-10.0.0b1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # LinkChecker-GUI
 
+[![Build Status](https://github.com/linkchecker/linkchecker-gui/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/linkchecker/linkchecker-gui/actions/workflows/build.yml)
 [![GPL-3](https://img.shields.io/badge/license-GPL3-d49a6a.svg)](https://opensource.org/licenses/GPL-3.0)
 
 This is the GUI client for [LinkChecker](https://linkchecker.github.io/linkchecker/).
 
 ## Installation
 
 Python 3.9 or later is needed. Using pip to install LinkChecker-GUI:
@@ -11,17 +12,17 @@
 `pip3 install linkchecker-gui`
 
 You may wish to first install the dependencies from you distribution e.g.:
 
 `apt install linkchecker python3-pyqt6.qsci python3-pyqt6.qthelp`
 
 The version in the pip repository may be old, to install the latest code first
-install qhelpgenerator e.g.
+install qhelpgenerator and rcc e.g.
 
-`apt install qt6-documentation-tools`
+`apt install qt6-documentation-tools qt6-base-dev-tools`
 
 Then:
 
 `pip3 install https://github.com/linkchecker/linkchecker-gui/archive/master.tar.gz`
 
 ## Usage
```

### Comparing `LinkChecker_GUI-10.0.0a4/pyproject.toml` & `LinkChecker_GUI-10.0.0b1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 dynamic = ["version"]
 description = "GUI for LinkChecker"
 readme = "README.md"
 authors = [{name = "LinkChecker Authors"}]
 maintainers = [{name = "LinkChecker Authors"}]
 classifiers = [
     "Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking",
-    "Development Status :: 3 - Alpha",
+    "Development Status :: 4 - Beta",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
```

### Comparing `LinkChecker_GUI-10.0.0a4/PKG-INFO` & `LinkChecker_GUI-10.0.0b1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 Metadata-Version: 2.1
 Name: LinkChecker-GUI
-Version: 10.0.0a4
+Version: 10.0.0b1
 Summary: GUI for LinkChecker
 Project-URL: Homepage, https://github.com/linkchecker/linkchecker-gui
 Author: LinkChecker Authors
 Maintainer: LinkChecker Authors
+License-File: COPYING.icons
 License-File: LICENSE
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Site Management :: Link Checking
 Requires-Python: >=3.9
 Requires-Dist: linkchecker>=10.1
 Requires-Dist: pyqt6
 Requires-Dist: pyqt6-qscintilla
 Description-Content-Type: text/markdown
 
 # LinkChecker-GUI
 
+[![Build Status](https://github.com/linkchecker/linkchecker-gui/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/linkchecker/linkchecker-gui/actions/workflows/build.yml)
 [![GPL-3](https://img.shields.io/badge/license-GPL3-d49a6a.svg)](https://opensource.org/licenses/GPL-3.0)
 
 This is the GUI client for [LinkChecker](https://linkchecker.github.io/linkchecker/).
 
 ## Installation
 
 Python 3.9 or later is needed. Using pip to install LinkChecker-GUI:
@@ -32,17 +34,17 @@
 `pip3 install linkchecker-gui`
 
 You may wish to first install the dependencies from you distribution e.g.:
 
 `apt install linkchecker python3-pyqt6.qsci python3-pyqt6.qthelp`
 
 The version in the pip repository may be old, to install the latest code first
-install qhelpgenerator e.g.
+install qhelpgenerator and rcc e.g.
 
-`apt install qt6-documentation-tools`
+`apt install qt6-documentation-tools qt6-base-dev-tools`
 
 Then:
 
 `pip3 install https://github.com/linkchecker/linkchecker-gui/archive/master.tar.gz`
 
 ## Usage
```

