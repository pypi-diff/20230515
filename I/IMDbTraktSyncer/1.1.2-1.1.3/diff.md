# Comparing `tmp/IMDbTraktSyncer-1.1.2.tar.gz` & `tmp/IMDbTraktSyncer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IMDbTraktSyncer-1.1.2.tar", last modified: Sun May 14 21:24:30 2023, max compression
+gzip compressed data, was "IMDbTraktSyncer-1.1.3.tar", last modified: Mon May 15 08:57:01 2023, max compression
```

## Comparing `IMDbTraktSyncer-1.1.2.tar` & `IMDbTraktSyncer-1.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.065591 IMDbTraktSyncer-1.1.2/
-drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.030559 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/
--rw-rw-rw-   0        0        0    10477 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/IMDbTraktSyncer.py
--rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/__init__.py
--rw-rw-rw-   0        0        0     1805 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/authTrakt.py
--rw-rw-rw-   0        0        0     3511 2023-05-14 21:13:51.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/checkChromedriver.py
--rw-rw-rw-   0        0        0     2060 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/imdbRatings.py
--rw-rw-rw-   0        0        0     1408 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/traktRatings.py
--rw-rw-rw-   0        0        0     2516 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/verifyCredentials.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:24:30.062595 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/
--rw-rw-rw-   0        0        0     6624 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      491 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       29 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-14 21:24:29.000000 IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.2/LICENSE
--rw-rw-rw-   0        0        0     6624 2023-05-14 21:24:30.064592 IMDbTraktSyncer-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6004 2023-05-14 21:23:43.000000 IMDbTraktSyncer-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 21:24:30.065591 IMDbTraktSyncer-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1287 2023-05-14 21:23:18.000000 IMDbTraktSyncer-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.719166 IMDbTraktSyncer-1.1.3/
+drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.684212 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/
+-rw-rw-rw-   0        0        0    10477 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/IMDbTraktSyncer.py
+-rw-rw-rw-   0        0        0        0 2023-04-29 22:05:24.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/__init__.py
+-rw-rw-rw-   0        0        0     1805 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/authTrakt.py
+-rw-rw-rw-   0        0        0     4079 2023-05-15 08:55:47.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/checkChromedriver.py
+-rw-rw-rw-   0        0        0     2060 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/imdbRatings.py
+-rw-rw-rw-   0        0        0     1408 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/traktRatings.py
+-rw-rw-rw-   0        0        0     2516 2023-05-14 16:27:09.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/verifyCredentials.py
+drwxrwxrwx   0        0        0        0 2023-05-15 08:57:01.716669 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/
+-rw-rw-rw-   0        0        0     6624 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      491 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-15 08:57:01.000000 IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1079 2023-04-26 18:19:27.000000 IMDbTraktSyncer-1.1.3/LICENSE
+-rw-rw-rw-   0        0        0     6624 2023-05-15 08:57:01.718667 IMDbTraktSyncer-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6004 2023-05-15 08:56:12.000000 IMDbTraktSyncer-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 08:57:01.719674 IMDbTraktSyncer-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1287 2023-05-15 08:56:35.000000 IMDbTraktSyncer-1.1.3/setup.py
```

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/IMDbTraktSyncer.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/IMDbTraktSyncer.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/authTrakt.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/authTrakt.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/checkChromedriver.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/checkChromedriver.py`

 * *Files 20% similar despite different names*

```diff
@@ -37,14 +37,23 @@
 
     return None
 
 def install_chromedriver(version):
     # Install the chromedriver-py package using pip
     subprocess.run(['pip', 'install', f'chromedriver-py=={version}'])
 
+def install_chromedriver_fallback_method():
+    print("Using install chromedriver-py fallback method")
+    # Install the chromedriver-py package using pip
+    feed = feedparser.parse('https://pypi.org/rss/project/chromedriver-py/releases.xml')
+    # Get the second latest release version
+    version = feed.entries[1].title.split()[-1]
+    # Install the chromedriver-py package using pip
+    subprocess.run(['pip', 'install', f'chromedriver-py=={version}'])
+
 # Check if chromedriver-py is already installed
 try:
     dist = pkg_resources.get_distribution('chromedriver-py')
     installed_version = dist.version.split('.')[0]  # Retrieve only the prefix
     chrome_version = get_chrome_version()
 
     if chrome_version and installed_version != chrome_version:
@@ -83,9 +92,11 @@
                 break
 
         if matching_version:
             # Install the corresponding chromedriver-py version
             install_chromedriver(matching_version)
         else:
             print(f"No matching chromedriver-py version found for Chrome {chrome_version}")
+            install_chromedriver_fallback_method()
     else:
         print("Failed to retrieve Chrome version.")
+        install_chromedriver_fallback_method()
```

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/imdbRatings.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/imdbRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/traktRatings.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/traktRatings.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer/verifyCredentials.py` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer/verifyCredentials.py`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/IMDbTraktSyncer.egg-info/PKG-INFO` & `IMDbTraktSyncer-1.1.3/IMDbTraktSyncer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.2
+Version: 1.1.3
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.1.2/LICENSE` & `IMDbTraktSyncer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/PKG-INFO` & `IMDbTraktSyncer-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IMDbTraktSyncer
-Version: 1.1.2
+Version: 1.1.3
 Summary: This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.
 Home-page: https://github.com/RileyXX/IMDb-Trakt-Syncer
 Keywords: python,video,trakt,imdb,ratings,sync,movies,tv shows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `IMDbTraktSyncer-1.1.2/README.md` & `IMDbTraktSyncer-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `IMDbTraktSyncer-1.1.2/setup.py` & `IMDbTraktSyncer-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #To upload package: twine upload dist/*
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = 'This python script will sync user ratings for Movies and TV Shows both ways between Trakt and IMDb.'
 
 # Setting up
 setup(
     name="IMDbTraktSyncer",
     version=VERSION,
     description=DESCRIPTION,
```

