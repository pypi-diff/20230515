# Comparing `tmp/chyp-0.3.2.tar.gz` & `tmp/chyp-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.3.2.tar", last modified: Sat May 13 12:30:19 2023, max compression
+gzip compressed data, was "chyp-0.3.3.tar", last modified: Mon May 15 12:11:41 2023, max compression
```

## Comparing `chyp-0.3.2.tar` & `chyp-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-13 12:30:19.371249 chyp-0.3.2/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3.2/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9929 2023-05-13 12:30:19.371249 chyp-0.3.2/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9388 2023-05-13 12:23:04.000000 chyp-0.3.2/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-13 12:30:19.371249 chyp-0.3.2/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3.2/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3.2/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3.2/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-13 12:30:19.371249 chyp-0.3.2/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3.2/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3.2/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3.2/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     5986 2023-05-11 09:13:14.000000 chyp-0.3.2/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    15296 2023-05-11 09:14:44.000000 chyp-0.3.2/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3.2/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3.2/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3.2/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3.2/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3.2/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10454 2023-05-13 12:29:20.000000 chyp-0.3.2/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11254 2023-05-10 22:12:14.000000 chyp-0.3.2/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     8791 2023-05-13 11:26:15.000000 chyp-0.3.2/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3.2/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3.2/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3.2/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4602 2023-05-11 09:04:26.000000 chyp-0.3.2/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4143 2023-05-11 20:25:03.000000 chyp-0.3.2/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-13 12:30:19.371249 chyp-0.3.2/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     9929 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-13 12:30:19.000000 chyp-0.3.2/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3.2/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-13 12:30:19.371249 chyp-0.3.2/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-13 12:30:04.000000 chyp-0.3.2/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.3.3/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-15 12:11:41.629822 chyp-0.3.3/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     9508 2023-05-13 17:50:25.000000 chyp-0.3.3/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      727 2023-05-01 10:30:52.000000 chyp-0.3.3/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      699 2023-05-01 10:09:37.000000 chyp-0.3.3/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16930 2023-05-08 13:24:18.000000 chyp-0.3.3/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      634 2023-05-01 10:14:39.000000 chyp-0.3.3/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3739 2023-05-09 07:10:05.000000 chyp-0.3.3/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1108 2023-05-06 10:32:00.000000 chyp-0.3.3/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     5986 2023-05-11 09:13:14.000000 chyp-0.3.3/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15809 2023-05-15 12:09:38.000000 chyp-0.3.3/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2283 2023-05-08 16:45:36.000000 chyp-0.3.3/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     7056 2023-05-05 22:42:20.000000 chyp-0.3.3/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1242 2023-05-05 22:33:30.000000 chyp-0.3.3/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2357 2023-05-08 12:36:17.000000 chyp-0.3.3/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1672 2023-05-05 22:32:53.000000 chyp-0.3.3/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10454 2023-05-13 12:29:20.000000 chyp-0.3.3/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11316 2023-05-15 07:42:45.000000 chyp-0.3.3/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8791 2023-05-13 11:26:15.000000 chyp-0.3.3/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3774 2023-05-07 18:11:57.000000 chyp-0.3.3/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1775 2023-05-08 10:53:38.000000 chyp-0.3.3/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.3.3/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4602 2023-05-11 09:04:26.000000 chyp-0.3.3/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4143 2023-05-11 20:25:03.000000 chyp-0.3.3/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-15 12:11:41.629822 chyp-0.3.3/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10049 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      588 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-15 12:11:41.000000 chyp-0.3.3/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.3.3/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-15 12:11:41.629822 chyp-0.3.3/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1065 2023-05-15 12:11:16.000000 chyp-0.3.3/setup.py
```

### Comparing `chyp-0.3.2/LICENSE` & `chyp-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/PKG-INFO` & `chyp-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3.2
+Version: 0.3.3
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Chyp (pronounced "chip") is an interactive theorem prover for symmetric monoidal categories (SMCs), a.k.a. process theories. Symmetric monoidal categories are a very general way to reason about processes that can be composed in sequence or in parallel. String diagrams are a convenient notation for maps in an SMC, where processes are represented as boxes connected to each other by wires.
 
 ![Chyp screenshot](https://github.com/akissinger/chyp/raw/master/chyp-screen.png)
 
-Chyp is short for _Composing HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching to a combinatoric structure based on hypergraphs, we obtain a convenient rewrite theory for string diagrams. There is a lot of theory behind this, which has been developed over a series of papers:
+Chyp is short for _Cospans of HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching from terms to this combinatoric structure, we obtain a convenient rewrite theory for string diagrams that automatically handles the extra "bureaucracy" that comes from working with sequential and parallel composition together. There is a lot of theory behind this, which has been developed over a series of papers:
 
 * [String Diagram Rewrite Theory I: Rewriting with Frobenius Structure](https://arxiv.org/abs/2012.01847)
 * [String Diagram Rewrite Theory II: Rewriting with Symmetric Monoidal Structure](https://arxiv.org/abs/2104.14686)
 * [String diagram rewrite theory III: Confluence with and without Frobenius](https://discovery.ucl.ac.uk/id/eprint/10151067/1/string-diagram-rewrite-theory-iii-confluence-with-and-without-frobenius.pdf)
 
 Currently, Chyp implements the theory described in part II, using monogamous acyclic hypergraphs to represent morphisms in a symmetric monoidal category. Fancier types of rewriting (e.g. rewriting modulo Frobenius structure) is planned for the future.
 
@@ -86,14 +86,15 @@
 Note these indices are local to the swap map, so splitting or combining swap maps will change some indices in general. For example:
 
     sw[1, 2, 0] * sw[1, 0] = sw[1, 2, 0, 4, 3]
 
 
 ## Rules and rewriting
 
+
 An algebraic theory can be presented by introducing some generators as well as some rewrite rules. Rules are defined via the `rule` statement, which gives the rule a name, then takes as input a pair of terms with the same number of inputs and outputs. For example, we could introduce a pair of rules relating the `f` and `g` generators as follows:
 
     rule assoc : f * id ; f = id * f ; f
     rule bialg : f ; g = g * g ; id * sw * id ; f * f
 
 Now for the good part! The `rewrite` statement represents a transitive chain of rule applications. It consists of the keyword `rewrite` followed by a name to use for the resulting theorem, then a sequence of equalities, each giving a justifying rule. For example:
```

### Comparing `chyp-0.3.2/README.md` & `chyp-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Chyp (pronounced "chip") is an interactive theorem prover for symmetric monoidal categories (SMCs), a.k.a. process theories. Symmetric monoidal categories are a very general way to reason about processes that can be composed in sequence or in parallel. String diagrams are a convenient notation for maps in an SMC, where processes are represented as boxes connected to each other by wires.
 
 ![Chyp screenshot](https://github.com/akissinger/chyp/raw/master/chyp-screen.png)
 
-Chyp is short for _Composing HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching to a combinatoric structure based on hypergraphs, we obtain a convenient rewrite theory for string diagrams. There is a lot of theory behind this, which has been developed over a series of papers:
+Chyp is short for _Cospans of HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching from terms to this combinatoric structure, we obtain a convenient rewrite theory for string diagrams that automatically handles the extra "bureaucracy" that comes from working with sequential and parallel composition together. There is a lot of theory behind this, which has been developed over a series of papers:
 
 * [String Diagram Rewrite Theory I: Rewriting with Frobenius Structure](https://arxiv.org/abs/2012.01847)
 * [String Diagram Rewrite Theory II: Rewriting with Symmetric Monoidal Structure](https://arxiv.org/abs/2104.14686)
 * [String diagram rewrite theory III: Confluence with and without Frobenius](https://discovery.ucl.ac.uk/id/eprint/10151067/1/string-diagram-rewrite-theory-iii-confluence-with-and-without-frobenius.pdf)
 
 Currently, Chyp implements the theory described in part II, using monogamous acyclic hypergraphs to represent morphisms in a symmetric monoidal category. Fancier types of rewriting (e.g. rewriting modulo Frobenius structure) is planned for the future.
 
@@ -70,14 +70,15 @@
 Note these indices are local to the swap map, so splitting or combining swap maps will change some indices in general. For example:
 
     sw[1, 2, 0] * sw[1, 0] = sw[1, 2, 0, 4, 3]
 
 
 ## Rules and rewriting
 
+
 An algebraic theory can be presented by introducing some generators as well as some rewrite rules. Rules are defined via the `rule` statement, which gives the rule a name, then takes as input a pair of terms with the same number of inputs and outputs. For example, we could introduce a pair of rules relating the `f` and `g` generators as follows:
 
     rule assoc : f * id ; f = id * f ; f
     rule bialg : f ; g = g * g ; id * sw * id ; f * f
 
 Now for the good part! The `rewrite` statement represents a transitive chain of rule applications. It consists of the keyword `rewrite` followed by a name to use for the resulting theorem, then a sequence of equalities, each giving a justifying rule. For example:
```

### Comparing `chyp-0.3.2/chyp/__init__.py` & `chyp-0.3.3/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/__main__.py` & `chyp-0.3.3/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/graph.py` & `chyp-0.3.3/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/__init__.py` & `chyp-0.3.3/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/app.py` & `chyp-0.3.3/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/codeview.py` & `chyp-0.3.3/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/document.py` & `chyp-0.3.3/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/editor.py` & `chyp-0.3.3/chyp/gui/editor.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
 from typing import Callable, Dict, Optional, Tuple
-from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, Qt, QSettings
+from PySide6.QtCore import QByteArray, QFileInfo, QObject, QThread, QTimer, Qt, QSettings
 from PySide6.QtGui import QCloseEvent, QKeySequence, QTextCursor
 from PySide6.QtWidgets import QApplication, QHBoxLayout, QMainWindow, QMenuBar, QSplitter, QTreeView, QVBoxLayout, QWidget
 
 from ..layout import convex_layout
 from ..graph import Graph
 from ..state import RewriteState, State
 from ..term import graph_to_term
@@ -90,14 +90,17 @@
         self.code_view.cursorPositionChanged.connect(self.show_at_cursor)
         self.code_view.textChanged.connect(self.invalidate_text)
         self.parsed = True
 
         # keep a cache of graphs that have already been laid out
         self.graph_cache : Dict[int, Tuple[Graph, Optional[Graph]]] = dict()
 
+        # keep a revision count, so we don't trigger parsing until the user stops typing for a bit
+        self.revision = 0
+
     def build_menu(self) -> None:
         menu = QMenuBar()
         file_menu = menu.addMenu("&File")
         edit_menu = menu.addMenu("&Edit")
         code_menu = menu.addMenu("&Code")
 
         file_new = file_menu.addAction("&New")
@@ -197,15 +200,24 @@
         cursor.setPosition(0)
         self.code_view.setTextCursor(cursor)
 
     def invalidate_text(self) -> None:
         self.parsed = False
         self.graph_cache = dict()
         self.code_view.set_current_region(None)
-        self.update_state(quiet=True)
+        self.revision += 1
+
+        def update(r: int) -> Callable:
+            def f():
+                if r == self.revision:
+                    self.update_state()
+            return f
+
+        QTimer.singleShot(100, update(self.revision))
+        # self.update_state(sync=False)
 
     def next_part(self, step:int=1) -> None:
         if not self.parsed: return
 
         cursor = self.code_view.textCursor()
         pos = cursor.position()
         p = self.state.part_with_index_at(pos)
@@ -350,31 +362,30 @@
             rule = self.state.rewrites[part[3]].rule
 
             if rule:
                 self.code_view.add_line_below('  = ? by ' + rule.name)
                 self.update_state()
                 self.next_rewrite_at_cursor()
 
-    def update_state(self, quiet: bool=False) -> None:
+    def update_state(self) -> None:
+        self.state = State()
         self.code_view.set_current_region(None)
-        self.state.update(self.code_view.toPlainText())
         
+        self.state.update(self.code_view.toPlainText())
         model = self.error_view.model()
         if isinstance(model, ErrorListModel):
             model.set_errors(self.state.errors)
 
         if len(self.state.errors) == 0:
             self.lhs_view.set_graph(Graph())
             self.rhs_view.setVisible(False)
             self.parsed = True
             self.show_at_cursor()
-        elif not quiet:
-            print('**********************************************************************')
-            for err in self.state.errors:
-                print("%d: %s" % err)
+
+
 
     def closeEvent(self, e: QCloseEvent) -> None:
         if self.doc.confirm_close():
             conf = QSettings('chyp', 'chyp')
             conf.setValue("editor_window_geometry", self.saveGeometry())
             conf.setValue("editor_splitter_state", self.splitter.saveState())
             sizes = self.splitter.sizes()
@@ -387,7 +398,17 @@
 class CheckThread(QThread):
     def __init__(self, rw: RewriteState, parent: Optional[QObject] = None) -> None:
         super().__init__(parent)
         self.rw = rw
 
     def run(self) -> None:
         self.rw.check()
+
+# class UpdateStateThread(QThread):
+#     def __init__(self, state: State, code: str, parent: Optional[QObject] = None) -> None:
+#         super().__init__(parent)
+#         self.state = state
+#         self.code = code
+
+#     def run(self) -> None:
+#         self.msleep(300)
+#         self.state.update(self.code)
```

### Comparing `chyp-0.3.2/chyp/gui/errorlist.py` & `chyp-0.3.3/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/graphscene.py` & `chyp-0.3.3/chyp/gui/graphscene.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/graphview.py` & `chyp-0.3.3/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/highlighter.py` & `chyp-0.3.3/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/gui/mainwindow.py` & `chyp-0.3.3/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/layout.py` & `chyp-0.3.3/chyp/layout.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/matcher.py` & `chyp-0.3.3/chyp/matcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,14 +237,17 @@
     def is_surjective(self) -> bool:
         return len(self.vimg) == self.cod.num_vertices() and len(self.eimg) == self.cod.num_edges()
 
     def is_injective(self) -> bool:
         return len(self.vmap) == len(self.vimg)
 
     def is_convex(self) -> bool:
+        if not self.is_injective():
+            return False
+
         future = self.cod.successors([self.vmap[v] for v in self.dom.outputs() if v in self.vmap])
         for v in self.dom.inputs():
             if v in self.vmap and self.vmap[v] in future:
                 return False
         return True
```

### Comparing `chyp-0.3.2/chyp/parser.py` & `chyp-0.3.3/chyp/parser.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/rewrite.py` & `chyp-0.3.3/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/rule.py` & `chyp-0.3.3/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/scraps.py` & `chyp-0.3.3/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/state.py` & `chyp-0.3.3/chyp/state.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp/term.py` & `chyp-0.3.3/chyp/term.py`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/chyp.egg-info/PKG-INFO` & `chyp-0.3.3/chyp.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.3.2
+Version: 0.3.3
 Summary: An interactive theorem prover for monoidal categories
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -14,15 +14,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 Chyp (pronounced "chip") is an interactive theorem prover for symmetric monoidal categories (SMCs), a.k.a. process theories. Symmetric monoidal categories are a very general way to reason about processes that can be composed in sequence or in parallel. String diagrams are a convenient notation for maps in an SMC, where processes are represented as boxes connected to each other by wires.
 
 ![Chyp screenshot](https://github.com/akissinger/chyp/raw/master/chyp-screen.png)
 
-Chyp is short for _Composing HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching to a combinatoric structure based on hypergraphs, we obtain a convenient rewrite theory for string diagrams. There is a lot of theory behind this, which has been developed over a series of papers:
+Chyp is short for _Cospans of HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching from terms to this combinatoric structure, we obtain a convenient rewrite theory for string diagrams that automatically handles the extra "bureaucracy" that comes from working with sequential and parallel composition together. There is a lot of theory behind this, which has been developed over a series of papers:
 
 * [String Diagram Rewrite Theory I: Rewriting with Frobenius Structure](https://arxiv.org/abs/2012.01847)
 * [String Diagram Rewrite Theory II: Rewriting with Symmetric Monoidal Structure](https://arxiv.org/abs/2104.14686)
 * [String diagram rewrite theory III: Confluence with and without Frobenius](https://discovery.ucl.ac.uk/id/eprint/10151067/1/string-diagram-rewrite-theory-iii-confluence-with-and-without-frobenius.pdf)
 
 Currently, Chyp implements the theory described in part II, using monogamous acyclic hypergraphs to represent morphisms in a symmetric monoidal category. Fancier types of rewriting (e.g. rewriting modulo Frobenius structure) is planned for the future.
 
@@ -86,14 +86,15 @@
 Note these indices are local to the swap map, so splitting or combining swap maps will change some indices in general. For example:
 
     sw[1, 2, 0] * sw[1, 0] = sw[1, 2, 0, 4, 3]
 
 
 ## Rules and rewriting
 
+
 An algebraic theory can be presented by introducing some generators as well as some rewrite rules. Rules are defined via the `rule` statement, which gives the rule a name, then takes as input a pair of terms with the same number of inputs and outputs. For example, we could introduce a pair of rules relating the `f` and `g` generators as follows:
 
     rule assoc : f * id ; f = id * f ; f
     rule bialg : f ; g = g * g ; id * sw * id ; f * f
 
 Now for the good part! The `rewrite` statement represents a transitive chain of rule applications. It consists of the keyword `rewrite` followed by a name to use for the resulting theorem, then a sequence of equalities, each giving a justifying rule. For example:
```

### Comparing `chyp-0.3.2/chyp.egg-info/SOURCES.txt` & `chyp-0.3.3/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.3.2/setup.py` & `chyp-0.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.3.2",
+    version="0.3.3",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for monoidal categories",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

