# Comparing `tmp/feedfilter-1.0.1.tar.gz` & `tmp/feedfilter-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feedfilter-1.0.1.tar", max compression
+gzip compressed data, was "feedfilter-1.0.3.tar", max compression
```

## Comparing `feedfilter-1.0.1.tar` & `feedfilter-1.0.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    35150 2022-12-31 23:31:41.428384 feedfilter-1.0.1/LICENSE
--rw-r--r--   0        0        0     4210 2023-01-09 13:25:32.157093 feedfilter-1.0.1/README.md
--rw-r--r--   0        0        0      911 2023-01-09 13:29:36.934474 feedfilter-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      359 2022-12-31 23:41:18.220255 feedfilter-1.0.1/src/feedfilter/__init__.py
--rwxr-xr-x   0        0        0    13467 2023-01-01 20:50:07.830931 feedfilter-1.0.1/src/feedfilter/feed_filter.py
--rw-r--r--   0        0        0     3254 2022-12-31 23:41:17.808252 feedfilter-1.0.1/src/feedfilter/logger.py
--rw-r--r--   0        0        0     5249 1970-01-01 00:00:00.000000 feedfilter-1.0.1/setup.py
--rw-r--r--   0        0        0     5061 1970-01-01 00:00:00.000000 feedfilter-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    35150 2022-12-31 23:31:41.428384 feedfilter-1.0.3/LICENSE
+-rw-r--r--   0        0        0     4210 2023-01-09 13:25:32.157093 feedfilter-1.0.3/README.md
+-rw-r--r--   0        0        0      932 2023-05-15 11:36:15.557204 feedfilter-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      359 2022-12-31 23:41:18.220255 feedfilter-1.0.3/src/feedfilter/__init__.py
+-rwxr-xr-x   0        0        0    13806 2023-05-15 11:56:42.820107 feedfilter-1.0.3/src/feedfilter/feed_filter.py
+-rw-r--r--   0        0        0     3254 2022-12-31 23:41:17.808252 feedfilter-1.0.3/src/feedfilter/logger.py
+-rw-r--r--   0        0        0     5098 1970-01-01 00:00:00.000000 feedfilter-1.0.3/PKG-INFO
```

### Comparing `feedfilter-1.0.1/LICENSE` & `feedfilter-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feedfilter-1.0.1/README.md` & `feedfilter-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `feedfilter-1.0.1/pyproject.toml` & `feedfilter-1.0.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # For how poetry is configured with this file, see
 # https://python-poetry.org/docs/pyproject/
 
 
 [tool.poetry]
 name = "feedfilter"
-version = "1.0.1"
+version = "1.0.3"
 description = "Modify RSS/Atom feeds"
 authors = ["Jim Bauer"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 #homepage = "url-to-homepage"
 repository = "https://gitlab.com/jim_bauer/feed-filter"
 #documentation = "url-to-documentation"
@@ -23,21 +23,21 @@
 
 [tool.poetry.scripts]
 feed-filter = "feedfilter:main"
 
 
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = ">=3.10"
 feedparser = "^6.0.10"
 feedgen = "^0.9.0"
 pytz = ">=2022.6"
 bs4 = "^0.0.1"
 requests = "^2.28.1"
-
+sgmllib3k = "^1.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.2.0"
 flake8 = ">=6.0.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `feedfilter-1.0.1/src/feedfilter/feed_filter.py` & `feedfilter-1.0.3/src/feedfilter/feed_filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -111,18 +111,22 @@
         logger.debug('Content changed (old): %s', orig)
         logger.debug('Content changed (new): %s', new)
 
     return new
 
 
 class MangleTitle:
-    def __init__(self, title_re=None, title_sub=None, add_date=None):
+    def __init__(self, title_re=None, title_sub=None, add_date=None,
+                 date_spaces=150):
         logger.debug('title_re=%s', title_re)
         logger.debug('title_sub=%s', title_sub)
         logger.debug('add_date=%s', add_date)
+        logger.debug('date_spaces=%s', date_spaces)
+
+        self.date_spaces = date_spaces
 
         if title_re is None:
             self.title_re = None
         else:
             self.title_re = re.compile(title_re, re.IGNORECASE)
 
         # Handle someone using '\0' as a reference to the whole match
@@ -141,15 +145,15 @@
 
     def mangle(self, title, date):
         if self.title_re and self.title_sub:
             title = self.title_re.sub(self.title_sub, title)
 
         if self.add_date:
             dt = date.astimezone(timezone('UTC'))
-            title += ' ' * 150 + f'({dt})'
+            title += ' ' * self.date_spaces + f'({dt})'
 
         logger.debug('new title = %s', title)
         return title
 
 
 class FeedParserToFeedGenerator:
     def __init__(self, extensions=None, auto_links=False):
@@ -340,14 +344,16 @@
     p.add_argument('--title-re', default=reg,
                    help='python regex used to match titles')
     p.add_argument('--title-sub', default=sub,
                    help='python regex subsitution')
     p.add_argument('--add-date-to-title', default='yes',
                    choices=['yes', 'no'],
                    help='add date/time string to entry title (for sorting)')
+    p.add_argument('--date_spaces', type=int, default=200,
+                   help='number of spaces to insert before date for --add-date-to-title')
     p.add_argument('--add-posts', action='store_true',
                    help='Add posts made to this topic '
                    '(requires network access)')
     p.add_argument('--auto-links', action='store_true',
                    help='Automatically add links for test that looks like URLs')
     p.add_argument('--version', action='store_true',
                    help='display version and exit')
@@ -384,15 +390,16 @@
         print(f'{prog_name} {__version__}')
         sys.exit(0)
 
     logger.init(prog_name, args=args)
     logger.info('%s %s starting', prog_name, __version__)
     logger.info('Options: %s', args)
 
-    mt = MangleTitle(args.title_re, args.title_sub, args.add_date_to_title)
+    mt = MangleTitle(args.title_re, args.title_sub, args.add_date_to_title,
+                     date_spaces=args.date_spaces)
     fp2fg = FeedParserToFeedGenerator(auto_links=args.auto_links)
 
     parsed = get_feed_data(args.forum)
 
     fp2fg.create_feed(parsed.feed)
 
     if args.add_posts:
```

### Comparing `feedfilter-1.0.1/src/feedfilter/logger.py` & `feedfilter-1.0.3/src/feedfilter/logger.py`

 * *Files identical despite different names*

### Comparing `feedfilter-1.0.1/setup.py` & `feedfilter-1.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,161 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: feedfilter
+Version: 1.0.3
+Summary: Modify RSS/Atom feeds
+Home-page: https://gitlab.com/jim_bauer/feed-filter
+License: GPL-3.0-or-later
+Keywords: rss,atom
+Author: Jim Bauer
+Requires-Python: >=3.10
+Classifier: Environment :: Console
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Text Processing :: Filters
+Requires-Dist: bs4 (>=0.0.1,<0.0.2)
+Requires-Dist: feedgen (>=0.9.0,<0.10.0)
+Requires-Dist: feedparser (>=6.0.10,<7.0.0)
+Requires-Dist: pytz (>=2022.6)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: sgmllib3k (>=1.0.0,<2.0.0)
+Project-URL: Repository, https://gitlab.com/jim_bauer/feed-filter
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# feed-filter
 
-packages = \
-['feedfilter']
+Filter for modifying feed data.  By default, reads feed from stdin and writes a
+modified feed to stdout in either Atom (default) or RSS format.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['bs4>=0.0.1,<0.0.2',
- 'feedgen>=0.9.0,<0.10.0',
- 'feedparser>=6.0.10,<7.0.0',
- 'pytz>=2022.6',
- 'requests>=2.28.1,<3.0.0']
-
-entry_points = \
-{'console_scripts': ['feed-filter = feedfilter:main']}
-
-setup_kwargs = {
-    'name': 'feedfilter',
-    'version': '1.0.1',
-    'description': 'Modify RSS/Atom feeds',
-    'long_description': "# feed-filter\n\nFilter for modifying feed data.  By default, reads feed from stdin and writes a\nmodified feed to stdout in either Atom (default) or RSS format.\n\nfeed-filter can modify the titles of entries via a regular expression\n(python re syntax) and also add the entry's date to the far end of the\ntitle as an aid to sorting for feed readers that cannot have both a\nprimary sort and secondary sort fields.\n\nfeed-filter can also optionaly make some modification to the content\nsuch as converting URLs into links.\n\n## Options\n\n### --title-re and --title-sub\n\nThe --title-re option specifies a regular expression.  And the --title-sub option can use backrefferences to the RE in --title-re.\n\nSo for example, if you have the following options\n> --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\\3'\n\nIt will make the following modification to the title\n\nOriginal title:\n> Tutorials and videos • Re: Part design Tutorials and much more ...\n\nModified title:\n> Part design Tutorials and much more ...\n\nThat change did 2 things.  It removed a common prefix (forum title) that all entries have, and also removed the 'Re: ' that is added to replies.\n\nIf you wanted to keep the prefix, but just remove the 'Re: ', then\nchange the second option like the example below:\n\n> --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\\1\\3'\n\nAnd the modified title will now be\n\nModified title:\n> Tutorials and videos • Part design Tutorials and much more ...\n\nEither of the above two examples can be helpfull for modifying a feed\nfor a forum so that you can sort the entries by title (headline) so\nall posts and their responses are groups together.\n\n### --add-date-to-title\n\nJust grouping all related posts together is helpfull, but you probably\nwant to display them in the order they were created.  If you happen to\nhave a feed reader that can sort on titles with a secondary sort on\nthe date, then you are all set.  But if you can only do one sort\n(title), the posts may be in the wrong order.  This is where the\n--add-date-to-title option comes in.\n\nIt does pretty much what it says.  It appends the posting's date to\nthe end of the title after a bunch of spaces.  All the spaces are just\nto hide the date string.  The date aids in sorting.  Now when you sort\non the title, the entries will implicitly have a secondary sort on the\ndate due to its inclusion in the titles.\n\n### --add-posts\n\nFor each entry, it attempts to download a topic-specific rss or atom\nfeed and adds each entry in place of the original entry.  This is\nusefull for sites whos forum feed only shows the topics (first post)\nand not any replies.  Note that this option won't work on many sites\ndue to having to parse web pages.  Raise issue for any site that\ndoesn't seem to work.  Titles on additional posts fetched will all\nbe taken from the original entry.\n\n### --auto-links\n\nIn the content sections, anything that looks like a URL but is not already\nan HTML link, will be made into a link.\n\n### --output-fmt\n\nValue can be either 'atom' (default), 'rss', or 'summary'.  The\n'summary' options just prints out a few fields in plain text format.\nUsed primary for debugging.\n\n### Others\n\nRun feed-filter with the --help option to see what other options\nare available.\n\n\n# Installation\n\nThis [package](https://pypi.org/project/feedfilter/) is on [PyPI.org](https://pypi.org/), so just install with pip or pipx like\n\n```\npipx install feedfilter\n```\n\n# Development setup\n\nIt is recommended that you do any development in a virtual\nenvironment.  If you use direnv, a .envrc file is provided.  You\nshould always look it over before allowing it to be used.\n\npoetry is required.  You can install it in your virtual enviroment\nfor this project via ```pip install poetry``` or alternatively via\n\n```\npipx install poetry\n```\n\nOnce that is installed, just run\n```\nmake install-requirements\n  or\npoetry install\n```\n\nTo run feed-filter in development, you should be able to just run\n\n```\nfeed-filter <args>\n```\n\n## Building\n\nTo create a build (sdist, wheel) run the following\n\n```\nmake build\n```\n\nResults will be in the dist/ directory.\n\n# Licensing\n\nThis project is licensed under the GNU GPL version 3 or later.  See the\nLICENSE file in the top-level directory.\n",
-    'author': 'Jim Bauer',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://gitlab.com/jim_bauer/feed-filter',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
+feed-filter can modify the titles of entries via a regular expression
+(python re syntax) and also add the entry's date to the far end of the
+title as an aid to sorting for feed readers that cannot have both a
+primary sort and secondary sort fields.
 
+feed-filter can also optionaly make some modification to the content
+such as converting URLs into links.
+
+## Options
+
+### --title-re and --title-sub
+
+The --title-re option specifies a regular expression.  And the --title-sub option can use backrefferences to the RE in --title-re.
+
+So for example, if you have the following options
+> --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\3'
+
+It will make the following modification to the title
+
+Original title:
+> Tutorials and videos • Re: Part design Tutorials and much more ...
+
+Modified title:
+> Part design Tutorials and much more ...
+
+That change did 2 things.  It removed a common prefix (forum title) that all entries have, and also removed the 'Re: ' that is added to replies.
+
+If you wanted to keep the prefix, but just remove the 'Re: ', then
+change the second option like the example below:
+
+> --title-re='([^•]+ • )?(Re: )?(.*)' --title-sub='\1\3'
+
+And the modified title will now be
+
+Modified title:
+> Tutorials and videos • Part design Tutorials and much more ...
+
+Either of the above two examples can be helpfull for modifying a feed
+for a forum so that you can sort the entries by title (headline) so
+all posts and their responses are groups together.
+
+### --add-date-to-title
+
+Just grouping all related posts together is helpfull, but you probably
+want to display them in the order they were created.  If you happen to
+have a feed reader that can sort on titles with a secondary sort on
+the date, then you are all set.  But if you can only do one sort
+(title), the posts may be in the wrong order.  This is where the
+--add-date-to-title option comes in.
+
+It does pretty much what it says.  It appends the posting's date to
+the end of the title after a bunch of spaces.  All the spaces are just
+to hide the date string.  The date aids in sorting.  Now when you sort
+on the title, the entries will implicitly have a secondary sort on the
+date due to its inclusion in the titles.
+
+### --add-posts
+
+For each entry, it attempts to download a topic-specific rss or atom
+feed and adds each entry in place of the original entry.  This is
+usefull for sites whos forum feed only shows the topics (first post)
+and not any replies.  Note that this option won't work on many sites
+due to having to parse web pages.  Raise issue for any site that
+doesn't seem to work.  Titles on additional posts fetched will all
+be taken from the original entry.
+
+### --auto-links
+
+In the content sections, anything that looks like a URL but is not already
+an HTML link, will be made into a link.
+
+### --output-fmt
+
+Value can be either 'atom' (default), 'rss', or 'summary'.  The
+'summary' options just prints out a few fields in plain text format.
+Used primary for debugging.
+
+### Others
+
+Run feed-filter with the --help option to see what other options
+are available.
+
+
+# Installation
+
+This [package](https://pypi.org/project/feedfilter/) is on [PyPI.org](https://pypi.org/), so just install with pip or pipx like
+
+```
+pipx install feedfilter
+```
+
+# Development setup
+
+It is recommended that you do any development in a virtual
+environment.  If you use direnv, a .envrc file is provided.  You
+should always look it over before allowing it to be used.
+
+poetry is required.  You can install it in your virtual enviroment
+for this project via ```pip install poetry``` or alternatively via
+
+```
+pipx install poetry
+```
+
+Once that is installed, just run
+```
+make install-requirements
+  or
+poetry install
+```
+
+To run feed-filter in development, you should be able to just run
+
+```
+feed-filter <args>
+```
+
+## Building
+
+To create a build (sdist, wheel) run the following
+
+```
+make build
+```
+
+Results will be in the dist/ directory.
+
+# Licensing
+
+This project is licensed under the GNU GPL version 3 or later.  See the
+LICENSE file in the top-level directory.
 
-setup(**setup_kwargs)
```

