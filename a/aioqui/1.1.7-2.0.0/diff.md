# Comparing `tmp/aioqui-1.1.7.tar.gz` & `tmp/aioqui-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioqui-1.1.7.tar", last modified: Sun May 14 18:21:33 2023, max compression
+gzip compressed data, was "aioqui-2.0.0.tar", last modified: Mon May 15 09:05:51 2023, max compression
```

## Comparing `aioqui-1.1.7.tar` & `aioqui-2.0.0.tar`

### file list

```diff
@@ -1,368 +1,368 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.743716 aioqui-1.1.7/
--rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-1.1.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2641 2023-05-14 18:21:33.743716 aioqui-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      401 2023-05-14 05:04:46.000000 aioqui-1.1.7/README.md
--rw-rw-rw-   0        0        0     1551 2023-05-14 18:21:10.000000 aioqui-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-14 18:21:33.743716 aioqui-1.1.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.451689 aioqui-1.1.7/src/
--rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-1.1.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.454688 aioqui-1.1.7/src/aioqui/
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.445700 aioqui-1.1.7/src/aioqui/.assets/
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.702714 aioqui-1.1.7/src/aioqui/.assets/icons/
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/activity.svg
--rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/airplay.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/alert-circle.svg
--rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/alert-octagon.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/alert-triangle.svg
--rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/align-center.svg
--rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/align-justify.svg
--rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/align-left.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/align-right.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/anchor.svg
--rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/aperture.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/archive.svg
--rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-down-circle.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-down-left.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-down-right.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-down.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-left-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-left.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-right-circle.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-right.svg
--rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-up-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-up-left.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-up-right.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/arrow-up.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/at-sign.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/award.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bar-chart-2.svg
--rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bar-chart.svg
--rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/battery-charging.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/battery.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bell-off.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bell.svg
--rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bluetooth.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bold.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/book-open.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/book.svg
--rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/bookmark.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/box.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/briefcase.svg
--rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/calendar.svg
--rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/camera-off.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/camera.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cast.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/check-circle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/check-square.svg
--rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/check.svg
--rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevron-down.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevron-left.svg
--rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevron-right.svg
--rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevron-up.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevrons-down.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevrons-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevrons-right.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chevrons-up.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/chrome.svg
--rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/circle.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/clipboard.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/clock.svg
--rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud-drizzle.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud-lightning.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud-off.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud-rain.svg
--rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud-snow.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cloud.svg
--rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/code.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/codepen.svg
--rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/codesandbox.svg
--rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/coffee.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/columns.svg
--rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/command.svg
--rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/compass.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/copy.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-down-left.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-down-right.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-left-down.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-left-up.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-right-down.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-right-up.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-up-left.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/corner-up-right.svg
--rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/cpu.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/credit-card.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/crop.svg
--rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/crosshair.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/database.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/delete.svg
--rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/disc.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/divide-circle.svg
--rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/divide-square.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/divide.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/dollar-sign.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/download-cloud.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/download.svg
--rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/dribbble.svg
--rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/droplet.svg
--rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/edit-2.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/edit-3.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/edit.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/external-link.svg
--rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/eye-off.svg
--rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/eye.svg
--rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/facebook.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/fast-forward.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/feather.svg
--rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/figma.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/file-minus.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/file-plus.svg
--rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/file-text.svg
--rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/file.svg
--rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/film.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/filter.svg
--rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/flag.svg
--rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/folder-minus.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/folder-plus.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/folder.svg
--rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/framer.svg
--rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/frown.svg
--rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/gift.svg
--rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/git-branch.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/git-commit.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/git-merge.svg
--rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/git-pull-request.svg
--rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/github.svg
--rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/gitlab.svg
--rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/globe.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/grid.svg
--rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/hard-drive.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/hash.svg
--rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/headphones.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/heart.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/help-circle.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/hexagon.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/home.svg
--rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/image.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/inbox.svg
--rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/info.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/instagram.svg
--rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/italic.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/key.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/layers.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/layout.svg
--rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/life-buoy.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/link-2.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/link.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/linkedin.svg
--rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/list.svg
--rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/loader.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/lock.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/log-in.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/log-out.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/mail.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/map-pin.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/map.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/maximize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/maximize.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/meh.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/menu.svg
--rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/message-circle.svg
--rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/message-square.svg
--rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/mic-off.svg
--rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/mic.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/minimize-2.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/minimize.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/minus-circle.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/minus-square.svg
--rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/minus.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/monitor.svg
--rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/moon.svg
--rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/more-horizontal.svg
--rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/more-vertical.svg
--rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/mouse-pointer.svg
--rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/move.svg
--rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/music.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/navigation-2.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/navigation.svg
--rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/octagon.svg
--rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/package.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/paperclip.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/pause-circle.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/pause.svg
--rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/pen-tool.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/percent.svg
--rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-call.svg
--rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-forwarded.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-incoming.svg
--rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-missed.svg
--rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-off.svg
--rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone-outgoing.svg
--rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/phone.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/pie-chart.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/play-circle.svg
--rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/play.svg
--rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/plus-circle-gray.svg
--rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/plus-circle.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/plus-square.svg
--rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/plus.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/pocket.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/power.svg
--rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/printer.svg
--rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/radio.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/refresh-ccw.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/refresh-cw.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/repeat.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/rewind.svg
--rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/rotate-ccw.svg
--rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/rotate-cw.svg
--rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/rss.svg
--rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/save.svg
--rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/schedule.svg
--rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/scissors.svg
--rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/search.svg
--rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/send.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/server.svg
--rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/settings.svg
--rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/share-2.svg
--rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/share.svg
--rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/shield-off.svg
--rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/shield.svg
--rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/shopping-bag.svg
--rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/shopping-cart.svg
--rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/shuffle.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/sidebar.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/skip-back.svg
--rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/skip-forward.svg
--rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/slack.svg
--rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/slash.svg
--rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/sliders.svg
--rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/smartphone.svg
--rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/smile.svg
--rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/speaker.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/square.svg
--rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-1.1.7/src/aioqui/.assets/icons/star-fill.svg
--rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/star.svg
--rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/stop-circle.svg
--rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/sun.svg
--rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/sunrise.svg
--rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/sunset.svg
--rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/table.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/tablet.svg
--rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/tag.svg
--rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/target.svg
--rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/terminal.svg
--rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/thermometer.svg
--rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/thumbs-down.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/thumbs-up.svg
--rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/toggle-left.svg
--rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/toggle-right.svg
--rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/tool.svg
--rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/trash-2.svg
--rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/trash.svg
--rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/trello.svg
--rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/trending-down.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/trending-up.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/triangle.svg
--rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/truck.svg
--rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/tv.svg
--rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/twitch.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/twitter.svg
--rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/type.svg
--rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/umbrella.svg
--rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/underline.svg
--rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/unlock.svg
--rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/upload-cloud.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/upload.svg
--rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/user-check.svg
--rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/user-minus.svg
--rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/user-plus.svg
--rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/user-x.svg
--rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/user.svg
--rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/users.svg
--rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/video-off.svg
--rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/video.svg
--rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/voicemail.svg
--rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/volume-1.svg
--rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/volume-2.svg
--rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/volume-x.svg
--rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/volume.svg
--rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/watch.svg
--rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/wifi-off.svg
--rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/wifi.svg
--rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/wind.svg
--rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/x-circle-gray.svg
--rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/x-circle.svg
--rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/x-octagon.svg
--rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/x-square.svg
--rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/x.svg
--rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/youtube.svg
--rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/zap-off.svg
--rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/zap.svg
--rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/zoom-in.svg
--rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-1.1.7/src/aioqui/.assets/icons/zoom-out.svg
--rw-rw-rw-   0        0        0      161 2023-05-14 00:40:20.000000 aioqui-1.1.7/src/aioqui/__init__.py
--rw-rw-rw-   0        0        0      443 2023-05-14 00:18:53.000000 aioqui-1.1.7/src/aioqui/contextapi.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.707690 aioqui-1.1.7/src/aioqui/enums/
--rw-rw-rw-   0        0        0      222 2023-05-14 01:09:08.000000 aioqui-1.1.7/src/aioqui/enums/__init__.py
--rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-1.1.7/src/aioqui/enums/alignment.py
--rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-1.1.7/src/aioqui/enums/elide_mode.py
--rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-1.1.7/src/aioqui/enums/orientation.py
--rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-1.1.7/src/aioqui/enums/scroll_policy.py
--rw-rw-rw-   0        0        0      228 2023-05-14 15:05:15.000000 aioqui-1.1.7/src/aioqui/enums/size_policy.py
--rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-1.1.7/src/aioqui/enums/window_hint.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.713689 aioqui-1.1.7/src/aioqui/misc/
--rw-rw-rw-   0        0        0      225 2023-05-14 18:12:36.000000 aioqui-1.1.7/src/aioqui/misc/__init__.py
--rw-rw-rw-   0        0        0     1931 2023-05-12 16:41:32.000000 aioqui-1.1.7/src/aioqui/misc/aiorequest.py
--rw-rw-rw-   0        0        0     1062 2023-05-02 22:09:01.000000 aioqui-1.1.7/src/aioqui/misc/ctq.py
--rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-1.1.7/src/aioqui/misc/dialogs.py
--rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-1.1.7/src/aioqui/misc/parser.py
--rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-1.1.7/src/aioqui/misc/server.py
--rw-rw-rw-   0        0        0      679 2023-05-14 00:09:55.000000 aioqui-1.1.7/src/aioqui/misc/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.716699 aioqui-1.1.7/src/aioqui/objects/
--rw-rw-rw-   0        0        0      107 2023-05-14 01:38:47.000000 aioqui-1.1.7/src/aioqui/objects/__init__.py
--rw-rw-rw-   0        0        0     2407 2023-05-14 02:31:01.000000 aioqui-1.1.7/src/aioqui/objects/context_obj.py
--rw-rw-rw-   0        0        0     2666 2023-05-14 07:00:25.000000 aioqui-1.1.7/src/aioqui/objects/evented_obj.py
--rw-rw-rw-   0        0        0     3053 2023-05-14 15:04:27.000000 aioqui-1.1.7/src/aioqui/objects/sized_obj.py
--rw-rw-rw-   0        0        0     1135 2023-05-14 00:38:47.000000 aioqui-1.1.7/src/aioqui/qasyncio.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.719691 aioqui-1.1.7/src/aioqui/types/
--rw-rw-rw-   0        0        0       71 2023-05-14 03:02:21.000000 aioqui-1.1.7/src/aioqui/types/__init__.py
--rw-rw-rw-   0        0        0      167 2023-05-14 04:46:50.000000 aioqui-1.1.7/src/aioqui/types/common.py
--rw-rw-rw-   0        0        0     3539 2023-05-14 00:07:05.000000 aioqui-1.1.7/src/aioqui/types/icon.py
--rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 aioqui-1.1.7/src/aioqui/types/size.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.733689 aioqui-1.1.7/src/aioqui/widgets/
--rw-rw-rw-   0        0        0      589 2023-05-13 22:32:44.000000 aioqui-1.1.7/src/aioqui/widgets/__init__.py
--rw-rw-rw-   0        0        0      846 2023-05-14 03:24:34.000000 aioqui-1.1.7/src/aioqui/widgets/button.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.739690 aioqui-1.1.7/src/aioqui/widgets/custom/
--rw-rw-rw-   0        0        0      236 2023-05-14 05:29:24.000000 aioqui-1.1.7/src/aioqui/widgets/custom/__init__.py
--rw-rw-rw-   0        0        0     5557 2023-05-13 22:43:13.000000 aioqui-1.1.7/src/aioqui/widgets/custom/date_picker.py
--rw-rw-rw-   0        0        0     1897 2023-05-14 15:09:59.000000 aioqui-1.1.7/src/aioqui/widgets/custom/error_label.py
--rw-rw-rw-   0        0        0     2029 2023-05-14 05:11:48.000000 aioqui-1.1.7/src/aioqui/widgets/custom/favourite_button.py
--rw-rw-rw-   0        0        0     2720 2023-05-14 05:11:48.000000 aioqui-1.1.7/src/aioqui/widgets/custom/image_button.py
--rw-rw-rw-   0        0        0     1436 2023-05-14 15:07:11.000000 aioqui-1.1.7/src/aioqui/widgets/custom/menu_button.py
--rw-rw-rw-   0        0        0     1270 2023-05-14 05:30:25.000000 aioqui-1.1.7/src/aioqui/widgets/custom/search_bar.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.742714 aioqui-1.1.7/src/aioqui/widgets/extensions/
--rw-rw-rw-   0        0        0      127 2023-05-14 01:36:51.000000 aioqui-1.1.7/src/aioqui/widgets/extensions/__init__.py
--rw-rw-rw-   0        0        0     1899 2023-05-13 21:23:34.000000 aioqui-1.1.7/src/aioqui/widgets/extensions/layout_ext.py
--rw-rw-rw-   0        0        0      676 2023-05-13 21:23:34.000000 aioqui-1.1.7/src/aioqui/widgets/extensions/side_menu_ext.py
--rw-rw-rw-   0        0        0     1954 2023-05-14 04:55:20.000000 aioqui-1.1.7/src/aioqui/widgets/extensions/splitter_widget_ext.py
--rw-rw-rw-   0        0        0      792 2023-05-14 05:09:16.000000 aioqui-1.1.7/src/aioqui/widgets/frame.py
--rw-rw-rw-   0        0        0     1572 2023-05-14 07:20:30.000000 aioqui-1.1.7/src/aioqui/widgets/label.py
--rw-rw-rw-   0        0        0     1311 2023-05-14 01:40:16.000000 aioqui-1.1.7/src/aioqui/widgets/layout.py
--rw-rw-rw-   0        0        0     1056 2023-05-14 03:24:34.000000 aioqui-1.1.7/src/aioqui/widgets/line_input.py
--rw-rw-rw-   0        0        0     4132 2023-05-14 04:47:48.000000 aioqui-1.1.7/src/aioqui/widgets/popup.py
--rw-rw-rw-   0        0        0     1891 2023-05-14 05:26:43.000000 aioqui-1.1.7/src/aioqui/widgets/scroll_area.py
--rw-rw-rw-   0        0        0     1235 2023-05-14 03:24:34.000000 aioqui-1.1.7/src/aioqui/widgets/selector.py
--rw-rw-rw-   0        0        0      921 2023-05-14 01:40:16.000000 aioqui-1.1.7/src/aioqui/widgets/slider.py
--rw-rw-rw-   0        0        0      384 2023-05-14 00:57:08.000000 aioqui-1.1.7/src/aioqui/widgets/spacer.py
--rw-rw-rw-   0        0        0     1800 2023-05-14 01:40:16.000000 aioqui-1.1.7/src/aioqui/widgets/splitter.py
--rw-rw-rw-   0        0        0     1283 2023-05-14 05:08:46.000000 aioqui-1.1.7/src/aioqui/widgets/stacked_widget.py
--rw-rw-rw-   0        0        0      374 2023-05-14 01:40:16.000000 aioqui-1.1.7/src/aioqui/widgets/statusbar.py
--rw-rw-rw-   0        0        0      694 2023-05-14 04:49:44.000000 aioqui-1.1.7/src/aioqui/widgets/text_input.py
--rw-rw-rw-   0        0        0      799 2023-05-14 05:08:45.000000 aioqui-1.1.7/src/aioqui/widgets/widget.py
--rw-rw-rw-   0        0        0      570 2023-05-14 05:08:34.000000 aioqui-1.1.7/src/aioqui/widgets/window.py
-drwxrwxrwx   0        0        0        0 2023-05-14 18:21:33.459689 aioqui-1.1.7/src/aioqui.egg-info/
--rw-rw-rw-   0        0        0     2641 2023-05-14 18:21:33.000000 aioqui-1.1.7/src/aioqui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    13070 2023-05-14 18:21:33.000000 aioqui-1.1.7/src/aioqui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 18:21:33.000000 aioqui-1.1.7/src/aioqui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-14 18:21:33.000000 aioqui-1.1.7/src/aioqui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-14 18:21:33.000000 aioqui-1.1.7/src/aioqui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.529507 aioqui-2.0.0/
+-rw-rw-rw-   0        0        0     1093 2023-02-26 16:41:50.000000 aioqui-2.0.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2629 2023-05-15 09:05:51.528507 aioqui-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      282 2023-05-15 08:21:18.000000 aioqui-2.0.0/README.md
+-rw-rw-rw-   0        0        0     1488 2023-05-15 09:05:20.000000 aioqui-2.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-15 09:05:51.529507 aioqui-2.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.219508 aioqui-2.0.0/src/
+-rw-rw-rw-   0        0        0        0 2023-03-20 19:19:08.000000 aioqui-2.0.0/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.221513 aioqui-2.0.0/src/aioqui/
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.214507 aioqui-2.0.0/src/aioqui/.assets/
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.484507 aioqui-2.0.0/src/aioqui/.assets/icons/
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/activity.svg
+-rw-rw-rw-   0        0        0      357 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/airplay.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-circle.svg
+-rw-rw-rw-   0        0        0      411 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-octagon.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/alert-triangle.svg
+-rw-rw-rw-   0        0        0      393 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-center.svg
+-rw-rw-rw-   0        0        0      394 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-justify.svg
+-rw-rw-rw-   0        0        0      391 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-left.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/align-right.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/anchor.svg
+-rw-rw-rw-   0        0        0      563 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/aperture.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/archive.svg
+-rw-rw-rw-   0        0        0      355 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-circle.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-left.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down-right.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-down.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-left-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-left.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-right-circle.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-right.svg
+-rw-rw-rw-   0        0        0      352 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-left.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up-right.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/arrow-up.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/at-sign.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/award.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bar-chart-2.svg
+-rw-rw-rw-   0        0        0      348 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bar-chart.svg
+-rw-rw-rw-   0        0        0      422 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/battery-charging.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/battery.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bell-off.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bell.svg
+-rw-rw-rw-   0        0        0      293 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bluetooth.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bold.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/book-open.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/book.svg
+-rw-rw-rw-   0        0        0      282 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/bookmark.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/box.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/briefcase.svg
+-rw-rw-rw-   0        0        0      405 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/calendar.svg
+-rw-rw-rw-   0        0        0      380 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/camera-off.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/camera.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cast.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check-circle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check-square.svg
+-rw-rw-rw-   0        0        0      257 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/check.svg
+-rw-rw-rw-   0        0        0      264 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-down.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-left.svg
+-rw-rw-rw-   0        0        0      265 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-right.svg
+-rw-rw-rw-   0        0        0      263 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevron-up.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-down.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-right.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chevrons-up.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/chrome.svg
+-rw-rw-rw-   0        0        0      253 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/circle.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/clipboard.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/clock.svg
+-rw-rw-rw-   0        0        0      552 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-drizzle.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-lightning.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-off.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-rain.svg
+-rw-rw-rw-   0        0        0      567 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud-snow.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cloud.svg
+-rw-rw-rw-   0        0        0      302 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/code.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/codepen.svg
+-rw-rw-rw-   0        0        0      633 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/codesandbox.svg
+-rw-rw-rw-   0        0        0      442 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/coffee.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/columns.svg
+-rw-rw-rw-   0        0        0      416 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/command.svg
+-rw-rw-rw-   0        0        0      337 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/compass.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/copy.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-down-left.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-down-right.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-left-down.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-left-up.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-right-down.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-right-up.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-up-left.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/corner-up-right.svg
+-rw-rw-rw-   0        0        0      662 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/cpu.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/credit-card.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/crop.svg
+-rw-rw-rw-   0        0        0      432 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/crosshair.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/database.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/delete.svg
+-rw-rw-rw-   0        0        0      290 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/disc.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide-circle.svg
+-rw-rw-rw-   0        0        0      414 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide-square.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/divide.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/dollar-sign.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/download-cloud.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/download.svg
+-rw-rw-rw-   0        0        0      419 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/dribbble.svg
+-rw-rw-rw-   0        0        0      269 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/droplet.svg
+-rw-rw-rw-   0        0        0      286 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit-2.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit-3.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/edit.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/external-link.svg
+-rw-rw-rw-   0        0        0      455 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/eye-off.svg
+-rw-rw-rw-   0        0        0      311 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/eye.svg
+-rw-rw-rw-   0        0        0      298 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/facebook.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/fast-forward.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/feather.svg
+-rw-rw-rw-   0        0        0      548 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/figma.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-minus.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-plus.svg
+-rw-rw-rw-   0        0        0      468 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file-text.svg
+-rw-rw-rw-   0        0        0      332 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/file.svg
+-rw-rw-rw-   0        0        0      581 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/film.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/filter.svg
+-rw-rw-rw-   0        0        0      329 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/flag.svg
+-rw-rw-rw-   0        0        0      356 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder-minus.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder-plus.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/folder.svg
+-rw-rw-rw-   0        0        0      273 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/framer.svg
+-rw-rw-rw-   0        0        0      385 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/frown.svg
+-rw-rw-rw-   0        0        0      476 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/gift.svg
+-rw-rw-rw-   0        0        0      372 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-branch.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-commit.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-merge.svg
+-rw-rw-rw-   0        0        0      382 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/git-pull-request.svg
+-rw-rw-rw-   0        0        0      522 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/github.svg
+-rw-rw-rw-   0        0        0      485 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/gitlab.svg
+-rw-rw-rw-   0        0        0      404 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/globe.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/grid.svg
+-rw-rw-rw-   0        0        0      479 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hard-drive.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hash.svg
+-rw-rw-rw-   0        0        0      390 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/headphones.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/heart.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/help-circle.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/hexagon.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/home.svg
+-rw-rw-rw-   0        0        0      364 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/image.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/inbox.svg
+-rw-rw-rw-   0        0        0      342 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/info.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/instagram.svg
+-rw-rw-rw-   0        0        0      343 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/italic.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/key.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/layers.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/layout.svg
+-rw-rw-rw-   0        0        0      570 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/life-buoy.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/link-2.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/link.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/linkedin.svg
+-rw-rw-rw-   0        0        0      477 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/list.svg
+-rw-rw-rw-   0        0        0      609 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/loader.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/lock.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/log-in.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/log-out.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mail.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/map-pin.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/map.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/maximize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/maximize.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/meh.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/menu.svg
+-rw-rw-rw-   0        0        0      423 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/message-circle.svg
+-rw-rw-rw-   0        0        0      300 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/message-square.svg
+-rw-rw-rw-   0        0        0      489 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mic-off.svg
+-rw-rw-rw-   0        0        0      413 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mic.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minimize-2.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minimize.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus-circle.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus-square.svg
+-rw-rw-rw-   0        0        0      256 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/minus.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/monitor.svg
+-rw-rw-rw-   0        0        0      276 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/moon.svg
+-rw-rw-rw-   0        0        0      338 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/more-horizontal.svg
+-rw-rw-rw-   0        0        0      336 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/more-vertical.svg
+-rw-rw-rw-   0        0        0      306 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/mouse-pointer.svg
+-rw-rw-rw-   0        0        0      481 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/move.svg
+-rw-rw-rw-   0        0        0      322 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/music.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/navigation-2.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/navigation.svg
+-rw-rw-rw-   0        0        0      313 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/octagon.svg
+-rw-rw-rw-   0        0        0      512 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/package.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/paperclip.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pause-circle.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pause.svg
+-rw-rw-rw-   0        0        0      386 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pen-tool.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/percent.svg
+-rw-rw-rw-   0        0        0      571 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-call.svg
+-rw-rw-rw-   0        0        0      613 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-forwarded.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-incoming.svg
+-rw-rw-rw-   0        0        0      608 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-missed.svg
+-rw-rw-rw-   0        0        0      586 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-off.svg
+-rw-rw-rw-   0        0        0      612 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone-outgoing.svg
+-rw-rw-rw-   0        0        0      515 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/phone.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pie-chart.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/play-circle.svg
+-rw-rw-rw-   0        0        0      258 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/play.svg
+-rw-rw-rw-   0        0        0      345 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-circle-gray.svg
+-rw-rw-rw-   0        0        0      346 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-circle.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus-square.svg
+-rw-rw-rw-   0        0        0      299 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/plus.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/pocket.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/power.svg
+-rw-rw-rw-   0        0        0      402 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/printer.svg
+-rw-rw-rw-   0        0        0      384 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/radio.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/refresh-ccw.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/refresh-cw.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/repeat.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rewind.svg
+-rw-rw-rw-   0        0        0      312 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rotate-ccw.svg
+-rw-rw-rw-   0        0        0      316 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rotate-cw.svg
+-rw-rw-rw-   0        0        0      325 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/rss.svg
+-rw-rw-rw-   0        0        0      387 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/save.svg
+-rw-rw-rw-   0        0        0      366 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/schedule.svg
+-rw-rw-rw-   0        0        0      439 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/scissors.svg
+-rw-rw-rw-   0        0        0      303 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/search.svg
+-rw-rw-rw-   0        0        0      309 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/send.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/server.svg
+-rw-rw-rw-   0        0        0     1006 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/settings.svg
+-rw-rw-rw-   0        0        0      440 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/share-2.svg
+-rw-rw-rw-   0        0        0      359 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/share.svg
+-rw-rw-rw-   0        0        0      400 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shield-off.svg
+-rw-rw-rw-   0        0        0      274 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shield.svg
+-rw-rw-rw-   0        0        0      367 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shopping-bag.svg
+-rw-rw-rw-   0        0        0      378 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shopping-cart.svg
+-rw-rw-rw-   0        0        0      436 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/shuffle.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sidebar.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/skip-back.svg
+-rw-rw-rw-   0        0        0      310 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/skip-forward.svg
+-rw-rw-rw-   0        0        0      994 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/slack.svg
+-rw-rw-rw-   0        0        0      307 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/slash.svg
+-rw-rw-rw-   0        0        0      606 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sliders.svg
+-rw-rw-rw-   0        0        0      327 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/smartphone.svg
+-rw-rw-rw-   0        0        0      383 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/smile.svg
+-rw-rw-rw-   0        0        0      361 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/speaker.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/square.svg
+-rw-rw-rw-   0        0        0      391 2023-04-06 21:10:35.000000 aioqui-2.0.0/src/aioqui/.assets/icons/star-fill.svg
+-rw-rw-rw-   0        0        0      334 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/star.svg
+-rw-rw-rw-   0        0        0      304 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/stop-circle.svg
+-rw-rw-rw-   0        0        0      645 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sun.svg
+-rw-rw-rw-   0        0        0      584 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sunrise.svg
+-rw-rw-rw-   0        0        0      583 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/sunset.svg
+-rw-rw-rw-   0        0        0      335 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/table.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tablet.svg
+-rw-rw-rw-   0        0        0      350 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tag.svg
+-rw-rw-rw-   0        0        0      331 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/target.svg
+-rw-rw-rw-   0        0        0      305 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/terminal.svg
+-rw-rw-rw-   0        0        0      292 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thermometer.svg
+-rw-rw-rw-   0        0        0      369 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thumbs-down.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/thumbs-up.svg
+-rw-rw-rw-   0        0        0      318 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/toggle-left.svg
+-rw-rw-rw-   0        0        0      320 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/toggle-right.svg
+-rw-rw-rw-   0        0        0      381 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tool.svg
+-rw-rw-rw-   0        0        0      443 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trash-2.svg
+-rw-rw-rw-   0        0        0      351 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trash.svg
+-rw-rw-rw-   0        0        0      368 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trello.svg
+-rw-rw-rw-   0        0        0      326 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trending-down.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/trending-up.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/triangle.svg
+-rw-rw-rw-   0        0        0      410 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/truck.svg
+-rw-rw-rw-   0        0        0      315 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/tv.svg
+-rw-rw-rw-   0        0        0      272 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/twitch.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/twitter.svg
+-rw-rw-rw-   0        0        0      347 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/type.svg
+-rw-rw-rw-   0        0        0      285 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/umbrella.svg
+-rw-rw-rw-   0        0        0      314 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/underline.svg
+-rw-rw-rw-   0        0        0      317 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/unlock.svg
+-rw-rw-rw-   0        0        0      426 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/upload-cloud.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/upload.svg
+-rw-rw-rw-   0        0        0      362 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-check.svg
+-rw-rw-rw-   0        0        0      360 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-minus.svg
+-rw-rw-rw-   0        0        0      403 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-plus.svg
+-rw-rw-rw-   0        0        0      399 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user-x.svg
+-rw-rw-rw-   0        0        0      308 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/user.svg
+-rw-rw-rw-   0        0        0      395 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/users.svg
+-rw-rw-rw-   0        0        0      374 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/video-off.svg
+-rw-rw-rw-   0        0        0      324 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/video.svg
+-rw-rw-rw-   0        0        0      353 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/voicemail.svg
+-rw-rw-rw-   0        0        0      323 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-1.svg
+-rw-rw-rw-   0        0        0      354 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-2.svg
+-rw-rw-rw-   0        0        0      365 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume-x.svg
+-rw-rw-rw-   0        0        0      275 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/volume.svg
+-rw-rw-rw-   0        0        0      457 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/watch.svg
+-rw-rw-rw-   0        0        0      564 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wifi-off.svg
+-rw-rw-rw-   0        0        0      396 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wifi.svg
+-rw-rw-rw-   0        0        0      321 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/wind.svg
+-rw-rw-rw-   0        0        0      340 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-circle-gray.svg
+-rw-rw-rw-   0        0        0      341 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-circle.svg
+-rw-rw-rw-   0        0        0      401 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-octagon.svg
+-rw-rw-rw-   0        0        0      363 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x-square.svg
+-rw-rw-rw-   0        0        0      294 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/x.svg
+-rw-rw-rw-   0        0        0      560 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/youtube.svg
+-rw-rw-rw-   0        0        0      428 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zap-off.svg
+-rw-rw-rw-   0        0        0      277 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zap.svg
+-rw-rw-rw-   0        0        0      392 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zoom-in.svg
+-rw-rw-rw-   0        0        0      349 2023-03-18 18:50:21.000000 aioqui-2.0.0/src/aioqui/.assets/icons/zoom-out.svg
+-rw-rw-rw-   0        0        0      158 2023-05-15 07:06:29.000000 aioqui-2.0.0/src/aioqui/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.487507 aioqui-2.0.0/src/aioqui/context/
+-rw-rw-rw-   0        0        0       70 2023-05-15 07:06:13.000000 aioqui-2.0.0/src/aioqui/context/__init__.py
+-rw-rw-rw-   0        0        0     8784 2023-05-15 08:45:31.000000 aioqui-2.0.0/src/aioqui/context/context_obj.py
+-rw-rw-rw-   0        0        0      443 2023-05-14 00:18:53.000000 aioqui-2.0.0/src/aioqui/context/contextapi.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.493507 aioqui-2.0.0/src/aioqui/enums/
+-rw-rw-rw-   0        0        0      255 2023-05-15 05:17:48.000000 aioqui-2.0.0/src/aioqui/enums/__init__.py
+-rw-rw-rw-   0        0        0      687 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/alignment.py
+-rw-rw-rw-   0        0        0      182 2023-05-15 05:17:48.000000 aioqui-2.0.0/src/aioqui/enums/echo_mode.py
+-rw-rw-rw-   0        0        0      227 2023-05-14 07:18:50.000000 aioqui-2.0.0/src/aioqui/enums/elide_mode.py
+-rw-rw-rw-   0        0        0      151 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/orientation.py
+-rw-rw-rw-   0        0        0      264 2023-05-14 00:48:52.000000 aioqui-2.0.0/src/aioqui/enums/scroll_policy.py
+-rw-rw-rw-   0        0        0      235 2023-05-15 05:48:40.000000 aioqui-2.0.0/src/aioqui/enums/size_policy.py
+-rw-rw-rw-   0        0        0      105 2023-05-13 23:00:29.000000 aioqui-2.0.0/src/aioqui/enums/window_hint.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.500507 aioqui-2.0.0/src/aioqui/misc/
+-rw-rw-rw-   0        0        0      128 2023-05-15 08:51:32.000000 aioqui-2.0.0/src/aioqui/misc/__init__.py
+-rw-rw-rw-   0        0        0     3736 2023-05-15 04:39:08.000000 aioqui-2.0.0/src/aioqui/misc/aiorequest.py
+-rw-rw-rw-   0        0        0     1014 2023-05-15 09:02:15.000000 aioqui-2.0.0/src/aioqui/misc/animation.py
+-rw-rw-rw-   0        0        0     1130 2023-05-15 08:41:25.000000 aioqui-2.0.0/src/aioqui/misc/conthrq.py
+-rw-rw-rw-   0        0        0     1386 2023-05-14 18:16:30.000000 aioqui-2.0.0/src/aioqui/misc/fileops.py
+-rw-rw-rw-   0        0        0     2181 2023-05-14 00:12:50.000000 aioqui-2.0.0/src/aioqui/misc/qss_parser.py
+-rw-rw-rw-   0        0        0      319 2023-05-15 08:04:15.000000 aioqui-2.0.0/src/aioqui/misc/utils.py
+-rw-rw-rw-   0        0        0      701 2023-05-14 00:40:28.000000 aioqui-2.0.0/src/aioqui/misc/uvithread.py
+-rw-rw-rw-   0        0        0     1151 2023-05-15 05:37:56.000000 aioqui-2.0.0/src/aioqui/qasyncio.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.503507 aioqui-2.0.0/src/aioqui/types/
+-rw-rw-rw-   0        0        0       71 2023-05-14 03:02:21.000000 aioqui-2.0.0/src/aioqui/types/__init__.py
+-rw-rw-rw-   0        0        0      192 2023-05-15 07:18:29.000000 aioqui-2.0.0/src/aioqui/types/common.py
+-rw-rw-rw-   0        0        0     3539 2023-05-14 00:07:05.000000 aioqui-2.0.0/src/aioqui/types/icon.py
+-rw-rw-rw-   0        0        0      274 2023-04-20 15:54:13.000000 aioqui-2.0.0/src/aioqui/types/size.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.516509 aioqui-2.0.0/src/aioqui/widgets/
+-rw-rw-rw-   0        0        0      616 2023-05-15 07:39:02.000000 aioqui-2.0.0/src/aioqui/widgets/__init__.py
+-rw-rw-rw-   0        0        0      524 2023-05-15 08:10:27.000000 aioqui-2.0.0/src/aioqui/widgets/button.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.523514 aioqui-2.0.0/src/aioqui/widgets/custom/
+-rw-rw-rw-   0        0        0      259 2023-05-15 07:57:18.000000 aioqui-2.0.0/src/aioqui/widgets/custom/__init__.py
+-rw-rw-rw-   0        0        0     5695 2023-05-15 08:00:01.000000 aioqui-2.0.0/src/aioqui/widgets/custom/date_picker.py
+-rw-rw-rw-   0        0        0     1939 2023-05-15 09:01:44.000000 aioqui-2.0.0/src/aioqui/widgets/custom/error_label.py
+-rw-rw-rw-   0        0        0     2648 2023-05-15 07:57:46.000000 aioqui-2.0.0/src/aioqui/widgets/custom/image_button.py
+-rw-rw-rw-   0        0        0     1423 2023-05-15 07:46:33.000000 aioqui-2.0.0/src/aioqui/widgets/custom/menu_button.py
+-rw-rw-rw-   0        0        0     3961 2023-05-15 07:38:01.000000 aioqui-2.0.0/src/aioqui/widgets/custom/popup.py
+-rw-rw-rw-   0        0        0     1027 2023-05-15 07:42:41.000000 aioqui-2.0.0/src/aioqui/widgets/custom/searchbar.py
+-rw-rw-rw-   0        0        0     1877 2023-05-15 07:56:53.000000 aioqui-2.0.0/src/aioqui/widgets/custom/state_icon_btn.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.527508 aioqui-2.0.0/src/aioqui/widgets/extensions/
+-rw-rw-rw-   0        0        0      160 2023-05-15 06:44:59.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-05-15 06:52:42.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/input_ext.py
+-rw-rw-rw-   0        0        0     1944 2023-05-15 06:42:58.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/layout_ext.py
+-rw-rw-rw-   0        0        0      710 2023-05-15 06:28:17.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/side_menu_ext.py
+-rw-rw-rw-   0        0        0     1925 2023-05-15 05:30:53.000000 aioqui-2.0.0/src/aioqui/widgets/extensions/splitter_widget_ext.py
+-rw-rw-rw-   0        0        0      667 2023-05-15 07:22:27.000000 aioqui-2.0.0/src/aioqui/widgets/frame.py
+-rw-rw-rw-   0        0        0     2369 2023-05-15 07:40:44.000000 aioqui-2.0.0/src/aioqui/widgets/input.py
+-rw-rw-rw-   0        0        0     1367 2023-05-15 07:43:50.000000 aioqui-2.0.0/src/aioqui/widgets/label.py
+-rw-rw-rw-   0        0        0     1348 2023-05-15 07:41:20.000000 aioqui-2.0.0/src/aioqui/widgets/layout.py
+-rw-rw-rw-   0        0        0     1736 2023-05-15 07:22:47.000000 aioqui-2.0.0/src/aioqui/widgets/scroll_area.py
+-rw-rw-rw-   0        0        0     1184 2023-05-15 07:23:03.000000 aioqui-2.0.0/src/aioqui/widgets/selector.py
+-rw-rw-rw-   0        0        0      862 2023-05-15 07:33:52.000000 aioqui-2.0.0/src/aioqui/widgets/slider.py
+-rw-rw-rw-   0        0        0      270 2023-05-15 05:49:01.000000 aioqui-2.0.0/src/aioqui/widgets/spacer.py
+-rw-rw-rw-   0        0        0     1580 2023-05-15 07:23:37.000000 aioqui-2.0.0/src/aioqui/widgets/splitter.py
+-rw-rw-rw-   0        0        0     1159 2023-05-15 07:23:57.000000 aioqui-2.0.0/src/aioqui/widgets/stacked_widget.py
+-rw-rw-rw-   0        0        0      327 2023-05-15 07:24:09.000000 aioqui-2.0.0/src/aioqui/widgets/statusbar.py
+-rw-rw-rw-   0        0        0      587 2023-05-15 07:24:24.000000 aioqui-2.0.0/src/aioqui/widgets/widget.py
+-rw-rw-rw-   0        0        0      516 2023-05-15 07:29:59.000000 aioqui-2.0.0/src/aioqui/widgets/window.py
+drwxrwxrwx   0        0        0        0 2023-05-15 09:05:51.227507 aioqui-2.0.0/src/aioqui.egg-info/
+-rw-rw-rw-   0        0        0     2629 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    13091 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 09:05:51.000000 aioqui-2.0.0/src/aioqui.egg-info/top_level.txt
```

### Comparing `aioqui-1.1.7/LICENSE.txt` & `aioqui-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/PKG-INFO` & `aioqui-2.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 1.1.7
+Version: 2.0.0
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -26,26 +26,31 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/cxllmerichie/aioqui
 Project-URL: Bug Tracker, https://github.com/cxllmerichie/aioqui/issues
 Project-URL: Repository, https://github.com/cxllmerichie/aioqui
 Project-URL: Documentation, https://github.com/cxllmerichie/aioqui/README.md
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# ToDo:
-- favourite_button is actually a StateButton ? IconButton
-- error_label is actually a PopupTextLabel ? DelayLabel
-- make all widgets to have:
-    - margins (in abstract frame)
-    - padding (in abstract frame)
-    - alignment (in abstract frame)
-- make popup to be generic (configure different buttons (ok, cancel, no, yes)
-- crete generic animation class to create simple animations
+## Overview
+## Documentation
+## Installation
+```
+pip install aioqui
+```
+### Package dependencies
+includes ```pip install pyside6 qasync loguru```
+
+speedups ```pip install aiodns ujson cchardet uvloop```
+
+depending on modules [optional] ```pip install aiohttp uvicorn```
```

### Comparing `aioqui-1.1.7/pyproject.toml` & `aioqui-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,35 @@
 [build-system]
 requires = ["setuptools>=63.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aioqui"
-version = "1.1.7"
+version = "2.0.0"
 authors = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 maintainers = [
     { name="cxllmerichie", email="cxllmerichie@gmail.com" },
 ]
 description = "Asynchronous GUI framework based on PySide6"
 readme = "README.md"
 license = { file="LICENSE.txt" }
 requires-python = ">=3.10"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
-#    "Topic :: Security :: Cryptography",
-#    "Topic :: Database :: Front-Ends",
-#
+    "Topic :: Software Development :: User Interfaces",
+
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: 3.10",
 
     "Natural Language :: English",
-#
-#    "Development Status :: 4 - Beta",
-#
-#    "Framework :: FastAPI",
-#
+
+    "Development Status :: 3 - Alpha",
+
     "Intended Audience :: Developers",
 
     "Operating System :: OS Independent",
 
     "License :: OSI Approved :: MIT License"
 ]
 dependencies=[
```

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/aperture.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/aperture.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/cloud-drizzle.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/cloud-drizzle.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/cloud-snow.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/cloud-snow.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/codesandbox.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/codesandbox.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/cpu.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/cpu.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/figma.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/figma.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/film.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/film.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/github.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/life-buoy.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/life-buoy.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/loader.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/loader.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/package.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/package.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-call.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-call.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-forwarded.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-forwarded.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-incoming.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-incoming.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-missed.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-missed.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-off.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone-outgoing.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone-outgoing.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/phone.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/phone.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/settings.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/settings.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/slack.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/slack.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/sliders.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/sliders.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/sun.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/sun.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/sunrise.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/sunrise.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/sunset.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/sunset.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/wifi-off.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/wifi-off.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/.assets/icons/youtube.svg` & `aioqui-2.0.0/src/aioqui/.assets/icons/youtube.svg`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/enums/alignment.py` & `aioqui-2.0.0/src/aioqui/enums/alignment.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/misc/ctq.py` & `aioqui-2.0.0/src/aioqui/misc/conthrq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 from uuid import uuid4, UUID
 from threading import Thread
 
 
-class ConditionalThread(Thread):
-    to_complete: bool = True
-
-    def kill(self):
-        self.to_complete = False
+class ConditionalThreadQueue:
+    class ConditionalThread(Thread):
+        to_complete: bool = True
 
+        def kill(self) -> None:
+            self.to_complete = False
 
-class ConditionalThreadQueue:
     def __init__(self):
-        self.__threads: dict[UUID, ConditionalThread] = {}
+        self.__threads: dict[UUID, ConditionalThreadQueue.ConditionalThread] = {}
 
     def new(self, pre: callable, post: callable) -> UUID:
         if self.__threads:  # kill prev thread if exists
             key = list(self.__threads.keys())[-1]
             self.__threads[key].kill()
 
         def target(thread_uuid: UUID):  # create target for the new thread
             pre()
             thread = self.__threads[thread_uuid]
             if thread.to_complete:  # call post() if thread was not killed
                 post()
             self.__threads.pop(thread_uuid)
 
         uuid = uuid4()
-        thread = ConditionalThread(target=target, args=(uuid, ))
+        thread = ConditionalThreadQueue.ConditionalThread(target=target, args=(uuid, ))
         self.__threads[uuid] = thread
         thread.start()
         return uuid
 
     def __getitem__(self, uuid: UUID):
         return self.__threads[uuid]
```

### Comparing `aioqui-1.1.7/src/aioqui/misc/dialogs.py` & `aioqui-2.0.0/src/aioqui/misc/fileops.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/misc/parser.py` & `aioqui-2.0.0/src/aioqui/misc/qss_parser.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/misc/server.py` & `aioqui-2.0.0/src/aioqui/misc/uvithread.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/qasyncio.py` & `aioqui-2.0.0/src/aioqui/qasyncio.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
         try:
             qasync.run(wrap())
         except asyncio.exceptions.CancelledError:
             sys.exit(0)
 
 
-def to_async_slot(to_call):
-    @asyncSlot()
-    async def wrapped():
-        print(type(to_call))
-        if to_call.__class__.__name__ in ('function', 'method'):
-            await to_call()
-        # elif
-    return wrapped
+# def to_async_slot(to_call):
+#     @asyncSlot()
+#     async def wrapped():
+#         print(type(to_call))
+#         if to_call.__class__.__name__ in ('function', 'method'):
+#             await to_call()
+#         # elif
+#     return wrapped
```

### Comparing `aioqui-1.1.7/src/aioqui/types/icon.py` & `aioqui-2.0.0/src/aioqui/types/icon.py`

 * *Files identical despite different names*

### Comparing `aioqui-1.1.7/src/aioqui/widgets/custom/date_picker.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/date_picker.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,21 @@
 from ..frame import Frame
 from ..layout import Layout
 from ..selector import Selector
 from ..label import Label
 
 
 class DateTimePicker(Frame):
+    DaySelector: Selector
+    MonthSelector: Selector
+    YearSelector: Selector
+    HourSelector: Selector
+    MinuteSelector: Selector
+    SecondSelector: Selector
+
     now = datetime.now()
     default_format = '%d.%m.%Y %H:%M'
 
     days = [str(day).zfill(2) for day in range(1, monthrange(now.year, now.month)[1] + 1)]
     months = [str(month).zfill(2) for month in range(1, 12 + 1)]
     years = [str(year) for year in range(now.year, now.year + 10)]
 
@@ -34,95 +41,95 @@
             items=[
                 await Frame(self, f'{self.objectName()}DateFrame').init(
                     layout=await Layout.horizontal().init(
                         items=[
                             await Label(self, f'{self.objectName()}DateLbl').init(
                                 text='Date:'
                             ),
-                            day_selector := await Selector(self, f'{self.objectName()}DaySelector').init(
+                            DaySelector := await Selector(self, f'{self.objectName()}DaySelector').init(
                                 items=self.days
                             ),
-                            month_selector := await Selector(self, f'{self.objectName()}MonthSelector').init(
+                            MonthSelector := await Selector(self, f'{self.objectName()}MonthSelector').init(
                                 items=self.months
                             ),
-                            year_selector := await Selector(self, f'{self.objectName()}YearSelector').init(
+                            YearSelector := await Selector(self, f'{self.objectName()}YearSelector').init(
                                 items=self.years
                             )
                         ]
                     )
                 ),
                 await Frame(self, f'{self.objectName()}TimeFrame').init(
                     layout=await Layout.horizontal().init(
                         items=[
                             await Label(self, f'{self.objectName()}TimeLbl').init(
                                 text='Time:'
                             ),
-                            hour_selector := await Selector(self, f'{self.objectName()}HourSelector').init(
+                            HourSelector := await Selector(self, f'{self.objectName()}HourSelector').init(
                                 items=self.hours
                             ),
-                            minute_selector := await Selector(self, f'{self.objectName()}MinuteSelector').init(
+                            MinuteSelector := await Selector(self, f'{self.objectName()}MinuteSelector').init(
                                 items=self.minutes
                             ),
-                            second_selector := await Selector(self, f'{self.objectName()}SecondSelector').init(
+                            SecondSelector := await Selector(self, f'{self.objectName()}SecondSelector').init(
                                 items=self.seconds
                             )
                         ]
                     )
                 )
             ]
         ))
-        self.day_selector = day_selector
-        self.month_selector = month_selector
-        self.year_selector = year_selector
-        self.hour_selector = hour_selector
-        self.minute_selector = minute_selector
-        self.second_selector = second_selector
+        self.DaySelector = DaySelector
+        self.MonthSelector = MonthSelector
+        self.YearSelector = YearSelector
+        self.HourSelector = HourSelector
+        self.MinuteSelector = MinuteSelector
+        self.SecondSelector = SecondSelector
         return self
 
     def get_datetime(self, tz: bool) -> datetime:
-        dt = datetime(day=int(self.day_selector.currentText()),
-                      month=int(self.month_selector.currentText()),
-                      year=int(self.year_selector.currentText()),
-                      hour=int(self.hour_selector.currentText()),
-                      minute=int(self.minute_selector.currentText()),
-                      second=int(self.second_selector.currentText()),
+        dt = datetime(day=int(self.DaySelector.currentText()),
+                      month=int(self.MonthSelector.currentText()),
+                      year=int(self.YearSelector.currentText()),
+                      hour=int(self.HourSelector.currentText()),
+                      minute=int(self.MinuteSelector.currentText()),
+                      second=int(self.SecondSelector.currentText()),
         )
         if tz:
             dt.replace(tzinfo=timezone.utc)
         else:
             dt.replace(tzinfo=None)
         return dt
 
     def get_date(self) -> date:
         return date(
-            day=int(self.day_selector.currentText()),
-            month=int(self.month_selector.currentText()),
-            year=int(self.year_selector.currentText())
+            day=int(self.DaySelector.currentText()),
+            month=int(self.MonthSelector.currentText()),
+            year=int(self.YearSelector.currentText())
         )
 
     def get_time(self) -> time:
         return time(
-            hour=int(self.hour_selector.currentText()),
-            minute=int(self.minute_selector.currentText()),
-            second=int(self.second_selector.currentText())
+            hour=int(self.HourSelector.currentText()),
+            minute=int(self.MinuteSelector.currentText()),
+            second=int(self.SecondSelector.currentText())
         )
 
     def set_date(self, dt: date | datetime | str):
         if isinstance(dt, str):
             dt = self.parse(dt)
-        self.day_selector.setCurrentText(str(dt.day).zfill(2))
-        self.month_selector.setCurrentText(str(dt.month).zfill(2))
-        self.year_selector.setCurrentText(str(dt.year).zfill(2))
+        self.DaySelector.setCurrentText(str(dt.day).zfill(2))
+        self.MonthSelector.setCurrentText(str(dt.month).zfill(2))
+        self.YearSelector.setCurrentText(str(dt.year).zfill(2))
 
     def set_time(self, dt: time | datetime):
         if isinstance(dt, str):
             dt = self.parse(dt)
-        self.hour_selector.setCurrentText(str(dt.hour).zfill(2))
-        self.minute_selector.setCurrentText(str(dt.minute).zfill(2))
-        self.second_selector.setCurrentText(str(dt.second).zfill(2))
+        self.HourSelector.setCurrentText(str(dt.hour).zfill(2))
+        self.MinuteSelector.setCurrentText(str(dt.minute).zfill(2))
+        self.SecondSelector.setCurrentText(str(dt.second).zfill(2))
 
     def set_datetime(self, dt: datetime):
         self.set_date(dt)
         self.set_time(dt)
 
     @staticmethod
     def parse(timestr: str) -> datetime:
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/custom/error_label.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/error_label.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,23 +4,26 @@
 
 from ...misc import ConditionalThreadQueue
 from ..label import Label
 from ...qasyncio import asyncSlot
 
 
 class ErrorLabel(Label):
+    __duration: float = 0.5
+    __ctq: ConditionalThreadQueue = ConditionalThreadQueue()
+
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
-        self.__ctq = ConditionalThreadQueue()
-        self.__opacity: float = 1
-        self.__duration: float = 0.5
-
-    async def init(self, *args, **kwargs) -> 'ErrorLabel':
-        await super().init(*args, **kwargs)
-        return self
+
+    async def init(
+            self, *,
+            _=None,
+            **kwargs
+    ) -> 'ErrorLabel':
+        return await Label.init(self, **kwargs)
 
     def setText(self, text: str, delay: float = 2, duration: int = 0.5) -> None:
         if delay == 0:  # if delay is 0, just set the text
             return Label.setText(self, '')
 
         if not text:  # text == '' means instantly clear the text and hide label without `post` action
             self.setVisible(False)
@@ -49,8 +52,9 @@
     def _get_opacity(self):
         return self.__opacity
 
     def _set_opacity(self, opacity):
         self.__opacity = opacity
         self.setStyleSheet(f'color: rgba(255, 0, 0, {opacity});')
 
-    _opacity = Property(float, _get_opacity, _set_opacity)
+    __opacity: float = 1
+    _opacity: Property = Property(float, _get_opacity, _set_opacity)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/custom/image_button.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/image_button.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 from PySide6.QtWidgets import QWidget, QFileDialog
 from PySide6.QtGui import QIcon
 from contextlib import suppress
 
 from ..button import Button
-from ..popup import Popup
+from src.aioqui.widgets.custom.popup import Popup
 from ...types import Icon, Size
 from ...qasyncio import asyncSlot
 
 
 class ImageButton(Button):
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
         self.image_bytes = None
 
     async def init(
             self, *,
             icon: Icon, slot: callable = lambda: None, directory: str = ''
     ) -> 'ImageButton':
-        await super().init(icon=icon, events=Button.Events(on_click=lambda: self.choose_image(slot, directory)))
+        await super().init(icon=icon, on_click=lambda: self.choose_image(slot, directory))
         self.RemoveImageBtn = await Button(self, f'{self.objectName()}RemoveImageBtn').init(
-            icon=Icon('x-circle.svg', (30, 30)), sizes=Button.Sizes(fixed_size=Size(30, 30)),
-            events=Button.Events(
-                on_click=lambda: Popup(self.core).display(message=f'Remove icon?', on_success=self.remove_icon)
-            )
+            icon=Icon('x-circle.svg', (30, 30)), fixed_size=Size(30, 30),
+            on_click=lambda: Popup(self.core).display(message=f'Remove icon?', on_success=self.remove_icon)
         )
         self.RemoveImageBtn.move(self.width() - 30, 0)
         self.RemoveImageBtn.setStyleSheet(f'''
             #{self.objectName()}RemoveImageBtn {{background-color: transparent; border-radius: 14px;}}
             #{self.objectName()}RemoveImageBtn:hover {{background-color: rgba(255, 255, 255, 0.3);}}
         ''')
         return self
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/custom/menu_button.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/menu_button.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,34 +3,37 @@
 from ..button import Button
 from ..label import Label
 from ..layout import Layout
 from ...types import Icon, Size
 
 
 class MenuButton(Button):
+    IconBtn: Button
+    TextLbl: Label
+    TotalLbl: Label
+
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         super().__init__(parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
-            icon: Icon, text: str, total: int = 0, slot: callable = None
+            icon: Icon, text: str, total: int = 0,
+            **kwargs
     ) -> 'MenuButton':
         self.setLayout(await Layout.horizontal().init(
             margins=(10, 5, 10, 5), spacing=10,
             items=[
-                icon_btn := await Button(self, f'{self.objectName()}IconBtn').init(
-                    icon=icon, disabled=True, sizes=Button.Sizes(fixed_size=Size(icon.size.width(), icon.size.height()))
+                IconBtn := await Button(self, f'{self.objectName()}IconBtn').init(
+                    icon=icon, disabled=True, fixed_size=Size(icon.size.width(), icon.size.height())
                 ), Layout.Left,
-                text_lbl := await Label(self, f'{self.objectName()}TextLbl').init(
-                    text=text, sizes=Label.Sizes(hpolicy=Label.Expanding), elide=Label.ElideRight
+                TextLbl := await Label(self, f'{self.objectName()}TextLbl').init(
+                    text=text, hpolicy=Label.Expanding, elide=Label.ElideRight
                 ),
-                total_lbl := await Label(self, f'{self.objectName()}TotalLbl').init(
+                TotalLbl := await Label(self, f'{self.objectName()}TotalLbl').init(
                     text=str(total)
                 ), Layout.Right
             ]
         ))
-        self.icon_btn = icon_btn
-        self.text_lbl = text_lbl
-        self.total_lbl = total_lbl
-        if slot:
-            self.clicked.connect(slot)
-        return self
+        self.IconBtn = IconBtn
+        self.TextLbl = TextLbl
+        self.TotalLbl = TotalLbl
+        return await Button.init(self, **kwargs)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/custom/search_bar.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/searchbar.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 from PySide6.QtWidgets import QWidget, QCompleter, QStyledItemDelegate
 from PySide6.QtCore import Qt
 from typing import Sequence
 
-from ..line_input import LineInput
-from ...types import Applicable
-from ...objects import SizedObj, EventedObj
+from ..input import LineInput
 
 
 class SearchBar(LineInput):
     class Completer(QCompleter):
         def __init__(self, parent: QWidget, *, items: Sequence[str], stylesheet: str = ''):
             super().__init__(items, parent)
             self.setCaseSensitivity(Qt.CaseInsensitive)
@@ -17,13 +15,13 @@
             self.popup().setStyleSheet(stylesheet)
 
     def __init__(self, parent: QWidget, name: str = None, visible: bool = True):
         LineInput.__init__(self, parent, name if name else self.__class__.__name__, visible)
 
     async def init(
             self, *,
-            placeholder: str, completer: Completer, hidden: bool = False,
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            completer: Completer,
+            **kwargs
     ) -> 'LineInput':
-        await super().init(placeholder=placeholder, hidden=hidden, events=events, sizes=sizes)
+        await LineInput.init(self, **kwargs)
         self.setCompleter(completer)
         return self
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/extensions/layout_ext.py` & `aioqui-2.0.0/src/aioqui/widgets/extensions/layout_ext.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from PySide6.QtWidgets import QWidget, QLayoutItem, QSpacerItem
 from PySide6.QtCore import Qt, QObject
 from typing import Sequence, Iterable
 
+from ...enums import Alignment
 
-class LayoutExt:
+
+class LayoutExt(Alignment):
     async def init(
             self, *,
             margins: tuple[int, ...] = (0, 0, 0, 0), spacing: int = 0, alignment: Qt.Alignment = None,
             items: Sequence[QObject] = ()
     ) -> 'LayoutExt':
         self.setContentsMargins(*margins)
         self.setSpacing(spacing)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/extensions/splitter_widget_ext.py` & `aioqui-2.0.0/src/aioqui/widgets/extensions/splitter_widget_ext.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from PySide6.QtWidgets import QSplitter
-from loguru import logger as _logger
 
-from ...enums import Orientation, SizePolicy
+from ...enums import Orientation
 
 
 class SplitterWidgetExt(Orientation):
     splitter: QSplitter
+    __orientation: Orientation.Orientation
 
-    def __init__(self, expand_to: int,
-                 expand_min: int = None, expand_max: int = None, orientation: Orientation.Orientation = None,
-                 policy: tuple[SizePolicy.SizePolicy, SizePolicy.SizePolicy] = (SizePolicy.Expanding, SizePolicy.Expanding)):
+    def __init__(self, expand_to: int, expand_min: int = None, expand_max: int = None, collapsible: bool = True):
         self.expand_to: int = expand_to
-        self.setSizePolicy(*policy)
-
-        if expand_min or expand_max:
-            if orientation:
-                dimension = 'width' if orientation is Orientation.Horizontal else 'height'
-                if expand_min:
-                    getattr(self, f'setMinimum{dimension.capitalize()}')(expand_min)
-                if expand_max:
-                    getattr(self, f'setMaximum{dimension.capitalize()}')(expand_max)
-            else:
-                _logger.info('`expand_min` and `expand_max` set but `orientation` is `None`')
+        self.expand_min: int = expand_min
+        self.expand_max: int = expand_max
+        self.collapsible: bool = collapsible
+
+    @property
+    def orientation(self) -> Orientation.Orientation:
+        return self.Orientation
+
+    @orientation.setter
+    def orientation(self, orientation: Orientation.Orientation) -> None:
+        dimension = 'width' if orientation is Orientation.Horizontal else 'height'
+        if self.expand_min:
+            getattr(self, f'setMinimum{dimension.capitalize()}')(self.expand_min)
+        if self.expand_max:
+            getattr(self, f'setMaximum{dimension.capitalize()}')(self.expand_max)
+        self.__orientation = orientation
 
     def _index(self) -> int:
         for index in range(self.splitter.count()):
             if self == self.splitter.widget(index):
                 return index
         raise IndexError(f'{self} not found in {self.splitter} widgets')
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/frame.py` & `aioqui-2.0.0/src/aioqui/widgets/frame.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from PySide6.QtWidgets import QFrame, QWidget, QLayout
+from PySide6.QtWidgets import QFrame, QLayout
 
-from ..objects import ContextObj, SizedObj, EventedObj
-from ..types import Applicable
+from ..types import QSS, Parent
+from ..context import ContextObj
 
 
 class Frame(ContextObj, QFrame):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
         QFrame.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        self.setStyleSheet(stylesheet)
+        self.qss = qss
 
     async def init(
             self, *,
             style: ... = None, layout: QLayout = None,
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            **kwargs,
     ) -> 'Frame':
         if style:
             self.setFrameStyle(style)
         if layout:
             self.setLayout(layout)
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/label.py` & `aioqui-2.0.0/src/aioqui/widgets/label.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 from PySide6.QtGui import QFontMetrics, QPaintEvent
-from PySide6.QtWidgets import QLabel, QWidget
+from PySide6.QtWidgets import QLabel
 
-from ..objects import ContextObj, SizedObj, EventedObj
-from ..enums import Alignment, ElideMode
-from ..types import Applicable, Icon
+from ..enums import Alignment, ElideMode, SizePolicy
+from ..types import Parent, QSS
+from ..context import ContextObj
 
 
-class Label(ContextObj, Alignment, ElideMode, QLabel):
+class Label(ContextObj, Alignment, SizePolicy, ElideMode, QLabel):
     __elide_mode: ElideMode.ElideMode
     __elide_text: str
 
-    def __init__(self, parent: QWidget, name: str, visible: bool = True):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
         QLabel.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
+        self.qss = qss
 
     async def init(
             self, *,
-            text: str = '', wrap: bool = False, icon: Icon = None, elide: ElideMode.ElideMode = None,
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            wrap: bool = False, elide: ElideMode.ElideMode = None,
+            **kwargs
     ) -> 'Label':
-        self.__elide_mode, self.__elide_text = elide, text
-        self.setText(text)
+        self.__elide_mode = elide
         self.setWordWrap(wrap)
-        if icon:
-            self.setPixmap(icon.icon.pixmap(icon.size))
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
 
     def paintEvent(self, event: QPaintEvent):
         if self.elided():
-            elided_text = self.__elide_text
+            elided_text = self.text()
             self.setText(QFontMetrics(self.font()).elidedText(elided_text, self.__elide_mode, self.width() - 10))
             self.__elide_text = elided_text
-        super().paintEvent(event)
+        QLabel.paintEvent(self, event)
 
     def elided(self) -> bool:
         return self.__elide_mode is not None
 
     def setText(self, text: str) -> None:
         if self.elided():
             self.__elide_text = text
-        super().setText(text)
+        QLabel.setText(self, text)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/layout.py` & `aioqui-2.0.0/src/aioqui/widgets/slider.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-from PySide6.QtWidgets import QVBoxLayout, QWidget, QHBoxLayout
+from PySide6.QtWidgets import QSlider
 from PySide6.QtCore import Qt
-from typing import Union
-from abc import ABC
 
-from .extensions import LayoutExt
-from ..objects import ContextObj
-from ..enums import Alignment, SizePolicy, Orientation
-
-
-class Layout(ABC, Alignment, SizePolicy, Orientation):
-    @classmethod
-    def horizontal(cls, parent: QWidget = None, name: str = None) -> 'HLayout':
-        return HLayout(parent, name)
-
-    @classmethod
-    def vertical(cls, parent: QWidget = None, name: str = None) -> 'VLayout':
-        return VLayout(parent, name)
-
-    @classmethod
-    def oriented(cls, orientation: Qt.Orientation, parent: QWidget = None, name: str = None) -> Union['VLayout', 'HLayout']:
-        return Layout.vertical(parent, name) if orientation is Layout.Vertical else Layout.horizontal(parent, name)
-
-
-class VLayout(ContextObj, LayoutExt, QVBoxLayout):
-    def __init__(self, parent: QWidget = None, name: str = None):
-        QVBoxLayout.__init__(self, parent)
-        ContextObj.__init__(self, parent, name, True)
-
-
-class HLayout(ContextObj, LayoutExt, QHBoxLayout):
-    def __init__(self, parent: QWidget = None, name: str = None):
-        QHBoxLayout.__init__(self, parent)
-        ContextObj.__init__(self, parent, name, True)
+from ..context import ContextObj
+from ..enums import Orientation
+from ..types import Parent
+
+
+class Slider(ContextObj, Orientation, QSlider):
+    def __init__(self, parent: Parent, name: str, visible: bool = True,
+                 orientation: Orientation.Orientation = Orientation.Horizontal):
+        QSlider.__init__(self, orientation, parent)
+        ContextObj.__init__(self, parent, name, visible)
+
+    async def init(
+            self, *,
+            step: int, value: int,
+            **kwargs
+    ) -> 'Slider':
+        self.setFocusPolicy(Qt.StrongFocus)
+        self.setTickPosition(QSlider.TickPosition.TicksBothSides)
+        self.setTickInterval(10)
+        self.setSingleStep(step)
+        self.setValue(value)
+        return await self.apply(**kwargs)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/popup.py` & `aioqui-2.0.0/src/aioqui/widgets/custom/popup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from PySide6.QtGui import QResizeEvent
-from PySide6.QtWidgets import QMessageBox, QWidget
+from PySide6.QtWidgets import QMessageBox
 from qasync import asyncSlot
 from typing import Iterable
 
-from .widget import Widget
-from .layout import Layout
-from .button import Button
-from .label import Label
-from .frame import Frame
+from .. import Widget, Layout, Button, Label, Frame
+from ...types import Parent
 
 
 class Popup(Widget):
     YES = QMessageBox.StandardButton.Yes
     NO = QMessageBox.StandardButton.No
     OK = QMessageBox.StandardButton.Ok
     CANCEL = QMessageBox.StandardButton.Cancel
@@ -62,52 +59,52 @@
 
         #PopupCancelBtn:hover,
         #PopupNoBtn:hover {{
             background-color: rgba(182, 0, 40, 0.5);
         }}
         '''
 
-    def __init__(self, parent: QWidget, name: str = None, stylesheet: str = stylesheet):
+    def __init__(self, parent: Parent, name: str = None, stylesheet: str = stylesheet):
         super().__init__(parent, name if name else self.__class__.__name__, True, stylesheet)
 
     @asyncSlot()
     async def display(
             self, *,
             message: str = '', buttons: Iterable = (),
             on_success: callable = lambda: None, on_failure: callable = lambda: None
     ) -> 'Popup':
         if not buttons:
             buttons = [Popup.YES, Popup.NO]
         btns = []
         if Popup.YES in buttons:
             btns.append(await Button(self, f'{self.objectName()}YesBtn').init(
-                text='Yes', events=Button.Events(on_click=lambda: self.slot(on_success))
+                text='Yes', on_click=lambda: self.slot(on_success)
             ))
         if Popup.NO in buttons:
             btns.append(await Button(self, f'{self.objectName()}NoBtn').init(
-                text='No', events=Button.Events(on_click=lambda: self.slot(on_failure))
+                text='No', on_click=lambda: self.slot(on_failure)
             ))
         if Popup.OK in buttons:
             btns.append(await Button(self, f'{self.objectName()}OkBtn').init(
-                text='Ok', events=Button.Events(on_click=lambda: self.slot(on_success))
+                text='Ok', on_click=lambda: self.slot(on_success)
             ))
         if Popup.CANCEL in buttons:
             btns.append(await Button(self, f'{self.objectName()}CancelBtn').init(
-                text='Cancel', events=Button.Events(on_click=lambda: self.slot(on_failure))
+                text='Cancel', on_click=lambda: self.slot(on_failure)
             ))
 
         self.setLayout(await Layout.vertical().init(
             spacing=10, alignment=Layout.Center, margins=(20, 20, 20, 20),
             items=[
                 await Frame(self, f'{self.objectName()}Frame').init(
                     layout=await Layout.vertical().init(
                         spacing=20, margins=(20, 20, 20, 20),
                         items=[
                             await Label(self, f'{self.objectName()}MessageLbl').init(
-                                text=message, wrap=True, sizes=Label.Sizes(alignment=Layout.Center)
+                                text=message, wrap=True, alignment=Layout.Center
                             ),
                             await Layout.horizontal().init(
                                 spacing=20, items=btns
                             )
                         ]
                     )
                 )
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/scroll_area.py` & `aioqui-2.0.0/src/aioqui/widgets/scroll_area.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from PySide6.QtWidgets import QScrollArea, QWidget
+from PySide6.QtWidgets import QScrollArea
 from PySide6.QtCore import QObject
 from typing import Sequence, Iterable
 
 from .frame import Frame
 from .layout import Layout
-from ..objects import ContextObj, SizedObj, EventedObj
+from ..context import ContextObj
 from ..enums import Orientation, ScrollPolicy
-from ..types import Applicable
+from ..types import QSS, Parent
 
 
 class ScrollArea(ContextObj, ScrollPolicy, Orientation, QScrollArea):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
         QScrollArea.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        if stylesheet:
-            self.setStyleSheet(stylesheet)
+        self.qss = qss
 
     async def init(
             self, *,
             orientation: Orientation.Orientation,
             hpolicy: ScrollPolicy.ScrollPolicy = ScrollPolicy.WhenNeeded,
             vpolicy: ScrollPolicy.ScrollPolicy = ScrollPolicy.WhenNeeded,
 
             margins: tuple[int, ...] = (0, 0, 0, 0), spacing: int = 0, alignment: Layout.Alignment = None,
             items: Sequence[QObject] = (),
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+
+            **kwargs
     ) -> 'ScrollArea':
         self.setHorizontalScrollBarPolicy(hpolicy)
         self.setVerticalScrollBarPolicy(vpolicy)
         self.setWidgetResizable(True)
         frame = Frame(self, f'{self.objectName()}Widget')
         self.setWidget(await frame.init(
             layout=await Layout.oriented(orientation, frame, f'{frame.objectName()}Layout').init(
                 margins=margins, spacing=spacing, alignment=alignment, items=items
             )
         ))
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
 
-    def addWidget(self, widget: QWidget) -> None:
+    def addWidget(self, widget: Parent) -> None:
         self.widget().layout().addWidget(widget)
 
     def clear(self, exceptions: Iterable[QObject] = ()):
         self.widget().layout().clear(exceptions)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/selector.py` & `aioqui-2.0.0/src/aioqui/widgets/selector.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-from PySide6.QtWidgets import QComboBox, QWidget
+from PySide6.QtWidgets import QComboBox
 from typing import Iterable, Any
 
-from ..objects import ContextObj, SizedObj, EventedObj
-from ..types import Applicable, Icon
+from ..context import ContextObj
+from ..types import Icon, QSS, Parent
 
 
 class Selector(ContextObj, QComboBox):
     class Item:
         def __init__(self, text: str, icon: Icon = None, data: Any = None):
             self.params = []
             if icon:
-                self.params.append(icon)
+                self.params.append(icon.icon)
             self.params.append(str(text))
             if data:
                 self.params.append(data)
 
-    def __init__(self, parent: QWidget, name: str, visible: bool = True):
-        QComboBox.__init__(self)
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
+        QComboBox.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
+        self.qss = qss
 
     async def init(
             self, *,
             items: Iterable[Item | str] = (),
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            **kwargs
     ) -> 'Selector':
         for item in items:
             if isinstance(item, Selector.Item):
                 self.addItem(*item.params)
             elif isinstance(item, str):
                 self.addItem(item)
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
 
     def setCurrentText(self, text: Any) -> None:
         super().setCurrentText(str(text))
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/splitter.py` & `aioqui-2.0.0/src/aioqui/widgets/splitter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,46 +1,41 @@
-from PySide6.QtWidgets import QWidget, QSplitter, QSizePolicy
-from PySide6.QtCore import Qt
+from PySide6.QtWidgets import QSplitter
 from typing import Iterable
 
-from .widget import Widget
+from .frame import Frame
 from .extensions import SplitterWidgetExt
-from ..objects import ContextObj
+from ..context import ContextObj
 from ..enums import Orientation
+from ..types import QSS, Parent
 
 
-class SplitterHandle(Widget):
-    def __init__(self, parent: QWidget, name: str):
-        super().__init__(parent, name, True)
-
-
-class SplitterWidget(SplitterWidgetExt, Widget):
-    def __init__(self, parent: QWidget, name: str,
-                 expand_to: int, expand_min: int = None, expand_max: int = None,
-                 orientation: Orientation.Orientation = None):
-        Widget.__init__(self, parent, name, True)
-        SplitterWidgetExt.__init__(self, expand_to, expand_min, expand_max, orientation)
-
-
-class Splitter(ContextObj, QSplitter):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = None,
-                 orientation: Orientation.Orientation = Orientation.Horizontal,
-                 policy: tuple[QSizePolicy, QSizePolicy] = (QSizePolicy.Expanding, QSizePolicy.Expanding)):
+class Splitter(ContextObj, Orientation, QSplitter):
+    class Handle(Frame):
+        def __init__(self, parent: Parent, name: str):
+            super().__init__(parent, name, True)
+
+    class Widget(SplitterWidgetExt, Frame):
+        def __init__(self, parent: Parent, name: str, *, collapsible: bool = True,
+                     expand_to: int, expand_min: int = None, expand_max: int = None):
+            Frame.__init__(self, parent, name, True)
+            SplitterWidgetExt.__init__(self, expand_to, expand_min, expand_max, collapsible)
+
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None,
+                 orientation: Orientation.Orientation = Orientation.Horizontal):
         QSplitter.__init__(self, orientation, parent)
         ContextObj.__init__(self, parent, name, visible)
-        if stylesheet:
-            self.setStyleSheet(stylesheet)
-            self.setAttribute(Qt.WA_StyledBackground, True)
-        self.setSizePolicy(*policy)
+        self.qss = qss
 
     async def init(
             self, *,
-            items: Iterable[QWidget] = ()
+            items: Iterable[Widget] = (),
+            **kwargs
     ) -> 'Splitter':
         for item in items:
             self.addWidget(item)
-        return self
+        return await self._apply(**kwargs)
 
-    def addWidget(self, widget: QWidget, collapsible: bool = True) -> None:
+    def addWidget(self, widget: Widget) -> None:
         super().addWidget(widget)
-        self.setCollapsible(self.count() - 1, collapsible)
         widget.splitter = self
+        widget.orientation = self.orientation()
+        self.setCollapsible(self.count() - 1, widget.collapsible)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/stacked_widget.py` & `aioqui-2.0.0/src/aioqui/widgets/stacked_widget.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,30 @@
-from PySide6.QtWidgets import QWidget, QStackedWidget
-from PySide6.QtCore import Qt, QObject
+from PySide6.QtWidgets import QStackedWidget, QFrame
+from PySide6.QtCore import QObject
 from typing import Iterable
 
-from ..objects import ContextObj, SizedObj, EventedObj
+from ..context import ContextObj
 from ..enums import Alignment, Orientation
-from ..types import Applicable
+from ..types import QSS, Parent
 
 
 class StackedWidget(ContextObj, Orientation, QStackedWidget):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
+    def __init__(self, parent: Parent, name: str, visible: bool = True, qss: QSS = None):
         QStackedWidget.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        self.setStyleSheet(stylesheet)
-        self.setAttribute(Qt.WA_StyledBackground, True)
+        self.qss = qss
 
         # workaround which includes override of `setCurrentIndex`, otherwise problems with `parent()`
-        self.addWidget(QWidget(self))
+        self.addWidget(QFrame(self))  # QFrame is likely the most lightweight QWidget in Qt6
 
     async def init(
             self, *,
             alignment: Alignment.Alignment = Alignment.HCenter, items: Iterable[QObject] = (),
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            **kwargs
     ) -> 'StackedWidget':
         self.layout().setAlignment(alignment)
         for item in items:
             self.addWidget(item)
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
 
     def setCurrentIndex(self, index: int) -> None:
         super().setCurrentIndex(index + 1)
```

### Comparing `aioqui-1.1.7/src/aioqui/widgets/widget.py` & `aioqui-2.0.0/src/aioqui/widgets/widget.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from PySide6.QtWidgets import QWidget, QLayout
-from PySide6.QtCore import Qt
 
-from ..objects import ContextObj, SizedObj, EventedObj
-from ..types import Applicable
+from ..context import ContextObj
+from ..types import QSS
 
 
 class Widget(ContextObj, QWidget):
-    def __init__(self, parent: QWidget, name: str, visible: bool = True, stylesheet: str = ''):
+    def __init__(self, parent: QWidget, name: str, visible: bool = True, qss: QSS = None):
         QWidget.__init__(self, parent)
         ContextObj.__init__(self, parent, name, visible)
-        self.setAttribute(Qt.WA_StyledBackground, True)
-        self.setStyleSheet(stylesheet)
+        self.qss = qss
 
     async def init(
             self, *,
             layout: QLayout = None,
-            sizes: Applicable = SizedObj.Sizes(), events: Applicable = EventedObj.Events()
+            **kwargs
     ) -> 'Widget':
         if layout:
             self.setLayout(layout)
-        return await sizes(await events(self))
+        return await self._apply(**kwargs)
```

### Comparing `aioqui-1.1.7/src/aioqui.egg-info/PKG-INFO` & `aioqui-2.0.0/src/aioqui.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioqui
-Version: 1.1.7
+Version: 2.0.0
 Summary: Asynchronous GUI framework based on PySide6
 Author-email: cxllmerichie <cxllmerichie@gmail.com>
 Maintainer-email: cxllmerichie <cxllmerichie@gmail.com>
 License: MIT License
         
         Copyright (c) 2022-2023 cxllmerichie
         
@@ -26,26 +26,31 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/cxllmerichie/aioqui
 Project-URL: Bug Tracker, https://github.com/cxllmerichie/aioqui/issues
 Project-URL: Repository, https://github.com/cxllmerichie/aioqui
 Project-URL: Documentation, https://github.com/cxllmerichie/aioqui/README.md
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: Software Development :: User Interfaces
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Natural Language :: English
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# ToDo:
-- favourite_button is actually a StateButton ? IconButton
-- error_label is actually a PopupTextLabel ? DelayLabel
-- make all widgets to have:
-    - margins (in abstract frame)
-    - padding (in abstract frame)
-    - alignment (in abstract frame)
-- make popup to be generic (configure different buttons (ok, cancel, no, yes)
-- crete generic animation class to create simple animations
+## Overview
+## Documentation
+## Installation
+```
+pip install aioqui
+```
+### Package dependencies
+includes ```pip install pyside6 qasync loguru```
+
+speedups ```pip install aiodns ujson cchardet uvloop```
+
+depending on modules [optional] ```pip install aiohttp uvicorn```
```

### Comparing `aioqui-1.1.7/src/aioqui.egg-info/SOURCES.txt` & `aioqui-2.0.0/src/aioqui.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/__init__.py
 src/aioqui/__init__.py
-src/aioqui/contextapi.py
 src/aioqui/qasyncio.py
 src/aioqui.egg-info/PKG-INFO
 src/aioqui.egg-info/SOURCES.txt
 src/aioqui.egg-info/dependency_links.txt
 src/aioqui.egg-info/requires.txt
 src/aioqui.egg-info/top_level.txt
 src/aioqui/.assets/icons/activity.svg
@@ -297,57 +296,58 @@
 src/aioqui/.assets/icons/x-square.svg
 src/aioqui/.assets/icons/x.svg
 src/aioqui/.assets/icons/youtube.svg
 src/aioqui/.assets/icons/zap-off.svg
 src/aioqui/.assets/icons/zap.svg
 src/aioqui/.assets/icons/zoom-in.svg
 src/aioqui/.assets/icons/zoom-out.svg
+src/aioqui/context/__init__.py
+src/aioqui/context/context_obj.py
+src/aioqui/context/contextapi.py
 src/aioqui/enums/__init__.py
 src/aioqui/enums/alignment.py
+src/aioqui/enums/echo_mode.py
 src/aioqui/enums/elide_mode.py
 src/aioqui/enums/orientation.py
 src/aioqui/enums/scroll_policy.py
 src/aioqui/enums/size_policy.py
 src/aioqui/enums/window_hint.py
 src/aioqui/misc/__init__.py
 src/aioqui/misc/aiorequest.py
-src/aioqui/misc/ctq.py
-src/aioqui/misc/dialogs.py
-src/aioqui/misc/parser.py
-src/aioqui/misc/server.py
+src/aioqui/misc/animation.py
+src/aioqui/misc/conthrq.py
+src/aioqui/misc/fileops.py
+src/aioqui/misc/qss_parser.py
 src/aioqui/misc/utils.py
-src/aioqui/objects/__init__.py
-src/aioqui/objects/context_obj.py
-src/aioqui/objects/evented_obj.py
-src/aioqui/objects/sized_obj.py
+src/aioqui/misc/uvithread.py
 src/aioqui/types/__init__.py
 src/aioqui/types/common.py
 src/aioqui/types/icon.py
 src/aioqui/types/size.py
 src/aioqui/widgets/__init__.py
 src/aioqui/widgets/button.py
 src/aioqui/widgets/frame.py
+src/aioqui/widgets/input.py
 src/aioqui/widgets/label.py
 src/aioqui/widgets/layout.py
-src/aioqui/widgets/line_input.py
-src/aioqui/widgets/popup.py
 src/aioqui/widgets/scroll_area.py
 src/aioqui/widgets/selector.py
 src/aioqui/widgets/slider.py
 src/aioqui/widgets/spacer.py
 src/aioqui/widgets/splitter.py
 src/aioqui/widgets/stacked_widget.py
 src/aioqui/widgets/statusbar.py
-src/aioqui/widgets/text_input.py
 src/aioqui/widgets/widget.py
 src/aioqui/widgets/window.py
 src/aioqui/widgets/custom/__init__.py
 src/aioqui/widgets/custom/date_picker.py
 src/aioqui/widgets/custom/error_label.py
-src/aioqui/widgets/custom/favourite_button.py
 src/aioqui/widgets/custom/image_button.py
 src/aioqui/widgets/custom/menu_button.py
-src/aioqui/widgets/custom/search_bar.py
+src/aioqui/widgets/custom/popup.py
+src/aioqui/widgets/custom/searchbar.py
+src/aioqui/widgets/custom/state_icon_btn.py
 src/aioqui/widgets/extensions/__init__.py
+src/aioqui/widgets/extensions/input_ext.py
 src/aioqui/widgets/extensions/layout_ext.py
 src/aioqui/widgets/extensions/side_menu_ext.py
 src/aioqui/widgets/extensions/splitter_widget_ext.py
```

