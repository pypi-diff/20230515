# Comparing `tmp/ukitai-0.1.2.tar.gz` & `tmp/ukitai-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ukitai-0.1.2.tar", last modified: Wed May 19 07:41:34 2021, max compression
+gzip compressed data, last modified: Mon May 15 06:37:11 2023, from Unix
```

## Comparing `ukitai-0.1.2.tar` & `ukitai-0.1.5.tar`

### file list

```diff
@@ -1,68 +1,134 @@
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.682269 ukitai-0.1.2/
--rw-rw-r--   0 bright.lin   (501) staff       (20)      316 2021-05-12 02:44:59.000000 ukitai-0.1.2/MANIFEST.in
--rw-r--r--   0 bright.lin   (501) staff       (20)      218 2021-05-19 07:41:34.682402 ukitai-0.1.2/PKG-INFO
--rw-r--r--   0 bright.lin   (501) staff       (20)     1774 2021-05-19 07:32:52.000000 ukitai-0.1.2/README.md
--rw-r--r--   0 bright.lin   (501) staff       (20)      145 2021-05-19 07:32:52.000000 ukitai-0.1.2/pyproject.toml
--rw-rw-r--   0 bright.lin   (501) staff       (20)       38 2021-05-19 07:41:34.682891 ukitai-0.1.2/setup.cfg
--rw-rw-r--   0 bright.lin   (501) staff       (20)      990 2021-05-19 07:28:59.000000 ukitai-0.1.2/setup.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.656681 ukitai-0.1.2/ukitai/
--rw-rw-r--   0 bright.lin   (501) staff       (20)      103 2021-05-19 07:28:59.000000 ukitai-0.1.2/ukitai/__init__.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.664391 ukitai-0.1.2/ukitai/apis/
--rw-rw-r--   0 bright.lin   (501) staff       (20)    12308 2021-05-06 07:24:09.000000 ukitai-0.1.2/ukitai/apis/Audio.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     1115 2021-04-30 03:10:51.000000 ukitai-0.1.2/ukitai/apis/Battery.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     1598 2021-04-30 03:04:24.000000 ukitai-0.1.2/ukitai/apis/ColorSensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     4183 2021-05-06 07:44:48.000000 ukitai-0.1.2/ukitai/apis/CommonApi.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     1108 2021-04-30 02:46:39.000000 ukitai-0.1.2/ukitai/apis/HumiditySensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      883 2021-04-30 03:05:07.000000 ukitai-0.1.2/ukitai/apis/InfraredSensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     6112 2021-05-06 04:25:28.000000 ukitai-0.1.2/ukitai/apis/LedBox.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     4073 2021-04-30 07:39:36.000000 ukitai-0.1.2/ukitai/apis/LedEyes.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      407 2021-04-30 03:07:11.000000 ukitai-0.1.2/ukitai/apis/LuxSensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2641 2021-04-29 11:14:57.000000 ukitai-0.1.2/ukitai/apis/Motor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    10150 2021-05-06 10:26:56.000000 ukitai-0.1.2/ukitai/apis/Screen.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     6080 2021-04-29 11:18:11.000000 ukitai-0.1.2/ukitai/apis/Servo.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      420 2021-04-30 03:08:03.000000 ukitai-0.1.2/ukitai/apis/SoundSensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      928 2021-04-30 03:11:42.000000 ukitai-0.1.2/ukitai/apis/TouchSensor.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2240 2021-04-30 03:17:18.000000 ukitai-0.1.2/ukitai/apis/Ultrasonic.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    16798 2021-05-07 08:44:37.000000 ukitai-0.1.2/ukitai/apis/Vision.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      537 2021-05-06 11:04:46.000000 ukitai-0.1.2/ukitai/apis/__init__.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.666135 ukitai-0.1.2/ukitai/common/
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2989 2021-04-30 03:21:29.000000 ukitai-0.1.2/ukitai/common/Color.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     1176 2021-05-06 07:50:57.000000 ukitai-0.1.2/ukitai/common/Common.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      253 2021-05-12 02:49:57.000000 ukitai-0.1.2/ukitai/common/CompType.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      265 2021-04-29 08:45:31.000000 ukitai-0.1.2/ukitai/common/DataType.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      131 2021-04-29 06:32:44.000000 ukitai-0.1.2/ukitai/common/RangMode.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      171 2021-04-29 09:06:37.000000 ukitai-0.1.2/ukitai/common/__init__.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.667738 ukitai-0.1.2/ukitai/depend/
--rw-rw-r--   0 bright.lin   (501) staff       (20)       40 2021-04-26 10:01:07.000000 ukitai-0.1.2/ukitai/depend/__init__.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     5261 2021-05-08 02:49:03.000000 ukitai-0.1.2/ukitai/depend/binaries.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)  3591442 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/depend/filecontents.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.674933 ukitai-0.1.2/ukitai/link/
--rw-rw-r--   0 bright.lin   (501) staff       (20)      468 2021-04-30 04:13:05.000000 ukitai-0.1.2/ukitai/link/LinkInterface.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)      153 2021-04-29 09:06:20.000000 ukitai-0.1.2/ukitai/link/__init__.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    11944 2021-05-08 11:09:32.000000 ukitai-0.1.2/ukitai/link/uKitAiBleLink.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     9381 2021-05-07 08:33:44.000000 ukitai-0.1.2/ukitai/link/uKitAiLink.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     3318 2021-04-29 08:37:39.000000 ukitai-0.1.2/ukitai/link/uKitAiSerialLink.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.682016 ukitai-0.1.2/ukitai/protos/
--rw-rw-r--   0 bright.lin   (501) staff       (20)      374 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/__init__.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2918 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d11_Luxmeter_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    35247 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d1A_LedBelt_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    27299 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d1B_Lcd_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    13206 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d20_VisionModule_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    10947 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d3_Servo_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     6929 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d4_Motor_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2826 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d5_Infrared_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     3106 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d6_TempHum_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2970 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d7_Sound_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     7947 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d8_Led_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     6766 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/d9_Ultrasonic_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2873 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/dB_TouchSwitch_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     2819 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/dD_Color_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)    35973 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/dE_VoiceRecognition_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     5403 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/dF_Battery_pb2.py
--rw-rw-r--   0 bright.lin   (501) staff       (20)     5264 2021-05-19 07:28:55.000000 ukitai-0.1.2/ukitai/protos/header_pb2.py
-drwxr-xr-x   0 bright.lin   (501) staff       (20)        0 2021-05-19 07:41:34.658561 ukitai-0.1.2/ukitai.egg-info/
--rw-rw-r--   0 bright.lin   (501) staff       (20)      218 2021-05-19 07:41:33.000000 ukitai-0.1.2/ukitai.egg-info/PKG-INFO
--rw-rw-r--   0 bright.lin   (501) staff       (20)     1557 2021-05-19 07:41:34.000000 ukitai-0.1.2/ukitai.egg-info/SOURCES.txt
--rw-rw-r--   0 bright.lin   (501) staff       (20)        1 2021-05-19 07:41:33.000000 ukitai-0.1.2/ukitai.egg-info/dependency_links.txt
--rw-rw-r--   0 bright.lin   (501) staff       (20)       35 2021-05-19 07:41:33.000000 ukitai-0.1.2/ukitai.egg-info/requires.txt
--rw-rw-r--   0 bright.lin   (501) staff       (20)        7 2021-05-19 07:41:33.000000 ukitai-0.1.2/ukitai.egg-info/top_level.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      318 2023-05-15 06:34:36.000000 ._ukitai-0.1.5
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:36.000000 ukitai-0.1.5/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:36.000000 ukitai-0.1.5/._PKG-INFO
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:36.000000 ukitai-0.1.5/PKG-INFO
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/._ukitai.egg-info
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai.egg-info/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-12 02:44:58.000000 ukitai-0.1.5/._MANIFEST.in
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      316 2021-05-12 02:44:58.000000 ukitai-0.1.5/MANIFEST.in
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:36:48.000000 ukitai-0.1.5/._README
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      116 2023-05-15 06:36:48.356332 ukitai-0.1.5/README
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:30.000000 ukitai-0.1.5/._setup.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      990 2023-05-15 06:34:30.000000 ukitai-0.1.5/setup.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:36.000000 ukitai-0.1.5/._setup.cfg
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)       38 2023-05-15 06:34:36.000000 ukitai-0.1.5/setup.cfg
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/._ukitai
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/._apis
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/apis/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:36.000000 ukitai-0.1.5/ukitai/._protos
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:36.000000 ukitai-0.1.5/ukitai/protos/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:30.000000 ukitai-0.1.5/ukitai/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      103 2023-05-15 06:34:30.000000 ukitai-0.1.5/ukitai/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/._common
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/common/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/._link
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/link/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/._depend
+drwxrwxrwx   0 bright.lin   (501) staff       (20)        0 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai/depend/
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/depend/._filecontents.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)  9057693 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/depend/filecontents.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-11-24 10:08:18.000000 ukitai-0.1.5/ukitai/depend/._binaries.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     5372 2021-11-24 10:08:18.000000 ukitai-0.1.5/ukitai/depend/binaries.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-26 10:01:06.000000 ukitai-0.1.5/ukitai/depend/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)       40 2021-04-26 10:01:06.000000 ukitai-0.1.5/ukitai/depend/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2022-07-08 08:24:44.000000 ukitai-0.1.5/ukitai/link/._uKitAiBleLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)    12379 2022-07-08 08:24:44.000000 ukitai-0.1.5/ukitai/link/uKitAiBleLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 09:06:20.000000 ukitai-0.1.5/ukitai/link/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      153 2021-04-29 09:06:20.000000 ukitai-0.1.5/ukitai/link/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-11-17 03:31:26.000000 ukitai-0.1.5/ukitai/link/._uKitAiSerialLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     3716 2021-11-17 03:31:26.000000 ukitai-0.1.5/ukitai/link/uKitAiSerialLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-07 08:33:44.000000 ukitai-0.1.5/ukitai/link/._uKitAiLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     9381 2021-05-07 08:33:44.000000 ukitai-0.1.5/ukitai/link/uKitAiLink.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 04:13:04.000000 ukitai-0.1.5/ukitai/link/._LinkInterface.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      468 2021-04-30 04:13:04.000000 ukitai-0.1.5/ukitai/link/LinkInterface.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 06:32:44.000000 ukitai-0.1.5/ukitai/common/._RangMode.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      131 2021-04-29 06:32:44.000000 ukitai-0.1.5/ukitai/common/RangMode.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:21:28.000000 ukitai-0.1.5/ukitai/common/._Color.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     2989 2021-04-30 03:21:28.000000 ukitai-0.1.5/ukitai/common/Color.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 09:06:36.000000 ukitai-0.1.5/ukitai/common/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      171 2021-04-29 09:06:36.000000 ukitai-0.1.5/ukitai/common/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-12 02:49:56.000000 ukitai-0.1.5/ukitai/common/._CompType.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      253 2021-05-12 02:49:56.000000 ukitai-0.1.5/ukitai/common/CompType.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 07:50:56.000000 ukitai-0.1.5/ukitai/common/._Common.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1176 2021-05-06 07:50:56.000000 ukitai-0.1.5/ukitai/common/Common.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 08:45:30.000000 ukitai-0.1.5/ukitai/common/._DataType.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      265 2021-04-29 08:45:30.000000 ukitai-0.1.5/ukitai/common/DataType.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._dF_Battery_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1562 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/dF_Battery_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d5_Infrared_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1156 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d5_Infrared_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d1A_LedBelt_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     6026 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d1A_LedBelt_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d7_Sound_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1185 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d7_Sound_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._dD_Color_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1146 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/dD_Color_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._dE_VoiceRecognition_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     6314 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/dE_VoiceRecognition_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d1B_Lcd_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     4856 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d1B_Lcd_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._header_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1455 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/header_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d20_VisionModule_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     2515 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d20_VisionModule_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      374 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d11_Luxmeter_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1184 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d11_Luxmeter_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._dB_TouchSwitch_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1171 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/dB_TouchSwitch_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d6_TempHum_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1169 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d6_TempHum_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d4_Motor_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1804 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d4_Motor_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d3_Servo_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     2344 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d3_Servo_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d8_Led_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1887 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d8_Led_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/._d9_Ultrasonic_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1665 2023-05-15 06:34:26.000000 ukitai-0.1.5/ukitai/protos/d9_Ultrasonic_pb2.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:07:10.000000 ukitai-0.1.5/ukitai/apis/._LuxSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      407 2021-04-30 03:07:10.000000 ukitai-0.1.5/ukitai/apis/LuxSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 10:26:56.000000 ukitai-0.1.5/ukitai/apis/._Screen.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)    10150 2021-05-06 10:26:56.000000 ukitai-0.1.5/ukitai/apis/Screen.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 07:39:36.000000 ukitai-0.1.5/ukitai/apis/._LedEyes.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     4073 2021-04-30 07:39:36.000000 ukitai-0.1.5/ukitai/apis/LedEyes.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:08:02.000000 ukitai-0.1.5/ukitai/apis/._SoundSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      420 2021-04-30 03:08:02.000000 ukitai-0.1.5/ukitai/apis/SoundSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 11:18:10.000000 ukitai-0.1.5/ukitai/apis/._Servo.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     6080 2021-04-29 11:18:10.000000 ukitai-0.1.5/ukitai/apis/Servo.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-29 11:14:56.000000 ukitai-0.1.5/ukitai/apis/._Motor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     2641 2021-04-29 11:14:56.000000 ukitai-0.1.5/ukitai/apis/Motor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-07 08:44:36.000000 ukitai-0.1.5/ukitai/apis/._Vision.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)    16798 2021-05-07 08:44:36.000000 ukitai-0.1.5/ukitai/apis/Vision.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:17:18.000000 ukitai-0.1.5/ukitai/apis/._Ultrasonic.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     2240 2021-04-30 03:17:18.000000 ukitai-0.1.5/ukitai/apis/Ultrasonic.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:04:24.000000 ukitai-0.1.5/ukitai/apis/._ColorSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1598 2021-04-30 03:04:24.000000 ukitai-0.1.5/ukitai/apis/ColorSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:10:50.000000 ukitai-0.1.5/ukitai/apis/._Battery.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1115 2021-04-30 03:10:50.000000 ukitai-0.1.5/ukitai/apis/Battery.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 04:25:28.000000 ukitai-0.1.5/ukitai/apis/._LedBox.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     6112 2021-05-06 04:25:28.000000 ukitai-0.1.5/ukitai/apis/LedBox.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 11:04:46.000000 ukitai-0.1.5/ukitai/apis/.___init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      537 2021-05-06 11:04:46.000000 ukitai-0.1.5/ukitai/apis/__init__.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:11:42.000000 ukitai-0.1.5/ukitai/apis/._TouchSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      928 2021-04-30 03:11:42.000000 ukitai-0.1.5/ukitai/apis/TouchSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 02:46:38.000000 ukitai-0.1.5/ukitai/apis/._HumiditySensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1108 2021-04-30 02:46:38.000000 ukitai-0.1.5/ukitai/apis/HumiditySensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 07:44:48.000000 ukitai-0.1.5/ukitai/apis/._CommonApi.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     4183 2021-05-06 07:44:48.000000 ukitai-0.1.5/ukitai/apis/CommonApi.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-04-30 03:05:06.000000 ukitai-0.1.5/ukitai/apis/._InfraredSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      883 2021-04-30 03:05:06.000000 ukitai-0.1.5/ukitai/apis/InfraredSensor.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2021-05-06 07:24:08.000000 ukitai-0.1.5/ukitai/apis/._Audio.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)    12308 2021-05-06 07:24:08.000000 ukitai-0.1.5/ukitai/apis/Audio.py
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/._PKG-INFO
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/PKG-INFO
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai.egg-info/._SOURCES.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)     1529 2023-05-15 06:34:34.000000 ukitai-0.1.5/ukitai.egg-info/SOURCES.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/._requires.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)       35 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/requires.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/._top_level.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)        7 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/top_level.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)      218 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/._dependency_links.txt
+-rwxrwxrwx   0 bright.lin   (501) staff       (20)        1 2023-05-15 06:34:32.000000 ukitai-0.1.5/ukitai.egg-info/dependency_links.txt
```

### Comparing `ukitai-0.1.2/setup.py` & `ukitai-0.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 
 name = 'ukitai'
-version = '0.1.2'
+version = '0.1.5'
 description = 'Python SDK for uKit AI'
 author = 'naOKi Chan'
 author_email = 'eduswengineers@ubtrobot.com'
 
 packages = [
     'ukitai',
     'ukitai.apis',
```

### Comparing `ukitai-0.1.2/ukitai/apis/Audio.py` & `ukitai-0.1.5/ukitai/apis/Audio.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Battery.py` & `ukitai-0.1.5/ukitai/apis/Battery.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/ColorSensor.py` & `ukitai-0.1.5/ukitai/apis/ColorSensor.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/CommonApi.py` & `ukitai-0.1.5/ukitai/apis/CommonApi.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/HumiditySensor.py` & `ukitai-0.1.5/ukitai/apis/HumiditySensor.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/InfraredSensor.py` & `ukitai-0.1.5/ukitai/apis/InfraredSensor.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/LedBox.py` & `ukitai-0.1.5/ukitai/apis/LedBox.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/LedEyes.py` & `ukitai-0.1.5/ukitai/apis/LedEyes.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Motor.py` & `ukitai-0.1.5/ukitai/apis/Motor.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Screen.py` & `ukitai-0.1.5/ukitai/apis/Screen.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Servo.py` & `ukitai-0.1.5/ukitai/apis/Servo.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/TouchSensor.py` & `ukitai-0.1.5/ukitai/apis/TouchSensor.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Ultrasonic.py` & `ukitai-0.1.5/ukitai/apis/Ultrasonic.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/Vision.py` & `ukitai-0.1.5/ukitai/apis/Vision.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/apis/__init__.py` & `ukitai-0.1.5/ukitai/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/common/Color.py` & `ukitai-0.1.5/ukitai/common/Color.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/common/Common.py` & `ukitai-0.1.5/ukitai/common/Common.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/depend/binaries.py` & `ukitai-0.1.5/ukitai/depend/binaries.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,9 +156,11 @@
         os.rename(logPath, logPath + ".last")
     if os.path.exists(errLogPath):
         if os.path.exists(errLogPath + ".last"):
             os.remove(errLogPath + ".last")
         os.rename(errLogPath, errLogPath + ".last")
     if isWindows:
         subprocess.call("\"{}\" {} >>\"{}\" 2>>\"{}\"".format(linkPath, logLevel, logPath, errLogPath), shell=True)
-    elif isDarwin or isLinux:
+    elif isDarwin:
+        subprocess.call("\"{}\" {} \"{}\" > /dev/null".format(linkPath, logLevel, logPath), shell=True)
+    elif isLinux:
         subprocess.call("\"{}\" {} 2>&1 | tee \"{}\" > /dev/null".format(linkPath, logLevel, logPath), shell=True)
```

### Comparing `ukitai-0.1.2/ukitai/link/uKitAiBleLink.py` & `ukitai-0.1.5/ukitai/link/uKitAiBleLink.py`

 * *Files 4% similar despite different names*

```diff
@@ -186,15 +186,15 @@
         """判断是否已经和目标设备成功建立连接
 
         返回值说明:
             (bool): 是否已经成功连接设备
         """
         return self._websocket and self._ws_connected and self._ble_connected
 
-    def open(self, timeout: float = 10, **kw参数值说明) -> bool:
+    def open(self, timeout: float = 10, **kwargs) -> bool:
         """与目标设备建立连接
 
         参数值说明:
             timeout (float): 超时时间，单位秒
 
         返回值说明:
             (bool): 是否已经成功连接设备
@@ -235,24 +235,25 @@
             self._websocket.send(self._makeRequest("write", params={
                 "serviceId": uKitAiBleLink._GATT_SERVICE_UUID,
                 "characteristicId": uKitAiBleLink._GATT_WRITE_CHARACTERISTIC_UUID,
                 "message": intArray
             }))
 
 
-def listDevices(timeout_ms: int = 15000) -> None:
+def getDevices(timeout_ms: int = 10000) -> None:
     """列出当前通过蓝牙扫描的所有uKitAi设备信息
 
     参数值说明:
         timeout_ms(int): 超时时间，单位毫秒
 
     返回值说明:
-        (None): 通过控制台显示结果
+        (list): 设备信息列表
     """
     ws = None
+    deviceInfos = []
     try:
         _prepare_server()
         ws = websocket.create_connection(_ws_url)
 
         def timeout_callback(ws, timeout_ms):
             if ws:
                 time.sleep(timeout_ms / 1000.0)
@@ -261,39 +262,54 @@
         _thread.start_new_thread(timeout_callback, (ws, timeout_ms))
 
         ws.send(_makeRequest("discover", params={
             "filters": [{"namePrefix": "uKit2_"}],
             "optionalServices": [uKitAiBleLink._GATT_SERVICE_UUID]
         }))
         endtime_ms = (time.time() * 1000.0) + timeout_ms
-        index = 0
         devices = []
         while True:
             remaining = endtime_ms - (time.time() * 1000.0)
             if remaining <= 0.0:
-                return
+                break
             try:
                 message = ws.recv()
                 response = json.loads(message)
                 method = response.get('method')
                 if method != 'didDiscoverPeripheral':
                     continue
                 params = response.get('params')
                 name = params.get('name')
                 mac = _id2mac(params.get('peripheralId'))
                 if mac in devices:
                     continue
                 devices.append(mac)
-                index = index + 1
-                print("Device %d: %s\n\t%s" % (index, name, mac))
+                deviceInfos.append({'name': name, 'mac': mac})
             except Exception:
                 continue
     finally:
         if ws:
             ws.close()
+    return deviceInfos
+
+
+def listDevices(timeout_ms: int = 10000) -> None:
+    """列出当前通过蓝牙扫描的所有uKitAi设备信息
+
+    参数值说明:
+        timeout_ms(int): 超时时间，单位毫秒
+
+    返回值说明:
+        (None): 通过控制台显示结果
+    """
+    index = 0
+    deviceInfos = getDevices(timeout_ms)
+    for deviceInfo in deviceInfos:
+        index = index + 1
+        print("Device %d: %s\n\t%s" % (index, deviceInfo['name'], deviceInfo['mac']))
 
 
 def _prepare_server():
     _serverLock = threading.Lock()
     try:
         def __check_server(lock):
             endtime_ms = (time.time() * 1000.0) + 10000
```

### Comparing `ukitai-0.1.2/ukitai/link/uKitAiLink.py` & `ukitai-0.1.5/ukitai/link/uKitAiLink.py`

 * *Files identical despite different names*

### Comparing `ukitai-0.1.2/ukitai/link/uKitAiSerialLink.py` & `ukitai-0.1.5/ukitai/link/uKitAiSerialLink.py`

 * *Files 22% similar despite different names*

```diff
@@ -75,30 +75,43 @@
                 return self._serial.write(data)
             else:
                 return -1
         except Exception:
             return -1
 
 
-def listDevices():
+def getDevices():
     """列出当前通过串口识别到的所有uKitAi设备信息
 
-    返回值说明:
-        (None): 通过控制台显示结果
-    """
+        返回值说明:
+            (list): 设备信息列表
+        """
+    deviceInfos = []
     try:
-        index = 0
         port_list = list(serial.tools.list_ports.comports())
         if len(port_list) > 0:
             for dev in list(port_list):
                 if dev.vid == 0x0403 and dev.pid == 0x6001:
-                    index = index + 1
-                    print("Device %d: %s %s\n\t%s" % (index, dev.manufacturer, dev.product, dev.device))
+                    deviceInfos.append({'manufacturer': dev.manufacturer, 'product': dev.product, 'device': dev.device})
     except Exception:
         pass
+    return deviceInfos
+
+
+def listDevices():
+    """列出当前通过串口识别到的所有uKitAi设备信息
+
+    返回值说明:
+        (None): 通过控制台显示结果
+    """
+    index = 0
+    deviceInfos = getDevices()
+    for deviceInfo in deviceInfos:
+        index = index + 1
+        print("Device %d: %s %s\n\t%s" % (index, deviceInfo['manufacturer'], deviceInfo['product'], deviceInfo['device']))
 
 
 def create(port: str = None) -> uKitAiSerialLink:
     """创建一个uKitAi串口连接对象
 
     参数值说明:
         port (str): 串口设备端口
```

### Comparing `ukitai-0.1.2/ukitai.egg-info/SOURCES.txt` & `ukitai-0.1.5/ukitai.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 MANIFEST.in
-README.md
-pyproject.toml
-setup.cfg
+README
 setup.py
 ukitai/__init__.py
 ukitai.egg-info/PKG-INFO
 ukitai.egg-info/SOURCES.txt
 ukitai.egg-info/dependency_links.txt
 ukitai.egg-info/requires.txt
 ukitai.egg-info/top_level.txt
```

