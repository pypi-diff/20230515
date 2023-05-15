# Comparing `tmp/xpydf-0.1.4.tar.gz` & `tmp/xpydf-0.1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xpydf-0.1.4.tar", last modified: Mon May  8 16:10:19 2023, max compression
+gzip compressed data, was "xpydf-0.1.4.1.tar", last modified: Mon May 15 08:43:09 2023, max compression
```

## Comparing `xpydf-0.1.4.tar` & `xpydf-0.1.4.1.tar`

### file list

```diff
@@ -1,257 +1,257 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.254602 xpydf-0.1.4/
--rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.4/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-04-12 11:54:25.000000 xpydf-0.1.4/MANIFEST.in
--rw-r--r--   0 matthijs   (501) staff       (20)      844 2023-05-08 16:10:19.254399 xpydf-0.1.4/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.4/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)      785 2023-05-08 16:08:33.000000 xpydf-0.1.4/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-05-08 16:10:19.254655 xpydf-0.1.4/setup.cfg
--rw-r--r--   0 matthijs   (501) staff       (20)     1998 2023-05-05 08:47:39.000000 xpydf-0.1.4/setup.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.124865 xpydf-0.1.4/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.130558 xpydf-0.1.4/src/xpdf-4.04/
--rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-04-13 10:48:09.000000 xpydf-0.1.4/src/xpdf-4.04/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/ANNOUNCE
--rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/CHANGES
--rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/CMakeLists.txt
--rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/COPYING
--rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/COPYING3
--rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/INSTALL
--rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/README
--rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpdf-4.04/aconf.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/aconf.h.in
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/aconf2.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/cmake-config.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.145414 xpydf-0.1.4/src/xpdf-4.04/fofi/
--rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiBase.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiBase.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiEncodings.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiEncodings.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiIdentifier.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiIdentifier.h
--rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiTrueType.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiTrueType.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1.h
--rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1C.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1C.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.155118 xpydf-0.1.4/src/xpdf-4.04/goo/
--rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/FixedPoint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/FixedPoint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GHash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GHash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GList.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GList.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GMutex.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/GString.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/Trace.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/Trace.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gfile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gfile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gmem.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gmem.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gmempp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gmempp.h
--rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/gtypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/goo/parseargs.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.179651 xpydf-0.1.4/src/xpdf-4.04/splash/
--rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/Splash.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/Splash.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashBitmap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashClip.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashClip.h
--rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontEngine.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontEngine.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFile.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFile.h
--rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFileID.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFileID.h
--rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashGlyphBitmap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashMath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashPattern.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashPattern.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashScreen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashScreen.h
--rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPath.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPath.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPathScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPathScanner.h
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.244980 xpydf-0.1.4/src/xpdf-4.04/xpdf/
--rw-r--r--   0 matthijs   (501) staff       (20)   104168 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/AcroForm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5229 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/AcroForm.h
--rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Annot.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Annot.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Array.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Array.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    28608 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Catalog.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Catalog.h
--rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
--rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CharTypes.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/CompactFontTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Decrypt.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Decrypt.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2993 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Dict.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Dict.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/DisplayState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/DisplayState.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Error.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Error.h
--rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/ErrorCodes.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/FontEncodingTables.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/FontEncodingTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Function.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Function.h
--rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-04-13 10:47:44.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Gfx.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Gfx.h
--rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-04-13 10:47:45.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxState.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    43452 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxState.h
--rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-02-21 10:47:30.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GlobalParams.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/GlobalParams.h
--rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/HTMLGen.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/HTMLGen.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/ImageOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/ImageOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
--rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JBIG2Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JBIG2Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JPXStream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/JPXStream.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Lexer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Lexer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Link.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Link.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToCharCode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToCharCode.h
--rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-03-01 15:38:49.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Object.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9081 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Object.h
--rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/OptionalContent.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/OptionalContent.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Outline.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Outline.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/OutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/OutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDF417Barcode.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDF417Barcode.h
--rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    16078 2023-03-01 14:01:13.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDoc.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDoc.h
--rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDocEncoding.h
--rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PSOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PSOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PSTokenizer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PSTokenizer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Page.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Page.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Parser.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Parser.h
--rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/PreScanOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/SecurityHandler.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/SecurityHandler.h
--rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/ShadingImage.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/ShadingImage.h
--rw-r--r--   0 matthijs   (501) staff       (20)   127634 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/SplashOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/SplashOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream-CCITT.h
--rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream.h
--rw-r--r--   0 matthijs   (501) staff       (20)   183404 2023-04-13 10:47:47.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TextOutputDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TextOutputDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TextString.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TextString.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCache.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCache.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCompositor.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCompositor.h
--rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/TileMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UTF8.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UTF8.h
--rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMap.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMap.h
--rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMapTables.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeRemapping.h
--rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
--rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/WebFont.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/WebFont.h
--rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/XFAScanner.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/XFAScanner.h
--rw-r--r--   0 matthijs   (501) staff       (20)    33740 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/XRef.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/XRef.h
--rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Zoox.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/Zoox.h
--rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/config.h
--rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfdetach.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdffonts.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfimages.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfinfo.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftohtml.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    10873 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftopng.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftoppm.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftops.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftotext.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.248638 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/
--rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
--rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfApp.h
--rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
--rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
--rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
--rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/xpdf.cc
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.252483 xpydf-0.1.4/src/xpydf/
--rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.4/src/xpydf/.DS_Store
--rw-r--r--   0 matthijs   (501) staff       (20)     3555 2023-05-05 08:47:39.000000 xpydf-0.1.4/src/xpydf/ImageDataDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.4/src/xpydf/ImageDataDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/ImageInfoDev.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/ImageInfoDev.h
--rw-r--r--   0 matthijs   (501) staff       (20)     4729 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/PdfLoader.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/PdfLoader.h
--rw-r--r--   0 matthijs   (501) staff       (20)     7478 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/PdfLoaderWrapper.cc
--rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/PyCppConversion.cc
--rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/PyCppConversion.h
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4/src/xpydf/__init__.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)      760 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/cXpdfPython.pyi
--rw-r--r--   0 matthijs   (501) staff       (20)     4684 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/pdf_loader.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1159 2023-05-08 13:59:17.000000 xpydf-0.1.4/src/xpydf/pdf_loader.pyi
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.253700 xpydf-0.1.4/src/xpydf.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)      844 2023-05-08 16:10:19.000000 xpydf-0.1.4/src/xpydf.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     7675 2023-05-08 16:10:19.000000 xpydf-0.1.4/src/xpydf.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-05-08 16:10:19.000000 xpydf-0.1.4/src/xpydf.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-05-08 16:10:19.000000 xpydf-0.1.4/src/xpydf.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       18 2023-05-08 16:10:19.000000 xpydf-0.1.4/src/xpydf.egg-info/top_level.txt
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-08 16:10:19.253889 xpydf-0.1.4/tests/
--rw-r--r--   0 matthijs   (501) staff       (20)     4094 2023-05-08 13:59:17.000000 xpydf-0.1.4/tests/test_pdf_loader.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.366479 xpydf-0.1.4.1/
+-rw-r--r--   0 matthijs   (501) staff       (20)    35149 2023-02-17 12:43:21.000000 xpydf-0.1.4.1/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)      118 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/MANIFEST.in
+-rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-15 08:43:09.366293 xpydf-0.1.4.1/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)      240 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)      787 2023-05-15 08:42:52.000000 xpydf-0.1.4.1/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2023-05-15 08:43:09.366522 xpydf-0.1.4.1/setup.cfg
+-rw-r--r--   0 matthijs   (501) staff       (20)     1998 2023-05-05 08:47:39.000000 xpydf-0.1.4.1/setup.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.167919 xpydf-0.1.4.1/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.192639 xpydf-0.1.4.1/src/xpdf-4.04/
+-rw-r--r--   0 matthijs   (501) staff       (20)     8196 2023-05-15 08:40:49.000000 xpydf-0.1.4.1/src/xpdf-4.04/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     1330 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/ANNOUNCE
+-rw-r--r--   0 matthijs   (501) staff       (20)   139475 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/CHANGES
+-rw-r--r--   0 matthijs   (501) staff       (20)     1053 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/CMakeLists.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)    17982 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/COPYING
+-rw-r--r--   0 matthijs   (501) staff       (20)    35147 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/COPYING3
+-rw-r--r--   0 matthijs   (501) staff       (20)     5614 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/INSTALL
+-rw-r--r--   0 matthijs   (501) staff       (20)    13778 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/README
+-rw-r--r--   0 matthijs   (501) staff       (20)     2002 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpdf-4.04/aconf.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1985 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/aconf.h.in
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/aconf2.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10676 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/cmake-config.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.204597 xpydf-0.1.4.1/src/xpdf-4.04/fofi/
+-rw-r--r--   0 matthijs   (501) staff       (20)     3275 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiBase.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1344 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiBase.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14853 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiEncodings.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiEncodings.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21889 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiIdentifier.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1659 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiIdentifier.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    77637 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiTrueType.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8227 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiTrueType.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8796 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1434 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    97383 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1C.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8299 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1C.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.215723 xpydf-0.1.4.1/src/xpdf-4.04/goo/
+-rw-r--r--   0 matthijs   (501) staff       (20)     2748 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/FixedPoint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7361 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/FixedPoint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6201 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GHash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2209 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GHash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2276 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GList.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2724 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GList.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2629 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GMutex.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17722 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4269 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/GString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2406 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/Trace.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1171 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/Trace.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17381 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gfile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4565 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gfile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8259 2023-03-01 15:38:49.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gmem.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2029 2023-03-01 15:38:49.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gmem.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1005 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gmempp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1714 2023-03-01 15:38:49.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gmempp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      562 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/gtypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1583 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/goo/parseargs.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.250496 xpydf-0.1.4.1/src/xpdf-4.04/splash/
+-rw-r--r--   0 matthijs   (501) staff       (20)   230071 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/Splash.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    20193 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/Splash.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6603 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashBitmap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2881 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11473 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashClip.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4007 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashClip.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      930 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13929 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1345 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8902 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2248 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4055 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2241 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4995 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3666 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9673 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontEngine.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3358 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontEngine.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1589 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFile.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2168 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFile.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      603 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFileID.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      687 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFileID.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      758 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashGlyphBitmap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9510 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashMath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5135 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3876 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1042 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPattern.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1447 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPattern.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9844 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashScreen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2167 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashScreen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     9521 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3669 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4155 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17088 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPath.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3761 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPath.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12936 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPathScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2482 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPathScanner.h
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.356508 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/
+-rw-r--r--   0 matthijs   (501) staff       (20)   104168 2023-05-15 08:40:39.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/AcroForm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5229 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/AcroForm.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    38840 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Annot.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4895 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Annot.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1385 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Array.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1400 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Array.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1387 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1080 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   229548 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFontTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      556 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10417 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3178 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    28608 2023-05-15 08:40:37.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Catalog.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4742 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Catalog.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    19175 2023-04-13 10:47:41.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3702 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      526 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharTypes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8379 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CompactFontTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    45644 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Decrypt.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3530 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Decrypt.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2993 2023-05-15 08:40:36.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Dict.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2088 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Dict.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5247 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/DisplayState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5225 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/DisplayState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2123 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Error.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1353 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Error.h
+-rw-r--r--   0 matthijs   (501) staff       (20)      984 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ErrorCodes.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21312 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/FontEncodingTables.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      564 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/FontEncodingTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    36553 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Function.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6722 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Function.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   144837 2023-04-13 10:47:44.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Gfx.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11911 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Gfx.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    65646 2023-04-13 10:47:45.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12828 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   120789 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxState.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    43452 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxState.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   103543 2023-02-21 10:47:30.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GlobalParams.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    23054 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GlobalParams.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    34442 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/HTMLGen.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3131 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/HTMLGen.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11293 2023-05-02 12:54:18.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ImageOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3942 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ImageOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8327 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2802 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   109724 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JBIG2Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4824 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JBIG2Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   107255 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JPXStream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11092 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JPXStream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11674 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Lexer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2035 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Lexer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    21632 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Link.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11370 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Link.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2191 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToCharCode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      726 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToCharCode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   117065 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToUnicodeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4471 2023-05-15 08:40:34.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Object.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9081 2023-05-15 08:40:32.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Object.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    12818 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OptionalContent.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3617 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OptionalContent.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4001 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Outline.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1774 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Outline.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4131 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8935 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    87382 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDF417Barcode.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      838 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDF417Barcode.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    51111 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11579 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    16084 2023-05-15 08:40:48.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDoc.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6774 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDoc.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     2530 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDocEncoding.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      339 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDocEncoding.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   230372 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    19106 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3295 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSTokenizer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      771 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSTokenizer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13874 2023-03-01 15:38:49.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Page.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6412 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Page.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8100 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Parser.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1674 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Parser.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     8588 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PreScanOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4810 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PreScanOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10354 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SecurityHandler.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3962 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SecurityHandler.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    37941 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ShadingImage.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     3215 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ShadingImage.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   127634 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SplashOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10811 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SplashOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    17471 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream-CCITT.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   131758 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    31826 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   183404 2023-04-13 10:47:47.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextOutputDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    27134 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextOutputDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4302 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextString.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1587 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextString.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13862 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCache.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2041 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCache.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10913 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCompositor.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1895 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCompositor.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    44674 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8164 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4636 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UTF8.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1408 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UTF8.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     6033 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMap.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2971 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMap.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    11532 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMapTables.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5024 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeRemapping.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1138 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeRemapping.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    73118 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      719 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    10592 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/WebFont.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2139 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/WebFont.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    18912 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XFAScanner.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4518 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XFAScanner.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    33740 2023-05-15 08:40:18.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XRef.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     5955 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XRef.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    23997 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Zoox.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6378 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Zoox.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     3128 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/config.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     5663 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfdetach.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    12108 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdffonts.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     4538 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfimages.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    15031 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfinfo.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     8525 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftohtml.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    10873 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftopng.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     7820 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftoppm.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    11515 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftops.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     9928 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftotext.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.361385 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/
+-rw-r--r--   0 matthijs   (501) staff       (20)    30301 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     6596 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    14925 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfApp.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2452 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfApp.h
+-rw-r--r--   0 matthijs   (501) staff       (20)   148791 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    18968 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    54075 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)    39531 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.h
+-rw-r--r--   0 matthijs   (501) staff       (20)    13035 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      520 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1327 2022-04-18 21:11:23.000000 xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/xpdf.cc
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.364910 xpydf-0.1.4.1/src/xpydf/
+-rw-r--r--   0 matthijs   (501) staff       (20)     6148 2023-05-01 14:11:15.000000 xpydf-0.1.4.1/src/xpydf/.DS_Store
+-rw-r--r--   0 matthijs   (501) staff       (20)     3555 2023-05-15 08:40:16.000000 xpydf-0.1.4.1/src/xpydf/ImageDataDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1095 2023-05-05 08:47:39.000000 xpydf-0.1.4.1/src/xpydf/ImageDataDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     1121 2023-05-15 08:40:14.000000 xpydf-0.1.4.1/src/xpydf/ImageInfoDev.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      941 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpydf/ImageInfoDev.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     4729 2023-05-15 08:40:09.000000 xpydf-0.1.4.1/src/xpydf/PdfLoader.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     1118 2023-05-08 13:59:17.000000 xpydf-0.1.4.1/src/xpydf/PdfLoader.h
+-rw-r--r--   0 matthijs   (501) staff       (20)     7466 2023-05-09 07:36:01.000000 xpydf-0.1.4.1/src/xpydf/PdfLoaderWrapper.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)     2198 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpydf/PyCppConversion.cc
+-rw-r--r--   0 matthijs   (501) staff       (20)      441 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpydf/PyCppConversion.h
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpydf/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)        0 2023-04-12 11:54:25.000000 xpydf-0.1.4.1/src/xpydf/__init__.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)      760 2023-05-08 13:59:17.000000 xpydf-0.1.4.1/src/xpydf/cXpdfPython.pyi
+-rw-r--r--   0 matthijs   (501) staff       (20)     4684 2023-05-08 13:59:17.000000 xpydf-0.1.4.1/src/xpydf/pdf_loader.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1159 2023-05-08 13:59:17.000000 xpydf-0.1.4.1/src/xpydf/pdf_loader.pyi
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.365811 xpydf-0.1.4.1/src/xpydf.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)      846 2023-05-15 08:43:09.000000 xpydf-0.1.4.1/src/xpydf.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     7675 2023-05-15 08:43:09.000000 xpydf-0.1.4.1/src/xpydf.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2023-05-15 08:43:09.000000 xpydf-0.1.4.1/src/xpydf.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       14 2023-05-15 08:43:09.000000 xpydf-0.1.4.1/src/xpydf.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       18 2023-05-15 08:43:09.000000 xpydf-0.1.4.1/src/xpydf.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2023-05-15 08:43:09.365984 xpydf-0.1.4.1/tests/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4094 2023-05-08 13:59:17.000000 xpydf-0.1.4.1/tests/test_pdf_loader.py
```

### Comparing `xpydf-0.1.4/LICENSE` & `xpydf-0.1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/PKG-INFO` & `xpydf-0.1.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.4/pyproject.toml` & `xpydf-0.1.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "xpydf"
-version = "0.1.4"
+version = "0.1.4.1"
 authors = [
     { name  = "Matthijs Wesseling", email = "matthijs.wesseling@bigdatarepublic.nl" },
 ]
 
 description = "Python wrapper around the pdftotext and pdfimages functionalities of xpdf."
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `xpydf-0.1.4/setup.py` & `xpydf-0.1.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/.DS_Store` & `xpydf-0.1.4.1/src/xpdf-4.04/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -325,19 +325,19 @@
 00001440: 6473 5b53 686f 7753 6964 6562 6172 0909  ds[ShowSidebar..
 00001450: 0809 5f10 187b 7b33 3335 2c20 3131 397d  .._..{{335, 119}
 00001460: 2c20 7b39 3537 2c20 3532 377d 7d09 0815  , {957, 527}}...
 00001470: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
 00001480: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
 00001490: 0000 0000 0000 0000 0000 8b00 0000 0400  ................
 000014a0: 7800 7000 6400 666c 6731 5363 6f6d 7000  x.p.d.flg1Scomp.
-000014b0: 0000 0000 2f42 7300 0000 0400 7800 7000  ..../Bs.....x.p.
-000014c0: 6400 666d 6f44 4462 6c6f 6200 0000 089d  d.fmoDDblob.....
-000014d0: 13d1 a90a f4c4 4100 0000 0400 7800 7000  ......A.....x.p.
-000014e0: 6400 666d 6f64 4462 6c6f 6200 0000 0800  d.fmodDblob.....
-000014f0: 0080 bd05 07c4 4100 0000 0400 7800 7000  ......A.....x.p.
+000014b0: 0000 0000 2f42 7900 0000 0400 7800 7000  ..../By.....x.p.
+000014c0: 6400 666d 6f44 4462 6c6f 6200 0000 087f  d.fmoDDblob.....
+000014d0: afbe c313 09c5 4100 0000 0400 7800 7000  ......A.....x.p.
+000014e0: 6400 666d 6f64 4462 6c6f 6200 0000 087f  d.fmodDblob.....
+000014f0: afbe c313 09c5 4100 0000 0400 7800 7000  ......A.....x.p.
 00001500: 6400 6670 6831 5363 6f6d 7000 0000 0000  d.fph1Scomp.....
 00001510: 3380 0000 0000 0400 7800 7000 6400 6676  3.......x.p.d.fv
 00001520: 5372 6e6c 6f6e 6700 0000 0100 0000 0700  Srnlong.........
 00001530: 7800 7000 6400 6600 2d00 7100 746c 6731  x.p.d.f.-.q.tlg1
 00001540: 5363 6f6d 7000 0000 0000 057b b400 0000  Scomp......{....
 00001550: 0700 7800 7000 6400 6600 2d00 7100 746d  ..x.p.d.f.-.q.tm
 00001560: 6f44 4462 6c6f 6200 0000 0800 0080 bd05  oDDblob.........
```

### Comparing `xpydf-0.1.4/src/xpdf-4.04/ANNOUNCE` & `xpydf-0.1.4.1/src/xpdf-4.04/ANNOUNCE`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/CHANGES` & `xpydf-0.1.4.1/src/xpdf-4.04/CHANGES`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/CMakeLists.txt` & `xpydf-0.1.4.1/src/xpdf-4.04/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/COPYING` & `xpydf-0.1.4.1/src/xpdf-4.04/COPYING`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/COPYING3` & `xpydf-0.1.4.1/src/xpdf-4.04/COPYING3`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/INSTALL` & `xpydf-0.1.4.1/src/xpdf-4.04/INSTALL`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/README` & `xpydf-0.1.4.1/src/xpdf-4.04/README`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/aconf.h` & `xpydf-0.1.4.1/src/xpdf-4.04/aconf.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/aconf.h.in` & `xpydf-0.1.4.1/src/xpdf-4.04/aconf.h.in`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/aconf2.h` & `xpydf-0.1.4.1/src/xpdf-4.04/aconf2.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/cmake-config.txt` & `xpydf-0.1.4.1/src/xpdf-4.04/cmake-config.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiBase.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiBase.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiBase.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiBase.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiEncodings.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiEncodings.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiEncodings.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiEncodings.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiIdentifier.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiIdentifier.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiIdentifier.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiIdentifier.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiTrueType.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiTrueType.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiTrueType.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiTrueType.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1C.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1C.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/fofi/FoFiType1C.h` & `xpydf-0.1.4.1/src/xpdf-4.04/fofi/FoFiType1C.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/FixedPoint.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/FixedPoint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/FixedPoint.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/FixedPoint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GHash.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GHash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GHash.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GHash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GList.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GList.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GList.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GList.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GMutex.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GMutex.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GString.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/GString.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/GString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/Trace.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/Trace.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/Trace.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/Trace.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gfile.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gfile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gfile.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gfile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gmem.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gmem.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gmem.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gmem.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gmempp.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gmempp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gmempp.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gmempp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/gtypes.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/gtypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/goo/parseargs.h` & `xpydf-0.1.4.1/src/xpdf-4.04/goo/parseargs.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/Splash.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/Splash.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/Splash.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/Splash.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashBitmap.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashBitmap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashBitmap.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashClip.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashClip.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashClip.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashClip.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashErrorCodes.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFont.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFont.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontEngine.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontEngine.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontFile.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFTFontFile.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFTFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFont.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFont.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontEngine.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontEngine.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontEngine.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontEngine.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFile.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFile.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFile.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFile.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFileID.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFileID.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashFontFileID.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashFontFileID.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashGlyphBitmap.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashGlyphBitmap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashMath.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashMath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashPath.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashPath.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashPattern.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPattern.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashPattern.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashPattern.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashScreen.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashScreen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashScreen.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashScreen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashState.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashState.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashTypes.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPath.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPath.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPath.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPath.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPathScanner.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPathScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/splash/SplashXPathScanner.h` & `xpydf-0.1.4.1/src/xpdf-4.04/splash/SplashXPathScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/AcroForm.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/AcroForm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/AcroForm.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/AcroForm.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Annot.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Annot.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Annot.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Annot.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Array.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Array.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Array.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Array.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFont.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFont.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFontTables.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFontTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/BuiltinFontTables.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/BuiltinFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CMap.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CMap.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Catalog.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Catalog.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Catalog.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Catalog.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CharCodeToUnicode.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharCodeToUnicode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CharTypes.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CharTypes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/CompactFontTables.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/CompactFontTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Decrypt.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Decrypt.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Decrypt.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Decrypt.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Dict.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Dict.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Dict.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Dict.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/DisplayState.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/DisplayState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/DisplayState.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/DisplayState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Error.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Error.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Error.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Error.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/ErrorCodes.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ErrorCodes.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/FontEncodingTables.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/FontEncodingTables.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/FontEncodingTables.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/FontEncodingTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Function.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Function.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Function.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Function.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Gfx.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Gfx.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Gfx.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Gfx.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxFont.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxFont.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxState.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxState.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GfxState.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GfxState.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GlobalParams.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GlobalParams.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/GlobalParams.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/GlobalParams.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/HTMLGen.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/HTMLGen.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/HTMLGen.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/HTMLGen.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/ImageOutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ImageOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/ImageOutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ImageOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JArithmeticDecoder.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JArithmeticDecoder.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JBIG2Stream.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JBIG2Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JBIG2Stream.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JBIG2Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JPXStream.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JPXStream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/JPXStream.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/JPXStream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Lexer.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Lexer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Lexer.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Lexer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Link.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Link.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Link.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Link.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToCharCode.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToCharCode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToCharCode.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToCharCode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/NameToUnicodeTable.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/NameToUnicodeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Object.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Object.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Object.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Object.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/OptionalContent.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OptionalContent.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/OptionalContent.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OptionalContent.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Outline.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Outline.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Outline.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Outline.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/OutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/OutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/OutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDF417Barcode.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDF417Barcode.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDF417Barcode.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDF417Barcode.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFCore.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFCore.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDoc.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDoc.cc`

 * *Files 0% similar despite different names*

```diff
@@ -269,17 +269,17 @@
 
   // read the xref and catalog
   if (!PDFDoc::setup2(ownerPassword, userPassword, gFalse)) {
     if (errCode == errDamaged || errCode == errBadCatalog) {
       // try repairing the xref table
       error(errSyntaxWarning, -1,
 	    "PDF file is damaged - attempting to reconstruct xref table...");
-      if (!PDFDoc::setup2(ownerPassword, userPassword, gTrue)) {
+      // if (!PDFDoc::setup2(ownerPassword, userPassword, gTrue)) {
 	return gFalse;
-      }
+      // }
     } else {
       return gFalse;
     }
   }
 
 #ifndef DISABLE_OUTLINE
   // read outline
```

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDoc.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDoc.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PDFDocEncoding.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PDFDocEncoding.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PSOutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PSOutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PSTokenizer.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSTokenizer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PSTokenizer.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PSTokenizer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Page.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Page.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Page.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Page.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Parser.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Parser.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Parser.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Parser.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PreScanOutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PreScanOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/PreScanOutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/PreScanOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/SecurityHandler.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SecurityHandler.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/SecurityHandler.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SecurityHandler.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/ShadingImage.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ShadingImage.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/ShadingImage.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/ShadingImage.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/SplashOutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SplashOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/SplashOutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/SplashOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream-CCITT.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream-CCITT.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Stream.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Stream.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TextOutputDev.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextOutputDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TextOutputDev.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextOutputDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TextString.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextString.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TextString.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TextString.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCache.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCache.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCache.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCache.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCompositor.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCompositor.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileCompositor.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileCompositor.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileMap.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/TileMap.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/TileMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UTF8.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UTF8.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UTF8.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UTF8.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMap.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMap.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMap.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMap.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeMapTables.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeMapTables.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeRemapping.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeRemapping.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeRemapping.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeRemapping.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/UnicodeTypeTable.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/UnicodeTypeTable.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/WebFont.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/WebFont.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/WebFont.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/WebFont.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/XFAScanner.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XFAScanner.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/XFAScanner.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XFAScanner.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/XRef.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XRef.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/XRef.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/XRef.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Zoox.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Zoox.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/Zoox.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/Zoox.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/config.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/config.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfdetach.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfdetach.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdffonts.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdffonts.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfimages.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfimages.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdfinfo.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdfinfo.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftohtml.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftohtml.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftopng.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftopng.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftoppm.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftoppm.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftops.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftops.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf/pdftotext.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf/pdftotext.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/QtPDFCore.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/QtPDFCore.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfApp.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfApp.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfApp.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfApp.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfViewer.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfViewer.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidget.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidget.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/XpdfWidgetPrint.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpdf-4.04/xpdf-qt/xpdf.cc` & `xpydf-0.1.4.1/src/xpdf-4.04/xpdf-qt/xpdf.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/.DS_Store` & `xpydf-0.1.4.1/src/xpydf/.DS_Store`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/ImageDataDev.cc` & `xpydf-0.1.4.1/src/xpydf/ImageDataDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/ImageDataDev.h` & `xpydf-0.1.4.1/src/xpydf/ImageDataDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/ImageInfoDev.cc` & `xpydf-0.1.4.1/src/xpydf/ImageInfoDev.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/ImageInfoDev.h` & `xpydf-0.1.4.1/src/xpydf/ImageInfoDev.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/PdfLoader.cc` & `xpydf-0.1.4.1/src/xpydf/PdfLoader.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/PdfLoader.h` & `xpydf-0.1.4.1/src/xpydf/PdfLoader.h`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/PdfLoaderWrapper.cc` & `xpydf-0.1.4.1/src/xpydf/PdfLoaderWrapper.cc`

 * *Files 0% similar despite different names*

```diff
@@ -51,19 +51,19 @@
             break;
           case errOpenFile: // couldn't open the PDF file
             snprintf(message, 1000, "Error opening file %s", fileName);
             PyErr_SetString(PyExc_OSError, message);
             break;
           case errBadCatalog: // couldn't read the page catalog
             snprintf(message, 1000, "Error parsing PDF catalog in file %s", fileName);
-            PyErr_SetString(PyExc_ImportError, message);
+            PyErr_SetString(PyExc_IOError, message);
             break;
           case errDamaged: // PDF file was damaged and couldn't be repaired
             snprintf(message, 1000, "Error parsing PDF file %s. File might be damaged", fileName);            
-            PyErr_SetString(PyExc_ImportError, message);
+            PyErr_SetString(PyExc_IOError, message);
             break;
           case errEncrypted: // file was encrypted and password was incorrect or not supplied
             snprintf(message, 1000, "Error decrypting PDF file %s", fileName);
             PyErr_SetString(PyExc_PermissionError, message);
             break;
           case errHighlightFile: // nonexistent or invalid highlight file
             snprintf(message, 1000, "Error highlight PDF file %s", fileName);
@@ -79,15 +79,15 @@
             break;
           case errPermission: // PDF file doesn't allow that operation
             snprintf(message, 1000, "Error permissions PDF file %s", fileName);
             PyErr_SetString(PyExc_PermissionError, message);
             break;
           case errBadPageNum: // invalid page number
             snprintf(message, 1000, "Error bad PDF page number in file %s", fileName);
-            PyErr_SetString(PyExc_ImportError, message);
+            PyErr_SetString(PyExc_IOError, message);
             break;
           case errFileIO: // file I/O error
             snprintf(message, 1000, "Error while read/write file %s", fileName);
             PyErr_SetString(PyExc_OSError, message);
             break;
         }
         delete loader;
```

### Comparing `xpydf-0.1.4/src/xpydf/PyCppConversion.cc` & `xpydf-0.1.4.1/src/xpydf/PyCppConversion.cc`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/cXpdfPython.pyi` & `xpydf-0.1.4.1/src/xpydf/cXpdfPython.pyi`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/pdf_loader.py` & `xpydf-0.1.4.1/src/xpydf/pdf_loader.py`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf/pdf_loader.pyi` & `xpydf-0.1.4.1/src/xpydf/pdf_loader.pyi`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/src/xpydf.egg-info/PKG-INFO` & `xpydf-0.1.4.1/src/xpydf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xpydf
-Version: 0.1.4
+Version: 0.1.4.1
 Summary: Python wrapper around the pdftotext and pdfimages functionalities of xpdf.
 Author-email: Matthijs Wesseling <matthijs.wesseling@bigdatarepublic.nl>
 Project-URL: Homepage, https://github.com/Bladieblah/xpdf-python
 Project-URL: Bug Tracker, https://github.com/Bladieblah/xpdf-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `xpydf-0.1.4/src/xpydf.egg-info/SOURCES.txt` & `xpydf-0.1.4.1/src/xpydf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xpydf-0.1.4/tests/test_pdf_loader.py` & `xpydf-0.1.4.1/tests/test_pdf_loader.py`

 * *Files identical despite different names*

