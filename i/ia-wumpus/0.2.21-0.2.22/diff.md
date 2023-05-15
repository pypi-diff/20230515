# Comparing `tmp/ia_wumpus-0.2.21.tar.gz` & `tmp/ia_wumpus-0.2.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ia_wumpus-0.2.21.tar", max compression
+gzip compressed data, was "ia_wumpus-0.2.22.tar", max compression
```

## Comparing `ia_wumpus-0.2.21.tar` & `ia_wumpus-0.2.22.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.2.21/LICENSE
--rw-r--r--   0        0        0     3921 2023-05-14 23:26:43.291386 ia_wumpus-0.2.21/README.md
--rw-r--r--   0        0        0       68 2023-05-13 02:13:49.858124 ia_wumpus-0.2.21/ia_wumpus/__init__.py
--rw-r--r--   0        0        0     4961 2023-05-13 02:13:49.858124 ia_wumpus-0.2.21/ia_wumpus/ambiente.py
--rw-r--r--   0        0        0      477 2023-05-15 05:22:42.310310 ia_wumpus-0.2.21/pyproject.toml
--rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 ia_wumpus-0.2.21/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 13:51:13.656383 ia_wumpus-0.2.22/LICENSE
+-rw-r--r--   0        0        0     3921 2023-05-14 23:26:43.291386 ia_wumpus-0.2.22/README.md
+-rw-r--r--   0        0        0       68 2023-05-15 05:24:04.316474 ia_wumpus-0.2.22/ia_wumpus/__init__.py
+-rw-r--r--   0        0        0     5003 2023-05-15 07:10:08.869769 ia_wumpus-0.2.22/ia_wumpus/ambiente.py
+-rw-r--r--   0        0        0      477 2023-05-15 07:13:55.134336 ia_wumpus-0.2.22/pyproject.toml
+-rw-r--r--   0        0        0     4498 1970-01-01 00:00:00.000000 ia_wumpus-0.2.22/PKG-INFO
```

### Comparing `ia_wumpus-0.2.21/LICENSE` & `ia_wumpus-0.2.22/LICENSE`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.21/README.md` & `ia_wumpus-0.2.22/README.md`

 * *Files identical despite different names*

### Comparing `ia_wumpus-0.2.21/ia_wumpus/ambiente.py` & `ia_wumpus-0.2.22/ia_wumpus/ambiente.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,37 +20,43 @@
 
         # Percepções
         self.percepcoes: dict = {"pocos":  [],
                                  "wumpus": [],
                                  "ouro":   []}
 
         # Posicionando o Agente no ambiente.
-        self.add_pos_agente()
+        self.__add_pos_agente()
         # Posicionando o(s) Wumpu(s) no ambiente.
-        self.add_pos_wumpus()
+        self.__add_pos_wumpus()
         # Posicionando o(s) Poço(s) no ambiente.
-        self.add_pos_pocos()
+        self.__add_pos_pocos()
         # Posicionando o(s) Ouro(s) no ambiente.
-        self.add_pos_ouro()
+        self.__add_pos_ouro()
         # Menu
-        self.menu()
+        self.__menu()
 
     def add_pos_obj(self, obj: int) -> npt.NDArray:
         """Posiciona os Objetos no Ambiente."""
-        self.pos_sort = self.sortear_pos()
+        self.pos_sort = self.__sortear_pos()
         if self.mundo[self.pos_sort[0], self.pos_sort[1]] == 0:
             self.mundo[self.pos_sort[0], self.pos_sort[1]] = obj
             return self.pos_sort
         elif ((self.pos_sort[0] == 0) and (self.pos_sort[1] == 0)):
             self.add_pos_obj(obj)
         else:
             self.add_pos_obj(obj)
         return self.pos_sort
 
-    def add_percepcoes(self, objeto: str, pos: npt.NDArray) -> None:
+    def __sortear_pos(self) -> npt.NDArray:
+        """Sortea as posições dos Objetos no Ambiente."""
+        x = randint(0, self.dimensoes[0]-1)
+        y = randint(0, self.dimensoes[0]-1)
+        return np.array([x, y])
+
+    def __add_percepcoes_obj(self, objeto: str, pos: npt.NDArray) -> None:
         """Posiciona as percepções no Ambiente."""
         if pos[0] == 0:
             self.percepcoes[objeto].append((pos[1], pos[0] + 1))
         elif pos[0] == (self.dimensoes[0] - 1):
             self.percepcoes[objeto].append((pos[1], pos[0] - 1))
         elif (pos[0] > 0) and (pos[0] < (self.dimensoes[0] - 1)):
             self.percepcoes[objeto].append((pos[1], pos[0] + 1))
@@ -60,55 +66,49 @@
             self.percepcoes[objeto].append((pos[1] + 1, pos[0]))
         elif pos[1] == (self.dimensoes[0] - 1):
             self.percepcoes[objeto].append((pos[1] - 1, pos[0]))
         elif (pos[1] > 0) and (pos[1] < (self.dimensoes[0] - 1)):
             self.percepcoes[objeto].append((pos[1] + 1, pos[0]))
             self.percepcoes[objeto].append((pos[1] - 1, pos[0]))
 
-    def add_pos_wumpus(self) -> None:
+    def __add_pos_wumpus(self) -> None:
         """Posicionando os Wumpo(s) no Ambiente."""
         for i in range(self.wumpus):
             pos_wumpus = self.add_pos_obj(1)
-            self.add_percepcoes(objeto="wumpus", pos=pos_wumpus)
+            self.__add_percepcoes_obj(objeto="wumpus", pos=pos_wumpus)
             # print(f"Wumpus pos: {pos_wumpus}")
 
-    def add_pos_pocos(self) -> None:
+    def __add_pos_pocos(self) -> None:
         """Posicionando os Poços no Ambiente."""
         for i in range(self.pocos):
             pos_poco = self.add_pos_obj(2)
-            self.add_percepcoes(objeto="pocos", pos=pos_poco)
+            self.__add_percepcoes_obj(objeto="pocos", pos=pos_poco)
             # print(f"Poço pos: {pos_poco}")
 
-    def add_pos_ouro(self) -> None:
+    def __add_pos_ouro(self) -> None:
         """Posicionando o(s) Ouro(s) no Ambiente."""
         for i in range(self.ouro):
             pos_ouro = self.add_pos_obj(3)
             self.percepcoes["ouro"].append((pos_ouro[1], pos_ouro[0]))
             # print(f"Ouro pos: {pos_ouro}")
 
-    def sortear_pos(self) -> npt.NDArray:
-        """Sortea as posições dos Objetos no Ambiente."""
-        x = randint(0, self.dimensoes[0]-1)
-        y = randint(0, self.dimensoes[0]-1)
-        return np.array([x, y])
+    def __add_pos_agente(self) -> None:
+        """Posicionando o(s) Agente(s) no Ambiente."""
+        self.mundo[0, 0] = 4
 
     @classmethod
-    def menu(self) -> None:
+    def __menu(self) -> None:
         """Menu com a descrições dos Objetos."""
         print("\n====== Menu - Mundo do Wumpus ======")
         print("\t+ 1 - Wumpus")
         print("\t+ 2 - Poços")
         print("\t+ 3 - Ouro")
         print("\t+ 4 - Agente")
         print("====================================")
 
-    def add_pos_agente(self) -> None:
-        """Posicionando o(s) Agente(s) no Ambiente."""
-        self.mundo[0, 0] = 4
-
     def infos_ambiente(self) -> None:
         """Exibe a dimensão do mundo do Wumpus."""
         print(f"\nTamanho do Ambiente: {self.mundo.shape}")
 
     def mostrar_ambiente(self) -> None:
         """Exibe o Mundo do Wumpus com os objetos em suas posições."""
         print(f"\nMundo do Wumpus:\n{self.mundo}")
```

### Comparing `ia_wumpus-0.2.21/PKG-INFO` & `ia_wumpus-0.2.22/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ia-wumpus
-Version: 0.2.21
+Version: 0.2.22
 Summary: Projeto O Mundo do Wumpus - Anbiente para estudo da disciplina de Inteligencia Computacional.
 Author: Oseiasdfarias
 Author-email: oseias.dfarias@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

