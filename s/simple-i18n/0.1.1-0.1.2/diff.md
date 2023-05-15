# Comparing `tmp/simple-i18n-0.1.1.tar.gz` & `tmp/simple-i18n-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple-i18n-0.1.1.tar", last modified: Sat Dec 31 10:23:17 2022, max compression
+gzip compressed data, was "simple-i18n-0.1.2.tar", last modified: Mon May 15 15:19:02 2023, max compression
```

## Comparing `simple-i18n-0.1.1.tar` & `simple-i18n-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-12-31 10:23:17.454002 simple-i18n-0.1.1/
--rw-rw-rw-   0        0        0     1378 2022-12-31 10:23:17.452012 simple-i18n-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      560 2022-12-31 09:20:46.000000 simple-i18n-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2022-12-31 10:23:17.454002 simple-i18n-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1058 2022-12-31 10:22:11.000000 simple-i18n-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-31 10:23:17.414663 simple-i18n-0.1.1/simple_i18n/
--rw-rw-rw-   0        0        0    45388 2022-12-31 10:22:11.000000 simple-i18n-0.1.1/simple_i18n/I18n.py
--rw-rw-rw-   0        0        0       44 2022-12-31 08:24:58.000000 simple-i18n-0.1.1/simple_i18n/__init__.py
-drwxrwxrwx   0        0        0        0 2022-12-31 10:23:17.447004 simple-i18n-0.1.1/simple_i18n.egg-info/
--rw-rw-rw-   0        0        0     1378 2022-12-31 10:23:17.000000 simple-i18n-0.1.1/simple_i18n.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2022-12-31 10:23:17.000000 simple-i18n-0.1.1/simple_i18n.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-31 10:23:17.000000 simple-i18n-0.1.1/simple_i18n.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-12-31 10:23:17.000000 simple-i18n-0.1.1/simple_i18n.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2022-12-31 10:23:17.000000 simple-i18n-0.1.1/simple_i18n.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-12-31 10:15:37.000000 simple-i18n-0.1.1/simple_i18n.egg-info/zip-safe
-drwxrwxrwx   0        0        0        0 2022-12-31 10:23:17.449002 simple-i18n-0.1.1/test/
--rw-rw-rw-   0        0        0     3008 2022-12-31 09:48:38.000000 simple-i18n-0.1.1/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-15 15:19:02.571244 simple-i18n-0.1.2/
+-rw-rw-rw-   0        0        0     1378 2023-05-15 15:19:02.569280 simple-i18n-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      560 2022-12-31 09:55:18.000000 simple-i18n-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-15 15:19:02.571244 simple-i18n-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1061 2023-05-15 15:18:49.000000 simple-i18n-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-15 15:19:02.524271 simple-i18n-0.1.2/simple_i18n/
+-rw-rw-rw-   0        0        0    47671 2023-05-15 15:12:39.000000 simple-i18n-0.1.2/simple_i18n/I18n.py
+-rw-rw-rw-   0        0        0       44 2022-12-31 09:55:18.000000 simple-i18n-0.1.2/simple_i18n/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-15 15:19:02.567281 simple-i18n-0.1.2/simple_i18n.egg-info/
+-rw-rw-rw-   0        0        0     1378 2023-05-15 15:19:02.000000 simple-i18n-0.1.2/simple_i18n.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-05-15 15:19:02.000000 simple-i18n-0.1.2/simple_i18n.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-15 15:19:02.000000 simple-i18n-0.1.2/simple_i18n.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-15 15:19:02.000000 simple-i18n-0.1.2/simple_i18n.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-15 15:19:02.000000 simple-i18n-0.1.2/simple_i18n.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 15:17:07.000000 simple-i18n-0.1.2/simple_i18n.egg-info/zip-safe
```

### Comparing `simple-i18n-0.1.1/PKG-INFO` & `simple-i18n-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-i18n
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/iDkGK/simple-i18n
 Author: iDkGK
 Author-email: 1444807655@qq.com
 Maintainer: iDkGK
 Maintainer-email: 1444807655@qq.com
 License: MIT
 Keywords: i18n,gettext,translation
```

### Comparing `simple-i18n-0.1.1/README.md` & `simple-i18n-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `simple-i18n-0.1.1/simple_i18n/I18n.py` & `simple-i18n-0.1.2/simple_i18n/I18n.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,113 +1,106 @@
-__all__ = ['I18n']
-__title__ = 'simple-i18n'
-__description__ = 'Lightweight simple translation JavaScript module \'i18n\' in Python implementation.'
-__url__ = 'https://github.com/iDkGK/simple-i18n'
-__version__ = '0.1.1'
-__author__ = 'iDkGK'
-__author_email__ = '1444807655@qq.com'
-__license__ = 'MIT'
+__all__ = ["I18n"]
+__title__ = "simple-i18n"
+__description__ = (
+    "Lightweight simple translation JavaScript module 'i18n' in Python implementation."
+)
+__url__ = "https://github.com/iDkGK/simple-i18n"
+__version__ = "0.1.1"
+__author__ = "iDkGK"
+__author_email__ = "1444807655@qq.com"
+__license__ = "MIT"
 
 
 # dependencies
 import functools
 import inspect
 import json
 import logging
 import math
 import os
 import pystache
 import re
 import shutil
 import stat
 from threading import Lock
-from typing import (
-    Any,
-    Callable,
-    overload,
-    NotRequired,
-    TypedDict
-)
-from types import (
-    FunctionType,
-    ModuleType
-)
+from typing import Any, Callable, overload, Optional, TypedDict
+from types import FunctionType, ModuleType
 from watchdog.observers import Observer
 from watchdog.events import FileSystemEventHandler
 
+
 # type hinting
 class _MustacheConfigT(TypedDict):
-    tags: NotRequired[list[str]]
-    disable: NotRequired[bool]
+    tags: Optional[list[str]]
+    disable: Optional[bool]
+
 
 class _OptionType(TypedDict):
-    locales: NotRequired[list[str]]
-    fallbacks: NotRequired[dict[str, str]]
-    defaultLocale: NotRequired[str]
-    retryInDefaultLocale: NotRequired[bool]
-    cookie: NotRequired[str]
-    header: NotRequired[str]
-    queryParameter: NotRequired[str]
-    directory: NotRequired[str]
-    directoryPermissions: NotRequired[str]
-    autoReload: NotRequired[bool]
-    updateFiles: NotRequired[bool]
-    syncFiles: NotRequired[bool]
-    indent: NotRequired[str]
-    extension: NotRequired[str]
-    prefix: NotRequired[str]
-    objectNotation: NotRequired[bool]
-    logDebugFn: NotRequired[Callable[[str], None]]
-    logWarnFn: NotRequired[Callable[[str], None]]
-    logErrorFn: NotRequired[Callable[[str], None]]
-    missingKeyFn: NotRequired[Callable[[str, str], str]]
-    register: NotRequired[dict[str, Any]]
-    api: NotRequired[dict[str, str]]
-    preserveLegacyCase: NotRequired[bool]
-    staticCatalog: NotRequired[dict[str, dict[str, dict[str, str]]]]
-    mustacheConfig: NotRequired[_MustacheConfigT]
-    parser: NotRequired[ModuleType | Any]
+    locales: Optional[list[str]]
+    fallbacks: Optional[dict[str, str]]
+    defaultLocale: Optional[str]
+    retryInDefaultLocale: Optional[bool]
+    cookie: Optional[str]
+    header: Optional[str]
+    queryParameter: Optional[str]
+    directory: Optional[str]
+    directoryPermissions: Optional[str]
+    autoReload: Optional[bool]
+    updateFiles: Optional[bool]
+    syncFiles: Optional[bool]
+    indent: Optional[str]
+    extension: Optional[str]
+    prefix: Optional[str]
+    objectNotation: Optional[bool]
+    logDebugFn: Optional[Callable[[str], None]]
+    logWarnFn: Optional[Callable[[str], None]]
+    logErrorFn: Optional[Callable[[str], None]]
+    missingKeyFn: Optional[Callable[[str, str], str]]
+    register: Optional[dict[str, Any]]
+    api: Optional[dict[str, str]]
+    preserveLegacyCase: Optional[bool]
+    staticCatalog: Optional[dict[str, dict[str, dict[str, str]]]]
+    mustacheConfig: Optional[_MustacheConfigT]
+    parser: Optional[ModuleType | Any]
+
 
 # create constructor function
 def I18n(_OPTS: _OptionType = False):
-    '''Create and return an I18n singleton
+    """Create and return an I18n singleton
 
     Create an I18n singleton according to user-provided options and return the singleton.\n
     User can create as many as possible since the base class is locally defined.
 
     Args:
         _OPTS: A dict including user-provided options.
 
     Returns:
         An I18n singleton with user-provided options applied to itself.
 
     Raises:
         NotImplementedError: ...
         FileExistsError: ...
-    '''
+    """
     MessageformatInstanceForLocale = {}
     PluralsForLocale = {}
     locales = {}
     api = {
-        '__': '__',
-        '__n': '__n',
-        '__l': '__l',
-        '__h': '__h',
-        '__mf': '__mf',
-        'getLocale': 'getLocale',
-        'setLocale': 'setLocale',
-        'getCatalog': 'getCatalog',
-        'getLocales': 'getLocales',
-        'addLocale': 'addLocale',
-        'removeLocale': 'removeLocale'
-    }
-    mustacheConfig = {
-        'tags': ['{{', '}}'],
-        'disable': False
+        "__": "__",
+        "__n": "__n",
+        "__l": "__l",
+        "__h": "__h",
+        "__mf": "__mf",
+        "getLocale": "getLocale",
+        "setLocale": "setLocale",
+        "getCatalog": "getCatalog",
+        "getLocales": "getLocales",
+        "addLocale": "addLocale",
+        "removeLocale": "removeLocale",
     }
+    mustacheConfig = {"tags": ["{{", "}}"], "disable": False}
     mustacheRegex = None
     pathsep = os.path.sep
     autoReload = False
     cookiename = None
     languageHeaderName = None
     defaultLocale = None
     retryInDefaultLocale = False
@@ -128,211 +121,280 @@
     syncFiles = False
     missingKeyFn = None
     parser = None
 
     # public exports
     i18n = {}
 
-    i18n['version'] = '0.1.1'
+    i18n["version"] = "0.1.1"
 
     def i18nConfigure(opt=_OPTS, *args, **kwargs):
         # access variables from upper function
         nonlocal locales, api, mustacheConfig, mustacheRegex, autoReload, cookiename, languageHeaderName, defaultLocale, retryInDefaultLocale, directory, directoryPermissions, extension, fallbacks, indent, logDebugFn, logErrorFn, logWarnFn, preserveLegacyCase, objectNotation, prefix, queryParameter, register, updateFiles, syncFiles, missingKeyFn, parser
 
         # reset locales
         locales = {}
 
         # Provide custom API method aliases if desired
         # This needs to be processed before the first call to applyAPItoObject()
-        if checkValues(opt, ['api', dict]):
-            for method in opt['api']:
-                alias = opt['api'][method]
+        if checkValues(opt, ["api", dict]):
+            for method in opt["api"]:
+                alias = opt["api"][method]
                 if checkValues(api, method):
                     api[method] = alias
 
         # you may register i18n in global scope, up to you
-        if checkValues(opt, ['register', dict, list]):
-            register = opt['register']
+        if checkValues(opt, ["register", dict, list]):
+            register = opt["register"]
             # or give an array objects to register to
-            if type(opt['register']) is list:
-                register = opt['register']
+            if type(opt["register"]) is list:
+                register = opt["register"]
                 for method in register:
                     applyAPItoObject(method)
             else:
-                applyAPItoObject(opt['register'])
+                applyAPItoObject(opt["register"])
 
         # sets a custom cookie name to parse locale settings from
-        cookiename = opt['cookie'] if checkValues(opt, ['cookie', str]) else None
+        cookiename = opt["cookie"] if checkValues(opt, ["cookie", str]) else None
 
         # set the custom header name to extract the language locale
-        languageHeaderName = opt['header'] if checkValues(opt, ['header', str]) else 'accept-language'
+        languageHeaderName = (
+            opt["header"] if checkValues(opt, ["header", str]) else "accept-language"
+        )
 
         # query-string parameter to be watched - @todo: add test & doc
-        queryParameter = opt['queryParameter'] if checkValues(opt, ['queryParameter', str]) else None
+        queryParameter = (
+            opt["queryParameter"] if checkValues(opt, ["queryParameter", str]) else None
+        )
 
         # where to store json files
-        directory = opt['directory'] if checkValues(opt, ['directory', str]) else os.path.join(os.getcwd(), 'locales')
+        directory = (
+            opt["directory"]
+            if checkValues(opt, ["directory", str])
+            else os.path.join(os.getcwd(), "locales")
+        )
 
         # permissions when creating new directories
-        directoryPermissions = int(opt['directoryPermissions'], 8) if checkValues(opt, ['directoryPermissions', str]) else None
+        directoryPermissions = (
+            int(opt["directoryPermissions"], 8)
+            if checkValues(opt, ["directoryPermissions", str])
+            else None
+        )
 
         # write new locale information to disk
-        updateFiles = opt['updateFiles'] if checkValues(opt, ['updateFiles', bool]) else True
+        updateFiles = (
+            opt["updateFiles"] if checkValues(opt, ["updateFiles", bool]) else True
+        )
 
         # sync locale information accros all files
-        syncFiles = opt['syncFiles'] if checkValues(opt, ['syncFiles', bool]) else False
+        syncFiles = opt["syncFiles"] if checkValues(opt, ["syncFiles", bool]) else False
 
         # what to use as the indentation unit (ex: '\t', '  ')
-        indent = opt['indent'] if checkValues(opt, ['indent', str]) else '\t'
+        indent = opt["indent"] if checkValues(opt, ["indent", str]) else "\t"
 
         # json files prefix
-        prefix = opt['prefix'] if checkValues(opt, ['prefix', str]) else ''
+        prefix = opt["prefix"] if checkValues(opt, ["prefix", str]) else ""
 
         # where to store json files
-        extension = opt['extension'] if checkValues(opt, ['extension', str]) else '.json'
+        extension = (
+            opt["extension"] if checkValues(opt, ["extension", str]) else ".json"
+        )
 
         # setting defaultLocale
-        defaultLocale = opt['defaultLocale'] if checkValues(opt, ['defaultLocale', str]) else 'en'
+        defaultLocale = (
+            opt["defaultLocale"] if checkValues(opt, ["defaultLocale", str]) else "en"
+        )
 
         # allow to retry in default locale, useful for production
-        retryInDefaultLocale = opt['retryInDefaultLocale'] if checkValues(opt, ['retryInDefaultLocale', bool]) else False
+        retryInDefaultLocale = (
+            opt["retryInDefaultLocale"]
+            if checkValues(opt, ["retryInDefaultLocale", bool])
+            else False
+        )
 
         # auto reload locale files when changed
-        autoReload = opt['autoReload'] if checkValues(opt, ['autoReload', bool]) else False
+        autoReload = (
+            opt["autoReload"] if checkValues(opt, ["autoReload", bool]) else False
+        )
 
         # enable object notation?
-        objectNotation = opt['objectNotation'] if checkValues(opt, 'objectNotation') else False
+        objectNotation = (
+            opt["objectNotation"] if checkValues(opt, "objectNotation") else False
+        )
         if objectNotation == True:
-            objectNotation = '.'
+            objectNotation = "."
 
         # read language fallback map
-        fallbacks = opt['fallbacks'] if checkValues(opt, ['fallbacks', dict]) else {}
+        fallbacks = opt["fallbacks"] if checkValues(opt, ["fallbacks", dict]) else {}
 
         # setting custom logger functions
         logging.basicConfig(level=logging.CRITICAL)
         logger = logging.getLogger(__name__)
-        logDebugFn = opt['logDebugFn'] if checkValues(opt, ['logDebugFn', FunctionType]) else logger.debug
-        logWarnFn = opt['logWarnFn'] if checkValues(opt, ['logWarnFn', FunctionType]) else logger.warning
-        logErrorFn = opt['logErrorFn'] if checkValues(opt, ['logErrorFn', FunctionType]) else logger.error
-        preserveLegacyCase = opt['preserveLegacyCase'] if checkValues(opt, ['preserveLegacyCase', bool]) else True
+        logDebugFn = (
+            opt["logDebugFn"]
+            if checkValues(opt, ["logDebugFn", FunctionType])
+            else logger.debug
+        )
+        logWarnFn = (
+            opt["logWarnFn"]
+            if checkValues(opt, ["logWarnFn", FunctionType])
+            else logger.warning
+        )
+        logErrorFn = (
+            opt["logErrorFn"]
+            if checkValues(opt, ["logErrorFn", FunctionType])
+            else logger.error
+        )
+        preserveLegacyCase = (
+            opt["preserveLegacyCase"]
+            if checkValues(opt, ["preserveLegacyCase", bool])
+            else True
+        )
 
         # setting custom missing key function
-        missingKeyFn = opt['missingKeyFn'] if checkValues(opt, ['missingKeyFn', FunctionType]) else missingKey
-        parser = opt['parser'] if checkValues(opt, 'parser') and hasattr(opt['parser'], 'loads') and hasattr(opt['parser'], 'dumps') else json
+        missingKeyFn = (
+            opt["missingKeyFn"]
+            if checkValues(opt, ["missingKeyFn", FunctionType])
+            else missingKey
+        )
+        parser = (
+            opt["parser"]
+            if checkValues(opt, "parser")
+            and hasattr(opt["parser"], "loads")
+            and hasattr(opt["parser"], "dumps")
+            else json
+        )
 
         # when missing locales we try to guess that from directory
-        opt['locales'] = list(opt['staticCatalog'].keys()) if checkValues(opt, 'staticCatalog') else opt['locales'] if checkValues(opt, 'locales') else guessLocales(directory)
+        opt["locales"] = (
+            list(opt["staticCatalog"].keys())
+            if checkValues(opt, "staticCatalog")
+            else opt["locales"]
+            if checkValues(opt, "locales")
+            else guessLocales(directory)
+        )
 
         # some options should be disabled when using staticCatalog
-        if checkValues(opt, 'staticCatalog'):
+        if checkValues(opt, "staticCatalog"):
             updateFiles = False
             autoReload = False
             syncFiles = False
 
         # customize mustache parsing
-        if checkValues(opt, 'mustacheConfig'):
-            if checkValues(opt['mustacheConfig'], ['tags', list]):
-                mustacheConfig['tags'] = opt['mustacheConfig']['tags']
-            if checkValues(opt['mustacheConfig'], 'disable') and opt['mustacheConfig']['disable'] == True:
-                mustacheConfig['disable'] = True
+        if checkValues(opt, "mustacheConfig"):
+            if checkValues(opt["mustacheConfig"], ["tags", list]):
+                mustacheConfig["tags"] = opt["mustacheConfig"]["tags"]
+            if (
+                checkValues(opt["mustacheConfig"], "disable")
+                and opt["mustacheConfig"]["disable"] == True
+            ):
+                mustacheConfig["disable"] = True
 
-        [start, end] = mustacheConfig['tags']
-        mustacheRegex = re.compile(rf'{escapeRegExp(start)}.*{escapeRegExp(end)}')
+        [start, end] = mustacheConfig["tags"]
+        mustacheRegex = re.compile(rf"{escapeRegExp(start)}.*{escapeRegExp(end)}")
 
         # implicitly read all locales
-        if checkValues(opt, ['locales', list]):
-            if checkValues(opt, 'staticCatalog'):
-                locales = opt['staticCatalog']
+        if checkValues(opt, ["locales", list]):
+            if checkValues(opt, "staticCatalog"):
+                locales = opt["staticCatalog"]
             else:
-                for locale in opt['locales']:
+                for locale in opt["locales"]:
                     read(locale)
 
             # auto reload locale files when changed
             if autoReload:
                 # watch changes of locale files (it's called twice because watchFiles is still unstable)
                 def handler(event):
                     # access variables from upper function
                     nonlocal opt
 
                     filename = os.path.basename(event.src_path)
                     localeFromFile = guessLocaleFromFile(filename)
 
-                    if localeFromFile and checkValues(opt['locales'], localeFromFile) and opt['locales'].index(localeFromFile) > -1:
-                        logDebug(f'Auto reloading locale file \'{filename}\'.')
+                    if (
+                        localeFromFile
+                        and checkValues(opt["locales"], localeFromFile)
+                        and opt["locales"].index(localeFromFile) > -1
+                    ):
+                        logDebug(f"Auto reloading locale file '{filename}'.")
                         read(localeFromFile)
+
                 watchFiles(directory, handler)
 
-    i18n['configure'] = i18nConfigure
+    i18n["configure"] = i18nConfigure
 
     def i18nInit(request, response, next, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['init'] = i18nInit
+    i18n["init"] = i18nInit
 
     def i18nTranslate(phrase=None, *args, **kwargs):
         # access variables from upper function
         nonlocal i18n
 
         msg = None
         argv = parseArgv(getArgsList(dict(locals().items()), i18nTranslate))
         namedValues = argv[0]
         arguments = argv[1]
 
         # called like __({phrase: 'Hello', locale: 'en'})
         if type(phrase) is dict:
-            if (checkValues(phrase, ['locale', str]) and
-                checkValues(phrase, ['phrase', str])):
-                msg = translate(phrase['locale'], phrase['phrase'])
+            if checkValues(phrase, ["locale", str]) and checkValues(
+                phrase, ["phrase", str]
+            ):
+                msg = translate(phrase["locale"], phrase["phrase"])
         # called like __('Hello')
         else:
             # get translated message with locale from scope (deprecated) or object
             msg = translate(getLocaleFromObject(i18n), phrase)
 
         # postprocess to get compatible to plurals
-        if (type(msg) is dict or type(msg) is list) and checkValues(msg, 'one'):
-            msg = msg['one']
+        if (type(msg) is dict or type(msg) is list) and checkValues(msg, "one"):
+            msg = msg["one"]
 
         # in case there is no 'one' but an 'other' rule
-        if (type(msg) is dict or type(msg) is list) and checkValues(msg, 'other'):
-            msg = msg['other']
+        if (type(msg) is dict or type(msg) is list) and checkValues(msg, "other"):
+            msg = msg["other"]
 
         # head over to postProcessing
         return postProcess(msg, namedValues, arguments)
 
-    i18n['__'] = i18nTranslate
+    i18n["__"] = i18nTranslate
 
     def i18nMessageformat(phrase, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['__mf'] = i18nMessageformat
+    i18n["__mf"] = i18nMessageformat
 
     def i18nTranslationList(phrase, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['__l'] = i18nTranslationList
+    i18n["__l"] = i18nTranslationList
 
     def i18nTranslationHash(phrase, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['__h'] = i18nTranslationHash
+    i18n["__h"] = i18nTranslationHash
 
     def i18nTranslatePlural(singular, plural, count, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['__n'] = i18nTranslatePlural
+    i18n["__n"] = i18nTranslatePlural
 
-    def i18nSetLocale(obj=None, locale=None, skipImplicitObjects=False, *args, **kwargs):
+    def i18nSetLocale(
+        obj=None, locale=None, skipImplicitObjects=False, *args, **kwargs
+    ):
         # access variables from upper function
         nonlocal i18n, locales, defaultLocale, fallbacks, register
 
         # when given an array of objects => setLocale on each
         if type(obj) is list and type(locale) is str:
             for i in range(len(obj), 0, -1):
-                i18n['setLocale'](obj[i], locale, True)
-            return i18n['getLocale'](obj[0])
+                i18n["setLocale"](obj[i], locale, True)
+            return i18n["getLocale"](obj[0])
 
         # defaults to called like i18n.setLocale(req, 'en')
         targetObject = obj
         targetLocale = locale
 
         # called like req.setLocale('en') or i18n.setLocale('en')
         if locale is None and type(obj) is str:
@@ -340,121 +402,131 @@
             targetLocale = obj
 
         # consider a fallback
         if checkValues(locales, targetLocale):
             targetLocale = getFallback(targetLocale, fallbacks) or targetLocale
 
         # now set locale on object
-        targetObject['locale'] = targetLocale if checkValues(locales, targetLocale) else defaultLocale
+        targetObject["locale"] = (
+            targetLocale if checkValues(locales, targetLocale) else defaultLocale
+        )
 
         # consider any extra registered objects
         if type(register) is dict or type(register) is list:
             if type(register) is list and not skipImplicitObjects:
                 for r in register:
-                    r['locale'] = targetObject['locale']
+                    r["locale"] = targetObject["locale"]
             else:
-                register['locale'] = targetObject['locale']
+                register["locale"] = targetObject["locale"]
 
         # consider res
-        if checkValues(targetObject, 'res') and not skipImplicitObjects:
+        if checkValues(targetObject, "res") and not skipImplicitObjects:
             # escape recursion
             # @see  - https://github.com/balderdashy/sails/pull/3631
             #       - https://github.com/mashpie/i18n-node/pull/218.
-            if checkValues(targetObject['res'], 'locals'):
-                i18n['setLocale'](targetObject['res'], targetObject['locale'], True)
-                i18n['setLocale'](targetObject['res']['locals'], targetObject['locale'], True)
+            if checkValues(targetObject["res"], "locals"):
+                i18n["setLocale"](targetObject["res"], targetObject["locale"], True)
+                i18n["setLocale"](
+                    targetObject["res"]["locals"], targetObject["locale"], True
+                )
             else:
-                i18n['setLocale'](targetObject['res'], targetObject['locale'])
+                i18n["setLocale"](targetObject["res"], targetObject["locale"])
 
         # consider locals
-        if checkValues(targetObject, 'locals') and not skipImplicitObjects:
+        if checkValues(targetObject, "locals") and not skipImplicitObjects:
             # escape recursion
             # @see  - https://github.com/balderdashy/sails/pull/3631
             #       - https://github.com/mashpie/i18n-node/pull/218
-            if checkValues(targetObject['locals'], 'res'):
-                i18n['setLocale'](targetObject['locals'], targetObject['locale'], True)
-                i18n['setLocale'](targetObject['locals']['res'], targetObject['locale'], True)
+            if checkValues(targetObject["locals"], "res"):
+                i18n["setLocale"](targetObject["locals"], targetObject["locale"], True)
+                i18n["setLocale"](
+                    targetObject["locals"]["res"], targetObject["locale"], True
+                )
             else:
-                i18n['setLocale'](targetObject['locals'], targetObject['locale'])
+                i18n["setLocale"](targetObject["locals"], targetObject["locale"])
 
-        return i18n['getLocale'](targetObject)
+        return i18n["getLocale"](targetObject)
 
-    i18n['setLocale'] = i18nSetLocale
+    i18n["setLocale"] = i18nSetLocale
 
     def i18nGetLocale(request, *args, **kwargs):
         # access variables from upper function
         nonlocal i18n, defaultLocale
 
         # called like i18n.getLocale(req)
-        if type(request) is dict and checkValues(request, 'locale'):
-            return request['locale']
+        if type(request) is dict and checkValues(request, "locale"):
+            return request["locale"]
 
         # called like req.getLocale()
-        return i18n['locale'] or defaultLocale
+        return i18n["locale"] or defaultLocale
 
-    i18n['getLocale'] = i18nGetLocale
+    i18n["getLocale"] = i18nGetLocale
 
     def i18nGetCatalog(obj, locale, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['getCatalog'] = i18nGetCatalog
+    i18n["getCatalog"] = i18nGetCatalog
 
     def i18nGetLocales(*args, **kwargs):
         raise NotImplementedError
 
-    i18n['getLocales'] = i18nGetLocales
+    i18n["getLocales"] = i18nGetLocales
 
     def i18nAddLocale(locale, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['addLocale'] = i18nAddLocale
+    i18n["addLocale"] = i18nAddLocale
 
     def i18nRemoveLocale(locale, *args, **kwargs):
         raise NotImplementedError
 
-    i18n['removeLocale'] = i18nRemoveLocale
+    i18n["removeLocale"] = i18nRemoveLocale
 
     # ===================
     # = private methods =
     # ===================
 
-    def postProcess(msg=None, namedValues=None, arguments=[], count=None, *args, **kwargs):
+    def postProcess(
+        msg=None, namedValues=None, arguments=[], count=None, *args, **kwargs
+    ):
         # access variables from upper function
         nonlocal mustacheConfig, mustacheRegex
 
         # in case msg is None
         if msg is None:
             return msg
 
         # test for parsable interval string
-        if re.compile(r'\|').search(msg):
+        if re.compile(r"\|").search(msg):
             msg = parsePluralInterval(msg, count)
 
         # replace the counter
         if type(count) is int:
             msg = msg % count
 
         # if the msg string contains {{Mustache}} patterns we render it as a mini template
-        if not mustacheConfig['disable'] and mustacheRegex.search(msg):
-            pystache.defaults.DELIMITERS = tuple(mustacheConfig['tags'])
-            msg = pystache.render(msg, namedValues, partials = {})
+        if not mustacheConfig["disable"] and mustacheRegex.search(msg):
+            pystache.defaults.DELIMITERS = tuple(mustacheConfig["tags"])
+            msg = pystache.render(msg, namedValues, partials={})
 
         # if we have extra arguments with values to get replaced,
         # an additional substition injects those strings afterwards
-        if re.compile(r'%').search(msg) and arguments and len(arguments) > 0:
+        if re.compile(r"%").search(msg) and arguments and len(arguments) > 0:
             msg = msg % tuple(arguments)
 
         return msg
 
     def argsEndWithNamedObject(arguments=[], *args, **kwargs):
         return (
-            len(arguments) > 1 and
-            arguments[len(arguments) - 1] is not None and
-            (type(arguments[len(arguments) - 1]) is dict or 
-             type(arguments[len(arguments) - 1]) is list)
+            len(arguments) > 1
+            and arguments[len(arguments) - 1] is not None
+            and (
+                type(arguments[len(arguments) - 1]) is dict
+                or type(arguments[len(arguments) - 1]) is list
+            )
         )
 
     def parseArgv(arguments=[], *args, **kwargs):
         if argsEndWithNamedObject(arguments):
             namedValues = arguments[len(arguments) - 1]
             returnArgs = arguments[1:-1]
         else:
@@ -475,194 +547,216 @@
 
             # be kind rewind, or better not touch anything already existing
             if not checkValues(obj, alias):
                 alreadySetted = False
                 obj[alias] = i18n[method]
 
         # set initial locale if not set
-        if checkValues(obj, 'locale'):
-            obj['locale'] = defaultLocale
+        if checkValues(obj, "locale"):
+            obj["locale"] = defaultLocale
 
         # escape recursion
         if alreadySetted:
             return
 
         # attach to response if present (ie. in express)
-        if checkValues(obj, 'res'):
-            applyAPItoObject(obj['res'])
+        if checkValues(obj, "res"):
+            applyAPItoObject(obj["res"])
 
         # attach to locals if present (ie. in express)
-        if checkValues(obj, 'locals'):
-            applyAPItoObject(obj['locals'])
+        if checkValues(obj, "locals"):
+            applyAPItoObject(obj["locals"])
 
     def guessLocales(dir=None, *args, **kwargs):
         entries = os.listdir(dir)
         localesFound = []
 
         for i in range(len(entries), 0, -1):
-            if re.compile(r'^\.').search(entries[i]):
+            if re.compile(r"^\.").search(entries[i]):
                 continue
             localeFromFile = guessLocaleFromFile(entries[i])
             if localeFromFile:
                 localesFound.append(localeFromFile)
 
         return sorted(localesFound)
 
     def guessLocaleFromFile(filename=None, *args, **kwargs):
         # access variables from upper function
         nonlocal extension, prefix
 
-        extensionRegex = re.compile(rf'{extension}$')
-        prefixRegex = re.compile(rf'^{prefix}')
+        extensionRegex = re.compile(rf"{extension}$")
+        prefixRegex = re.compile(rf"^{prefix}")
 
         if not filename:
             return False
         if prefix and not prefixRegex.search(filename):
             return False
         if extension and not extensionRegex.search(filename):
             return False
-        return extensionRegex.sub('', prefixRegex.sub('', filename))
+        return extensionRegex.sub("", prefixRegex.sub("", filename))
 
     def extractQueryLanguage(queryLanguage, *args, **kwargs):
         raise NotImplementedError
 
     def guessLanguage(request, *args, **kwargs):
         raise NotImplementedError
 
     def getAcceptedLanguagesFromHeader(header, *args, **kwargs):
         raise NotImplementedError
 
     def getLocaleFromObject(obj=None, *args, **kwargs):
         locale = None
-        if type(obj) is dict and checkValues(obj, 'scope') and checkValues(obj['scope'], 'locale'):
-            locale = obj['scope']['locale']
-        if checkValues(obj, 'locale'):
-            locale = obj['locale']
+        if (
+            type(obj) is dict
+            and checkValues(obj, "scope")
+            and checkValues(obj["scope"], "locale")
+        ):
+            locale = obj["scope"]["locale"]
+        if checkValues(obj, "locale"):
+            locale = obj["locale"]
         return locale
 
     def parsePluralInterval(phrase, count, *args, **kwargs):
         returnPhrase = phrase
-        phrases = re.split(r'\|', phrase)
+        phrases = re.split(r"\|", phrase)
         intervalRuleExists = False
 
         # some() breaks on 1st true
         def test(p):
             # access variables from upper function
             nonlocal returnPhrase, intervalRuleExists
-            
-            matches = re.search(r'^\s*([()[\]]+[\d,]+[()[\]]+)?\s*(.*)$', p)
+
+            matches = re.search(r"^\s*([()[\]]+[\d,]+[()[\]]+)?\s*(.*)$", p)
 
             # not the same as in combined condition
             if matches and matches.group(1):
                 intervalRuleExists = True
                 if matchInterval(count, matches.group(1)) == True:
                     returnPhrase = matches.group(2)
                     return True
             else:
                 # this is a other or catch all case, this only is taken into account if there is actually another rule
                 if intervalRuleExists:
                     returnPhrase = p
             return False
+
         for p in phrases:
             if test(p):
                 break
         return returnPhrase
 
     def matchInterval(number, interval, *args, **kwargs):
         interval = parseInterval(interval)
         if interval and type(number) is int:
-            if interval['from']['value'] == number:
-                return interval['from']['included']
-            if interval['to']['value'] == number:
-                return interval['to']['included']
+            if interval["from"]["value"] == number:
+                return interval["from"]["included"]
+            if interval["to"]["value"] == number:
+                return interval["to"]["included"]
 
             return (
-                min(interval['from']['value'], number) == interval['from']['value'] and
-                max(interval['to']['value'], number) == interval['to']['value']
+                min(interval["from"]["value"], number) == interval["from"]["value"]
+                and max(interval["to"]["value"], number) == interval["to"]["value"]
             )
         return False
 
-    def translate(locale=None, singular=None, plural=None, skipSyncToAllFiles=False, *args, **kwargs):
+    def translate(
+        locale=None,
+        singular=None,
+        plural=None,
+        skipSyncToAllFiles=False,
+        *args,
+        **kwargs,
+    ):
         # access variables from upper function
         nonlocal locales, defaultLocale, retryInDefaultLocale, fallbacks, objectNotation, syncFiles
 
         # add same key to all translations
         if not skipSyncToAllFiles and syncFiles:
             syncToAllFiles(singular, plural)
 
         if locale is None:
-            logWarn(f'WARN: No locale found - check the context of the call to __(). Using {defaultLocale} as current locale')
+            logWarn(
+                f"WARN: No locale found - check the context of the call to __(). Using {defaultLocale} as current locale"
+            )
             locale = defaultLocale
 
         # try to get a fallback
         if not checkValues(locales, locale):
             locale = getFallback(locale, fallbacks) or locale
 
         # attempt to read when defined as valid locale
         if not checkValues(locales, locale):
             read(locale)
 
         # fallback to default when missed
         if not checkValues(locales, locale):
-            logWarn(f'WARN: Locale {locale} couldn\'t be read - check the context of the call to $__. Using {defaultLocale} (default) as current locale')
+            logWarn(
+                f"WARN: Locale {locale} couldn't be read - check the context of the call to $__. Using {defaultLocale} (default) as current locale"
+            )
 
             locale = defaultLocale
             read(locale)
 
         # dotnotaction add on, @todo: factor out
         defaultSingular = singular
         defaultPlural = plural
         if objectNotation:
-            indexOfColon = singular.index(':')
+            indexOfColon = singular.index(":")
             # We compare against 0 instead of -1 because
             # we don't really expect the string to start with ':'.
             if indexOfColon > 0:
-                defaultSingular = singular[indexOfColon+1]
+                defaultSingular = singular[indexOfColon + 1]
                 singular = singular[0:indexOfColon]
             if plural and type(plural) is not int:
-                indexOfColon = plural.index(':')
+                indexOfColon = plural.index(":")
                 if indexOfColon > 0:
-                    defaultPlural = plural[indexOfColon+1]
+                    defaultPlural = plural[indexOfColon + 1]
                     plural = plural[0:indexOfColon]
 
         accessor = localeAccessor(locale, singular)
         mutator = localeMutator(locale, singular)
 
         if plural:
             if accessor() is None:
                 # when retryInDefaultLocale is true - try to set default value from defaultLocale
                 if retryInDefaultLocale and locale != defaultLocale:
-                    logDebug(f'Missing {singular} in {locale} retrying in {defaultLocale}')
+                    logDebug(
+                        f"Missing {singular} in {locale} retrying in {defaultLocale}"
+                    )
                     mutator(translate(defaultLocale, singular, plural, True))
                 else:
-                    mutator({
-                        'one': defaultSingular or singular,
-                        'other': defaultPlural or plural
-                    })
+                    mutator(
+                        {
+                            "one": defaultSingular or singular,
+                            "other": defaultPlural or plural,
+                        }
+                    )
                 write(locale)
 
         if accessor() is None:
             # when retryInDefaultLocale is true - try to set default value from defaultLocale
-                if retryInDefaultLocale and locale != defaultLocale:
-                    logDebug(f'Missing {singular} in {locale} retrying in {defaultLocale}')
-                    mutator(translate(defaultLocale, singular, plural, True))
-                else:
-                    mutator(defaultSingular or singular)
-                write(locale)
+            if retryInDefaultLocale and locale != defaultLocale:
+                logDebug(f"Missing {singular} in {locale} retrying in {defaultLocale}")
+                mutator(translate(defaultLocale, singular, plural, True))
+            else:
+                mutator(defaultSingular or singular)
+            write(locale)
 
         return accessor()
 
     def syncToAllFiles(singular=None, plural=None, *args, **kwargs):
         # access variables from upper function
         nonlocal locales
 
         for locale in locales:
             translate(locale, singular, plural, True)
 
-    def localeAccessor(locale=None, singular=None, allowDelayedTraversal=True, *args, **kwargs):
+    def localeAccessor(
+        locale=None, singular=None, allowDelayedTraversal=True, *args, **kwargs
+    ):
         # access variables from upper function
         nonlocal locales, objectNotation
 
         # Bail out on non-existent locales to defend against internal errors.
         if not checkValues(locales, locale):
             return lambda *args, **kwargs: None
 
@@ -672,14 +766,15 @@
             # If delayed traversal wasn't specifically forbidden, it is allowed.
             # The accessor we're trying to find and which we want to return.
             accessor = None
             # An accessor that returns null.
             nullAccessor = lambda *args, **kwargs: None
             # Do we need to re-traverse the tree upon invocation of the accessor?
             reTraverse = False
+
             # Split the provided term and run the callback for each subterm.
             def reducer(obj, index):
                 # access variables from upper function
                 nonlocal accessor, nullAccessor, reTraverse, allowDelayedTraversal
 
                 # Make the accessor return null.
                 accessor = nullAccessor
@@ -690,25 +785,36 @@
                     reTraverse = allowDelayedTraversal
                     # Return null to avoid deeper iterations.
                     return None
                 # We can traverse deeper, so we generate an accessor for this current level.
                 accessor = lambda *args, **kwargs: obj[index]
                 # Return a reference to the next deeper level in the locale tree.
                 return obj[index]
+
             functools.reduce(reducer, singular.split(objectNotation), locales[locale])
             # Return the requested accessor.
             # If we need to re-traverse (because we didn't find our target term)
             # traverse again and return the new result (but don't allow further iterations)
             # or return the previously found accessor if it was already valid.
-            return lambda *args, **kwargs: localeAccessor(locale, singular, False)() if reTraverse else accessor()
+            return (
+                lambda *args, **kwargs: localeAccessor(locale, singular, False)()
+                if reTraverse
+                else accessor()
+            )
         else:
             # No object notation, just return an accessor that performs array lookup.
-            return lambda *args, **kwargs: locales[locale][singular] if checkValues(locales[locale], singular) else None
+            return (
+                lambda *args, **kwargs: locales[locale][singular]
+                if checkValues(locales[locale], singular)
+                else None
+            )
 
-    def localeMutator(locale=None, singular=None, allowBranching=False, *args, **kwargs):
+    def localeMutator(
+        locale=None, singular=None, allowBranching=False, *args, **kwargs
+    ):
         # access variables from upper function
         nonlocal locales, objectNotation, missingKeyFn
 
         # Bail out on non-existent locales to defend against internal errors.
         if not checkValues(locales, locale):
             return lambda *args, **kwargs: None
 
@@ -720,14 +826,15 @@
             accessor = None
             # An accessor that takes one argument and returns null.
             nullAccessor = lambda *args, **kwargs: None
             # Fix object path.
             fixObject = lambda *args, **kwargs: {}
             # Are we going to need to re-traverse the tree when the mutator is invoked?
             reTraverse = False
+
             # Split the provided term and run the callback for each subterm.
             def reducer(obj, index):
                 # access variables from upper function
                 nonlocal accessor, nullAccessor, allowBranching, fixObject, reTraverse
 
                 # Make the mutator do nothing.
                 accessor = nullAccessor
@@ -742,73 +849,86 @@
                         # If we are allowed to, create a new object along the path.
                         obj[index] = {}
                     else:
                         # If we aren't allowed, remember that we need to re-traverse later on and...
                         reTraverse = True
                         # ...return null to make the next iteration bail our early on.
                         return None
+
                 # Generate a mutator for the current level.
                 def accessor(value):
                     obj[index] = value
                     return value
+
                 # Generate a fixer for the current level.
                 def fixObject(*args, **kwargs):
                     obj[index] = {}
                     return obj[index]
 
                 # Return a reference to the next deeper level in the locale tree.
                 return obj[index]
+
             functools.reduce(reducer, singular.split(objectNotation), locales[locale])
+
             # Return the final mutator.
             def returnAbove(value):
                 # access variables from upper function
                 nonlocal locale, singular, reTraverse, accessor
 
                 # If we need to re-traverse the tree
                 # invoke the search again, but allow branching
                 # this time (because here the mutator is being invoked)
                 # otherwise, just change the value directly.
                 value = missingKeyFn(locale, value)
-                return localeMutator(locale, singular, True)(value) if reTraverse else accessor(value)
+                return (
+                    localeMutator(locale, singular, True)(value)
+                    if reTraverse
+                    else accessor(value)
+                )
+
             return returnAbove
         else:
             # No object notation, just return a mutator that performs array lookup and changes the value.
             def returnBelow(value):
                 # access variables from upper function
                 nonlocal locale, singular
 
                 value = missingKeyFn(locale, value)
                 locales[locale][singular] = value
                 return value
+
             return returnBelow
 
     def read(locale=None, *args, **kwargs):
         # access variables from upper function
         nonlocal locales, parser
 
         localeFile = {}
         file = getStorageFilePath(locale)
         try:
-            with open(file, 'r', encoding='utf-8') as localeFile:
+            with open(file, "r", encoding="utf-8") as localeFile:
                 content = localeFile.read()
             try:
                 # parsing filecontents to locales[locale]
                 locales[locale] = parser.loads(content)
             except Exception as parseError:
-                logError(f'unable to parse locales from file (maybe {file} is empty or invalid json?): ', parseError)
+                logError(
+                    f"unable to parse locales from file (maybe {file} is empty or invalid json?): ",
+                    parseError,
+                )
         except Exception as readError:
             # unable to read, so intialize that file
             # locales[locale] are already set in memory, so no extra read required
             # or locales[locale] are empty, which initializes an empty locale.json file
             # since the current invalid locale could exist, we should back it up
             if os.path.exists(file):
-                logDebug(f'backing up invalid locale {locale} to {file}.invalid')
-                blockedRename(file, f'{file}.invalid')
+                logDebug(f"backing up invalid locale {locale} to {file}.invalid")
+                blockedRename(file, f"{file}.invalid")
 
-            logDebug(f'initializing {file}')
+            logDebug(f"initializing {file}")
             write(locale)
 
     def write(locale=None, *args, **kwargs):
         # access variables from upper function
         nonlocal locales, directory, directoryPermissions, indent, updateFiles, parser
 
         tmp = None
@@ -818,15 +938,15 @@
         if not updateFiles:
             return
 
         # creating directory if necessary
         try:
             stats = os.lstat(directory)
         except Exception as e:
-            logDebug(f'creating locales dir in: {directory}')
+            logDebug(f"creating locales dir in: {directory}")
             try:
                 if type(directoryPermissions) is int:
                     os.makedirs(directory, mode=directoryPermissions)
                 else:
                     os.makedirs(directory)
             except Exception as e:
                 # in case of parallel tasks utilizing in same dir
@@ -836,51 +956,58 @@
         # first time init has an empty file
         if not checkValues(locales, locale):
             locales[locale] = {}
 
         # writing to tmp and rename on success
         try:
             target = getStorageFilePath(locale)
-            tmp = f'{target}.tmp'
-            with open(tmp, 'w', encoding='utf-8') as file:
-                file.write(parser.dumps(locales[locale], ensure_ascii=False, indent=indent))
+            tmp = f"{target}.tmp"
+            with open(tmp, "w", encoding="utf-8") as file:
+                file.write(
+                    parser.dumps(locales[locale], ensure_ascii=False, indent=indent)
+                )
             stats = os.stat(tmp)
             if stats.st_file_attributes == stat.FILE_ATTRIBUTE_ARCHIVE:
                 shutil.move(tmp, target)
             else:
-                logError(f'unable to write locales to file (either {tmp} or {target} are not writeable?): ')
+                logError(
+                    f"unable to write locales to file (either {tmp} or {target} are not writeable?): "
+                )
         except Exception as e:
-            logError(f'unexpected error writing files (either {tmp} or {target} are not writeable?): ', e)    
+            logError(
+                f"unexpected error writing files (either {tmp} or {target} are not writeable?): ",
+                e,
+            )
 
     def getStorageFilePath(locale=None, *args, **kwargs):
         # access variables from upper function
         nonlocal pathsep, directory, extension, prefix
 
         # changed API to use .json as default, #16
-        ext = extension or '.json'
-        filepath = os.path.normpath(f'{directory}{pathsep}{prefix}{locale}{ext}')
-        filepathJS = os.path.normpath(f'{directory}{pathsep}{prefix}{locale}.py')
+        ext = extension or ".json"
+        filepath = os.path.normpath(f"{directory}{pathsep}{prefix}{locale}{ext}")
+        filepathJS = os.path.normpath(f"{directory}{pathsep}{prefix}{locale}.py")
 
         # use .py as fallback if already existing
         try:
             if os.stat(filepathJS):
-                logDebug(f'using existing file {filepathJS}')
-                extension = '.py'
+                logDebug(f"using existing file {filepathJS}")
+                extension = ".py"
                 return filepathJS
         except Exception as e:
-            logDebug(f'will use {filepath}')
+            logDebug(f"will use {filepath}")
         return filepath
 
     def getFallback(targetLocale=None, fallbacks=None, *args, **kwargs):
         fallbacks = fallbacks or {}
         if checkValues(fallbacks, targetLocale):
             return fallbacks[targetLocale]
         fallBackLocale = None
         for key in fallbacks:
-            if re.search(r'^'+key.replace('*', '.*')+r'$', str(targetLocale)):
+            if re.search(r"^" + key.replace("*", ".*") + r"$", str(targetLocale)):
                 fallBackLocale = fallbacks[key]
                 break
         return fallBackLocale
 
     def logDebug(msg=None, *args, **kwargs):
         # access variables from upper function
         nonlocal logDebugFn
@@ -904,15 +1031,17 @@
 
     # ===================
     # =    utilities    =
     # ===================
 
     # api
 
-    escapeRegExp = lambda string: re.sub(r'[.*+?^${}()|[\]\\]', lambda substring: f'\\{substring.group(0)}', string)
+    escapeRegExp = lambda string: re.sub(
+        r"[.*+?^${}()|[\]\\]", lambda substring: f"\\{substring.group(0)}", string
+    )
 
     checkValues = lambda obj, *keytypes: _checkValues(obj, *keytypes)
 
     watchFiles = lambda path, handler: _watch(path, handler)
 
     getArgsList = lambda locals, function: _getArgsList(locals, function)
 
@@ -936,128 +1065,145 @@
                 return False
         return True
 
     class _WatchDogFactory(object):
         __dogs = {}
 
         @staticmethod
-        def create(path, dog):
+        def create(dog, path):
             name = os.path.abspath(path)
             if name not in _WatchDogFactory.__dogs:
-                _WatchDogFactory.__dogs[name] = {
-                    'mutex': Lock(),
-                    'observer': dog
-                }
+                _WatchDogFactory.__dogs[name] = {"mutex": Lock(), "observer": dog}
 
         @staticmethod
         def delete(path):
             name = os.path.abspath(path)
             if name in _WatchDogFactory.__dogs:
-                _WatchDogFactory.__dogs[name]['observer'].stop()
+                _WatchDogFactory.__dogs[name]["observer"].stop()
                 del _WatchDogFactory.__dogs[name]
 
         @staticmethod
         def obtainMutex(path):
             name = os.path.abspath(path)
             if name not in _WatchDogFactory.__dogs:
                 raise
-            return _WatchDogFactory.__dogs[name]['mutex']
+            return _WatchDogFactory.__dogs[name]["mutex"]
 
         @staticmethod
         def obtainDog(path):
             name = os.path.abspath(path)
             if name not in _WatchDogFactory.__dogs:
                 raise
-            return _WatchDogFactory.__dogs[name]['observer']
+            return _WatchDogFactory.__dogs[name]["observer"]
 
     class _EventHandler(FileSystemEventHandler):
-        def __init__(self, path, handler):
-            self.path = path
+        def __init__(self, handler, path):
+            self.path = os.path.abspath(path)
             self.handler = handler
 
         def on_any_event(self, event):
-            if _WatchDogFactory.obtainMutex(self.path).acquire(blocking=True, timeout=1):
+            if _WatchDogFactory.obtainMutex(self.path).acquire(
+                blocking=True, timeout=1
+            ):
                 self.handler(event)
                 _WatchDogFactory.obtainMutex(self.path).release()
             return super().on_any_event(event)
 
     def _watch(path, handler):
-        handler = _EventHandler(path, handler)
+        handler = _EventHandler(handler, path)
         observer = Observer()
-        _WatchDogFactory.create(path, observer)
+        _WatchDogFactory.create(observer, path)
         observer.schedule(handler, path)
         observer.start()
 
     def _getArgsList(locals, function):
         result = []
         for key in inspect.signature(function).parameters.keys():
             value = locals[key]
-            if key == 'args':
+            if key == "args":
                 result += list(value)
-            elif key == 'kwargs':
+            elif key == "kwargs":
                 result += list(value.values())
             else:
                 result.append(value)
         return result
 
     _patternParts = {
-        'value': '[-+]?(?:inf|\[[0-9]*\.?\d*(?:[eE][-+]?\d+)?)',
-        'leftBrace': '[\(\]\[]',
-        'delimeter': ',',
-        'rightBrace': '[\)\]\[]',
+        "value": "[-+]?(?:inf|\[[0-9]*\.?\d*(?:[eE][-+]?\d+)?)",
+        "leftBrace": "[\(\]\[]",
+        "delimeter": ",",
+        "rightBrace": "[\)\]\[]",
     }
 
-    _PATTERN = re.compile(rf'({_patternParts["leftBrace"]})({_patternParts["value"]})?({_patternParts["delimeter"]})?({_patternParts["value"]})?({_patternParts["rightBrace"]})')
+    _PATTERN = re.compile(
+        rf'({_patternParts["leftBrace"]})({_patternParts["value"]})?({_patternParts["delimeter"]})?({_patternParts["value"]})?({_patternParts["rightBrace"]})'
+    )
 
     def _execPattern(string):
         match = _PATTERN.search(string)
         if not match:
             return None
-        matchList = [match.group()] + [match.groups()[i] if i < len(match.groups()) and match.groups()[i] != '' else None for i in range(5)]
+        matchList = [match.group()] + [
+            match.groups()[i]
+            if i < len(match.groups()) and match.groups()[i] != ""
+            else None
+            for i in range(5)
+        ]
         _ = matchList[0]
         leftBrace = matchList[1]
         fromValue = matchList[2]
         delimeter = matchList[3]
         toValue = matchList[4]
         rightBrace = matchList[5]
         return {
-            'leftBrace': leftBrace,
-            'fromValue': fromValue,
-            'delimeter': delimeter,
-            'toValue': toValue,
-            'rightBrace': rightBrace
+            "leftBrace": leftBrace,
+            "fromValue": fromValue,
+            "delimeter": delimeter,
+            "toValue": toValue,
+            "rightBrace": rightBrace,
         }
 
     def _convert(string):
         try:
             return eval(str(string)).real
         except:
             return math.nan
 
     def _parse(string):
         match = _execPattern(string)
         if not match:
             return None
         return {
-            'from': {
-                'value': _convert(match['fromValue']) if match['fromValue'] is not None else -math.inf,
-                'included': match['leftBrace'] == '['
+            "from": {
+                "value": _convert(match["fromValue"])
+                if match["fromValue"] is not None
+                else -math.inf,
+                "included": match["leftBrace"] == "[",
+            },
+            "to": {
+                "value": _convert(match["toValue"])
+                if match["toValue"] is not None
+                else +math.inf
+                if match["delimeter"]
+                else _convert(match["fromValue"])
+                if match["fromValue"] is not None
+                else math.nan,
+                "included": match["rightBrace"] == "]",
             },
-            'to': {
-                'value': _convert(match['toValue']) if match['toValue'] is not None else +math.inf if match['delimeter'] else _convert(match['fromValue']) if match['fromValue'] is not None else math.nan,
-                'included': match['rightBrace'] == ']'
-            }
         }
 
     def _check(interval):
-        if not interval or interval['to']['value'] is math.nan:
+        if not interval or interval["to"]["value"] is math.nan:
             return None
-        if interval['from']['value'] == interval['to']['value']:
-            return interval['from']['included'] and interval['to']['included']
-        return min(interval['from']['value'], interval['to']['value']) == interval['from']['value']
+        if interval["from"]["value"] == interval["to"]["value"]:
+            return interval["from"]["included"] and interval["to"]["included"]
+        return (
+            min(interval["from"]["value"], interval["to"]["value"])
+            == interval["from"]["value"]
+        )
 
     def _entry(string):
         if type(string) is not str:
             return None
         interval = _parse(string)
         if not _check(interval):
             return None
@@ -1068,98 +1214,126 @@
             try:
                 os.rename(source, target)
                 break
             except:
                 pass
 
     # implicitly configure when created with given options
-    # 
+    #
     # i18n = I18n({
     #   'locales': ['en', 'fr']
     # })
     if type(_OPTS) is dict or _OPTS:
-        i18n['configure'](_OPTS)
+        i18n["configure"](_OPTS)
 
     class I18n(object):
         def __init__(self):
             self.__dict__ = i18n
 
         def __del__(self):
             # tricks
             nonlocal directory
             _WatchDogFactory.delete(os.path.abspath(directory))
 
         version: str
 
         @staticmethod
-        def configure(options: dict[str, Any] | bool) -> None: ...
+        def configure(options: dict[str, Any] | bool) -> None:
+            ...
 
         @staticmethod
-        def init(request: dict[str, Any], response: dict[str, Any], next: Callable[[], None]) -> None: ...
+        def init(
+            request: dict[str, Any], response: dict[str, Any], next: Callable[[], None]
+        ) -> None:
+            ...
 
         @overload
         @staticmethod
-        def __(phraseOrOptions: dict[str, str] | str, *replace: str | None) -> str: ...
+        def __(phraseOrOptions: dict[str, str] | str, *replace: str | None) -> str:
+            ...
 
         @overload
         @staticmethod
-        def __(phraseOrOptions: dict[str, str] | str, replacements: dict[str, str] | None) -> str: ...
+        def __(
+            phraseOrOptions: dict[str, str] | str, replacements: dict[str, str] | None
+        ) -> str:
+            ...
 
         @overload
         @staticmethod
-        def __n(phrase: dict[str, str] | str, count: int) -> str: ...
+        def __n(phrase: dict[str, str] | str, count: int) -> str:
+            ...
 
         @overload
         @staticmethod
-        def __n(phrase: str, plural: str, count: int) -> str: ...
+        def __n(phrase: str, plural: str, count: int) -> str:
+            ...
 
         @staticmethod
-        def __l(phrase: str) -> list[str]: ...
+        def __l(phrase: str) -> list[str]:
+            ...
 
         @staticmethod
-        def __h(phrase: str) -> list[dict[str, str]]: ...
+        def __h(phrase: str) -> list[dict[str, str]]:
+            ...
 
         @overload
         @staticmethod
-        def __mf(phraseOrOptions: str, *replace: dict[str, Any] | None) -> str: ...
+        def __mf(phraseOrOptions: str, *replace: dict[str, Any] | None) -> str:
+            ...
 
         @overload
         @staticmethod
-        def __mf(phraseOrOptions: str, replacements: dict[str, Any]) -> str: ...
+        def __mf(phraseOrOptions: str, replacements: dict[str, Any]) -> str:
+            ...
 
         @staticmethod
-        def getLocale(request: dict[str, Any]) -> str: ...
+        def getLocale(request: dict[str, Any]) -> str:
+            ...
 
         @overload
         @staticmethod
-        def setLocale(locale: str) -> str: ...
+        def setLocale(locale: str) -> str:
+            ...
 
         @overload
         @staticmethod
-        def setLocale(requestOrResponse: dict[str, Any], locale: str, inheritance: bool) -> str: ...
+        def setLocale(
+            requestOrResponse: dict[str, Any], locale: str, inheritance: bool
+        ) -> str:
+            ...
 
         @overload
         @staticmethod
-        def setLocale(objects: list[dict[str, Any]], locale: str, inheritance: bool) -> str: ...
+        def setLocale(
+            objects: list[dict[str, Any]], locale: str, inheritance: bool
+        ) -> str:
+            ...
 
         @overload
         @staticmethod
-        def getCatalog() -> Any: ...
+        def getCatalog() -> Any:
+            ...
 
         @overload
         @staticmethod
-        def getCatalog(locale: str) -> Any: ...
+        def getCatalog(locale: str) -> Any:
+            ...
 
         @overload
         @staticmethod
-        def getCatalog(request: dict[str, Any], locale: str) -> Any: ...
+        def getCatalog(request: dict[str, Any], locale: str) -> Any:
+            ...
 
         @staticmethod
-        def getLocales() -> list[str]: ...
+        def getLocales() -> list[str]:
+            ...
 
         @staticmethod
-        def addLocale(locale: str) -> None: ...
+        def addLocale(locale: str) -> None:
+            ...
 
         @staticmethod
-        def removeLocale(locale: str) -> None: ...
+        def removeLocale(locale: str) -> None:
+            ...
 
-    return I18n()
+    return I18n()
```

### Comparing `simple-i18n-0.1.1/simple_i18n.egg-info/PKG-INFO` & `simple-i18n-0.1.2/simple_i18n.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-i18n
-Version: 0.1.1
+Version: 0.1.2
 Home-page: https://github.com/iDkGK/simple-i18n
 Author: iDkGK
 Author-email: 1444807655@qq.com
 Maintainer: iDkGK
 Maintainer-email: 1444807655@qq.com
 License: MIT
 Keywords: i18n,gettext,translation
```

