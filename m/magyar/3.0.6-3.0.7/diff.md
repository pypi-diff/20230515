# Comparing `tmp/magyar-3.0.6.tar.gz` & `tmp/magyar-3.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magyar-3.0.6.tar", last modified: Sun May 14 21:46:25 2023, max compression
+gzip compressed data, was "magyar-3.0.7.tar", last modified: Sun May 14 22:26:12 2023, max compression
```

## Comparing `magyar-3.0.6.tar` & `magyar-3.0.7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:46:25.523926 magyar-3.0.6/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6726 2023-05-14 21:46:25.523926 magyar-3.0.6/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)     6316 2023-05-14 21:42:14.000000 magyar-3.0.6/README.md
-drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 21:46:25.523926 magyar-3.0.6/magyar.egg-info/
--rw-rw-r--   0 bela      (1000) bela      (1000)     6726 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/PKG-INFO
--rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/SOURCES.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/dependency_links.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 21:46:25.000000 magyar-3.0.6/magyar.egg-info/top_level.txt
--rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.6/magyar.py
--rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 21:46:25.523926 magyar-3.0.6/setup.cfg
--rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 21:18:14.000000 magyar-3.0.6/setup.py
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 22:26:12.952434 magyar-3.0.7/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6499 2023-05-14 22:26:12.952434 magyar-3.0.7/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6089 2023-05-14 22:25:50.000000 magyar-3.0.7/README.md
+drwxrwxr-x   0 bela      (1000) bela      (1000)        0 2023-05-14 22:26:12.952434 magyar-3.0.7/magyar.egg-info/
+-rw-rw-r--   0 bela      (1000) bela      (1000)     6499 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/PKG-INFO
+-rw-rw-r--   0 bela      (1000) bela      (1000)      148 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/SOURCES.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        1 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/dependency_links.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)        7 2023-05-14 22:26:12.000000 magyar-3.0.7/magyar.egg-info/top_level.txt
+-rw-rw-r--   0 bela      (1000) bela      (1000)    38936 2023-05-12 19:16:45.000000 magyar-3.0.7/magyar.py
+-rw-rw-r--   0 bela      (1000) bela      (1000)       38 2023-05-14 22:26:12.952434 magyar-3.0.7/setup.cfg
+-rw-rw-r--   0 bela      (1000) bela      (1000)      627 2023-05-14 22:08:52.000000 magyar-3.0.7/setup.py
```

### Comparing `magyar-3.0.6/PKG-INFO` & `magyar-3.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.6
+Version: 3.0.7
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -91,15 +91,15 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 <br>
 
 ![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
 
-</br>
+
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -123,33 +123,35 @@
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)  
 
  pl: </br>   
-magyar.tordel(magyar.leves,5) </br>
-Eredmény: </br></br>
-Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
-Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
-Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
-Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
-Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
-Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
+magyar.tordel(magyar.telepules,5) </br>
+
 
-3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
+<br>
+
+![Sima tördelés](https://raw.githubusercontent.com/kobanya/nevek/master/sima_tordel.png)
+
+<br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny <br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
 gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
-
+<br> 
+<br>
+![ABC](https://raw.githubusercontent.com/kobanya/nevek/master/abc.png)
+<br>
 4. Listák tördelése "behúzással" </br></br>
 
         magyar.ftordel(lst,n,'') 
 </br></br>
 lst = a lista neve</br>
 n = hány szó legyen egy sorban</br>
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
```

### Comparing `magyar-3.0.6/README.md` & `magyar-3.0.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -79,15 +79,15 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 <br>
 
 ![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
 
-</br>
+
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -111,33 +111,35 @@
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)  
 
  pl: </br>   
-magyar.tordel(magyar.leves,5) </br>
-Eredmény: </br></br>
-Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
-Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
-Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
-Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
-Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
-Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
+magyar.tordel(magyar.telepules,5) </br>
+
 
-3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
+<br>
+
+![Sima tördelés](https://raw.githubusercontent.com/kobanya/nevek/master/sima_tordel.png)
+
+<br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny <br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
 gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
-
+<br> 
+<br>
+![ABC](https://raw.githubusercontent.com/kobanya/nevek/master/abc.png)
+<br>
 4. Listák tördelése "behúzással" </br></br>
 
         magyar.ftordel(lst,n,'') 
 </br></br>
 lst = a lista neve</br>
 n = hány szó legyen egy sorban</br>
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
```

### Comparing `magyar-3.0.6/magyar.egg-info/PKG-INFO` & `magyar-3.0.7/magyar.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magyar
-Version: 3.0.6
+Version: 3.0.7
 Summary: Hungarian lists of names,animals,foods, fruits, rivers ..
 Home-page: https://github.com/kobanya/nevek
 Author: Nagy Béla
 Author-email: nagy.belabudapest@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -91,15 +91,15 @@
             utca = random.sample(magyar.utca, k=16) 
             random.choices()
             telepulesek = random.choice(magyar.telepules)
 <br>
 
 ![Listák](https://raw.githubusercontent.com/kobanya/nevek/master/listak.png)
 
-</br>
+
 ## Szótárak:
 Több adatot tartalmaznak összekapcsolva.
 
     magyar.kiraly tartalma :   {'király neve' : (uralkodása tól, ig)}
     magyar.megye_szekhely :    {'megye neve' : 'székhelye'}
     magyar.jaras :             {'megye' : (székhely, megye)}
     magyar.villamos:    kulcs  {'viszonylat', indulas, erkezes, menetido, varos}
@@ -123,33 +123,35 @@
     **lst** = a kiírandó lista neve </br>
     **n** = soronkénti elemek száma.  Alapbeállítás, ha üres, 10 elem
 
 
         magyar.tordel(lst , n)  
 
  pl: </br>   
-magyar.tordel(magyar.leves,5) </br>
-Eredmény: </br></br>
-Gulyásleves, Halászlé, Hideg meggyleves, Zöldborsóleves, 
-Jókai bableves, Csontleves, Marhahúsleves, Zellerkrémleves, 
-Sárgaborsóleves, Babgulyásleves, Karalábéleves, Zöldségleves, 
-Kukoricaleves, Karfiolleves, Hideg gyümölcsleves, Korhelyleves, 
-Tyúkhúsleves, Pirított tarhonyaleves, Gombaleves, Lencseleves, 
-Gulyáskrémleves, Csülökleves, Paradicsomleves, Borleves, 
+magyar.tordel(magyar.telepules,5) </br>
+
 
-3. Listák ABC sorrendbe rendezése, ékezet érzékeny </br>
+<br>
+
+![Sima tördelés](https://raw.githubusercontent.com/kobanya/nevek/master/sima_tordel.png)
+
+<br>
+3. Listák ABC sorrendbe rendezése, ékezet érzékeny <br>
 
 
          magyar.abc(lista):
 
 Használat : </br> </br>
 gyumolcs =['Áfonya', 'Eper', 'Alma', 'Meggy','Őszibarack',] </br>
 sorban =magyar.abc(gyumolcs) </br>
 ['Alma', 'Áfonya', 'Eper', 'Meggy', 'Őszibarack']
-
+<br> 
+<br>
+![ABC](https://raw.githubusercontent.com/kobanya/nevek/master/abc.png)
+<br>
 4. Listák tördelése "behúzással" </br></br>
 
         magyar.ftordel(lst,n,'') 
 </br></br>
 lst = a lista neve</br>
 n = hány szó legyen egy sorban</br>
 '  ' = a behúzás mértéke ami sztring. '\t' </br>
```

### Comparing `magyar-3.0.6/magyar.py` & `magyar-3.0.7/magyar.py`

 * *Files identical despite different names*

### Comparing `magyar-3.0.6/setup.py` & `magyar-3.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="magyar",
-    version="3.0.6",
+    version="3.0.7",
     author="Nagy Béla",
     author_email="nagy.belabudapest@gmail.com",
     description="Hungarian lists of names,animals,foods, fruits, rivers ..",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/kobanya/nevek",
     py_modules=["magyar"],
```

