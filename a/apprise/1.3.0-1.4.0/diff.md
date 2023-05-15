# Comparing `tmp/apprise-1.3.0.tar.gz` & `tmp/apprise-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apprise-1.3.0.tar", last modified: Wed Feb 22 22:31:02 2023, max compression
+gzip compressed data, was "apprise-1.4.0.tar", last modified: Mon May 15 20:33:07 2023, max compression
```

## Comparing `apprise-1.3.0.tar` & `apprise-1.4.0.tar`

### file list

```diff
@@ -1,318 +1,318 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.336393 apprise-1.3.0/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      712 2023-02-22 22:17:54.000000 apprise-1.3.0/KEYWORDS
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1530 2023-02-22 22:17:57.000000 apprise-1.3.0/LICENSE
--rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2022-12-18 21:46:05.000000 apprise-1.3.0/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40443 2023-02-22 22:31:02.337393 apprise-1.3.0/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38401 2023-02-22 22:17:54.000000 apprise-1.3.0/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.254393 apprise-1.3.0/apprise/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    30462 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/Apprise.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2022-12-19 22:58:15.000000 apprise-1.3.0/apprise/Apprise.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11489 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/AppriseAsset.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/AppriseAsset.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12778 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/AppriseAttachment.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2022-12-19 22:58:15.000000 apprise-1.3.0/apprise/AppriseAttachment.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17116 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/AppriseConfig.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2022-12-19 22:58:15.000000 apprise-1.3.0/apprise/AppriseConfig.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7216 2023-02-17 23:22:02.000000 apprise-1.3.0/apprise/AppriseLocale.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25067 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/URLBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/URLBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3573 2023-02-22 22:24:46.000000 apprise-1.3.0/apprise/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.256393 apprise-1.3.0/apprise/assets/
--rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/assets/NotifyXML-1.0.xsd
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/assets/NotifyXML-1.1.xsd
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.247393 apprise-1.3.0/apprise/assets/themes/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.268393 apprise-1.3.0/apprise/assets/themes/default/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-failure-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16135 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-failure-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    41931 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-failure-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2437 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-failure-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7600 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-failure-72x72.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-info-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16671 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-info-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    43331 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-info-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2485 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-info-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7875 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-info-72x72.png
--rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-logo.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-success-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    17446 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-success-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    48729 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-success-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2471 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-success-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7858 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-success-72x72.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-warning-128x128.ico
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    16784 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-warning-128x128.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    43708 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-warning-256x256.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2472 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-warning-32x32.png
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7913 2019-12-22 13:31:28.000000 apprise-1.3.0/apprise/assets/themes/default/apprise-warning-72x72.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.270393 apprise-1.3.0/apprise/attachment/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13764 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/attachment/AttachBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2022-12-19 22:58:15.000000 apprise-1.3.0/apprise/attachment/AttachBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4970 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/attachment/AttachFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12200 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/attachment/AttachHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4534 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/attachment/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18616 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2022-12-19 22:58:15.000000 apprise-1.3.0/apprise/common.pyi
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.271393 apprise-1.3.0/apprise/config/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    45093 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/config/ConfigBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/config/ConfigBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6343 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/config/ConfigFile.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9662 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/config/ConfigHTTP.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3034 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/config/ConfigMemory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4116 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/config/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6402 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/conversion.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.271393 apprise-1.3.0/apprise/decorators/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9106 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/decorators/CustomNotifyPlugin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1692 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/decorators/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5316 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/decorators/notify.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.271393 apprise-1.3.0/apprise/i18n/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)        0 2019-10-13 18:35:45.000000 apprise-1.3.0/apprise/i18n/__init__.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.248393 apprise-1.3.0/apprise/i18n/en/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.271393 apprise-1.3.0/apprise/i18n/en/LC_MESSAGES/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      455 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise/i18n/en/LC_MESSAGES/apprise.mo
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7126 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/logger.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.285393 apprise-1.3.0/apprise/plugins/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13176 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyAppriseAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15743 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyBark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20079 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyBase.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/plugins/NotifyBase.pyi
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12394 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyBoxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15543 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyBulkSMS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10994 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyClickSend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14980 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyD7Networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14662 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyDBus.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13389 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyDapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11875 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyDingTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20621 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyDiscord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38013 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyEmail.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24244 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyEmby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11703 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyEnigma2.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.286393 apprise-1.3.0/apprise/plugins/NotifyFCM/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21721 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFCM/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4797 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFCM/color.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1923 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFCM/common.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11327 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFCM/oauth.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8368 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFCM/priority.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7177 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFaast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12713 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyFlock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16109 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyForm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14213 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9342 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12827 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGoogleChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10786 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14228 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGrowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3846 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyGuilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10944 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyHomeAssistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13480 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyIFTTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13249 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyJSON.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13663 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyJoin.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12672 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyKavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8419 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyKumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    37724 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyLametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10699 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyLine.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19480 2023-02-19 01:26:26.000000 apprise-1.3.0/apprise/plugins/NotifyMQTT.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11632 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMSG91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23181 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMSTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8642 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMacOSX.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24935 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    34986 2023-02-22 22:17:54.000000 apprise-1.3.0/apprise/plugins/NotifyMastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    43534 2023-02-19 01:26:26.000000 apprise-1.3.0/apprise/plugins/NotifyMatrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12926 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12252 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyMessageBird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9804 2023-02-22 22:17:54.000000 apprise-1.3.0/apprise/plugins/NotifyMisskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12004 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyNextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9749 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyNextcloudTalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13186 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyNotica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12240 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyNotifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28156 2023-02-22 22:17:54.000000 apprise-1.3.0/apprise/plugins/NotifyNtfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25109 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyOffice365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17633 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyOneSignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20313 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyOpsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    18075 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPagerDuty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14054 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyPagerTree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10570 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyParsePlatform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10322 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPopcornNotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyProwl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15290 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPushBullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    26723 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPushSafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12255 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9157 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyPushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    21227 2023-02-12 19:45:58.000000 apprise-1.3.0/apprise/plugins/NotifyPushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25602 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyReddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24591 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyRocketChat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11992 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyRyver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    33289 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySES.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23059 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySMSEagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19385 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySMTP2Go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24094 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySNS.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16267 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySendGrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5985 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyServerChan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16404 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySignalAPI.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11101 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySimplePush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16817 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40750 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySlack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    27462 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySparkPost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13423 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySpontit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16254 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyStreamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15465 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifySyslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7458 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyTechulusPush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    31345 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyTelegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15980 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyTwilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28808 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyTwist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    30245 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyTwitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12567 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyVoipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13435 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyVonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9369 2023-02-12 19:45:58.000000 apprise-1.3.0/apprise/plugins/NotifyWebexTeams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8849 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyWindows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12301 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyXBMC.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15156 2023-02-17 22:24:25.000000 apprise-1.3.0/apprise/plugins/NotifyXML.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13777 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/NotifyZulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    20913 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/plugins/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2022-12-18 17:34:53.000000 apprise-1.3.0/apprise/py.typed
--rw-r--r--   0 l2g       (1000) l2g       (1000)    57150 2023-02-10 17:06:11.000000 apprise-1.3.0/apprise/utils.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.255393 apprise-1.3.0/apprise.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)    40443 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9213 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       46 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-02-22 22:31:02.000000 apprise-1.3.0/apprise.egg-info/top_level.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2022-12-19 22:58:15.000000 apprise-1.3.0/dev-requirements.txt
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.286393 apprise-1.3.0/packaging/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2022-12-19 22:58:15.000000 apprise-1.3.0/packaging/README.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.286393 apprise-1.3.0/packaging/man/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8306 2023-02-17 23:21:59.000000 apprise-1.3.0/packaging/man/apprise.1
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7663 2022-12-19 22:58:15.000000 apprise-1.3.0/packaging/man/apprise.md
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.288393 apprise-1.3.0/packaging/redhat/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1554 2022-12-19 22:58:15.000000 apprise-1.3.0/packaging/redhat/apprise-click67-support.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      524 2022-12-19 22:58:15.000000 apprise-1.3.0/packaging/redhat/apprise-no-macosx-testing.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)      837 2022-12-19 22:58:15.000000 apprise-1.3.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12395 2023-02-22 22:27:19.000000 apprise-1.3.0/packaging/redhat/python-apprise.spec
--rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2022-12-19 22:58:15.000000 apprise-1.3.0/requirements.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)      842 2023-02-22 22:31:02.338393 apprise-1.3.0/setup.cfg
--rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4542 2023-02-22 22:22:12.000000 apprise-1.3.0/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.329393 apprise-1.3.0/test/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2159 2023-02-10 17:06:11.000000 apprise-1.3.0/test/conftest.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.330393 apprise-1.3.0/test/helpers/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1823 2023-02-17 22:24:25.000000 apprise-1.3.0/test/helpers/__init__.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-02-17 22:24:25.000000 apprise-1.3.0/test/helpers/asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2692 2023-02-12 22:31:02.000000 apprise-1.3.0/test/helpers/module.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19579 2023-02-17 22:24:25.000000 apprise-1.3.0/test/helpers/rest.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    65027 2023-02-17 23:22:02.000000 apprise-1.3.0/test/test_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12791 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_apprise_attachments.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    41114 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_apprise_config.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    97294 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_apprise_utils.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3850 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_asyncio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3629 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_attach_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8696 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_attach_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16131 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_attach_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    38417 2023-02-17 23:22:02.000000 apprise-1.3.0/test/test_cli.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    32106 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_config_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4317 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_config_file.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10987 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_config_http.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2563 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_config_memory.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5204 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_conversion.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15782 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_decorator_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7800 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_escapes.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6828 2023-02-17 23:22:02.000000 apprise-1.3.0/test/test_locale.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14566 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_logger.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13351 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_notify_base.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6580 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_apprise_api.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5479 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_bark.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6132 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_boxcar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7183 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_bulksms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3563 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_clicksend.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15388 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_plugin_custom_form.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9189 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_plugin_custom_json.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9718 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_plugin_custom_xml.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7691 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_d7networks.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7367 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_dapnet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4185 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_dingtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16910 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_discord.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    53501 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_email.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14726 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_emby.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6293 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_enigma2.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3183 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_faast.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    31528 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_fcm.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6513 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_flock.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9429 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_gitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17909 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_glib.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12515 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_gnome.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6526 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_google_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6620 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_gotify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12895 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_growl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6775 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_guilded.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5438 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_homeassistant.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6966 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_ifttt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7653 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_join.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4431 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_kavenegar.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4268 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_kumulos.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_lametric.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3560 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_line.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7906 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_macosx.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14756 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_mailgun.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25170 2023-02-22 22:17:54.000000 apprise-1.3.0/test/test_plugin_mastodon.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    28712 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_matrix.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5145 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_mattermost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4780 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_messagebird.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4018 2023-02-22 22:17:54.000000 apprise-1.3.0/test/test_plugin_misskey.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14286 2023-02-19 01:26:26.000000 apprise-1.3.0/test/test_plugin_mqtt.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5279 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_msg91.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    24031 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_msteams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5641 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_nextcloud.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5367 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_nextcloudtalk.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5284 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_notica.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4581 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_notifico.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    19775 2023-02-22 22:17:54.000000 apprise-1.3.0/test/test_plugin_ntfy.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    12600 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_office365.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4841 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_onesignal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7316 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_opsgenie.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5148 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pagerduty.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5076 2023-02-17 22:24:25.000000 apprise-1.3.0/test/test_plugin_pagertree.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3955 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_parse_platform.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3824 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_popcorn_notify.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6837 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_prowl.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13285 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pushbullet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7441 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pushed.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3986 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pushjet.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    15365 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pushover.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9248 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_pushsafer.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14541 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_reddit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    11403 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_rocket_chat.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5272 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_ryver.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5702 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_sendgrid.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2915 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_serverchan.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14848 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_ses.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13560 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_signal.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5900 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_simplepush.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6451 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_sinch.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    23258 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_slack.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    25491 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_smseagle.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8848 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_smtp2go.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14499 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_sns.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    14266 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_sparkpost.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4848 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_spontit.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     5241 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_streamlabs.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     9643 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_syslog.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3266 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_techululs_push.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    34598 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_telegram.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8458 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_twilio.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    16971 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_twist.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    35809 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_twitter.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7789 2023-02-12 18:36:59.000000 apprise-1.3.0/test/test_plugin_voipms.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     8123 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_vonage.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4175 2023-02-12 19:45:58.000000 apprise-1.3.0/test/test_plugin_webex_teams.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    10991 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_windows.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     6700 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_xbmc_kodi.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)     4960 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_plugin_zulip.py
--rw-r--r--   0 l2g       (1000) l2g       (1000)    13376 2023-02-10 17:06:11.000000 apprise-1.3.0/test/test_rest_plugins.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.334393 apprise-1.3.0/test/var/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2022-12-18 21:46:05.000000 apprise-1.3.0/test/var/01_test_example.html
--rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2022-12-19 22:58:15.000000 apprise-1.3.0/test/var/apprise-archive.zip
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    76646 2019-12-22 13:31:28.000000 apprise-1.3.0/test/var/apprise-test.gif
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    73667 2019-12-22 13:31:28.000000 apprise-1.3.0/test/var/apprise-test.jpeg
--rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2022-12-18 21:46:05.000000 apprise-1.3.0/test/var/apprise-test.mp4
--rw-rw-r--   0 l2g       (1000) l2g       (1000)   248280 2019-12-22 13:31:28.000000 apprise-1.3.0/test/var/apprise-test.png
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-02-22 22:31:02.336393 apprise-1.3.0/test/var/fcm/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2022-12-18 17:34:53.000000 apprise-1.3.0/test/var/fcm/service_account-bad-type.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2022-12-18 17:34:53.000000 apprise-1.3.0/test/var/fcm/service_account.json
--rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2022-12-18 17:34:53.000000 apprise-1.3.0/win-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.301585 apprise-1.4.0/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      712 2023-05-13 16:20:00.000000 apprise-1.4.0/KEYWORDS
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1530 2023-05-12 22:30:02.000000 apprise-1.4.0/LICENSE
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      237 2022-12-18 21:46:05.000000 apprise-1.4.0/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    40904 2023-05-15 20:33:07.302585 apprise-1.4.0/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38862 2023-05-13 16:20:00.000000 apprise-1.4.0/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.208585 apprise-1.4.0/apprise/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    31245 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/Apprise.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2203 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/Apprise.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11489 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseAsset.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      979 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/AppriseAsset.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12778 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseAttachment.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1145 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/AppriseAttachment.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17116 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseConfig.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1568 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/AppriseConfig.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7216 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/AppriseLocale.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25284 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/URLBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      520 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/URLBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3573 2023-05-15 20:31:40.000000 apprise-1.4.0/apprise/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.210585 apprise-1.4.0/apprise/assets/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      986 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/NotifyXML-1.0.xsd
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1758 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/NotifyXML-1.1.xsd
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.201585 apprise-1.4.0/apprise/assets/themes/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.225585 apprise-1.4.0/apprise/assets/themes/default/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.ico
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    16135 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    41931 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-256x256.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2437 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-32x32.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7600 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-failure-72x72.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.ico
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    16671 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    43331 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-256x256.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2485 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-32x32.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7875 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-info-72x72.png
+-rw-r--r--   0 l2g       (1000) l2g       (1000)   160907 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-logo.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.ico
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    17446 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    48729 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-256x256.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2471 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-32x32.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7858 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-success-72x72.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    67646 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.ico
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    16784 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    43708 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-256x256.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2472 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-32x32.png
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7913 2019-12-22 13:31:28.000000 apprise-1.4.0/apprise/assets/themes/default/apprise-warning-72x72.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.226585 apprise-1.4.0/apprise/attachment/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13764 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      961 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/attachment/AttachBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4970 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12200 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/AttachHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4534 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/attachment/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19701 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7285 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      447 2022-12-19 22:58:15.000000 apprise-1.4.0/apprise/common.pyi
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.228585 apprise-1.4.0/apprise/config/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    45093 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       54 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/config/ConfigBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6343 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigFile.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9662 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigHTTP.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3034 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/ConfigMemory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4116 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/config/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6402 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/conversion.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/decorators/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9106 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/CustomNotifyPlugin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1692 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5316 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/decorators/notify.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/i18n/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)        0 2019-10-13 18:35:45.000000 apprise-1.4.0/apprise/i18n/__init__.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.202585 apprise-1.4.0/apprise/i18n/en/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.229585 apprise-1.4.0/apprise/i18n/en/LC_MESSAGES/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      455 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise/i18n/en/LC_MESSAGES/apprise.mo
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7126 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/logger.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.245585 apprise-1.4.0/apprise/plugins/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16863 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyAppriseAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15891 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20079 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyBase.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       21 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/plugins/NotifyBase.pyi
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12639 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBoxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16118 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyBulkSMS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11434 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyClickSend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15218 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyD7Networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14662 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyDBus.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13829 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyDapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12076 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyDingTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20677 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyDiscord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38214 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyEmail.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24244 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyEmby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11703 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyEnigma2.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.245585 apprise-1.4.0/apprise/plugins/NotifyFCM/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21874 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4797 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/color.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1923 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/common.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11327 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/oauth.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8368 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFCM/priority.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7177 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyFaast.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12914 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyFlock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18025 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyForm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14366 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyGitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9342 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12827 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGoogleChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10786 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14228 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGrowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3846 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyGuilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10944 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyHomeAssistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13632 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyIFTTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15331 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyJSON.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13816 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyJoin.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12825 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyKavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8419 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyKumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    37724 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyLametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10852 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyLine.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19632 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMQTT.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11785 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMSG91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23181 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMSTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8642 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMacOSX.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25396 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35187 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    43733 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMatrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12926 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12453 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyMessageBird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9804 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyMisskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12157 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9902 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNextcloudTalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13186 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyNotica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12240 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyNotifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    28308 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyNtfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25262 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOffice365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18328 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOneSignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20720 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyOpsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    18075 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPagerDuty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14054 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPagerTree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10570 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyParsePlatform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10762 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPopcornNotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyProwl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15443 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushBullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    26876 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushSafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12475 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9157 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyPushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    21380 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyPushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25758 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyReddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24829 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyRocketChat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11992 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyRyver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    33490 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySES.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24221 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySMSEagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19847 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySMTP2Go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24264 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySNS.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16420 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySendGrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5985 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyServerChan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16844 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySignalAPI.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11101 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifySimplePush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17018 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41877 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySlack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    27924 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySparkPost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13624 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifySpontit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16254 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyStreamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15465 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifySyslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7458 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyTechulusPush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    32361 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTelegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16181 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    28986 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    30048 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyTwitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12768 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyVoipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13636 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyVonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9369 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyWebexTeams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8846 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyWindows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12301 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/NotifyXBMC.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17127 2023-05-15 20:30:07.000000 apprise-1.4.0/apprise/plugins/NotifyXML.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13930 2023-05-13 02:23:07.000000 apprise-1.4.0/apprise/plugins/NotifyZulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20913 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/plugins/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        0 2022-12-18 17:34:53.000000 apprise-1.4.0/apprise/py.typed
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    57545 2023-05-12 22:30:02.000000 apprise-1.4.0/apprise/utils.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.209585 apprise-1.4.0/apprise.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    40904 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9213 2023-05-15 20:33:07.000000 apprise-1.4.0/apprise.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       46 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      101 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2023-05-15 20:33:06.000000 apprise-1.4.0/apprise.egg-info/top_level.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       65 2022-12-19 22:58:15.000000 apprise-1.4.0/dev-requirements.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.246585 apprise-1.4.0/packaging/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1281 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/README.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.246585 apprise-1.4.0/packaging/man/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8306 2023-02-17 23:21:59.000000 apprise-1.4.0/packaging/man/apprise.1
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7785 2023-05-13 02:23:07.000000 apprise-1.4.0/packaging/man/apprise.md
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.248585 apprise-1.4.0/packaging/redhat/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1554 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-click67-support.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      524 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-no-macosx-testing.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      837 2022-12-19 22:58:15.000000 apprise-1.4.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12476 2023-05-15 20:32:18.000000 apprise-1.4.0/packaging/redhat/python-apprise.spec
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      164 2022-12-19 22:58:15.000000 apprise-1.4.0/requirements.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      842 2023-05-15 20:33:07.302585 apprise-1.4.0/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     4542 2023-05-15 20:31:30.000000 apprise-1.4.0/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.294585 apprise-1.4.0/test/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2159 2023-05-12 22:30:02.000000 apprise-1.4.0/test/conftest.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.295585 apprise-1.4.0/test/helpers/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1823 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/__init__.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1668 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2692 2023-05-12 22:30:02.000000 apprise-1.4.0/test/helpers/module.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    20392 2023-05-13 02:23:07.000000 apprise-1.4.0/test/helpers/rest.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    65226 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12791 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_attachments.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    41102 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_config.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    98018 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_apprise_utils.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3850 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_asyncio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3629 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8696 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16131 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_attach_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    38417 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    32106 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4317 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_file.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10987 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_http.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2563 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_config_memory.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5204 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_conversion.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15782 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_decorator_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7800 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_escapes.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6828 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_locale.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14566 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13351 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_notify_base.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9886 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_apprise_api.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5479 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_bark.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6375 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_boxcar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7485 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_bulksms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3563 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_clicksend.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15886 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_form.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9598 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_json.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11978 2023-05-15 20:30:07.000000 apprise-1.4.0/test/test_plugin_custom_xml.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7691 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_d7networks.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8239 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_dapnet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4185 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_dingtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17508 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_discord.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    54366 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_email.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14726 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_emby.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6293 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_enigma2.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3183 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_faast.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    31528 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_fcm.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6513 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_flock.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9429 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17909 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_glib.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12515 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gnome.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6526 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_google_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6620 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_gotify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12895 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_growl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6775 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_guilded.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5438 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_homeassistant.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6966 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ifttt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7653 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_join.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4431 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_kavenegar.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4268 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_kumulos.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9987 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_lametric.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3560 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_line.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7906 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_macosx.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14877 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_mailgun.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25170 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_mastodon.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    28712 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_matrix.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5145 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_mattermost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4780 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_messagebird.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4018 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_misskey.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14403 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_mqtt.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5279 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_msg91.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    24031 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_msteams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5641 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_nextcloud.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5367 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_nextcloudtalk.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5284 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_notica.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4581 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_notifico.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    19775 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ntfy.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    12600 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_office365.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8154 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_onesignal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7644 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_opsgenie.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5148 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pagerduty.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5076 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pagertree.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3955 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_parse_platform.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3824 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_popcorn_notify.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6837 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_prowl.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13285 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushbullet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7441 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushed.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3986 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushjet.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    15365 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushover.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9248 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_pushsafer.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14541 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_reddit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    11403 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_rocket_chat.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5272 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ryver.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5702 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sendgrid.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2915 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_serverchan.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14848 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_ses.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13560 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_signal.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5900 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_simplepush.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6451 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sinch.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    23392 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_slack.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    25763 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_smseagle.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8969 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_smtp2go.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14499 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_sns.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    14377 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_sparkpost.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4848 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_spontit.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     5241 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_streamlabs.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     9643 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_syslog.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3266 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_techululs_push.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    34883 2023-05-13 02:23:07.000000 apprise-1.4.0/test/test_plugin_telegram.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8458 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twilio.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    16971 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twist.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    35809 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_twitter.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7789 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_voipms.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     8123 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_vonage.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4175 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_webex_teams.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    10991 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_windows.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6700 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_xbmc_kodi.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4960 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_plugin_zulip.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    13376 2023-05-12 22:30:02.000000 apprise-1.4.0/test/test_rest_plugins.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.299585 apprise-1.4.0/test/var/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1913 2022-12-18 21:46:05.000000 apprise-1.4.0/test/var/01_test_example.html
+-rw-r--r--   0 l2g       (1000) l2g       (1000)      277 2022-12-19 22:58:15.000000 apprise-1.4.0/test/var/apprise-archive.zip
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    76646 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.gif
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    73667 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.jpeg
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    17856 2022-12-18 21:46:05.000000 apprise-1.4.0/test/var/apprise-test.mp4
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)   248280 2019-12-22 13:31:28.000000 apprise-1.4.0/test/var/apprise-test.png
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-15 20:33:07.301585 apprise-1.4.0/test/var/fcm/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2231 2022-12-18 17:34:53.000000 apprise-1.4.0/test/var/fcm/service_account-bad-type.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     2238 2022-12-18 17:34:53.000000 apprise-1.4.0/test/var/fcm/service_account.json
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        8 2022-12-18 17:34:53.000000 apprise-1.4.0/win-requirements.txt
```

### Comparing `apprise-1.3.0/KEYWORDS` & `apprise-1.4.0/KEYWORDS`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/LICENSE` & `apprise-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/PKG-INFO` & `apprise-1.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.3.0
+Version: 1.4.0
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
 Keywords: Alerts API AWS Boxcar BulkSMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex Windows Voipms XBMC
 Platform: UNKNOWN
@@ -249,26 +249,36 @@
 ```bash
 # By default if no url or configuration is specified apprise will attempt to load
 # configuration files (if present) from:
 #  ~/.apprise
 #  ~/.apprise.yml
 #  ~/.config/apprise
 #  ~/.config/apprise.yml
+#  /etc/apprise
+#  /etc/apprise.yml
 
 # Also a subdirectory handling allows you to leverage plugins
 #  ~/.apprise/apprise
 #  ~/.apprise/apprise.yml
 #  ~/.config/apprise/apprise
 #  ~/.config/apprise/apprise.yml
+#  /etc/apprise/apprise
+#  /etc/apprise/apprise.yml
 
 # Windows users can store their default configuration files here:
 #  %APPDATA%/Apprise/apprise
 #  %APPDATA%/Apprise/apprise.yml
 #  %LOCALAPPDATA%/Apprise/apprise
 #  %LOCALAPPDATA%/Apprise/apprise.yml
+#  %ALLUSERSPROFILE%\Apprise\apprise
+#  %ALLUSERSPROFILE%\Apprise\apprise.yml
+#  %PROGRAMFILES%\Apprise\apprise
+#  %PROGRAMFILES%\Apprise\apprise.yml
+#  %COMMONPROGRAMFILES%\Apprise\apprise
+#  %COMMONPROGRAMFILES%\Apprise\apprise.yml
 
 # If you loaded one of those files, your command line gets really easy:
 apprise -vv -t 'my title' -b 'my notification body'
 
 # If you want to deviate from the default paths or specify more than one,
 # just specify them using the --config switch:
 apprise -vv -t 'my title' -b 'my notification body' \
@@ -321,18 +331,22 @@
 
 Once you've defined your custom hook, you just need to tell Apprise where it is at runtime.
 ```bash
 # By default if no plugin path is specified apprise will attempt to load
 # all plugin files (if present) from the following directory paths:
 #  ~/.apprise/plugins
 #  ~/.config/apprise/plugins
+#  /var/lib/apprise/plugins
 
 # Windows users can store their default plugin files in these directories:
 #  %APPDATA%/Apprise/plugins
 #  %LOCALAPPDATA%/Apprise/plugins
+#  %ALLUSERSPROFILE%\Apprise\plugins
+#  %PROGRAMFILES%\Apprise\plugins
+#  %COMMONPROGRAMFILES%\Apprise\plugins
 
 # If you placed your plugin file within one of the directories already defined
 # above, then your call simply needs to look like:
 apprise -vv --title 'custom override' \
         --body 'the body of my message' \
         foobar:\\
```

### Comparing `apprise-1.3.0/README.md` & `apprise-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -217,26 +217,36 @@
 ```bash
 # By default if no url or configuration is specified apprise will attempt to load
 # configuration files (if present) from:
 #  ~/.apprise
 #  ~/.apprise.yml
 #  ~/.config/apprise
 #  ~/.config/apprise.yml
+#  /etc/apprise
+#  /etc/apprise.yml
 
 # Also a subdirectory handling allows you to leverage plugins
 #  ~/.apprise/apprise
 #  ~/.apprise/apprise.yml
 #  ~/.config/apprise/apprise
 #  ~/.config/apprise/apprise.yml
+#  /etc/apprise/apprise
+#  /etc/apprise/apprise.yml
 
 # Windows users can store their default configuration files here:
 #  %APPDATA%/Apprise/apprise
 #  %APPDATA%/Apprise/apprise.yml
 #  %LOCALAPPDATA%/Apprise/apprise
 #  %LOCALAPPDATA%/Apprise/apprise.yml
+#  %ALLUSERSPROFILE%\Apprise\apprise
+#  %ALLUSERSPROFILE%\Apprise\apprise.yml
+#  %PROGRAMFILES%\Apprise\apprise
+#  %PROGRAMFILES%\Apprise\apprise.yml
+#  %COMMONPROGRAMFILES%\Apprise\apprise
+#  %COMMONPROGRAMFILES%\Apprise\apprise.yml
 
 # If you loaded one of those files, your command line gets really easy:
 apprise -vv -t 'my title' -b 'my notification body'
 
 # If you want to deviate from the default paths or specify more than one,
 # just specify them using the --config switch:
 apprise -vv -t 'my title' -b 'my notification body' \
@@ -289,18 +299,22 @@
 
 Once you've defined your custom hook, you just need to tell Apprise where it is at runtime.
 ```bash
 # By default if no plugin path is specified apprise will attempt to load
 # all plugin files (if present) from the following directory paths:
 #  ~/.apprise/plugins
 #  ~/.config/apprise/plugins
+#  /var/lib/apprise/plugins
 
 # Windows users can store their default plugin files in these directories:
 #  %APPDATA%/Apprise/plugins
 #  %LOCALAPPDATA%/Apprise/plugins
+#  %ALLUSERSPROFILE%\Apprise\plugins
+#  %PROGRAMFILES%\Apprise\plugins
+#  %COMMONPROGRAMFILES%\Apprise\plugins
 
 # If you placed your plugin file within one of the directories already defined
 # above, then your call simply needs to look like:
 apprise -vv --title 'custom override' \
         --body 'the body of my message' \
         foobar:\\
```

### Comparing `apprise-1.3.0/apprise/Apprise.py` & `apprise-1.4.0/apprise/Apprise.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 import asyncio
+import concurrent.futures as cf
 import os
-from functools import partial
 from itertools import chain
 from . import common
 from .conversion import convert_between
 from .utils import is_exclusive_match
 from .utils import parse_list
 from .utils import parse_urls
 from .utils import cwe312_url
@@ -372,115 +372,80 @@
         Set interpret_escapes to True if you want to pre-escape a string
         such as turning a \n into an actual new line, etc.
         """
 
         try:
             # Process arguments and build synchronous and asynchronous calls
             # (this step can throw internal errors).
-            sync_partials, async_cors = self._create_notify_calls(
+            sequential_calls, parallel_calls = self._create_notify_calls(
                 body, title,
                 notify_type=notify_type, body_format=body_format,
                 tag=tag, match_always=match_always, attach=attach,
                 interpret_escapes=interpret_escapes
             )
 
         except TypeError:
             # No notifications sent, and there was an internal error.
             return False
 
-        if not sync_partials and not async_cors:
+        if not sequential_calls and not parallel_calls:
             # Nothing to send
             return None
 
-        sync_result = Apprise._notify_all(*sync_partials)
-
-        if async_cors:
-            # A single coroutine sends all asynchronous notifications in
-            # parallel.
-            all_cor = Apprise._async_notify_all(*async_cors)
-
-            try:
-                # Python <3.7 automatically starts an event loop if there isn't
-                # already one for the main thread.
-                loop = asyncio.get_event_loop()
-
-            except RuntimeError:
-                # Python >=3.7 raises this exception if there isn't already an
-                # event loop. So, we can spin up our own.
-                loop = asyncio.new_event_loop()
-                asyncio.set_event_loop(loop)
-                loop.set_debug(self.debug)
-
-                # Run the coroutine and wait for the result.
-                async_result = loop.run_until_complete(all_cor)
-
-                # Clean up the loop.
-                loop.close()
-                asyncio.set_event_loop(None)
-
-            else:
-                old_debug = loop.get_debug()
-                loop.set_debug(self.debug)
-
-                # Run the coroutine and wait for the result.
-                async_result = loop.run_until_complete(all_cor)
-
-                loop.set_debug(old_debug)
-
-        else:
-            async_result = True
-
-        return sync_result and async_result
+        sequential_result = Apprise._notify_sequential(*sequential_calls)
+        parallel_result = Apprise._notify_parallel_threadpool(*parallel_calls)
+        return sequential_result and parallel_result
 
     async def async_notify(self, *args, **kwargs):
         """
         Send a notification to all the plugins previously loaded, for
         asynchronous callers.
 
         The arguments are identical to those of Apprise.notify().
 
         """
         try:
             # Process arguments and build synchronous and asynchronous calls
             # (this step can throw internal errors).
-            sync_partials, async_cors = self._create_notify_calls(
+            sequential_calls, parallel_calls = self._create_notify_calls(
                 *args, **kwargs)
 
         except TypeError:
             # No notifications sent, and there was an internal error.
             return False
 
-        if not sync_partials and not async_cors:
+        if not sequential_calls and not parallel_calls:
             # Nothing to send
             return None
 
-        sync_result = Apprise._notify_all(*sync_partials)
-        async_result = await Apprise._async_notify_all(*async_cors)
-        return sync_result and async_result
+        sequential_result = Apprise._notify_sequential(*sequential_calls)
+        parallel_result = \
+            await Apprise._notify_parallel_asyncio(*parallel_calls)
+        return sequential_result and parallel_result
 
     def _create_notify_calls(self, *args, **kwargs):
         """
         Creates notifications for all the plugins loaded.
 
-        Returns a list of synchronous calls (partial functions with no
-        arguments required) for plugins with async disabled and a list of
-        asynchronous calls (coroutines) for plugins with async enabled.
+        Returns a list of (server, notify() kwargs) tuples for plugins with
+        parallelism disabled and another list for plugins with parallelism
+        enabled.
         """
 
         all_calls = list(self._create_notify_gen(*args, **kwargs))
 
-        # Split into synchronous partials and asynchronous coroutines.
-        sync_partials, async_cors = [], []
-        for notify in all_calls:
-            if asyncio.iscoroutine(notify):
-                async_cors.append(notify)
+        # Split into sequential and parallel notify() calls.
+        sequential, parallel = [], []
+        for (server, notify_kwargs) in all_calls:
+            if server.asset.async_mode:
+                parallel.append((server, notify_kwargs))
             else:
-                sync_partials.append(notify)
+                sequential.append((server, notify_kwargs))
 
-        return sync_partials, async_cors
+        return sequential, parallel
 
     def _create_notify_gen(self, body, title='',
                            notify_type=common.NotifyType.INFO,
                            body_format=None, tag=common.MATCH_ALL_TAG,
                            match_always=True, attach=None,
                            interpret_escapes=None):
         """
@@ -580,31 +545,28 @@
             kwargs = dict(
                 body=conversion_body_map[server.notify_format],
                 title=conversion_title_map[server.notify_format],
                 notify_type=notify_type,
                 attach=attach,
                 body_format=body_format
             )
-            if server.asset.async_mode:
-                yield server.async_notify(**kwargs)
-            else:
-                yield partial(server.notify, **kwargs)
+            yield (server, kwargs)
 
     @staticmethod
-    def _notify_all(*partials):
+    def _notify_sequential(*servers_kwargs):
         """
-        Process a list of synchronous notify() calls.
+        Process a list of notify() calls sequentially and synchronously.
         """
 
         success = True
 
-        for notify in partials:
+        for (server, kwargs) in servers_kwargs:
             try:
                 # Send notification
-                result = notify()
+                result = server.notify(**kwargs)
                 success = success and result
 
             except TypeError:
                 # These are our internally thrown notifications.
                 success = False
 
             except Exception:
@@ -612,22 +574,79 @@
                 # just because one of our plugins has a bug in it.
                 logger.exception("Unhandled Notification Exception")
                 success = False
 
         return success
 
     @staticmethod
-    async def _async_notify_all(*cors):
+    def _notify_parallel_threadpool(*servers_kwargs):
         """
-        Process a list of asynchronous async_notify() calls.
+        Process a list of notify() calls in parallel and synchronously.
         """
 
+        n_calls = len(servers_kwargs)
+
+        # 0-length case
+        if n_calls == 0:
+            return True
+
+        # There's no need to use a thread pool for just a single notification
+        if n_calls == 1:
+            return Apprise._notify_sequential(servers_kwargs[0])
+
         # Create log entry
-        logger.info('Notifying %d service(s) asynchronously.', len(cors))
+        logger.info(
+            'Notifying %d service(s) with threads.', len(servers_kwargs))
+
+        with cf.ThreadPoolExecutor() as executor:
+            success = True
+            futures = [executor.submit(server.notify, **kwargs)
+                       for (server, kwargs) in servers_kwargs]
+
+            for future in cf.as_completed(futures):
+                try:
+                    result = future.result()
+                    success = success and result
+
+                except TypeError:
+                    # These are our internally thrown notifications.
+                    success = False
+
+                except Exception:
+                    # A catch all so we don't have to abort early
+                    # just because one of our plugins has a bug in it.
+                    logger.exception("Unhandled Notification Exception")
+                    success = False
+
+            return success
+
+    @staticmethod
+    async def _notify_parallel_asyncio(*servers_kwargs):
+        """
+        Process a list of async_notify() calls in parallel and asynchronously.
+        """
+
+        n_calls = len(servers_kwargs)
 
+        # 0-length case
+        if n_calls == 0:
+            return True
+
+        # (Unlike with the thread pool, we don't optimize for the single-
+        # notification case because asyncio can do useful work while waiting
+        # for that thread to complete)
+
+        # Create log entry
+        logger.info(
+            'Notifying %d service(s) asynchronously.', len(servers_kwargs))
+
+        async def do_call(server, kwargs):
+            return await server.async_notify(**kwargs)
+
+        cors = (do_call(server, kwargs) for (server, kwargs) in servers_kwargs)
         results = await asyncio.gather(*cors, return_exceptions=True)
 
         if any(isinstance(status, Exception)
                and not isinstance(status, TypeError) for status in results):
             # A catch all so we don't have to abort early just because
             # one of our plugins has a bug in it.
             logger.exception("Unhandled Notification Exception")
@@ -661,14 +680,15 @@
 
             content = {
                 'service_name': getattr(plugin, 'service_name', None),
                 'service_url': getattr(plugin, 'service_url', None),
                 'setup_url': getattr(plugin, 'setup_url', None),
                 # Placeholder - populated below
                 'details': None,
+
                 # Differentiat between what is a custom loaded plugin and
                 # which is native.
                 'category': getattr(plugin, 'category', None)
             }
 
             # Standard protocol(s) should be None or a tuple
             enabled = getattr(plugin, 'enabled', True)
```

### Comparing `apprise-1.3.0/apprise/Apprise.pyi` & `apprise-1.4.0/apprise/Apprise.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseAsset.py` & `apprise-1.4.0/apprise/AppriseAsset.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseAsset.pyi` & `apprise-1.4.0/apprise/AppriseAsset.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseAttachment.py` & `apprise-1.4.0/apprise/AppriseAttachment.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseAttachment.pyi` & `apprise-1.4.0/apprise/AppriseAttachment.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseConfig.py` & `apprise-1.4.0/apprise/AppriseConfig.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseConfig.pyi` & `apprise-1.4.0/apprise/AppriseConfig.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/AppriseLocale.py` & `apprise-1.4.0/apprise/AppriseLocale.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/URLBase.py` & `apprise-1.4.0/apprise/URLBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -681,14 +681,23 @@
             response = HTML_LOOKUP[code]
 
         except KeyError:
             response = ''
 
         return response
 
+    def __len__(self):
+        """
+        Should be over-ridden and allows the tracking of how many targets
+        are associated with each URLBase object.
+
+        Default is always 1
+        """
+        return 1
+
     def schemas(self):
         """A simple function that returns a set of all schemas associated
         with this object based on the object.protocol and
         object.secure_protocol
         """
 
         schemas = set([])
```

### Comparing `apprise-1.3.0/apprise/URLBase.pyi` & `apprise-1.4.0/apprise/URLBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/__init__.py` & `apprise-1.4.0/apprise/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 __title__ = 'Apprise'
-__version__ = '1.3.0'
+__version__ = '1.4.0'
 __author__ = 'Chris Caron'
 __license__ = 'BSD'
 __copywrite__ = 'Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .common import NotifyType
```

### Comparing `apprise-1.3.0/apprise/assets/NotifyXML-1.0.xsd` & `apprise-1.4.0/apprise/assets/NotifyXML-1.0.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/NotifyXML-1.1.xsd` & `apprise-1.4.0/apprise/assets/NotifyXML-1.1.xsd`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-failure-128x128.ico` & `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-failure-128x128.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-failure-256x256.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-failure-32x32.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-failure-72x72.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-failure-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-info-128x128.ico` & `apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-info-128x128.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-info-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-info-256x256.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-info-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-info-32x32.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-info-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-info-72x72.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-info-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-logo.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-logo.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-success-128x128.ico` & `apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-success-128x128.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-success-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-success-256x256.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-success-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-success-32x32.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-success-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-success-72x72.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-success-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-warning-128x128.ico` & `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.ico`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-warning-128x128.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-128x128.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-warning-256x256.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-256x256.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-warning-32x32.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-32x32.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/assets/themes/default/apprise-warning-72x72.png` & `apprise-1.4.0/apprise/assets/themes/default/apprise-warning-72x72.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/attachment/AttachBase.py` & `apprise-1.4.0/apprise/attachment/AttachBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/attachment/AttachBase.pyi` & `apprise-1.4.0/apprise/attachment/AttachBase.pyi`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/attachment/AttachFile.py` & `apprise-1.4.0/apprise/attachment/AttachFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/attachment/AttachHTTP.py` & `apprise-1.4.0/apprise/attachment/AttachHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/attachment/__init__.py` & `apprise-1.4.0/apprise/attachment/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/cli.py` & `apprise-1.4.0/apprise/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,36 +76,72 @@
     '~/.config/apprise.yml',
 
     # Plugin Support Extended Directory Search Paths
     '~/.apprise/apprise',
     '~/.apprise/apprise.yml',
     '~/.config/apprise/apprise',
     '~/.config/apprise/apprise.yml',
+
+    # Global Configuration Support
+    '/etc/apprise',
+    '/etc/apprise.yml',
+    '/etc/apprise/apprise',
+    '/etc/apprise/apprise.yml',
 )
 
 # Define our paths to search for plugins
 DEFAULT_PLUGIN_PATHS = (
     '~/.apprise/plugins',
     '~/.config/apprise/plugins',
+
+    # Global Plugin Support
+    '/var/lib/apprise/plugins',
 )
 
 # Detect Windows
 if platform.system() == 'Windows':
     # Default Config Search Path for Windows Users
     DEFAULT_CONFIG_PATHS = (
-        expandvars('%APPDATA%/Apprise/apprise'),
-        expandvars('%APPDATA%/Apprise/apprise.yml'),
-        expandvars('%LOCALAPPDATA%/Apprise/apprise'),
-        expandvars('%LOCALAPPDATA%/Apprise/apprise.yml'),
+        expandvars('%APPDATA%\\Apprise\\apprise'),
+        expandvars('%APPDATA%\\Apprise\\apprise.yml'),
+        expandvars('%LOCALAPPDATA%\\Apprise\\apprise'),
+        expandvars('%LOCALAPPDATA%\\Apprise\\apprise.yml'),
+
+        #
+        # Global Support
+        #
+
+        # C:\ProgramData\Apprise\
+        expandvars('%ALLUSERSPROFILE%\\Apprise\\apprise'),
+        expandvars('%ALLUSERSPROFILE%\\Apprise\\apprise.yml'),
+
+        # C:\Program Files\Apprise
+        expandvars('%PROGRAMFILES%\\Apprise\\apprise'),
+        expandvars('%PROGRAMFILES%\\Apprise\\apprise.yml'),
+
+        # C:\Program Files\Common Files
+        expandvars('%COMMONPROGRAMFILES%\\Apprise\\apprise'),
+        expandvars('%COMMONPROGRAMFILES%\\Apprise\\apprise.yml'),
     )
 
     # Default Plugin Search Path for Windows Users
     DEFAULT_PLUGIN_PATHS = (
-        expandvars('%APPDATA%/Apprise/plugins'),
-        expandvars('%LOCALAPPDATA%/Apprise/plugins'),
+        expandvars('%APPDATA%\\Apprise\\plugins'),
+        expandvars('%LOCALAPPDATA%\\Apprise\\plugins'),
+
+        #
+        # Global Support
+        #
+
+        # C:\ProgramData\Apprise\plugins
+        expandvars('%ALLUSERSPROFILE%\\Apprise\\plugins'),
+        # C:\Program Files\Apprise\plugins
+        expandvars('%PROGRAMFILES%\\Apprise\\plugins'),
+        # C:\Program Files\Common Files
+        expandvars('%COMMONPROGRAMFILES%\\Apprise\\plugins'),
     )
 
 
 def print_help_msg(command):
     """
     Prints help message when -h or --help is specified.
```

### Comparing `apprise-1.3.0/apprise/common.py` & `apprise-1.4.0/apprise/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/config/ConfigBase.py` & `apprise-1.4.0/apprise/config/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/config/ConfigFile.py` & `apprise-1.4.0/apprise/config/ConfigFile.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/config/ConfigHTTP.py` & `apprise-1.4.0/apprise/config/ConfigHTTP.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/config/ConfigMemory.py` & `apprise-1.4.0/apprise/config/ConfigMemory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/config/__init__.py` & `apprise-1.4.0/apprise/config/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/conversion.py` & `apprise-1.4.0/apprise/conversion.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/decorators/CustomNotifyPlugin.py` & `apprise-1.4.0/apprise/decorators/CustomNotifyPlugin.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/decorators/__init__.py` & `apprise-1.4.0/apprise/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/decorators/notify.py` & `apprise-1.4.0/apprise/decorators/notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/logger.py` & `apprise-1.4.0/apprise/logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyAppriseAPI.py` & `apprise-1.4.0/apprise/plugins/NotifyRyver.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,355 +26,336 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
+# To use this plugin, you need to first generate a webhook.
+
+# When you're complete, you will recieve a URL that looks something like this:
+#                https://apprise.ryver.com/application/webhook/ckhrjW8w672m6HG
+#                          ^                                        ^
+#                          |                                        |
+#  These are important <---^----------------------------------------^
+#
 import re
 import requests
 from json import dumps
 
 from .NotifyBase import NotifyBase
-from ..URLBase import PrivacyMode
+from ..common import NotifyImageSize
 from ..common import NotifyType
-from ..utils import parse_list
+from ..utils import parse_bool
 from ..utils import validate_regex
 from ..AppriseLocale import gettext_lazy as _
 
 
-class NotifyAppriseAPI(NotifyBase):
+class RyverWebhookMode:
     """
-    A wrapper for Apprise (Persistent) API Notifications
+    Ryver supports to webhook modes
+    """
+    SLACK = 'slack'
+    RYVER = 'ryver'
+
+
+# Define the types in a list for validation purposes
+RYVER_WEBHOOK_MODES = (
+    RyverWebhookMode.SLACK,
+    RyverWebhookMode.RYVER,
+)
+
+
+class NotifyRyver(NotifyBase):
+    """
+    A wrapper for Ryver Notifications
     """
 
     # The default descriptive name associated with the Notification
-    service_name = 'Apprise API'
+    service_name = 'Ryver'
 
     # The services URL
-    service_url = 'https://github.com/caronc/apprise-api'
-
-    # The default protocol
-    protocol = 'apprise'
+    service_url = 'https://ryver.com/'
 
     # The default secure protocol
-    secure_protocol = 'apprises'
+    secure_protocol = 'ryver'
 
     # A URL that takes you to the setup/help of the specific protocol
-    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_apprise_api'
+    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_ryver'
+
+    # Allows the user to specify the NotifyImageSize object
+    image_size = NotifyImageSize.XY_72
 
-    # Depending on the number of transactions/notifications taking place, this
-    # could take a while. 30 seconds should be enough to perform the task
-    socket_connect_timeout = 30.0
-
-    # Disable throttle rate for Apprise API requests since they are normally
-    # local anyway
-    request_rate_per_sec = 0.0
+    # The maximum allowable characters allowed in the body per message
+    body_maxlen = 1000
 
     # Define object templates
     templates = (
-        '{schema}://{host}/{token}',
-        '{schema}://{host}:{port}/{token}',
-        '{schema}://{user}@{host}/{token}',
-        '{schema}://{user}@{host}:{port}/{token}',
-        '{schema}://{user}:{password}@{host}/{token}',
-        '{schema}://{user}:{password}@{host}:{port}/{token}',
+        '{schema}://{organization}/{token}',
+        '{schema}://{user}@{organization}/{token}',
     )
 
-    # Define our tokens; these are the minimum tokens required required to
-    # be passed into this function (as arguments). The syntax appends any
-    # previously defined in the base package and builds onto them
+    # Define our template tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
-        'host': {
-            'name': _('Hostname'),
+        'organization': {
+            'name': _('Organization'),
             'type': 'string',
             'required': True,
-        },
-        'port': {
-            'name': _('Port'),
-            'type': 'int',
-            'min': 1,
-            'max': 65535,
-        },
-        'user': {
-            'name': _('Username'),
-            'type': 'string',
-        },
-        'password': {
-            'name': _('Password'),
-            'type': 'string',
-            'private': True,
+            'regex': (r'^[A-Z0-9_-]{3,32}$', 'i'),
         },
         'token': {
             'name': _('Token'),
             'type': 'string',
             'required': True,
             'private': True,
-            'regex': (r'^[A-Z0-9_-]{1,32}$', 'i'),
+            'regex': (r'^[A-Z0-9]{15}$', 'i'),
+        },
+        'user': {
+            'name': _('Bot Name'),
+            'type': 'string',
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
-        'tags': {
-            'name': _('Tags'),
-            'type': 'string',
+        'mode': {
+            'name': _('Webhook Mode'),
+            'type': 'choice:string',
+            'values': RYVER_WEBHOOK_MODES,
+            'default': RyverWebhookMode.RYVER,
         },
-        'to': {
-            'alias_of': 'token',
+        'image': {
+            'name': _('Include Image'),
+            'type': 'bool',
+            'default': True,
+            'map_to': 'include_image',
         },
     })
 
-    # Define any kwargs we're using
-    template_kwargs = {
-        'headers': {
-            'name': _('HTTP Header'),
-            'prefix': '+',
-        },
-    }
-
-    def __init__(self, token=None, tags=None, headers=None, **kwargs):
+    def __init__(self, organization, token, mode=RyverWebhookMode.RYVER,
+                 include_image=True, **kwargs):
         """
-        Initialize Apprise API Object
-
-        headers can be a dictionary of key/value pairs that you want to
-        additionally include as part of the server headers to post with
-
+        Initialize Ryver Object
         """
         super().__init__(**kwargs)
 
-        self.fullpath = kwargs.get('fullpath')
-        if not isinstance(self.fullpath, str):
-            self.fullpath = '/'
-
+        # API Token (associated with project)
         self.token = validate_regex(
             token, *self.template_tokens['token']['regex'])
         if not self.token:
-            msg = 'The Apprise API token specified ({}) is invalid.'\
-                .format(token)
+            msg = 'An invalid Ryver API Token ' \
+                  '({}) was specified.'.format(token)
             self.logger.warning(msg)
             raise TypeError(msg)
 
-        # Build list of tags
-        self.__tags = parse_list(tags)
-
-        self.headers = {}
-        if headers:
-            # Store our extra headers
-            self.headers.update(headers)
-
-        return
-
-    def url(self, privacy=False, *args, **kwargs):
-        """
-        Returns the URL built dynamically based on specified arguments.
-        """
-
-        # Our URL parameters
-        params = self.url_parameters(privacy=privacy, *args, **kwargs)
+        # Organization (associated with project)
+        self.organization = validate_regex(
+            organization, *self.template_tokens['organization']['regex'])
+        if not self.organization:
+            msg = 'An invalid Ryver Organization ' \
+                  '({}) was specified.'.format(organization)
+            self.logger.warning(msg)
+            raise TypeError(msg)
 
-        # Append our headers into our parameters
-        params.update({'+{}'.format(k): v for k, v in self.headers.items()})
+        # Store our webhook mode
+        self.mode = None \
+            if not isinstance(mode, str) else mode.lower()
+
+        if self.mode not in RYVER_WEBHOOK_MODES:
+            msg = 'The Ryver webhook mode specified ({}) is invalid.' \
+                .format(mode)
+            self.logger.warning(msg)
+            raise TypeError(msg)
 
-        if self.__tags:
-            params['tags'] = ','.join([x for x in self.__tags])
+        # Place an image inline with the message body
+        self.include_image = include_image
 
-        # Determine Authentication
-        auth = ''
-        if self.user and self.password:
-            auth = '{user}:{password}@'.format(
-                user=NotifyAppriseAPI.quote(self.user, safe=''),
-                password=self.pprint(
-                    self.password, privacy, mode=PrivacyMode.Secret, safe=''),
-            )
-        elif self.user:
-            auth = '{user}@'.format(
-                user=NotifyAppriseAPI.quote(self.user, safe=''),
-            )
+        # Slack formatting requirements are defined here which Ryver supports:
+        # https://api.slack.com/docs/message-formatting
+        self._re_formatting_map = {
+            # New lines must become the string version
+            r'\r\*\n': '\\n',
+            # Escape other special characters
+            r'&': '&amp;',
+            r'<': '&lt;',
+            r'>': '&gt;',
+        }
 
-        default_port = 443 if self.secure else 80
+        # Iterate over above list and store content accordingly
+        self._re_formatting_rules = re.compile(
+            r'(' + '|'.join(self._re_formatting_map.keys()) + r')',
+            re.IGNORECASE,
+        )
 
-        fullpath = self.fullpath.strip('/')
-        return '{schema}://{auth}{hostname}{port}{fullpath}{token}' \
-               '/?{params}'.format(
-                   schema=self.secure_protocol
-                   if self.secure else self.protocol,
-                   auth=auth,
-                   # never encode hostname since we're expecting it to be a
-                   # valid one
-                   hostname=self.host,
-                   port='' if self.port is None or self.port == default_port
-                        else ':{}'.format(self.port),
-                   fullpath='/{}/'.format(NotifyAppriseAPI.quote(
-                       fullpath, safe='/')) if fullpath else '/',
-                   token=self.pprint(self.token, privacy, safe=''),
-                   params=NotifyAppriseAPI.urlencode(params))
+        return
 
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
-        Perform Apprise API Notification
+        Perform Ryver Notification
         """
 
-        headers = {}
-        # Apply any/all header over-rides defined
-        headers.update(self.headers)
-
-        # prepare Apprise API Object
-        payload = {
-            # Apprise API Payload
-            'title': title,
-            'body': body,
-            'type': notify_type,
-            'format': self.notify_format,
+        headers = {
+            'User-Agent': self.app_id,
+            'Content-Type': 'application/json',
         }
 
-        if self.__tags:
-            payload['tag'] = self.__tags
-
-        auth = None
-        if self.user:
-            auth = (self.user, self.password)
+        if self.mode == RyverWebhookMode.SLACK:
+            # Perform Slack formatting
+            title = self._re_formatting_rules.sub(  # pragma: no branch
+                lambda x: self._re_formatting_map[x.group()], title,
+            )
+            body = self._re_formatting_rules.sub(  # pragma: no branch
+                lambda x: self._re_formatting_map[x.group()], body,
+            )
 
-        # Set our schema
-        schema = 'https' if self.secure else 'http'
+        url = 'https://{}.ryver.com/application/webhook/{}'.format(
+            self.organization,
+            self.token,
+        )
 
-        url = '%s://%s' % (schema, self.host)
-        if isinstance(self.port, int):
-            url += ':%d' % self.port
+        # prepare JSON Object
+        payload = {
+            'body': body if not title else '**{}**\r\n{}'.format(title, body),
+            'createSource': {
+                'displayName': self.user,
+                'avatar': None,
+            },
+        }
 
-        fullpath = self.fullpath.strip('/')
-        url += '/{}/'.format(fullpath) if fullpath else '/'
-        url += 'notify/{}'.format(self.token)
+        # Acquire our image url if configured to do so
+        image_url = None if not self.include_image else \
+            self.image_url(notify_type)
 
-        # Some entries can not be over-ridden
-        headers.update({
-            'User-Agent': self.app_id,
-            'Content-Type': 'application/json',
-            # Pass our Source UUID4 Identifier
-            'X-Apprise-ID': self.asset._uid,
-            # Pass our current recursion count to our upstream server
-            'X-Apprise-Recursion-Count': str(self.asset._recursion + 1),
-        })
+        if image_url:
+            payload['createSource']['avatar'] = image_url
 
-        self.logger.debug('Apprise API POST URL: %s (cert_verify=%r)' % (
+        self.logger.debug('Ryver POST URL: %s (cert_verify=%r)' % (
             url, self.verify_certificate,
         ))
-        self.logger.debug('Apprise API Payload: %s' % str(payload))
+        self.logger.debug('Ryver Payload: %s' % str(payload))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         try:
             r = requests.post(
                 url,
                 data=dumps(payload),
                 headers=headers,
-                auth=auth,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
+
             if r.status_code != requests.codes.ok:
                 # We had a problem
                 status_str = \
-                    NotifyAppriseAPI.http_response_code_lookup(r.status_code)
+                    NotifyBase.http_response_code_lookup(r.status_code)
 
                 self.logger.warning(
-                    'Failed to send Apprise API notification: '
+                    'Failed to send Ryver notification: '
                     '{}{}error={}.'.format(
                         status_str,
                         ', ' if status_str else '',
                         r.status_code))
 
                 self.logger.debug('Response Details:\r\n{}'.format(r.content))
 
                 # Return; we're done
                 return False
 
             else:
-                self.logger.info('Sent Apprise API notification.')
+                self.logger.info('Sent Ryver notification.')
 
         except requests.RequestException as e:
             self.logger.warning(
-                'A Connection error occurred sending Apprise API '
-                'notification to %s.' % self.host)
+                'A Connection error occurred sending Ryver:%s ' % (
+                    self.organization) + 'notification.'
+            )
             self.logger.debug('Socket Exception: %s' % str(e))
-
-            # Return; we're done
             return False
 
         return True
 
-    @staticmethod
-    def parse_native_url(url):
+    def url(self, privacy=False, *args, **kwargs):
         """
-        Support http://hostname/notify/token and
-                http://hostname/path/notify/token
+        Returns the URL built dynamically based on specified arguments.
         """
 
-        result = re.match(
-            r'^http(?P<secure>s?)://(?P<hostname>[A-Z0-9._-]+)'
-            r'(:(?P<port>[0-9]+))?'
-            r'(?P<path>/[^?]+?)?/notify/(?P<token>[A-Z0-9_-]{1,32})/?'
-            r'(?P<params>\?.+)?$', url, re.I)
+        # Define any URL parameters
+        params = {
+            'image': 'yes' if self.include_image else 'no',
+            'mode': self.mode,
+        }
 
-        if result:
-            return NotifyAppriseAPI.parse_url(
-                '{schema}://{hostname}{port}{path}/{token}/{params}'.format(
-                    schema=NotifyAppriseAPI.secure_protocol
-                    if result.group('secure') else NotifyAppriseAPI.protocol,
-                    hostname=result.group('hostname'),
-                    port='' if not result.group('port')
-                    else ':{}'.format(result.group('port')),
-                    path='' if not result.group('path')
-                    else result.group('path'),
-                    token=result.group('token'),
-                    params='' if not result.group('params')
-                    else '?{}'.format(result.group('params'))))
+        # Extend our parameters
+        params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
-        return None
+        # Determine if there is a botname present
+        botname = ''
+        if self.user:
+            botname = '{botname}@'.format(
+                botname=NotifyRyver.quote(self.user, safe=''),
+            )
+
+        return '{schema}://{botname}{organization}/{token}/?{params}'.format(
+            schema=self.secure_protocol,
+            botname=botname,
+            organization=NotifyRyver.quote(self.organization, safe=''),
+            token=self.pprint(self.token, privacy, safe=''),
+            params=NotifyRyver.urlencode(params),
+        )
 
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
-        results = NotifyBase.parse_url(url)
+
+        results = NotifyBase.parse_url(url, verify_host=False)
         if not results:
             # We're done early as we couldn't load the results
             return results
 
-        # Add our headers that the user can potentially over-ride if they wish
-        # to to our returned result set and tidy entries by unquoting them
-        results['headers'] = \
-            {NotifyAppriseAPI.unquote(x): NotifyAppriseAPI.unquote(y)
-             for x, y in results['qsd+'].items()}
-
-        # Support the passing of tags in the URL
-        if 'tags' in results['qsd'] and len(results['qsd']['tags']):
-            results['tags'] = \
-                NotifyAppriseAPI.parse_list(results['qsd']['tags'])
-
-        # Support the 'to' & 'token' variable so that we can support rooms
-        # this way too.
-        if 'token' in results['qsd'] and len(results['qsd']['token']):
+        # The first token is stored in the hostname
+        results['organization'] = NotifyRyver.unquote(results['host'])
+
+        # Now fetch the remaining tokens
+        try:
             results['token'] = \
-                NotifyAppriseAPI.unquote(results['qsd']['token'])
+                NotifyRyver.split_path(results['fullpath'])[0]
 
-        elif 'to' in results['qsd'] and len(results['qsd']['to']):
-            results['token'] = NotifyAppriseAPI.unquote(results['qsd']['to'])
+        except IndexError:
+            # no token
+            results['token'] = None
+
+        # Retrieve the mode
+        results['mode'] = results['qsd'].get('mode', RyverWebhookMode.RYVER)
+
+        # use image= for consistency with the other plugins
+        results['include_image'] = \
+            parse_bool(results['qsd'].get('image', True))
 
-        else:
-            # Start with a list of path entries to work with
-            entries = NotifyAppriseAPI.split_path(results['fullpath'])
-            if entries:
-                # use our last entry found
-                results['token'] = entries[-1]
+        return results
 
-                # pop our last entry off
-                entries = entries[:-1]
+    @staticmethod
+    def parse_native_url(url):
+        """
+        Support https://RYVER_ORG.ryver.com/application/webhook/TOKEN
+        """
+
+        result = re.match(
+            r'^https?://(?P<org>[A-Z0-9_-]+)\.ryver\.com/application/webhook/'
+            r'(?P<webhook_token>[A-Z0-9]+)/?'
+            r'(?P<params>\?.+)?$', url, re.I)
 
-                # re-assemble our full path
-                results['fullpath'] = '/'.join(entries)
+        if result:
+            return NotifyRyver.parse_url(
+                '{schema}://{org}/{webhook_token}/{params}'.format(
+                    schema=NotifyRyver.secure_protocol,
+                    org=result.group('org'),
+                    webhook_token=result.group('webhook_token'),
+                    params='' if not result.group('params')
+                    else result.group('params')))
 
-        return results
+        return None
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyBark.py` & `apprise-1.4.0/apprise/plugins/NotifyBark.py`

 * *Files 2% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         """
         Perform Bark Notification
         """
 
         # error tracking (used for function return)
         has_error = False
 
-        if not len(self.targets):
+        if not self.targets:
             # We have nothing to notify; we're done
             self.logger.warning('There are no Bark devices to notify')
             return False
 
         # Prepare our headers
         headers = {
             'User-Agent': self.app_id,
@@ -452,14 +452,20 @@
             port='' if self.port is None or self.port == default_port
                  else ':{}'.format(self.port),
             targets='/'.join(
                 [NotifyBark.quote('{}'.format(x)) for x in self.targets]),
             params=NotifyBark.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyBase.py` & `apprise-1.4.0/apprise/plugins/NotifyBase.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyBoxcar.py` & `apprise-1.4.0/apprise/plugins/NotifyBoxcar.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,27 +42,28 @@
 
 except ImportError:
     from urllib.parse import urlparse
 
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..utils import parse_bool
+from ..utils import parse_list
 from ..utils import validate_regex
 from ..common import NotifyType
 from ..common import NotifyImageSize
 from ..AppriseLocale import gettext_lazy as _
 
 # Default to sending to all devices if nothing is specified
 DEFAULT_TAG = '@all'
 
 # The tags value is an structure containing an array of strings defining the
 # list of tagged devices that the notification need to be send to, and a
 # boolean operator (‘and’ / ‘or’) that defines the criteria to match devices
 # against those tags.
-IS_TAG = re.compile(r'^[@](?P<name>[A-Z0-9]{1,63})$', re.I)
+IS_TAG = re.compile(r'^[@]?(?P<name>[A-Z0-9]{1,63})$', re.I)
 
 # Device tokens are only referenced when developing.
 # It's not likely you'll send a message directly to a device, but if you do;
 # this plugin supports it.
 IS_DEVICETOKEN = re.compile(r'^[A-Z0-9]{64}$', re.I)
 
 # Used to break apart list of potential tags by their delimiter into a useable
@@ -156,15 +157,15 @@
                  **kwargs):
         """
         Initialize Boxcar Object
         """
         super().__init__(**kwargs)
 
         # Initialize tag list
-        self.tags = list()
+        self._tags = list()
 
         # Initialize device_token list
         self.device_tokens = list()
 
         # Access Key (associated with project)
         self.access = validate_regex(
             access, *self.template_tokens['access_key']['regex'])
@@ -180,37 +181,35 @@
         if not self.secret:
             msg = 'An invalid Boxcar Secret Key ' \
                   '({}) was specified.'.format(secret)
             self.logger.warning(msg)
             raise TypeError(msg)
 
         if not targets:
-            self.tags.append(DEFAULT_TAG)
+            self._tags.append(DEFAULT_TAG)
             targets = []
 
-        elif isinstance(targets, str):
-            targets = [x for x in filter(bool, TAGS_LIST_DELIM.split(
-                targets,
-            ))]
-
         # Validate targets and drop bad ones:
-        for target in targets:
-            if IS_TAG.match(target):
+        for target in parse_list(targets):
+            result = IS_TAG.match(target)
+            if result:
                 # store valid tag/alias
-                self.tags.append(IS_TAG.match(target).group('name'))
+                self._tags.append(result.group('name'))
+                continue
 
-            elif IS_DEVICETOKEN.match(target):
+            result = IS_DEVICETOKEN.match(target)
+            if result:
                 # store valid device
                 self.device_tokens.append(target)
+                continue
 
-            else:
-                self.logger.warning(
-                    'Dropped invalid tag/alias/device_token '
-                    '({}) specified.'.format(target),
-                )
+            self.logger.warning(
+                'Dropped invalid tag/alias/device_token '
+                '({}) specified.'.format(target),
+            )
 
         # Track whether or not we want to send an image with our notification
         # or not.
         self.include_image = include_image
 
         return
 
@@ -234,16 +233,16 @@
 
         if title:
             payload['aps']['@title'] = title
 
         if body:
             payload['aps']['alert'] = body
 
-        if self.tags:
-            payload['tags'] = {'or': self.tags}
+        if self._tags:
+            payload['tags'] = {'or': self._tags}
 
         if self.device_tokens:
             payload['device_tokens'] = self.device_tokens
 
         # Source picture should be <= 450 DP wide, ~2:1 aspect.
         image_url = None if not self.include_image \
             else self.image_url(notify_type)
@@ -337,18 +336,26 @@
         return '{schema}://{access}/{secret}/{targets}?{params}'.format(
             schema=self.secure_protocol,
             access=self.pprint(self.access, privacy, safe=''),
             secret=self.pprint(
                 self.secret, privacy, mode=PrivacyMode.Secret, safe=''),
             targets='/'.join([
                 NotifyBoxcar.quote(x, safe='') for x in chain(
-                    self.tags, self.device_tokens) if x != DEFAULT_TAG]),
+                    self._tags, self.device_tokens) if x != DEFAULT_TAG]),
             params=NotifyBoxcar.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self._tags) + len(self.device_tokens)
+        # DEFAULT_TAG is set if no tokens/tags are otherwise set
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns it broken apart into a dictionary.
 
         """
         results = NotifyBase.parse_url(url, verify_host=False)
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyBulkSMS.py` & `apprise-1.4.0/apprise/plugins/NotifyBulkSMS.py`

 * *Files 4% similar despite different names*

```diff
@@ -410,14 +410,32 @@
             targets='/'.join(chain(
                 [NotifyBulkSMS.quote('{}'.format(x), safe='+')
                  for x in self.targets],
                 [NotifyBulkSMS.quote('@{}'.format(x), safe='@')
                  for x in self.groups])),
             params=NotifyBulkSMS.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+
+        #
+        # Factor batch into calculation
+        #
+        # Note: Groups always require a separate request (and can not be
+        # included in batch calculations)
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets + len(self.groups)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyClickSend.py` & `apprise-1.4.0/apprise/plugins/NotifyClickSend.py`

 * *Files 7% similar despite different names*

```diff
@@ -284,14 +284,29 @@
             schema=self.secure_protocol,
             auth=auth,
             targets='/'.join(
                 [NotifyClickSend.quote(x, safe='') for x in self.targets]),
             params=NotifyClickSend.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyD7Networks.py` & `apprise-1.4.0/apprise/plugins/NotifyD7Networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -353,14 +353,23 @@
         return '{schema}://{token}@{targets}/?{params}'.format(
             schema=self.secure_protocol,
             token=self.pprint(self.token, privacy, safe=''),
             targets='/'.join(
                 [NotifyD7Networks.quote(x, safe='') for x in self.targets]),
             params=NotifyD7Networks.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        return len(self.targets) if not self.batch else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyDBus.py` & `apprise-1.4.0/apprise/plugins/NotifyDBus.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyDapnet.py` & `apprise-1.4.0/apprise/plugins/NotifyDapnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,14 +346,29 @@
             schema=self.secure_protocol,
             auth=auth,
             targets='/'.join([self.pprint(x, privacy, safe='')
                               for x in self.targets]),
             params=NotifyDapnet.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyDingTalk.py` & `apprise-1.4.0/apprise/plugins/NotifyDingTalk.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,14 +305,21 @@
             secret='' if not self.secret else '{}@'.format(self.pprint(
                 self.secret, privacy, mode=PrivacyMode.Secret, safe='')),
             token=self.pprint(self.token, privacy, safe=''),
             targets='/'.join(
                 [NotifyDingTalk.quote(x, safe='') for x in self.targets]),
             args=NotifyDingTalk.urlencode(args))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to substantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyDiscord.py` & `apprise-1.4.0/apprise/plugins/NotifyDiscord.py`

 * *Files 2% similar despite different names*

```diff
@@ -286,26 +286,24 @@
                     fields = fields[self.discord_max_fields:]
 
         else:
             # not markdown
             payload['content'] = \
                 body if not title else "{}\r\n{}".format(title, body)
 
-        if self.thread_id:
-            payload['thread_id'] = self.thread_id
-
         if self.avatar and (image_url or self.avatar_url):
             payload['avatar_url'] = \
                 self.avatar_url if self.avatar_url else image_url
 
         if self.user:
             # Optionally override the default username of the webhook
             payload['username'] = self.user
 
-        if not self._send(payload):
+        params = {'thread_id': self.thread_id} if self.thread_id else None
+        if not self._send(payload, params=params):
             # We failed to post our message
             return False
 
         # Process any remaining fields IF set
         if fields:
             payload['embeds'][0]['description'] = ''
             for i in range(0, len(fields), self.discord_max_fields):
@@ -341,15 +339,15 @@
                 if not self._send(payload, attach=attachment):
                     # We failed to post our message
                     return False
 
         # Otherwise return
         return True
 
-    def _send(self, payload, attach=None, **kwargs):
+    def _send(self, payload, attach=None, params=None, **kwargs):
         """
         Wrapper to the requests (post) object
         """
 
         # Our headers
         headers = {
             'User-Agent': self.app_id,
@@ -392,14 +390,15 @@
                 files = {'file': (attach.name, open(attach.path, 'rb'))}
 
             else:
                 headers['Content-Type'] = 'application/json; charset=utf-8'
 
             r = requests.post(
                 notify_url,
+                params=params,
                 data=payload if files else dumps(payload),
                 headers=headers,
                 files=files,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
             if r.status_code not in (
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyEmail.py` & `apprise-1.4.0/apprise/plugins/NotifyEmail.py`

 * *Files 2% similar despite different names*

```diff
@@ -995,14 +995,21 @@
             targets='' if not has_targets else '/'.join(
                 [NotifyEmail.quote('{}{}'.format(
                     '' if not e[0] else '{}:'.format(e[0]), e[1]),
                     safe='') for e in self.targets]),
             params=NotifyEmail.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyEmby.py` & `apprise-1.4.0/apprise/plugins/NotifyEmby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyEnigma2.py` & `apprise-1.4.0/apprise/plugins/NotifyEnigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFCM/__init__.py` & `apprise-1.4.0/apprise/plugins/NotifyFCM/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -551,14 +551,20 @@
             schema=self.secure_protocol,
             reference=reference,
             targets='/'.join(
                 [NotifyFCM.quote(x) for x in self.targets]),
             params=NotifyFCM.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFCM/color.py` & `apprise-1.4.0/apprise/plugins/NotifyFCM/color.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFCM/common.py` & `apprise-1.4.0/apprise/plugins/NotifyFCM/common.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFCM/oauth.py` & `apprise-1.4.0/apprise/plugins/NotifyFCM/oauth.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFCM/priority.py` & `apprise-1.4.0/apprise/plugins/NotifyFCM/priority.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFaast.py` & `apprise-1.4.0/apprise/plugins/NotifyFaast.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyFlock.py` & `apprise-1.4.0/apprise/plugins/NotifyFlock.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,21 @@
                 token=self.pprint(self.token, privacy, safe=''),
                 targets='/'.join(
                     [NotifyFlock.quote(target, safe='')
                      for target in self.targets]),
                 params=NotifyFlock.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
         """
         results = NotifyBase.parse_url(url, verify_host=False)
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyForm.py` & `apprise-1.4.0/apprise/plugins/NotifyForm.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,24 @@
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyImageSize
 from ..common import NotifyType
 from ..AppriseLocale import gettext_lazy as _
 
 
+class FORMPayloadField:
+    """
+    Identifies the fields available in the FORM Payload
+    """
+    VERSION = 'version'
+    TITLE = 'title'
+    MESSAGE = 'message'
+    MESSAGETYPE = 'type'
+
+
 # Defines the method to send the notification
 METHODS = (
     'POST',
     'GET',
     'DELETE',
     'PUT',
     'HEAD',
@@ -92,14 +102,20 @@
     # Allows the user to specify the NotifyImageSize object
     image_size = NotifyImageSize.XY_128
 
     # Disable throttle rate for Form requests since they are normally
     # local anyway
     request_rate_per_sec = 0
 
+    # Define the FORM version to place in all payloads
+    # Version: Major.Minor,  Major is only updated if the entire schema is
+    # changed. If just adding new items (or removing old ones, only increment
+    # the Minor!
+    form_version = '1.0'
+
     # Define object templates
     templates = (
         '{schema}://{host}',
         '{schema}://{host}:{port}',
         '{schema}://{user}@{host}',
         '{schema}://{user}@{host}:{port}',
         '{schema}://{user}:{password}@{host}',
@@ -214,28 +230,50 @@
 
             else:  # result.group('match2'):
                 self.attach_as += result.group('id2')
                 if result.group('wc2'):
                     self.attach_as += self.attach_as_count
                     self.attach_multi_support = True
 
+        # A payload map allows users to over-ride the default mapping if
+        # they're detected with the :overide=value.  Normally this would
+        # create a new key and assign it the value specified.  However
+        # if the key you specify is actually an internally mapped one,
+        # then a re-mapping takes place using the value
+        self.payload_map = {
+            FORMPayloadField.VERSION: FORMPayloadField.VERSION,
+            FORMPayloadField.TITLE: FORMPayloadField.TITLE,
+            FORMPayloadField.MESSAGE: FORMPayloadField.MESSAGE,
+            FORMPayloadField.MESSAGETYPE: FORMPayloadField.MESSAGETYPE,
+        }
+
         self.params = {}
         if params:
             # Store our extra headers
             self.params.update(params)
 
         self.headers = {}
         if headers:
             # Store our extra headers
             self.headers.update(headers)
 
+        self.payload_overrides = {}
         self.payload_extras = {}
         if payload:
             # Store our extra payload entries
             self.payload_extras.update(payload)
+            for key in list(self.payload_extras.keys()):
+                # Any values set in the payload to alter a system related one
+                # alters the system key.  Hence :message=msg maps the 'message'
+                # variable that otherwise already contains the payload to be
+                # 'msg' instead (containing the payload)
+                if key in self.payload_map:
+                    self.payload_map[key] = self.payload_extras[key]
+                    self.payload_overrides[key] = self.payload_extras[key]
+                    del self.payload_extras[key]
 
         return
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
@@ -253,14 +291,16 @@
 
         # Append our GET params into our parameters
         params.update({'-{}'.format(k): v for k, v in self.params.items()})
 
         # Append our payload extra's into our parameters
         params.update(
             {':{}'.format(k): v for k, v in self.payload_extras.items()})
+        params.update(
+            {':{}'.format(k): v for k, v in self.payload_overrides.items()})
 
         if self.attach_as != self.attach_as_default:
             # Provide Attach-As extension details
             params['attach-as'] = self.attach_as
 
         # Determine Authentication
         auth = ''
@@ -333,23 +373,26 @@
 
             if not self.attach_multi_support and no > 1:
                 self.logger.warning(
                     'Multiple attachments provided while '
                     'form:// Multi-Attachment Support not enabled')
 
         # prepare Form Object
-        payload = {
-            # Version: Major.Minor,  Major is only updated if the entire
-            # schema is changed. If just adding new items (or removing
-            # old ones, only increment the Minor!
-            'version': '1.0',
-            'title': title,
-            'message': body,
-            'type': notify_type,
-        }
+        payload = {}
+
+        for key, value in (
+                (FORMPayloadField.VERSION, self.form_version),
+                (FORMPayloadField.TITLE, title),
+                (FORMPayloadField.MESSAGE, body),
+                (FORMPayloadField.MESSAGETYPE, notify_type)):
+
+            if not self.payload_map[key]:
+                # Do not store element in payload response
+                continue
+            payload[self.payload_map[key]] = value
 
         # Apply any/all payload over-rides defined
         payload.update(self.payload_extras)
 
         auth = None
         if self.user:
             auth = (self.user, self.password)
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGitter.py` & `apprise-1.4.0/apprise/plugins/NotifyGitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,14 +385,20 @@
         return '{schema}://{token}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             token=self.pprint(self.token, privacy, safe=''),
             targets='/'.join(
                 [NotifyGitter.quote(x, safe='') for x in self.targets]),
             params=NotifyGitter.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGnome.py` & `apprise-1.4.0/apprise/plugins/NotifyGnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGoogleChat.py` & `apprise-1.4.0/apprise/plugins/NotifyGoogleChat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGotify.py` & `apprise-1.4.0/apprise/plugins/NotifyGotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGrowl.py` & `apprise-1.4.0/apprise/plugins/NotifyGrowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyGuilded.py` & `apprise-1.4.0/apprise/plugins/NotifyGuilded.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyHomeAssistant.py` & `apprise-1.4.0/apprise/plugins/NotifyHomeAssistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyIFTTT.py` & `apprise-1.4.0/apprise/plugins/NotifyIFTTT.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,20 @@
             schema=self.secure_protocol,
             webhook_id=self.pprint(self.webhook_id, privacy, safe=''),
             events='/'.join([NotifyIFTTT.quote(x, safe='')
                              for x in self.events]),
             params=NotifyIFTTT.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.events)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyJSON.py` & `apprise-1.4.0/apprise/plugins/NotifyJSON.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,25 @@
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyImageSize
 from ..common import NotifyType
 from ..AppriseLocale import gettext_lazy as _
 
 
+class JSONPayloadField:
+    """
+    Identifies the fields available in the JSON Payload
+    """
+    VERSION = 'version'
+    TITLE = 'title'
+    MESSAGE = 'message'
+    ATTACHMENTS = 'attachments'
+    MESSAGETYPE = 'type'
+
+
 # Defines the method to send the notification
 METHODS = (
     'POST',
     'GET',
     'DELETE',
     'PUT',
     'HEAD',
@@ -72,14 +83,20 @@
     # Allows the user to specify the NotifyImageSize object
     image_size = NotifyImageSize.XY_128
 
     # Disable throttle rate for JSON requests since they are normally
     # local anyway
     request_rate_per_sec = 0
 
+    # Define the JSON version to place in all payloads
+    # Version: Major.Minor,  Major is only updated if the entire schema is
+    # changed. If just adding new items (or removing old ones, only increment
+    # the Minor!
+    json_version = '1.0'
+
     # Define object templates
     templates = (
         '{schema}://{host}',
         '{schema}://{host}:{port}',
         '{schema}://{user}@{host}',
         '{schema}://{user}@{host}:{port}',
         '{schema}://{user}:{password}@{host}',
@@ -158,28 +175,52 @@
             if not isinstance(method, str) else method.upper()
 
         if self.method not in METHODS:
             msg = 'The method specified ({}) is invalid.'.format(method)
             self.logger.warning(msg)
             raise TypeError(msg)
 
+        # A payload map allows users to over-ride the default mapping if
+        # they're detected with the :overide=value.  Normally this would
+        # create a new key and assign it the value specified.  However
+        # if the key you specify is actually an internally mapped one,
+        # then a re-mapping takes place using the value
+        self.payload_map = {
+            JSONPayloadField.VERSION: JSONPayloadField.VERSION,
+            JSONPayloadField.TITLE: JSONPayloadField.TITLE,
+            JSONPayloadField.MESSAGE: JSONPayloadField.MESSAGE,
+            JSONPayloadField.ATTACHMENTS: JSONPayloadField.ATTACHMENTS,
+            JSONPayloadField.MESSAGETYPE: JSONPayloadField.MESSAGETYPE,
+        }
+
         self.params = {}
         if params:
             # Store our extra headers
             self.params.update(params)
 
         self.headers = {}
         if headers:
             # Store our extra headers
             self.headers.update(headers)
 
+        self.payload_overrides = {}
         self.payload_extras = {}
         if payload:
             # Store our extra payload entries
             self.payload_extras.update(payload)
+            for key in list(self.payload_extras.keys()):
+                # Any values set in the payload to alter a system related one
+                # alters the system key.  Hence :message=msg maps the 'message'
+                # variable that otherwise already contains the payload to be
+                # 'msg' instead (containing the payload)
+                if key in self.payload_map:
+                    self.payload_map[key] = self.payload_extras[key].strip()
+                    self.payload_overrides[key] = \
+                        self.payload_extras[key].strip()
+                    del self.payload_extras[key]
 
         return
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
@@ -197,14 +238,16 @@
 
         # Append our GET params into our parameters
         params.update({'-{}'.format(k): v for k, v in self.params.items()})
 
         # Append our payload extra's into our parameters
         params.update(
             {':{}'.format(k): v for k, v in self.payload_extras.items()})
+        params.update(
+            {':{}'.format(k): v for k, v in self.payload_overrides.items()})
 
         # Determine Authentication
         auth = ''
         if self.user and self.password:
             auth = '{user}:{password}@'.format(
                 user=NotifyJSON.quote(self.user, safe=''),
                 password=self.pprint(
@@ -271,24 +314,26 @@
                     self.logger.warning(
                         'An I/O error occurred while reading {}.'.format(
                             attachment.name if attachment else 'attachment'))
                     self.logger.debug('I/O Exception: %s' % str(e))
                     return False
 
         # prepare JSON Object
-        payload = {
-            # Version: Major.Minor,  Major is only updated if the entire
-            # schema is changed. If just adding new items (or removing
-            # old ones, only increment the Minor!
-            'version': '1.0',
-            'title': title,
-            'message': body,
-            'attachments': attachments,
-            'type': notify_type,
-        }
+        payload = {}
+        for key, value in (
+                (JSONPayloadField.VERSION, self.json_version),
+                (JSONPayloadField.TITLE, title),
+                (JSONPayloadField.MESSAGE, body),
+                (JSONPayloadField.ATTACHMENTS, attachments),
+                (JSONPayloadField.MESSAGETYPE, notify_type)):
+
+            if not self.payload_map[key]:
+                # Do not store element in payload response
+                continue
+            payload[self.payload_map[key]] = value
 
         # Apply any/all payload over-rides defined
         payload.update(self.payload_extras)
 
         auth = None
         if self.user:
             auth = (self.user, self.password)
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyJoin.py` & `apprise-1.4.0/apprise/plugins/NotifyJoin.py`

 * *Files 2% similar despite different names*

```diff
@@ -369,14 +369,20 @@
         return '{schema}://{apikey}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='/'.join([NotifyJoin.quote(x, safe='')
                               for x in self.targets]),
             params=NotifyJoin.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyKavenegar.py` & `apprise-1.4.0/apprise/plugins/NotifyKavenegar.py`

 * *Files 2% similar despite different names*

```diff
@@ -320,14 +320,20 @@
             schema=self.secure_protocol,
             source='' if not self.source else '{}@'.format(self.source),
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='/'.join(
                 [NotifyKavenegar.quote(x, safe='') for x in self.targets]),
             params=NotifyKavenegar.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyKumulos.py` & `apprise-1.4.0/apprise/plugins/NotifyKumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyLametric.py` & `apprise-1.4.0/apprise/plugins/NotifyLametric.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyLine.py` & `apprise-1.4.0/apprise/plugins/NotifyLine.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,20 @@
             token=self.pprint(
                 self.token, privacy, mode=PrivacyMode.Secret, safe=''),
             targets='/'.join(
                 [self.pprint(x, privacy, safe='') for x in self.targets]),
             params=NotifyLine.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMQTT.py` & `apprise-1.4.0/apprise/plugins/NotifyMQTT.py`

 * *Files 1% similar despite different names*

```diff
@@ -472,14 +472,20 @@
             port='' if self.port is None or self.port == default_port
                  else ':{}'.format(self.port),
             targets=','.join(
                 [NotifyMQTT.quote(x, safe='/') for x in self.topics]),
             params=NotifyMQTT.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.topics)
+
     @staticmethod
     def parse_url(url):
         """
         There are no parameters nessisary for this protocol; simply having
         windows:// is all you need.  This function just makes sure that
         is in place.
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMSG91.py` & `apprise-1.4.0/apprise/plugins/NotifyMSG91.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,20 @@
         return '{schema}://{authkey}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             authkey=self.pprint(self.authkey, privacy, safe=''),
             targets='/'.join(
                 [NotifyMSG91.quote(x, safe='') for x in self.targets]),
             params=NotifyMSG91.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMSTeams.py` & `apprise-1.4.0/apprise/plugins/NotifyMSTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMacOSX.py` & `apprise-1.4.0/apprise/plugins/NotifyMacOSX.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMailgun.py` & `apprise-1.4.0/apprise/plugins/NotifyMailgun.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,14 +623,28 @@
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='' if not has_targets else '/'.join(
                 [NotifyMailgun.quote('{}{}'.format(
                     '' if not e[0] else '{}:'.format(e[0]), e[1]),
                     safe='') for e in self.targets]),
             params=NotifyMailgun.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMastodon.py` & `apprise-1.4.0/apprise/plugins/NotifyMastodon.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,14 +374,21 @@
             port='' if self.port is None or self.port == default_port
                  else ':{}'.format(self.port),
             targets='/'.join(
                 [NotifyMastodon.quote(x, safe='@') for x in self.targets]),
             params=NotifyMastodon.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     def send(self, body, title='', notify_type=NotifyType.INFO, attach=None,
              **kwargs):
         """
         wrapper to _send since we can alert more then one channel
         """
 
         # Build a list of our attachments
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMatrix.py` & `apprise-1.4.0/apprise/plugins/NotifyMatrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -1192,14 +1192,21 @@
             else self.pprint(self.access_token, privacy, safe=''),
             port='' if self.port is None
             or self.port == default_port else ':{}'.format(self.port),
             rooms=NotifyMatrix.quote('/'.join(self.rooms)),
             params=NotifyMatrix.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.rooms)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMattermost.py` & `apprise-1.4.0/apprise/plugins/NotifyMattermost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMessageBird.py` & `apprise-1.4.0/apprise/plugins/NotifyMessageBird.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,14 +307,21 @@
             schema=self.secure_protocol,
             apikey=self.pprint(self.apikey, privacy, safe=''),
             source=self.source,
             targets='/'.join(
                 [NotifyMessageBird.quote(x, safe='') for x in self.targets]),
             params=NotifyMessageBird.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyMisskey.py` & `apprise-1.4.0/apprise/plugins/NotifyMisskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyNextcloud.py` & `apprise-1.4.0/apprise/plugins/NotifyNextcloud.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,14 +308,20 @@
                    port='' if self.port is None or self.port == default_port
                         else ':{}'.format(self.port),
                    targets='/'.join([NotifyNextcloud.quote(x)
                                      for x in self.targets]),
                    params=NotifyNextcloud.urlencode(params),
                )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyNextcloudTalk.py` & `apprise-1.4.0/apprise/plugins/NotifyNextcloudTalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -259,14 +259,20 @@
                    hostname=self.host,
                    port='' if self.port is None or self.port == default_port
                         else ':{}'.format(self.port),
                    targets='/'.join([NotifyNextcloudTalk.quote(x)
                                      for x in self.targets]),
                )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyNotica.py` & `apprise-1.4.0/apprise/plugins/NotifyNotica.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyNotifico.py` & `apprise-1.4.0/apprise/plugins/NotifyNotifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyNtfy.py` & `apprise-1.4.0/apprise/plugins/NotifyNtfy.py`

 * *Files 1% similar despite different names*

```diff
@@ -694,14 +694,20 @@
             return '{schema}://{targets}?{params}'.format(
                 schema=self.secure_protocol,
                 targets='/'.join(
                     [NotifyNtfy.quote(x, safe='') for x in self.topics]),
                 params=NotifyNtfy.urlencode(params)
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.topics)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
         """
         results = NotifyBase.parse_url(url, verify_host=False)
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyOffice365.py` & `apprise-1.4.0/apprise/plugins/NotifyOffice365.py`

 * *Files 2% similar despite different names*

```diff
@@ -592,14 +592,20 @@
                     safe=''),
                 targets='/'.join(
                     [NotifyOffice365.quote('{}{}'.format(
                         '' if not e[0] else '{}:'.format(e[0]), e[1]),
                         safe='') for e in self.targets]),
                 params=NotifyOffice365.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyOneSignal.py` & `apprise-1.4.0/apprise/plugins/NotifyOneSignal.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 from ..utils import validate_regex
 from ..utils import parse_list
 from ..utils import parse_bool
 from ..utils import is_email
 from ..AppriseLocale import gettext_lazy as _
 
 
-class OneSignalCategory(NotifyBase):
+class OneSignalCategory:
     """
     We define the different category types that we can notify via OneSignal
     """
     PLAYER = 'include_player_ids'
     EMAIL = 'include_email_tokens'
     USER = 'include_external_user_ids'
     SEGMENT = 'included_segments'
@@ -88,15 +88,15 @@
     # Notification
     notify_url = "https://onesignal.com/api/v1/notifications"
 
     # Allows the user to specify the NotifyImageSize object
     image_size = NotifyImageSize.XY_72
 
     # The maximum allowable batch sizes per message
-    maximum_batch_size = 2000
+    default_batch_size = 2000
 
     # Define object templates
     templates = (
         '{schema}://{app}@{apikey}/{targets}',
         '{schema}://{template}:{app}@{apikey}/{targets}',
     )
 
@@ -117,15 +117,15 @@
         },
         'apikey': {
             'name': _('API Key'),
             'type': 'string',
             'private': True,
             'required': True,
         },
-        'target_device': {
+        'target_player': {
             'name': _('Target Player ID'),
             'type': 'string',
             'map_to': 'targets',
         },
         'target_email': {
             'name': _('Target Email'),
             'type': 'string',
@@ -200,15 +200,15 @@
         if not self.app:
             msg = 'An invalid OneSignal Application ID ' \
                   '({}) was specified.'.format(app)
             self.logger.warning(msg)
             raise TypeError(msg)
 
         # Prepare Batch Mode Flag
-        self.batch_size = self.maximum_batch_size if batch else 1
+        self.batch_size = self.default_batch_size if batch else 1
 
         # Place a thumbnail image inline with the message body
         self.include_image = include_image
 
         # Our Assorted Types of Targets
         self.targets = {
             OneSignalCategory.PLAYER: [],
@@ -428,14 +428,34 @@
                 [NotifyOneSignal.quote('{}{}'.format(
                     NotifyOneSignal.template_tokens
                     ['target_segment']['prefix'], x), safe='')
                     for x in self.targets[OneSignalCategory.SEGMENT]])),
             params=NotifyOneSignal.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        if self.batch_size > 1:
+            # Batches can only be sent by group (you can't combine groups into
+            # a single batch)
+            total_targets = 0
+            for k, m in self.targets.items():
+                targets = len(m)
+                total_targets += int(targets / self.batch_size) + \
+                    (1 if targets % self.batch_size else 0)
+            return total_targets
+
+        # Normal batch count; just count the targets
+        return sum([len(m) for _, m in self.targets.items()])
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyOpsgenie.py` & `apprise-1.4.0/apprise/plugins/NotifyOpsgenie.py`

 * *Files 1% similar despite different names*

```diff
@@ -168,15 +168,15 @@
     # the body directive
     opsgenie_body_minlen = 130
 
     # The default region to use if one isn't otherwise specified
     opsgenie_default_region = OpsgenieRegion.US
 
     # The maximum allowable targets within a notification
-    maximum_batch_size = 50
+    default_batch_size = 50
 
     # Define object templates
     templates = (
         '{schema}://{apikey}',
         '{schema}://{apikey}/{targets}',
     )
 
@@ -304,15 +304,15 @@
 
         self.details = {}
         if details:
             # Store our extra details
             self.details.update(details)
 
         # Prepare Batch Mode Flag
-        self.batch_size = self.maximum_batch_size if batch else 1
+        self.batch_size = self.default_batch_size if batch else 1
 
         # Assign our tags (if defined)
         self.__tags = parse_list(tags)
 
         # Assign our entity (if defined)
         self.entity = entity
 
@@ -532,14 +532,28 @@
             targets='/'.join(
                 [NotifyOpsgenie.quote('{}{}'.format(
                     __map[x['type']],
                     x.get('id', x.get('name', x.get('username')))))
                     for x in self.targets]),
             params=NotifyOpsgenie.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        targets = len(self.targets)
+        if self.batch_size > 1:
+            targets = int(targets / self.batch_size) + \
+                (1 if targets % self.batch_size else 0)
+
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPagerDuty.py` & `apprise-1.4.0/apprise/plugins/NotifyPagerDuty.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPagerTree.py` & `apprise-1.4.0/apprise/plugins/NotifyPagerTree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyParsePlatform.py` & `apprise-1.4.0/apprise/plugins/NotifyParsePlatform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPopcornNotify.py` & `apprise-1.4.0/apprise/plugins/NotifyPopcornNotify.py`

 * *Files 2% similar despite different names*

```diff
@@ -261,14 +261,29 @@
         return '{schema}://{apikey}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='/'.join(
                 [NotifyPopcornNotify.quote(x, safe='') for x in self.targets]),
             params=NotifyPopcornNotify.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyProwl.py` & `apprise-1.4.0/apprise/plugins/NotifyProwl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPushBullet.py` & `apprise-1.4.0/apprise/plugins/NotifyPushBullet.py`

 * *Files 2% similar despite different names*

```diff
@@ -402,14 +402,20 @@
 
         return '{schema}://{accesstoken}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             accesstoken=self.pprint(self.accesstoken, privacy, safe=''),
             targets=targets,
             params=NotifyPushBullet.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPushSafer.py` & `apprise-1.4.0/apprise/plugins/NotifyPushSafer.py`

 * *Files 0% similar despite different names*

```diff
@@ -790,14 +790,20 @@
 
         return '{schema}://{privatekey}/{targets}?{params}'.format(
             schema=self.secure_protocol if self.secure else self.protocol,
             privatekey=self.pprint(self.privatekey, privacy, safe=''),
             targets=targets,
             params=NotifyPushSafer.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPushed.py` & `apprise-1.4.0/apprise/plugins/NotifyPushed.py`

 * *Files 1% similar despite different names*

```diff
@@ -325,14 +325,21 @@
                     # Channels are prefixed with a pound/hashtag symbol
                     ['#{}'.format(x) for x in self.channels],
                     # Users are prefixed with an @ symbol
                     ['@{}'.format(x) for x in self.users],
                 )]),
             params=NotifyPushed.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.channels) + len(self.users)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPushjet.py` & `apprise-1.4.0/apprise/plugins/NotifyPushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyPushover.py` & `apprise-1.4.0/apprise/plugins/NotifyPushover.py`

 * *Files 2% similar despite different names*

```diff
@@ -573,14 +573,20 @@
         return '{schema}://{user_key}@{token}/{devices}/?{params}'.format(
             schema=self.secure_protocol,
             user_key=self.pprint(self.user_key, privacy, safe=''),
             token=self.pprint(self.token, privacy, safe=''),
             devices=devices,
             params=NotifyPushover.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyReddit.py` & `apprise-1.4.0/apprise/plugins/NotifyReddit.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,20 @@
                     self.client_secret, privacy, mode=PrivacyMode.Secret,
                     safe=''),
                 targets='/'.join(
                     [NotifyReddit.quote(x, safe='') for x in self.subreddits]),
                 params=NotifyReddit.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.subreddits)
+
     def login(self):
         """
         A simple wrapper to authenticate with the Reddit Server
         """
 
         # Prepare our payload
         payload = {
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyRocketChat.py` & `apprise-1.4.0/apprise/plugins/NotifyRocketChat.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,14 +344,21 @@
                     self.rooms,
                     # Users
                     ['@{}'.format(x) for x in self.users],
                 )]),
             params=NotifyRocketChat.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.channels) + len(self.rooms) + len(self.users)
+        return targets if targets > 0 else 1
+
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
         wrapper to _send since we can alert more then one channel
         """
 
         # Call the _send_ function applicable to whatever mode we're in
         # - calls _send_webhook_notification if the mode variable is set
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyRyver.py` & `apprise-1.4.0/apprise/plugins/NotifyXBMC.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,336 +26,363 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-# To use this plugin, you need to first generate a webhook.
-
-# When you're complete, you will recieve a URL that looks something like this:
-#                https://apprise.ryver.com/application/webhook/ckhrjW8w672m6HG
-#                          ^                                        ^
-#                          |                                        |
-#  These are important <---^----------------------------------------^
-#
-import re
 import requests
 from json import dumps
 
 from .NotifyBase import NotifyBase
-from ..common import NotifyImageSize
+from ..URLBase import PrivacyMode
 from ..common import NotifyType
+from ..common import NotifyImageSize
 from ..utils import parse_bool
-from ..utils import validate_regex
 from ..AppriseLocale import gettext_lazy as _
 
 
-class RyverWebhookMode:
+class NotifyXBMC(NotifyBase):
     """
-    Ryver supports to webhook modes
+    A wrapper for XBMC/KODI Notifications
     """
-    SLACK = 'slack'
-    RYVER = 'ryver'
 
+    # The default descriptive name associated with the Notification
+    service_name = 'Kodi/XBMC'
 
-# Define the types in a list for validation purposes
-RYVER_WEBHOOK_MODES = (
-    RyverWebhookMode.SLACK,
-    RyverWebhookMode.RYVER,
-)
+    # The services URL
+    service_url = 'http://kodi.tv/'
 
+    xbmc_protocol = 'xbmc'
+    xbmc_secure_protocol = 'xbmcs'
+    kodi_protocol = 'kodi'
+    kodi_secure_protocol = 'kodis'
 
-class NotifyRyver(NotifyBase):
-    """
-    A wrapper for Ryver Notifications
-    """
+    # The default protocols
+    protocol = (xbmc_protocol, kodi_protocol)
 
-    # The default descriptive name associated with the Notification
-    service_name = 'Ryver'
+    # The default secure protocols
+    secure_protocol = (xbmc_secure_protocol, kodi_secure_protocol)
 
-    # The services URL
-    service_url = 'https://ryver.com/'
+    # A URL that takes you to the setup/help of the specific protocol
+    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_kodi'
 
-    # The default secure protocol
-    secure_protocol = 'ryver'
+    # Disable throttle rate for XBMC/KODI requests since they are normally
+    # local anyway
+    request_rate_per_sec = 0
+
+    # Limit results to just the first 2 line otherwise there is just to much
+    # content to display
+    body_max_line_count = 2
 
-    # A URL that takes you to the setup/help of the specific protocol
-    setup_url = 'https://github.com/caronc/apprise/wiki/Notify_ryver'
+    # XBMC uses the http protocol with JSON requests
+    xbmc_default_port = 8080
 
     # Allows the user to specify the NotifyImageSize object
-    image_size = NotifyImageSize.XY_72
+    image_size = NotifyImageSize.XY_128
+
+    # XBMC default protocol version (v2)
+    xbmc_remote_protocol = 2
 
-    # The maximum allowable characters allowed in the body per message
-    body_maxlen = 1000
+    # KODI default protocol version (v6)
+    kodi_remote_protocol = 6
 
     # Define object templates
     templates = (
-        '{schema}://{organization}/{token}',
-        '{schema}://{user}@{organization}/{token}',
+        '{schema}://{host}',
+        '{schema}://{host}:{port}',
+        '{schema}://{user}:{password}@{host}',
+        '{schema}://{user}:{password}@{host}:{port}',
     )
 
-    # Define our template tokens
+    # Define our tokens
     template_tokens = dict(NotifyBase.template_tokens, **{
-        'organization': {
-            'name': _('Organization'),
+        'host': {
+            'name': _('Hostname'),
             'type': 'string',
             'required': True,
-            'regex': (r'^[A-Z0-9_-]{3,32}$', 'i'),
         },
-        'token': {
-            'name': _('Token'),
-            'type': 'string',
-            'required': True,
-            'private': True,
-            'regex': (r'^[A-Z0-9]{15}$', 'i'),
+        'port': {
+            'name': _('Port'),
+            'type': 'int',
+            'min': 1,
+            'max': 65535,
         },
         'user': {
-            'name': _('Bot Name'),
+            'name': _('Username'),
+            'type': 'string',
+        },
+        'password': {
+            'name': _('Password'),
             'type': 'string',
+            'private': True,
         },
     })
 
     # Define our template arguments
     template_args = dict(NotifyBase.template_args, **{
-        'mode': {
-            'name': _('Webhook Mode'),
-            'type': 'choice:string',
-            'values': RYVER_WEBHOOK_MODES,
-            'default': RyverWebhookMode.RYVER,
+        'duration': {
+            'name': _('Duration'),
+            'type': 'int',
+            'min': 1,
+            'default': 12,
         },
         'image': {
             'name': _('Include Image'),
             'type': 'bool',
             'default': True,
             'map_to': 'include_image',
         },
     })
 
-    def __init__(self, organization, token, mode=RyverWebhookMode.RYVER,
-                 include_image=True, **kwargs):
+    def __init__(self, include_image=True, duration=None, **kwargs):
         """
-        Initialize Ryver Object
+        Initialize XBMC/KODI Object
         """
         super().__init__(**kwargs)
 
-        # API Token (associated with project)
-        self.token = validate_regex(
-            token, *self.template_tokens['token']['regex'])
-        if not self.token:
-            msg = 'An invalid Ryver API Token ' \
-                  '({}) was specified.'.format(token)
-            self.logger.warning(msg)
-            raise TypeError(msg)
-
-        # Organization (associated with project)
-        self.organization = validate_regex(
-            organization, *self.template_tokens['organization']['regex'])
-        if not self.organization:
-            msg = 'An invalid Ryver Organization ' \
-                  '({}) was specified.'.format(organization)
-            self.logger.warning(msg)
-            raise TypeError(msg)
-
-        # Store our webhook mode
-        self.mode = None \
-            if not isinstance(mode, str) else mode.lower()
-
-        if self.mode not in RYVER_WEBHOOK_MODES:
-            msg = 'The Ryver webhook mode specified ({}) is invalid.' \
-                .format(mode)
-            self.logger.warning(msg)
-            raise TypeError(msg)
+        # Number of seconds to display notification for
+        self.duration = self.template_args['duration']['default'] \
+            if not (isinstance(duration, int) and
+                    self.template_args['duration']['min'] > 0) else duration
 
-        # Place an image inline with the message body
-        self.include_image = include_image
+        # Build our schema
+        self.schema = 'https' if self.secure else 'http'
 
-        # Slack formatting requirements are defined here which Ryver supports:
-        # https://api.slack.com/docs/message-formatting
-        self._re_formatting_map = {
-            # New lines must become the string version
-            r'\r\*\n': '\\n',
-            # Escape other special characters
-            r'&': '&amp;',
-            r'<': '&lt;',
-            r'>': '&gt;',
+        # Prepare the default header
+        self.headers = {
+            'User-Agent': self.app_id,
+            'Content-Type': 'application/json'
         }
 
-        # Iterate over above list and store content accordingly
-        self._re_formatting_rules = re.compile(
-            r'(' + '|'.join(self._re_formatting_map.keys()) + r')',
-            re.IGNORECASE,
-        )
+        # Default protocol
+        self.protocol = kwargs.get('protocol', self.xbmc_remote_protocol)
 
-        return
+        # Track whether or not we want to send an image with our notification
+        # or not.
+        self.include_image = include_image
 
-    def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
+    def _payload_60(self, title, body, notify_type, **kwargs):
         """
-        Perform Ryver Notification
+        Builds payload for KODI API v6.0
+
+        Returns (headers, payload)
         """
 
-        headers = {
-            'User-Agent': self.app_id,
-            'Content-Type': 'application/json',
+        # prepare JSON Object
+        payload = {
+            'jsonrpc': '2.0',
+            'method': 'GUI.ShowNotification',
+            'params': {
+                'title': title,
+                'message': body,
+                # displaytime is defined in microseconds so we need to just
+                # do some simple math
+                'displaytime': int(self.duration * 1000),
+            },
+            'id': 1,
         }
 
-        if self.mode == RyverWebhookMode.SLACK:
-            # Perform Slack formatting
-            title = self._re_formatting_rules.sub(  # pragma: no branch
-                lambda x: self._re_formatting_map[x.group()], title,
-            )
-            body = self._re_formatting_rules.sub(  # pragma: no branch
-                lambda x: self._re_formatting_map[x.group()], body,
-            )
+        # Acquire our image url if configured to do so
+        image_url = None if not self.include_image else \
+            self.image_url(notify_type)
 
-        url = 'https://{}.ryver.com/application/webhook/{}'.format(
-            self.organization,
-            self.token,
-        )
+        if image_url:
+            payload['params']['image'] = image_url
+            if notify_type is NotifyType.FAILURE:
+                payload['type'] = 'error'
+
+            elif notify_type is NotifyType.WARNING:
+                payload['type'] = 'warning'
+
+            else:
+                payload['type'] = 'info'
+
+        return (self.headers, dumps(payload))
+
+    def _payload_20(self, title, body, notify_type, **kwargs):
+        """
+        Builds payload for XBMC API v2.0
+
+        Returns (headers, payload)
+        """
 
         # prepare JSON Object
         payload = {
-            'body': body if not title else '**{}**\r\n{}'.format(title, body),
-            'createSource': {
-                'displayName': self.user,
-                'avatar': None,
+            'jsonrpc': '2.0',
+            'method': 'GUI.ShowNotification',
+            'params': {
+                'title': title,
+                'message': body,
+                # displaytime is defined in microseconds so we need to just
+                # do some simple math
+                'displaytime': int(self.duration * 1000),
             },
+            'id': 1,
         }
 
-        # Acquire our image url if configured to do so
-        image_url = None if not self.include_image else \
-            self.image_url(notify_type)
+        # Include our logo if configured to do so
+        image_url = None if not self.include_image \
+            else self.image_url(notify_type)
 
         if image_url:
-            payload['createSource']['avatar'] = image_url
+            payload['params']['image'] = image_url
+
+        return (self.headers, dumps(payload))
+
+    def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
+        """
+        Perform XBMC/KODI Notification
+        """
+
+        if self.protocol == self.xbmc_remote_protocol:
+            # XBMC v2.0
+            (headers, payload) = self._payload_20(
+                title, body, notify_type, **kwargs)
+
+        else:
+            # KODI v6.0
+            (headers, payload) = self._payload_60(
+                title, body, notify_type, **kwargs)
+
+        auth = None
+        if self.user:
+            auth = (self.user, self.password)
 
-        self.logger.debug('Ryver POST URL: %s (cert_verify=%r)' % (
+        url = '%s://%s' % (self.schema, self.host)
+        if self.port:
+            url += ':%d' % self.port
+
+        url += '/jsonrpc'
+
+        self.logger.debug('XBMC/KODI POST URL: %s (cert_verify=%r)' % (
             url, self.verify_certificate,
         ))
-        self.logger.debug('Ryver Payload: %s' % str(payload))
+        self.logger.debug('XBMC/KODI Payload: %s' % str(payload))
 
         # Always call throttle before any remote server i/o is made
         self.throttle()
 
         try:
             r = requests.post(
                 url,
-                data=dumps(payload),
+                data=payload,
                 headers=headers,
+                auth=auth,
                 verify=self.verify_certificate,
                 timeout=self.request_timeout,
             )
-
             if r.status_code != requests.codes.ok:
                 # We had a problem
                 status_str = \
-                    NotifyBase.http_response_code_lookup(r.status_code)
+                    NotifyXBMC.http_response_code_lookup(r.status_code)
 
                 self.logger.warning(
-                    'Failed to send Ryver notification: '
+                    'Failed to send XBMC/KODI notification: '
                     '{}{}error={}.'.format(
                         status_str,
                         ', ' if status_str else '',
                         r.status_code))
 
                 self.logger.debug('Response Details:\r\n{}'.format(r.content))
 
                 # Return; we're done
                 return False
 
             else:
-                self.logger.info('Sent Ryver notification.')
+                self.logger.info('Sent XBMC/KODI notification.')
 
         except requests.RequestException as e:
             self.logger.warning(
-                'A Connection error occurred sending Ryver:%s ' % (
-                    self.organization) + 'notification.'
+                'A Connection error occurred sending XBMC/KODI '
+                'notification.'
             )
             self.logger.debug('Socket Exception: %s' % str(e))
+
+            # Return; we're done
             return False
 
         return True
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
         # Define any URL parameters
         params = {
             'image': 'yes' if self.include_image else 'no',
-            'mode': self.mode,
+            'duration': str(self.duration),
         }
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
-        # Determine if there is a botname present
-        botname = ''
-        if self.user:
-            botname = '{botname}@'.format(
-                botname=NotifyRyver.quote(self.user, safe=''),
+        # Determine Authentication
+        auth = ''
+        if self.user and self.password:
+            auth = '{user}:{password}@'.format(
+                user=NotifyXBMC.quote(self.user, safe=''),
+                password=self.pprint(
+                    self.password, privacy, mode=PrivacyMode.Secret, safe=''),
+            )
+        elif self.user:
+            auth = '{user}@'.format(
+                user=NotifyXBMC.quote(self.user, safe=''),
             )
 
-        return '{schema}://{botname}{organization}/{token}/?{params}'.format(
-            schema=self.secure_protocol,
-            botname=botname,
-            organization=NotifyRyver.quote(self.organization, safe=''),
-            token=self.pprint(self.token, privacy, safe=''),
-            params=NotifyRyver.urlencode(params),
+        default_schema = self.xbmc_protocol if (
+            self.protocol <= self.xbmc_remote_protocol) else self.kodi_protocol
+        default_port = 443 if self.secure else self.xbmc_default_port
+        if self.secure:
+            # Append 's' to schema
+            default_schema += 's'
+
+        return '{schema}://{auth}{hostname}{port}/?{params}'.format(
+            schema=default_schema,
+            auth=auth,
+            # never encode hostname since we're expecting it to be a valid one
+            hostname=self.host,
+            port='' if not self.port or self.port == default_port
+                 else ':{}'.format(self.port),
+            params=NotifyXBMC.urlencode(params),
         )
 
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
-
-        results = NotifyBase.parse_url(url, verify_host=False)
+        results = NotifyBase.parse_url(url)
         if not results:
-            # We're done early as we couldn't load the results
+            # We're done early
             return results
 
-        # The first token is stored in the hostname
-        results['organization'] = NotifyRyver.unquote(results['host'])
-
-        # Now fetch the remaining tokens
-        try:
-            results['token'] = \
-                NotifyRyver.split_path(results['fullpath'])[0]
-
-        except IndexError:
-            # no token
-            results['token'] = None
-
-        # Retrieve the mode
-        results['mode'] = results['qsd'].get('mode', RyverWebhookMode.RYVER)
+        # We want to set our protocol depending on whether we're using XBMC
+        # or KODI
+        if results.get('schema', '').startswith('xbmc'):
+            # XBMC Support
+            results['protocol'] = NotifyXBMC.xbmc_remote_protocol
+
+            # Assign Default XBMC Port
+            if not results['port']:
+                results['port'] = NotifyXBMC.xbmc_default_port
+
+        else:
+            # KODI Support
+            results['protocol'] = NotifyXBMC.kodi_remote_protocol
 
-        # use image= for consistency with the other plugins
+        # Include images with our message
         results['include_image'] = \
             parse_bool(results['qsd'].get('image', True))
 
-        return results
-
-    @staticmethod
-    def parse_native_url(url):
-        """
-        Support https://RYVER_ORG.ryver.com/application/webhook/TOKEN
-        """
+        # Set duration
+        try:
+            results['duration'] = abs(int(results['qsd'].get('duration')))
 
-        result = re.match(
-            r'^https?://(?P<org>[A-Z0-9_-]+)\.ryver\.com/application/webhook/'
-            r'(?P<webhook_token>[A-Z0-9]+)/?'
-            r'(?P<params>\?.+)?$', url, re.I)
-
-        if result:
-            return NotifyRyver.parse_url(
-                '{schema}://{org}/{webhook_token}/{params}'.format(
-                    schema=NotifyRyver.secure_protocol,
-                    org=result.group('org'),
-                    webhook_token=result.group('webhook_token'),
-                    params='' if not result.group('params')
-                    else result.group('params')))
+        except (TypeError, ValueError):
+            # Not a valid integer; ignore entry
+            pass
 
-        return None
+        return results
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySES.py` & `apprise-1.4.0/apprise/plugins/NotifySES.py`

 * *Files 1% similar despite different names*

```diff
@@ -812,14 +812,21 @@
                 targets='' if not has_targets else '/'.join(
                     [NotifySES.quote('{}{}'.format(
                         '' if not e[0] else '{}:'.format(e[0]), e[1]),
                         safe='') for e in self.targets]),
                 params=NotifySES.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySMSEagle.py` & `apprise-1.4.0/apprise/plugins/NotifySMSEagle.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,14 +69,30 @@
     'normal': SMSEaglePriority.NORMAL,
     # short for 'high'
     '+': SMSEaglePriority.HIGH,
     'high': SMSEaglePriority.HIGH,
 }
 
 
+class SMSEagleCategory:
+    """
+    We define the different category types that we can notify via SMS Eagle
+    """
+    PHONE = 'phone'
+    GROUP = 'group'
+    CONTACT = 'contact'
+
+
+SMSEAGLE_CATEGORIES = (
+    SMSEagleCategory.PHONE,
+    SMSEagleCategory.GROUP,
+    SMSEagleCategory.CONTACT,
+)
+
+
 class NotifySMSEagle(NotifyBase):
     """
     A wrapper for SMSEagle Notifications
     """
 
     # The default descriptive name associated with the Notification
     service_name = 'SMS Eagle'
@@ -399,32 +415,32 @@
             notify_url += ':%d' % self.port
         notify_url += self.notify_path
 
         # Send in batches if identified to do so
         batch_size = 1 if not self.batch else self.default_batch_size
 
         notify_by = {
-            'phone': {
+            SMSEagleCategory.PHONE: {
                 "method": "sms.send_sms",
                 'target': 'to',
             },
-            'group': {
+            SMSEagleCategory.GROUP: {
                 "method": "sms.send_togroup",
                 'target': 'groupname',
             },
-            'contact': {
+            SMSEagleCategory.CONTACT: {
                 "method": "sms.send_tocontact",
                 'target': 'contactname',
             },
         }
 
         # categories separated into a tuple since notify_by.keys()
         # returns an unpredicable list in Python 2.7 which causes
         # tests to fail every so often
-        for category in ('phone', 'group', 'contact'):
+        for category in SMSEAGLE_CATEGORIES:
             # Create a copy of our template
             payload = {
                 'method': notify_by[category]['method'],
                 'params': {
                     notify_by[category]['target']: None,
                 },
             }
@@ -592,14 +608,36 @@
                     ['#{}'.format(x) for x in self.target_groups],
                     # Pass along the same invalid entries as were provided
                     self.invalid_targets,
                 )]),
             params=NotifySMSEagle.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        if batch_size > 1:
+            # Batches can only be sent by group (you can't combine groups into
+            # a single batch)
+            total_targets = 0
+            for c in SMSEAGLE_CATEGORIES:
+                targets = len(getattr(self, f'target_{c}s'))
+                total_targets += int(targets / batch_size) + \
+                    (1 if targets % batch_size else 0)
+            return total_targets
+
+        # Normal batch count; just count the targets
+        return len(self.target_phones) + len(self.target_contacts) + \
+            len(self.target_groups)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySMTP2Go.py` & `apprise-1.4.0/apprise/plugins/NotifySMTP2Go.py`

 * *Files 2% similar despite different names*

```diff
@@ -509,14 +509,29 @@
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='' if not has_targets else '/'.join(
                 [NotifySMTP2Go.quote('{}{}'.format(
                     '' if not e[0] else '{}:'.format(e[0]), e[1]),
                     safe='') for e in self.targets]),
             params=NotifySMTP2Go.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySNS.py` & `apprise-1.4.0/apprise/plugins/NotifySNS.py`

 * *Files 1% similar despite different names*

```diff
@@ -596,14 +596,20 @@
                         self.phone,
                         # Topics are prefixed with a pound/hashtag symbol
                         ['#{}'.format(x) for x in self.topics],
                     )]),
                 params=NotifySNS.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.phone) + len(self.topics)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySendGrid.py` & `apprise-1.4.0/apprise/plugins/NotifySendGrid.py`

 * *Files 2% similar despite different names*

```diff
@@ -283,14 +283,20 @@
             # never encode email since it plays a huge role in our hostname
             from_email=self.from_email,
             targets='' if not has_targets else '/'.join(
                 [NotifySendGrid.quote(x, safe='') for x in self.targets]),
             params=NotifySendGrid.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
         Perform SendGrid Notification
         """
 
         headers = {
             'User-Agent': self.app_id,
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyServerChan.py` & `apprise-1.4.0/apprise/plugins/NotifyServerChan.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifySignalAPI.py` & `apprise-1.4.0/apprise/plugins/NotifySignalAPI.py`

 * *Files 3% similar despite different names*

```diff
@@ -427,14 +427,29 @@
                  else ':{}'.format(self.port),
             src=self.source,
             dst='/'.join(
                 [NotifySignalAPI.quote(x, safe='@+') for x in targets]),
             params=NotifySignalAPI.urlencode(params),
         )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySimplePush.py` & `apprise-1.4.0/apprise/plugins/NotifySimplePush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifySinch.py` & `apprise-1.4.0/apprise/plugins/NotifySinch.py`

 * *Files 2% similar despite different names*

```diff
@@ -404,14 +404,21 @@
                 self.service_plan_id, privacy, mode=PrivacyMode.Tail, safe=''),
             token=self.pprint(self.api_token, privacy, safe=''),
             source=NotifySinch.quote(self.source, safe=''),
             targets='/'.join(
                 [NotifySinch.quote(x, safe='') for x in self.targets]),
             params=NotifySinch.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySlack.py` & `apprise-1.4.0/apprise/plugins/NotifySlack.py`

 * *Files 4% similar despite different names*

```diff
@@ -350,14 +350,21 @@
             r'\r\*\n': '\\n',
             # Escape other special characters
             r'&': '&amp;',
             r'<': '&lt;',
             r'>': '&gt;',
         }
 
+        # To notify a channel, one uses <!channel|channel>
+        self._re_channel_support = re.compile(
+            r'(?P<match>(?:<|\&lt;)?[ \t]*'
+            r'!(?P<channel>[^| \n]+)'
+            r'(?:[ \t]*\|[ \t]*(?:(?P<val>[^\n]+?)[ \t]*)?(?:>|\&gt;)'
+            r'|(?:>|\&gt;)))', re.IGNORECASE)
+
         # The markdown in slack isn't [desc](url), it's <url|desc>
         #
         # To accomodate this, we need to ensure we don't escape URLs that match
         self._re_url_support = re.compile(
             r'(?P<match>(?:<|\&lt;)?[ \t]*'
             r'(?P<url>(?:https?|mailto)://[^| \n]+)'
             r'(?:[ \t]*\|[ \t]*(?:(?P<val>[^\n]+?)[ \t]*)?(?:>|\&gt;)'
@@ -451,14 +458,29 @@
             # Legacy API Formatting
             #
             if self.notify_format == NotifyFormat.MARKDOWN:
                 body = self._re_formatting_rules.sub(  # pragma: no branch
                     lambda x: self._re_formatting_map[x.group()], body,
                 )
 
+                # Support <!channel|desc>, <!channel> entries
+                for match in self._re_channel_support.findall(body):
+                    # Swap back any ampersands previously updaated
+                    channel = match[1].strip()
+                    desc = match[2].strip()
+
+                    # Update our string
+                    body = re.sub(
+                        re.escape(match[0]),
+                        '<!{channel}|{desc}>'.format(
+                            channel=channel, desc=desc)
+                        if desc else '<!{channel}>'.format(channel=channel),
+                        body,
+                        re.IGNORECASE)
+
                 # Support <url|desc>, <url> entries
                 for match in self._re_url_support.findall(body):
                     # Swap back any ampersands previously updaated
                     url = match[1].replace('&amp;', '&')
                     desc = match[2].strip()
 
                     # Update our string
@@ -989,14 +1011,20 @@
                 botname=botname,
                 access_token=self.pprint(self.access_token, privacy, safe=''),
                 targets='/'.join(
                     [NotifySlack.quote(x, safe='') for x in self.channels]),
                 params=NotifySlack.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.channels)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySparkPost.py` & `apprise-1.4.0/apprise/plugins/NotifySparkPost.py`

 * *Files 2% similar despite different names*

```diff
@@ -718,14 +718,29 @@
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='' if not has_targets else '/'.join(
                 [NotifySparkPost.quote('{}{}'.format(
                     '' if not e[0] else '{}:'.format(e[0]), e[1]),
                     safe='') for e in self.targets]),
             params=NotifySparkPost.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        #
+        # Factor batch into calculation
+        #
+        batch_size = 1 if not self.batch else self.default_batch_size
+        targets = len(self.targets)
+        if batch_size > 1:
+            targets = int(targets / batch_size) + \
+                (1 if targets % batch_size else 0)
+
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifySpontit.py` & `apprise-1.4.0/apprise/plugins/NotifySpontit.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,14 +346,21 @@
             schema=self.secure_protocol,
             userid=self.user,
             apikey=self.pprint(self.apikey, privacy, safe=''),
             targets='/'.join(
                 [NotifySpontit.quote(x, safe='') for x in self.targets]),
             params=NotifySpontit.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyStreamlabs.py` & `apprise-1.4.0/apprise/plugins/NotifyStreamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifySyslog.py` & `apprise-1.4.0/apprise/plugins/NotifySyslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyTechulusPush.py` & `apprise-1.4.0/apprise/plugins/NotifyTechulusPush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyTelegram.py` & `apprise-1.4.0/apprise/plugins/NotifyTelegram.py`

 * *Files 2% similar despite different names*

```diff
@@ -308,21 +308,26 @@
             'default': False,
         },
         'preview': {
             'name': _('Web Page Preview'),
             'type': 'bool',
             'default': False,
         },
+        'topic': {
+            'name': _('Topic Thread ID'),
+            'type': 'int',
+        },
         'to': {
             'alias_of': 'targets',
         },
     })
 
     def __init__(self, bot_token, targets, detect_owner=True,
-                 include_image=False, silent=None, preview=None, **kwargs):
+                 include_image=False, silent=None, preview=None, topic=None,
+                 **kwargs):
         """
         Initialize Telegram Object
         """
         super().__init__(**kwargs)
 
         self.bot_token = validate_regex(
             bot_token, *self.template_tokens['bot_token']['regex'],
@@ -340,14 +345,28 @@
         self.silent = self.template_args['silent']['default'] \
             if silent is None else bool(silent)
 
         # Define whether or not we should display a web page preview
         self.preview = self.template_args['preview']['default'] \
             if preview is None else bool(preview)
 
+        if topic:
+            try:
+                self.topic = int(topic)
+
+            except (TypeError, ValueError):
+                # Not a valid integer; ignore entry
+                err = 'The Telegram Topic ID specified ({}) is invalid.'\
+                    .format(topic)
+                self.logger.warning(err)
+                raise TypeError(err)
+        else:
+            # No Topic Thread
+            self.topic = None
+
         # if detect_owner is set to True, we will attempt to determine who
         # the bot owner is based on the first person who messaged it.  This
         # is not a fool proof way of doing things as over time Telegram removes
         # the message history for the bot.  So what appears (later on) to be
         # the first message to it, maybe another user who sent it a message
         # much later.  Users who set this flag should update their Apprise
         # URL later to directly include the user that we should message.
@@ -631,14 +650,17 @@
         payload = {
             # Notification Audible Control
             'disable_notification': self.silent,
             # Display Web Page Preview (if possible)
             'disable_web_page_preview': not self.preview,
         }
 
+        if self.topic:
+            payload['message_thread_id'] = self.topic
+
         # Prepare Message Body
         if self.notify_format == NotifyFormat.MARKDOWN:
             payload['parse_mode'] = 'MARKDOWN'
 
             payload['text'] = body
 
         else:  # HTML
@@ -778,26 +800,35 @@
         params = {
             'image': self.include_image,
             'detect': 'yes' if self.detect_owner else 'no',
             'silent': 'yes' if self.silent else 'no',
             'preview': 'yes' if self.preview else 'no',
         }
 
+        if self.topic:
+            params['topic'] = self.topic
+
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
         # No need to check the user token because the user automatically gets
         # appended into the list of chat ids
         return '{schema}://{bot_token}/{targets}/?{params}'.format(
             schema=self.secure_protocol,
             bot_token=self.pprint(self.bot_token, privacy, safe=''),
             targets='/'.join(
                 [NotifyTelegram.quote('@{}'.format(x)) for x in self.targets]),
             params=NotifyTelegram.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
@@ -859,14 +890,18 @@
         if 'to' in results['qsd'] and len(results['qsd']['to']):
             results['targets'] += \
                 NotifyTelegram.parse_list(results['qsd']['to'])
 
         # Store our bot token
         results['bot_token'] = bot_token
 
+        # Support Thread Topic
+        if 'topic' in results['qsd'] and len(results['qsd']['topic']):
+            results['topic'] = results['qsd']['topic']
+
         # Silent (Sends the message Silently); users will receive
         # notification with no sound.
         results['silent'] = \
             parse_bool(results['qsd'].get('silent', False))
 
         # Show Web Page Preview
         results['preview'] = \
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyTwilio.py` & `apprise-1.4.0/apprise/plugins/NotifyTwilio.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,14 +381,21 @@
                 self.account_sid, privacy, mode=PrivacyMode.Tail, safe=''),
             token=self.pprint(self.auth_token, privacy, safe=''),
             source=NotifyTwilio.quote(self.source, safe=''),
             targets='/'.join(
                 [NotifyTwilio.quote(x, safe='') for x in self.targets]),
             params=NotifyTwilio.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyTwist.py` & `apprise-1.4.0/apprise/plugins/NotifyTwist.py`

 * *Files 1% similar despite different names*

```diff
@@ -252,14 +252,20 @@
                         ['#{}'.format(x) for x in self.channels],
                         # Channel IDs
                         self.channel_ids,
                     )]),
                 params=NotifyTwist.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.channels) + len(self.channel_ids)
+
     def login(self):
         """
         A simple wrapper to authenticate with the Twist Server
         """
 
         # Prepare our payload
         payload = {
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyTwitter.py` & `apprise-1.4.0/apprise/plugins/NotifyTwitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -789,66 +789,63 @@
             'batch': 'yes' if self.batch else 'no',
             'cache': 'yes' if self.cache else 'no',
         }
 
         # Extend our parameters
         params.update(self.url_parameters(privacy=privacy, *args, **kwargs))
 
-        if len(self.targets) > 0:
-            params['to'] = ','.join(
-                [NotifyTwitter.quote(x, safe='') for x in self.targets])
-
         return '{schema}://{ckey}/{csecret}/{akey}/{asecret}' \
             '/{targets}/?{params}'.format(
                 schema=self.secure_protocol[0],
                 ckey=self.pprint(self.ckey, privacy, safe=''),
                 csecret=self.pprint(
                     self.csecret, privacy, mode=PrivacyMode.Secret, safe=''),
                 akey=self.pprint(self.akey, privacy, safe=''),
                 asecret=self.pprint(
                     self.asecret, privacy, mode=PrivacyMode.Secret, safe=''),
                 targets='/'.join(
                     [NotifyTwitter.quote('@{}'.format(target), safe='@')
                      for target in self.targets]),
                 params=NotifyTwitter.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
         results = NotifyBase.parse_url(url, verify_host=False)
         if not results:
             # We're done early as we couldn't load the results
             return results
 
-        # The first token is stored in the hostname
-        consumer_key = NotifyTwitter.unquote(results['host'])
-
         # Acquire remaining tokens
         tokens = NotifyTwitter.split_path(results['fullpath'])
 
+        # The consumer token is stored in the hostname
+        results['ckey'] = NotifyTwitter.unquote(results['host'])
+
+        #
         # Now fetch the remaining tokens
-        try:
-            consumer_secret, access_token_key, access_token_secret = \
-                tokens[0:3]
-
-        except (ValueError, AttributeError, IndexError):
-            # Force some bad values that will get caught
-            # in parsing later
-            consumer_secret = None
-            access_token_key = None
-            access_token_secret = None
-
-        results['ckey'] = consumer_key
-        results['csecret'] = consumer_secret
-        results['akey'] = access_token_key
-        results['asecret'] = access_token_secret
+        #
+
+        # Consumer Secret
+        results['csecret'] = tokens.pop(0) if tokens else None
+        # Access Token Key
+        results['akey'] = tokens.pop(0) if tokens else None
+        # Access Token Secret
+        results['asecret'] = tokens.pop(0) if tokens else None
 
         # The defined twitter mode
         if 'mode' in results['qsd'] and len(results['qsd']['mode']):
             results['mode'] = \
                 NotifyTwitter.unquote(results['qsd']['mode'])
 
         elif results['schema'].startswith('tweet'):
@@ -857,15 +854,15 @@
         results['targets'] = []
 
         # if a user has been defined, add it to the list of targets
         if results.get('user'):
             results['targets'].append(results.get('user'))
 
         # Store any remaining items as potential targets
-        results['targets'].extend(tokens[3:])
+        results['targets'].extend(tokens)
 
         # Get Cache Flag (reduces lookup hits)
         if 'cache' in results['qsd'] and len(results['qsd']['cache']):
             results['cache'] = \
                 parse_bool(results['qsd']['cache'], True)
 
         # Get Batch Mode Flag
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyVoipms.py` & `apprise-1.4.0/apprise/plugins/NotifyVoipms.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,14 +325,21 @@
             email=self.email,
             password=self.pprint(self.password, privacy, safe=''),
             from_phone='1' + self.pprint(self.source, privacy, safe=''),
             targets='/'.join(
                 ['1' + NotifyVoipms.quote(x, safe='') for x in self.targets]),
             params=NotifyVoipms.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyVonage.py` & `apprise-1.4.0/apprise/plugins/NotifyVonage.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,14 +330,21 @@
             secret=self.pprint(
                 self.secret, privacy, mode=PrivacyMode.Secret, safe=''),
             source=NotifyVonage.quote(self.source, safe=''),
             targets='/'.join(
                 [NotifyVonage.quote(x, safe='') for x in self.targets]),
             params=NotifyVonage.urlencode(params))
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        targets = len(self.targets)
+        return targets if targets > 0 else 1
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyWebexTeams.py` & `apprise-1.4.0/apprise/plugins/NotifyWebexTeams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/plugins/NotifyWindows.py` & `apprise-1.4.0/apprise/plugins/NotifyWindows.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
         Destroy callback function
         """
 
         nid = (self.hwnd, 0)
         win32gui.Shell_NotifyIcon(win32gui.NIM_DELETE, nid)
         win32api.PostQuitMessage(0)
 
-        return None
+        return 0
 
     def send(self, body, title='', notify_type=NotifyType.INFO, **kwargs):
         """
         Perform Windows Notification
         """
 
         # Always call throttle before any remote server i/o is made
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyXML.py` & `apprise-1.4.0/apprise/plugins/NotifyXML.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,24 @@
 from .NotifyBase import NotifyBase
 from ..URLBase import PrivacyMode
 from ..common import NotifyImageSize
 from ..common import NotifyType
 from ..AppriseLocale import gettext_lazy as _
 
 
+class XMLPayloadField:
+    """
+    Identifies the fields available in the JSON Payload
+    """
+    VERSION = 'Version'
+    TITLE = 'Subject'
+    MESSAGE = 'Message'
+    MESSAGETYPE = 'MessageType'
+
+
 # Defines the method to send the notification
 METHODS = (
     'POST',
     'GET',
     'DELETE',
     'PUT',
     'HEAD',
@@ -74,15 +84,16 @@
 
     # Disable throttle rate for JSON requests since they are normally
     # local anyway
     request_rate_per_sec = 0
 
     # XSD Information
     xsd_ver = '1.1'
-    xsd_url = 'https://raw.githubusercontent.com/caronc/apprise/master' \
+    xsd_default_url = \
+        'https://raw.githubusercontent.com/caronc/apprise/master' \
         '/apprise/assets/NotifyXML-{version}.xsd'
 
     # Define object templates
     templates = (
         '{schema}://{host}',
         '{schema}://{host}:{port}',
         '{schema}://{user}@{host}',
@@ -157,15 +168,15 @@
 
         self.payload = """<?xml version='1.0' encoding='utf-8'?>
 <soapenv:Envelope
     xmlns:soapenv="http://schemas.xmlsoap.org/soap/envelope/"
     xmlns:xsd="http://www.w3.org/2001/XMLSchema"
     xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance">
     <soapenv:Body>
-        <Notification xmlns:xsi="{{XSD_URL}}">
+        <Notification{{XSD_URL}}>
             {{CORE}}
             {{ATTACHMENTS}}
        </Notification>
     </soapenv:Body>
 </soapenv:Envelope>"""
 
         self.fullpath = kwargs.get('fullpath')
@@ -176,37 +187,65 @@
             if not isinstance(method, str) else method.upper()
 
         if self.method not in METHODS:
             msg = 'The method specified ({}) is invalid.'.format(method)
             self.logger.warning(msg)
             raise TypeError(msg)
 
+        # A payload map allows users to over-ride the default mapping if
+        # they're detected with the :overide=value.  Normally this would
+        # create a new key and assign it the value specified.  However
+        # if the key you specify is actually an internally mapped one,
+        # then a re-mapping takes place using the value
+        self.payload_map = {
+            XMLPayloadField.VERSION: XMLPayloadField.VERSION,
+            XMLPayloadField.TITLE: XMLPayloadField.TITLE,
+            XMLPayloadField.MESSAGE: XMLPayloadField.MESSAGE,
+            XMLPayloadField.MESSAGETYPE: XMLPayloadField.MESSAGETYPE,
+        }
+
         self.params = {}
         if params:
             # Store our extra headers
             self.params.update(params)
 
         self.headers = {}
         if headers:
             # Store our extra headers
             self.headers.update(headers)
 
+        # Set our xsd url
+        self.xsd_url = self.xsd_default_url.format(version=self.xsd_ver)
+
+        self.payload_overrides = {}
         self.payload_extras = {}
         if payload:
             # Store our extra payload entries (but tidy them up since they will
             # become XML Keys (they can't contain certain characters
             for k, v in payload.items():
                 key = re.sub(r'[^A-Za-z0-9_-]*', '', k)
                 if not key:
                     self.logger.warning(
                         'Ignoring invalid XML Stanza element name({})'
                         .format(k))
                     continue
-                self.payload_extras[key] = v
 
+                # Any values set in the payload to alter a system related one
+                # alters the system key.  Hence :message=msg maps the 'message'
+                # variable that otherwise already contains the payload to be
+                # 'msg' instead (containing the payload)
+                if key in self.payload_map:
+                    self.payload_map[key] = v
+                    self.payload_overrides[key] = v
+
+                    # Over-ride XSD URL as data is no longer known
+                    self.xsd_url = None
+
+                else:
+                    self.payload_extras[key] = v
         return
 
     def url(self, privacy=False, *args, **kwargs):
         """
         Returns the URL built dynamically based on specified arguments.
         """
 
@@ -223,14 +262,16 @@
 
         # Append our GET params into our parameters
         params.update({'-{}'.format(k): v for k, v in self.params.items()})
 
         # Append our payload extra's into our parameters
         params.update(
             {':{}'.format(k): v for k, v in self.payload_extras.items()})
+        params.update(
+            {':{}'.format(k): v for k, v in self.payload_overrides.items()})
 
         # Determine Authentication
         auth = ''
         if self.user and self.password:
             auth = '{user}:{password}@'.format(
                 user=NotifyXML.quote(self.user, safe=''),
                 password=self.pprint(
@@ -269,22 +310,29 @@
 
         # Apply any/all header over-rides defined
         headers.update(self.headers)
 
         # Our XML Attachmement subsitution
         xml_attachments = ''
 
-        # Our Payload Base
-        payload_base = {
-            'Version': self.xsd_ver,
-            'Subject': NotifyXML.escape_html(title, whitespace=False),
-            'MessageType': NotifyXML.escape_html(
-                notify_type, whitespace=False),
-            'Message': NotifyXML.escape_html(body, whitespace=False),
-        }
+        payload_base = {}
+
+        for key, value in (
+                (XMLPayloadField.VERSION, self.xsd_ver),
+                (XMLPayloadField.TITLE, NotifyXML.escape_html(
+                    title, whitespace=False)),
+                (XMLPayloadField.MESSAGE, NotifyXML.escape_html(
+                    body, whitespace=False)),
+                (XMLPayloadField.MESSAGETYPE, NotifyXML.escape_html(
+                    notify_type, whitespace=False))):
+
+            if not self.payload_map[key]:
+                # Do not store element in payload response
+                continue
+            payload_base[self.payload_map[key]] = value
 
         # Apply our payload extras
         payload_base.update(
             {k: NotifyXML.escape_html(v, whitespace=False)
                 for k, v in self.payload_extras.items()})
 
         # Base Entres
@@ -324,15 +372,16 @@
 
             # Update our xml_attachments record:
             xml_attachments = \
                 '<Attachments format="base64">' + \
                 ''.join(attachments) + '</Attachments>'
 
         re_map = {
-            '{{XSD_URL}}': self.xsd_url.format(version=self.xsd_ver),
+            '{{XSD_URL}}':
+            f' xmlns:xsi="{self.xsd_url}"' if self.xsd_url else '',
             '{{ATTACHMENTS}}': xml_attachments,
             '{{CORE}}': xml_base,
         }
 
         # Iterate over above list and store content accordingly
         re_table = re.compile(
             r'(' + '|'.join(re_map.keys()) + r')',
```

### Comparing `apprise-1.3.0/apprise/plugins/NotifyZulip.py` & `apprise-1.4.0/apprise/plugins/NotifyZulip.py`

 * *Files 3% similar despite different names*

```diff
@@ -355,14 +355,20 @@
                 org=NotifyZulip.quote(organization, safe=''),
                 token=self.pprint(self.token, privacy, safe=''),
                 targets='/'.join(
                     [NotifyZulip.quote(x, safe='') for x in self.targets]),
                 params=NotifyZulip.urlencode(params),
             )
 
+    def __len__(self):
+        """
+        Returns the number of targets associated with this notification
+        """
+        return len(self.targets)
+
     @staticmethod
     def parse_url(url):
         """
         Parses the URL and returns enough arguments that can allow
         us to re-instantiate this object.
 
         """
```

### Comparing `apprise-1.3.0/apprise/plugins/__init__.py` & `apprise-1.4.0/apprise/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/apprise/utils.py` & `apprise-1.4.0/apprise/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,21 @@
         module = importlib.util.module_from_spec(spec)
         sys.modules[name] = module
 
         spec.loader.exec_module(module)
 
     except Exception as e:
         # module isn't loadable
-        del sys.modules[name]
+        try:
+            del sys.modules[name]
+
+        except KeyError:
+            # nothing to clean up
+            pass
+
         module = None
 
         logger.debug(
             'Custom module exception raised from %s (name=%s) %s',
             path, name, str(e))
 
     return module
@@ -196,14 +202,17 @@
     re.IGNORECASE)
 
 # Used to prepare our UUID regex matching
 UUID4_RE = re.compile(
     r'[0-9a-f]{8}-[0-9a-f]{4}-4[0-9a-f]{3}-[89ab][0-9a-f]{3}-[0-9a-f]{12}',
     re.IGNORECASE)
 
+# Validate if we're a loadable Python file or not
+VALID_PYTHON_FILE_RE = re.compile(r'.+\.py(o|c)?$', re.IGNORECASE)
+
 # validate_regex() utilizes this mapping to track and re-use pre-complied
 # regular expressions
 REGEX_VALIDATE_LOOKUP = {}
 
 
 class TemplateType:
     """
@@ -1561,14 +1570,19 @@
         # We're done
         return None
 
     def _import_module(path):
         # Since our plugin name can conflict (as a module) with another
         # we want to generate random strings to avoid steping on
         # another's namespace
+        if not (path and VALID_PYTHON_FILE_RE.match(path)):
+            # Ignore file/module type
+            logger.trace('Plugin Scan: Skipping %s', path)
+            return None
+
         module_name = hashlib.sha1(path.encode('utf-8')).hexdigest()
         module_pyname = "{prefix}.{name}".format(
             prefix='apprise.custom.module', name=module_name)
 
         if module_pyname in common.NOTIFY_CUSTOM_MODULE_MAP:
             # First clear out existing entries
             for schema in common.\
```

### Comparing `apprise-1.3.0/apprise.egg-info/PKG-INFO` & `apprise-1.4.0/apprise.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apprise
-Version: 1.3.0
+Version: 1.4.0
 Summary: Push Notifications that work with just about every platform!
 Home-page: https://github.com/caronc/apprise
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: BSD
 Keywords: Alerts API AWS Boxcar BulkSMS Chat CLI ClickSend DAPNET Dbus Dingtalk Discord Email Emby Faast FCM Flock Gitter Gnome Google Gotify Growl Guilded Home Assistant IFTTT Join Kavenegar KODI Kumulos LaMetric Line Mastodon MacOS Mailgun Matrix Mattermost MessageBird Microsoft Misskey MQTT MSG91 MSTeams Nexmo Nextcloud NextcloudTalk Notica Notifico Ntfy Office365 OneSignal Opsgenie PagerDuty PagerTree ParsePlatform PopcornNotify Prowl PushBullet Pushed Pushjet Push Notifications Pushover PushSafer Reddit Rocket.Chat Ryver SendGrid ServerChan SES Signal SimplePush Sinch Slack SMSEagle SMTP2Go SNS SparkPost Spontit Streamlabs Stride Syslog Techulus Telegram Twilio Twist Twitter Vonage Webex Windows Voipms XBMC
 Platform: UNKNOWN
@@ -249,26 +249,36 @@
 ```bash
 # By default if no url or configuration is specified apprise will attempt to load
 # configuration files (if present) from:
 #  ~/.apprise
 #  ~/.apprise.yml
 #  ~/.config/apprise
 #  ~/.config/apprise.yml
+#  /etc/apprise
+#  /etc/apprise.yml
 
 # Also a subdirectory handling allows you to leverage plugins
 #  ~/.apprise/apprise
 #  ~/.apprise/apprise.yml
 #  ~/.config/apprise/apprise
 #  ~/.config/apprise/apprise.yml
+#  /etc/apprise/apprise
+#  /etc/apprise/apprise.yml
 
 # Windows users can store their default configuration files here:
 #  %APPDATA%/Apprise/apprise
 #  %APPDATA%/Apprise/apprise.yml
 #  %LOCALAPPDATA%/Apprise/apprise
 #  %LOCALAPPDATA%/Apprise/apprise.yml
+#  %ALLUSERSPROFILE%\Apprise\apprise
+#  %ALLUSERSPROFILE%\Apprise\apprise.yml
+#  %PROGRAMFILES%\Apprise\apprise
+#  %PROGRAMFILES%\Apprise\apprise.yml
+#  %COMMONPROGRAMFILES%\Apprise\apprise
+#  %COMMONPROGRAMFILES%\Apprise\apprise.yml
 
 # If you loaded one of those files, your command line gets really easy:
 apprise -vv -t 'my title' -b 'my notification body'
 
 # If you want to deviate from the default paths or specify more than one,
 # just specify them using the --config switch:
 apprise -vv -t 'my title' -b 'my notification body' \
@@ -321,18 +331,22 @@
 
 Once you've defined your custom hook, you just need to tell Apprise where it is at runtime.
 ```bash
 # By default if no plugin path is specified apprise will attempt to load
 # all plugin files (if present) from the following directory paths:
 #  ~/.apprise/plugins
 #  ~/.config/apprise/plugins
+#  /var/lib/apprise/plugins
 
 # Windows users can store their default plugin files in these directories:
 #  %APPDATA%/Apprise/plugins
 #  %LOCALAPPDATA%/Apprise/plugins
+#  %ALLUSERSPROFILE%\Apprise\plugins
+#  %PROGRAMFILES%\Apprise\plugins
+#  %COMMONPROGRAMFILES%\Apprise\plugins
 
 # If you placed your plugin file within one of the directories already defined
 # above, then your call simply needs to look like:
 apprise -vv --title 'custom override' \
         --body 'the body of my message' \
         foobar:\\
```

### Comparing `apprise-1.3.0/apprise.egg-info/SOURCES.txt` & `apprise-1.4.0/apprise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/README.md` & `apprise-1.4.0/packaging/README.md`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/man/apprise.1` & `apprise-1.4.0/packaging/man/apprise.1`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/man/apprise.md` & `apprise-1.4.0/packaging/man/apprise.md`

 * *Files 2% similar despite different names*

```diff
@@ -147,14 +147,15 @@
 entries that you can trigger on and call services you've defined.
 
 By default **apprise** looks in the following local locations for custom plugin
 files and loads them:
 
     ~/.apprise/plugins
     ~/.config/apprise/plugins
+    /var/lib/apprise/plugins
 
 Simply create your own python file with the following bare minimum content in
 it:
     from apprise.decorators import notify
 
     # This example assumes you want your function to trigger on foobar://
     # references:
@@ -188,14 +189,19 @@
     ~/.config/apprise.yml
 
     ~/.apprise/apprise
     ~/.apprise/apprise.yaml
     ~/.config/apprise/apprise
     ~/.config/apprise/apprise.yaml
 
+    /etc/apprise
+    /etc/apprise.yml
+    /etc/apprise/apprise
+    /etc/apprise/apprise.yml
+
 If a default configuration file is referenced in any way by the **apprise**
 tool, you no longer need to provide it a Service URL.  Usage of the **apprise**
 tool simplifies to:
 
     $ apprise -vv -t "my title" -b "my notification body"
 
 If you leveraged [tagging][tagging], you can define all of Apprise Service URLs in your
@@ -211,8 +217,8 @@
 ## BUGS
 
 If you find any bugs, please make them known at:
 <https://github.com/caronc/apprise/issues>
 
 ## COPYRIGHT
 
-Apprise is Copyright (C) 2021 Chris Caron <lead2gold@gmail.com>
+Apprise is Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>
```

### Comparing `apprise-1.3.0/packaging/redhat/apprise-click67-support.patch` & `apprise-1.4.0/packaging/redhat/apprise-click67-support.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/redhat/apprise-no-macosx-testing.patch` & `apprise-1.4.0/packaging/redhat/apprise-no-macosx-testing.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch` & `apprise-1.4.0/packaging/redhat/apprise-pytest-session_mocker-removal.patch`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/packaging/redhat/python-apprise.spec` & `apprise-1.4.0/packaging/redhat/python-apprise.spec`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 Opsgenie, PagerDuty, PagerTree, ParsePlatform, PopcornNotify, Prowl, Pushalot,
 PushBullet, Pushjet, Pushover, PushSafer, Reddit, Rocket.Chat, SendGrid,
 ServerChan, Signal, SimplePush, Sinch, Slack, SMSEagle, SMTP2Go, Spontit,
 SparkPost, Super Toasty, Streamlabs, Stride, Syslog, Techulus Push, Telegram,
 Twilio, Twitter, Twist, XBMC, Voipms, Vonage, Webex Teams}
 
 Name:           python-%{pypi_name}
-Version:        1.3.0
+Version:        1.4.0
 Release:        1%{?dist}
 Summary:        A simple wrapper to many popular notification services used today
 License:        BSD
 URL:            https://github.com/caronc/%{pypi_name}
 Source0:        %{url}/archive/v%{version}/%{pypi_name}-%{version}.tar.gz
 
 # RHEL/Rocky 8 ship with Click v6.7 which does not support the .stdout
@@ -182,15 +182,18 @@
 
 %files -n %{pypi_name}
 %{_bindir}/%{pypi_name}
 %{_mandir}/man1/%{pypi_name}.1*
 %{python3_sitelib}/%{pypi_name}/cli.*
 
 %changelog
-* Wed Feb  3 2023 Chris Caron <lead2gold@gmail.com> - 1.3.0
+* Mon May 15 2023 Chris Caron <lead2gold@gmail.com> - 1.4.0
+- Updated to v1.4.0
+
+* Wed Feb 22 2023 Chris Caron <lead2gold@gmail.com> - 1.3.0
 - Updated to v1.3.0
 
 * Fri Jan 20 2023 Fedora Release Engineering <releng@fedoraproject.org> - 1.2.1-2
 - Rebuilt for https://fedoraproject.org/wiki/Fedora_38_Mass_Rebuild
 
 * Wed Dec 28 2022 Chris Caron <lead2gold@gmail.com> - 1.2.1-1
 - Updated to v1.2.1
```

### Comparing `apprise-1.3.0/setup.cfg` & `apprise-1.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/setup.py` & `apprise-1.4.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['apprise = apprise.cli:main']
 
 setup(
     name='apprise',
-    version='1.3.0',
+    version='1.4.0',
     description='Push Notifications that work with just about every platform!',
     license='BSD',
     long_description=open('README.md', encoding="utf-8").read(),
     long_description_content_type='text/markdown',
     cmdclass=cmdclass,
     url='https://github.com/caronc/apprise',
     keywords=' '.join(re.split(r'\s+', open('KEYWORDS').read())),
```

### Comparing `apprise-1.3.0/test/conftest.py` & `apprise-1.4.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/helpers/__init__.py` & `apprise-1.4.0/test/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/helpers/asyncio.py` & `apprise-1.4.0/test/helpers/asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/helpers/module.py` & `apprise-1.4.0/test/helpers/module.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/helpers/rest.py` & `apprise-1.4.0/test/helpers/rest.py`

 * *Files 2% similar despite different names*

```diff
@@ -199,14 +199,17 @@
             # Ensure we are not performing any type of thorttling
             obj.request_rate_per_sec = 0
 
             # We loaded okay; now lets make sure we can reverse
             # this url
             assert isinstance(obj.url(), str) is True
 
+            # Verify we can acquire a target count as an integer
+            assert isinstance(len(obj), int)
+
             # Test url() with privacy=True
             assert isinstance(
                 obj.url(privacy=True), str) is True
 
             # Some Simple Invalid Instance Testing
             assert instance.parse_url(None) is None
             assert instance.parse_url(object) is None
@@ -236,14 +239,22 @@
                 # way these tests work. Just printing before
                 # throwing our assertion failure makes things
                 # easier to debug later on
                 print('TEST FAIL: {} regenerated as {}'.format(
                     url, obj.url()))
                 assert False
 
+            # Verify there is no change from the old and the new
+            if len(obj) != len(obj_cmp):
+                print('%d targets found in %s' % (
+                    len(obj), obj.url(privacy=True)))
+                print('But %d targets found in %s' % (
+                    len(obj_cmp), obj_cmp.url(privacy=True)))
+                raise AssertionError("Target miscount %d != %d")
+
             # Tidy our object
             del obj_cmp
 
         if _self:
             # Iterate over our expected entries inside of our
             # object
             for key, val in self.items():
@@ -367,19 +378,27 @@
             # Handle exception testing; first we turn the boolean flag
             # into a list of exceptions
             test_requests_exceptions = self.req_exceptions
 
         try:
             if test_requests_exceptions is False:
 
+                # Verify we can acquire a target count as an integer
+                targets = len(obj)
+
                 # check that we're as expected
                 assert obj.notify(
                     body=self.body, title=self.title,
                     notify_type=notify_type) == notify_response
 
+                if notify_response:
+                    # If we successfully got a response, there must have been
+                    # at least 1 target present
+                    assert targets > 0
+
                 # check that this doesn't change using different overflow
                 # methods
                 assert obj.notify(
                     body=self.body, title=self.title,
                     notify_type=notify_type,
                     overflow=OverflowMode.UPSTREAM) == notify_response
                 assert obj.notify(
@@ -443,14 +462,15 @@
 
                     # Same results should apply to a list of attachments
                     attach = AppriseAttachment((
                         os.path.join(self.__test_var_dir, 'apprise-test.gif'),
                         os.path.join(self.__test_var_dir, 'apprise-test.png'),
                         os.path.join(self.__test_var_dir, 'apprise-test.jpeg'),
                     ))
+
                     assert obj.notify(
                         body=self.body, title=self.title,
                         notify_type=notify_type,
                         attach=attach) == attach_response
 
             else:
```

### Comparing `apprise-1.3.0/test/test_api.py` & `apprise-1.4.0/test/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
 from __future__ import print_function
 import asyncio
+import concurrent.futures
 import re
 import sys
 import pytest
 import requests
 from unittest import mock
 
 from os.path import dirname
@@ -1777,15 +1778,17 @@
                 # in the template_tokens is accounted for in at least one of
                 # the defined templates
                 assert arg in defined_tokens
 
 
 @mock.patch('requests.post')
 @mock.patch('asyncio.gather', wraps=asyncio.gather)
-def test_apprise_async_mode(mock_gather, mock_post, tmpdir):
+@mock.patch('concurrent.futures.ThreadPoolExecutor',
+            wraps=concurrent.futures.ThreadPoolExecutor)
+def test_apprise_async_mode(mock_threadpool, mock_gather, mock_post, tmpdir):
     """
     API: Apprise() async_mode tests
 
     """
     mock_post.return_value.status_code = requests.codes.ok
 
     # Define some servers
@@ -1810,17 +1813,17 @@
     # Our servers should carry this flag
     for server in a:
         assert server.asset.async_mode is True
 
     # Send Notifications Asyncronously
     assert a.notify("async") is True
 
-    # Verify our async code got executed
-    assert mock_gather.call_count > 0
-    mock_gather.reset_mock()
+    # Verify our thread pool was created
+    assert mock_threadpool.call_count == 1
+    mock_threadpool.reset_mock()
 
     # Provide an over-ride now
     asset = AppriseAsset(async_mode=False)
     assert asset.async_mode is False
 
     # Load our asset
     a = Apprise(asset=asset)
@@ -1859,17 +1862,17 @@
     a[1].asset = AppriseAsset(async_mode=False)
     assert a[0].asset.async_mode is True
     assert a[1].asset.async_mode is False
 
     # Send 1 Notification Syncronously, the other Asyncronously
     assert a.notify("a mixed batch") is True
 
-    # Verify our async code got called
-    assert mock_gather.call_count > 0
-    mock_gather.reset_mock()
+    # Verify we didn't use a thread pool for a single notification
+    assert mock_threadpool.call_count == 0
+    mock_threadpool.reset_mock()
 
 
 def test_notify_matrix_dynamic_importing(tmpdir):
     """
     API: Apprise() Notify Matrix Importing
 
     """
```

### Comparing `apprise-1.3.0/test/test_apprise_attachments.py` & `apprise-1.4.0/test/test_apprise_attachments.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_apprise_config.py` & `apprise-1.4.0/test/test_apprise_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -557,15 +557,15 @@
 
     # Define our good:// url
     class GoodNotification(NotifyBase):
         def __init__(self, **kwargs):
             super().__init__(
                 notify_format=NotifyFormat.HTML, **kwargs)
 
-        async def async_notify(self, **kwargs):
+        def notify(self, **kwargs):
             # Pretend everything is okay
             return True
 
         def url(self, **kwargs):
             # support url()
             return ''
```

### Comparing `apprise-1.3.0/test/test_apprise_utils.py` & `apprise-1.4.0/test/test_apprise_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -2011,14 +2011,29 @@
 
     assert results == sorted([
         '.divx', '.wmv', '.iso', '.mkv', '.mov', '.mpg', '.avi', '.vob',
         '.xvid', '.mpeg', '.mp4',
     ])
 
 
+def test_import_module(tmpdir):
+    """utils: imort_module testing
+    """
+    # Prepare ourselves a file to work with
+    bad_file_base = tmpdir.mkdir('a')
+    bad_file = bad_file_base.join('README.md')
+    bad_file.write(cleandoc("""
+    I'm a README file, not a Python one.
+
+    I can't be loaded
+    """))
+    assert utils.import_module(str(bad_file), 'invalidfile1') is None
+    assert utils.import_module(str(bad_file_base), 'invalidfile2') is None
+
+
 def test_module_detection(tmpdir):
     """utils: test_module_detection() testing
     """
 
     # Clear our working variables so they don't obstruct with the tests here
     utils.PATHS_PREVIOUSLY_SCANNED.clear()
     common.NOTIFY_CUSTOM_MODULE_MAP.clear()
@@ -2037,31 +2052,38 @@
     from apprise.decorators import notify
 
     @notify(on="clihook")
     def mywrapper(body, title, notify_type, *args, **kwargs):
         pass
     """))
 
+    notify_ignore = notify_hook_a_base.join('README.md')
+    notify_ignore.write(cleandoc("""
+    We're not a .py file, so this file gets gracefully skipped
+    """))
+
     # Not previously loaded
     assert 'clihook' not in common.NOTIFY_SCHEMA_MAP
 
     # load entry by string
     utils.module_detection(str(notify_hook_a))
+    utils.module_detection(str(notify_ignore))
+    utils.module_detection(str(notify_hook_a_base))
 
-    assert len(utils.PATHS_PREVIOUSLY_SCANNED) == 1
+    assert len(utils.PATHS_PREVIOUSLY_SCANNED) == 3
     assert len(common.NOTIFY_CUSTOM_MODULE_MAP) == 1
 
     # Now loaded
     assert 'clihook' in common.NOTIFY_SCHEMA_MAP
 
     # load entry by array
     utils.module_detection([str(notify_hook_a)])
 
     # No changes to our path
-    assert len(utils.PATHS_PREVIOUSLY_SCANNED) == 1
+    assert len(utils.PATHS_PREVIOUSLY_SCANNED) == 3
     assert len(common.NOTIFY_CUSTOM_MODULE_MAP) == 1
 
     # Reset our variables for the next test
     utils.PATHS_PREVIOUSLY_SCANNED.clear()
     common.NOTIFY_CUSTOM_MODULE_MAP.clear()
     del common.NOTIFY_SCHEMA_MAP['clihook']
```

### Comparing `apprise-1.3.0/test/test_asyncio.py` & `apprise-1.4.0/test/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_attach_base.py` & `apprise-1.4.0/test/test_attach_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_attach_file.py` & `apprise-1.4.0/test/test_attach_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_attach_http.py` & `apprise-1.4.0/test/test_attach_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_cli.py` & `apprise-1.4.0/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_config_base.py` & `apprise-1.4.0/test/test_config_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_config_file.py` & `apprise-1.4.0/test/test_config_file.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_config_http.py` & `apprise-1.4.0/test/test_config_http.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_config_memory.py` & `apprise-1.4.0/test/test_config_memory.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_conversion.py` & `apprise-1.4.0/test/test_conversion.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_decorator_notify.py` & `apprise-1.4.0/test/test_decorator_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_escapes.py` & `apprise-1.4.0/test/test_escapes.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_locale.py` & `apprise-1.4.0/test/test_locale.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_logger.py` & `apprise-1.4.0/test/test_logger.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_notify_base.py` & `apprise-1.4.0/test/test_notify_base.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_apprise_api.py` & `apprise-1.4.0/test/test_plugin_guilded.py`

 * *Files 22% similar despite different names*

```diff
@@ -26,149 +26,165 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from apprise.plugins.NotifyAppriseAPI import NotifyAppriseAPI
-from helpers import AppriseURLTester
+import os
+from unittest import mock
+
+import pytest
 import requests
 
+from apprise.plugins.NotifyGuilded import NotifyGuilded
+from helpers import AppriseURLTester
+
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
+# Attachment Directory
+TEST_VAR_DIR = os.path.join(os.path.dirname(__file__), 'var')
+
 # Our Testing URLs
 apprise_url_tests = (
-    ('apprise://', {
-        # invalid url (not complete)
-        'instance': None,
-    }),
-    # A a bad url
-    ('apprise://:@/', {
-        'instance': None,
-    }),
-    # No token specified
-    ('apprise://localhost', {
+    ('guilded://', {
         'instance': TypeError,
     }),
-    # invalid token
-    ('apprise://localhost/!', {
+    # An invalid url
+    ('guilded://:@/', {
         'instance': TypeError,
     }),
-    # No token specified (whitespace is trimmed)
-    ('apprise://localhost/%%20', {
+    # No webhook_token specified
+    ('guilded://%s' % ('i' * 24), {
         'instance': TypeError,
     }),
-    # A valid URL with Token
-    ('apprise://localhost/%s' % ('a' * 32), {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprise://localhost/a...a/',
-    }),
-    # A valid URL with Token (using port)
-    ('apprise://localhost:8080/%s' % ('b' * 32), {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprise://localhost:8080/b...b/',
-    }),
-    # A secure (https://) reference
-    ('apprises://localhost/%s' % ('c' * 32), {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprises://localhost/c...c/',
-    }),
-    # Native URL suport (https)
-    ('https://example.com/path/notify/%s' % ('d' * 32), {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprises://example.com/path/d...d/',
-    }),
-    # Native URL suport (http)
-    ('http://example.com/notify/%s' % ('d' * 32), {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprise://example.com/d...d/',
-    }),
-    # support to= keyword
-    ('apprises://localhost/?to=%s' % ('e' * 32), {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprises://localhost/e...e/',
-    }),
-    # support token= keyword (even when passed with to=, token over-rides)
-    ('apprise://localhost/?token=%s&to=%s' % ('f' * 32, 'abcd'), {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprise://localhost/f...f/',
-    }),
-    # Test tags
-    ('apprise://localhost/?token=%s&tags=admin,team' % ('abcd'), {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprise://localhost/a...d/',
-    }),
-    # Test Format string
-    ('apprise://user@localhost/mytoken0/?format=markdown', {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprise://user@localhost/m...0/',
-    }),
-    ('apprise://user@localhost/mytoken1/', {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprise://user@localhost/m...1/',
-    }),
-    ('apprise://localhost:8080/mytoken/', {
-        'instance': NotifyAppriseAPI,
-    }),
-    ('apprise://user:pass@localhost:8080/mytoken2/', {
-        'instance': NotifyAppriseAPI,
-        'privacy_url': 'apprise://user:****@localhost:8080/m...2/',
-    }),
-    ('apprises://localhost/mytoken/', {
-        'instance': NotifyAppriseAPI,
-    }),
-    ('apprises://user:pass@localhost/mytoken3/', {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprises://user:****@localhost/m...3/',
-    }),
-    ('apprises://localhost:8080/mytoken4/', {
-        'instance': NotifyAppriseAPI,
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprises://localhost:8080/m...4/',
-    }),
-    ('apprises://user:password@localhost:8080/mytoken5/', {
-        'instance': NotifyAppriseAPI,
-
-        # Our expected url(privacy=True) startswith() response:
-        'privacy_url': 'apprises://user:****@localhost:8080/m...5/',
-    }),
-    ('apprises://localhost:8080/path?+HeaderKey=HeaderValue', {
-        'instance': NotifyAppriseAPI,
+    # Provide both an webhook id and a webhook token
+    ('guilded://%s/%s' % ('i' * 24, 't' * 64), {
+        'instance': NotifyGuilded,
+        'requests_response_code': requests.codes.no_content,
+    }),
+    # Provide a temporary username
+    ('guilded://l2g@%s/%s' % ('i' * 24, 't' * 64), {
+        'instance': NotifyGuilded,
+        'requests_response_code': requests.codes.no_content,
+    }),
+    # test image= field
+    ('guilded://%s/%s?format=markdown&footer=Yes&image=Yes' % (
+        'i' * 24, 't' * 64), {
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+            # don't include an image by default
+            'include_image': False,
+    }),
+    ('guilded://%s/%s?format=markdown&footer=Yes&image=No&fields=no' % (
+        'i' * 24, 't' * 64), {
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+    }),
+    ('guilded://%s/%s?format=markdown&footer=Yes&image=Yes' % (
+        'i' * 24, 't' * 64), {
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+    }),
+    ('https://media.guilded.gg/webhooks/{}/{}'.format(
+        '0' * 10, 'B' * 40), {
+            # Native URL Support, support the provided guilded URL from their
+            # webpage.
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+    }),
+    ('guilded://%s/%s?format=markdown&avatar=No&footer=No' % (
+        'i' * 24, 't' * 64), {
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+    }),
+    # different format support
+    ('guilded://%s/%s?format=markdown' % ('i' * 24, 't' * 64), {
+        'instance': NotifyGuilded,
+        'requests_response_code': requests.codes.no_content,
+    }),
+    ('guilded://%s/%s?format=text' % ('i' * 24, 't' * 64), {
+        'instance': NotifyGuilded,
+        'requests_response_code': requests.codes.no_content,
+    }),
+    # Test with avatar URL
+    ('guilded://%s/%s?avatar_url=http://localhost/test.jpg' % (
+        'i' * 24, 't' * 64), {
+            'instance': NotifyGuilded,
+            'requests_response_code': requests.codes.no_content,
+    }),
+    # Test without image set
+    ('guilded://%s/%s' % ('i' * 24, 't' * 64), {
+        'instance': NotifyGuilded,
+        'requests_response_code': requests.codes.no_content,
+        # don't include an image by default
+        'include_image': False,
     }),
-    ('apprise://localhost/%s' % ('a' * 32), {
-        'instance': NotifyAppriseAPI,
+    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
+        'instance': NotifyGuilded,
         # force a failure
         'response': False,
         'requests_response_code': requests.codes.internal_server_error,
     }),
-    ('apprise://localhost/%s' % ('a' * 32), {
-        'instance': NotifyAppriseAPI,
+    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
+        'instance': NotifyGuilded,
         # throw a bizzare code forcing us to fail to look it up
         'response': False,
         'requests_response_code': 999,
     }),
-    ('apprise://localhost/%s' % ('a' * 32), {
-        'instance': NotifyAppriseAPI,
+    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
+        'instance': NotifyGuilded,
         # Throws a series of connection and transfer exceptions when this flag
         # is set and tests that we gracfully handle them
         'test_requests_exceptions': True,
     }),
 )
 
 
-def test_plugin_apprise_urls():
+def test_plugin_guilded_urls():
     """
-    NotifyAppriseAPI() General Checks
+    NotifyGuilded() Apprise URLs
 
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
+
+
+@mock.patch('requests.post')
+def test_plugin_guilded_general(mock_post):
+    """
+    NotifyGuilded() General Checks
+
+    """
+
+    # Initialize some generic (but valid) tokens
+    webhook_id = 'A' * 24
+    webhook_token = 'B' * 64
+
+    # Prepare Mock
+    mock_post.return_value = requests.Request()
+    mock_post.return_value.status_code = requests.codes.ok
+
+    # Invalid webhook id
+    with pytest.raises(TypeError):
+        NotifyGuilded(webhook_id=None, webhook_token=webhook_token)
+    # Invalid webhook id (whitespace)
+    with pytest.raises(TypeError):
+        NotifyGuilded(webhook_id="  ", webhook_token=webhook_token)
+
+    # Invalid webhook token
+    with pytest.raises(TypeError):
+        NotifyGuilded(webhook_id=webhook_id, webhook_token=None)
+    # Invalid webhook token (whitespace)
+    with pytest.raises(TypeError):
+        NotifyGuilded(webhook_id=webhook_id, webhook_token="   ")
+
+    obj = NotifyGuilded(
+        webhook_id=webhook_id,
+        webhook_token=webhook_token,
+        footer=True, thumbnail=False)
+
+    # Test that we get a string response
+    assert isinstance(obj.url(), str) is True
```

### Comparing `apprise-1.3.0/test/test_plugin_bark.py` & `apprise-1.4.0/test/test_plugin_bark.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_boxcar.py` & `apprise-1.4.0/test/test_plugin_boxcar.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,12 +164,18 @@
     # Test notifications without a body or a title
     p = NotifyBoxcar(access=access, secret=secret, targets=None)
 
     assert p.notify(body=None, title=None, notify_type=NotifyType.INFO) is True
 
     # Test comma, separate values
     device = 'a' * 64
-
     p = NotifyBoxcar(
         access=access, secret=secret,
         targets=','.join([device, device, device]))
+    # unique entries are colapsed into 1
+    assert len(p.device_tokens) == 1
+
+    p = NotifyBoxcar(
+        access=access, secret=secret,
+        targets=','.join(['a' * 64, 'b' * 64, 'c' * 64]))
+    # not unique, so we get the same data here
     assert len(p.device_tokens) == 3
```

### Comparing `apprise-1.3.0/test/test_plugin_bulksms.py` & `apprise-1.4.0/test/test_plugin_bulksms.py`

 * *Files 3% similar despite different names*

```diff
@@ -169,14 +169,17 @@
     # Test our markdown
     obj = Apprise.instantiate(
         'bulksms://{}:{}@{}?batch=n'.format(user, pwd, '/'.join(targets)))
 
     assert obj.notify(
         body='body', title='title', notify_type=NotifyType.INFO) is True
 
+    # We know there are 4 targets
+    assert len(obj) == 4
+
     # Test our call count
     assert mock_post.call_count == 4
 
     # Test
     details = mock_post.call_args_list[0]
     payload = loads(details[1]['data'])
     assert payload['to'] == '+15551231234'
@@ -201,7 +204,13 @@
 
     # Verify our URL looks good
     assert obj.url().startswith(
         'bulksms://{}:{}@{}'.format(user, pwd, '/'.join(
             ['+15551231234', '+15555555555', '@group', '@12'])))
 
     assert 'batch=no' in obj.url()
+
+    # With our batch in place, our calculations are different
+    obj = Apprise.instantiate(
+        'bulksms://{}:{}@{}?batch=y'.format(user, pwd, '/'.join(targets)))
+    # 2 groups and 2 phones are lumped together
+    assert len(obj) == 3
```

### Comparing `apprise-1.3.0/test/test_plugin_clicksend.py` & `apprise-1.4.0/test/test_plugin_clicksend.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_custom_form.py` & `apprise-1.4.0/test/test_plugin_custom_form.py`

 * *Files 3% similar despite different names*

```diff
@@ -314,28 +314,29 @@
     response.status_code = requests.codes.ok
 
     # Prepare Mock
     mock_post.return_value = response
     mock_get.return_value = response
 
     results = NotifyForm.parse_url(
-        'form://localhost:8080/command?:abcd=test&method=POST')
+        'form://localhost:8080/command?:message=msg&:abcd=test&method=POST')
 
     assert isinstance(results, dict)
     assert results['user'] is None
     assert results['password'] is None
     assert results['port'] == 8080
     assert results['host'] == 'localhost'
     assert results['fullpath'] == '/command'
     assert results['path'] == '/'
     assert results['query'] == 'command'
     assert results['schema'] == 'form'
     assert results['url'] == 'form://localhost:8080/command'
     assert isinstance(results['qsd:'], dict) is True
     assert results['qsd:']['abcd'] == 'test'
+    assert results['qsd:']['message'] == 'msg'
 
     instance = NotifyForm(**results)
     assert isinstance(instance, NotifyForm)
 
     response = instance.send(title='title', body='body')
     assert response is True
     assert mock_post.call_count == 1
@@ -343,16 +344,19 @@
 
     details = mock_post.call_args_list[0]
     assert details[0][0] == 'http://localhost:8080/command'
     assert 'abcd' in details[1]['data']
     assert details[1]['data']['abcd'] == 'test'
     assert 'title' in details[1]['data']
     assert details[1]['data']['title'] == 'title'
-    assert 'message' in details[1]['data']
-    assert details[1]['data']['message'] == 'body'
+    assert 'message' not in details[1]['data']
+    # message over-ride was provided; the body is now in `msg` and not
+    # `message`
+    assert 'msg' in details[1]['data']
+    assert details[1]['data']['msg'] == 'body'
 
     assert instance.url(privacy=False).startswith(
         'form://localhost:8080/command?')
 
     # Generate a new URL based on our last and verify key values are the same
     new_results = NotifyForm.parse_url(instance.url(safe=False))
     for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
@@ -360,44 +364,53 @@
         assert new_results[k] == results[k]
 
     # Reset our mock configuration
     mock_post.reset_mock()
     mock_get.reset_mock()
 
     results = NotifyForm.parse_url(
-        'form://localhost:8080/command?:message=test&method=POST')
+        'form://localhost:8080/command?:type=&:message=msg&method=POST')
 
     assert isinstance(results, dict)
     assert results['user'] is None
     assert results['password'] is None
     assert results['port'] == 8080
     assert results['host'] == 'localhost'
     assert results['fullpath'] == '/command'
     assert results['path'] == '/'
     assert results['query'] == 'command'
     assert results['schema'] == 'form'
     assert results['url'] == 'form://localhost:8080/command'
     assert isinstance(results['qsd:'], dict) is True
-    assert results['qsd:']['message'] == 'test'
+    assert results['qsd:']['message'] == 'msg'
 
     instance = NotifyForm(**results)
     assert isinstance(instance, NotifyForm)
 
     response = instance.send(title='title', body='body')
     assert response is True
     assert mock_post.call_count == 1
     assert mock_get.call_count == 0
 
     details = mock_post.call_args_list[0]
     assert details[0][0] == 'http://localhost:8080/command'
     assert 'title' in details[1]['data']
     assert details[1]['data']['title'] == 'title'
+
+    # type was removed from response object
+    assert 'type' not in details[1]['data']
+
+    # message over-ride was provided; the body is now in `msg` and not
+    # `message`
+    assert details[1]['data']['msg'] == 'body'
+
     # 'body' is over-ridden by 'test' passed inline with the URL
-    assert 'message' in details[1]['data']
-    assert details[1]['data']['message'] == 'test'
+    assert 'message' not in details[1]['data']
+    assert 'msg' in details[1]['data']
+    assert details[1]['data']['msg'] == 'body'
 
     assert instance.url(privacy=False).startswith(
         'form://localhost:8080/command?')
 
     # Generate a new URL based on our last and verify key values are the same
     new_results = NotifyForm.parse_url(instance.url(safe=False))
     for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
@@ -434,16 +447,17 @@
 
     details = mock_get.call_args_list[0]
     assert details[0][0] == 'http://localhost:8080/command'
 
     assert 'title' in details[1]['params']
     assert details[1]['params']['title'] == 'title'
     # 'body' is over-ridden by 'test' passed inline with the URL
-    assert 'message' in details[1]['params']
-    assert details[1]['params']['message'] == 'test'
+    assert 'message' not in details[1]['params']
+    assert 'test' in details[1]['params']
+    assert details[1]['params']['test'] == 'body'
 
     assert instance.url(privacy=False).startswith(
         'form://localhost:8080/command?')
 
     # Generate a new URL based on our last and verify key values are the same
     new_results = NotifyForm.parse_url(instance.url(safe=False))
     for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
```

### Comparing `apprise-1.3.0/test/test_plugin_custom_json.py` & `apprise-1.4.0/test/test_plugin_custom_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -172,46 +172,58 @@
     response = requests.Request()
     response.status_code = requests.codes.ok
 
     # Prepare Mock
     mock_post.return_value = response
     mock_get.return_value = response
 
+    # This string also tests that type is set to nothing
     results = NotifyJSON.parse_url(
-        'json://localhost:8080/command?:message=test&method=GET')
+        'json://localhost:8080/command?'
+        ':message=msg&:test=value&method=GET'
+        '&:type=')
 
     assert isinstance(results, dict)
     assert results['user'] is None
     assert results['password'] is None
     assert results['port'] == 8080
     assert results['host'] == 'localhost'
     assert results['fullpath'] == '/command'
     assert results['path'] == '/'
     assert results['query'] == 'command'
     assert results['schema'] == 'json'
     assert results['url'] == 'json://localhost:8080/command'
     assert isinstance(results['qsd:'], dict) is True
-    assert results['qsd:']['message'] == 'test'
+    assert results['qsd:']['message'] == 'msg'
+    # empty special mapping
+    assert results['qsd:']['type'] == ''
 
     instance = NotifyJSON(**results)
     assert isinstance(instance, NotifyJSON)
 
     response = instance.send(title='title', body='body')
     assert response is True
     assert mock_post.call_count == 0
     assert mock_get.call_count == 1
 
     details = mock_get.call_args_list[0]
     assert details[0][0] == 'http://localhost:8080/command'
     assert 'title' in details[1]['data']
     dataset = json.loads(details[1]['data'])
     assert dataset['title'] == 'title'
-    assert 'message' in dataset
-    # message over-ride was provided
-    assert dataset['message'] == 'test'
+    assert 'message' not in dataset
+    assert 'msg' in dataset
+    # type was set to nothing which implies it should be removed
+    assert 'type' not in dataset
+    # message over-ride was provided; the body is now in `msg` and not
+    # `message`
+    assert dataset['msg'] == 'body'
+
+    assert 'test' in dataset
+    assert dataset['test'] == 'value'
 
     assert instance.url(privacy=False).startswith(
         'json://localhost:8080/command?')
 
     # Generate a new URL based on our last and verify key values are the same
     new_results = NotifyJSON.parse_url(instance.url(safe=False))
     for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
```

### Comparing `apprise-1.3.0/test/test_plugin_custom_xml.py` & `apprise-1.4.0/test/test_plugin_custom_xml.py`

 * *Files 13% similar despite different names*

```diff
@@ -247,35 +247,38 @@
     response.status_code = requests.codes.ok
 
     # Prepare Mock
     mock_post.return_value = response
     mock_get.return_value = response
 
     results = NotifyXML.parse_url(
-        'xml://localhost:8080/command?:Message=test&method=GET'
-        '&:Key=value&:,=invalid')
+        'xml://localhost:8080/command?:Message=Body&method=GET'
+        '&:Key=value&:,=invalid&:MessageType=')
 
     assert isinstance(results, dict)
     assert results['user'] is None
     assert results['password'] is None
     assert results['port'] == 8080
     assert results['host'] == 'localhost'
     assert results['fullpath'] == '/command'
     assert results['path'] == '/'
     assert results['query'] == 'command'
     assert results['schema'] == 'xml'
     assert results['url'] == 'xml://localhost:8080/command'
     assert isinstance(results['qsd:'], dict) is True
-    assert results['qsd:']['Message'] == 'test'
+    assert results['qsd:']['Message'] == 'Body'
     assert results['qsd:']['Key'] == 'value'
     assert results['qsd:'][','] == 'invalid'
 
     instance = NotifyXML(**results)
     assert isinstance(instance, NotifyXML)
 
+    # XSD URL is disabled due to custom formatting
+    assert instance.xsd_url is None
+
     response = instance.send(title='title', body='body')
     assert response is True
     assert mock_post.call_count == 0
     assert mock_get.call_count == 1
 
     details = mock_get.call_args_list[0]
     assert details[0][0] == 'http://localhost:8080/command'
@@ -286,13 +289,67 @@
     new_results = NotifyXML.parse_url(instance.url(safe=False))
     for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
               'schema', 'url', 'method'):
         assert new_results[k] == results[k]
 
     # Test our data set for our key/value pair
     assert re.search(r'<Version>[1-9]+\.[0-9]+</Version>', details[1]['data'])
-    assert re.search('<MessageType>info</MessageType>', details[1]['data'])
     assert re.search('<Subject>title</Subject>', details[1]['data'])
-    # Custom entry Message acts as Over-ride and kicks in here
-    assert re.search('<Message>test</Message>', details[1]['data'])
+
+    assert re.search('<Message>test</Message>', details[1]['data']) is None
+    assert re.search('<Message>', details[1]['data']) is None
+    # MessageType was removed from the payload
+    assert re.search('<MessageType>', details[1]['data']) is None
+    # However we can find our mapped Message to the new value Body
+    assert re.search('<Body>body</Body>', details[1]['data'])
     # Custom entry
     assert re.search('<Key>value</Key>', details[1]['data'])
+
+    mock_post.reset_mock()
+    mock_get.reset_mock()
+
+    results = NotifyXML.parse_url(
+        'xml://localhost:8081/command?method=POST&:New=Value')
+
+    assert isinstance(results, dict)
+    assert results['user'] is None
+    assert results['password'] is None
+    assert results['port'] == 8081
+    assert results['host'] == 'localhost'
+    assert results['fullpath'] == '/command'
+    assert results['path'] == '/'
+    assert results['query'] == 'command'
+    assert results['schema'] == 'xml'
+    assert results['url'] == 'xml://localhost:8081/command'
+    assert isinstance(results['qsd:'], dict) is True
+    assert results['qsd:']['New'] == 'Value'
+
+    instance = NotifyXML(**results)
+    assert isinstance(instance, NotifyXML)
+
+    # XSD URL is disabled due to custom formatting
+    assert instance.xsd_url is not None
+
+    response = instance.send(title='title', body='body')
+    assert response is True
+    assert mock_post.call_count == 1
+    assert mock_get.call_count == 0
+
+    details = mock_post.call_args_list[0]
+    assert details[0][0] == 'http://localhost:8081/command'
+    assert instance.url(privacy=False).startswith(
+        'xml://localhost:8081/command?')
+
+    # Generate a new URL based on our last and verify key values are the same
+    new_results = NotifyXML.parse_url(instance.url(safe=False))
+    for k in ('user', 'password', 'port', 'host', 'fullpath', 'path', 'query',
+              'schema', 'url', 'method'):
+        assert new_results[k] == results[k]
+
+    # Test our data set for our key/value pair
+    assert re.search(r'<Version>[1-9]+\.[0-9]+</Version>', details[1]['data'])
+    assert re.search(r'<MessageType>info</MessageType>', details[1]['data'])
+    assert re.search(r'<Subject>title</Subject>', details[1]['data'])
+    # No over-ride
+    assert re.search(r'<Message>body</Message>', details[1]['data'])
+    # since there is no over-ride, an xmlns:xsi is provided
+    assert re.search(r'<Notification xmlns:xsi=', details[1]['data'])
```

### Comparing `apprise-1.3.0/test/test_plugin_d7networks.py` & `apprise-1.4.0/test/test_plugin_d7networks.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_dapnet.py` & `apprise-1.4.0/test/test_plugin_dapnet.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 import requests
 from unittest import mock
 
 import apprise
 from apprise.plugins.NotifyDapnet import DapnetPriority, NotifyDapnet
 from helpers import AppriseURLTester
+from apprise import NotifyType
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
@@ -138,14 +139,43 @@
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
 
 
 @mock.patch('requests.post')
+def test_plugin_dapnet_edge_cases(mock_post):
+    """
+    NotifyDapnet() Edge Cases
+    """
+    # Prepare Mock
+    mock_post.return_value = requests.Request()
+    mock_post.return_value.status_code = requests.codes.created
+
+    # test the handling of our batch modes
+    obj = apprise.Apprise.instantiate(
+        'dapnet://user:pass@{}?batch=yes'.format(
+            '/'.join(['DF1ABC', 'DF1DEF'])))
+    assert isinstance(obj, NotifyDapnet)
+
+    # objects will be combined into a single post in batch mode
+    assert len(obj) == 1
+
+    # Force our batch to break into separate messages
+    obj.default_batch_size = 1
+
+    # We'll send 2 messages now
+    assert len(obj) == 2
+
+    assert obj.notify(
+        body='body', title='title', notify_type=NotifyType.INFO) is True
+    assert mock_post.call_count == 2
+
+
+@mock.patch('requests.post')
 def test_plugin_dapnet_config_files(mock_post):
     """
     NotifyDapnet() Config File Cases
     """
     content = """
     urls:
       - dapnet://user:pass@DF1ABC:
```

### Comparing `apprise-1.3.0/test/test_plugin_dingtalk.py` & `apprise-1.4.0/test/test_plugin_dingtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_discord.py` & `apprise-1.4.0/test/test_plugin_discord.py`

 * *Files 5% similar despite different names*

```diff
@@ -364,14 +364,35 @@
                     body_format=NotifyFormat.MARKDOWN) is True
 
     # Toggle our logo availability
     a.asset.image_url_logo = None
     assert a.notify(
         body='body', title='title', notify_type=NotifyType.INFO) is True
 
+    # Create an apprise instance
+    a = Apprise()
+
+    # Reset our object
+    mock_post.reset_mock()
+
+    # Test our threading
+    assert a.add(
+        'discord://{webhook_id}/{webhook_token}/'
+        '?thread=12345'.format(
+            webhook_id=webhook_id,
+            webhook_token=webhook_token)) is True
+
+    # This call includes an image with it's payload:
+    assert a.notify(body='test', title='title') is True
+
+    assert mock_post.call_count == 1
+    response = mock_post.call_args_list[0][1]
+    assert 'params' in response
+    assert response['params'].get('thread_id') == '12345'
+
 
 @mock.patch('requests.post')
 def test_plugin_discord_markdown_extra(mock_post):
     """
     NotifyDiscord() Markdown Extra Checks
 
     """
```

### Comparing `apprise-1.3.0/test/test_plugin_email.py` & `apprise-1.4.0/test/test_plugin_email.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,17 @@
 
             assert isinstance(obj, instance)
 
             if isinstance(obj, NotifyBase):
                 # We loaded okay; now lets make sure we can reverse this url
                 assert isinstance(obj.url(), str) is True
 
+                # Verify we can acquire a target count as an integer
+                assert isinstance(len(obj), int)
+
                 # Test url() with privacy=True
                 assert isinstance(
                     obj.url(privacy=True), str) is True
 
                 # Some Simple Invalid Instance Testing
                 assert instance.parse_url(None) is None
                 assert instance.parse_url(object) is None
@@ -365,28 +368,44 @@
                     # Assert messages are hard to trace back with the way
                     # these tests work. Just printing before throwing our
                     # assertion failure makes things easier to debug later on
                     print('TEST FAIL: {} regenerated as {}'.format(
                         url, obj.url()))
                     assert False
 
+                # Verify there is no change from the old and the new
+                if len(obj) != len(obj_cmp):
+                    print('%d targets found in %s' % (
+                        len(obj), obj.url(privacy=True)))
+                    print('But %d targets found in %s' % (
+                        len(obj_cmp), obj_cmp.url(privacy=True)))
+                    raise AssertionError("Target miscount %d != %d")
+
             if self:
                 # Iterate over our expected entries inside of our object
                 for key, val in self.items():
                     # Test that our object has the desired key
                     assert hasattr(key, obj)
                     assert getattr(key, obj) == val
 
             try:
                 if test_smtplib_exceptions is False:
+                    # Verify we can acquire a target count as an integer
+                    targets = len(obj)
+
                     # check that we're as expected
                     assert obj.notify(
                         title='test', body='body',
                         notify_type=NotifyType.INFO) == response
 
+                    if response:
+                        # If we successfully got a response, there must have
+                        # been at least 1 target present
+                        assert targets > 0
+
                 else:
                     for exception in test_smtplib_exceptions:
                         mock_socket.sendmail.side_effect = exception
                         try:
                             assert obj.notify(
                                 title='test', body='body',
                                 notify_type=NotifyType.INFO) is False
```

### Comparing `apprise-1.3.0/test/test_plugin_emby.py` & `apprise-1.4.0/test/test_plugin_emby.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_enigma2.py` & `apprise-1.4.0/test/test_plugin_enigma2.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_faast.py` & `apprise-1.4.0/test/test_plugin_faast.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_fcm.py` & `apprise-1.4.0/test/test_plugin_fcm.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_flock.py` & `apprise-1.4.0/test/test_plugin_flock.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_gitter.py` & `apprise-1.4.0/test/test_plugin_gitter.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_glib.py` & `apprise-1.4.0/test/test_plugin_glib.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_gnome.py` & `apprise-1.4.0/test/test_plugin_gnome.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_google_chat.py` & `apprise-1.4.0/test/test_plugin_google_chat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_gotify.py` & `apprise-1.4.0/test/test_plugin_gotify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_growl.py` & `apprise-1.4.0/test/test_plugin_growl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_guilded.py` & `apprise-1.4.0/test/test_plugin_vonage.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,165 +26,212 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-import os
 from unittest import mock
 
 import pytest
 import requests
+from json import dumps
 
-from apprise.plugins.NotifyGuilded import NotifyGuilded
+from apprise.plugins.NotifyVonage import NotifyVonage
 from helpers import AppriseURLTester
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
-# Attachment Directory
-TEST_VAR_DIR = os.path.join(os.path.dirname(__file__), 'var')
-
 # Our Testing URLs
 apprise_url_tests = (
-    ('guilded://', {
+    ('vonage://', {
+        # No API Key specified
+        'instance': TypeError,
+    }),
+    ('vonage://:@/', {
+        # invalid Auth key
+        'instance': TypeError,
+    }),
+    ('vonage://AC{}@12345678'.format('a' * 8), {
+        # Just a key provided
+        'instance': TypeError,
+    }),
+    ('vonage://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '3' * 9), {
+        # key and secret provided and from but invalid from no
+        'instance': TypeError,
+    }),
+    ('vonage://AC{}:{}@{}/?ttl=0'.format('b' * 8, 'c' * 16, '3' * 11), {
+        # Invalid ttl defined
         'instance': TypeError,
     }),
-    # An invalid url
-    ('guilded://:@/', {
+    ('vonage://AC{}:{}@{}'.format('d' * 8, 'e' * 16, 'a' * 11), {
+        # Invalid source number
         'instance': TypeError,
     }),
-    # No webhook_token specified
-    ('guilded://%s' % ('i' * 24), {
-        'instance': TypeError,
-    }),
-    # Provide both an webhook id and a webhook token
-    ('guilded://%s/%s' % ('i' * 24, 't' * 64), {
-        'instance': NotifyGuilded,
-        'requests_response_code': requests.codes.no_content,
-    }),
-    # Provide a temporary username
-    ('guilded://l2g@%s/%s' % ('i' * 24, 't' * 64), {
-        'instance': NotifyGuilded,
-        'requests_response_code': requests.codes.no_content,
-    }),
-    # test image= field
-    ('guilded://%s/%s?format=markdown&footer=Yes&image=Yes' % (
-        'i' * 24, 't' * 64), {
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-            # don't include an image by default
-            'include_image': False,
-    }),
-    ('guilded://%s/%s?format=markdown&footer=Yes&image=No&fields=no' % (
-        'i' * 24, 't' * 64), {
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-    }),
-    ('guilded://%s/%s?format=markdown&footer=Yes&image=Yes' % (
-        'i' * 24, 't' * 64), {
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-    }),
-    ('https://media.guilded.gg/webhooks/{}/{}'.format(
-        '0' * 10, 'B' * 40), {
-            # Native URL Support, support the provided guilded URL from their
-            # webpage.
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-    }),
-    ('guilded://%s/%s?format=markdown&avatar=No&footer=No' % (
-        'i' * 24, 't' * 64), {
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-    }),
-    # different format support
-    ('guilded://%s/%s?format=markdown' % ('i' * 24, 't' * 64), {
-        'instance': NotifyGuilded,
-        'requests_response_code': requests.codes.no_content,
-    }),
-    ('guilded://%s/%s?format=text' % ('i' * 24, 't' * 64), {
-        'instance': NotifyGuilded,
-        'requests_response_code': requests.codes.no_content,
-    }),
-    # Test with avatar URL
-    ('guilded://%s/%s?avatar_url=http://localhost/test.jpg' % (
-        'i' * 24, 't' * 64), {
-            'instance': NotifyGuilded,
-            'requests_response_code': requests.codes.no_content,
-    }),
-    # Test without image set
-    ('guilded://%s/%s' % ('i' * 24, 't' * 64), {
-        'instance': NotifyGuilded,
-        'requests_response_code': requests.codes.no_content,
-        # don't include an image by default
-        'include_image': False,
-    }),
-    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
-        'instance': NotifyGuilded,
-        # force a failure
+    ('vonage://AC{}:{}@{}/123/{}/abcd/'.format(
+        'f' * 8, 'g' * 16, '3' * 11, '9' * 15), {
+        # valid everything but target numbers
+        'instance': NotifyVonage,
+
+        # Our expected url(privacy=True) startswith() response:
+        'privacy_url': 'vonage://A...f:****@',
+    }),
+    ('vonage://AC{}:{}@{}'.format('h' * 8, 'i' * 16, '5' * 11), {
+        # using phone no with no target - we text ourselves in
+        # this case
+        'instance': NotifyVonage,
+    }),
+    ('vonage://_?key=AC{}&secret={}&from={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11), {
+        # use get args to acomplish the same thing
+        'instance': NotifyVonage,
+    }),
+    ('vonage://_?key=AC{}&secret={}&source={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11), {
+        # use get args to acomplish the same thing (use source instead of from)
+        'instance': NotifyVonage,
+    }),
+    ('vonage://_?key=AC{}&secret={}&from={}&to={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11, '7' * 13), {
+        # use to=
+        'instance': NotifyVonage,
+    }),
+    ('vonage://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '6' * 11), {
+        'instance': NotifyVonage,
+        # throw a bizzare code forcing us to fail to look it up
         'response': False,
-        'requests_response_code': requests.codes.internal_server_error,
+        'requests_response_code': 999,
     }),
-    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
-        'instance': NotifyGuilded,
+    ('vonage://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '6' * 11), {
+        'instance': NotifyVonage,
+        # Throws a series of connection and transfer exceptions when this flag
+        # is set and tests that we gracfully handle them
+        'test_requests_exceptions': True,
+    }),
+
+    # Nexmo Backwards Support
+    ('nexmo://', {
+        # No API Key specified
+        'instance': TypeError,
+    }),
+    ('nexmo://:@/', {
+        # invalid Auth key
+        'instance': TypeError,
+    }),
+    ('nexmo://AC{}@12345678'.format('a' * 8), {
+        # Just a key provided
+        'instance': TypeError,
+    }),
+    ('nexmo://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '3' * 9), {
+        # key and secret provided and from but invalid from no
+        'instance': TypeError,
+    }),
+    ('nexmo://AC{}:{}@{}/?ttl=0'.format('b' * 8, 'c' * 16, '3' * 11), {
+        # Invalid ttl defined
+        'instance': TypeError,
+    }),
+    ('nexmo://AC{}:{}@{}'.format('d' * 8, 'e' * 16, 'a' * 11), {
+        # Invalid source number
+        'instance': TypeError,
+    }),
+    ('nexmo://AC{}:{}@{}/123/{}/abcd/'.format(
+        'f' * 8, 'g' * 16, '3' * 11, '9' * 15), {
+        # valid everything but target numbers
+        'instance': NotifyVonage,
+
+        # Our expected url(privacy=True) startswith() response:
+        'privacy_url': 'vonage://A...f:****@',
+    }),
+    ('nexmo://AC{}:{}@{}'.format('h' * 8, 'i' * 16, '5' * 11), {
+        # using phone no with no target - we text ourselves in
+        # this case
+        'instance': NotifyVonage,
+    }),
+    ('nexmo://_?key=AC{}&secret={}&from={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11), {
+        # use get args to acomplish the same thing
+        'instance': NotifyVonage,
+    }),
+    ('nexmo://_?key=AC{}&secret={}&source={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11), {
+        # use get args to acomplish the same thing (use source instead of from)
+        'instance': NotifyVonage,
+    }),
+    ('nexmo://_?key=AC{}&secret={}&from={}&to={}'.format(
+        'a' * 8, 'b' * 16, '5' * 11, '7' * 13), {
+        # use to=
+        'instance': NotifyVonage,
+    }),
+    ('nexmo://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '6' * 11), {
+        'instance': NotifyVonage,
         # throw a bizzare code forcing us to fail to look it up
         'response': False,
         'requests_response_code': 999,
     }),
-    ('guilded://%s/%s/' % ('a' * 24, 'b' * 64), {
-        'instance': NotifyGuilded,
+    ('nexmo://AC{}:{}@{}'.format('a' * 8, 'b' * 16, '6' * 11), {
+        'instance': NotifyVonage,
         # Throws a series of connection and transfer exceptions when this flag
         # is set and tests that we gracfully handle them
         'test_requests_exceptions': True,
     }),
 )
 
 
-def test_plugin_guilded_urls():
+def test_plugin_vonage_urls():
     """
-    NotifyGuilded() Apprise URLs
+    NotifyVonage() Apprise URLs
 
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
 
 
 @mock.patch('requests.post')
-def test_plugin_guilded_general(mock_post):
+def test_plugin_vonage_edge_cases(mock_post):
     """
-    NotifyGuilded() General Checks
+    NotifyVonage() Edge Cases
 
     """
 
-    # Initialize some generic (but valid) tokens
-    webhook_id = 'A' * 24
-    webhook_token = 'B' * 64
+    # Prepare our response
+    response = requests.Request()
+    response.status_code = requests.codes.ok
 
     # Prepare Mock
-    mock_post.return_value = requests.Request()
-    mock_post.return_value.status_code = requests.codes.ok
+    mock_post.return_value = response
 
-    # Invalid webhook id
+    # Initialize some generic (but valid) tokens
+    apikey = 'AC{}'.format('b' * 8)
+    secret = '{}'.format('b' * 16)
+    source = '+1 (555) 123-3456'
+
+    # No apikey specified
     with pytest.raises(TypeError):
-        NotifyGuilded(webhook_id=None, webhook_token=webhook_token)
-    # Invalid webhook id (whitespace)
+        NotifyVonage(apikey=None, secret=secret, source=source)
+
     with pytest.raises(TypeError):
-        NotifyGuilded(webhook_id="  ", webhook_token=webhook_token)
+        NotifyVonage(apikey="  ", secret=secret, source=source)
 
-    # Invalid webhook token
+    # No secret specified
     with pytest.raises(TypeError):
-        NotifyGuilded(webhook_id=webhook_id, webhook_token=None)
-    # Invalid webhook token (whitespace)
+        NotifyVonage(apikey=apikey, secret=None, source=source)
+
     with pytest.raises(TypeError):
-        NotifyGuilded(webhook_id=webhook_id, webhook_token="   ")
+        NotifyVonage(apikey=apikey, secret="  ", source=source)
 
-    obj = NotifyGuilded(
-        webhook_id=webhook_id,
-        webhook_token=webhook_token,
-        footer=True, thumbnail=False)
+    # a error response
+    response.status_code = 400
+    response.content = dumps({
+        'code': 21211,
+        'message': "The 'To' number +1234567 is not a valid phone number.",
+    })
+    mock_post.return_value = response
+
+    # Initialize our object
+    obj = NotifyVonage(
+        apikey=apikey, secret=secret, source=source)
 
-    # Test that we get a string response
-    assert isinstance(obj.url(), str) is True
+    # We will fail with the above error code
+    assert obj.notify('title', 'body', 'info') is False
```

### Comparing `apprise-1.3.0/test/test_plugin_homeassistant.py` & `apprise-1.4.0/test/test_plugin_homeassistant.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_ifttt.py` & `apprise-1.4.0/test/test_plugin_ifttt.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_join.py` & `apprise-1.4.0/test/test_plugin_join.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_kavenegar.py` & `apprise-1.4.0/test/test_plugin_kavenegar.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_kumulos.py` & `apprise-1.4.0/test/test_plugin_kumulos.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_lametric.py` & `apprise-1.4.0/test/test_plugin_lametric.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_line.py` & `apprise-1.4.0/test/test_plugin_line.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_macosx.py` & `apprise-1.4.0/test/test_plugin_macosx.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_mailgun.py` & `apprise-1.4.0/test/test_plugin_mailgun.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,17 +284,23 @@
 
     # test the handling of our batch modes
     obj = Apprise.instantiate(
         'mailgun://no-reply@example.com/{}/'
         'user1@example.com/user2@example.com?batch=yes'.format(apikey))
     assert isinstance(obj, NotifyMailgun)
 
+    # objects will be combined into a single post in batch mode
+    assert len(obj) == 1
+
     # Force our batch to break into separate messages
     obj.default_batch_size = 1
-    # We'll send 2 messages
+
+    # We'll send 2 messages now
+    assert len(obj) == 2
+
     mock_post.reset_mock()
 
     assert obj.notify(
         body='body', title='title', notify_type=NotifyType.INFO,
         attach=attach) is True
     assert mock_post.call_count == 2
```

### Comparing `apprise-1.3.0/test/test_plugin_mastodon.py` & `apprise-1.4.0/test/test_plugin_mastodon.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_matrix.py` & `apprise-1.4.0/test/test_plugin_matrix.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_mattermost.py` & `apprise-1.4.0/test/test_plugin_mattermost.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_messagebird.py` & `apprise-1.4.0/test/test_plugin_messagebird.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_misskey.py` & `apprise-1.4.0/test/test_plugin_misskey.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_mqtt.py` & `apprise-1.4.0/test/test_plugin_mqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,16 @@
     Verify `NotifyMQTT` succeeds and has appropriate default settings.
     """
 
     # Instantiate the notifier.
     obj = apprise.Apprise.instantiate(
         'mqtt://localhost:1234/my/topic', suppress_exceptions=False)
     assert isinstance(obj, NotifyMQTT)
+    # We only loaded 1 topic
+    assert len(obj) == 1
     assert obj.url().startswith('mqtt://localhost:1234/my/topic')
 
     # Verify default settings.
     assert re.search(r'qos=0', obj.url())
     assert re.search(r'version=v3.1.1', obj.url())
     assert re.search(r'session=no', obj.url())
     assert re.search(r'client_id=', obj.url()) is None
@@ -131,14 +133,17 @@
     """
 
     # Designate multiple topic targets.
     obj = apprise.Apprise.instantiate(
         'mqtt://localhost/my/topic,my/other/topic',
         suppress_exceptions=False)
 
+    # Verify we have loaded 2 topics
+    assert len(obj) == 2
+
     assert isinstance(obj, NotifyMQTT)
     assert obj.url().startswith('mqtt://localhost')
     assert re.search(r'my/topic', obj.url())
     assert re.search(r'my/other/topic', obj.url())
     assert obj.notify(body="test=test") is True
 
     # Verify the right calls have been made to the MQTT client object.
```

### Comparing `apprise-1.3.0/test/test_plugin_msg91.py` & `apprise-1.4.0/test/test_plugin_msg91.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_msteams.py` & `apprise-1.4.0/test/test_plugin_msteams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_nextcloud.py` & `apprise-1.4.0/test/test_plugin_nextcloud.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_nextcloudtalk.py` & `apprise-1.4.0/test/test_plugin_nextcloudtalk.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_notica.py` & `apprise-1.4.0/test/test_plugin_notica.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_notifico.py` & `apprise-1.4.0/test/test_plugin_notifico.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_ntfy.py` & `apprise-1.4.0/test/test_plugin_ntfy.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_office365.py` & `apprise-1.4.0/test/test_plugin_office365.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_onesignal.py` & `apprise-1.4.0/test/test_plugin_ryver.py`

 * *Files 23% similar despite different names*

```diff
@@ -26,108 +26,127 @@
 # CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
 # SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
 # INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
 # CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
 # ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 # POSSIBILITY OF SUCH DAMAGE.
 
-from apprise.plugins.NotifyOneSignal import NotifyOneSignal
+import pytest
+import requests
+
+from apprise.plugins.NotifyRyver import NotifyRyver
 from helpers import AppriseURLTester
 
 # Disable logging for a cleaner testing output
 import logging
 logging.disable(logging.CRITICAL)
 
 # Our Testing URLs
 apprise_url_tests = (
-    ('onesignal://', {
-        # We failed to identify any valid authentication
+    ('ryver://', {
         'instance': TypeError,
     }),
-    ('onesignal://:@/', {
-        # We failed to identify any valid authentication
+    ('ryver://:@/', {
         'instance': TypeError,
     }),
-    ('onesignal://apikey/', {
-        # no app id specified
+    ('ryver://apprise', {
+        # Just org provided (no token)
         'instance': TypeError,
     }),
-    ('onesignal://appid@%20%20/', {
-        # invalid apikey
+    ('ryver://apprise/ckhrjW8w672m6HG?mode=invalid', {
+        # invalid mode provided
         'instance': TypeError,
     }),
-    ('onesignal://appid@apikey/playerid/?lang=X', {
-        # invalid language id (must be 2 characters)
+    ('ryver://x/ckhrjW8w672m6HG?mode=slack', {
+        # Invalid org
         'instance': TypeError,
     }),
-    ('onesignal://appid@apikey/', {
-        # No targets specified; we will initialize but not notify anything
-        'instance': NotifyOneSignal,
-        'notify_response': False,
-    }),
-    ('onesignal://appid@apikey/playerid', {
-        # Valid playerid
-        'instance': NotifyOneSignal,
-        'privacy_url': 'onesignal://a...d@a...y/playerid',
-    }),
-    ('onesignal://appid@apikey/player', {
-        # Valid player id
-        'instance': NotifyOneSignal,
+    ('ryver://apprise/ckhrjW8w672m6HG?mode=slack', {
+        # No username specified; this is still okay as we use whatever
+        # the user told the webhook to use; set our slack mode
+        'instance': NotifyRyver,
+    }),
+    ('ryver://apprise/ckhrjW8w672m6HG?mode=ryver', {
+        # No username specified; this is still okay as we use whatever
+        # the user told the webhook to use; set our ryver mode
+        'instance': NotifyRyver,
+    }),
+    # Legacy webhook mode setting:
+    # Legacy webhook mode setting:
+    ('ryver://apprise/ckhrjW8w672m6HG?webhook=slack', {
+        # No username specified; this is still okay as we use whatever
+        # the user told the webhook to use; set our slack mode
+        'instance': NotifyRyver,
+    }),
+    ('ryver://apprise/ckhrjW8w672m6HG?webhook=ryver', {
+        # No username specified; this is still okay as we use whatever
+        # the user told the webhook to use; set our ryver mode
+        'instance': NotifyRyver,
+
+        # Our expected url(privacy=True) startswith() response:
+        'privacy_url': 'ryver://apprise/c...G',
+    }),
+    # Support Native URLs
+    ('https://apprise.ryver.com/application/webhook/ckhrjW8w672m6HG', {
+        'instance': NotifyRyver,
+    }),
+    # Support Native URLs with arguments
+    ('https://apprise.ryver.com/application/webhook/ckhrjW8w672m6HG'
+     '?webhook=ryver',
+        {
+            'instance': NotifyRyver,
+        }),
+    ('ryver://caronc@apprise/ckhrjW8w672m6HG', {
+        'instance': NotifyRyver,
         # don't include an image by default
         'include_image': False,
     }),
-    ('onesignal://appid@apikey/@user?image=no', {
-        # Valid userid, no image
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://appid@apikey/user@email.com/#seg/player/@user/%20/a', {
-        # Valid email, valid playerid, valid user, invalid entry (%20),
-        # and too short of an entry (a)
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://appid@apikey?to=#segment,playerid', {
-        # Test to=
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://appid@apikey/#segment/@user/?batch=yes', {
-        # Test batch=
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://appid@apikey/#segment/@user/?batch=no', {
-        # Test batch=
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://templateid:appid@apikey/playerid', {
-        # Test Template ID
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://appid@apikey/playerid/?lang=es&subtitle=Sub', {
-        # Test Language and Subtitle Over-ride
-        'instance': NotifyOneSignal,
-    }),
-    ('onesignal://?apikey=abc&template=tp&app=123&to=playerid', {
-        # Test Kwargs
-        'instance': NotifyOneSignal,
+    ('ryver://apprise/ckhrjW8w672m6HG', {
+        'instance': NotifyRyver,
+        # force a failure
+        'response': False,
+        'requests_response_code': requests.codes.internal_server_error,
     }),
-    ('onesignal://appid@apikey/#segment/playerid/', {
-        'instance': NotifyOneSignal,
+    ('ryver://apprise/ckhrjW8w672m6HG', {
+        'instance': NotifyRyver,
         # throw a bizzare code forcing us to fail to look it up
         'response': False,
         'requests_response_code': 999,
     }),
-    ('onesignal://appid@apikey/#segment/playerid/', {
-        'instance': NotifyOneSignal,
+    ('ryver://apprise/ckhrjW8w672m6HG', {
+        'instance': NotifyRyver,
         # Throws a series of connection and transfer exceptions when this flag
         # is set and tests that we gracfully handle them
         'test_requests_exceptions': True,
     }),
 )
 
 
-def test_plugin_onesignal_urls():
+def test_plugin_ryver_urls():
     """
-    NotifyOneSignal() Apprise URLs
+    NotifyRyver() Apprise URLs
 
     """
 
     # Run our general tests
     AppriseURLTester(tests=apprise_url_tests).run_all()
+
+
+def test_plugin_ryver_edge_cases():
+    """
+    NotifyRyver() Edge Cases
+
+    """
+
+    # No token
+    with pytest.raises(TypeError):
+        NotifyRyver(organization="abc", token=None)
+
+    with pytest.raises(TypeError):
+        NotifyRyver(organization="abc", token="  ")
+
+    # No organization
+    with pytest.raises(TypeError):
+        NotifyRyver(organization=None, token="abc")
+
+    with pytest.raises(TypeError):
+        NotifyRyver(organization="  ", token="abc")
```

### Comparing `apprise-1.3.0/test/test_plugin_opsgenie.py` & `apprise-1.4.0/test/test_plugin_opsgenie.py`

 * *Files 9% similar despite different names*

```diff
@@ -97,16 +97,23 @@
         'instance': NotifyOpsgenie,
     }),
     ('opsgenie://apikey/user@email.com/#team/*sche/^esc/%20/a', {
         # Valid user (email), valid schedule, Escalated ID,
         # an invalid entry (%20), and too short of an entry (a)
         'instance': NotifyOpsgenie,
     }),
-    ('opsgenie://apikey/{}/@{}/#{}/*{}/^{}/'.format(
-        UUID4, UUID4, UUID4, UUID4, UUID4), {
+    ('opsgenie://apikey/@{}/#{}/*{}/^{}/'.format(
+        UUID4, UUID4, UUID4, UUID4), {
+        # similar to the above, except we use the UUID's
+        'instance': NotifyOpsgenie,
+    }),
+    # Same link as before but @ missing at the front causing an ambigious
+    # lookup however the entry is treated a though a @ was in front (user)
+    ('opsgenie://apikey/{}/#{}/*{}/^{}/'.format(
+        UUID4, UUID4, UUID4, UUID4), {
         # similar to the above, except we use the UUID's
         'instance': NotifyOpsgenie,
     }),
     ('opsgenie://apikey?to=#team,user&+key=value&+type=override', {
         # Test to= and details (key/value pair) also override 'type'
         'instance': NotifyOpsgenie,
     }),
```

### Comparing `apprise-1.3.0/test/test_plugin_pagerduty.py` & `apprise-1.4.0/test/test_plugin_pagerduty.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pagertree.py` & `apprise-1.4.0/test/test_plugin_pagertree.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_parse_platform.py` & `apprise-1.4.0/test/test_plugin_parse_platform.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_popcorn_notify.py` & `apprise-1.4.0/test/test_plugin_popcorn_notify.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_prowl.py` & `apprise-1.4.0/test/test_plugin_prowl.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pushbullet.py` & `apprise-1.4.0/test/test_plugin_pushbullet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pushed.py` & `apprise-1.4.0/test/test_plugin_pushed.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pushjet.py` & `apprise-1.4.0/test/test_plugin_pushjet.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pushover.py` & `apprise-1.4.0/test/test_plugin_pushover.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_pushsafer.py` & `apprise-1.4.0/test/test_plugin_pushsafer.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_reddit.py` & `apprise-1.4.0/test/test_plugin_reddit.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_rocket_chat.py` & `apprise-1.4.0/test/test_plugin_rocket_chat.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_sendgrid.py` & `apprise-1.4.0/test/test_plugin_sendgrid.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_serverchan.py` & `apprise-1.4.0/test/test_plugin_serverchan.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_ses.py` & `apprise-1.4.0/test/test_plugin_ses.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_signal.py` & `apprise-1.4.0/test/test_plugin_signal.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_simplepush.py` & `apprise-1.4.0/test/test_plugin_simplepush.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_sinch.py` & `apprise-1.4.0/test/test_plugin_sinch.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_slack.py` & `apprise-1.4.0/test/test_plugin_slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,14 +676,18 @@
     Here is a <https://slack.com|Slack Link> we want to support as part of it's
     markdown.
 
     This one has arguments we want to preserve:
        <https://slack.com?arg=val&arg2=val2|Slack Link>.
     We also want to be able to support <https://slack.com> links without the
     description.
+
+    Channel Testing
+    <!channelA>
+    <!channelA|Description>
     """)
 
     # Send our notification
     assert aobj.notify(
         body=body, title='title', notify_type=NotifyType.INFO)
 
     # We would have failed to look up the email, therefore we wouldn't have
@@ -696,8 +700,9 @@
 
     data = loads(mock_post.call_args_list[0][1]['data'])
     assert data['attachments'][0]['text'] == \
         "Here is a <https://slack.com|Slack Link> we want to support as part "\
         "of it's\nmarkdown.\n\nThis one has arguments we want to preserve:"\
         "\n   <https://slack.com?arg=val&arg2=val2|Slack Link>.\n"\
         "We also want to be able to support <https://slack.com> "\
-        "links without the\ndescription."
+        "links without the\ndescription."\
+        "\n\nChannel Testing\n<!channelA>\n<!channelA|Description>"
```

### Comparing `apprise-1.3.0/test/test_plugin_smseagle.py` & `apprise-1.4.0/test/test_plugin_smseagle.py`

 * *Files 2% similar despite different names*

```diff
@@ -295,32 +295,32 @@
     target = '+1 (555) 987-5432'
     body = "test body"
     title = "My Title"
 
     aobj = Apprise()
     assert aobj.add(
         "smseagles://token@localhost:231/{}".format(target))
+    assert len(aobj) == 1
     assert aobj.notify(title=title, body=body)
-
     assert mock_post.call_count == 1
 
     details = mock_post.call_args_list[0]
     assert details[0][0] == 'https://localhost:231/jsonrpc/sms'
     payload = loads(details[1]['data'])
     assert payload['params']['message'] == 'My Title\r\ntest body'
 
     # Reset our mock object
     mock_post.reset_mock()
 
     aobj = Apprise()
     assert aobj.add(
         "smseagles://token@localhost:231/{}?status=Yes".format(
             target))
+    assert len(aobj) == 1
     assert aobj.notify(title=title, body=body)
-
     assert mock_post.call_count == 1
 
     details = mock_post.call_args_list[0]
     assert details[0][0] == 'https://localhost:231/jsonrpc/sms'
     payload = loads(details[1]['data'])
     # Status flag is set
     assert payload['params']['message'] == '[i] My Title\r\ntest body'
@@ -344,14 +344,16 @@
     body = "test body"
     title = "My Title"
 
     aobj = Apprise()
     aobj.add(
         'smseagle://token@10.0.0.112:8080/+12512222222/+12513333333/'
         '12514444444?batch=yes')
+    # In a batch mode we can shove them all into 1 call
+    assert len(aobj[0]) == 1
 
     assert aobj.notify(title=title, body=body)
 
     # If a batch, there is only 1 post
     assert mock_post.call_count == 1
 
     details = mock_post.call_args_list[0]
@@ -382,14 +384,15 @@
     # Reset our test and turn batch mode off
     mock_post.reset_mock()
 
     aobj = Apprise()
     aobj.add(
         'smseagle://token@10.0.0.112:8080/#group/Contact/'
         '123456789?batch=no')
+    assert len(aobj[0]) == 3
 
     assert aobj.notify(title=title, body=body)
 
     # If batch is off then there is a post per entry
     assert mock_post.call_count == 3
 
     details = mock_post.call_args_list[0]
@@ -459,14 +462,16 @@
 
     # Test groups and contact names
     aobj = Apprise()
     aobj.add(
         'smseagle://token@10.0.0.112:8080/513333333/#group1/@contact1/'
         'contact2/12514444444?batch=yes')
 
+    # contacts and numbers can be combined and is calculated in batch response
+    assert len(aobj[0]) == 3
     assert aobj.notify(title=title, body=body)
 
     # There is a unique post to each (group, contact x2, and phone x2)
     # The key is the contacts were grouped here in 1 post each
     assert mock_post.call_count == 3
 
     details = mock_post.call_args_list[0]
```

### Comparing `apprise-1.3.0/test/test_plugin_smtp2go.py` & `apprise-1.4.0/test/test_plugin_smtp2go.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,17 +221,23 @@
 
     # test the handling of our batch modes
     obj = Apprise.instantiate(
         'smtp2go://no-reply@example.com/{}/'
         'user1@example.com/user2@example.com?batch=yes'.format(apikey))
     assert isinstance(obj, NotifySMTP2Go)
 
+    # objects will be combined into a single post in batch mode
+    assert len(obj) == 1
+
     # Force our batch to break into separate messages
     obj.default_batch_size = 1
-    # We'll send 2 messages
+
+    # We'll send 2 messages now
+    assert len(obj) == 2
+
     mock_post.reset_mock()
 
     assert obj.notify(
         body='body', title='title', notify_type=NotifyType.INFO,
         attach=attach) is True
     assert mock_post.call_count == 2
```

### Comparing `apprise-1.3.0/test/test_plugin_sns.py` & `apprise-1.4.0/test/test_plugin_sns.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_sparkpost.py` & `apprise-1.4.0/test/test_plugin_sparkpost.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,17 +387,22 @@
             attach=attach) is False
 
     obj = Apprise.instantiate(
         'sparkpost://no-reply@example.com/{}/'
         'user1@example.com/user2@example.com?batch=yes'.format(apikey))
     assert isinstance(obj, NotifySparkPost)
 
+    # As a batch mode, both emails can be lumped into 1
+    assert len(obj) == 1
+
     # Force our batch to break into separate messages
     obj.default_batch_size = 1
-    # We'll send 2 messages
+
+    # We'll send 2 messages no
+    assert len(obj) == 2
     mock_post.reset_mock()
 
     assert obj.notify(
         body='body', title='title', notify_type=NotifyType.INFO,
         attach=attach) is True
     assert mock_post.call_count == 2
```

### Comparing `apprise-1.3.0/test/test_plugin_spontit.py` & `apprise-1.4.0/test/test_plugin_spontit.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_streamlabs.py` & `apprise-1.4.0/test/test_plugin_streamlabs.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_syslog.py` & `apprise-1.4.0/test/test_plugin_syslog.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_techululs_push.py` & `apprise-1.4.0/test/test_plugin_techululs_push.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_telegram.py` & `apprise-1.4.0/test/test_plugin_telegram.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,14 +94,22 @@
         # don't include an image by default
         'include_image': False,
     }),
     # Support bot keyword prefix
     ('tgram://bottest@123456789:abcdefg_hijklmnop/lead2gold/', {
         'instance': NotifyTelegram,
     }),
+    # Support Thread Topics
+    ('tgram://bottest@123456789:abcdefg_hijklmnop/id1/?topic=12345', {
+        'instance': NotifyTelegram,
+    }),
+    # Threads must be numeric
+    ('tgram://bottest@123456789:abcdefg_hijklmnop/id1/?topic=invalid', {
+        'instance': TypeError,
+    }),
     # Testing image
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?image=Yes', {
         'instance': NotifyTelegram,
     }),
     # Testing invalid format (fall's back to html)
     ('tgram://123456789:abcdefg_hijklmnop/lead2gold/?format=invalid', {
         'instance': NotifyTelegram,
```

### Comparing `apprise-1.3.0/test/test_plugin_twilio.py` & `apprise-1.4.0/test/test_plugin_twilio.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_twist.py` & `apprise-1.4.0/test/test_plugin_twist.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_twitter.py` & `apprise-1.4.0/test/test_plugin_twitter.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_voipms.py` & `apprise-1.4.0/test/test_plugin_voipms.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_webex_teams.py` & `apprise-1.4.0/test/test_plugin_webex_teams.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_windows.py` & `apprise-1.4.0/test/test_plugin_windows.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_xbmc_kodi.py` & `apprise-1.4.0/test/test_plugin_xbmc_kodi.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_plugin_zulip.py` & `apprise-1.4.0/test/test_plugin_zulip.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/test_rest_plugins.py` & `apprise-1.4.0/test/test_rest_plugins.py`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/01_test_example.html` & `apprise-1.4.0/test/var/01_test_example.html`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/apprise-test.gif` & `apprise-1.4.0/test/var/apprise-test.gif`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/apprise-test.jpeg` & `apprise-1.4.0/test/var/apprise-test.jpeg`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/apprise-test.mp4` & `apprise-1.4.0/test/var/apprise-test.mp4`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/apprise-test.png` & `apprise-1.4.0/test/var/apprise-test.png`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/fcm/service_account-bad-type.json` & `apprise-1.4.0/test/var/fcm/service_account-bad-type.json`

 * *Files identical despite different names*

### Comparing `apprise-1.3.0/test/var/fcm/service_account.json` & `apprise-1.4.0/test/var/fcm/service_account.json`

 * *Files identical despite different names*

