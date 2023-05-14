# Comparing `tmp/mdforest-0.2.0.tar.gz` & `tmp/mdforest-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-0.2.0.tar", last modified: Sat May 13 16:28:55 2023, max compression
+gzip compressed data, was "mdforest-1.0.0.tar", last modified: Sun May 14 22:57:56 2023, max compression
```

## Comparing `mdforest-0.2.0.tar` & `mdforest-1.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-13 16:28:55.803940 mdforest-0.2.0/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-0.2.0/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      403 2023-05-13 16:28:55.803940 mdforest-0.2.0/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2191 2023-05-13 16:15:30.000000 mdforest-0.2.0/README.md
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-13 16:28:55.802940 mdforest-0.2.0/markdown_tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      429 2023-05-13 15:36:02.000000 mdforest-0.2.0/markdown_tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1726 2023-05-13 15:38:34.000000 mdforest-0.2.0/markdown_tree/markdown_tree.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6426 2023-05-13 15:14:14.000000 mdforest-0.2.0/markdown_tree/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-13 16:28:55.803940 mdforest-0.2.0/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      403 2023-05-13 16:28:55.000000 mdforest-0.2.0/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      305 2023-05-13 16:28:55.000000 mdforest-0.2.0/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-13 16:28:55.000000 mdforest-0.2.0/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       24 2023-05-13 16:28:55.000000 mdforest-0.2.0/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       14 2023-05-13 16:28:55.000000 mdforest-0.2.0/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-0.2.0/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-13 16:28:55.803940 mdforest-0.2.0/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1234 2023-05-13 16:28:42.000000 mdforest-0.2.0/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-13 16:28:55.803940 mdforest-0.2.0/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      841 2023-05-13 16:01:15.000000 mdforest-0.2.0/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.531424 mdforest-1.0.0/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.0.0/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      413 2023-05-14 22:57:56.531424 mdforest-1.0.0/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2457 2023-05-14 20:42:59.000000 mdforest-1.0.0/README.md
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.529424 mdforest-1.0.0/markdown_tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      430 2023-05-14 20:59:45.000000 mdforest-1.0.0/markdown_tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2444 2023-05-14 21:19:06.000000 mdforest-1.0.0/markdown_tree/markdown_tree.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-14 20:59:45.000000 mdforest-1.0.0/markdown_tree/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.530424 mdforest-1.0.0/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      413 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      305 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       24 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       14 2023-05-14 22:57:56.000000 mdforest-1.0.0/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.0.0/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-14 22:57:56.531424 mdforest-1.0.0/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1244 2023-05-14 20:45:08.000000 mdforest-1.0.0/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-14 22:57:56.530424 mdforest-1.0.0/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1201 2023-05-14 21:06:28.000000 mdforest-1.0.0/tests/test_mdtree.py
```

### Comparing `mdforest-0.2.0/LICENSE` & `mdforest-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-0.2.0/README.md` & `mdforest-1.0.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-# Markdown Tree
+![icon](media/forest-icon-display.png)
 
-A library to convert Markdown documents into tree data structures and vice versa. There is greater functionality available to modify, prune, add and delete parts of documents when there are in the MarkdownTree structure. 
+# mdforest - Markdown Forest
+
+A library to convert Markdown documents into tree data structures and vice versa. There is greater functionality available to modify, prune, add and delete parts of documents when there are in the MarkdownTree structure.
 
 markdown-tree is a fork of [md2py](https://github.com/alvinwan/md2py) which is no longer maintained. This library adds far more functionality and broadens the scope of the older libary. The full list of features can be found under [Features](## Features)
 
 ## Install
 
 Install via pip
 
@@ -23,24 +25,27 @@
 Take, for example, the following markdown file.
 
 [[ chikin.md ]]
 
 ```markdown
 # Chikin Tales
 
+Once there was a chikin.
+
 ## Chapter 1 : Chikin Fly
 
 Chickens don't fly. They do only the following:
 
 - waddle
-- plop
+- plop 
+
 
 ### Waddling
 
-A waddle is what these birds do. 
+A waddle is what these birds do.
 
 ## Chapter 2 : Chikin Scream
 
 ### Plopping
 
 Plopping involves three steps:
 
@@ -51,23 +56,29 @@
 ```
 
 Akin to a navigation bar, the `TreeOfContents` object allows you to expand a
 markdown file one level at a time. Running `md2py` on the above markdown file
 will generate a tree, abstracting the below structure.
 
 ```text
-          Chikin Tales
-          /           \
-    Chapter 1       Chapter 2
-      /                 |
-  Waddling            Plopping
-     |                  |
-     |                  |        
-  A waddle...           |          
-                    Plopping inv...
+               Chikin Tales
+              /     \       \
+             /       \       \ 
+       (Once th..)    |       \
+                      |        \
+                  Chapter 1     \
+                  /     |     Chapter 2   
+                 /      |         |
+       (Chickens do..)  |       Plopping
+                        |         |
+                     Waddling   (Plopping...)
+                        |
+                    (A waddle...)
+
+
 ```
 
 For the full usage guide, access the SAMPLES.md file.
 
 ## Features
 
 Some of the features of this library are:
```

### Comparing `mdforest-0.2.0/markdown_tree/markdown_tree.py` & `mdforest-1.0.0/markdown_tree/markdown_tree.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .treebuild import TreeOfContents
+from .treebuild import __TreeOfContents
 from .tree.types import *
 
-def generateRootNodeFromContents(currTree:TreeOfContents, parent:Node=None) -> Node:
+def generateRootNodeFromContents(currTree:__TreeOfContents, parent:Node=None) -> Node:
     """ Function to generate the tree of a specfic header's section.
     """    
     # BASE CASE: If there is no depth, then it is just a paragraph
     if currTree.depth == None:
         return TextNode(currTree.source.string, parent=parent)
     
     # Get the current header of the tree
@@ -23,37 +23,63 @@
 
 def mdtreeify(md:str, *args, **kwargs) -> MarkdownForest:
     """
     Converts markdown file to a MarkdownForest
     """
 
     returnForest = MarkdownForest("test2")
-    toc =  TreeOfContents.fromMarkdown(md, *args, **kwargs)
+    toc =  __TreeOfContents.fromMarkdown(md, *args, **kwargs)
     for tree in toc.branches:
         root = generateRootNodeFromContents(tree)
         returnForest.add_tree(MarkdownTree(root))
         
     return returnForest
     
-def mdtextify(tree:MarkdownForest, *args, **kwargs) -> str:
-    pass
+def convertRootToText(rootNode: Node) -> str:
+    
+    # BASE CASE: We just have text node.
+    if isinstance(rootNode, TextNode):
+        return repr(rootNode) + "\n"
+    
+    headerLevel = rootNode.get_header_level()
+    returnString = '#'*headerLevel + " " + str(rootNode) + "\n"
+    for i, child in enumerate(rootNode):
+        returnString += convertRootToText(child)
+    
+    return returnString    
+        
+
+def mdtextify(forest:MarkdownForest, *args, **kwargs) -> str:
+    
+    finalText = ""
+    for i, tree in enumerate(forest):
+        finalText += convertRootToText(tree.get_root())
+    return finalText
         
 # test = """# Header 1
 # ## Header 2.1
 # Some text here and there
 # ### Header 3
 # Some more text here and there
 # ## Header 2.2
 # Thats' all folks!
 # """
 
 # test2 = """
-# # asdasd
-# ok then
-# ## 1238123
+# # Header 1
+# ## Header 2.1
+# Some text here and there
+# ### Header 3
+# Some more text here and there
+# ## Header 2.2
+# Thats' all folks!
 # """
 
-# a = mdtreeify(test)
+# a = mdtreeify(test2)
+# print(a)
+# ret_test2 = mdtextify(a)
+
+# print(ret_test2)
 
 # print(a)
 # a[0].root.add_child(TextNode("asdasd", parent=a[0].root))
 # print(a)
```

### Comparing `mdforest-0.2.0/markdown_tree/treebuild.py` & `mdforest-1.0.0/markdown_tree/treebuild.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from markdown import markdown
 from bs4 import BeautifulSoup
 import re
 
-class TreeOfContents:
+class __TreeOfContents:
     """Tree abstraction for markdown source"""
 
     source_type = BeautifulSoup
     valid_tags = ('a', 'abbr', 'address', 'area', 'article', 'aside', 'audio',
         'b', 'base', 'bdi', 'bdo', 'blockquote', 'body', 'br', 'button',
         'canvas', 'caption', 'cite', 'code', 'col', 'colgroup', 'data',
         'datalist', 'dd', 'del', 'details', 'dfn', 'dialog', 'div', 'dl', 'dt',
@@ -114,19 +114,20 @@
         return self.branches[i]
 
     @staticmethod
     def fromMarkdown(md, *args, **kwargs):
         """
         Creates abstraction using path to file
         """
-        
-        
+                
         def clean_headers(markdown_text):
-            """ Remove bold and italics formatting from headers
+            """ 
+            Remove bold and italics formatting from headers
             """
+            
             # Regular expressions to match bold and italics formatting
             bold_pattern = re.compile(r'\*\*(.*?)\*\*')
             alt_bold_pattern = re.compile(r'__(.*?)__')
             italics_pattern = re.compile(r'\*(.*?)\*')
             alt_italics_pattern = re.compile(r'_(.*?)_')
 
             # Split the Markdown text into lines
@@ -150,21 +151,14 @@
                     lines[i] = line
 
             # Join the modified lines back into a single string
             modified_text = '\n'.join(lines)
             return modified_text
     
         md = clean_headers(md)
-        return TOC.fromHTML(markdown(md, *args, **kwargs))
-
-    @staticmethod
-    def fromHTML(html, *args, **kwargs):
-        """
-        Creates abstraction using HTML
-        """
-        
-        source = BeautifulSoup(html, 'html.parser', *args, **kwargs)
+        html_convert = markdown(md, *args, **kwargs)
+        source = BeautifulSoup(html_convert, 'html.parser', *args, **kwargs)
         return TOC('[document]',
                     source=source,
                     descendants=source.children)
 
-TOC = TreeOfContents
+TOC = __TreeOfContents
```

### Comparing `mdforest-0.2.0/setup.py` & `mdforest-1.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 
     def run_tests(self):
         # import here, cause outside the eggs aren't loaded
         import pytest
         errno = pytest.main(self.pytest_args)
         sys.exit(errno)
 
-VERSION = '0.2.0'
-DESCRIPTION = 'A package to convert between Markdown and a forest data structure for processing.'
+VERSION = '1.0.0'
+DESCRIPTION = 'A package to convert between Markdown and a forest data structure for effecient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
     description = DESCRIPTION,
```

