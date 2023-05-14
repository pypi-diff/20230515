# Comparing `tmp/dinero-0.1.8.tar.gz` & `tmp/dinero-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dinero-0.1.8.tar", max compression
+gzip compressed data, was "dinero-0.2.0.tar", max compression
```

## Comparing `dinero-0.1.8.tar` & `dinero-0.2.0.tar`

### file list

```diff
@@ -1,133 +1,137 @@
--rw-r--r--   0        0        0     1068 2022-10-16 19:46:47.550493 dinero-0.1.8/LICENSE
--rw-r--r--   0        0        0     7538 2023-03-06 00:00:59.608106 dinero-0.1.8/README.md
--rw-r--r--   0        0        0       74 2023-03-11 20:03:02.641207 dinero-0.1.8/dinero/__init__.py
--rw-r--r--   0        0        0    17552 2023-02-25 18:05:40.273225 dinero-0.1.8/dinero/_dinero.py
--rw-r--r--   0        0        0      384 2022-11-19 17:22:22.723648 dinero-0.1.8/dinero/_utils.py
--rw-r--r--   0        0        0     2494 2023-02-25 17:12:08.978874 dinero-0.1.8/dinero/_validators.py
--rw-r--r--   0        0        0     4008 2022-10-23 17:56:24.151144 dinero-0.1.8/dinero/currencies/__init__.py
--rw-r--r--   0        0        0      166 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_aed.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_afn.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_amd.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_aoa.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_ars.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_aud.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_awg.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_azn.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bbd.py
--rw-r--r--   0        0        0      150 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bdt.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bgn.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bhd.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bif.py
--rw-r--r--   0        0        0      130 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bmd.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_bnd.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bov.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_brl.py
--rw-r--r--   0        0        0      146 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bwp.py
--rw-r--r--   0        0        0      130 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_byn.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_bzd.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cdf.py
--rw-r--r--   0        0        0      122 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_che.py
--rw-r--r--   0        0        0      146 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_chf.py
--rw-r--r--   0        0        0      123 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_chw.py
--rw-r--r--   0        0        0      125 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_clp.py
--rw-r--r--   0        0        0      145 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cny.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cop.py
--rw-r--r--   0        0        0      134 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cou.py
--rw-r--r--   0        0        0      144 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_crc.py
--rw-r--r--   0        0        0      136 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cuc.py
--rw-r--r--   0        0        0      133 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_cve.py
--rw-r--r--   0        0        0      147 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_czk.py
--rw-r--r--   0        0        0      130 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_djf.py
--rw-r--r--   0        0        0      147 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_dkk.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_dop.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_dzd.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_egp.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_etb.py
--rw-r--r--   0        0        0      139 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_eur.py
--rw-r--r--   0        0        0      125 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_fjd.py
--rw-r--r--   0        0        0      136 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_fkp.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_gbp.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_gtq.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_hrk.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_htg.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_idr.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_ils.py
--rw-r--r--   0        0        0      147 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_inr.py
--rw-r--r--   0        0        0      125 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_iqd.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_irr.py
--rw-r--r--   0        0        0      130 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_isk.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_jmd.py
--rw-r--r--   0        0        0      145 2022-11-03 23:37:13.310111 dinero-0.1.8/dinero/currencies/_jpy.py
--rw-r--r--   0        0        0      150 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_kes.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_kgs.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_khr.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_kmf.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_krw.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_kwd.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_kzt.py
--rw-r--r--   0        0        0      121 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_lak.py
--rw-r--r--   0        0        0      150 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_lkr.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_lrd.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_lsl.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mad.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mdl.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mga.py
--rw-r--r--   0        0        0      145 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mmk.py
--rw-r--r--   0        0        0      153 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mnt.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mop.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mur.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mvr.py
--rw-r--r--   0        0        0      141 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_mxv.py
--rw-r--r--   0        0        0      152 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_mzn.py
--rw-r--r--   0        0        0      153 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_nio.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_npr.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_nzd.py
--rw-r--r--   0        0        0      124 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_omr.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_pab.py
--rw-r--r--   0        0        0      147 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_pen.py
--rw-r--r--   0        0        0      155 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_pgk.py
--rw-r--r--   0        0        0      150 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_php.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_pln.py
--rw-r--r--   0        0        0      153 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_pyg.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_ron.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_rsd.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_rub.py
--rw-r--r--   0        0        0      125 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_sar.py
--rw-r--r--   0        0        0      136 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sbd.py
--rw-r--r--   0        0        0      150 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_scr.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sdg.py
--rw-r--r--   0        0        0      127 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sek.py
--rw-r--r--   0        0        0      130 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sgd.py
--rw-r--r--   0        0        0      134 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sll.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_sos.py
--rw-r--r--   0        0        0      134 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_ssp.py
--rw-r--r--   0        0        0      144 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_stn.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_svc.py
--rw-r--r--   0        0        0      147 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_syp.py
--rw-r--r--   0        0        0      129 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_szl.py
--rw-r--r--   0        0        0      123 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_thb.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_tjs.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_tmt.py
--rw-r--r--   0        0        0      128 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_tnd.py
--rw-r--r--   0        0        0      140 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_ttd.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_twd.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_tzs.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_ugx.py
--rw-r--r--   0        0        0      133 2022-11-03 23:00:17.469995 dinero-0.1.8/dinero/currencies/_usd.py
--rw-r--r--   0        0        0      145 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_usn.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_uyi.py
--rw-r--r--   0        0        0      132 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_vnd.py
--rw-r--r--   0        0        0      126 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_vuv.py
--rw-r--r--   0        0        0      148 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_wst.py
--rw-r--r--   0        0        0      156 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_xcd.py
--rw-r--r--   0        0        0      157 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_xof.py
--rw-r--r--   0        0        0      123 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_xpf.py
--rw-r--r--   0        0        0      125 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_yer.py
--rw-r--r--   0        0        0      151 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_zar.py
--rw-r--r--   0        0        0      149 2022-11-03 23:00:12.619995 dinero-0.1.8/dinero/currencies/_zmw.py
--rw-r--r--   0        0        0      131 2022-11-03 23:00:12.629995 dinero-0.1.8/dinero/currencies/_zwl.py
--rw-r--r--   0        0        0      387 2022-11-06 15:09:48.237457 dinero-0.1.8/dinero/exceptions.py
--rw-r--r--   0        0        0      331 2022-11-19 17:24:08.559818 dinero-0.1.8/dinero/types.py
--rw-r--r--   0        0        0      850 2023-03-11 20:03:32.323073 dinero-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8676 1970-01-01 00:00:00.000000 dinero-0.1.8/setup.py
--rw-r--r--   0        0        0     8238 1970-01-01 00:00:00.000000 dinero-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-08 23:53:16.955810 dinero-0.2.0/LICENSE
+-rw-r--r--   0        0        0     5114 2023-05-14 23:48:13.953964 dinero-0.2.0/README.md
+-rw-r--r--   0        0        0       74 2023-05-10 02:57:39.253099 dinero-0.2.0/dinero/__init__.py
+-rw-r--r--   0        0        0    17552 2023-05-09 22:33:57.525601 dinero-0.2.0/dinero/_dinero.py
+-rw-r--r--   0        0        0      384 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/_utils.py
+-rw-r--r--   0        0        0     2494 2023-05-10 00:19:53.843673 dinero-0.2.0/dinero/_validators.py
+-rw-r--r--   0        0        0     4008 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/__init__.py
+-rw-r--r--   0        0        0      166 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aed.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_afn.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_amd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aoa.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_ars.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_aud.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_awg.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_azn.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bbd.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bdt.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bgn.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bhd.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bif.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bmd.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bnd.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bov.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_brl.py
+-rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bwp.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_byn.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_bzd.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cdf.py
+-rw-r--r--   0        0        0      122 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_che.py
+-rw-r--r--   0        0        0      146 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_chf.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_chw.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_clp.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cny.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cop.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cou.py
+-rw-r--r--   0        0        0      144 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_crc.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cuc.py
+-rw-r--r--   0        0        0      133 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_cve.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_czk.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_djf.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dkk.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dop.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_dzd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_egp.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_etb.py
+-rw-r--r--   0        0        0      139 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_eur.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_fjd.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_fkp.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_gbp.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_gtq.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_hrk.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_htg.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_idr.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_ils.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_inr.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_iqd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_irr.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_isk.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_jmd.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_jpy.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kes.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kgs.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_khr.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kmf.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_krw.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kwd.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_kzt.py
+-rw-r--r--   0        0        0      121 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lak.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lkr.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lrd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_lsl.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mad.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mdl.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mga.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mmk.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mnt.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mop.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mur.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.955810 dinero-0.2.0/dinero/currencies/_mvr.py
+-rw-r--r--   0        0        0      141 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_mxv.py
+-rw-r--r--   0        0        0      152 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_mzn.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_nio.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_npr.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_nzd.py
+-rw-r--r--   0        0        0      124 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_omr.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pab.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pen.py
+-rw-r--r--   0        0        0      155 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pgk.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_php.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pln.py
+-rw-r--r--   0        0        0      153 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_pyg.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ron.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_rsd.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_rub.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sar.py
+-rw-r--r--   0        0        0      136 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sbd.py
+-rw-r--r--   0        0        0      150 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_scr.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sdg.py
+-rw-r--r--   0        0        0      127 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sek.py
+-rw-r--r--   0        0        0      130 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sgd.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sll.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_sos.py
+-rw-r--r--   0        0        0      134 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ssp.py
+-rw-r--r--   0        0        0      144 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_stn.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_svc.py
+-rw-r--r--   0        0        0      147 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_syp.py
+-rw-r--r--   0        0        0      129 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_szl.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_thb.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tjs.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tmt.py
+-rw-r--r--   0        0        0      128 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tnd.py
+-rw-r--r--   0        0        0      140 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ttd.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_twd.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_tzs.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_ugx.py
+-rw-r--r--   0        0        0      133 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_usd.py
+-rw-r--r--   0        0        0      145 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_usn.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_uyi.py
+-rw-r--r--   0        0        0      132 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_vnd.py
+-rw-r--r--   0        0        0      126 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_vuv.py
+-rw-r--r--   0        0        0      148 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_wst.py
+-rw-r--r--   0        0        0      156 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xcd.py
+-rw-r--r--   0        0        0      157 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xof.py
+-rw-r--r--   0        0        0      123 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_xpf.py
+-rw-r--r--   0        0        0      125 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_yer.py
+-rw-r--r--   0        0        0      151 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zar.py
+-rw-r--r--   0        0        0      149 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zmw.py
+-rw-r--r--   0        0        0      131 2023-05-08 23:53:16.965810 dinero-0.2.0/dinero/currencies/_zwl.py
+-rw-r--r--   0        0        0      387 2023-05-09 23:46:15.080607 dinero-0.2.0/dinero/exceptions.py
+-rw-r--r--   0        0        0      362 2023-05-10 01:59:35.240655 dinero-0.2.0/dinero/tools/__init__.py
+-rw-r--r--   0        0        0     2108 2023-05-10 02:53:58.158738 dinero-0.2.0/dinero/tools/calculate_compound_interest.py
+-rw-r--r--   0        0        0     1339 2023-05-14 22:42:56.383362 dinero-0.2.0/dinero/tools/calculate_percentage.py
+-rw-r--r--   0        0        0     1858 2023-05-14 22:46:39.176259 dinero-0.2.0/dinero/tools/calculate_simple_interest.py
+-rw-r--r--   0        0        0     1356 2023-05-14 22:29:33.710063 dinero-0.2.0/dinero/tools/calculate_vat.py
+-rw-r--r--   0        0        0      331 2023-05-09 22:06:45.830428 dinero-0.2.0/dinero/types.py
+-rw-r--r--   0        0        0      850 2023-05-10 02:57:31.043073 dinero-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5814 1970-01-01 00:00:00.000000 dinero-0.2.0/PKG-INFO
```

### Comparing `dinero-0.1.8/LICENSE` & `dinero-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dinero-0.1.8/dinero/_dinero.py` & `dinero-0.2.0/dinero/_dinero.py`

 * *Files identical despite different names*

### Comparing `dinero-0.1.8/dinero/_validators.py` & `dinero-0.2.0/dinero/_validators.py`

 * *Files identical despite different names*

### Comparing `dinero-0.1.8/dinero/currencies/__init__.py` & `dinero-0.2.0/dinero/currencies/__init__.py`

 * *Files identical despite different names*

### Comparing `dinero-0.1.8/pyproject.toml` & `dinero-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dinero"
-version = "0.1.8"
+version = "0.2.0"
 description = "Dinero is a library for working with monetary values in Python."
 license = "MIT"
 authors = ["Carlos Montecinos Geisse <carlos@pythoncheatsheet.org>"]
 readme = "README.md"
 repository = "https://github.com/wilfredinni/dinero"
 keywords = ["python3", "money", "decimals", "calculations", "currency"]
 
@@ -15,20 +15,20 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^23.0.0"
 flake8 = "^6.0.0"
 mypy = "^1.1"
 ipykernel = "^6.16.0"
-pandas = "^1.5.0"
+pandas = "^2.0.0"
 coverage = "^7.0.0"
 pytest-cov = "^4.0.0"
 
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.2"
-mkdocstrings = {extras = ["python"], version = "^0.20.0"}
+mkdocstrings = {extras = ["python"], version = "^0.21.0"}
 mkdocs-material = "^9.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

