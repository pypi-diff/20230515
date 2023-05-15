# Comparing `tmp/pqmusic-1.2.1.tar.gz` & `tmp/pqmusic-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqmusic-1.2.1.tar", last modified: Fri Jul 29 19:45:25 2022, max compression
+gzip compressed data, was "pqmusic-1.3.0.tar", last modified: Mon May 15 20:06:39 2023, max compression
```

## Comparing `pqmusic-1.2.1.tar` & `pqmusic-1.3.0.tar`

### file list

```diff
@@ -1,38 +1,164 @@
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.819740 pqmusic-1.2.1/
--rw-r--r--   0 son_link  (1000) son_link  (1000)    35149 2022-04-24 14:11:12.000000 pqmusic-1.2.1/LICENSE
--rw-r--r--   0 son_link  (1000) son_link  (1000)     4431 2022-07-29 19:45:25.819740 pqmusic-1.2.1/PKG-INFO
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.816407 pqmusic-1.2.1/PQMusic/
--rw-r--r--   0 son_link  (1000) son_link  (1000)   529672 2011-02-01 22:00:00.000000 pqmusic-1.2.1/PQMusic/OpenSans.ttf
--rwxr-xr-x   0 son_link  (1000) son_link  (1000)      180 2022-06-28 17:02:02.000000 pqmusic-1.2.1/PQMusic/PQMusic.pro
--rw-r--r--   0 son_link  (1000) son_link  (1000)    16309 2022-07-29 16:44:30.000000 pqmusic-1.2.1/PQMusic/__init__.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)    10920 2022-05-10 04:38:23.000000 pqmusic-1.2.1/PQMusic/__init__.py.bck
--rw-r--r--   0 son_link  (1000) son_link  (1000)     4692 2022-07-26 18:36:33.000000 pqmusic-1.2.1/PQMusic/config.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     2174 2022-07-25 20:01:21.000000 pqmusic-1.2.1/PQMusic/covers.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     5790 2022-04-24 11:25:21.000000 pqmusic-1.2.1/PQMusic/icon.svg
--rwxr-xr-x   0 son_link  (1000) son_link  (1000)     2641 2022-06-29 15:04:29.000000 pqmusic-1.2.1/PQMusic/images.qrc
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.816407 pqmusic-1.2.1/PQMusic/locales/
--rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-07-26 12:52:12.000000 pqmusic-1.2.1/PQMusic/locales/es.qm
--rw-r--r--   0 son_link  (1000) son_link  (1000)      872 2022-07-08 15:12:47.000000 pqmusic-1.2.1/PQMusic/minimal-player.spec
--rw-r--r--   0 son_link  (1000) son_link  (1000)    11295 2022-04-24 13:26:03.000000 pqmusic-1.2.1/PQMusic/no_cover.svg
--rw-r--r--   0 son_link  (1000) son_link  (1000)    17607 2022-07-27 17:48:39.000000 pqmusic-1.2.1/PQMusic/player.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)    13716 2022-05-07 13:22:17.000000 pqmusic-1.2.1/PQMusic/player.py.bck
--rw-r--r--   0 son_link  (1000) son_link  (1000)    10327 2022-05-07 13:12:06.000000 pqmusic-1.2.1/PQMusic/style.qss
--rw-r--r--   0 son_link  (1000) son_link  (1000)     7235 2022-06-29 14:40:39.000000 pqmusic-1.2.1/PQMusic/sys_notify.py
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.819740 pqmusic-1.2.1/PQMusic/ui/
--rw-r--r--   0 son_link  (1000) son_link  (1000)     2614 2022-04-29 15:00:27.000000 pqmusic-1.2.1/PQMusic/ui/Ui_add_url_dialog.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     4054 2022-07-26 18:33:05.000000 pqmusic-1.2.1/PQMusic/ui/Ui_config.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)    11983 2022-07-26 05:46:52.000000 pqmusic-1.2.1/PQMusic/ui/Ui_gui.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)   725859 2022-07-27 17:56:04.000000 pqmusic-1.2.1/PQMusic/ui/images_rc.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     2137 2022-04-29 05:47:49.000000 pqmusic-1.2.1/PQMusic/ui/open_url_dialog.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     5088 2022-07-26 20:09:34.000000 pqmusic-1.2.1/PQMusic/utils.py
--rw-r--r--   0 son_link  (1000) son_link  (1000)     3217 2022-07-29 16:58:57.000000 pqmusic-1.2.1/README.md
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.819740 pqmusic-1.2.1/bin/
--rwxr-xr-x   0 son_link  (1000) son_link  (1000)      486 2022-06-29 15:33:44.000000 pqmusic-1.2.1/bin/pqmusic
-drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2022-07-29 19:45:25.819740 pqmusic-1.2.1/pqmusic.egg-info/
--rw-r--r--   0 son_link  (1000) son_link  (1000)     4431 2022-07-29 19:45:25.000000 pqmusic-1.2.1/pqmusic.egg-info/PKG-INFO
--rw-r--r--   0 son_link  (1000) son_link  (1000)      658 2022-07-29 19:45:25.000000 pqmusic-1.2.1/pqmusic.egg-info/SOURCES.txt
--rw-r--r--   0 son_link  (1000) son_link  (1000)        1 2022-07-29 19:45:25.000000 pqmusic-1.2.1/pqmusic.egg-info/dependency_links.txt
--rw-r--r--   0 son_link  (1000) son_link  (1000)       34 2022-07-29 19:45:25.000000 pqmusic-1.2.1/pqmusic.egg-info/requires.txt
--rw-r--r--   0 son_link  (1000) son_link  (1000)        8 2022-07-29 19:45:25.000000 pqmusic-1.2.1/pqmusic.egg-info/top_level.txt
--rw-r--r--   0 son_link  (1000) son_link  (1000)      184 2022-07-29 19:45:25.819740 pqmusic-1.2.1/setup.cfg
--rwxr-xr-x   0 son_link  (1000) son_link  (1000)     1695 2022-07-29 16:59:59.000000 pqmusic-1.2.1/setup.py
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:06:39.518731 pqmusic-1.3.0/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)        0 2022-07-08 15:12:47.000000 pqmusic-1.3.0/.SRCINFO
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.011651 pqmusic-1.3.0/.github/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.044984 pqmusic-1.3.0/.github/workflows/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     1306 2023-05-15 11:48:36.000000 pqmusic-1.3.0/.github/workflows/main.yml
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)      194 2022-05-17 15:16:54.000000 pqmusic-1.3.0/.gitignore
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4453 2023-05-15 19:51:20.000000 pqmusic-1.3.0/CHANGELOG.md
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    35149 2022-04-24 14:11:12.000000 pqmusic-1.3.0/LICENSE
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4489 2023-05-15 20:06:39.522065 pqmusic-1.3.0/PKG-INFO
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.068318 pqmusic-1.3.0/PQMusic/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)   529672 2011-02-01 22:00:00.000000 pqmusic-1.3.0/PQMusic/OpenSans.ttf
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)      180 2022-06-28 17:02:02.000000 pqmusic-1.3.0/PQMusic/PQMusic.pro
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    16018 2023-05-15 10:13:51.000000 pqmusic-1.3.0/PQMusic/__init__.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    10920 2022-05-10 04:38:23.000000 pqmusic-1.3.0/PQMusic/__init__.py.bck
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4669 2023-05-08 14:15:36.000000 pqmusic-1.3.0/PQMusic/config.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     2283 2023-05-15 17:59:05.000000 pqmusic-1.3.0/PQMusic/covers.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     1291 2023-03-31 17:31:17.000000 pqmusic-1.3.0/PQMusic/dbus.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     5790 2022-04-24 11:25:21.000000 pqmusic-1.3.0/PQMusic/icon.svg
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.011651 pqmusic-1.3.0/PQMusic/icons/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.071651 pqmusic-1.3.0/PQMusic/icons/luv/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/PQMusic/icons/luv/actions/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.084985 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3907 2022-05-07 06:42:29.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/application-exit.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3336 2022-05-07 06:42:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/application-menu.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3948 2022-04-23 18:31:53.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/audio-volume-high.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3775 2022-06-29 15:03:10.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/configure.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3897 2022-05-05 20:15:43.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/document-export.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4329 2022-05-05 20:15:57.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/document-import.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3547 2022-04-23 18:32:11.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/edit-clear-all.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3491 2022-04-27 05:05:57.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/folder-add.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3288 2022-04-23 18:32:19.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/list-add.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3002 2022-04-23 18:32:26.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/list-remove.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3346 2022-04-23 18:32:32.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-playback-pause.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3429 2022-04-23 17:07:31.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-playback-start.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4547 2022-05-01 20:34:23.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-playlist-normal.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4255 2022-04-23 18:33:12.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-playlist-repeat.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     5461 2022-04-23 18:33:07.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-playlist-shuffle.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)      818 2022-04-03 00:10:25.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-repeat-playlist-amarok.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     1789 2022-05-02 11:08:20.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-repeat-song.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3319 2022-04-23 17:09:26.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-skip-backward.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3282 2022-04-23 17:09:48.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/media-skip-forward.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3504 2022-04-27 19:07:46.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/view-links.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3269 2022-04-23 18:32:40.000000 pqmusic-1.3.0/PQMusic/icons/luv/actions/22/view-media-playlist.svg
+-rwxrwxrw-   0 son_link  (1000) son_link  (1000)      230 2022-04-27 05:54:26.000000 pqmusic-1.3.0/PQMusic/icons/luv/index.theme
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/PQMusic/icons/luv/places/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.101651 pqmusic-1.3.0/PQMusic/icons/luv/places/22/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3293 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-cloud-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3293 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-cloud.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-documents-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-documents.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3417 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-download-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3417 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-download.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4012 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-music-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4012 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-music.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3798 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-network.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3704 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-pictures.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3519 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-publicshare.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3370 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4646 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-templates.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3338 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-videos-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3338 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder-videos.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3370 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/folder.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3798 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/network-workgroup.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3305 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/start-here.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3682 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/user-desktop.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4886 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/user-home-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4886 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/user-home.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3710 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/user-trash-full.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3504 2022-04-22 20:36:05.000000 pqmusic-1.3.0/PQMusic/icons/luv/places/22/user-trash.svg
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)     2641 2022-06-29 15:04:29.000000 pqmusic-1.3.0/PQMusic/images.qrc
+-rw-r--r--   0 son_link  (1000) son_link  (1000)   911701 2023-05-15 20:04:27.444986 pqmusic-1.3.0/PQMusic/images_rc.py
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.101651 pqmusic-1.3.0/PQMusic/locales/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-07-26 12:52:12.000000 pqmusic-1.3.0/PQMusic/locales/es.qm
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     6057 2022-07-26 12:52:10.000000 pqmusic-1.3.0/PQMusic/locales/es.ts
+-rw-r--r--   0 son_link  (1000) son_link  (1000)      872 2022-07-08 15:12:47.000000 pqmusic-1.3.0/PQMusic/minimal-player.spec
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    11295 2022-04-24 13:26:03.000000 pqmusic-1.3.0/PQMusic/no_cover.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    18398 2023-05-15 18:01:03.000000 pqmusic-1.3.0/PQMusic/player.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    13716 2022-05-07 13:22:17.000000 pqmusic-1.3.0/PQMusic/player.py.bck
+-rw-r--r--   0 son_link  (1000) son_link  (1000)   911083 2023-04-01 09:08:59.000000 pqmusic-1.3.0/PQMusic/rc_images.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    10327 2022-05-07 13:12:06.000000 pqmusic-1.3.0/PQMusic/style.qss
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     7235 2023-05-15 07:01:23.000000 pqmusic-1.3.0/PQMusic/sys_notify.py.bck
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.484986 pqmusic-1.3.0/PQMusic/ui/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     2614 2022-04-29 15:00:27.000000 pqmusic-1.3.0/PQMusic/ui/Ui_add_url_dialog.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4054 2022-07-26 18:33:05.000000 pqmusic-1.3.0/PQMusic/ui/Ui_config.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    12149 2022-08-20 12:17:21.000000 pqmusic-1.3.0/PQMusic/ui/Ui_gui.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     2839 2022-04-29 14:59:13.000000 pqmusic-1.3.0/PQMusic/ui/add_url_dialog.ui
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3392 2023-05-15 20:04:27.384986 pqmusic-1.3.0/PQMusic/ui/add_url_dialog_ui.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3513 2022-07-26 18:29:13.000000 pqmusic-1.3.0/PQMusic/ui/config.ui
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     5250 2023-05-15 20:04:27.451652 pqmusic-1.3.0/PQMusic/ui/config_ui.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    14544 2022-08-20 12:17:09.000000 pqmusic-1.3.0/PQMusic/ui/gui.ui
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    16399 2023-05-15 20:04:27.484986 pqmusic-1.3.0/PQMusic/ui/gui_ui.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)   725859 2022-07-27 17:56:04.000000 pqmusic-1.3.0/PQMusic/ui/images_rc.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     2137 2022-04-29 05:47:49.000000 pqmusic-1.3.0/PQMusic/ui/open_url_dialog.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     7890 2023-05-15 13:11:53.000000 pqmusic-1.3.0/PQMusic/utils.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3244 2023-05-15 16:35:02.000000 pqmusic-1.3.0/README.md
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.111651 pqmusic-1.3.0/bin/
+-rwxrwxrwx   0 son_link  (1000) son_link  (1000)      229 2022-05-10 04:53:41.000000 pqmusic-1.3.0/bin/AppRun.sh
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     1851 2022-07-29 17:01:12.000000 pqmusic-1.3.0/bin/io.sonlink.pqmusic.appdata.xml
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)      461 2022-05-17 15:16:54.000000 pqmusic-1.3.0/bin/io.sonlink.pqmusic.desktop
+-rw-------   0 son_link  (1000) son_link  (1000)    11391 2022-05-08 06:58:46.000000 pqmusic-1.3.0/bin/io.sonlink.pqmusic.png
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     5790 2022-04-24 11:25:21.000000 pqmusic-1.3.0/bin/io.sonlink.pqmusic.svg
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)      486 2022-06-29 15:33:44.000000 pqmusic-1.3.0/bin/pqmusic
+-rwxrwx---   0 son_link  (1000) son_link  (1000)     1055 2023-05-15 12:46:48.000000 pqmusic-1.3.0/build-appimage.sh
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    41401 2022-05-17 17:11:44.000000 pqmusic-1.3.0/file-manager-menu.png
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/icons/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.111651 pqmusic-1.3.0/icons/luv/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/icons/luv/actions/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.118318 pqmusic-1.3.0/icons/luv/actions/22/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3336 2022-04-23 18:31:04.000000 pqmusic-1.3.0/icons/luv/actions/22/application-menu.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3948 2022-04-23 18:31:53.000000 pqmusic-1.3.0/icons/luv/actions/22/audio-volume-high.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3547 2022-04-23 18:32:11.000000 pqmusic-1.3.0/icons/luv/actions/22/edit-clear-all.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3288 2022-04-23 18:32:19.000000 pqmusic-1.3.0/icons/luv/actions/22/list-add.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3002 2022-04-23 18:32:26.000000 pqmusic-1.3.0/icons/luv/actions/22/list-remove.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3346 2022-04-23 18:32:32.000000 pqmusic-1.3.0/icons/luv/actions/22/media-playback-pause.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3429 2022-04-23 17:07:31.000000 pqmusic-1.3.0/icons/luv/actions/22/media-playback-start.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4255 2022-04-23 18:33:12.000000 pqmusic-1.3.0/icons/luv/actions/22/media-playlist-repeat.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     5461 2022-04-23 18:33:07.000000 pqmusic-1.3.0/icons/luv/actions/22/media-playlist-shuffle.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3319 2022-04-23 17:09:26.000000 pqmusic-1.3.0/icons/luv/actions/22/media-skip-backward.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3282 2022-04-23 17:09:48.000000 pqmusic-1.3.0/icons/luv/actions/22/media-skip-forward.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3269 2022-04-23 18:32:40.000000 pqmusic-1.3.0/icons/luv/actions/22/view-media-playlist.svg
+-rwxrwxrw-   0 son_link  (1000) son_link  (1000)      157 2022-04-22 20:48:46.000000 pqmusic-1.3.0/icons/luv/index.theme
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/icons/luv/places/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.131651 pqmusic-1.3.0/icons/luv/places/22/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3293 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-cloud-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3293 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-cloud.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-documents-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3277 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-documents.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3417 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-download-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3417 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-download.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4012 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-music-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4012 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-music.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3798 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-network.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3704 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-pictures.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3519 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-publicshare.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3370 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4646 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-templates.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3338 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-videos-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3338 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder-videos.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3370 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/folder.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3798 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/network-workgroup.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3305 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/start-here.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3682 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/user-desktop.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4886 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/user-home-sidebar.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4886 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/user-home.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3710 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/user-trash-full.svg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3504 2022-04-22 20:36:05.000000 pqmusic-1.3.0/icons/luv/places/22/user-trash.svg
+-rwxrwx--x   0 son_link  (1000) son_link  (1000)     7259 2021-02-17 11:04:51.000000 pqmusic-1.3.0/linuxdeploy-plugin-conda.sh
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     3064 2022-04-24 10:49:52.000000 pqmusic-1.3.0/musical-note-2-dennis-b-01r.svg
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.014984 pqmusic-1.3.0/packages/
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:04:27.131651 pqmusic-1.3.0/packages/aur/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)      548 2022-05-07 13:29:07.000000 pqmusic-1.3.0/packages/aur/.SRCINFO
+-rw-r--r--   0 son_link  (1000) son_link  (1000)      934 2022-05-17 15:16:54.000000 pqmusic-1.3.0/packages/aur/PKGBUILD
+-rw-r--r--   0 son_link  (1000) son_link  (1000)   855032 2022-05-17 14:39:56.000000 pqmusic-1.3.0/pqmusic-drag-drop.mp4
+drwxr-xr-x   0 son_link  (1000) son_link  (1000)        0 2023-05-15 20:06:39.522065 pqmusic-1.3.0/pqmusic.egg-info/
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4489 2023-05-15 20:06:39.000000 pqmusic-1.3.0/pqmusic.egg-info/PKG-INFO
+-rw-r--r--   0 son_link  (1000) son_link  (1000)     4875 2023-05-15 20:06:39.000000 pqmusic-1.3.0/pqmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 son_link  (1000) son_link  (1000)        1 2023-05-15 20:06:39.000000 pqmusic-1.3.0/pqmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 son_link  (1000) son_link  (1000)       43 2023-05-15 20:06:39.000000 pqmusic-1.3.0/pqmusic.egg-info/requires.txt
+-rw-r--r--   0 son_link  (1000) son_link  (1000)        8 2023-05-15 20:06:39.000000 pqmusic-1.3.0/pqmusic.egg-info/top_level.txt
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)       43 2023-05-15 11:41:05.000000 pqmusic-1.3.0/requirements.txt
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    32222 2022-05-06 16:37:45.000000 pqmusic-1.3.0/screenshoot.jpg
+-rw-r--r--   0 son_link  (1000) son_link  (1000)      184 2023-05-15 20:06:39.522065 pqmusic-1.3.0/setup.cfg
+-rwxr-xr-x   0 son_link  (1000) son_link  (1000)     1811 2023-05-15 20:06:33.000000 pqmusic-1.3.0/setup.py
+-rw-r--r--   0 son_link  (1000) son_link  (1000)    10594 2022-05-07 13:07:32.000000 pqmusic-1.3.0/style.qsst
```

### Comparing `pqmusic-1.2.1/LICENSE` & `pqmusic-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PKG-INFO` & `pqmusic-1.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pqmusic
-Version: 1.2.1
+Version: 1.3.0
 Summary: A minimal music player.
 Home-page: https://github.com/son-link/PQMusic
-Download-URL: https://github.com/son-link/PQMusic/archive/refs/tags/v.1.1.1.tar.gz
+Download-URL: https://github.com/son-link/PQMusic/archive/refs/tags/v.1.3.0.tar.gz
 Author: Alfonso Saavedra 'Son Link'
 Author-email: sonlink.dourden@gmail.com
 License: GPL 3.0
 Keywords: music,audio,player
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PQMusic
 
@@ -38,43 +38,41 @@
 
 [https://github.com/son-link/PQMusic](https://github.com/son-link/PQMusic)
 
 ![PQMusic screenshoot](screenshoot.jpg)
 
 PQMusic is a minimalist and easy to use audio player for download and use.
 
-You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format.
+You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format. Also you can play some music trackers files (.it, .mod, .s3m and .xm)
 
 Adding files from Open with on your file manager
 ![Add files from Open with on your file manager](file-manager-menu.png)
 
 Drag and drop files to PQMusic's window:
 
 <video controls style="max-width: 720px">
   <source src="pqmusic-drag-drop.mp4" />
 </video>
 
 Only available for Linux.
 
 Licensed under GNU/GPL3 or higher.
 
-**Note**: this project is still under development, so some features are not yet available or complete.
-
 ## Install
 
 ### From source code:
 
 * Clone the repo, download the zip under Code -> Download ZIP or download the last release.
 * Open a terminal and go to the project folder.
 * Install the dependencies:
-  * **From PIP** (with administration permissions): `pip install -r requirements.txt`
+  * **From PIP**: `pip install -r requirements.txt` *use the --user parameter if you want to install the dependencies at your user level*
   * **Debian/Ubuntu/Mint/MX Linux**:
-    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic dbus-python`
+    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic python3-requests`
   * **Arch Linux/Manjaro**:
-    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic dbus-python`
+    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic python-requests`
 
   * Copy the icon and desktop file:
     * All users:
       * `install -m 644 bin/io.sonlink.pqmusic.desktop /usr/share/applications`
   	  * `install -m 644 bin/io.sonlink.pqmusic.svg /usr/share/icons/pqmusic.svg`
   	* Current user:
   	  * `cp bin/io.sonlink.pqmusic.desktop ~/.local/share/applications`
@@ -82,15 +80,15 @@
 
 ### From Pypi:
 
 `pip install PQMusic`
 
 ### AUR:
 
-If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install yhe official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
+If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install the official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
 
 For example: `yay -S pqmusic`
 
 ### Executables:
 
 You can download a **AppImage** for **GNU/Linux** on [releases page](https://github.com/son-link/PQMusic/releases)
 
@@ -113,9 +111,7 @@
 * Lüv icons theme: https://github.com/Nitrux/luv-icon-theme
 
 * Open Sans font: https://fonts.google.com/specimen/Open+Sans
 
 * [QssStylesheetEditor](https://github.com/hustlei/QssStylesheetEditor) for make the app theme
 
 * Musical note use in the app icon: https://openclipart.org/detail/110599/musical-note-2-dennis-b-01r
-
-
```

### Comparing `pqmusic-1.2.1/PQMusic/OpenSans.ttf` & `pqmusic-1.3.0/PQMusic/OpenSans.ttf`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/__init__.py` & `pqmusic-1.3.0/PQMusic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,24 +41,23 @@
         QtWidgets.QMainWindow.__init__(self, *args, **kwargs)
         self.setupUi(self)
 
         self.isMWShow = True
         self.player = Player(self)
         self.plModel = QStandardItemModel()
         self.playlistView.setModel(self.plModel)
-        self.resize_event = False
+        self.layout().setSizeConstraint(QtWidgets.QLayout.SetFixedSize)
         self.setAcceptDrops(True)
         self.config = ConfigDialog.loadConf()
 
         # Hide the playlisy layout
         self.blockSignals(True)
         self.playListFrame.hide()
         self.adjustSize()
         self.blockSignals(False)
-        self.resize_event = True
 
         self.listAddButton.clicked.connect(self.addFiles)
         self.listClearButton.clicked.connect(self.clearPlaylist)
         self.listRemoveButton.clicked.connect(self.delTracks)
         self.playButton.clicked.connect(self.player.playPause)
         self.playlistButton.clicked.connect(self.showHidePlaylist)
         self.playlistView.doubleClicked.connect(self.changeTrack)
@@ -218,16 +217,16 @@
         scQuit.activated.connect(self.closeEvent)
 
         if 'savevolume' in self.config and self.config['savevolume']:
             volume = getSaveVolume()
             self.volumeSlider.setValue(volume)
 
     def addDir(self):
-        """ Opens the dialog to select a folder to add the supported files inside it,
-            as well as subdirectories.
+        """ Opens the dialog to select a folder to add the supported files
+            inside it, as well as subdirectories.
         """
         folder = QtWidgets.QFileDialog.getExistingDirectory(
             self,
             _translate('MainWindow', 'Select folder'),
             self.config['musicfolder'],
             QtWidgets.QFileDialog.ShowDirsOnly
         )
@@ -374,15 +373,19 @@
             event.ignore()
         else:
             delLockFile()
             if 'savevolume' in self.config and self.config['savevolume']:
                 saveVolume(self.volumeSlider.value())
 
             if 'saveplaylist' in self.config and self.config['saveplaylist']:
-                saveM3U(self, COVER_CACHE + '/playlist.m3u8', self.player.queueData)
+                saveM3U(
+                    self,
+                    COVER_CACHE + '/playlist.m3u8',
+                    self.player.queueData
+                )
 
             sysExit()
 
     def delTracks(self):
         """ Remove the selected tracks in the playlist """
         model = self.playlistView.selectionModel()
         indexes = model.selectedIndexes()
@@ -435,47 +438,33 @@
         for f in sorted(listdir(folder)):
             file = path.join(folder, f)
             if path.isdir(file):
                 self.scanDir(file)
             elif path.isfile(file):
                 self.player.addFile(file)
 
-    def resizeEvent(self, event):
-        """ This function is called when resize the window.
-            Args:
-                event : The resize event
-                    The QStandarItem selected
-        """
-        if self.resize_event:
-            if event.size().height() >= 320:
-                self.playListFrame.show()
-                self.playlistButton.setChecked(True)
-
-            else:
-                self.playListFrame.hide()
-                self.playlistButton.setChecked(False)
-
     def showHidePlaylist(self):
         """ Show/Hide the playlist frame """
-        self.resize_event = False
+        self.layout().setSizeConstraint(QtWidgets.QLayout.SetMinAndMaxSize)
 
         if self.playlistButton.isChecked():
             self.playListFrame.show()
         else:
             self.playListFrame.hide()
+            self.layout().setSizeConstraint(QtWidgets.QLayout.SetFixedSize)
 
         QTimer.singleShot(0, self.adjustSize)
-        self.resize_event = True
 
 
 def init(custom_theme=True, files=[]):
     LOCAL_DIR = path.dirname(path.realpath(__file__))
 
     app = QtWidgets.QApplication([])
     app.setQuitOnLastWindowClosed(False)
+    app.setDesktopFileName('pqmusic')
     defaultLocale = QLocale.system().name()
     if defaultLocale.startswith('es_'):
         defaultLocale = 'es'
 
     translator = QTranslator()
     translator.load(LOCAL_DIR + "/locales/" + defaultLocale + ".qm")
     app.installTranslator(translator)
```

### Comparing `pqmusic-1.2.1/PQMusic/__init__.py.bck` & `pqmusic-1.3.0/PQMusic/__init__.py.bck`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/config.py` & `pqmusic-1.3.0/PQMusic/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,22 +46,22 @@
             self.ui.notifyOnChange.setChecked(True)
 
         self.ui.minimizeToTray.setChecked(False)
         if self.config['mintosystray'] == 1:
             self.ui.minimizeToTray.setChecked(True)
 
         self.ui.cbDownCover.setChecked(False)
-        if 'sdowncover' in self.config and self.config['downcover'] == 1:
+        if 'downcover' in self.config and self.config['downcover'] == 1:
             self.ui.cbDownCover.setChecked(True)
 
         self.ui.cbSaveVolume.setChecked(False)
         if 'savevolume' in self.config and self.config['savevolume'] == 1:
             self.ui.cbSaveVolume.setChecked(True)
-            
-        self.ui.cbSaveVolume.setChecked(False)
+
+        self.ui.cbSavePlaylist.setChecked(False)
         if 'saveplaylist' in self.config and self.config['saveplaylist'] == 1:
             self.ui.cbSavePlaylist.setChecked(True)
 
         self.exec_()
 
     @staticmethod
     def loadConf():
@@ -111,15 +111,15 @@
         else:
             cfg.set('pqmusic', 'downcover', '0')
 
         if self.ui.cbSaveVolume.isChecked():
             cfg.set('pqmusic', 'savevolume', '1')
         else:
             cfg.set('pqmusic', 'savevolume', '0')
-            
+
         if self.ui.cbSavePlaylist.isChecked():
             cfg.set('pqmusic', 'saveplaylist', '1')
         else:
             cfg.set('pqmusic', 'saveplaylist', '0')
 
         with open(configfile, "w") as file:
             cfg.write(file)
```

### Comparing `pqmusic-1.2.1/PQMusic/covers.py` & `pqmusic-1.3.0/PQMusic/covers.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,41 +31,46 @@
 
     try:
         with request.urlopen(full_url) as response:
             rawData = response.read().decode('utf-8')
             data = json.loads(rawData)
             return data
     except error.HTTPError:
-        return False
+        return None
 
 
 class searchTrackInfo(QThread):
     result = pyqtSignal(QVariant)
 
-    def __init__(self, artist, release):
-        super().__init__()
+    def __init__(self, artist, release, parent):
+        super().__init__(parent)
         self.params = {
             'fmt': 'json',
-            'query': 'artist:"{}" AND release:"{}"'.format(artist, release)
+            'query': f'artist:"{artist}" AND release:"{release}"'
         }
 
         self.url = 'https://musicbrainz.org/ws/2/release/'
 
     def run(self):
-        data = getData(self.url, self.params)
-        if data:
-            self.result.emit(data)
+        try:
+            data = getData(self.url, self.params)
+            if data:
+                self.result.emit(data)
+        except Exception:
+            self.result.emit({})
+
+        self.result.emit({})
 
 
 class downCover(QThread):
     downloaded = pyqtSignal(QVariant)
 
     def __init__(self, parent, albumId, filename):
         super(downCover, self).__init__(parent)
-        self.url = 'https://coverartarchive.org/release/{}/front-250'.format(albumId)
+        self.url = f'https://coverartarchive.org/release/{albumId}/front-250'
         self.filename = filename
 
     def run(self):
         try:
             request.urlretrieve(self.url, self.filename, self.progress)
         except error.HTTPError:
             self.downloaded.emit(False)
```

### Comparing `pqmusic-1.2.1/PQMusic/icon.svg` & `pqmusic-1.3.0/PQMusic/icon.svg`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/images.qrc` & `pqmusic-1.3.0/PQMusic/images.qrc`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/locales/es.qm` & `pqmusic-1.3.0/PQMusic/locales/es.qm`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/minimal-player.spec` & `pqmusic-1.3.0/PQMusic/minimal-player.spec`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/no_cover.svg` & `pqmusic-1.3.0/PQMusic/no_cover.svg`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/player.py` & `pqmusic-1.3.0/PQMusic/player.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,17 @@
     QMediaContent,
     QMediaMetaData,
 )
 from PyQt5.QtCore import QUrl, QCoreApplication, QSize, Qt
 from PyQt5.QtGui import QIcon, QPixmap, QStandardItem
 from PyQt5 import QtWidgets
 from pathlib import Path
-from .utils import getMetaData, openM3U, saveM3U
+from .utils import getMetaData, openM3U, saveM3U, getTrackerTitle, notify
 from urllib.parse import urlparse
 from os import path, access, R_OK, mkdir, environ, listdir
-from .sys_notify import Notification, init
 from .covers import searchTrackInfo, downCover
 
 import magic
 import re
 
 _translate = QCoreApplication.translate
 LOCAL_DIR = path.dirname(path.realpath(__file__))
@@ -48,35 +47,39 @@
         self.player.setPlaylist(self.queueList)
         self.queueData = []
         self.position = 0
         self.prevPosition = -1
         self.volume = 100
         self.blockCoverSearch = False
 
-        init('pqmusic')
-
         self.player.mediaStatusChanged.connect(self.qmp_mediaStatusChanged)
         self.player.metaDataChanged.connect(self.metaDataChanged)
         self.player.positionChanged.connect(self.qmp_positionChanged)
         self.player.durationChanged.connect(self.durationChanged)
         self.queueList.currentIndexChanged.connect(self.playlistPosChanged)
 
     def addFile(self, file):
         """ Add a file to the playlist """
         if self.checkValidFile(file):
             self.queueList.addMedia(QMediaContent(QUrl.fromLocalFile(file)))
             tags = getMetaData(file)
+            trackerTitle = getTrackerTitle(file)
 
-            if tags['notags']:
+            if trackerTitle:
+                item = QStandardItem(trackerTitle)
+            elif tags['notags']:
                 item = QStandardItem(tags['notags'])
             else:
-                item = QStandardItem('{} - {}'.format(
-                    tags['artist'],
-                    tags['title']
-                ))
+                if tags['artist']:
+                    item = QStandardItem('{} - {}'.format(
+                        tags['artist'],
+                        tags['title']
+                    ))
+                else:
+                    item = QStandardItem(tags['title'])
 
             tags['file'] = file
 
             self.parent.plModel.appendRow(item)
             self.queueData.append(tags)
             self.parent.playButton.setEnabled(True)
             self.parent.repeatButton.setEnabled(True)
@@ -160,14 +163,26 @@
         if duration > 0:
             total_time = ms_to_time(duration)
             self.parent.timeSlider.setMaximum(duration)
             self.parent.timeSlider.setEnabled(True)
             self.currentTrackDuration = duration
             self.parent.totalTimeLabel.setText(total_time)
 
+        filepath = self.player.currentMedia().canonicalUrl().toString()
+        trackerTitle = getTrackerTitle(filepath)
+        if trackerTitle:
+            self.parent.titleLabel.setText(trackerTitle)
+            self.parent.artistLabel.setText(
+                _translate('MainWindow', 'Unknown')
+            )
+
+            self.parent.albumLabel.setText(
+                _translate('MainWindow', 'Unknown')
+            )
+
     def metaDataChanged(self):
         """ This function is called whenever the metadata changes,
             e.g. track changes or is received during a live stream.
         """
         self.parent.tray.setToolTip('')
         artist = None
         title = None
@@ -208,20 +223,24 @@
                 self.parent.artistLabel.setText(
                     _translate('MainWindow', 'Unknown')
                 )
 
             if self.player.metaData(QMediaMetaData.AlbumTitle):
                 album = self.player.metaData(QMediaMetaData.AlbumTitle)
                 self.parent.albumLabel.setText(album)
+            else:
+                self.parent.albumLabel.setText(
+                    _translate('MainWindow', 'Unknown')
+                )
 
             release = title
             if album:
                 release = album
 
-            downCoverFile = '{}/{}-{}.jpg'.format(COVER_CACHE, artist, release)
+            downCoverFile = f'{COVER_CACHE}/{artist}-{release}.jpg'
 
             if self.player.metaData(QMediaMetaData.CoverArtImage):
                 cover = self.player.metaData(QMediaMetaData.CoverArtImage)
                 cover = QPixmap.fromImage(cover)
                 scaledCover = cover.scaled(
                     QSize(128, 128),
                     Qt.KeepAspectRatio,
@@ -238,72 +257,72 @@
                 self.parent.labelCover.setPixmap(
                     cover.scaled(QSize(128, 128), Qt.KeepAspectRatio)
                 )
                 notifyIcon = downCoverFile
 
             else:
                 # Buscar caratula
+                name = Path(file).stem
+                name = re.escape(name)
                 coverRegex = re.compile(
-                    "(albumartsmall|cover|folder).(jpg|png)",
+                    f"({name}|albumartsmall|cover|folder).(jpg|png)",
                     re.IGNORECASE
                 )
 
                 for f in sorted(listdir(currentFolder)):
                     findCover = re.search(coverRegex, f)
                     if findCover:
                         coverFile = path.join(currentFolder, f)
                         cover = QPixmap(coverFile)
                         self.parent.labelCover.setPixmap(
                             cover.scaled(QSize(128, 128), Qt.KeepAspectRatio)
                         )
                         notifyIcon = coverFile
 
             def __getcover(data):
-                if len(data['releases']) > 0:
+                if 'releases' in data and len(data['releases']) > 0:
                     albumId = data['releases'][0]['id']
                     thread = downCover(
                         self.parent, albumId,
-                        '{}/{}-{}.jpg'.format(COVER_CACHE, artist, release)
+                        f'{COVER_CACHE}/{artist}-{release}.jpg'
                     )
                     thread.downloaded.connect(self.setDownCover)
                     thread.start()
 
             if (
                 not cover and
                 not self.blockCoverSearch and
                 not path.isfile(downCoverFile)
             ):
-                thread = searchTrackInfo(artist, release)
+                thread = searchTrackInfo(artist, release, self.parent)
                 thread.result.connect(__getcover)
                 thread.start()
-                self.blockCoverSearch = True
 
             if not cover:
                 cover = QPixmap(':/no_cover.svg')
                 self.parent.labelCover.setPixmap(
                     cover.scaled(QSize(128, 128), Qt.KeepAspectRatio)
                 )
 
         if artist:
-            trayTooltip = '{} - {}'.format(artist, title)
+            trayTooltip = f'{artist} - {title}'
         else:
             trayTooltip = title
 
         if trayTooltip:
             self.parent.setWindowTitle('PQMusic: ' + trayTooltip)
             self.parent.tray.setToolTip(trayTooltip)
 
             if self.parent.config['shownotify']:
-                n = Notification(
+                notify(
                     'PQMusic',
                     trayTooltip,
                     notifyIcon,
                     timeout=3000
                 )
-                n.show()
 
     def openPlaylist(self, file=None):
         """ Opens the dialog to select files to add """
         if not file:
             file, _ = QtWidgets.QFileDialog.getOpenFileName(
                 self.parent,
                 _translate('MainWindow', 'Select playlist to open'),
```

### Comparing `pqmusic-1.2.1/PQMusic/player.py.bck` & `pqmusic-1.3.0/PQMusic/player.py.bck`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/style.qss` & `pqmusic-1.3.0/PQMusic/style.qss`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/sys_notify.py` & `pqmusic-1.3.0/PQMusic/sys_notify.py.bck`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/ui/Ui_add_url_dialog.py` & `pqmusic-1.3.0/PQMusic/ui/Ui_add_url_dialog.py`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/ui/Ui_config.py` & `pqmusic-1.3.0/PQMusic/ui/Ui_config.py`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/ui/Ui_gui.py` & `pqmusic-1.3.0/PQMusic/ui/Ui_gui.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,65 @@
         MainWindow.setStyleSheet("")
         MainWindow.setLocale(QtCore.QLocale(QtCore.QLocale.English, QtCore.QLocale.UnitedStates))
         MainWindow.setToolButtonStyle(QtCore.Qt.ToolButtonFollowStyle)
         self.centralwidget = QtWidgets.QWidget(MainWindow)
         self.centralwidget.setObjectName("centralwidget")
         self.gridLayout = QtWidgets.QGridLayout(self.centralwidget)
         self.gridLayout.setObjectName("gridLayout")
+        self.playListFrame = QtWidgets.QFrame(self.centralwidget)
+        self.playListFrame.setFrameShape(QtWidgets.QFrame.StyledPanel)
+        self.playListFrame.setFrameShadow(QtWidgets.QFrame.Raised)
+        self.playListFrame.setObjectName("playListFrame")
+        self.gridLayout_2 = QtWidgets.QGridLayout(self.playListFrame)
+        self.gridLayout_2.setContentsMargins(0, 0, 0, 0)
+        self.gridLayout_2.setSpacing(0)
+        self.gridLayout_2.setObjectName("gridLayout_2")
+        self.verticalLayout = QtWidgets.QVBoxLayout()
+        self.verticalLayout.setObjectName("verticalLayout")
+        self.playlistView = QtWidgets.QListView(self.playListFrame)
+        self.playlistView.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
+        self.playlistView.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
+        self.playlistView.setObjectName("playlistView")
+        self.verticalLayout.addWidget(self.playlistView)
+        self.gridLayout_2.addLayout(self.verticalLayout, 0, 0, 1, 1)
+        self.playlistBtnLayout = QtWidgets.QHBoxLayout()
+        self.playlistBtnLayout.setObjectName("playlistBtnLayout")
+        self.listAddButton = QtWidgets.QPushButton(self.playListFrame)
+        self.listAddButton.setText("")
+        icon = QtGui.QIcon.fromTheme("list-add")
+        self.listAddButton.setIcon(icon)
+        self.listAddButton.setFlat(True)
+        self.listAddButton.setObjectName("listAddButton")
+        self.playlistBtnLayout.addWidget(self.listAddButton)
+        self.listRemoveButton = QtWidgets.QPushButton(self.playListFrame)
+        self.listRemoveButton.setText("")
+        icon = QtGui.QIcon.fromTheme("list-remove")
+        self.listRemoveButton.setIcon(icon)
+        self.listRemoveButton.setFlat(True)
+        self.listRemoveButton.setObjectName("listRemoveButton")
+        self.playlistBtnLayout.addWidget(self.listRemoveButton)
+        self.listClearButton = QtWidgets.QPushButton(self.playListFrame)
+        self.listClearButton.setText("")
+        icon = QtGui.QIcon.fromTheme("edit-clear-all")
+        self.listClearButton.setIcon(icon)
+        self.listClearButton.setFlat(True)
+        self.listClearButton.setObjectName("listClearButton")
+        self.playlistBtnLayout.addWidget(self.listClearButton)
+        self.savePlButton = QtWidgets.QPushButton(self.playListFrame)
+        self.savePlButton.setText("")
+        icon = QtGui.QIcon.fromTheme("document-export")
+        self.savePlButton.setIcon(icon)
+        self.savePlButton.setFlat(True)
+        self.savePlButton.setObjectName("savePlButton")
+        self.playlistBtnLayout.addWidget(self.savePlButton)
+        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.playlistBtnLayout.addItem(spacerItem)
+        self.gridLayout_2.addLayout(self.playlistBtnLayout, 1, 0, 1, 1)
+        self.gridLayout_2.setRowStretch(0, 1)
+        self.gridLayout.addWidget(self.playListFrame, 3, 0, 1, 2)
         self.optionsLayout = QtWidgets.QHBoxLayout()
         self.optionsLayout.setObjectName("optionsLayout")
         self.playlistButton = QtWidgets.QPushButton(self.centralwidget)
         self.playlistButton.setText("")
         icon = QtGui.QIcon.fromTheme("view-media-playlist")
         self.playlistButton.setIcon(icon)
         self.playlistButton.setCheckable(True)
@@ -67,18 +118,31 @@
         self.menuButton.setObjectName("menuButton")
         self.optionsLayout.addWidget(self.menuButton)
         self.iconVol = QtWidgets.QLabel(self.centralwidget)
         self.iconVol.setText("")
         self.iconVol.setObjectName("iconVol")
         self.optionsLayout.addWidget(self.iconVol)
         self.volumeSlider = QtWidgets.QSlider(self.centralwidget)
+        self.volumeSlider.setMinimumSize(QtCore.QSize(80, 0))
+        self.volumeSlider.setMaximumSize(QtCore.QSize(80, 16777215))
         self.volumeSlider.setOrientation(QtCore.Qt.Horizontal)
         self.volumeSlider.setObjectName("volumeSlider")
         self.optionsLayout.addWidget(self.volumeSlider)
+        spacerItem1 = QtWidgets.QSpacerItem(0, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
+        self.optionsLayout.addItem(spacerItem1)
         self.gridLayout.addLayout(self.optionsLayout, 2, 1, 1, 1)
+        self.labelCover = QtWidgets.QLabel(self.centralwidget)
+        self.labelCover.setMinimumSize(QtCore.QSize(0, 128))
+        self.labelCover.setMaximumSize(QtCore.QSize(128, 128))
+        self.labelCover.setText("")
+        self.labelCover.setPixmap(QtGui.QPixmap(":/icon.svg"))
+        self.labelCover.setScaledContents(True)
+        self.labelCover.setAlignment(QtCore.Qt.AlignCenter)
+        self.labelCover.setObjectName("labelCover")
+        self.gridLayout.addWidget(self.labelCover, 0, 0, 1, 1)
         self.playerLayout = QtWidgets.QHBoxLayout()
         self.playerLayout.setObjectName("playerLayout")
         self.queuePrevButton = QtWidgets.QPushButton(self.centralwidget)
         self.queuePrevButton.setEnabled(False)
         self.queuePrevButton.setText("")
         icon = QtGui.QIcon.fromTheme("media-skip-backward")
         self.queuePrevButton.setIcon(icon)
@@ -105,23 +169,14 @@
         self.queueNextButton.setText("")
         icon = QtGui.QIcon.fromTheme("media-skip-forward")
         self.queueNextButton.setIcon(icon)
         self.queueNextButton.setFlat(True)
         self.queueNextButton.setObjectName("queueNextButton")
         self.playerLayout.addWidget(self.queueNextButton)
         self.gridLayout.addLayout(self.playerLayout, 2, 0, 1, 1)
-        self.labelCover = QtWidgets.QLabel(self.centralwidget)
-        self.labelCover.setMinimumSize(QtCore.QSize(0, 128))
-        self.labelCover.setMaximumSize(QtCore.QSize(128, 128))
-        self.labelCover.setText("")
-        self.labelCover.setPixmap(QtGui.QPixmap(":/icon.svg"))
-        self.labelCover.setScaledContents(True)
-        self.labelCover.setAlignment(QtCore.Qt.AlignCenter)
-        self.labelCover.setObjectName("labelCover")
-        self.gridLayout.addWidget(self.labelCover, 0, 0, 1, 1)
         self.infoWidget = QtWidgets.QWidget(self.centralwidget)
         self.infoWidget.setMaximumSize(QtCore.QSize(340, 16777215))
         self.infoWidget.setObjectName("infoWidget")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout(self.infoWidget)
         self.verticalLayout_2.setContentsMargins(0, 0, 0, 0)
         self.verticalLayout_2.setSpacing(0)
         self.verticalLayout_2.setObjectName("verticalLayout_2")
@@ -157,67 +212,15 @@
         self.totalTimeLabel = QtWidgets.QLabel(self.infoWidget)
         self.totalTimeLabel.setText("0:00:00")
         self.totalTimeLabel.setAlignment(QtCore.Qt.AlignCenter)
         self.totalTimeLabel.setObjectName("totalTimeLabel")
         self.timeLayout.addWidget(self.totalTimeLabel)
         self.verticalLayout_2.addLayout(self.timeLayout)
         self.gridLayout.addWidget(self.infoWidget, 0, 1, 1, 1)
-        self.playListFrame = QtWidgets.QFrame(self.centralwidget)
-        self.playListFrame.setFrameShape(QtWidgets.QFrame.StyledPanel)
-        self.playListFrame.setFrameShadow(QtWidgets.QFrame.Raised)
-        self.playListFrame.setObjectName("playListFrame")
-        self.gridLayout_2 = QtWidgets.QGridLayout(self.playListFrame)
-        self.gridLayout_2.setContentsMargins(0, 0, 0, 0)
-        self.gridLayout_2.setSpacing(0)
-        self.gridLayout_2.setObjectName("gridLayout_2")
-        self.verticalLayout = QtWidgets.QVBoxLayout()
-        self.verticalLayout.setObjectName("verticalLayout")
-        self.playlistView = QtWidgets.QListView(self.playListFrame)
-        self.playlistView.setEditTriggers(QtWidgets.QAbstractItemView.NoEditTriggers)
-        self.playlistView.setSelectionMode(QtWidgets.QAbstractItemView.MultiSelection)
-        self.playlistView.setObjectName("playlistView")
-        self.verticalLayout.addWidget(self.playlistView)
-        self.gridLayout_2.addLayout(self.verticalLayout, 0, 0, 1, 1)
-        self.playlistBtnLayout = QtWidgets.QHBoxLayout()
-        self.playlistBtnLayout.setObjectName("playlistBtnLayout")
-        self.listAddButton = QtWidgets.QPushButton(self.playListFrame)
-        self.listAddButton.setText("")
-        icon = QtGui.QIcon.fromTheme("list-add")
-        self.listAddButton.setIcon(icon)
-        self.listAddButton.setFlat(True)
-        self.listAddButton.setObjectName("listAddButton")
-        self.playlistBtnLayout.addWidget(self.listAddButton)
-        self.listRemoveButton = QtWidgets.QPushButton(self.playListFrame)
-        self.listRemoveButton.setText("")
-        icon = QtGui.QIcon.fromTheme("list-remove")
-        self.listRemoveButton.setIcon(icon)
-        self.listRemoveButton.setFlat(True)
-        self.listRemoveButton.setObjectName("listRemoveButton")
-        self.playlistBtnLayout.addWidget(self.listRemoveButton)
-        self.listClearButton = QtWidgets.QPushButton(self.playListFrame)
-        self.listClearButton.setText("")
-        icon = QtGui.QIcon.fromTheme("edit-clear-all")
-        self.listClearButton.setIcon(icon)
-        self.listClearButton.setFlat(True)
-        self.listClearButton.setObjectName("listClearButton")
-        self.playlistBtnLayout.addWidget(self.listClearButton)
-        self.savePlButton = QtWidgets.QPushButton(self.playListFrame)
-        self.savePlButton.setText("")
-        icon = QtGui.QIcon.fromTheme("document-export")
-        self.savePlButton.setIcon(icon)
-        self.savePlButton.setFlat(True)
-        self.savePlButton.setObjectName("savePlButton")
-        self.playlistBtnLayout.addWidget(self.savePlButton)
-        spacerItem = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Expanding, QtWidgets.QSizePolicy.Minimum)
-        self.playlistBtnLayout.addItem(spacerItem)
-        self.gridLayout_2.addLayout(self.playlistBtnLayout, 1, 0, 1, 1)
-        self.gridLayout_2.setRowStretch(0, 1)
-        self.gridLayout.addWidget(self.playListFrame, 3, 0, 1, 2)
-        spacerItem1 = QtWidgets.QSpacerItem(20, 0, QtWidgets.QSizePolicy.Minimum, QtWidgets.QSizePolicy.Expanding)
-        self.gridLayout.addItem(spacerItem1, 4, 0, 1, 1)
+        self.gridLayout.setRowStretch(3, 1)
         MainWindow.setCentralWidget(self.centralwidget)
 
         self.retranslateUi(MainWindow)
         QtCore.QMetaObject.connectSlotsByName(MainWindow)
 
     def retranslateUi(self, MainWindow):
         _translate = QtCore.QCoreApplication.translate
```

### Comparing `pqmusic-1.2.1/PQMusic/ui/images_rc.py` & `pqmusic-1.3.0/PQMusic/ui/images_rc.py`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/PQMusic/ui/open_url_dialog.py` & `pqmusic-1.3.0/PQMusic/ui/open_url_dialog.py`

 * *Files identical despite different names*

### Comparing `pqmusic-1.2.1/README.md` & `pqmusic-1.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -9,43 +9,41 @@
 
 [https://github.com/son-link/PQMusic](https://github.com/son-link/PQMusic)
 
 ![PQMusic screenshoot](screenshoot.jpg)
 
 PQMusic is a minimalist and easy to use audio player for download and use.
 
-You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format.
+You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format. Also you can play some music trackers files (.it, .mod, .s3m and .xm)
 
 Adding files from Open with on your file manager
 ![Add files from Open with on your file manager](file-manager-menu.png)
 
 Drag and drop files to PQMusic's window:
 
 <video controls style="max-width: 720px">
   <source src="pqmusic-drag-drop.mp4" />
 </video>
 
 Only available for Linux.
 
 Licensed under GNU/GPL3 or higher.
 
-**Note**: this project is still under development, so some features are not yet available or complete.
-
 ## Install
 
 ### From source code:
 
 * Clone the repo, download the zip under Code -> Download ZIP or download the last release.
 * Open a terminal and go to the project folder.
 * Install the dependencies:
-  * **From PIP** (with administration permissions): `pip install -r requirements.txt`
+  * **From PIP**: `pip install -r requirements.txt` *use the --user parameter if you want to install the dependencies at your user level*
   * **Debian/Ubuntu/Mint/MX Linux**:
-    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic dbus-python`
+    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic python3-requests`
   * **Arch Linux/Manjaro**:
-    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic dbus-python`
+    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic python-requests`
 
   * Copy the icon and desktop file:
     * All users:
       * `install -m 644 bin/io.sonlink.pqmusic.desktop /usr/share/applications`
   	  * `install -m 644 bin/io.sonlink.pqmusic.svg /usr/share/icons/pqmusic.svg`
   	* Current user:
   	  * `cp bin/io.sonlink.pqmusic.desktop ~/.local/share/applications`
@@ -53,15 +51,15 @@
 
 ### From Pypi:
 
 `pip install PQMusic`
 
 ### AUR:
 
-If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install yhe official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
+If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install the official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
 
 For example: `yay -S pqmusic`
 
 ### Executables:
 
 You can download a **AppImage** for **GNU/Linux** on [releases page](https://github.com/son-link/PQMusic/releases)
```

### Comparing `pqmusic-1.2.1/pqmusic.egg-info/PKG-INFO` & `pqmusic-1.3.0/pqmusic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: pqmusic
-Version: 1.2.1
+Version: 1.3.0
 Summary: A minimal music player.
 Home-page: https://github.com/son-link/PQMusic
-Download-URL: https://github.com/son-link/PQMusic/archive/refs/tags/v.1.1.1.tar.gz
+Download-URL: https://github.com/son-link/PQMusic/archive/refs/tags/v.1.3.0.tar.gz
 Author: Alfonso Saavedra 'Son Link'
 Author-email: sonlink.dourden@gmail.com
 License: GPL 3.0
 Keywords: music,audio,player
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: X11 Applications :: Qt
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # PQMusic
 
@@ -38,43 +38,41 @@
 
 [https://github.com/son-link/PQMusic](https://github.com/son-link/PQMusic)
 
 ![PQMusic screenshoot](screenshoot.jpg)
 
 PQMusic is a minimalist and easy to use audio player for download and use.
 
-You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format.
+You can play your local files, from a direct url or streaming (for example a online radio) and import/export playlists on M3U format. Also you can play some music trackers files (.it, .mod, .s3m and .xm)
 
 Adding files from Open with on your file manager
 ![Add files from Open with on your file manager](file-manager-menu.png)
 
 Drag and drop files to PQMusic's window:
 
 <video controls style="max-width: 720px">
   <source src="pqmusic-drag-drop.mp4" />
 </video>
 
 Only available for Linux.
 
 Licensed under GNU/GPL3 or higher.
 
-**Note**: this project is still under development, so some features are not yet available or complete.
-
 ## Install
 
 ### From source code:
 
 * Clone the repo, download the zip under Code -> Download ZIP or download the last release.
 * Open a terminal and go to the project folder.
 * Install the dependencies:
-  * **From PIP** (with administration permissions): `pip install -r requirements.txt`
+  * **From PIP**: `pip install -r requirements.txt` *use the --user parameter if you want to install the dependencies at your user level*
   * **Debian/Ubuntu/Mint/MX Linux**:
-    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic dbus-python`
+    * apt: `apt install python3-pyqt5 python3-pyqt5.qtmultimedia libqt5multimedia5 libqt5multimedia5-plugins qtgstreamer-plugins-qt5 python3-mutagen python3-magic python3-requests`
   * **Arch Linux/Manjaro**:
-    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic dbus-python`
+    * pacman: `python-pip python-mutagen python-pyqt5 qt5-multimedia python-mutagen python-magic python-requests`
 
   * Copy the icon and desktop file:
     * All users:
       * `install -m 644 bin/io.sonlink.pqmusic.desktop /usr/share/applications`
   	  * `install -m 644 bin/io.sonlink.pqmusic.svg /usr/share/icons/pqmusic.svg`
   	* Current user:
   	  * `cp bin/io.sonlink.pqmusic.desktop ~/.local/share/applications`
@@ -82,15 +80,15 @@
 
 ### From Pypi:
 
 `pip install PQMusic`
 
 ### AUR:
 
-If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install yhe official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
+If you use Arch Linux, Manjaro, or other Arch Linux base distributions, you can install the official package from [AUR](https://aur.archlinux.org/packages/pqmusic)
 
 For example: `yay -S pqmusic`
 
 ### Executables:
 
 You can download a **AppImage** for **GNU/Linux** on [releases page](https://github.com/son-link/PQMusic/releases)
 
@@ -113,9 +111,7 @@
 * Lüv icons theme: https://github.com/Nitrux/luv-icon-theme
 
 * Open Sans font: https://fonts.google.com/specimen/Open+Sans
 
 * [QssStylesheetEditor](https://github.com/hustlei/QssStylesheetEditor) for make the app theme
 
 * Musical note use in the app icon: https://openclipart.org/detail/110599/musical-note-2-dennis-b-01r
-
-
```

### Comparing `pqmusic-1.2.1/setup.py` & `pqmusic-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="pqmusic",
-    version="1.2.1",
+    version="1.3.0",
     description="A minimal music player.",
     author="Alfonso Saavedra 'Son Link'",
     author_email='sonlink.dourden@gmail.com',
     license="GPL 3.0",
     url="https://github.com/son-link/PQMusic",
     scripts=['bin/pqmusic'],
     packages=['PQMusic'],
@@ -14,24 +14,27 @@
     package_data={'PQMusic': ['*', 'locales/*.qm', 'ui/*.py', 'LICENSE']},
     include_package_data=True,
     exclude_package_data={
         '/': [
             'build-appimage.sh',
             'build/',
             'dist/',
-            'icons/luv-icon-theme'
+            'icons/luv-icon-theme',
+            'packages/'
+            'icons/'
         ]
     },
-    download_url='https://github.com/son-link/PQMusic/archive/refs/tags/v.1.1.1.tar.gz',
+    download_url='https://github.com/son-link/PQMusic/archive/refs/tags/v.1.3.0.tar.gz',
     keywords=['music', 'audio', 'player'],
     install_requires=[
         'pyqt5',
         'mutagen',
         'python-magic',
-        'psutil'
+        'psutil',
+        'requests'
     ],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: X11 Applications :: Qt',
         'Topic :: Multimedia :: Sound/Audio',
         'Topic :: Multimedia :: Sound/Audio :: Players',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
@@ -39,11 +42,12 @@
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Intended Audience :: End Users/Desktop',
         'Operating System :: POSIX :: Linux'
     ],
 )
```

