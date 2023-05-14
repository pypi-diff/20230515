# Comparing `tmp/Flask-Static-Digest-0.3.0.tar.gz` & `tmp/Flask-Static-Digest-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-Static-Digest-0.3.0.tar", last modified: Fri Mar 17 01:15:53 2023, max compression
+gzip compressed data, was "Flask-Static-Digest-0.4.0.tar", last modified: Sun May 14 23:30:16 2023, max compression
```

## Comparing `Flask-Static-Digest-0.3.0.tar` & `Flask-Static-Digest-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-17 01:15:53.825670 Flask-Static-Digest-0.3.0/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-17 01:15:53.825670 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)      819 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      434 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       57 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/entry_points.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/not-zip-safe
--rw-r--r--   0 nick      (1000) nick      (1000)       11 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/requires.txt
--rw-r--r--   0 nick      (1000) nick      (1000)       20 2023-03-17 01:15:53.000000 Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/top_level.txt
--rw-r--r--   0 nick      (1000) nick      (1000)     1081 2019-10-30 15:21:50.000000 Flask-Static-Digest-0.3.0/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)      819 2023-03-17 01:15:53.825670 Flask-Static-Digest-0.3.0/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)    23579 2023-03-17 01:02:35.000000 Flask-Static-Digest-0.3.0/README.md
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-03-17 01:15:53.825670 Flask-Static-Digest-0.3.0/flask_static_digest/
--rw-r--r--   0 nick      (1000) nick      (1000)     2855 2023-03-17 01:04:04.000000 Flask-Static-Digest-0.3.0/flask_static_digest/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1229 2023-03-17 01:04:04.000000 Flask-Static-Digest-0.3.0/flask_static_digest/cli.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4763 2023-03-17 01:04:04.000000 Flask-Static-Digest-0.3.0/flask_static_digest/digester.py
--rw-r--r--   0 nick      (1000) nick      (1000)      104 2023-03-17 01:03:17.000000 Flask-Static-Digest-0.3.0/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)       38 2023-03-17 01:15:53.825670 Flask-Static-Digest-0.3.0/setup.cfg
--rw-r--r--   0 nick      (1000) nick      (1000)     1128 2023-03-17 01:08:10.000000 Flask-Static-Digest-0.3.0/setup.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)      871 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)      434 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/SOURCES.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/dependency_links.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       58 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/entry_points.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)        1 2023-05-14 23:30:09.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/not-zip-safe
+-rw-r--r--   0 nick      (1000) nick      (1000)       35 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/requires.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)       20 2023-05-14 23:30:15.000000 Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/top_level.txt
+-rw-r--r--   0 nick      (1000) nick      (1000)     1115 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)      871 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/PKG-INFO
+-rw-r--r--   0 nick      (1000) nick      (1000)    24264 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/README.md
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/flask_static_digest/
+-rw-r--r--   0 nick      (1000) nick      (1000)     3024 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/__init__.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     2132 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/cli.py
+-rw-r--r--   0 nick      (1000) nick      (1000)     5650 2023-05-14 23:23:06.000000 Flask-Static-Digest-0.4.0/flask_static_digest/digester.py
+-rw-r--r--   0 nick      (1000) nick      (1000)      104 2023-03-17 01:03:17.000000 Flask-Static-Digest-0.4.0/pyproject.toml
+-rw-r--r--   0 nick      (1000) nick      (1000)       38 2023-05-14 23:30:16.012017 Flask-Static-Digest-0.4.0/setup.cfg
+-rw-r--r--   0 nick      (1000) nick      (1000)     1197 2023-05-14 23:25:07.000000 Flask-Static-Digest-0.4.0/setup.py
```

### Comparing `Flask-Static-Digest-0.3.0/Flask_Static_Digest.egg-info/PKG-INFO` & `Flask-Static-Digest-0.4.0/Flask_Static_Digest.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Flask-Static-Digest
-Version: 0.3.0
-Summary: Flask extension for md5 tagging and gzipping static files.
+Version: 0.4.0
+Summary: Flask extension for md5 tagging and compressing (gzip / brotli) static files.
 Home-page: https://github.com/nickjj/flask-static-digest
 Author: Nick Janetakis
 Author-email: nick.janetakis@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -14,8 +14,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.6
+Provides-Extra: brotli
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `Flask-Static-Digest-0.3.0/LICENSE` & `Flask-Static-Digest-0.4.0/LICENSE`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 The MIT License (MIT)
 
 Copyright (c) 2019 Nick Janetakis
+Copyright (c) 2023 Matthew Swabey
 
 Permission is hereby granted, free of charge, to any person obtaining
 a copy of this software and associated documentation files (the
 'Software'), to deal in the Software without restriction, including
 without limitation the rights to use, copy, modify, merge, publish,
 distribute, sublicense, and/or sell copies of the Software, and to
 permit persons to whom the Software is furnished to do so, subject to
```

### Comparing `Flask-Static-Digest-0.3.0/PKG-INFO` & `Flask-Static-Digest-0.4.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Flask-Static-Digest
-Version: 0.3.0
-Summary: Flask extension for md5 tagging and gzipping static files.
+Version: 0.4.0
+Summary: Flask extension for md5 tagging and compressing (gzip / brotli) static files.
 Home-page: https://github.com/nickjj/flask-static-digest
 Author: Nick Janetakis
 Author-email: nick.janetakis@gmail.com
 License: MIT
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
@@ -14,8 +14,12 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Archiving :: Compression
 Requires-Python: >=3.6
+Provides-Extra: brotli
 License-File: LICENSE
+
+UNKNOWN
+
```

### Comparing `Flask-Static-Digest-0.3.0/README.md` & `Flask-Static-Digest-0.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # What is Flask-Static-Digest? ![CI](https://github.com/nickjj/flask-static-digest/workflows/CI/badge.svg?branch=master)
 
 It is a Flask extension that will help make your static files production ready
-with very minimal effort on your part. It does this by md5 tagging and gzipping
-your static files after running a `flask digest compile` command that this
-extension adds to your Flask app.
+with very minimal effort on your part. It does this by creating md5 tagged
+versions and gzip and / or brotli compressed versions of your static files by
+running a `flask digest compile` command that this extension adds to your Flask
+app.
 
 It should be the last thing you do to your static files before uploading them
 to your server or CDN. Speaking of which, if you're using a CDN this extension
 optionally lets you configure a host URL that will get prepended to your static
 file paths. If you're not using a CDN, no problem everything will work as you
 would expect by default.
 
 Other web frameworks like Django, Ruby on Rails and Phoenix all have this
 feature built into their framework, and now with this extension Flask does too.
 
 **This extension will work if you're not using any asset build tools but at the
-same time it also works with Webpack, Grunt, Gulp or any other build tool you
-can think of. This tool does not depend on or compete with existing asset build
-tools.**
+same time it also works with esbuild, Webpack, Grunt, Gulp or any other build
+tool you can think of. This tool does not depend on or compete with existing
+asset build tools.**
 
 If you're already using Webpack or a similar tool, that's great. Webpack takes
 care of bundling your assets and helps convert things like SASS to CSS and ES6+
 JS to browser compatible JS. That is solving a completely different problem
 than what this extension solves. This extension will further optimize your
 static files after your build tool produces its output files.
 
@@ -32,15 +33,16 @@
 
 ## How does it work?
 
 There's 3 pieces to this extension:
 
 1. It adds a custom Flask CLI command to your project. When you run this
    command it looks at your static files and then generates an md5 tagged
-   version of each file along with optionally gzipping them too.
+   version of each file along with optionally compressing them with gzip
+   and / or brotli.
 
 2. When the above command finishes it creates a `cache_manifest.json` file in
    your static folder which maps the regular file names, such as
    `images/flask.png` to `images/flask-f86b271a51b3cfad5faa9299dacd987f.png`.
 
 3. It adds a new template helper called `static_url_for` which uses Flask's
    `url_for` under the hood but is aware of the `cache_manifest.json` file so
@@ -58,39 +60,45 @@
 [![Demo
 Video](https://img.youtube.com/vi/-Xd84hlIjkI/0.jpg)](https://www.youtube.com/watch?v=-Xd84hlIjkI)
 
 #### Changes since this video
 
 - `FLASK_STATIC_DIGEST_HOST_URL` has been added to configure an optional external host, aka. CDN ([explained here](#configuring-this-extension))
 - If your blueprints have static files they will get digested now too (including nested blueprints!)
+- Optional Brotli support has been added
+- `FLASK_STATIC_DIGEST_COMPRESSION` has been added to control compression ([explained here](#configuring-this-extension))
 
 ## Table of Contents
 
 - [Installation](#installation)
 - [Using the newly added Flask CLI command](#using-the-newly-added-flask-cli-command)
 - [Going over the Flask CLI commands](#going-over-the-flask-cli-commands)
 - [Configuring this extension](#configuring-this-extension)
 - [Modifying your templates to use static_url_for instead of url_for](#modifying-your-templates-to-use-static_url_for-instead-of-url_for)
 - [Potentially updating your .gitignore file](#potentially-updating-your-gitignore-file)
 - [FAQ](#faq)
   - [What about development vs production and performance implications?](#what-about-development-vs-production-and-performance-implications)
-  - [Why bother gzipping your static files here instead of with nginx?](#why-bother-gzipping-your-static-files-here-instead-of-with-nginx)
+  - [Why bother compressing your static files here instead of with nginx?](#why-bother-compressing-your-static-files-here-instead-of-with-nginx)
   - [How do you use this extension with Webpack or another build tool?](#how-do-you-use-this-extension-with-webpack-or-another-build-tool)
   - [Migrating from Flask-Webpack](#migrating-from-flask-webpack)
   - [How do you use this extension with Docker?](#how-do-you-use-this-extension-with-docker)
   - [How do you use this extension with Heroku?](#how-do-you-use-this-extension-with-heroku)
   - [What about user uploaded files?](#what-about-user-uploaded-files)
 - [About the author](#about-the-author)
 
 ## Installation
 
-*You'll need to be running Python 3.5+ and using Flask 1.0 or greater.*
+*You'll need to be running Python 3.6+ and using Flask 1.0 or greater.*
 
 `pip install Flask-Static-Digest`
 
+To install with Brotli support:
+
+`pip install Flask-Static-Digest[brotli]`
+
 ### Example directory structure for a 'hello' app
 
 ```
 ├── hello
 │   ├── __init__.py
 │   ├── app.py
 │   └── static
@@ -140,15 +148,15 @@
   ...
 
 Options:
   --version  Show the flask version
   --help     Show this message and exit.
 
 Commands:
-  digest  md5 tag and gzip static files.
+  digest  md5 tag and compress static files.
   routes  Show the routes for the app.
   run     Run a development server.
   shell   Run a shell in the app context.
 ```
 
 If all went as planned you should see the new `digest` command added to the
 list of commands.
@@ -156,15 +164,15 @@
 ## Going over the Flask CLI commands
 
 Running `flask digest` will produce this help menu:
 
 ```sh
 Usage: flask digest [OPTIONS] COMMAND [ARGS]...
 
-  md5 tag and gzip static files.
+  md5 tag and compress static files.
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   clean    Remove generated static files and cache manifest.
   compile  Generate optimized static files and a cache manifest.
@@ -175,16 +183,16 @@
 ### compile
 
 Inspects your Flask app's and blueprint's `static_folder` and uses that as both
 the input and output path of where to look for and create the newly digested
 and compressed files.
 
 At a high level it recursively loops over all of the files it finds in that
-directory and then generates the md5 tagged and gzipped versions of each file.
-It also creates a `cache_manifest.json` file in the root of your
+directory and then generates the md5 tagged and compressed versions of each
+file. It also creates a `cache_manifest.json` file in the root of your
 `static_folder`.
 
 That manifest file is machine generated meaning you should not edit it unless
 you really know what you're doing.
 
 This file maps the human readable file name of let's say `images/flask.png` to
 the digested file name. It's a simple key / value set up. It's basically a
@@ -213,48 +221,54 @@
 - `cache_manifest.json`
 
 *Your md5 hashes will be different because it depends on what the contents of
 the file are.*
 
 ### clean
 
-Inspects your Flask app's `static_folder` and uses that as the input path of
-where to look for digested and compressed files.
+Inspects your Flask app's and blueprint's `static_folder` and uses that as the
+input path of where to look for digested and compressed files.
 
-It will recursively delete files that have a file extension of `.gz` and also
-deletes files that have been digested. It determines if a file has been
-digested based on its file name. In other words, it will delete files that
-match this regexp `r"-[a-f\d]{32}"`.
+It will recursively delete files that have a file extension of `.gz` or `.br`
+and files that have been digested. It determines if a file has been digested
+based on its file name. In other words, it will delete files that match this
+regexp `r"-[a-f\d]{32}"`.
 
-In the end that means if you had these 4 files in your static folder:
+In the end that means if you had these 6 files in your static folder:
 
 - `images/flask.png`
 - `images/flask.png.gz`
+- `images/flask.png.br`
 - `images/flask-f86b271a51b3cfad5faa9299dacd987f.png`
 - `images/flask-f86b271a51b3cfad5faa9299dacd987f.png.gz`
+- `images/flask-f86b271a51b3cfad5faa9299dacd987f.png.br`
 
-And you decided to run the clean command, the last 3 files would be deleted
+And you decided to run the clean command, the last 5 files would be deleted
 leaving you with the original `images/flask.png`.
 
 ## Configuring this extension
 
-By default this extension will md5 tag all files it finds in your configured
-`static_folder`. It will also create gzipped versions of each file and it won't
-prefix your static files with an external host.
+By default this extension will create md5 tagged versions of all files it finds
+in your configured `static_folder`. It will also create gzip'ed versions of each
+file and it won't prefix your static files with an external host.
 
-If you don't like any of this behavior, you can optionally configure:
+If you don't like any of this behavior or you wish to enable brotli you can
+optionally configure:
 
 ```py
 FLASK_STATIC_DIGEST_BLACKLIST_FILTER = []
 # If you want specific extensions to not get md5 tagged you can add them to
 # the list, such as: [".htm", ".html", ".txt"]. Make sure to include the ".".
 
-FLASK_STATIC_DIGEST_GZIP_FILES = True
-# When set to False then gzipped files will not be created but static files
-# will still get md5 tagged.
+FLASK_STATIC_DIGEST_COMPRESSION = ["gzip"]
+# Optionally compress your static files, supported values are:
+#   []                 avoids any compression
+#   ["gzip"]           uses gzip
+#   ["brotli"]         uses brotli (prefer either gzip or both)
+#   ["gzip", "brotli"] uses both
 
 FLASK_STATIC_DIGEST_HOST_URL = None
 # When set to a value such as https://cdn.example.com and you use static_url_for
 # it will prefix your static path with this URL. This would be useful if you
 # host your files from a CDN. Make sure to include the protocol (aka. https://).
 ```
 
@@ -324,15 +338,15 @@
 ignoring the static files it produces as output. It's a common pattern to
 commit your Webpack source static files but ignore the compiled static files
 it produces.
 
 But if you're not using Webpack or another asset build tool then the static
 files that are a part of your project might have the same source and
 destination directory. If that's the case, chances are you'll want to git
-ignore the md5 tagged files as well as the gzipped and `cache_manifest.json`
+ignore the md5 tagged files as well as the compressed and `cache_manifest.json`
 files from version control.
 
 For clarity, you want to ignore them because you'll be generating them on your
 server at deploy time or within a Docker image if you're using Docker.  They
 don't need to be tracked in version control.
 
 Add this to your `.gitignore` file to ignore certain files this extension
@@ -367,15 +381,15 @@
 run time which is many orders of magnitude faster than even the most simple
 database query.
 
 **In other words, this extension is not going to negatively impact the
 performance of your web application. If anything it's going to speed it up and
 save you money on hosting**.
 
-That's because gzipped files can be upwards of 5-10x smaller so there's less
+That's because compressed files can be upwards of 5-10x smaller so there's less
 bytes to transfer over the network.
 
 Also with md5 tagging each file it means you can configure your web server such
 as nginx to cache each file forever. That means if a user visits your site a
 second time in the future, nginx will be smart enough to load it from their
 local browser's cache without even contacting your server. It's a 100% local
 look up.
@@ -388,42 +402,43 @@
 
 This tactic is commonly referred to as "cache busting" and it's a very good
 idea to do this in production. You can even go 1 step further and serve your
 static files using a CDN. Using this cache busting strategy makes configuring
 your CDN a piece of cake since you don't need to worry about ever expiring your
 cache manually.
 
-### Why bother gzipping your static files here instead of with nginx?
+### Why bother compressing your static files here instead of with nginx?
 
-You would still be using nginx's gzip features, but now instead of nginx having
-to gzip your files on the fly at run time you can configure nginx to use the
-pre-made gzipped files that this extension creates.
+You would still be using nginx's gzip / brotli features, but now instead of
+nginx having to compress your files on the fly at run time you can configure
+nginx to use the pre-made compressed files that this extension creates.
 
 This way you can benefit from having maximum compression without having nginx
-waste precious CPU cycles gzipping files on the fly. This gives you the best of
-both worlds -- the highest compression ratio with no noticeable run time
+waste precious CPU cycles compressing files on the fly. This gives you the best
+of both worlds -- the highest compression ratio with no noticeable run time
 performance penalty.
 
 ### How do you use this extension with Webpack or another build tool?
 
 It works out of the box with no extra configuration or plugins needed for
 Webpack or your build tool of choice.
 
 Typically the Webpack (or another build tool) work flow would look like this:
 
 - You configure Webpack with your source static files directory
 - You configure Webpack with your destination static files directory
-- Webpack processes your files in the source directory and copies them to the destination directory
+- Webpack processes your files in the source directory and copies them to the
+  destination directory
 - Flask is configured to serve static files from that destination directory
 
 For example, your source directory might be `assets/` inside of your project
 and the destination might be `myapp/static`.
 
 This extension will look at your Flask configuration for the `static_folder`
-and determine it's set to `myapp/static` so it will md5 tag and gzip those
+and determine it's set to `myapp/static` so it will md5 tag and compress those
 files. Your Webpack source files will not get digested and compressed.
 
 ### Migrating from Flask-Webpack
 
 [Flask-Webpack](https://github.com/nickjj/flask-webpack) is another extension I
 wrote a long time ago which was specific to Webpack but had a similar idea to
 this extension. Flask-Webpack is now deprecated in favor of
@@ -488,19 +503,19 @@
 
 ### What about user uploaded files?
 
 Let's say that besides having static files like your logo and CSS / JavaScript
 bundles you also have files uploaded by users. This could be things like a user
 avatar, blog post images or anything else.
 
-**You would still want to md5 tag and gzip these files but now we've run into a
-situation**. The `flask digest compile` command is meant to be run at deploy
-time and it could potentially be run from your dev box, inside of a Docker
-image, on a CI server or your production server. In these cases you wouldn't
-have access to the user uploaded files.
+**You would still want to md5 tag and compress these files but now we've run
+into a situation**. The `flask digest compile` command is meant to be run at
+deploy time and it could potentially be run from your dev box, inside of a
+Docker image, on a CI server or your production server. In these cases you
+wouldn't have access to the user uploaded files.
 
 But at the same time you have users uploading files at run time. They are
 changing all the time.
 
 **Needless to say you can't use the `flask digest compile` command to digest
 user uploaded files**. The `cache_manifest.json` file should be reserved for
 files that exist in your code repo (such as your CSS / JS bundles, maybe a
@@ -522,39 +537,39 @@
 referencing that in your template helper (`static_url_for`), so it's never a
 hard coded thing that changes at the template level.
 
 What's cool about this is you already did the database query to retrieve the
 record(s) from the database, so there's no extra database work to do. All you
 have to do is reference the file name field that's a part of your model.
 
-But that doesn't fully solve the problem. You'll still want to md5 tag and gzip
-your user uploaded content at run time and you would want to do this before you
-save the uploaded file into its final destination (local file system, S3,
-etc.).
+But that doesn't fully solve the problem. You'll still want to md5 tag and
+compress your user uploaded content at run time and you would want to do this
+before you save the uploaded file into its final destination (local file system,
+S3, etc.).
 
 This can be done completely separate from this extension and it's really going
-to vary depending on where you host your user uploaded content. For example
-some CDNs will automatically create gzipped files for you and they use things
-like an ETag header in the response to include a unique file name (and this is
-what you can store in your DB).
+to vary depending on where you host your user uploaded content. For example some
+CDNs will automatically create compressed files for you and they use things like
+an ETag header in the response to include a unique file name (and this is what
+you can store in your DB).
 
-So maybe md5 hashing and maybe gzipping your user uploaded content becomes an
+So maybe md5 hashing and maybe compressing your user uploaded content becomes an
 app specific responsibility, although I'm not opposed to maybe creating helper
 functions you can use but that would need to be thought out carefully.
 
 However the implementation is not bad. It's really only about 5 lines of code
 to do both things. Feel free to `CTRL + F` around the [code
 base](https://github.com/nickjj/flask-static-digest/blob/master/flask_static_digest/digester.py)
-for `hashlib` and `gzip` and you'll find the related code.
+for `hashlib`, `gzip` and `brotli` and you'll find the related code.
 
 **So with that said, here's a work flow you can do to deal with this today:**
 
 - User uploads file
 - Your Flask app potentially md5 tags / gzips the file if necessary
-- Your Flask app saves the file name + gzipped file to its final destination (local file system, S3, etc.)
+- Your Flask app saves the file name + compressed file to its final destination (local file system, S3, etc.)
 - Your Flask app saves the final unique file name to your database
 
 That final unique file name would be the md5 tagged version of the file that
 you created or the unique file name that your CDN returned back to you. I hope
 that clears up how to deal with user uploaded files and efficiently serving
 them!
```

### Comparing `Flask-Static-Digest-0.3.0/flask_static_digest/__init__.py` & `Flask-Static-Digest-0.4.0/flask_static_digest/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import logging
 import json
+import logging
 import os
-
 from urllib.parse import urljoin
 
-from flask import request, url_for as flask_url_for
+from flask import request
+from flask import url_for as flask_url_for
 
 
 class FlaskStaticDigest(object):
     def __init__(self, app=None):
         self.app = app
 
         if app is not None:
@@ -18,16 +18,19 @@
         """
         Mutate the application passed in as explained here:
           https://flask.palletsprojects.com/en/1.1.x/extensiondev/
         :param app: Flask application
         :return: None
         """
         app.config.setdefault("FLASK_STATIC_DIGEST_BLACKLIST_FILTER", [])
-        app.config.setdefault("FLASK_STATIC_DIGEST_GZIP_FILES", True)
         app.config.setdefault("FLASK_STATIC_DIGEST_HOST_URL", None)
+        app.config.setdefault("FLASK_STATIC_DIGEST_COMPRESSION", ["gzip"])
+
+        compression = set(app.config["FLASK_STATIC_DIGEST_COMPRESSION"])
+        app.config["FLASK_STATIC_DIGEST_COMPRESSION"] = list(compression)
 
         self.host_url = app.config.get("FLASK_STATIC_DIGEST_HOST_URL")
 
         self.manifests = {}
 
         self._load_manifest("static", app)
         for endpoint, blueprint in app.blueprints.items():
```

### Comparing `Flask-Static-Digest-0.3.0/flask_static_digest/digester.py` & `Flask-Static-Digest-0.4.0/flask_static_digest/digester.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,78 +1,90 @@
+import functools
 import glob
 import gzip
 import hashlib
 import json
 import os.path
 import re
 import shutil
 
 DIGESTED_FILE_REGEX = r"-[a-f\d]{32}"
+CHUNK_SIZE = 1024 * 1024
 
 
-def compile(input_path, output_path, digest_blacklist_filter, gzip_files):
+def compile(
+    input_path, output_path, digest_blacklist_filter, gzip_files, brotli_files
+):
     """
-    Generate md5 tagged static files that are also compressed with gzip.
+    Generate md5 tagged static files compressed with gzip and brotli.
 
     :param input_path: The source path of your static files
     :type input_path: str
     :param output_path: The destination path of your static files
     :type output_path: str
     :param digest_blacklist_filter: Ignore compiling these file types
     :type digest_blacklist_filter: list
     :param gzip_files: Whether or not gzipped files will be generated
     :type gzip_files: bool
+    :param brotli_files: Whether or not brotli files will be generated
+    :type brotli_files: bool
     :return: None
     """
     if not os.path.exists(input_path):
         print(f"The input path '{input_path}' does not exist")
         return None
 
     if not os.path.exists(output_path):
         print(f"The output path '{output_path}' does not exist")
         return None
 
     files = _filter_files(input_path, digest_blacklist_filter)
-    manifest = _generate_manifest(files, gzip_files, output_path)
+    manifest = _generate_manifest(files, gzip_files, brotli_files, output_path)
     _save_manifest(manifest, output_path)
 
     print(f"Check your digested files at '{output_path}'")
     return None
 
 
-def clean(output_path, digest_blacklist_filter, gzip_files):
+def clean(output_path, digest_blacklist_filter, gzip_files, brotli_files):
     """
     Delete the generated md5 tagged and gzipped static files.
 
     :param input_path: The source path of your static files
     :type input_path: str
     :param output_path: The destination path of your static files
     :type output_path: str
-    :param digest_blacklist_filter: Ignore compiling these file types
+    :param digest_blacklist_filter: Ignore cleaning these file types
     :type digest_blacklist_filter: list
-    :param gzip_files: Whether or not gzipped files will be generated
+    :param gzip_files: Whether or not gzipped files will be cleaned
     :type gzip_files: bool
+    :param brotli_files: Whether or not brotli files will be cleaned
+    :type brotli_files: bool
     :return: None
     """
     for item in glob.iglob(output_path + "**/**", recursive=True):
         if os.path.isfile(item):
-            file_name, file_extension = os.path.splitext(item)
+            _, file_extension = os.path.splitext(item)
             basename = os.path.basename(item)
 
             if (
                 re.search(DIGESTED_FILE_REGEX, basename)
                 and file_extension not in digest_blacklist_filter
             ):
                 if os.path.exists(item):
                     os.remove(item)
 
             if gzip_files and file_extension == ".gz":
                 if os.path.exists(item):
                     os.remove(item)
 
+            if brotli_files and file_extension == ".br":
+                if os.path.exists(item):
+                    os.remove(item)
+
     manifest_path = os.path.join(output_path, "cache_manifest.json")
 
     if os.path.exists(manifest_path):
         os.remove(manifest_path)
 
     print(f"Check your cleaned files at '{output_path}'")
     return None
@@ -93,32 +105,35 @@
     file_name, file_extension = os.path.splitext(file_path)
     basename = os.path.basename(file_path)
 
     return (
         re.search(DIGESTED_FILE_REGEX, basename)
         or file_extension in digest_blacklist_filter
         or file_extension == ".gz"
+        or file_extension == ".br"
         or basename == "cache_manifest.json"
     )
 
 
-def _generate_manifest(files, gzip_files, output_path):
+def _generate_manifest(files, gzip_files, brotli_files, output_path):
     manifest = {}
 
     for file in files:
         rel_file_path = os.path.relpath(file, output_path).replace("\\", "/")
 
         file_name, file_extension = os.path.splitext(rel_file_path)
 
         digest = _generate_digest(file)
         digested_file_path = f"{file_name}-{digest}{file_extension}"
 
         manifest[rel_file_path] = digested_file_path
 
-        _write_to_disk(file, digested_file_path, gzip_files, output_path)
+        _write_to_disk(
+            file, digested_file_path, gzip_files, brotli_files, output_path
+        )
 
     return manifest
 
 
 def _generate_digest(file):
     digest = None
 
@@ -134,23 +149,39 @@
 
     with open(manifest_path, "w") as f:
         f.write(manifest_content)
 
     return None
 
 
-def _write_to_disk(file, digested_file_path, gzip_files, input_path):
+def _write_to_disk(
+    file, digested_file_path, gzip_files, brotli_files, input_path
+):
     full_digested_file_path = os.path.join(input_path, digested_file_path)
 
     # Copy file while preserving permissions and meta data if supported.
     shutil.copy2(file, full_digested_file_path)
 
     if gzip_files:
         with open(file, "rb") as f_in:
             with gzip.open(f"{file}.gz", "wb") as f_out:
                 shutil.copyfileobj(f_in, f_out)
 
-        with open(full_digested_file_path, "rb") as f_in:
-            with gzip.open(f"{full_digested_file_path}.gz", "wb") as f_out:
-                shutil.copyfileobj(f_in, f_out)
+        shutil.copy2(f"{file}.gz", f"{full_digested_file_path}.gz")
+
+    if brotli_files:
+        import brotli
+
+        compressor = brotli.Compressor(quality=11)
+
+        with open(file, "rb") as f_in:
+            with open(f"{file}.br", "wb") as f_out:
+                read_chunk = functools.partial(f_in.read, CHUNK_SIZE)
+
+                for data in iter(read_chunk, b""):
+                    f_out.write(compressor.process(data))
+
+                f_out.write(compressor.finish())
+
+        shutil.copy2(f"{file}.br", f"{full_digested_file_path}.br")
 
     return None
```

### Comparing `Flask-Static-Digest-0.3.0/setup.py` & `Flask-Static-Digest-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 
 setup(
     name="Flask-Static-Digest",
-    version="0.3.0",
+    version="0.4.0",
     author="Nick Janetakis",
     author_email="nick.janetakis@gmail.com",
     url="https://github.com/nickjj/flask-static-digest",
-    description="Flask extension for md5 tagging and gzipping static files.",
+    description="Flask extension for md5 tagging and compressing (gzip / brotli) static files.",
     license="MIT",
     package_data={"Flask-Static-Digest": ["VERSION"]},
     packages=["flask_static_digest"],
     platforms="any",
     python_requires=">=3.6",
     zip_safe=False,
     install_requires=["Flask>=1.0"],
+    extras_require={"brotli": ["Brotli>=1.0.9"]},
     entry_points={
         "flask.commands": ["digest=flask_static_digest.cli:digest"],
     },
     classifiers=[
         "Environment :: Web Environment",
         "Framework :: Flask",
         "Intended Audience :: Developers",
```

