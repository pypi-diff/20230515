# Comparing `tmp/ltchiptool-4.1.0.tar.gz` & `tmp/ltchiptool-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ltchiptool-4.1.0.tar", max compression
+gzip compressed data, was "ltchiptool-4.1.1.tar", max compression
```

## Comparing `ltchiptool-4.1.0.tar` & `ltchiptool-4.1.1.tar`

### file list

```diff
@@ -1,101 +1,101 @@
--rw-r--r--   0        0        0     1076 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/LICENSE
--rw-r--r--   0        0        0     2384 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/README.md
--rw-r--r--   0        0        0      376 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/__init__.py
--rw-r--r--   0        0        0     2339 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/__main__.py
--rw-r--r--   0        0        0     2517 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/dumptool.py
--rw-r--r--   0        0        0      908 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/elf2bin.py
--rw-r--r--   0        0        0      451 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/flash/__main__.py
--rw-r--r--   0        0        0     1724 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/flash/_utils.py
--rw-r--r--   0        0        0     1610 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/flash/file.py
--rw-r--r--   0        0        0     3157 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/flash/read.py
--rw-r--r--   0        0        0     7153 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/flash/write.py
--rw-r--r--   0        0        0      881 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/link2bin.py
--rw-r--r--   0        0        0     2331 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/list.py
--rw-r--r--   0        0        0      423 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/commands/soc.py
--rw-r--r--   0        0        0     2288 2023-05-13 15:36:04.671286 ltchiptool-4.1.0/ltchiptool/families.json
--rw-r--r--   0        0        0      127 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/__init__.py
--rw-r--r--   0        0        0     1459 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/__main__.py
--rw-r--r--   0        0        0     9477 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/ltchiptool-192x192.png
--rw-r--r--   0        0        0    15406 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.ico
--rw-r--r--   0        0        0    26033 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.wxui
--rw-r--r--   0        0        0    32878 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.xrc
--rw-r--r--   0        0        0     6613 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/main.py
--rw-r--r--   0        0        0       48 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/__init__.py
--rw-r--r--   0        0        0     2017 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/about.py
--rw-r--r--   0        0        0     4453 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/base.py
--rw-r--r--   0        0        0    17255 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/flash.py
--rw-r--r--   0        0        0     6995 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/log.py
--rw-r--r--   0        0        0    11834 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/panels/upk.py
--rw-r--r--   0        0        0      789 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/utils.py
--rw-r--r--   0        0        0       47 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/work/__init__.py
--rw-r--r--   0        0        0      950 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/work/base.py
--rw-r--r--   0        0        0     6027 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/work/flash.py
--rw-r--r--   0        0        0     2528 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/work/ports.py
--rw-r--r--   0        0        0     4397 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/gui/work/upk.py
--rw-r--r--   0        0        0      263 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/models/__init__.py
--rw-r--r--   0        0        0     3041 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/models/board.py
--rw-r--r--   0        0        0      155 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/models/enums.py
--rw-r--r--   0        0        0     5966 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/models/family.py
--rw-r--r--   0        0        0     3199 2023-05-13 15:36:04.671286 ltchiptool-4.1.0/ltchiptool/platform.json
--rw-r--r--   0        0        0      185 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/__init__.py
--rw-r--r--   0        0        0      111 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/__init__.py
--rw-r--r--   0        0        0     6198 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/binary.py
--rw-r--r--   0        0        0     6871 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/flash.py
--rw-r--r--   0        0        0      721 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/main.py
--rw-r--r--   0        0        0       48 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/util/__init__.py
--rw-r--r--   0        0        0    18071 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz/util/rtltool.py
--rw-r--r--   0        0        0      114 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz2/__init__.py
--rw-r--r--   0        0        0     2780 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz2/flash.py
--rw-r--r--   0        0        0      595 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz2/main.py
--rw-r--r--   0        0        0       49 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz2/util/__init__.py
--rw-r--r--   0        0        0    13040 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/ambz2/util/ambz2tool.py
--rw-r--r--   0        0        0      111 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/__init__.py
--rw-r--r--   0        0        0     9025 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/binary.py
--rw-r--r--   0        0        0     8305 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/bkpackager.py
--rw-r--r--   0        0        0     6820 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/flash.py
--rw-r--r--   0        0        0      723 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/main.py
--rw-r--r--   0        0        0      317 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/__init__.py
--rw-r--r--   0        0        0     7069 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/binary.py
--rw-r--r--   0        0        0     6175 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/crypto.py
--rw-r--r--   0        0        0      515 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/models.py
--rw-r--r--   0        0        0     2940 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/rbl.py
--rw-r--r--   0        0        0     2827 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/common.py
--rw-r--r--   0        0        0     6478 2023-05-13 15:35:47.743376 ltchiptool-4.1.0/ltchiptool/soc/interface.py
--rw-r--r--   0        0        0       48 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/__init__.py
--rw-r--r--   0        0        0     2408 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/bitint.py
--rw-r--r--   0        0        0     2727 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/cli.py
--rw-r--r--   0        0        0     5642 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/crc16.py
--rw-r--r--   0        0        0     2277 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/crypto.py
--rw-r--r--   0        0        0     6631 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/detection.py
--rw-r--r--   0        0        0     1987 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/dict.py
--rw-r--r--   0        0        0      252 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/env.py
--rw-r--r--   0        0        0     2420 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/fileio.py
--rw-r--r--   0        0        0     3591 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/flash.py
--rw-r--r--   0        0        0     3296 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/fwbinary.py
--rw-r--r--   0        0        0     6105 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/intbin.py
--rw-r--r--   0        0        0     4845 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/logging.py
--rw-r--r--   0        0        0     7308 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/lvm.py
--rw-r--r--   0        0        0     1401 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/misc.py
--rw-r--r--   0        0        0     1878 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/obj.py
--rw-r--r--   0        0        0      866 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/slice.py
--rw-r--r--   0        0        0     1612 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/util/toolchain.py
--rw-r--r--   0        0        0      772 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/ltchiptool/version.py
--rw-r--r--   0        0        0     1322 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/pyproject.toml
--rw-r--r--   0        0        0      172 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/__init__.py
--rw-r--r--   0        0        0      251 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/binpatch/__init__.py
--rw-r--r--   0        0        0      471 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/binpatch/apply.py
--rw-r--r--   0        0        0     1027 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/binpatch/bindiff.py
--rw-r--r--   0        0        0     1666 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/binpatch/diff32.py
--rw-r--r--   0        0        0     4306 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/cli.py
--rw-r--r--   0        0        0      360 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/__init__.py
--rw-r--r--   0        0        0     4805 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/block.py
--rw-r--r--   0        0        0     5803 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/context.py
--rw-r--r--   0        0        0     2210 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/enums.py
--rw-r--r--   0        0        0     1256 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/flags.py
--rw-r--r--   0        0        0     3311 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/image.py
--rw-r--r--   0        0        0      778 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/partition.py
--rw-r--r--   0        0        0     4552 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/models/uf2.py
--rw-r--r--   0        0        0      124 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/upload/__init__.py
--rw-r--r--   0        0        0     4846 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/upload/esphome.py
--rw-r--r--   0        0        0     7219 2023-05-13 15:35:47.747376 ltchiptool-4.1.0/uf2tool/writer.py
--rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 ltchiptool-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/LICENSE
+-rw-r--r--   0        0        0     2384 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/README.md
+-rw-r--r--   0        0        0      376 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/ltchiptool/__init__.py
+-rw-r--r--   0        0        0     2339 2023-05-15 18:28:20.522008 ltchiptool-4.1.1/ltchiptool/__main__.py
+-rw-r--r--   0        0        0     2517 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/dumptool.py
+-rw-r--r--   0        0        0      908 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/elf2bin.py
+-rw-r--r--   0        0        0      451 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/__main__.py
+-rw-r--r--   0        0        0     1724 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/_utils.py
+-rw-r--r--   0        0        0     1610 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/file.py
+-rw-r--r--   0        0        0     3157 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/read.py
+-rw-r--r--   0        0        0     7153 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/flash/write.py
+-rw-r--r--   0        0        0      881 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/link2bin.py
+-rw-r--r--   0        0        0     2331 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/list.py
+-rw-r--r--   0        0        0      423 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/commands/soc.py
+-rw-r--r--   0        0        0     2288 2023-05-15 18:28:43.810202 ltchiptool-4.1.1/ltchiptool/families.json
+-rw-r--r--   0        0        0      127 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/__init__.py
+-rw-r--r--   0        0        0     1459 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/__main__.py
+-rw-r--r--   0        0        0     9477 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool-192x192.png
+-rw-r--r--   0        0        0    15406 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.ico
+-rw-r--r--   0        0        0    26033 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.wxui
+-rw-r--r--   0        0        0    32878 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.xrc
+-rw-r--r--   0        0        0     6613 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/main.py
+-rw-r--r--   0        0        0       48 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/__init__.py
+-rw-r--r--   0        0        0     2017 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/about.py
+-rw-r--r--   0        0        0     4453 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/base.py
+-rw-r--r--   0        0        0    17255 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/flash.py
+-rw-r--r--   0        0        0     6995 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/log.py
+-rw-r--r--   0        0        0    11834 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/panels/upk.py
+-rw-r--r--   0        0        0      789 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/utils.py
+-rw-r--r--   0        0        0       47 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/__init__.py
+-rw-r--r--   0        0        0      950 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/base.py
+-rw-r--r--   0        0        0     6027 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/flash.py
+-rw-r--r--   0        0        0     2528 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/ports.py
+-rw-r--r--   0        0        0     4824 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/gui/work/upk.py
+-rw-r--r--   0        0        0      263 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/__init__.py
+-rw-r--r--   0        0        0     3041 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/board.py
+-rw-r--r--   0        0        0      155 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/enums.py
+-rw-r--r--   0        0        0     5966 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/models/family.py
+-rw-r--r--   0        0        0     3199 2023-05-15 18:28:43.810202 ltchiptool-4.1.1/ltchiptool/platform.json
+-rw-r--r--   0        0        0      185 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/__init__.py
+-rw-r--r--   0        0        0     6198 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/binary.py
+-rw-r--r--   0        0        0     6871 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/flash.py
+-rw-r--r--   0        0        0      721 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/main.py
+-rw-r--r--   0        0        0       48 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/util/__init__.py
+-rw-r--r--   0        0        0    18071 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz/util/rtltool.py
+-rw-r--r--   0        0        0      114 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/__init__.py
+-rw-r--r--   0        0        0     2780 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/flash.py
+-rw-r--r--   0        0        0      595 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/main.py
+-rw-r--r--   0        0        0       49 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/util/__init__.py
+-rw-r--r--   0        0        0    13040 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/ambz2/util/ambz2tool.py
+-rw-r--r--   0        0        0      111 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/__init__.py
+-rw-r--r--   0        0        0     9025 2023-05-15 18:28:20.526008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/binary.py
+-rw-r--r--   0        0        0     8305 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/bkpackager.py
+-rw-r--r--   0        0        0     6820 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/flash.py
+-rw-r--r--   0        0        0      723 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/main.py
+-rw-r--r--   0        0        0      317 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/__init__.py
+-rw-r--r--   0        0        0     7069 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/binary.py
+-rw-r--r--   0        0        0     6175 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/crypto.py
+-rw-r--r--   0        0        0      515 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/models.py
+-rw-r--r--   0        0        0     2940 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/rbl.py
+-rw-r--r--   0        0        0     2827 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/common.py
+-rw-r--r--   0        0        0     6478 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/soc/interface.py
+-rw-r--r--   0        0        0       48 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/__init__.py
+-rw-r--r--   0        0        0     2408 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/bitint.py
+-rw-r--r--   0        0        0     2727 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/cli.py
+-rw-r--r--   0        0        0     5642 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/crc16.py
+-rw-r--r--   0        0        0     2277 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/crypto.py
+-rw-r--r--   0        0        0     6631 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/detection.py
+-rw-r--r--   0        0        0     1987 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/dict.py
+-rw-r--r--   0        0        0      252 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/env.py
+-rw-r--r--   0        0        0     2420 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/fileio.py
+-rw-r--r--   0        0        0     3591 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/flash.py
+-rw-r--r--   0        0        0     3296 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/fwbinary.py
+-rw-r--r--   0        0        0     6105 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/intbin.py
+-rw-r--r--   0        0        0     4845 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/logging.py
+-rw-r--r--   0        0        0     7308 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/lvm.py
+-rw-r--r--   0        0        0     1401 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/misc.py
+-rw-r--r--   0        0        0     1878 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/obj.py
+-rw-r--r--   0        0        0      866 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/slice.py
+-rw-r--r--   0        0        0     1612 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/util/toolchain.py
+-rw-r--r--   0        0        0      772 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/ltchiptool/version.py
+-rw-r--r--   0        0        0     1322 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      172 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/__init__.py
+-rw-r--r--   0        0        0      251 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/__init__.py
+-rw-r--r--   0        0        0      471 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/apply.py
+-rw-r--r--   0        0        0     1027 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/bindiff.py
+-rw-r--r--   0        0        0     1666 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/binpatch/diff32.py
+-rw-r--r--   0        0        0     4306 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/cli.py
+-rw-r--r--   0        0        0      360 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/__init__.py
+-rw-r--r--   0        0        0     4805 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/block.py
+-rw-r--r--   0        0        0     5803 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/context.py
+-rw-r--r--   0        0        0     2210 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/enums.py
+-rw-r--r--   0        0        0     1256 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/flags.py
+-rw-r--r--   0        0        0     3311 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/image.py
+-rw-r--r--   0        0        0      778 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/partition.py
+-rw-r--r--   0        0        0     4552 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/models/uf2.py
+-rw-r--r--   0        0        0      124 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/upload/__init__.py
+-rw-r--r--   0        0        0     4846 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/upload/esphome.py
+-rw-r--r--   0        0        0     7219 2023-05-15 18:28:20.530008 ltchiptool-4.1.1/uf2tool/writer.py
+-rw-r--r--   0        0        0     3794 1970-01-01 00:00:00.000000 ltchiptool-4.1.1/PKG-INFO
```

### Comparing `ltchiptool-4.1.0/LICENSE` & `ltchiptool-4.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/README.md` & `ltchiptool-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/__main__.py` & `ltchiptool-4.1.1/ltchiptool/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/dumptool.py` & `ltchiptool-4.1.1/ltchiptool/commands/dumptool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/elf2bin.py` & `ltchiptool-4.1.1/ltchiptool/commands/elf2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/flash/_utils.py` & `ltchiptool-4.1.1/ltchiptool/commands/flash/_utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/flash/file.py` & `ltchiptool-4.1.1/ltchiptool/commands/flash/file.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/flash/read.py` & `ltchiptool-4.1.1/ltchiptool/commands/flash/read.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/flash/write.py` & `ltchiptool-4.1.1/ltchiptool/commands/flash/write.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/link2bin.py` & `ltchiptool-4.1.1/ltchiptool/commands/link2bin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/commands/list.py` & `ltchiptool-4.1.1/ltchiptool/commands/list.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/families.json` & `ltchiptool-4.1.1/ltchiptool/families.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/__main__.py` & `ltchiptool-4.1.1/ltchiptool/gui/__main__.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/ltchiptool-192x192.png` & `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool-192x192.png`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.ico` & `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.ico`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.wxui` & `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.wxui`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/ltchiptool.xrc` & `ltchiptool-4.1.1/ltchiptool/gui/ltchiptool.xrc`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/main.py` & `ltchiptool-4.1.1/ltchiptool/gui/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/panels/about.py` & `ltchiptool-4.1.1/ltchiptool/gui/panels/about.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/panels/base.py` & `ltchiptool-4.1.1/ltchiptool/gui/panels/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/panels/flash.py` & `ltchiptool-4.1.1/ltchiptool/gui/panels/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/panels/log.py` & `ltchiptool-4.1.1/ltchiptool/gui/panels/log.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/panels/upk.py` & `ltchiptool-4.1.1/ltchiptool/gui/panels/upk.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/utils.py` & `ltchiptool-4.1.1/ltchiptool/gui/utils.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/work/base.py` & `ltchiptool-4.1.1/ltchiptool/gui/work/base.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/work/flash.py` & `ltchiptool-4.1.1/ltchiptool/gui/work/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/work/ports.py` & `ltchiptool-4.1.1/ltchiptool/gui/work/ports.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/gui/work/upk.py` & `ltchiptool-4.1.1/ltchiptool/gui/work/upk.py`

 * *Files 12% similar despite different names*

```diff
@@ -67,15 +67,18 @@
             url = f"http://{ip}/hub/flash_read"
             params = dict(offset=0, length=init_size)
 
             bar.on_message(f"Connecting to {ip}...")
             with requests.get(url, params) as r:
                 data = r.content
                 if len(data) != init_size:
-                    self.on_error(f"Incomplete response read: {len(data)}/{init_size}")
+                    self.on_error(
+                        f"Incomplete response read: {len(data)}/{init_size}\n\n"
+                        f"Is the chip running Kickstart firmware?"
+                    )
                     return
 
             while start < end and self.should_run():
                 bar.on_message(f"Reading from 0x{offset + start:06X}")
                 read_size = min(block_size, end - start)
                 params["offset"] = offset + start
                 params["length"] = read_size
@@ -117,20 +120,29 @@
         with open(file, "rb") as f:
             data = f.read()
         self.run_data(data)
 
     def run_data(self, data: bytes):
         # parse raw storage
         st = TuyaStorage()
-        if st.load_raw(data) is None:
+        if st.load_raw(data, allow_incomplete=True) is None:
             self.on_error("File doesn't contain known storage area")
             return
         if not st.decrypt():
             self.on_error("Couldn't decrypt the storage area")
             return
         keys = st.find_all_keys()
         debug(f"Found {len(keys)} keys! {keys}")
+        if not keys:
+            self.on_error("No keys found in storage! Is the data corrupt?")
+            try:
+                from hexdump import hexdump
+
+                hexdump(st.data)
+            except (ImportError, ModuleNotFoundError):
+                pass
+            return
         storage = st.read_all_keys()
         self.on_storage(storage)
 
     def stop(self):
         super().stop()
```

### Comparing `ltchiptool-4.1.0/ltchiptool/models/board.py` & `ltchiptool-4.1.1/ltchiptool/models/board.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/models/family.py` & `ltchiptool-4.1.1/ltchiptool/models/family.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/platform.json` & `ltchiptool-4.1.1/ltchiptool/platform.json`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz/binary.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz/flash.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz/main.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz/util/rtltool.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz/util/rtltool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz2/flash.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz2/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz2/main.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz2/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/ambz2/util/ambz2tool.py` & `ltchiptool-4.1.1/ltchiptool/soc/ambz2/util/ambz2tool.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/binary.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/bkpackager.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/bkpackager.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/flash.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/main.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/main.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/binary.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/binary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/crypto.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/models.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/models.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/bk72xx/util/rbl.py` & `ltchiptool-4.1.1/ltchiptool/soc/bk72xx/util/rbl.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/common.py` & `ltchiptool-4.1.1/ltchiptool/soc/common.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/soc/interface.py` & `ltchiptool-4.1.1/ltchiptool/soc/interface.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/bitint.py` & `ltchiptool-4.1.1/ltchiptool/util/bitint.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/cli.py` & `ltchiptool-4.1.1/ltchiptool/util/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/crc16.py` & `ltchiptool-4.1.1/ltchiptool/util/crc16.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/crypto.py` & `ltchiptool-4.1.1/ltchiptool/util/crypto.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/detection.py` & `ltchiptool-4.1.1/ltchiptool/util/detection.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/dict.py` & `ltchiptool-4.1.1/ltchiptool/util/dict.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/fileio.py` & `ltchiptool-4.1.1/ltchiptool/util/fileio.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/flash.py` & `ltchiptool-4.1.1/ltchiptool/util/flash.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/fwbinary.py` & `ltchiptool-4.1.1/ltchiptool/util/fwbinary.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/intbin.py` & `ltchiptool-4.1.1/ltchiptool/util/intbin.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/logging.py` & `ltchiptool-4.1.1/ltchiptool/util/logging.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/lvm.py` & `ltchiptool-4.1.1/ltchiptool/util/lvm.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/misc.py` & `ltchiptool-4.1.1/ltchiptool/util/misc.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/obj.py` & `ltchiptool-4.1.1/ltchiptool/util/obj.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/slice.py` & `ltchiptool-4.1.1/ltchiptool/util/slice.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/util/toolchain.py` & `ltchiptool-4.1.1/ltchiptool/util/toolchain.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/ltchiptool/version.py` & `ltchiptool-4.1.1/ltchiptool/version.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/pyproject.toml` & `ltchiptool-4.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ltchiptool"
-version = "4.1.0"
+version = "4.1.1"
 description = "Universal flashing and binary manipulation tool for IoT chips"
 authors = ["Kuba Szczodrzyński <kuba@szczodrzynski.pl>"]
 license = "MIT"
 packages = [
     { include = "ltchiptool" },
     { include = "uf2tool" },
 ]
@@ -16,21 +16,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 click = "^8.1.3"
 colorama = "^0.4.5"
 importlib-metadata = "^4.12.0"
 prettytable = "^3.3.0"
-bk7231tools = "^1.3.5"
+bk7231tools = "^1.3.6"
 xmodem = "^0.4.6"
 wxPython = {version = "^4.2.0", optional = true}
 pywin32 = {version = "^305", optional = true, markers = "sys_platform == 'win32'"}
 py-datastruct = "^0.3.0"
 semantic-version = "^2.10.0"
-upk2esphome = "^1.0.0"
+upk2esphome = "^1.0.2"
 
 [tool.poetry.dependencies.pycryptodomex]
 version = "^3.15.0"
 markers = "platform_machine not in 'armv6l,armv7l,armv8l,armv8b,aarch64'"
 
 [tool.poetry.dependencies.pyaes]
 version = "^1.6.1"
```

### Comparing `ltchiptool-4.1.0/uf2tool/binpatch/bindiff.py` & `ltchiptool-4.1.1/uf2tool/binpatch/bindiff.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/binpatch/diff32.py` & `ltchiptool-4.1.1/uf2tool/binpatch/diff32.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/cli.py` & `ltchiptool-4.1.1/uf2tool/cli.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/block.py` & `ltchiptool-4.1.1/uf2tool/models/block.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/context.py` & `ltchiptool-4.1.1/uf2tool/models/context.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/enums.py` & `ltchiptool-4.1.1/uf2tool/models/enums.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/flags.py` & `ltchiptool-4.1.1/uf2tool/models/flags.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/image.py` & `ltchiptool-4.1.1/uf2tool/models/image.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/partition.py` & `ltchiptool-4.1.1/uf2tool/models/partition.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/models/uf2.py` & `ltchiptool-4.1.1/uf2tool/models/uf2.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/upload/esphome.py` & `ltchiptool-4.1.1/uf2tool/upload/esphome.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/uf2tool/writer.py` & `ltchiptool-4.1.1/uf2tool/writer.py`

 * *Files identical despite different names*

### Comparing `ltchiptool-4.1.0/PKG-INFO` & `ltchiptool-4.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: ltchiptool
-Version: 4.1.0
+Version: 4.1.1
 Summary: Universal flashing and binary manipulation tool for IoT chips
 License: MIT
 Author: Kuba Szczodrzyński
 Author-email: kuba@szczodrzynski.pl
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: gui
-Requires-Dist: bk7231tools (>=1.3.5,<2.0.0)
+Requires-Dist: bk7231tools (>=1.3.6,<2.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: colorama (>=0.4.5,<0.5.0)
 Requires-Dist: importlib-metadata (>=4.12.0,<5.0.0)
 Requires-Dist: prettytable (>=3.3.0,<4.0.0)
 Requires-Dist: py-datastruct (>=0.3.0,<0.4.0)
 Requires-Dist: pyaes (>=1.6.1,<2.0.0) ; platform_machine in "armv6l,armv7l,armv8l,armv8b,aarch64"
 Requires-Dist: pycryptodomex (>=3.15.0,<4.0.0) ; platform_machine not in "armv6l,armv7l,armv8l,armv8b,aarch64"
 Requires-Dist: pywin32 (>=305,<306) ; (sys_platform == "win32") and (extra == "gui")
 Requires-Dist: semantic-version (>=2.10.0,<3.0.0)
-Requires-Dist: upk2esphome (>=1.0.0,<2.0.0) ; extra == "gui"
+Requires-Dist: upk2esphome (>=1.0.2,<2.0.0) ; extra == "gui"
 Requires-Dist: wxPython (>=4.2.0,<5.0.0) ; extra == "gui"
 Requires-Dist: xmodem (>=0.4.6,<0.5.0)
 Description-Content-Type: text/markdown
 
 # ltchiptool
 
 Universal, easy-to-use GUI flashing/dumping tool for BK7231, RTL8710B and RTL8720C. Also contains some CLI utilities for binary firmware manipulation.
```

