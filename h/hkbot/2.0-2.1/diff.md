# Comparing `tmp/hkbot-2.0.tar.gz` & `tmp/hkbot-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkbot-2.0.tar", last modified: Mon May 15 05:11:19 2023, max compression
+gzip compressed data, was "hkbot-2.1.tar", last modified: Mon May 15 05:22:55 2023, max compression
```

## Comparing `hkbot-2.0.tar` & `hkbot-2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:11:19.938193 hkbot-2.0/
--rw-rw-rw-   0        0        0       96 2023-05-15 05:11:19.937193 hkbot-2.0/PKG-INFO
--rw-rw-rw-   0        0        0      715 2023-05-14 21:37:16.000000 hkbot-2.0/README.md
--rw-rw-rw-   0        0        0  1274238 2023-05-15 05:10:50.000000 hkbot-2.0/hkbot.c
-drwxrwxrwx   0        0        0        0 2023-05-15 05:11:19.935191 hkbot-2.0/hkbot.egg-info/
--rw-rw-rw-   0        0        0       96 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 05:11:19.000000 hkbot-2.0/hkbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 05:11:19.938193 hkbot-2.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-05-15 04:57:04.000000 hkbot-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:55.577833 hkbot-2.1/
+-rw-rw-rw-   0        0        0     2214 2023-05-15 05:22:55.576843 hkbot-2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2073 2023-05-15 05:18:06.000000 hkbot-2.1/README.md
+-rw-rw-rw-   0        0        0  1274325 2023-05-15 05:21:12.000000 hkbot-2.1/hkbot.c
+drwxrwxrwx   0        0        0        0 2023-05-15 05:22:55.574831 hkbot-2.1/hkbot.egg-info/
+-rw-rw-rw-   0        0        0     2214 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 05:22:55.577833 hkbot-2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2023-05-15 05:15:50.000000 hkbot-2.1/setup.py
```

### Comparing `hkbot-2.0/hkbot.c` & `hkbot-2.1/hkbot.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,16 @@
+
 /*
-AUTHOR : AkasakaID
-*/
+Author  : AkasakaID
+Youtube : https://youtube.com/@fawwazthoerif
+Github  : https://github.com/AkasakaID
 
 
+*/
+
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
@@ -2668,15 +2672,15 @@
 static PyObject *__pyx_pf_5hkbot_3Bot_34autoWithdraw(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self);
 static PyObject *__pyx_pf_5hkbot_3Bot_36setWallet(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self);
 static PyObject *__pyx_pf_5hkbot_3Bot_38main(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_self);
 static PyObject *__pyx_pf_5hkbot_main(CYTHON_UNUSED PyObject *__pyx_self);
 static PyObject *__pyx_pf_5hkbot_2getConfig(CYTHON_UNUSED PyObject *__pyx_self);
 static PyObject *__pyx_tp_new_5hkbot___pyx_scope_struct__gocap(PyTypeObject *t, PyObject *a, PyObject *k);
 static PyObject *__pyx_tp_new_5hkbot___pyx_scope_struct_1_genexpr(PyTypeObject *t, PyObject *a, PyObject *k);
-static PyObject *__pyx_float_2_0;
+static PyObject *__pyx_float_2_1;
 static PyObject *__pyx_float_0_01;
 static PyObject *__pyx_float_0_14;
 static PyObject *__pyx_float_0_086;
 static PyObject *__pyx_float_0_000021;
 static PyObject *__pyx_float_0_000025;
 static PyObject *__pyx_float_0_00000059;
 static PyObject *__pyx_float_0_00000820;
@@ -2778,15 +2782,15 @@
   PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
  
-  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_currentVersion, __pyx_float_2_0) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
+  if (__Pyx_PyObject_SetAttrStr(__pyx_v_self, __pyx_n_s_currentVersion, __pyx_float_2_1) < 0) __PYX_ERR(0, 35, __pyx_L1_error)
 
  
   __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_putih); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = PyNumber_Add(__pyx_t_1, __pyx_kp_u_); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -21966,15 +21970,15 @@
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_float_2_0 = PyFloat_FromDouble(2.0); if (unlikely(!__pyx_float_2_0)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_float_2_1 = PyFloat_FromDouble(2.1); if (unlikely(!__pyx_float_2_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_01 = PyFloat_FromDouble(0.01); if (unlikely(!__pyx_float_0_01)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_14 = PyFloat_FromDouble(0.14); if (unlikely(!__pyx_float_0_14)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_086 = PyFloat_FromDouble(0.086); if (unlikely(!__pyx_float_0_086)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_000021 = PyFloat_FromDouble(0.000021); if (unlikely(!__pyx_float_0_000021)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_000025 = PyFloat_FromDouble(0.000025); if (unlikely(!__pyx_float_0_000025)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_00000059 = PyFloat_FromDouble(0.00000059); if (unlikely(!__pyx_float_0_00000059)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_float_0_00000820 = PyFloat_FromDouble(0.00000820); if (unlikely(!__pyx_float_0_00000820)) __PYX_ERR(0, 1, __pyx_L1_error)
```

### Comparing `hkbot-2.0/setup.py` & `hkbot-2.1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,64 @@
 00000000: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
 00000010: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
 00000020: 2073 6574 7570 746f 6f6c 7320 696d 706f   setuptools impo
 00000030: 7274 2073 6574 7570 2c20 4578 7465 6e73  rt setup, Extens
 00000040: 696f 6e0d 0a0d 0a76 6572 7369 6f6e 203d  ion....version =
-00000050: 2022 322e 3022 0d0a 6578 7465 6e73 696f   "2.0"..extensio
+00000050: 2022 322e 3122 0d0a 6578 7465 6e73 696f   "2.1"..extensio
 00000060: 6e5f 6e61 6d65 203d 2022 6322 0d0a 6865  n_name = "c"..he
 00000070: 7265 203d 2050 6174 682e 6377 6428 290d  re = Path.cwd().
-00000080: 0a0d 0a0d 0a65 7874 5f6d 6f64 756c 6573  .....ext_modules
-00000090: 203d 205b 0d0a 2020 2020 4578 7465 6e73   = [..    Extens
-000000a0: 696f 6e28 0d0a 2020 2020 2020 2020 7265  ion(..        re
-000000b0: 736f 7572 6365 0d0a 2020 2020 2020 2020  source..        
-000000c0: 2e73 7465 6d2c 0d0a 2020 2020 2020 2020  .stem,..        
-000000d0: 736f 7572 6365 733d 5b0d 0a20 2020 2020  sources=[..     
-000000e0: 2020 2020 2020 2072 6573 6f75 7263 650d         resource.
-000000f0: 0a20 2020 2020 2020 2020 2020 202e 7265  .            .re
-00000100: 6c61 7469 7665 5f74 6f28 6865 7265 2e70  lative_to(here.p
-00000110: 6172 656e 7429 0d0a 2020 2020 2020 2020  arent)..        
-00000120: 2020 2020 2e61 735f 706f 7369 7828 290d      .as_posix().
-00000130: 0a20 2020 2020 2020 2020 2020 202e 7370  .            .sp
-00000140: 6c69 7428 222f 2229 5b31 5d0d 0a20 2020  lit("/")[1]..   
-00000150: 2020 2020 205d 0d0a 2020 2020 290d 0a20       ]..    ).. 
-00000160: 2020 2066 6f72 2072 6573 6f75 7263 6520     for resource 
-00000170: 696e 205b 2a68 6572 652e 676c 6f62 2866  in [*here.glob(f
-00000180: 222a 2e7b 6578 7465 6e73 696f 6e5f 6e61  "*.{extension_na
-00000190: 6d65 7d22 295d 0d0a 5d0d 0a73 6574 7570  me}")]..]..setup
-000001a0: 280d 0a20 2020 206e 616d 653d 2268 6b62  (..    name="hkb
-000001b0: 6f74 222c 0d0a 2020 2020 7665 7273 696f  ot",..    versio
-000001c0: 6e3d 7665 7273 696f 6e2c 0d0a 2020 2020  n=version,..    
-000001d0: 6465 7363 7269 7074 696f 6e3d 2268 6b62  description="hkb
-000001e0: 6f74 2061 7574 6f6d 6174 696f 6e22 2c0d  ot automation",.
-000001f0: 0a20 2020 2061 7574 686f 723d 2241 6b61  .    author="Aka
-00000200: 7361 6b61 4944 222c 0d0a 2020 2020 696e  sakaID",..    in
-00000210: 7374 616c 6c5f 7265 7175 6972 6573 3d5b  stall_requires=[
-00000220: 0d0a 2020 2020 2020 2020 2272 6571 7565  ..        "reque
-00000230: 7374 7322 2c0d 0a20 2020 2020 2020 2022  sts",..        "
-00000240: 7465 6c65 7468 6f6e 222c 0d0a 2020 2020  telethon",..    
-00000250: 2020 2020 2263 6f6c 6f72 616d 6122 2c0d      "colorama",.
-00000260: 0a20 2020 2020 2020 2022 7079 747a 220d  .        "pytz".
-00000270: 0a20 2020 205d 2c0d 0a20 2020 2065 7874  .    ],..    ext
-00000280: 5f6d 6f64 756c 6573 3d65 7874 5f6d 6f64  _modules=ext_mod
-00000290: 756c 6573 2c0d 0a20 2020 2065 6e74 7279  ules,..    entry
-000002a0: 5f70 6f69 6e74 733d 7b0d 0a20 2020 2020  _points={..     
-000002b0: 2020 2022 636f 6e73 6f6c 655f 7363 7269     "console_scri
-000002c0: 7074 7322 3a20 5b0d 0a20 2020 2020 2020  pts": [..       
-000002d0: 2020 2020 2022 686b 626f 743d 686b 626f       "hkbot=hkbo
-000002e0: 743a 6d61 696e 222c 0d0a 2020 2020 2020  t:main",..      
-000002f0: 2020 2020 2020 2268 6b62 6f74 2d63 7265        "hkbot-cre
-00000300: 6174 652d 636f 6e66 6967 3d68 6b62 6f74  ate-config=hkbot
-00000310: 3a67 6574 436f 6e66 6967 220d 0a20 2020  :getConfig"..   
-00000320: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
-00000330: 7d0d 0a29 0d0a                           }..)..
+00000080: 0a74 6869 735f 6469 7265 6374 6f72 7920  .this_directory 
+00000090: 3d20 5061 7468 285f 5f66 696c 655f 5f29  = Path(__file__)
+000000a0: 2e70 6172 656e 740d 0a6c 6f6e 675f 6465  .parent..long_de
+000000b0: 7363 7269 7074 696f 6e20 3d20 2874 6869  scription = (thi
+000000c0: 735f 6469 7265 6374 6f72 7920 2f20 2252  s_directory / "R
+000000d0: 4541 444d 452e 6d64 2229 2e72 6561 645f  EADME.md").read_
+000000e0: 7465 7874 2829 0d0a 0d0a 6578 745f 6d6f  text()....ext_mo
+000000f0: 6475 6c65 7320 3d20 5b0d 0a20 2020 2045  dules = [..    E
+00000100: 7874 656e 7369 6f6e 280d 0a20 2020 2020  xtension(..     
+00000110: 2020 2072 6573 6f75 7263 650d 0a20 2020     resource..   
+00000120: 2020 2020 202e 7374 656d 2c0d 0a20 2020       .stem,..   
+00000130: 2020 2020 2073 6f75 7263 6573 3d5b 0d0a       sources=[..
+00000140: 2020 2020 2020 2020 2020 2020 7265 736f              reso
+00000150: 7572 6365 0d0a 2020 2020 2020 2020 2020  urce..          
+00000160: 2020 2e72 656c 6174 6976 655f 746f 2868    .relative_to(h
+00000170: 6572 652e 7061 7265 6e74 290d 0a20 2020  ere.parent)..   
+00000180: 2020 2020 2020 2020 202e 6173 5f70 6f73           .as_pos
+00000190: 6978 2829 0d0a 2020 2020 2020 2020 2020  ix()..          
+000001a0: 2020 2e73 706c 6974 2822 2f22 295b 315d    .split("/")[1]
+000001b0: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
+000001c0: 2029 0d0a 2020 2020 666f 7220 7265 736f   )..    for reso
+000001d0: 7572 6365 2069 6e20 5b2a 6865 7265 2e67  urce in [*here.g
+000001e0: 6c6f 6228 6622 2a2e 7b65 7874 656e 7369  lob(f"*.{extensi
+000001f0: 6f6e 5f6e 616d 657d 2229 5d0d 0a5d 0d0a  on_name}")]..]..
+00000200: 7365 7475 7028 0d0a 2020 2020 6e61 6d65  setup(..    name
+00000210: 3d22 686b 626f 7422 2c0d 0a20 2020 2076  ="hkbot",..    v
+00000220: 6572 7369 6f6e 3d76 6572 7369 6f6e 2c0d  ersion=version,.
+00000230: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
+00000240: 3d22 686b 626f 7420 6175 746f 6d61 7469  ="hkbot automati
+00000250: 6f6e 222c 0d0a 2020 2020 6175 7468 6f72  on",..    author
+00000260: 3d22 416b 6173 616b 6149 4422 2c0d 0a20  ="AkasakaID",.. 
+00000270: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
+00000280: 696f 6e3d 6c6f 6e67 5f64 6573 6372 6970  ion=long_descrip
+00000290: 7469 6f6e 2c0d 0a20 2020 206c 6f6e 675f  tion,..    long_
+000002a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
+000002b0: 656e 745f 7479 7065 3d27 7465 7874 2f6d  ent_type='text/m
+000002c0: 6172 6b64 6f77 6e27 2c0d 0a20 2020 2069  arkdown',..    i
+000002d0: 6e73 7461 6c6c 5f72 6571 7569 7265 733d  nstall_requires=
+000002e0: 5b0d 0a20 2020 2020 2020 2022 7265 7175  [..        "requ
+000002f0: 6573 7473 222c 0d0a 2020 2020 2020 2020  ests",..        
+00000300: 2274 656c 6574 686f 6e22 2c0d 0a20 2020  "telethon",..   
+00000310: 2020 2020 2022 636f 6c6f 7261 6d61 222c       "colorama",
+00000320: 0d0a 2020 2020 2020 2020 2270 7974 7a22  ..        "pytz"
+00000330: 0d0a 2020 2020 5d2c 0d0a 2020 2020 6578  ..    ],..    ex
+00000340: 745f 6d6f 6475 6c65 733d 6578 745f 6d6f  t_modules=ext_mo
+00000350: 6475 6c65 732c 0d0a 2020 2020 656e 7472  dules,..    entr
+00000360: 795f 706f 696e 7473 3d7b 0d0a 2020 2020  y_points={..    
+00000370: 2020 2020 2263 6f6e 736f 6c65 5f73 6372      "console_scr
+00000380: 6970 7473 223a 205b 0d0a 2020 2020 2020  ipts": [..      
+00000390: 2020 2020 2020 2268 6b62 6f74 3d68 6b62        "hkbot=hkb
+000003a0: 6f74 3a6d 6169 6e22 2c0d 0a20 2020 2020  ot:main",..     
+000003b0: 2020 2020 2020 2022 686b 626f 742d 6372         "hkbot-cr
+000003c0: 6561 7465 2d63 6f6e 6669 673d 686b 626f  eate-config=hkbo
+000003d0: 743a 6765 7443 6f6e 6669 6722 0d0a 2020  t:getConfig"..  
+000003e0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
+000003f0: 207d 0d0a 290d 0a                         }..)..
```

