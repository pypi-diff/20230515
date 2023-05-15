# Comparing `tmp/magyar-3.0.7.tar.gz` & `tmp/magyar-3.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.7.tar", last modified: Sun May 14 22:26:12 2023, max compression
+gzip compressed data, was "magyar-3.0.8.tar", last modified: Mon May 15 07:47:21 2023, max compression
```

## Comparing `magyar-3.0.7.tar` & `magyar-3.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 22:26:12.952434 magyar-3.0.7/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6499 2023-05-14 22:26:12.952434 magyar-3.0.7/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6089 2023-05-14 22:25:50.000000 magyar-3.0.7/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 22:26:12.952434 magyar-3.0.7/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6499 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.7/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 22:26:12.952434 magyar-3.0.7/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 22:08:52.000000 magyar-3.0.7/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-15 07:47:21.897201 magyar-3.0.8/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6599 2023-05-15 07:47:21.897201 magyar-3.0.8/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6189 2023-05-15 07:45:16.000000 magyar-3.0.8/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-15 07:47:21.897201 magyar-3.0.8/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6599 2023-05-15 07:47:21.000000 magyar-3.0.8/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-15 07:47:21.000000 magyar-3.0.8/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-15 07:47:21.000000 magyar-3.0.8/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-15 07:47:21.000000 magyar-3.0.8/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.8/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-15 07:47:21.897201 magyar-3.0.8/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-15 07:29:49.000000 magyar-3.0.8/setup.py
```

### Comparing `magyar-3.0.7/PKG-INFO` & `magyar-3.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.7
+Version: 3.0.8
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
 22. Magyar desszertek = magyar.**desszert**
 23. Magyar borok = magyar.**bor**
-24. Magyar üdítők= magyar.**utito**
+24. Magyar üdítők= magyar.**udito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -114,15 +114,18 @@
 Pl: </br>
     import magyar</br>
     print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
 Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
+<br>
+![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/jaras_szotar.png)
 
+<br>
 2. A listák tartalmának kiíratása tetszőleges elemmel soronként.</br>
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)
```

### Comparing `magyar-3.0.7/README.md` & `magyar-3.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
 22. Magyar desszertek = magyar.**desszert**
 23. Magyar borok = magyar.**bor**
-24. Magyar üdítők= magyar.**utito**
+24. Magyar üdítők= magyar.**udito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -102,15 +102,18 @@
 Pl: </br>
     import magyar</br>
     print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
 Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
+<br>
+![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/jaras_szotar.png)
 
+<br>
 2. A listák tartalmának kiíratása tetszőleges elemmel soronként.</br>
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)
```

### Comparing `magyar-3.0.7/magyar.egg-info/PKG-INFO` & `magyar-3.0.8/magyar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.7
+Version: 3.0.8
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -35,15 +35,15 @@
 17. A naprendszer bolygóinak magyar neve = magyar.**bolygo**
 18. Magyar leves nevek =  magyar.**leves**
 19. Magyar főételek = magyar.**foetel**
 20. Magyar köretek = magyar.**koret**
 21. Magyar egytál ételek = magyar.**egytal**
 22. Magyar desszertek = magyar.**desszert**
 23. Magyar borok = magyar.**bor**
-24. Magyar üdítők= magyar.**utito**
+24. Magyar üdítők= magyar.**udito**
 
 ## Szótárak  (dictionary): 
 1. Királyok és uralkodásuk ideje  = magyar.kiraly
 2. Vármegyék és azok székhelyei = magyar.megye_szekhely
 3. Járások, székhelyük , megye = magyar.jaras
 4. Villamosvonalak, végállomások, menetidő = magyar.villamos
 5. Európa országai és fővárosai=  magyar.orszag
@@ -114,15 +114,18 @@
 Pl: </br>
     import magyar</br>
     print(magyar.szotarbol_veletlen_kulcs(magyar.jaras,15)) </br></br>
 Eredmény: </br>
     ['Szekszárdi járás', 'Gönci járás', 'Szigetvári járás', 'Mezőkovácsházi járás', 'Bátonyterenyei járás',
     'Körmendi járás', 'Váci járás', 'Edelényi járás', 'Pilisvörösvári járás', 'Kaposvári járás', 'Hódmezővásárhelyi járás',
     'Hatvani járás', 'Törökszentmiklósi járás', 'Putnoki járás', 'Mezőkövesdi járás']
+<br>
+![ABC rendezés](https://raw.githubusercontent.com/kobanya/nevek/master/jaras_szotar.png)
 
+<br>
 2. A listák tartalmának kiíratása tetszőleges elemmel soronként.</br>
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)
```

### Comparing `magyar-3.0.7/magyar.py` & `magyar-3.0.8/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-3.0.7/setup.py` & `magyar-3.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.7",
+    version="3.0.8",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

