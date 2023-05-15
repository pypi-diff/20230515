# Comparing `tmp/sh40_zenith-0.1.0.tar.gz` & `tmp/sh40_zenith-0.2.0.tar.gz`

## Comparing `sh40_zenith-0.1.0.tar` & `sh40_zenith-0.2.0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/dont_test_markup.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_color.py
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_lru_cache.py
--rw-r--r--   0        0        0     4229 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_markup.py
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/tests/test_palette.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/__about__.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/__init__.py
--rw-r--r--   0        0        0     8247 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/color.py
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/color_info.py
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/exceptions.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/lru_cache.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/macros.py
--rw-r--r--   0        0        0    12503 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/markup.old.py
--rw-r--r--   0        0        0    10714 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/markup.py
--rw-r--r--   0        0        0     7166 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/zenith/palette.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/.gitignore
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/README.md
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 sh40_zenith-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0     5049 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/tests/dont_test_markup.py
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/tests/test_lru_cache.py
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/tests/test_markup.py
+-rw-r--r--   0        0        0     1456 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/tests/test_palette.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/__about__.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/__init__.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/__main__.py
+-rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/exceptions.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/lru_cache.py
+-rw-r--r--   0        0        0     2016 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/macros.py
+-rw-r--r--   0        0        0    10853 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/markup.py
+-rw-r--r--   0        0        0     7172 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/zenith/palette.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/README.md
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2287 2020-02-02 00:00:00.000000 sh40_zenith-0.2.0/PKG-INFO
```

### Comparing `sh40_zenith-0.1.0/tests/dont_test_markup.py` & `sh40_zenith-0.2.0/tests/dont_test_markup.py`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/tests/test_markup.py` & `sh40_zenith-0.2.0/tests/test_markup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import time
 import pytest
 
 from zenith import zml, zml_alias, zml_macro, ZmlNameError, ZmlSemanticsError
-from zenith.markup import _parse_color
+from zenith.markup import parse_color
 
 
 def test_markup_builtin_only():
     assert (
         result := zml("[bold 141]Hello [@61]There ")
     ) == "\x1b[38;5;141;1mHello \x1b[48;5;61mThere ", repr(result)
 
@@ -41,15 +41,15 @@
 
     assert (
         result := zml("[test @red]Hello")
     ) == "\x1b[38;2;165;42;42;48;2;255;0;0;1mHello", repr(result)
 
     assert (
         result := zml("[test]Hello[/test]Reset")
-    ) == "\x1b[38;2;165;42;42;1mHello\x1b[39;22mReset", repr(result)
+    ) == "\x1b[38;2;165;42;42;1mHello\x1b[22;39mReset", repr(result)
 
 
 def test_markup_macros():
     @zml_macro
     def epoch(template: str, fmt: str = "%c") -> str:
         return template.format(time=f"the current time with {fmt=}")
 
@@ -103,30 +103,30 @@
     assert (
         (result := zml("[@yellow]Black[@black]White"))
         == "\x1b[38;2;35;35;35;48;2;255;255;0mBlack\x1b[38;2;245;245;245;48;2;0;0;0mWhite"
     ), repr(result)
 
 
 def test_markup_colors():
-    assert _parse_color("red", False) == "38;2;255;0;0"
-    assert _parse_color("blue", True) == "48;2;0;0;255"
-    assert _parse_color("2", False) == "32"
-    assert _parse_color("9", False) == "91"
-    assert _parse_color("14", True) == "106"
-    assert _parse_color("78", True) == "48;5;78"
+    assert parse_color("red", False) == "38;2;255;0;0"
+    assert parse_color("blue", True) == "48;2;0;0;255"
+    assert parse_color("2", False) == "32"
+    assert parse_color("9", False) == "91"
+    assert parse_color("14", True) == "106"
+    assert parse_color("78", True) == "48;5;78"
     assert (
-        _parse_color("#baebae", True)
-        == _parse_color("186;235;174", True)
+        parse_color("#baebae", True)
+        == parse_color("186;235;174", True)
         == "48;2;186;235;174"
     )
 
 
 def test_markup_parse_errors():
     with pytest.raises(ZmlNameError):
-        _parse_color("256", False)
+        parse_color("256", False)
 
     with pytest.raises(ZmlNameError):
         zml("[not-a-tag]Hello")
 
     with pytest.raises(ZmlNameError):
         zml("[!not-a-macro]Hello")
```

### Comparing `sh40_zenith-0.1.0/tests/test_palette.py` & `sh40_zenith-0.2.0/tests/test_palette.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from zenith.color import Color
+from slate.color import Color
 from zenith.markup import zml_context
 from zenith.palette import Palette, analogous, tetradic, triadic
 
 
 def test_palette_triadic():
     pal = Palette.from_hex("#FABCDE", strategy=triadic)
```

### Comparing `sh40_zenith-0.1.0/zenith/exceptions.py` & `sh40_zenith-0.2.0/zenith/exceptions.py`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/zenith/lru_cache.py` & `sh40_zenith-0.2.0/zenith/lru_cache.py`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/zenith/markup.py` & `sh40_zenith-0.2.0/zenith/markup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 import re
 
 from functools import lru_cache
 from typing import Callable, TypedDict
 
 from slate.span import UNSETTERS, SETTERS_TO_STYLES, Span
+from slate.color import Color
+from slate.color_info import NAMED_COLORS
 
-from .color import Color
-from .color_info import NAMED_COLORS
 from .exceptions import ZmlNameError, ZmlSemanticsError
 from .lru_cache import LRUCache
 
 __all__ = [
     "zml",
     "zml_alias",
     "zml_macro",
     "combine_spans",
     "zml_get_spans",
+    "zml_pre_process",
     "zml_context",
     "MarkupContext",
     "GLOBAL_CONTEXT",
 ]
 
 MacroType = Callable[[str], str]
 
@@ -148,15 +149,15 @@
 
         styles["background" if invert else "foreground"] = new
         return True
 
     return False
 
 
-def _parse_color(color: str, background: bool) -> str:
+def parse_color(color: str, background: bool) -> str:
     """Parses a color tag."""
 
     background *= 10
 
     color = color.lstrip("@")
 
     if color.isdigit():
@@ -211,15 +212,15 @@
         else:
             styles[tag] = not is_unsetter
 
         return
 
     if RE_COLOR.match(tag) or tag in NAMED_COLORS:
         layer = "background" if is_background else "foreground"
-        styles[layer] = _parse_color(tag, is_background)
+        styles[layer] = parse_color(tag, is_background)
         return
 
     if tag.startswith("~"):
         styles["hyperlink"] = "" if is_unsetter else tag[1:]
         return
 
     raise ZmlNameError(tag)
@@ -244,14 +245,17 @@
     Most importantly, this function can recognize `@tags`, and insert the prefix to the
     correct spot (between `@` and the first letter).
     """
 
     if tag.startswith("@"):
         return "@" + prefix + tag[1:]
 
+    if tag.startswith("!"):
+        return "!" + prefix + tag[1:]
+
     return prefix + tag
 
 
 @lru_cache(512)
 def combine_spans(spans: tuple[Span, ...]) -> str:
     """Combines the given span iterable into optimized ANSI text."""
 
@@ -403,18 +407,19 @@
                         expected_type="macro",
                     )
 
                 del macros[name]
 
             else:
                 name, args = _parse_macro(tag)
-                macro = get_macro(_apply_prefix(name, prefix), None)
+                prefixed = _apply_prefix(name, prefix)
+                macro = get_macro(prefixed, None)
 
                 if macro is None:
-                    raise ZmlNameError(tag, expected_type="macro")
+                    raise ZmlNameError(prefixed, expected_type="macro")
 
                 macros[name] = (macro, args)
 
             tag_list.remove(tag)
 
         if len(tag_list) > 0:
             output += f"[{' '.join(tag_list)}]"
```

### Comparing `sh40_zenith-0.1.0/zenith/palette.py` & `sh40_zenith-0.2.0/zenith/palette.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """The Palette class and its built-in strategies."""
 
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 from typing import Callable
 
-from .color import Color
+from slate.color import Color
+
 from .markup import MarkupContext, zml_alias
 
 __all__ = [
     "triadic",
     "analogous",
     "tetradic",
     "PalettingFunction",
```

### Comparing `sh40_zenith-0.1.0/.gitignore` & `sh40_zenith-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/LICENSE.txt` & `sh40_zenith-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/README.md` & `sh40_zenith-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sh40_zenith-0.1.0/pyproject.toml` & `sh40_zenith-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -26,14 +26,17 @@
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/shade40/zenith#readme"
 Issues = "https://github.com/shade40/zenith#issues"
 Source = "https://github.com/shade40/zenith"
 
+[project.scripts]
+zml = "zenith.__main__:command_zml"
+
 [tool.hatch.version]
 path = "zenith/__about__.py"
 
 [tool.hatch.build]
 include = [
   "zenith/*.py",
   "/tests",
```

### Comparing `sh40_zenith-0.1.0/PKG-INFO` & `sh40_zenith-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sh40-zenith
-Version: 0.1.0
+Version: 0.2.0
 Summary: A markup language and color palette generators targeting the terminal.
 Project-URL: Documentation, https://github.com/shade40/zenith#readme
 Project-URL: Issues, https://github.com/shade40/zenith#issues
 Project-URL: Source, https://github.com/shade40/zenith
 Author-email: bczsalba <bczsalba@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

