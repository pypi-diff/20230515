# Comparing `tmp/steamcrawl-0.2.0.tar.gz` & `tmp/steamcrawl-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "steamcrawl-0.2.0.tar", last modified: Wed May 10 13:35:58 2023, max compression
+gzip compressed data, was "steamcrawl-1.0.0.tar", last modified: Mon May 15 12:46:01 2023, max compression
```

## Comparing `steamcrawl-0.2.0.tar` & `steamcrawl-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.486869 steamcrawl-0.2.0/
--rw-rw-rw-   0        0        0     1085 2023-05-09 14:08:49.000000 steamcrawl-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4645 2023-05-10 13:35:58.485870 steamcrawl-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4235 2023-05-09 19:22:01.000000 steamcrawl-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-10 13:35:58.486869 steamcrawl-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      656 2023-05-10 13:30:45.000000 steamcrawl-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.463929 steamcrawl-0.2.0/steamcrawl/
--rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-0.2.0/steamcrawl/__init__.py
--rw-rw-rw-   0        0        0      543 2023-05-07 15:13:15.000000 steamcrawl-0.2.0/steamcrawl/exceptions.py
--rw-rw-rw-   0        0        0    25429 2023-05-10 13:29:36.000000 steamcrawl-0.2.0/steamcrawl/request.py
-drwxrwxrwx   0        0        0        0 2023-05-10 13:35:58.484873 steamcrawl-0.2.0/steamcrawl.egg-info/
--rw-rw-rw-   0        0        0     4645 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-10 13:35:58.000000 steamcrawl-0.2.0/steamcrawl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-15 12:46:01.524535 steamcrawl-1.0.0/
+-rw-rw-rw-   0        0        0     1085 2023-05-09 14:08:49.000000 steamcrawl-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0     4502 2023-05-15 12:46:01.523537 steamcrawl-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4092 2023-05-15 12:43:23.000000 steamcrawl-1.0.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 12:46:01.524535 steamcrawl-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      656 2023-05-15 12:08:48.000000 steamcrawl-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:46:01.499603 steamcrawl-1.0.0/steamcrawl/
+-rw-rw-rw-   0        0        0       28 2023-05-07 13:37:24.000000 steamcrawl-1.0.0/steamcrawl/__init__.py
+-rw-rw-rw-   0        0        0      543 2023-05-07 15:13:15.000000 steamcrawl-1.0.0/steamcrawl/exceptions.py
+-rw-rw-rw-   0        0        0    25574 2023-05-15 12:43:05.000000 steamcrawl-1.0.0/steamcrawl/request.py
+drwxrwxrwx   0        0        0        0 2023-05-15 12:46:01.522540 steamcrawl-1.0.0/steamcrawl.egg-info/
+-rw-rw-rw-   0        0        0     4502 2023-05-15 12:46:01.000000 steamcrawl-1.0.0/steamcrawl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-15 12:46:01.000000 steamcrawl-1.0.0/steamcrawl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 12:46:01.000000 steamcrawl-1.0.0/steamcrawl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-05-15 12:46:01.000000 steamcrawl-1.0.0/steamcrawl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-15 12:46:01.000000 steamcrawl-1.0.0/steamcrawl.egg-info/top_level.txt
```

### Comparing `steamcrawl-0.2.0/LICENSE` & `steamcrawl-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.2.0/PKG-INFO` & `steamcrawl-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.2.0
+Version: 1.0.0
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,16 +13,14 @@
 ![PyPI](https://img.shields.io/pypi/v/steamcrawl?label=pypi%20package)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
-This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
-
 A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
```

### Comparing `steamcrawl-0.2.0/README.md` & `steamcrawl-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 ![PyPI](https://img.shields.io/pypi/v/steamcrawl?label=pypi%20package)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
-This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
-
 A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
```

### Comparing `steamcrawl-0.2.0/setup.py` & `steamcrawl-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name='steamcrawl',
-    version='0.2.0',
+    version='1.0.0',
     description='A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.',
     packages=["steamcrawl"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Hungreeee',
     author_email='hungmnguyen13102003@gmail.com',
     license='MIT',
```

### Comparing `steamcrawl-0.2.0/steamcrawl/exceptions.py` & `steamcrawl-1.0.0/steamcrawl/exceptions.py`

 * *Files identical despite different names*

### Comparing `steamcrawl-0.2.0/steamcrawl/request.py` & `steamcrawl-1.0.0/steamcrawl/request.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
     :return: Nothing.
     :rtype: None
     """
 
     dfGather = []
     requestObject = requests.get(api, params=params, headers=headers)
     contentObject = json.loads(requestObject.content)
+    exception('network', contentObject, None, "No information for this API call. Please double check your parameters and try again.")
 
     for i in index:
       if i in contentObject:
         if contentObject[i] != []:
           dfGather.append(contentObject[i])
 
     exception('network', dfGather, [], "No information for this API call. Please double check your parameters and try again.")
@@ -119,15 +120,15 @@
     exception('contain', sortby, ['price', 'quantity', ''], 
       f"{sortby} is not valid as a sortby type. It should only be '', 'price', or 'quantity'.")
     exception('contain', sortdir, ['desc', 'asc'], 
       f"{sortdir} is not valid as a sortby type. It should only be 'desc' or 'asc'.")
     
     params = {
       'sort_column': sortby,
-      'sort_dir': '',
+      'sort_dir': sortdir,
       'start': 0, 
       'count': count,
       'norender': 1
     }
 
     jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
 
@@ -185,15 +186,15 @@
       f"{sortdir} is not valid as a sortby type. It should only be 'desc' or 'asc'.")
     if appid != '':
       exception('contain', int(appid), list(self.get_all_appid()['appid']), 
         f"{appid} is not a valid appid. Please check the complete list using get_all_appid().")
     
     params = {
       'sort_column': sortby,
-      'sort_dir': '',
+      'sort_dir': sortdir,
       'appid': appid,
       'start': 0, 
       'count': count,
       'norender': 1
     }
 
     jsonObject = self.__request_helper(self.__all_listings_api, params, self.headers, ['results'])[0]
```

### Comparing `steamcrawl-0.2.0/steamcrawl.egg-info/PKG-INFO` & `steamcrawl-1.0.0/steamcrawl.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: steamcrawl
-Version: 0.2.0
+Version: 1.0.0
 Summary: A package that helps extract Steam store and community market data as pandas DataFrame for better readabilty and usability.
 Home-page: https://github.com/Hungreeee/steamcrawl
 Author: Hungreeee
 Author-email: hungmnguyen13102003@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -13,16 +13,14 @@
 ![PyPI](https://img.shields.io/pypi/v/steamcrawl?label=pypi%20package)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Repo Size](https://img.shields.io/github/repo-size/Hungreeee/steamcrawl.svg)](https://github.com/Hungreeee/steamcrawl/)
 [![GitHub follow](https://img.shields.io/github/followers/Hungreeee.svg?style=social&label=Follow&maxAge=2592000)](https://github.com/Hungreeee?tab=followers)
 
 # steamcrawl
 
-This is still a work in progress. Some functionality are available but not quite fully tested. The final version will be release as v1.0.0.
-
 A package that helps extract Steam store and community market data as pandas DataFrame for better readability and usability. The package makes queries to different Steam API, clean and extract the important variables from the JSON object result and return a pandas Dataframe. 
 
 With the Steam request limit, you can make 200 requests every 5 minutes. If you exceed the limit, Steam can give you a cooldown of (possibly) a few 1,2 minutes to 6 hours (depending on the API). Please make an appropriate number of requests at a given time. It is recommended to close any Steam web and application to limit the requests you are sending.
 
 ## Installation and setup
 
 The following libraries are used in the package. Thus, the requirement of their installation must be met:
```

