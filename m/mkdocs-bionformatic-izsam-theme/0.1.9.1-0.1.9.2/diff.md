# Comparing `tmp/mkdocs-bionformatic-izsam-theme-0.1.9.1.tar.gz` & `tmp/mkdocs-bionformatic-izsam-theme-0.1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-bionformatic-izsam-theme-0.1.9.1.tar", last modified: Fri Dec  9 18:09:48 2022, max compression
+gzip compressed data, was "mkdocs-bionformatic-izsam-theme-0.1.9.2.tar", last modified: Tue Mar 28 18:29:29 2023, max compression
```

## Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1.tar` & `mkdocs-bionformatic-izsam-theme-0.1.9.2.tar`

### file list

```diff
@@ -1,119 +1,119 @@
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.978507 mkdocs-bionformatic-izsam-theme-0.1.9.1/
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1116 2022-12-09 18:08:41.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/LICENCE.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)      180 2022-12-09 18:08:41.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/MANIFEST.in
--rw-r--r--   0 alesdeluca   (501) staff       (20)     5657 2022-12-09 18:09:48.978278 mkdocs-bionformatic-izsam-theme-0.1.9.1/PKG-INFO
--rw-r--r--   0 alesdeluca   (501) staff       (20)     3000 2022-12-09 18:08:41.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/README.md
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.955557 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/
--rw-r--r--   0 alesdeluca   (501) staff       (20)      211 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/404.html
--rw-r--r--   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:08:41.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/__init__.py
--rw-r--r--   0 alesdeluca   (501) staff       (20)    10561 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/base.html
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.956757 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/
--rw-r--r--   0 alesdeluca   (501) staff       (20)      455 2022-12-09 18:08:49.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/footer.css
--rw-r--r--   0 alesdeluca   (501) staff       (20)     7797 2022-12-09 18:08:49.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/normalize.css
--rw-r--r--   0 alesdeluca   (501) staff       (20)     4889 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/pigments.css
--rw-r--r--   0 alesdeluca   (501) staff       (20)    11345 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/skeleton.css
--rw-r--r--   0 alesdeluca   (501) staff       (20)    29612 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/theme.css
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.952465 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.958488 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/
--rw-r--r--   0 alesdeluca   (501) staff       (20)   114752 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.ttf
--rw-r--r--   0 alesdeluca   (501) staff       (20)    26100 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    21128 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)   114624 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.ttf
--rw-r--r--   0 alesdeluca   (501) staff       (20)    26036 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    21168 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff2
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.961763 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/
--rw-r--r--   0 alesdeluca   (501) staff       (20)    30424 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    22992 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)    23572 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    17152 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)    31760 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    23648 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)    24632 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    18020 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)    31300 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    23472 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)    24456 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff
--rw-r--r--   0 alesdeluca   (501) staff       (20)    17804 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff2
--rw-r--r--   0 alesdeluca   (501) staff       (20)      526 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/footer.html
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.962515 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/
--rw-r--r--   0 alesdeluca   (501) staff       (20)     8805 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/favicon.ico
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.968919 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/
--rw-r--r--   0 alesdeluca   (501) staff       (20)      921 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      921 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      722 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      564 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-left-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      564 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-left.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-right-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-right.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      532 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      532 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1729 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/dots-vertical-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)     2419 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu-blu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)     2295 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      594 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      651 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/print-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      533 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/print.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      626 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/search-white.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)      626 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/search.svg
--rw-r--r--   0 alesdeluca   (501) staff       (20)    20299 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.png
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1169 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.svg
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.970139 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.976041 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/
--rw-r--r--   0 alesdeluca   (501) staff       (20)    24525 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ar.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    10349 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.da.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    13949 2022-12-09 18:09:05.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.de.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    15330 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.du.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    24406 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.es.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    20949 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.fi.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    25654 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.fr.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     6212 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.hi.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    21265 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.hu.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    24077 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.it.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     6125 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ja.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)      273 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.jp.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     3288 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.multi.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    15134 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.nl.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     9947 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.no.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    22141 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.pt.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    23157 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ro.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    19114 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ru.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    13504 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.stemmer.support.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     9635 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.sv.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     4947 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ta.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     3070 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.th.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    38283 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.tr.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     2558 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.vi.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     4917 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.zh.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)    99804 2022-12-09 18:08:51.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     4310 2022-12-09 18:08:52.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/search.js
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.976515 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-languages/
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1888 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-languages/theme-loc-en.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1970 2022-12-09 18:09:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-languages/theme-loc-it.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     2576 2022-12-09 18:08:52.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-localization.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)     4419 2022-12-09 18:08:52.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)      711 2022-12-09 18:08:52.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/zoom-img.js
--rw-r--r--   0 alesdeluca   (501) staff       (20)       25 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/main.html
--rw-r--r--   0 alesdeluca   (501) staff       (20)      184 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/mkdocs_theme.yml
--rw-r--r--   0 alesdeluca   (501) staff       (20)      498 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/nav.html
--rw-r--r--   0 alesdeluca   (501) staff       (20)      551 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/search.html
-drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2022-12-09 18:09:48.978002 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/
--rw-r--r--   0 alesdeluca   (501) staff       (20)     5657 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/PKG-INFO
--rw-r--r--   0 alesdeluca   (501) staff       (20)     5697 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/SOURCES.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)        1 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/dependency_links.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)       71 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/entry_points.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)        1 2022-12-09 18:08:47.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/not-zip-safe
--rw-r--r--   0 alesdeluca   (501) staff       (20)       14 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/requires.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)       26 2022-12-09 18:09:48.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/top_level.txt
--rw-r--r--   0 alesdeluca   (501) staff       (20)       38 2022-12-09 18:09:48.978576 mkdocs-bionformatic-izsam-theme-0.1.9.1/setup.cfg
--rw-r--r--   0 alesdeluca   (501) staff       (20)     1024 2022-12-09 18:08:41.000000 mkdocs-bionformatic-izsam-theme-0.1.9.1/setup.py
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.836506 mkdocs-bionformatic-izsam-theme-0.1.9.2/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1121 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/LICENCE.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      180 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/MANIFEST.in
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     5733 2023-03-28 18:29:29.836295 mkdocs-bionformatic-izsam-theme-0.1.9.2/PKG-INFO
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     3000 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/README.md
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.811712 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      211 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/404.html
+-rw-r--r--   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/__init__.py
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    10561 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/base.html
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.813387 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      455 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/footer.css
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     7797 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/normalize.css
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     4889 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/pigments.css
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    11345 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/skeleton.css
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    29724 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/theme.css
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.807174 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.815380 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)   114752 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.ttf
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    26100 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    21128 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)   114624 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.ttf
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    26036 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    21168 2023-03-28 18:28:04.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff2
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.818845 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    30424 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    22992 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    23572 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    17152 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    31760 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    23648 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    24632 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    18020 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    31300 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    23472 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    24456 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    17804 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff2
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      526 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/footer.html
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.819666 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     8805 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/favicon.ico
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.826263 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      921 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      921 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      722 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      564 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-left-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      564 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-left.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-right-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-right.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      532 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      666 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      532 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      698 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      566 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1729 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/dots-vertical-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     2419 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu-blu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     2295 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      594 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      651 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/print-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      533 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/print.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      626 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/search-white.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      626 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/search.svg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    20299 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.png
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1169 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.svg
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.827561 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.833881 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    24525 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ar.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    10349 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.da.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    13949 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.de.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    15330 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.du.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    24406 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.es.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    20949 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.fi.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    25654 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.fr.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     6212 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.hi.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    21265 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.hu.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    24077 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.it.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     6125 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ja.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      273 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.jp.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     3288 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.multi.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    15134 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.nl.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     9947 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.no.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    22141 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.pt.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    23157 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ro.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    19114 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ru.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    13504 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.stemmer.support.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     9635 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.sv.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     4947 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ta.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     3070 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.th.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    38283 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.tr.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     2558 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.vi.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     4917 2023-03-28 18:28:06.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.zh.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)    99804 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     4310 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/search.js
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.834372 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-languages/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1888 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-languages/theme-loc-en.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1970 2023-03-28 18:28:07.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-languages/theme-loc-it.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     2576 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-localization.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     4419 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      711 2023-03-28 18:28:03.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/zoom-img.js
+-rw-r--r--   0 alesdeluca   (501) staff       (20)       25 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/main.html
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      184 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/mkdocs_theme.yml
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      498 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/nav.html
+-rw-r--r--   0 alesdeluca   (501) staff       (20)      551 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/search.html
+drwxr-xr-x   0 alesdeluca   (501) staff       (20)        0 2023-03-28 18:29:29.835988 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     5733 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/PKG-INFO
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     5697 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/SOURCES.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)        1 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/dependency_links.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)       71 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/entry_points.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)        1 2023-03-28 18:28:02.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/not-zip-safe
+-rw-r--r--   0 alesdeluca   (501) staff       (20)       14 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/requires.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)       26 2023-03-28 18:29:29.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/top_level.txt
+-rw-r--r--   0 alesdeluca   (501) staff       (20)       38 2023-03-28 18:29:29.836581 mkdocs-bionformatic-izsam-theme-0.1.9.2/setup.cfg
+-rw-r--r--   0 alesdeluca   (501) staff       (20)     1024 2023-03-28 18:28:01.000000 mkdocs-bionformatic-izsam-theme-0.1.9.2/setup.py
```

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/LICENCE.txt` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/LICENCE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2021 Istituto Zooprofilattico Sperimentale dell'Abruzzo e del Molise "G. Caporale"
+Copyright 2021-2023 Istituto Zooprofilattico Sperimentale dell'Abruzzo e del Molise "G. Caporale"
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/PKG-INFO` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-bionformatic-izsam-theme
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: MkDocs theme designed for Bioiformatic Unit of the Istituto Zooprofilattico dell' Abruzzo e del Molise G. Caporale
 Home-page: UNKNOWN
 Author: Alessandro De Luca
 Author-email: al.deluca@izs.it
 License: MIT
 Keywords: MkDocs,Theme,Software documentation
 Platform: UNKNOWN
@@ -92,14 +92,19 @@
 
 #### Expand image
 
 `zoom-img.js` allows images to be expanded on click.
 
 # Change log
 
+## [0.1.9.2] - 2023-03-28
+
+### Bug fix for ordered list
+- Edited theme.css
+
 ## [0.1.9.1] - 2022-12-09
 
 ### Ux improvement for main menu in mobile view
 - Edited theme.css
 
 ## [0.1.9] - 2022-10-24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-bionformatic-izsam-theme Version: 0.1.9.1
+Metadata-Version: 2.1 Name: mkdocs-bionformatic-izsam-theme Version: 0.1.9.2
 Summary: MkDocs theme designed for Bioiformatic Unit of the Istituto
 Zooprofilattico dell' Abruzzo e del Molise G. Caporale Home-page: UNKNOWN
 Author: Alessandro De Luca Author-email: al.deluca@izs.it License: MIT
 Keywords: MkDocs,Theme,Software documentation Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENCE.txt # mkdocs-bioinformatic-
 izsam-theme This is an MkDocs theme designed to layout the documentation
 provided by Bioinformatic Unit of the Istituto Zooprofilattico Sperimentale
@@ -37,15 +37,16 @@
 "image title")` > A function in `theme.js` loops all images and if a title
 exists will append a `figcaption` tag after the image. #### Use icons inline To
 use icons inline inside the contents, please add the alt attribute `inline-
 icon`: ``` ![inline-icon](icona.png) ``` > Images will have inherent size and
 displayed inline. #### Use diagram as images (no plantuml) To use diagram
 inside the contents as images, please add the alt attribute `diagram` to avoid
 box shadow. ``` ![diagram](file.png) ``` #### Expand image `zoom-img.js` allows
-images to be expanded on click. # Change log ## [0.1.9.1] - 2022-12-09 ### Ux
+images to be expanded on click. # Change log ## [0.1.9.2] - 2023-03-28 ### Bug
+fix for ordered list - Edited theme.css ## [0.1.9.1] - 2022-12-09 ### Ux
 improvement for main menu in mobile view - Edited theme.css ## [0.1.9] - 2022-
 10-24 ### Small fix on Ux improvement for main menu in mobile view - Edited
 theme.css and base.html ## [0.1.8] - 2022-10-24 ### Ux improvement for main
 menu in mobile view - Edited theme.css and base.html ## [0.1.7] - 2022-05-12
 ### Debug and refactoring for theme.js - Edited theme.js ## [0.1.6] - 2022-05-
 12 ### Fix for image caption function - Edited theme.css and theme.js ##
 [0.1.5] - 2022-05-12 ### Added support for image caption - Edited theme.css and
```

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/README.md` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/base.html` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/base.html`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/normalize.css` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/normalize.css`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/pigments.css` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/pigments.css`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/skeleton.css` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/skeleton.css`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/css/theme.css` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/css/theme.css`

 * *Files 0% similar despite different names*

```diff
@@ -1114,14 +1114,25 @@
 
 .search-page .contents div#mkdocs-search-results article p.location {
   opacity: 0.5;
 }
 
 .contents ul, .contents ol {
   padding-left: 2.1rem;
+}
+
+.contents ol {
+  list-style: decimal outside;
+}
+
+.contents ul{
+  list-style: disc outside;
+}
+
+.contents ul {
   list-style: disc outside;
 }
 
 .contents table {
   display: block;
   width: 100%;
   overflow-x: scroll;
```

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.ttf` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.ttf` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Roboto_Mono/RobotoMono-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold-Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Bold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular-Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-Regular.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold-Italic.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff2` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/fonts/Titillium_Web/TitilliumWeb-SemiBold.woff2`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/footer.html` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/footer.html`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/favicon.ico` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/annotation-warning.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/annotation-warning.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-left-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-left-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-left.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-left.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-right-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-right-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/arrow-right.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/arrow-right.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down-circle.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down-circle.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-down.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-down.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up-circle.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up-circle.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/chevron-up.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/chevron-up.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-circle.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-circle.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/close.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/close.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/dots-vertical-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/dots-vertical-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu-blu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu-blu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/menu.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/menu.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/print-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/print-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/print.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/print.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/search-white.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/search-white.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/iconic/search.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/iconic/search.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.png` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.png`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.svg` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/img/piattaforma-genpat-logo.svg`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ar.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ar.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.da.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.da.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.de.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.de.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.du.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.du.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.es.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.es.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.fi.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.fi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.fr.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.fr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.hi.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.hi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.hu.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.hu.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.it.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ja.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ja.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.multi.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.multi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.nl.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.nl.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.no.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.no.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.pt.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.pt.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ro.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ro.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ru.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ru.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.stemmer.support.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.stemmer.support.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.sv.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.sv.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.ta.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.ta.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.th.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.th.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.tr.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.tr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.vi.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.vi.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr-languages/lunr.zh.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr-languages/lunr.zh.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/lunr.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/lunr.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/search.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/search.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-languages/theme-loc-en.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-languages/theme-loc-en.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-languages/theme-loc-it.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-languages/theme-loc-it.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme-localization.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme-localization.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/theme.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/theme.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/js/zoom-img.js` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/js/zoom-img.js`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/bioinformatic_izsam_theme/search.html` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/bioinformatic_izsam_theme/search.html`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/PKG-INFO` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-bionformatic-izsam-theme
-Version: 0.1.9.1
+Version: 0.1.9.2
 Summary: MkDocs theme designed for Bioiformatic Unit of the Istituto Zooprofilattico dell' Abruzzo e del Molise G. Caporale
 Home-page: UNKNOWN
 Author: Alessandro De Luca
 Author-email: al.deluca@izs.it
 License: MIT
 Keywords: MkDocs,Theme,Software documentation
 Platform: UNKNOWN
@@ -92,14 +92,19 @@
 
 #### Expand image
 
 `zoom-img.js` allows images to be expanded on click.
 
 # Change log
 
+## [0.1.9.2] - 2023-03-28
+
+### Bug fix for ordered list
+- Edited theme.css
+
 ## [0.1.9.1] - 2022-12-09
 
 ### Ux improvement for main menu in mobile view
 - Edited theme.css
 
 ## [0.1.9] - 2022-10-24
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-bionformatic-izsam-theme Version: 0.1.9.1
+Metadata-Version: 2.1 Name: mkdocs-bionformatic-izsam-theme Version: 0.1.9.2
 Summary: MkDocs theme designed for Bioiformatic Unit of the Istituto
 Zooprofilattico dell' Abruzzo e del Molise G. Caporale Home-page: UNKNOWN
 Author: Alessandro De Luca Author-email: al.deluca@izs.it License: MIT
 Keywords: MkDocs,Theme,Software documentation Platform: UNKNOWN Description-
 Content-Type: text/markdown License-File: LICENCE.txt # mkdocs-bioinformatic-
 izsam-theme This is an MkDocs theme designed to layout the documentation
 provided by Bioinformatic Unit of the Istituto Zooprofilattico Sperimentale
@@ -37,15 +37,16 @@
 "image title")` > A function in `theme.js` loops all images and if a title
 exists will append a `figcaption` tag after the image. #### Use icons inline To
 use icons inline inside the contents, please add the alt attribute `inline-
 icon`: ``` ![inline-icon](icona.png) ``` > Images will have inherent size and
 displayed inline. #### Use diagram as images (no plantuml) To use diagram
 inside the contents as images, please add the alt attribute `diagram` to avoid
 box shadow. ``` ![diagram](file.png) ``` #### Expand image `zoom-img.js` allows
-images to be expanded on click. # Change log ## [0.1.9.1] - 2022-12-09 ### Ux
+images to be expanded on click. # Change log ## [0.1.9.2] - 2023-03-28 ### Bug
+fix for ordered list - Edited theme.css ## [0.1.9.1] - 2022-12-09 ### Ux
 improvement for main menu in mobile view - Edited theme.css ## [0.1.9] - 2022-
 10-24 ### Small fix on Ux improvement for main menu in mobile view - Edited
 theme.css and base.html ## [0.1.8] - 2022-10-24 ### Ux improvement for main
 menu in mobile view - Edited theme.css and base.html ## [0.1.7] - 2022-05-12
 ### Debug and refactoring for theme.js - Edited theme.js ## [0.1.6] - 2022-05-
 12 ### Fix for image caption function - Edited theme.css and theme.js ##
 [0.1.5] - 2022-05-12 ### Added support for image caption - Edited theme.css and
```

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/mkdocs_bionformatic_izsam_theme.egg-info/SOURCES.txt` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/mkdocs_bionformatic_izsam_theme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-bionformatic-izsam-theme-0.1.9.1/setup.py` & `mkdocs-bionformatic-izsam-theme-0.1.9.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open('README.md') as readme_file:
     README = readme_file.read()
 
 with open('HISTORY.md') as history_file:
     HISTORY = history_file.read()
 
-VERSION = '0.1.9.1'
+VERSION = '0.1.9.2'
 
 setup(
     name='mkdocs-bionformatic-izsam-theme',
     version=VERSION,
     url='',
     description="MkDocs theme designed for Bioiformatic Unit of the Istituto Zooprofilattico dell' Abruzzo e del Molise G. Caporale",
     long_description_content_type="text/markdown",
```

