# Comparing `tmp/unearth-0.9.0.tar.gz` & `tmp/unearth-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unearth-0.9.0.tar", last modified: Thu Apr  6 05:44:06 2023, max compression
+gzip compressed data, was "unearth-0.9.1.tar", last modified: Mon May 15 07:34:57 2023, max compression
```

## Comparing `unearth-0.9.0.tar` & `unearth-0.9.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1059 2023-04-06 05:43:50.434534 unearth-0.9.0/LICENSE
--rw-r--r--   0        0        0     2885 2023-04-06 05:43:50.434534 unearth-0.9.0/README.md
--rw-r--r--   0        0        0     1919 2023-04-06 05:43:50.438534 unearth-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      616 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/__init__.py
--rw-r--r--   0        0        0     4893 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/__main__.py
--rw-r--r--   0        0        0    13606 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/auth.py
--rw-r--r--   0        0        0     7907 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/collector.py
--rw-r--r--   0        0        0      970 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/errors.py
--rw-r--r--   0        0        0    10841 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/evaluator.py
--rw-r--r--   0        0        0    15178 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/finder.py
--rw-r--r--   0        0        0     5538 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/link.py
--rw-r--r--   0        0        0     5406 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/pep425tags.py
--rw-r--r--   0        0        0    11520 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/preparer.py
--rw-r--r--   0        0        0        0 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/py.typed
--rw-r--r--   0        0        0     6687 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/session.py
--rw-r--r--   0        0        0     6405 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/utils.py
--rw-r--r--   0        0        0      258 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/__init__.py
--rw-r--r--   0        0        0     8415 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/base.py
--rw-r--r--   0        0        0     2589 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/bazaar.py
--rw-r--r--   0        0        0     4813 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/git.py
--rw-r--r--   0        0        0     2006 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/hg.py
--rw-r--r--   0        0        0     6238 2023-04-06 05:43:50.438534 unearth-0.9.0/src/unearth/vcs/svn.py
--rw-r--r--   0        0        0      132 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/__init__.py
--rw-r--r--   0        0        0     2581 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2173 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/app.py
--rw-r--r--   0        0        0    96588 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/files/click-8.1.3-py3-none-any.whl
--rw-r--r--   0        0        0   133101 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
--rw-r--r--   0        0        0      816 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/findlinks/index.html
--rw-r--r--   0        0        0     1860 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/index/black.html
--rw-r--r--   0        0        0      876 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/index/click.html
--rw-r--r--   0        0        0      461 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/index/first.html
--rw-r--r--   0        0        0      964 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/index/pipenv.html
--rw-r--r--   0        0        0     2345 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/json/black.json
--rw-r--r--   0        0        0     1081 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/json/click.json
--rw-r--r--   0        0        0      521 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/json/first.json
--rw-r--r--   0        0        0     1178 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/fixtures/json/pipenv.json
--rw-r--r--   0        0        0     2628 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_collector.py
--rw-r--r--   0        0        0     8229 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_evaluator.py
--rw-r--r--   0        0        0     6341 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_finder.py
--rw-r--r--   0        0        0     4044 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_link.py
--rw-r--r--   0        0        0     3380 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_session.py
--rw-r--r--   0        0        0      558 2023-04-06 05:43:50.438534 unearth-0.9.0/tests/test_utils.py
--rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 unearth-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-15 07:34:42.539511 unearth-0.9.1/LICENSE
+-rw-r--r--   0        0        0     2885 2023-05-15 07:34:42.539511 unearth-0.9.1/README.md
+-rw-r--r--   0        0        0     1919 2023-05-15 07:34:42.539511 unearth-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      616 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/__init__.py
+-rw-r--r--   0        0        0     5993 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/__main__.py
+-rw-r--r--   0        0        0    13606 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/auth.py
+-rw-r--r--   0        0        0     7912 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/collector.py
+-rw-r--r--   0        0        0      970 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/errors.py
+-rw-r--r--   0        0        0    10775 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/evaluator.py
+-rw-r--r--   0        0        0    15178 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/finder.py
+-rw-r--r--   0        0        0     5538 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/link.py
+-rw-r--r--   0        0        0     5406 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/pep425tags.py
+-rw-r--r--   0        0        0    11520 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/preparer.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/py.typed
+-rw-r--r--   0        0        0     6687 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/session.py
+-rw-r--r--   0        0        0     6405 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/utils.py
+-rw-r--r--   0        0        0      258 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/__init__.py
+-rw-r--r--   0        0        0     8415 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/base.py
+-rw-r--r--   0        0        0     2589 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/bazaar.py
+-rw-r--r--   0        0        0     4813 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/git.py
+-rw-r--r--   0        0        0     2006 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/hg.py
+-rw-r--r--   0        0        0     6238 2023-05-15 07:34:42.539511 unearth-0.9.1/src/unearth/vcs/svn.py
+-rw-r--r--   0        0        0      132 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/__init__.py
+-rw-r--r--   0        0        0     2581 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2173 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/app.py
+-rw-r--r--   0        0        0    96588 2023-05-15 07:34:42.539511 unearth-0.9.1/tests/fixtures/files/click-8.1.3-py3-none-any.whl
+-rw-r--r--   0        0        0   133101 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl
+-rw-r--r--   0        0        0      816 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/findlinks/index.html
+-rw-r--r--   0        0        0     1860 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/black.html
+-rw-r--r--   0        0        0      876 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/click.html
+-rw-r--r--   0        0        0      461 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/first.html
+-rw-r--r--   0        0        0      964 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/index/pipenv.html
+-rw-r--r--   0        0        0     2345 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/black.json
+-rw-r--r--   0        0        0     1081 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/click.json
+-rw-r--r--   0        0        0      521 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/first.json
+-rw-r--r--   0        0        0     1178 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/fixtures/json/pipenv.json
+-rw-r--r--   0        0        0     2628 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_collector.py
+-rw-r--r--   0        0        0     8267 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_evaluator.py
+-rw-r--r--   0        0        0     6341 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_finder.py
+-rw-r--r--   0        0        0     4044 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_link.py
+-rw-r--r--   0        0        0     3380 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_session.py
+-rw-r--r--   0        0        0      558 2023-05-15 07:34:42.543511 unearth-0.9.1/tests/test_utils.py
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 unearth-0.9.1/PKG-INFO
```

### Comparing `unearth-0.9.0/LICENSE` & `unearth-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/README.md` & `unearth-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/pyproject.toml` & `unearth-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3 :: Only",
 ]
-version = "0.9.0"
+version = "0.9.1"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/frostming/unearth"
 Documentation = "https://unearth.readthedocs.io"
```

### Comparing `unearth-0.9.0/src/unearth/__init__.py` & `unearth-0.9.1/src/unearth/__init__.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/__main__.py` & `unearth-0.9.1/src/unearth/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,18 +4,18 @@
 import argparse
 import json
 import logging
 import os
 import sys
 import tempfile
 from dataclasses import dataclass
-from typing import cast
 
 from packaging.requirements import Requirement
 
+from unearth.evaluator import TargetPython
 from unearth.finder import PackageFinder
 from unearth.link import Link
 from unearth.utils import splitext
 
 
 @dataclass(frozen=True)
 class CLIArgs:
@@ -26,26 +26,38 @@
     trusted_hosts: list[str]
     no_binary: bool
     only_binary: bool
     prefer_binary: bool
     all: bool
     link_only: bool
     download: str | None
+    py_ver: tuple[int, ...] | None
+    abis: list[str] | None
+    impl: str | None
+    platforms: list[str] | None
 
 
 def _setup_logger(verbosity: bool) -> None:
     logger = logging.getLogger("unearth")
     logger.setLevel(logging.DEBUG if verbosity else logging.WARNING)
     handler = logging.StreamHandler()
     handler.setLevel(logging.DEBUG)
     formatter = logging.Formatter("%(levelname)s: %(message)s")
     handler.setFormatter(formatter)
     logger.addHandler(handler)
 
 
+def comma_split(arg: str) -> list[str]:
+    return arg.split(",")
+
+
+def to_py_ver(arg: str) -> tuple[int, ...]:
+    return tuple(int(i) for i in arg.split(".") if i.isdigit())
+
+
 def cli_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser(
         description="Find and download packages from a PEP 508 requirement string.",
     )
     parser.add_argument(
         "requirement",
         type=Requirement,
@@ -105,34 +117,58 @@
         "--download",
         "-d",
         nargs="?",
         const=".",
         metavar="DIR",
         help="Download the package(s) to DIR.",
     )
+    group = parser.add_argument_group("Target Python options")
+    group.add_argument(
+        "--python-version",
+        "--py",
+        dest="py_ver",
+        type=to_py_ver,
+        help="Target Python version. e.g. 3.11.0",
+    )
+    group.add_argument(
+        "--abis", type=comma_split, help="Comma-separated list of ABIs. e.g. cp39,cp310"
+    )
+    group.add_argument(
+        "--implementation",
+        "--impl",
+        dest="impl",
+        help="Python implementation. e.g. cp,pp,jy,ip",
+    )
+    group.add_argument(
+        "--platforms",
+        type=comma_split,
+        help="Comma-separated list of platforms. e.g. win_amd64,linux_x86_64",
+    )
     return parser
 
 
 def get_dest_for_package(dest: str, link: Link) -> str:
     if link.is_wheel:
         return dest
     filename = link.filename.rsplit("@", 1)[0]
     fn, _ = splitext(filename)
     return os.path.join(dest, fn)
 
 
 def cli(argv: list[str] | None = None) -> None:
     parser = cli_parser()
-    args = cast(CLIArgs, parser.parse_args(argv))
+    args = CLIArgs(**vars(parser.parse_args(argv)))
     _setup_logger(args.verbose)
     name = args.requirement.name
+    target_python = TargetPython(args.py_ver, args.abis, args.impl, args.platforms)
     finder = PackageFinder(
         index_urls=args.index_urls or ["https://pypi.org/simple/"],
         find_links=args.find_links or [],
         trusted_hosts=args.trusted_hosts or [],
+        target_python=target_python,
         no_binary=[name] if args.no_binary else [],
         only_binary=[name] if args.only_binary else [],
         prefer_binary=[name] if args.prefer_binary else [],
         verbosity=int(args.verbose),
     )
     matches = list(finder.find_matches(args.requirement))
     if not matches:
```

### Comparing `unearth-0.9.0/src/unearth/auth.py` & `unearth-0.9.1/src/unearth/auth.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/collector.py` & `unearth-0.9.1/src/unearth/collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,15 +86,15 @@
         url = file.get("url")
         if not url:
             continue
         url = parse.urljoin(base_url, url)
         requires_python: str | None = file.get("requires-python")
         yank_reason: str | None = file.get("yanked") or None
         dist_info_metadata: bool | dict[str, str] | None = file.get(
-            "dist-info-metadata"
+            "data-dist-info-metadata"
         )
         hashes: dict[str, str] | None = file.get("hashes")
         yield Link(
             url,
             base_url,
             yank_reason=yank_reason,
             requires_python=requires_python,
```

### Comparing `unearth-0.9.0/src/unearth/errors.py` & `unearth-0.9.1/src/unearth/errors.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/evaluator.py` & `unearth-0.9.1/src/unearth/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,18 +278,17 @@
     if requirement.name:
         if canonicalize_name(package.name) != canonicalize_name(requirement.name):
             logger.debug(
                 "Skipping package %s: name doesn't match %s", package, requirement.name
             )
             return False
 
-    if requirement.specifier and package.version:
-        if not requirement.specifier.contains(
-            package.version, prereleases=allow_prereleases
-        ):
-            logger.debug(
-                "Skipping package %s: version doesn't match %s",
-                package,
-                requirement.specifier,
-            )
-            return False
+    if package.version and not requirement.specifier.contains(
+        package.version, prereleases=allow_prereleases
+    ):
+        logger.debug(
+            "Skipping package %s: version doesn't match %s",
+            package,
+            requirement.specifier,
+        )
+        return False
     return True
```

### Comparing `unearth-0.9.0/src/unearth/finder.py` & `unearth-0.9.1/src/unearth/finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/link.py` & `unearth-0.9.1/src/unearth/link.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/pep425tags.py` & `unearth-0.9.1/src/unearth/pep425tags.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/preparer.py` & `unearth-0.9.1/src/unearth/preparer.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/session.py` & `unearth-0.9.1/src/unearth/session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/utils.py` & `unearth-0.9.1/src/unearth/utils.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/vcs/base.py` & `unearth-0.9.1/src/unearth/vcs/base.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/vcs/bazaar.py` & `unearth-0.9.1/src/unearth/vcs/bazaar.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/vcs/git.py` & `unearth-0.9.1/src/unearth/vcs/git.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/vcs/hg.py` & `unearth-0.9.1/src/unearth/vcs/hg.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/src/unearth/vcs/svn.py` & `unearth-0.9.1/src/unearth/vcs/svn.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/conftest.py` & `unearth-0.9.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/app.py` & `unearth-0.9.1/tests/fixtures/app.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/files/click-8.1.3-py3-none-any.whl` & `unearth-0.9.1/tests/fixtures/files/click-8.1.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl` & `unearth-0.9.1/tests/fixtures/findlinks/Jinja2-3.1.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/findlinks/index.html` & `unearth-0.9.1/tests/fixtures/findlinks/index.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/index/black.html` & `unearth-0.9.1/tests/fixtures/index/black.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/index/click.html` & `unearth-0.9.1/tests/fixtures/index/click.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/index/pipenv.html` & `unearth-0.9.1/tests/fixtures/index/pipenv.html`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/json/black.json` & `unearth-0.9.1/tests/fixtures/json/black.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/json/click.json` & `unearth-0.9.1/tests/fixtures/json/click.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/json/first.json` & `unearth-0.9.1/tests/fixtures/json/first.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/fixtures/json/pipenv.json` & `unearth-0.9.1/tests/fixtures/json/pipenv.json`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/test_collector.py` & `unearth-0.9.1/tests/test_collector.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/test_evaluator.py` & `unearth-0.9.1/tests/test_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     "version,requires,allow_prereleases,expected",
     [
         ("8.1.3", ">=8.0", None, True),
         ("7.1", ">=8.0", None, False),
         ("8.0.0a0", ">=8.0.0dev0", None, True),
         ("8.0.0dev0", ">=7", None, False),
         ("8.0.0dev0", ">=7", True, True),
+        ("8.0.0a0", "", None, False),
         ("8.0.0a0", ">=8.0.0dev0", False, False),
     ],
 )
 def test_evaluate_packages_matching_version(
     version, requires, allow_prereleases, expected
 ):
     requirement = Requirement(f"click{requires}")
```

### Comparing `unearth-0.9.0/tests/test_finder.py` & `unearth-0.9.1/tests/test_finder.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/test_link.py` & `unearth-0.9.1/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/test_session.py` & `unearth-0.9.1/tests/test_session.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/tests/test_utils.py` & `unearth-0.9.1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unearth-0.9.0/PKG-INFO` & `unearth-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unearth
-Version: 0.9.0
+Version: 0.9.1
 Summary: A utility to fetch and download python packages
 License: MIT
 Author-email: Frost Ming <me@frostming.com>
 Requires-Python: >=3.7
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

