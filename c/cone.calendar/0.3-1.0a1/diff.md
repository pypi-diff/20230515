# Comparing `tmp/cone.calendar-0.3.tar.gz` & `tmp/cone.calendar-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cone.calendar-0.3.tar", last modified: Thu Oct  6 07:30:21 2022, max compression
+gzip compressed data, was "cone.calendar-1.0a1.tar", last modified: Mon May 15 12:02:26 2023, max compression
```

## Comparing `cone.calendar-0.3.tar` & `cone.calendar-1.0a1.tar`

### file list

```diff
@@ -1,226 +1,227 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:21.000000 cone.calendar-0.3/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      344 2022-10-06 07:30:20.000000 cone.calendar-0.3/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1373 2022-10-06 07:30:20.000000 cone.calendar-0.3/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2022-10-06 07:30:20.000000 cone.calendar-0.3/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7935 2022-10-06 07:30:21.000000 cone.calendar-0.3/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4122 2022-10-06 07:30:20.000000 cone.calendar-0.3/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2022-10-06 07:30:21.000000 cone.calendar-0.3/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1378 2022-10-06 07:30:20.000000 cone.calendar-0.3/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1345 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      188 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      606 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/calendar.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11359 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/calendar.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      417 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/calendar.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8197 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/calendar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3330 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/calendar.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/
--rw-r--r--   0 rnix      (1000) rnix      (1000)    30924 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   394028 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    15251 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)   131347 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5565 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5751 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/gcal.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2185 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/gcal.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2158 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/af.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2457 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-dz.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3514 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-ly.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2415 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-ma.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2907 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-sa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2418 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-tn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3837 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2839 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/bg.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2357 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3314 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/cs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1967 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/da.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2319 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/de-at.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2308 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/de.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3645 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/el.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-au.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1268 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1896 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-gb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1279 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-ie.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-nz.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2436 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/es-do.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2419 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/es.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2228 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/eu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2964 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2837 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2119 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr-ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2135 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr-ch.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2123 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2332 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/gl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2933 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/he.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3753 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2908 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2812 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2179 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/id.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2755 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/is.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2172 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/it.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2198 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ja.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/kk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2100 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ko.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2675 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3183 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2744 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2828 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/mk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2232 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ms-my.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2223 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ms.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2028 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2808 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nl-be.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2796 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1990 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2708 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2209 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pt-br.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2153 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2160 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ro.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5603 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ru.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2964 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3173 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3528 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sr-cyrl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3058 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2094 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3433 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/th.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2337 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/tr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4261 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/uk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2555 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/vi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3128 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/zh-cn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2686 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/zh-tw.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   157310 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale-all.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:21.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2392 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/af.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2219 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-dz.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4179 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-ly.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2251 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-ma.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3165 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-sa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2164 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-tn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4688 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3089 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/az.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5121 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/be.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3168 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bg.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4021 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4803 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3116 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/br.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4479 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2718 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6162 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2518 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2738 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cy.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1905 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/da.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2795 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/de-at.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2718 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/de.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2679 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/dv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3873 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/el.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2169 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-au.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2015 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2175 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-gb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-ie.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2178 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-nz.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2464 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/eo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2709 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/es-do.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2726 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/es.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2919 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/et.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2194 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/eu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3287 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3635 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1957 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1921 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr-ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2083 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr-ch.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2057 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2425 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fy.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2422 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/gd.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2580 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/gl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3488 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/he.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4164 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4608 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3781 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3428 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hy-am.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2672 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/id.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4279 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/is.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2254 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/it.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2228 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ja.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2681 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/jv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3903 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ka.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2759 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/kk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2579 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/km.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2036 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ko.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2770 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ky.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4468 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2827 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4110 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3655 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3788 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/me.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2243 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3190 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3489 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ml.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5870 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2631 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ms-my.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ms.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3252 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/my.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2061 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nb.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4200 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ne.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3211 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nl-be.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3191 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1917 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4360 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pa-in.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3699 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2075 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pt-br.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2169 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2397 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ro.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8162 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ru.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2088 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/se.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2914 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/si.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5292 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5938 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2259 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sq.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4248 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sr-cyrl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3766 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ss.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2202 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1915 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sw.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4923 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ta.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3612 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/te.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2245 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tet.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2909 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/th.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2003 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tl-ph.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3814 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tlh.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2657 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3336 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1960 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzm-latn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzm.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5642 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/uk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/uz.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2540 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/vi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2444 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/x-pseudo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/yo.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4403 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-cn.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3379 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-hk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3326 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-tw.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   303097 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locales.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   193988 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/locales.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   425984 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment-with-locales.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)   255277 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment-with-locales.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    61317 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      466 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/interfaces.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:21.000000 cone.calendar-0.3/src/cone/calendar/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/locale/cone.calendar.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/locale/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:21.000000 cone.calendar-0.3/src/cone/calendar/locale/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/locale/de/LC_MESSAGES/cone.calendar.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8640 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone/calendar/tests.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     7935 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11337 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2022-10-06 07:30:20.000000 cone.calendar-0.3/src/cone.calendar.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      443 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1373 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6415 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4122 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1380 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.468230 cone.calendar-1.0a1/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      473 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2865 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      606 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/calendar.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11359 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/calendar.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/browser/static/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      417 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/cone.calendar.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8197 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/cone.calendar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3330 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/cone.calendar.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    30924 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   394028 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    15251 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   131347 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5565 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5751 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/gcal.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2185 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/gcal.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.480230 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2158 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/af.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2457 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-dz.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3514 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-ly.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2415 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-ma.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2907 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-sa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2418 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-tn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3837 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2839 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/bg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2357 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3314 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/cs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1967 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/da.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2319 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/de-at.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2308 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/de.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3645 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/el.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-au.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1268 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1896 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-gb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1279 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-ie.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1900 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-nz.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2436 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/es-do.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2419 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/es.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2228 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/eu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2964 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2837 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2119 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr-ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2135 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr-ch.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2123 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2332 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/gl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2933 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/he.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3753 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2908 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2812 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2179 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/id.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2755 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/is.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2172 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/it.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2198 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ja.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2864 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/kk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2100 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ko.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2675 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3183 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2744 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2828 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/mk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2232 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ms-my.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2223 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ms.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2028 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2808 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nl-be.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2796 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1990 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2708 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2209 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pt-br.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2153 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2160 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ro.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5603 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ru.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2964 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3173 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3528 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sr-cyrl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3058 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2094 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3433 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/th.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2337 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/tr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4261 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/uk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2555 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/vi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3128 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/zh-cn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2686 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/zh-tw.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   157310 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale-all.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.480230 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2392 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/af.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2219 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-dz.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4179 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-ly.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2251 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-ma.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3165 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-sa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2164 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-tn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4688 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3089 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/az.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5121 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/be.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3168 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4021 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4803 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3116 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/br.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4479 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2718 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6162 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2518 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2738 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cy.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1905 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/da.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2795 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/de-at.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2718 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/de.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2679 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/dv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3873 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/el.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2169 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-au.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2015 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2175 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-gb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-ie.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2178 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-nz.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2464 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/eo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2709 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/es-do.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2726 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/es.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2919 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/et.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2194 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/eu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3287 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3635 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1957 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1921 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr-ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2083 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr-ch.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2057 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2425 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fy.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2422 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/gd.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2580 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/gl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3488 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/he.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4164 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4608 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3781 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3428 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hy-am.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2672 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/id.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4279 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/is.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2254 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/it.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2228 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ja.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2681 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/jv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3903 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ka.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2759 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/kk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2579 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/km.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2036 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ko.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2770 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ky.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4468 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2827 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4110 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3655 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3788 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/me.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2243 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3190 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3489 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ml.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5870 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2631 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ms-my.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ms.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3252 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/my.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2061 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nb.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4200 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ne.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3211 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nl-be.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3191 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1917 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4360 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pa-in.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3699 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2075 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pt-br.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2169 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2397 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ro.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8162 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ru.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2088 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/se.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2914 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/si.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5292 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5938 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2259 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sq.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4248 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sr-cyrl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3766 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2829 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ss.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2202 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1915 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sw.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4923 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ta.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3612 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/te.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2245 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tet.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2909 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/th.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2003 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tl-ph.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3814 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tlh.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2657 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3336 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1960 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzm-latn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2574 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzm.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5642 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/uk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/uz.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2540 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/vi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2444 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/x-pseudo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2173 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/yo.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4403 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-cn.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3379 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-hk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3326 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-tw.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   303097 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locales.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   193988 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locales.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   425984 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment-with-locales.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   255277 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment-with-locales.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    61317 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      466 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/interfaces.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/src/cone/calendar/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/locale/cone.calendar.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone/calendar/locale/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.488230 cone.calendar-1.0a1/src/cone/calendar/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/locale/de/LC_MESSAGES/cone.calendar.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12123 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone/calendar/tests.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:02:26.472230 cone.calendar-1.0a1/src/cone.calendar.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6415 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11379 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       64 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2023-05-15 12:02:26.000000 cone.calendar-1.0a1/src/cone.calendar.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cone.calendar-0.3/LICENSE.rst` & `cone.calendar-1.0a1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/README.rst` & `cone.calendar-1.0a1/README.rst`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/setup.py` & `cone.calendar-1.0a1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '0.3'
+version = '1.0a1'
 shortdesc = 'jQuery Fullcalendar integration for cone.app'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/calendar.pt` & `cone.calendar-1.0a1/src/cone/calendar/browser/calendar.pt`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/calendar.py` & `cone.calendar-1.0a1/src/cone/calendar/browser/calendar.py`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/calendar.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/cone.calendar.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/calendar.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/calendar/cone.calendar.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.css` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.css` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.css`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.css` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.min.css` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.min.css`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/gcal.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/gcal.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/gcal.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/gcal.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/af.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/af.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-dz.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-ly.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-ma.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-sa.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar-tn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ar.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ar.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/bg.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/bg.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/cs.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/cs.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/da.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/da.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/de-at.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/de.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/de.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/el.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/el.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-au.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-gb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-ie.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/en-nz.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/es-do.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/es.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/es.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/eu.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/eu.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fa.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fa.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr-ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr-ch.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/fr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/fr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/gl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/gl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/he.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/he.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/hu.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/hu.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/id.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/id.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/is.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/is.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/it.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/it.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ja.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ja.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/kk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/kk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ko.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ko.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lt.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lt.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/lv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/lv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/mk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/mk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ms-my.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ms.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ms.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nl-be.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/nn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/nn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pt-br.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/pt.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/pt.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ro.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ro.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/ru.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/ru.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sr-cyrl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/sv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/sv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/th.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/th.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/tr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/tr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/uk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/uk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/vi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/vi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/zh-cn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale/zh-tw.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/fullcalendar/locale-all.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/fullcalendar/locale-all.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/af.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/af.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-dz.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-dz.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-ly.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-ly.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-ma.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-ma.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-sa.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-sa.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar-tn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar-tn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ar.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ar.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/az.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/az.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/be.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/be.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bg.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bg.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/br.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/br.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/bs.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/bs.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cs.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cs.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/cy.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/cy.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/da.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/da.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/de-at.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/de-at.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/de.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/de.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/dv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/dv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/el.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/el.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-au.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-au.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-gb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-gb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-ie.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-ie.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/en-nz.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/en-nz.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/eo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/eo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/es-do.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/es-do.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/es.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/es.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/et.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/et.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/eu.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/eu.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fa.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fa.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr-ca.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr-ca.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr-ch.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr-ch.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/fy.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/fy.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/gd.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/gd.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/gl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/gl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/he.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/he.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hu.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hu.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/hy-am.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/hy-am.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/id.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/id.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/is.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/is.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/it.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/it.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ja.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ja.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/jv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/jv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ka.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ka.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/kk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/kk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/km.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/km.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ko.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ko.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ky.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ky.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lt.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lt.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/lv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/lv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/me.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/me.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ml.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ml.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/mr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/mr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ms-my.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ms-my.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ms.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ms.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/my.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/my.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nb.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nb.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ne.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ne.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nl-be.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nl-be.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/nn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/nn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pa-in.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pa-in.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pt-br.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pt-br.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/pt.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/pt.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ro.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ro.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ru.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ru.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/se.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/se.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/si.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/si.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sq.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sq.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sr-cyrl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sr-cyrl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ss.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ss.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sv.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sv.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/sw.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/sw.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/ta.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/ta.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/te.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/te.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tet.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tet.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/th.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/th.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tl-ph.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tl-ph.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tlh.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tlh.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tr.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tr.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzl.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzl.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzm-latn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzm-latn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/tzm.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/tzm.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/uk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/uk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/uz.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/uz.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/vi.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/vi.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/x-pseudo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/x-pseudo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/yo.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/yo.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-cn.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-cn.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-hk.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-hk.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locale/zh-tw.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locale/zh-tw.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locales.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locales.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/locales.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/locales.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment-with-locales.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment-with-locales.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment-with-locales.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment-with-locales.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone/calendar/browser/static/moment/moment.min.js` & `cone.calendar-1.0a1/src/cone/calendar/browser/static/moment/moment.min.js`

 * *Files identical despite different names*

### Comparing `cone.calendar-0.3/src/cone.calendar.egg-info/SOURCES.txt` & `cone.calendar-1.0a1/src/cone.calendar.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 src/cone.calendar.egg-info/top_level.txt
 src/cone/calendar/__init__.py
 src/cone/calendar/interfaces.py
 src/cone/calendar/tests.py
 src/cone/calendar/browser/__init__.py
 src/cone/calendar/browser/calendar.pt
 src/cone/calendar/browser/calendar.py
-src/cone/calendar/browser/static/calendar.css
-src/cone/calendar/browser/static/calendar.js
-src/cone/calendar/browser/static/calendar.min.js
+src/cone/calendar/browser/static/calendar/cone.calendar.css
+src/cone/calendar/browser/static/calendar/cone.calendar.js
+src/cone/calendar/browser/static/calendar/cone.calendar.min.js
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.css
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.js
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.css
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.min.js
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.css
 src/cone/calendar/browser/static/fullcalendar/fullcalendar.print.min.css
 src/cone/calendar/browser/static/fullcalendar/gcal.js
```

