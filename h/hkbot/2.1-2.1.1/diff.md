# Comparing `tmp/hkbot-2.1.tar.gz` & `tmp/hkbot-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hkbot-2.1.tar", last modified: Mon May 15 05:22:55 2023, max compression
+gzip compressed data, was "hkbot-2.1.1.tar", last modified: Mon May 15 07:27:43 2023, max compression
```

## Comparing `hkbot-2.1.tar` & `hkbot-2.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:55.577833 hkbot-2.1/
--rw-rw-rw-   0        0        0     2214 2023-05-15 05:22:55.576843 hkbot-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2073 2023-05-15 05:18:06.000000 hkbot-2.1/README.md
--rw-rw-rw-   0        0        0  1274325 2023-05-15 05:21:12.000000 hkbot-2.1/hkbot.c
-drwxrwxrwx   0        0        0        0 2023-05-15 05:22:55.574831 hkbot-2.1/hkbot.egg-info/
--rw-rw-rw-   0        0        0     2214 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      202 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-15 05:22:55.000000 hkbot-2.1/hkbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 05:22:55.577833 hkbot-2.1/setup.cfg
--rw-rw-rw-   0        0        0     1015 2023-05-15 05:15:50.000000 hkbot-2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 07:27:43.299977 hkbot-2.1.1/
+-rw-rw-rw-   0        0        0     2220 2023-05-15 07:27:43.298977 hkbot-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2077 2023-05-15 05:26:42.000000 hkbot-2.1.1/README.md
+-rw-rw-rw-   0        0        0  1274325 2023-05-15 05:21:12.000000 hkbot-2.1.1/hkbot.c
+drwxrwxrwx   0        0        0        0 2023-05-15 07:27:43.293978 hkbot-2.1.1/hkbot.egg-info/
+-rw-rw-rw-   0        0        0     2220 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       75 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-15 07:27:43.000000 hkbot-2.1.1/hkbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-15 07:27:43.300977 hkbot-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2023-05-15 07:24:39.000000 hkbot-2.1.1/setup.py
```

### Comparing `hkbot-2.1/PKG-INFO` & `hkbot-2.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkbot
-Version: 2.1
+Version: 2.1.1
 Summary: hkbot automation
 Author: AkasakaID
 Description-Content-Type: text/markdown
 
 # HKBOT Automation
 
 a program created to help complete tasks from hkbot telegram
@@ -51,13 +51,13 @@
 python3 -m pip install hkbot
 ```
 
 ## Run Program
 
 first create the config with command below
 ```
-hkbot-getconfig
+hkbot-create-config
 ```
 second, run the main command 
 ```
 hkbot
 ```
```

### Comparing `hkbot-2.1/README.md` & `hkbot-2.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -44,13 +44,13 @@
 python3 -m pip install hkbot
 ```
 
 ## Run Program
 
 first create the config with command below
 ```
-hkbot-getconfig
+hkbot-create-config
 ```
 second, run the main command 
 ```
 hkbot
 ```
```

### Comparing `hkbot-2.1/hkbot.c` & `hkbot-2.1.1/hkbot.c`

 * *Files identical despite different names*

### Comparing `hkbot-2.1/hkbot.egg-info/PKG-INFO` & `hkbot-2.1.1/hkbot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkbot
-Version: 2.1
+Version: 2.1.1
 Summary: hkbot automation
 Author: AkasakaID
 Description-Content-Type: text/markdown
 
 # HKBOT Automation
 
 a program created to help complete tasks from hkbot telegram
@@ -51,13 +51,13 @@
 python3 -m pip install hkbot
 ```
 
 ## Run Program
 
 first create the config with command below
 ```
-hkbot-getconfig
+hkbot-create-config
 ```
 second, run the main command 
 ```
 hkbot
 ```
```

### Comparing `hkbot-2.1/setup.py` & `hkbot-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,64 +1,64 @@
 00000000: 0d0a 6672 6f6d 2070 6174 686c 6962 2069  ..from pathlib i
 00000010: 6d70 6f72 7420 5061 7468 0d0a 6672 6f6d  mport Path..from
 00000020: 2073 6574 7570 746f 6f6c 7320 696d 706f   setuptools impo
 00000030: 7274 2073 6574 7570 2c20 4578 7465 6e73  rt setup, Extens
 00000040: 696f 6e0d 0a0d 0a76 6572 7369 6f6e 203d  ion....version =
-00000050: 2022 322e 3122 0d0a 6578 7465 6e73 696f   "2.1"..extensio
-00000060: 6e5f 6e61 6d65 203d 2022 6322 0d0a 6865  n_name = "c"..he
-00000070: 7265 203d 2050 6174 682e 6377 6428 290d  re = Path.cwd().
-00000080: 0a74 6869 735f 6469 7265 6374 6f72 7920  .this_directory 
-00000090: 3d20 5061 7468 285f 5f66 696c 655f 5f29  = Path(__file__)
-000000a0: 2e70 6172 656e 740d 0a6c 6f6e 675f 6465  .parent..long_de
-000000b0: 7363 7269 7074 696f 6e20 3d20 2874 6869  scription = (thi
-000000c0: 735f 6469 7265 6374 6f72 7920 2f20 2252  s_directory / "R
-000000d0: 4541 444d 452e 6d64 2229 2e72 6561 645f  EADME.md").read_
-000000e0: 7465 7874 2829 0d0a 0d0a 6578 745f 6d6f  text()....ext_mo
-000000f0: 6475 6c65 7320 3d20 5b0d 0a20 2020 2045  dules = [..    E
-00000100: 7874 656e 7369 6f6e 280d 0a20 2020 2020  xtension(..     
-00000110: 2020 2072 6573 6f75 7263 650d 0a20 2020     resource..   
-00000120: 2020 2020 202e 7374 656d 2c0d 0a20 2020       .stem,..   
-00000130: 2020 2020 2073 6f75 7263 6573 3d5b 0d0a       sources=[..
-00000140: 2020 2020 2020 2020 2020 2020 7265 736f              reso
-00000150: 7572 6365 0d0a 2020 2020 2020 2020 2020  urce..          
-00000160: 2020 2e72 656c 6174 6976 655f 746f 2868    .relative_to(h
-00000170: 6572 652e 7061 7265 6e74 290d 0a20 2020  ere.parent)..   
-00000180: 2020 2020 2020 2020 202e 6173 5f70 6f73           .as_pos
-00000190: 6978 2829 0d0a 2020 2020 2020 2020 2020  ix()..          
-000001a0: 2020 2e73 706c 6974 2822 2f22 295b 315d    .split("/")[1]
-000001b0: 0d0a 2020 2020 2020 2020 5d0d 0a20 2020  ..        ]..   
-000001c0: 2029 0d0a 2020 2020 666f 7220 7265 736f   )..    for reso
-000001d0: 7572 6365 2069 6e20 5b2a 6865 7265 2e67  urce in [*here.g
-000001e0: 6c6f 6228 6622 2a2e 7b65 7874 656e 7369  lob(f"*.{extensi
-000001f0: 6f6e 5f6e 616d 657d 2229 5d0d 0a5d 0d0a  on_name}")]..]..
-00000200: 7365 7475 7028 0d0a 2020 2020 6e61 6d65  setup(..    name
-00000210: 3d22 686b 626f 7422 2c0d 0a20 2020 2076  ="hkbot",..    v
-00000220: 6572 7369 6f6e 3d76 6572 7369 6f6e 2c0d  ersion=version,.
-00000230: 0a20 2020 2064 6573 6372 6970 7469 6f6e  .    description
-00000240: 3d22 686b 626f 7420 6175 746f 6d61 7469  ="hkbot automati
-00000250: 6f6e 222c 0d0a 2020 2020 6175 7468 6f72  on",..    author
-00000260: 3d22 416b 6173 616b 6149 4422 2c0d 0a20  ="AkasakaID",.. 
-00000270: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
-00000280: 696f 6e3d 6c6f 6e67 5f64 6573 6372 6970  ion=long_descrip
-00000290: 7469 6f6e 2c0d 0a20 2020 206c 6f6e 675f  tion,..    long_
-000002a0: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000002b0: 656e 745f 7479 7065 3d27 7465 7874 2f6d  ent_type='text/m
-000002c0: 6172 6b64 6f77 6e27 2c0d 0a20 2020 2069  arkdown',..    i
-000002d0: 6e73 7461 6c6c 5f72 6571 7569 7265 733d  nstall_requires=
-000002e0: 5b0d 0a20 2020 2020 2020 2022 7265 7175  [..        "requ
-000002f0: 6573 7473 222c 0d0a 2020 2020 2020 2020  ests",..        
-00000300: 2274 656c 6574 686f 6e22 2c0d 0a20 2020  "telethon",..   
-00000310: 2020 2020 2022 636f 6c6f 7261 6d61 222c       "colorama",
-00000320: 0d0a 2020 2020 2020 2020 2270 7974 7a22  ..        "pytz"
-00000330: 0d0a 2020 2020 5d2c 0d0a 2020 2020 6578  ..    ],..    ex
-00000340: 745f 6d6f 6475 6c65 733d 6578 745f 6d6f  t_modules=ext_mo
-00000350: 6475 6c65 732c 0d0a 2020 2020 656e 7472  dules,..    entr
-00000360: 795f 706f 696e 7473 3d7b 0d0a 2020 2020  y_points={..    
-00000370: 2020 2020 2263 6f6e 736f 6c65 5f73 6372      "console_scr
-00000380: 6970 7473 223a 205b 0d0a 2020 2020 2020  ipts": [..      
-00000390: 2020 2020 2020 2268 6b62 6f74 3d68 6b62        "hkbot=hkb
-000003a0: 6f74 3a6d 6169 6e22 2c0d 0a20 2020 2020  ot:main",..     
-000003b0: 2020 2020 2020 2022 686b 626f 742d 6372         "hkbot-cr
-000003c0: 6561 7465 2d63 6f6e 6669 673d 686b 626f  eate-config=hkbo
-000003d0: 743a 6765 7443 6f6e 6669 6722 0d0a 2020  t:getConfig"..  
-000003e0: 2020 2020 2020 2020 2020 5d0d 0a20 2020            ]..   
-000003f0: 207d 0d0a 290d 0a                         }..)..
+00000050: 2022 322e 312e 3122 0d0a 6578 7465 6e73   "2.1.1"..extens
+00000060: 696f 6e5f 6e61 6d65 203d 2022 6322 0d0a  ion_name = "c"..
+00000070: 6865 7265 203d 2050 6174 682e 6377 6428  here = Path.cwd(
+00000080: 290d 0a74 6869 735f 6469 7265 6374 6f72  )..this_director
+00000090: 7920 3d20 5061 7468 285f 5f66 696c 655f  y = Path(__file_
+000000a0: 5f29 2e70 6172 656e 740d 0a6c 6f6e 675f  _).parent..long_
+000000b0: 6465 7363 7269 7074 696f 6e20 3d20 2874  description = (t
+000000c0: 6869 735f 6469 7265 6374 6f72 7920 2f20  his_directory / 
+000000d0: 2252 4541 444d 452e 6d64 2229 2e72 6561  "README.md").rea
+000000e0: 645f 7465 7874 2829 0d0a 0d0a 6578 745f  d_text()....ext_
+000000f0: 6d6f 6475 6c65 7320 3d20 5b0d 0a20 2020  modules = [..   
+00000100: 2045 7874 656e 7369 6f6e 280d 0a20 2020   Extension(..   
+00000110: 2020 2020 2072 6573 6f75 7263 650d 0a20       resource.. 
+00000120: 2020 2020 2020 202e 7374 656d 2c0d 0a20         .stem,.. 
+00000130: 2020 2020 2020 2073 6f75 7263 6573 3d5b         sources=[
+00000140: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
+00000150: 736f 7572 6365 0d0a 2020 2020 2020 2020  source..        
+00000160: 2020 2020 2e72 656c 6174 6976 655f 746f      .relative_to
+00000170: 2868 6572 652e 7061 7265 6e74 290d 0a20  (here.parent).. 
+00000180: 2020 2020 2020 2020 2020 202e 6173 5f70             .as_p
+00000190: 6f73 6978 2829 0d0a 2020 2020 2020 2020  osix()..        
+000001a0: 2020 2020 2e73 706c 6974 2822 2f22 295b      .split("/")[
+000001b0: 315d 0d0a 2020 2020 2020 2020 5d0d 0a20  1]..        ].. 
+000001c0: 2020 2029 0d0a 2020 2020 666f 7220 7265     )..    for re
+000001d0: 736f 7572 6365 2069 6e20 5b2a 6865 7265  source in [*here
+000001e0: 2e67 6c6f 6228 6622 2a2e 7b65 7874 656e  .glob(f"*.{exten
+000001f0: 7369 6f6e 5f6e 616d 657d 2229 5d0d 0a5d  sion_name}")]..]
+00000200: 0d0a 7365 7475 7028 0d0a 2020 2020 6e61  ..setup(..    na
+00000210: 6d65 3d22 686b 626f 7422 2c0d 0a20 2020  me="hkbot",..   
+00000220: 2076 6572 7369 6f6e 3d76 6572 7369 6f6e   version=version
+00000230: 2c0d 0a20 2020 2064 6573 6372 6970 7469  ,..    descripti
+00000240: 6f6e 3d22 686b 626f 7420 6175 746f 6d61  on="hkbot automa
+00000250: 7469 6f6e 222c 0d0a 2020 2020 6175 7468  tion",..    auth
+00000260: 6f72 3d22 416b 6173 616b 6149 4422 2c0d  or="AkasakaID",.
+00000270: 0a20 2020 206c 6f6e 675f 6465 7363 7269  .    long_descri
+00000280: 7074 696f 6e3d 6c6f 6e67 5f64 6573 6372  ption=long_descr
+00000290: 6970 7469 6f6e 2c0d 0a20 2020 206c 6f6e  iption,..    lon
+000002a0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000002b0: 6e74 656e 745f 7479 7065 3d27 7465 7874  ntent_type='text
+000002c0: 2f6d 6172 6b64 6f77 6e27 2c0d 0a20 2020  /markdown',..   
+000002d0: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
+000002e0: 733d 5b0d 0a20 2020 2020 2020 2022 7265  s=[..        "re
+000002f0: 7175 6573 7473 222c 0d0a 2020 2020 2020  quests",..      
+00000300: 2020 2274 656c 6574 686f 6e22 2c0d 0a20    "telethon",.. 
+00000310: 2020 2020 2020 2022 636f 6c6f 7261 6d61         "colorama
+00000320: 222c 0d0a 2020 2020 2020 2020 2270 7974  ",..        "pyt
+00000330: 7a22 0d0a 2020 2020 5d2c 0d0a 2020 2020  z"..    ],..    
+00000340: 6578 745f 6d6f 6475 6c65 733d 6578 745f  ext_modules=ext_
+00000350: 6d6f 6475 6c65 732c 0d0a 2020 2020 656e  modules,..    en
+00000360: 7472 795f 706f 696e 7473 3d7b 0d0a 2020  try_points={..  
+00000370: 2020 2020 2020 2263 6f6e 736f 6c65 5f73        "console_s
+00000380: 6372 6970 7473 223a 205b 0d0a 2020 2020  cripts": [..    
+00000390: 2020 2020 2020 2020 2268 6b62 6f74 3d68          "hkbot=h
+000003a0: 6b62 6f74 3a6d 6169 6e22 2c0d 0a20 2020  kbot:main",..   
+000003b0: 2020 2020 2020 2020 2022 686b 626f 742d           "hkbot-
+000003c0: 6372 6561 7465 2d63 6f6e 6669 673d 686b  create-config=hk
+000003d0: 626f 743a 6765 7443 6f6e 6669 6722 0d0a  bot:getConfig"..
+000003e0: 2020 2020 2020 2020 2020 2020 5d0d 0a20              ].. 
+000003f0: 2020 207d 0d0a 290d 0a                      }..)..
```

