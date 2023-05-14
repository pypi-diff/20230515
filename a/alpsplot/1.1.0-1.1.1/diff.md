# Comparing `tmp/alpsplot-1.1.0.tar.gz` & `tmp/alpsplot-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpsplot-1.1.0.tar", last modified: Mon Jan  9 08:49:33 2023, max compression
+gzip compressed data, was "alpsplot-1.1.1.tar", last modified: Sun May 14 21:58:02 2023, max compression
```

## Comparing `alpsplot-1.1.0.tar` & `alpsplot-1.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.305736 alpsplot-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-09 08:48:56.000000 alpsplot-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-09 08:49:33.305736 alpsplot-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-01-09 08:48:56.000000 alpsplot-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.301736 alpsplot-1.1.0/alpsplot/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/alpsplot.mplstyle
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    40052 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/figure.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.301736 alpsplot-1.1.0/alpsplot/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/error_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.305736 alpsplot-1.1.0/alpsplot/utils/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56192 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Optima-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56400 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Optima-ExtraBlack.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    55012 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    53012 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Regular.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   304308 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Bold.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   540924 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-BoldItalic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   548104 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Italic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   514524 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Roman.ttf
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/utils/fonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-09 08:48:56.000000 alpsplot-1.1.0/alpsplot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.301736 alpsplot-1.1.0/alpsplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-01-09 08:49:33.000000 alpsplot-1.1.0/alpsplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-01-09 08:49:33.000000 alpsplot-1.1.0/alpsplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 08:49:33.000000 alpsplot-1.1.0/alpsplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-09 08:49:32.000000 alpsplot-1.1.0/alpsplot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-01-09 08:49:33.000000 alpsplot-1.1.0/alpsplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-09 08:49:33.000000 alpsplot-1.1.0/alpsplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-01-09 08:48:56.000000 alpsplot-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-01-09 08:49:33.309737 alpsplot-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-01-09 08:48:56.000000 alpsplot-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-09 08:49:33.305736 alpsplot-1.1.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-01-09 08:48:56.000000 alpsplot-1.1.0/test/test_figure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.049882 alpsplot-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-14 21:57:27.000000 alpsplot-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-14 21:58:02.049882 alpsplot-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-05-14 21:57:27.000000 alpsplot-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.041882 alpsplot-1.1.1/alpsplot/
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/alpsplot.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40255 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/figure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.045882 alpsplot-1.1.1/alpsplot/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4749 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/error_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12315 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.049882 alpsplot-1.1.1/alpsplot/utils/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    52936 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56192 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Optima-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56400 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Optima-ExtraBlack.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    55012 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    53012 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   304308 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Bold.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   540924 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-BoldItalic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   548104 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Italic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   514524 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Roman.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/utils/fonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-14 21:57:27.000000 alpsplot-1.1.1/alpsplot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.045882 alpsplot-1.1.1/alpsplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-14 21:58:02.000000 alpsplot-1.1.1/alpsplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-14 21:58:02.000000 alpsplot-1.1.1/alpsplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:58:02.000000 alpsplot-1.1.1/alpsplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 21:58:01.000000 alpsplot-1.1.1/alpsplot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 21:58:02.000000 alpsplot-1.1.1/alpsplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-14 21:58:02.000000 alpsplot-1.1.1/alpsplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 21:57:27.000000 alpsplot-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-14 21:58:02.049882 alpsplot-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-14 21:57:27.000000 alpsplot-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 21:58:02.049882 alpsplot-1.1.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-14 21:57:27.000000 alpsplot-1.1.1/test/test_figure.py
```

### Comparing `alpsplot-1.1.0/LICENSE` & `alpsplot-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/PKG-INFO` & `alpsplot-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpsplot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python plotting library of alps-lab style using matplotlib.
 Home-page: https://github.com/ain-soph/alpsplot
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: plot,python,matplotlib
 Platform: any
```

### Comparing `alpsplot-1.1.0/README.md` & `alpsplot-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/colormap.py` & `alpsplot-1.1.1/alpsplot/colormap.py`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/figure.py` & `alpsplot-1.1.1/alpsplot/figure.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         self.ax.grid(axis='y', linewidth=1, alpha=0.5)
         self.ax.set_axisbelow(True)
 
     def save(self, path: str = None,
              folder_path: str = None, filename: str = None,
              name: str = None, ext: str = '.pdf',
              dpi: int = 100, bbox_inches: str = 'tight',
-             **kwargs):
+             pad_inches: float = 0.0, **kwargs):
         r"""Class methods are similar to regular functions.
 
         Args:
             path (str, optional): The file path to save the figure.
                 Defaults to ``f'{folder_path}/{filename}'``.
             folder_path (str, optional): Called when :attr:`path` is ``None``.
                 Defaults to :attr:`~self.folder_path`.
@@ -217,14 +217,17 @@
                 Defaults to ``'.pdf'``.
             dpi (int): Passed to
                 :any:`Figure.savefig() <matplotlib.figure.Figure.savefig>`.
                 Defaults to ``100``.
             bbox_inches (str): Passed to
                 :any:`Figure.savefig() <matplotlib.figure.Figure.savefig>`.
                 Defaults to ``'tight'``.
+            pad_inches (float): Passed to
+                :any:`Figure.savefig() <matplotlib.figure.Figure.savefig>`.
+                Defaults to ``0.0``.
             **kwargs: Keyword arguments passed to
                 :any:`Figure.savefig() <matplotlib.figure.Figure.savefig>`.
 
         :Example:
             .. code-block:: python
                 :emphasize-lines: 17
 
@@ -256,15 +259,15 @@
                 ext = ext if ext.startswith('.') else '.' + ext
                 filename = f'{name}{ext}'
             path = os.path.join(folder_path, filename)
         else:
             folder_path = os.path.dirname(path)
         if not os.path.exists(folder_path):
             os.makedirs(folder_path)
-        self.fig.savefig(path, dpi=dpi, bbox_inches=bbox_inches, **kwargs)
+        self.fig.savefig(path, dpi=dpi, bbox_inches=bbox_inches, pad_inches=pad_inches, **kwargs)
 
     def set_title(self, text: str = None, **kwargs):
         r"""Call :any:`Axes.set_title() <matplotlib.axes.Axes.set_title>`.
 
         Args:
             text (str, optional): The text of title.
                 Defaults to :attr:`self.name`.
```

### Comparing `alpsplot-1.1.0/alpsplot/utils/basic.py` & `alpsplot-1.1.1/alpsplot/utils/basic.py`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/error_bar.py` & `alpsplot-1.1.1/alpsplot/utils/error_bar.py`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fit.py` & `alpsplot-1.1.1/alpsplot/utils/fit.py`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Bold.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Bold.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Optima-BoldItalic.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Optima-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Optima-ExtraBlack.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Optima-ExtraBlack.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Italic.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Italic.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Optima-Regular.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Optima-Regular.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Bold.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Bold.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-BoldItalic.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-BoldItalic.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Italic.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Italic.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/Palatino-Roman.ttf` & `alpsplot-1.1.1/alpsplot/utils/fonts/Palatino-Roman.ttf`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot/utils/fonts/__init__.py` & `alpsplot-1.1.1/alpsplot/utils/fonts/__init__.py`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/alpsplot.egg-info/PKG-INFO` & `alpsplot-1.1.1/alpsplot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpsplot
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python plotting library of alps-lab style using matplotlib.
 Home-page: https://github.com/ain-soph/alpsplot
 Author: Ren Pang
 Author-email: rbp5354@psu.edu
 License: GPL-3
 Keywords: plot,python,matplotlib
 Platform: any
```

### Comparing `alpsplot-1.1.0/alpsplot.egg-info/SOURCES.txt` & `alpsplot-1.1.1/alpsplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/setup.cfg` & `alpsplot-1.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `alpsplot-1.1.0/test/test_figure.py` & `alpsplot-1.1.1/test/test_figure.py`

 * *Files identical despite different names*

