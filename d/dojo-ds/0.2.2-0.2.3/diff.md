# Comparing `tmp/dojo_ds-0.2.2.tar.gz` & `tmp/dojo_ds-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dojo_ds-0.2.2.tar", last modified: Fri May 12 17:31:49 2023, max compression
+gzip compressed data, was "dojo_ds-0.2.3.tar", last modified: Mon May 15 20:57:48 2023, max compression
```

## Comparing `dojo_ds-0.2.2.tar` & `dojo_ds-0.2.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 17:31:49.452589 dojo_ds-0.2.2/
--rw-r--r--   0 codingdojo   (502) staff       (20)      160 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/AUTHORS.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/CONTRIBUTING.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/HISTORY.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-0.2.2/LICENSE
--rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/MANIFEST.in
--rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-12 17:31:49.452672 dojo_ds-0.2.2/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      903 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/README.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 17:31:49.442763 dojo_ds-0.2.2/docs/
--rw-r--r--   0 codingdojo   (502) staff       (20)      608 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/Makefile
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/authors.rst
--rwxr-xr-x   0 codingdojo   (502) staff       (20)     4778 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/conf.py
--rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/contributing.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/history.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      304 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/index.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)     1122 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/installation.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/make.bat
--rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/readme.rst
--rw-r--r--   0 codingdojo   (502) staff       (20)       69 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/docs/usage.rst
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 17:31:49.448099 dojo_ds-0.2.2/dojo_ds/
--rw-r--r--   0 codingdojo   (502) staff       (20)      249 2023-05-12 17:31:37.000000 dojo_ds-0.2.2/dojo_ds/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      399 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/dojo_ds/cli.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     4746 2023-02-15 01:18:18.000000 dojo_ds-0.2.2/dojo_ds/data_enrichment.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    25287 2023-02-15 01:38:29.000000 dojo_ds-0.2.2/dojo_ds/dojo_ds.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    10108 2023-05-12 17:31:25.000000 dojo_ds-0.2.2/dojo_ds/eda.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      293 2023-02-15 01:23:40.000000 dojo_ds-0.2.2/dojo_ds/lp_style.py
--rw-r--r--   0 codingdojo   (502) staff       (20)    26552 2023-05-12 16:29:09.000000 dojo_ds-0.2.2/dojo_ds/model_insights.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      245 2023-02-15 01:20:53.000000 dojo_ds-0.2.2/dojo_ds/standard_imports.py
--rw-r--r--   0 codingdojo   (502) staff       (20)     8839 2023-02-15 01:26:36.000000 dojo_ds-0.2.2/dojo_ds/utils.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 17:31:49.451813 dojo_ds-0.2.2/dojo_ds.egg-info/
--rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/PKG-INFO
--rw-r--r--   0 codingdojo   (502) staff       (20)      700 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/SOURCES.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/dependency_links.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)       45 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/entry_points.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-0.2.2/dojo_ds.egg-info/not-zip-safe
--rw-r--r--   0 codingdojo   (502) staff       (20)       79 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/requires.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)        8 2023-05-12 17:31:49.000000 dojo_ds-0.2.2/dojo_ds.egg-info/top_level.txt
--rw-r--r--   0 codingdojo   (502) staff       (20)      379 2023-05-12 17:31:49.453022 dojo_ds-0.2.2/setup.cfg
--rw-r--r--   0 codingdojo   (502) staff       (20)     1687 2023-05-12 17:31:37.000000 dojo_ds-0.2.2/setup.py
-drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-12 17:31:49.452391 dojo_ds-0.2.2/tests/
--rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/tests/__init__.py
--rw-r--r--   0 codingdojo   (502) staff       (20)      852 2023-02-15 01:14:18.000000 dojo_ds-0.2.2/tests/test_dojo_ds.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-15 20:57:48.492596 dojo_ds-0.2.3/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      160 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/AUTHORS.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     3530 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/CONTRIBUTING.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       89 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/HISTORY.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)    35129 2023-02-15 01:14:37.000000 dojo_ds-0.2.3/LICENSE
+-rw-r--r--   0 codingdojo   (502) staff       (20)      262 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/MANIFEST.in
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-15 20:57:48.492681 dojo_ds-0.2.3/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      903 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/README.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-15 20:57:48.477076 dojo_ds-0.2.3/docs/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      608 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/Makefile
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/authors.rst
+-rwxr-xr-x   0 codingdojo   (502) staff       (20)     5506 2023-05-15 16:08:44.000000 dojo_ds-0.2.3/docs/conf.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)       33 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/contributing.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       28 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/history.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      304 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/index.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1122 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/installation.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)      805 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/make.bat
+-rw-r--r--   0 codingdojo   (502) staff       (20)       27 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/readme.rst
+-rw-r--r--   0 codingdojo   (502) staff       (20)       69 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/docs/usage.rst
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-15 20:57:48.486745 dojo_ds-0.2.3/dojo_ds/
+-rw-r--r--   0 codingdojo   (502) staff       (20)      249 2023-05-15 20:57:28.000000 dojo_ds-0.2.3/dojo_ds/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      399 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/dojo_ds/cli.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     4746 2023-02-15 01:18:18.000000 dojo_ds-0.2.3/dojo_ds/data_enrichment.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    25287 2023-02-15 01:38:29.000000 dojo_ds-0.2.3/dojo_ds/dojo_ds.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    10153 2023-05-15 20:56:17.000000 dojo_ds-0.2.3/dojo_ds/eda.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      293 2023-02-15 01:23:40.000000 dojo_ds-0.2.3/dojo_ds/lp_style.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)    26552 2023-05-12 16:29:09.000000 dojo_ds-0.2.3/dojo_ds/model_insights.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      245 2023-02-15 01:20:53.000000 dojo_ds-0.2.3/dojo_ds/standard_imports.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)     8839 2023-02-15 01:26:36.000000 dojo_ds-0.2.3/dojo_ds/utils.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-15 20:57:48.490838 dojo_ds-0.2.3/dojo_ds.egg-info/
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1761 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/PKG-INFO
+-rw-r--r--   0 codingdojo   (502) staff       (20)      700 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/SOURCES.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/dependency_links.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)       45 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/entry_points.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        1 2023-02-15 01:30:10.000000 dojo_ds-0.2.3/dojo_ds.egg-info/not-zip-safe
+-rw-r--r--   0 codingdojo   (502) staff       (20)       79 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/requires.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)        8 2023-05-15 20:57:48.000000 dojo_ds-0.2.3/dojo_ds.egg-info/top_level.txt
+-rw-r--r--   0 codingdojo   (502) staff       (20)      379 2023-05-15 20:57:48.493656 dojo_ds-0.2.3/setup.cfg
+-rw-r--r--   0 codingdojo   (502) staff       (20)     1687 2023-05-15 20:57:28.000000 dojo_ds-0.2.3/setup.py
+drwxr-xr-x   0 codingdojo   (502) staff       (20)        0 2023-05-15 20:57:48.491962 dojo_ds-0.2.3/tests/
+-rw-r--r--   0 codingdojo   (502) staff       (20)       37 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/tests/__init__.py
+-rw-r--r--   0 codingdojo   (502) staff       (20)      852 2023-02-15 01:14:18.000000 dojo_ds-0.2.3/tests/test_dojo_ds.py
```

### Comparing `dojo_ds-0.2.2/CONTRIBUTING.rst` & `dojo_ds-0.2.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/LICENSE` & `dojo_ds-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/PKG-INFO` & `dojo_ds-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo_ds
-Version: 0.2.2
+Version: 0.2.3
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/jirvingphd/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-0.2.2/README.rst` & `dojo_ds-0.2.3/README.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/docs/Makefile` & `dojo_ds-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/docs/conf.py` & `dojo_ds-0.2.3/docs/conf.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,25 @@
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.viewcode',
+              'sphinx.ext.apidoc','sphinx.ext.napoleon']
 
+## Napoleon Docstring settings
+napoleon_numpy_docstring = True
+napoleon_google_docstring = True
+napoleon_include_private_with_doc = False
+napoleon_include_init_with_doc = True
+
+# From bs_ds's line 74
+add_module_name = False
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
@@ -154,9 +163,23 @@
      'dojo-ds Documentation',
      author,
      'dojo_ds',
      'One line description of project.',
      'Miscellaneous'),
 ]
 
+### FROM bs_ds's conf.py line 169
+def run_apidoc(_):
+    #https://www.sphinx-doc.org/en/master/man/sphinx-apidoc.html
+	from sphinx.ext.apidoc import main
+	import os
+	import sys
+	sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
+	cur_dir = os.path.abspath(os.path.dirname(__file__))
+	module = os.path.join(cur_dir,"..","bs_ds")
+	main(['-o', cur_dir, module,'-M','--force'])
+
+def setup(app):
+	app.connect('builder-inited', run_apidoc)
+
```

### Comparing `dojo_ds-0.2.2/docs/installation.rst` & `dojo_ds-0.2.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/docs/make.bat` & `dojo_ds-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/dojo_ds/data_enrichment.py` & `dojo_ds-0.2.3/dojo_ds/data_enrichment.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/dojo_ds/dojo_ds.py` & `dojo_ds-0.2.3/dojo_ds/dojo_ds.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/dojo_ds/eda.py` & `dojo_ds-0.2.3/dojo_ds/eda.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,22 +262,22 @@
 	fig, ax = plt.subplots(figsize=figsize)
 	scatter_kws={'ec':'white','lw':1,'alpha':0.8}
 	sns.regplot(data=df, x=x, y=y, ax=ax, scatter_kws=scatter_kws)
 
 	## Add the title with the correlation
 	ax.set_title(f"{x} vs. {y} (r = {r})", fontweight='bold')
 
+	# Make sure the plot is shown before the print statement
+	plt.show()
+
 	## Print message with info on the count and % of null values
 	null_count = df[x].isna().sum()
-	if null_count > 0:
-		null_perc = null_count/len(df)* 100
+	null_perc = null_count/len(df)* 100
 	print(f"- NaN's Found: {null_count} ({round(null_perc,2)}%)")
-	
-	
-	
+
 	return fig, ax
 
 
 
 
 def annotate_regplot_equation(ax):
   """Adapted from Source: https://www.statology.org/seaborn-regplot-equation/
```

### Comparing `dojo_ds-0.2.2/dojo_ds/model_insights.py` & `dojo_ds-0.2.3/dojo_ds/model_insights.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/dojo_ds/utils.py` & `dojo_ds-0.2.3/dojo_ds/utils.py`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/dojo_ds.egg-info/PKG-INFO` & `dojo_ds-0.2.3/dojo_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dojo-ds
-Version: 0.2.2
+Version: 0.2.3
 Summary: Code from Coding Dojo's Online Part-Time Data Science boot camp
 Home-page: https://github.com/jirvingphd/dojo_ds
 Author: James Irving
 Author-email: jirving@codingdojo.com
 License: GNU General Public License v3
 Keywords: dojo_ds
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `dojo_ds-0.2.2/dojo_ds.egg-info/SOURCES.txt` & `dojo_ds-0.2.3/dojo_ds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dojo_ds-0.2.2/setup.py` & `dojo_ds-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,10 +45,10 @@
     include_package_data=True,
     keywords='dojo_ds',
     name='dojo_ds',
     packages=find_packages(include=['dojo_ds', 'dojo_ds.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/jirvingphd/dojo_ds',
-    version='0.2.2',
+    version='0.2.3',
     zip_safe=False,
 )
```

### Comparing `dojo_ds-0.2.2/tests/test_dojo_ds.py` & `dojo_ds-0.2.3/tests/test_dojo_ds.py`

 * *Files identical despite different names*

