# Comparing `tmp/harlequin-0.0.7.tar.gz` & `tmp/harlequin-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harlequin-0.0.7.tar", max compression
+gzip compressed data, was "harlequin-0.0.8.tar", max compression
```

## Comparing `harlequin-0.0.7.tar` & `harlequin-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1068 2023-05-12 18:43:06.953114 harlequin-0.0.7/LICENSE
--rw-r--r--   0        0        0     1473 2023-05-12 18:43:06.953114 harlequin-0.0.7/README.md
--rw-r--r--   0        0        0     1438 2023-05-12 18:43:06.961115 harlequin-0.0.7/pyproject.toml
--rw-r--r--   0        0        0       53 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/__init__.py
--rw-r--r--   0        0        0       49 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/__main__.py
--rw-r--r--   0        0        0      336 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/cli.py
--rw-r--r--   0        0        0       53 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/__init__.py
--rw-r--r--   0        0        0     2647 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/app.css
--rw-r--r--   0        0        0     8744 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/app.py
--rw-r--r--   0        0        0      812 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/__init__.py
--rw-r--r--   0        0        0      913 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/code_editor.py
--rw-r--r--   0        0        0     1125 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/error_modal.py
--rw-r--r--   0        0        0      672 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/filename_modal.py
--rw-r--r--   0        0        0     3126 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/key_handlers.py
--rw-r--r--   0        0        0     2480 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/results_viewer.py
--rw-r--r--   0        0        0     3001 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/schema_viewer.py
--rw-r--r--   0        0        0    15911 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/components/textarea.py
--rw-r--r--   0        0        0      661 2023-05-12 18:43:06.961115 harlequin-0.0.7/src/harlequin/tui/utils.py
--rw-r--r--   0        0        0     2475 1970-01-01 00:00:00.000000 harlequin-0.0.7/setup.py
--rw-r--r--   0        0        0     2187 1970-01-01 00:00:00.000000 harlequin-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-15 19:56:23.010672 harlequin-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2050 2023-05-15 19:56:23.010672 harlequin-0.0.8/README.md
+-rw-r--r--   0        0        0     1460 2023-05-15 19:56:23.018673 harlequin-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0       53 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/__main__.py
+-rw-r--r--   0        0        0      336 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/cli.py
+-rw-r--r--   0        0        0       53 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/__init__.py
+-rw-r--r--   0        0        0     2647 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/app.css
+-rw-r--r--   0        0        0     8813 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/app.py
+-rw-r--r--   0        0        0      972 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/__init__.py
+-rw-r--r--   0        0        0      913 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/code_editor.py
+-rw-r--r--   0        0        0     1125 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/error_modal.py
+-rw-r--r--   0        0        0      672 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/filename_modal.py
+-rw-r--r--   0        0        0     3212 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/key_handlers.py
+-rw-r--r--   0        0        0      665 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/messages.py
+-rw-r--r--   0        0        0     2480 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/results_viewer.py
+-rw-r--r--   0        0        0     3001 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/schema_viewer.py
+-rw-r--r--   0        0        0    21184 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/components/textarea.py
+-rw-r--r--   0        0        0      661 2023-05-15 19:56:23.018673 harlequin-0.0.8/src/harlequin/tui/utils.py
+-rw-r--r--   0        0        0     3060 1970-01-01 00:00:00.000000 harlequin-0.0.8/setup.py
+-rw-r--r--   0        0        0     2764 1970-01-01 00:00:00.000000 harlequin-0.0.8/PKG-INFO
```

### Comparing `harlequin-0.0.7/LICENSE` & `harlequin-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/pyproject.toml` & `harlequin-0.0.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "harlequin"
-version = "0.0.7"
+version = "0.0.8"
 description = "A Text User Interface for DuckDB"
 authors = ["Ted Conbeer <tconbeer@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     { include = "harlequin", from = "src" },
 ]
@@ -22,15 +22,15 @@
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 textual = {version="*", extras=["dev"]}
 
 [tool.poetry.group.static.dependencies]
 black = "^23.3.0"
-ruff = ">=0.0.264,<0.0.266"
+ruff = ">=0.0.264,<0.0.268"
 mypy = "^1.2.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 
 [tool.poetry.scripts]
@@ -38,15 +38,16 @@
 
 [tool.ruff]
 select = ["E", "F", "I"]
 
 [tool.mypy]
 python_version = "3.11"
 files = [
-    "src/harlequin/**/*.py"
+    "src/harlequin/**/*.py",
+    "tests/**/*.py",
 ]
 
 show_column_numbers = true
 
 # show error messages from unrelated files
 follow_imports = "normal"
```

### Comparing `harlequin-0.0.7/src/harlequin/tui/app.css` & `harlequin-0.0.8/src/harlequin/tui/app.css`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/app.py` & `harlequin-0.0.8/src/harlequin/tui/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,22 +19,24 @@
     ResultsViewer,
     SchemaViewer,
     TextInput,
 )
 from harlequin.tui.utils import short_type
 
 
-class Harlequin(App):
+class Harlequin(App, inherit_bindings=False):
     """
     A Textual App for a SQL client for DuckDB.
     """
 
     CSS_PATH = "app.css"
     MAX_RESULTS = 50_000
 
+    BINDINGS = [("ctrl+q", "quit", "Quit")]
+
     query_text: reactive[str] = reactive(str)
     relation: reactive[Union[duckdb.DuckDBPyRelation, None]] = reactive(None)
     data: reactive[List[Tuple]] = reactive(list)
 
     def __init__(
         self,
         db_path: Path,
```

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/__init__.py` & `harlequin-0.0.8/src/harlequin/tui/components/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from harlequin.tui.components.code_editor import CodeEditor as CodeEditor
 from harlequin.tui.components.error_modal import ErrorModal as ErrorModal
 from harlequin.tui.components.filename_modal import FilenameModal as FilenameModal
+from harlequin.tui.components.messages import (
+    CursorMoved as CursorMoved,
+)
+from harlequin.tui.components.messages import (
+    ScrollOne as ScrollOne,
+)
 from harlequin.tui.components.results_viewer import (
     ResultsTable as ResultsTable,
 )
 from harlequin.tui.components.results_viewer import (
     ResultsViewer as ResultsViewer,
 )
 from harlequin.tui.components.schema_viewer import (
```

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/code_editor.py` & `harlequin-0.0.8/src/harlequin/tui/components/code_editor.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/error_modal.py` & `harlequin-0.0.8/src/harlequin/tui/components/error_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/filename_modal.py` & `harlequin-0.0.8/src/harlequin/tui/components/filename_modal.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/key_handlers.py` & `harlequin-0.0.8/src/harlequin/tui/components/key_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     lno: int
     pos: int
 
 
 def handle_arrow(key: str, lines: List[str], cursor: Cursor) -> Cursor:
     arrow = key.split("+")[-1]
     if "ctrl" in key:
+        assert arrow not in ("up", "down"), "ctrl+up/down should be handled first"
         if arrow == "right":
             return _handle_ctrl_right(lines, cursor)
-        else:  # arrow == "left":
+        else:  # if arrow == "left":
             return _handle_ctrl_left(lines, cursor)
     else:
         if arrow == "right":
             return _handle_right(lines, cursor)
         elif arrow == "left":
             return _handle_left(lines, cursor)
         elif arrow == "down":
```

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/results_viewer.py` & `harlequin-0.0.8/src/harlequin/tui/components/results_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/schema_viewer.py` & `harlequin-0.0.8/src/harlequin/tui/components/schema_viewer.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/src/harlequin/tui/components/textarea.py` & `harlequin-0.0.8/src/harlequin/tui/components/textarea.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,69 +1,58 @@
+from math import ceil, floor
 from typing import List, Tuple, Union
 
 from rich.console import RenderableType
 from rich.syntax import Syntax
 from sqlfmt.api import Mode, format_string
 from sqlfmt.exception import SqlfmtError
 from textual import events
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import ScrollableContainer
-from textual.message import Message
 from textual.reactive import reactive
 from textual.widget import Widget
 from textual.widgets import Static
 
 from harlequin.tui.components.error_modal import ErrorModal
 from harlequin.tui.components.filename_modal import FilenameModal
 from harlequin.tui.components.key_handlers import Cursor, handle_arrow
+from harlequin.tui.components.messages import CursorMoved, ScrollOne
 
 BRACKETS = {
     "(": ")",
     "[": "]",
     "{": "}",
 }
 CLOSERS = {'"': '"', "'": "'", **BRACKETS}
 TAB_SIZE = 4
 
 
 class TextInput(Static, can_focus=True):
     BINDINGS = [
-        ("ctrl+`", "format", "Format Query"),
+        Binding("ctrl+`", "format", "Format Query"),
         Binding("ctrl+@", "format", "Format Query", show=False),
-        ("ctrl+s", "save", "Save Query"),
-        ("ctrl+o", "load", "Open Query"),
+        Binding("ctrl+s", "save", "Save Query"),
+        Binding("ctrl+o", "load", "Open Query"),
     ]
 
     DEFAULT_CSS = """
     TextInput{
         height: auto;
         width: auto;
         padding: 0 1;
     }
     """
 
     lines: reactive[List[str]] = reactive(lambda: list(" "))
     cursor: reactive[Cursor] = reactive(Cursor(0, 0))
     selection_anchor: reactive[Union[Cursor, None]] = reactive(None)
+    clipboard: List[str] = list()
     cursor_visible: reactive[bool] = reactive(True)
 
-    class CursorMoved(Message, bubble=True):
-        """Posted when the cursor moves
-
-        Attributes:
-            cursor_x: The x position of the cursor
-            cursor_y: The y position
-        """
-
-        def __init__(self, cursor_x: int, cursor_y: int) -> None:
-            super().__init__()
-            self.cursor_x = cursor_x
-            self.cursor_y = cursor_y
-
     def on_mount(self) -> None:
         self.blink_timer = self.set_interval(
             0.5,
             self._toggle_cursor,
             pause=not self.has_focus,
         )
 
@@ -74,24 +63,41 @@
         self.update(self._content)
 
     def on_blur(self) -> None:
         self.blink_timer.pause()
         self.cursor_visible = False
         self.update(self._content)
 
+    def on_paste(self, event: events.Paste) -> None:
+        """
+        If the user hits ctrl+v, we don't get that keypress;
+        we get a Paste event instead.
+
+        For now, ignore the system clipboard and mimic ctrl+u.
+        Todo: Use the system clipboard for copy/paste.
+        """
+        event.stop()
+        self.cursor_visible = True
+        self.blink_timer.reset()
+        self._insert_clipboard_at_selection(self.selection_anchor, self.cursor)
+        self.selection_anchor = None
+        self.update(self._content)
+
     def on_key(self, event: events.Key) -> None:
         self.cursor_visible = True
         self.blink_timer.reset()
         selection_before = self.selection_anchor
 
         # set selection_anchor if it's unset
         if event.key == "shift+delete":
             pass  # todo: shift+delete should delete the whole line
-        if event.key == "ctrl+underscore":
-            pass  # this comments out a section, which should maintain selection
+        elif event.key == "shift+tab":
+            pass
+        elif event.key in ("ctrl+underscore", "ctrl+`", "ctrl+@", "ctrl+s", "ctrl+c"):
+            pass  #  these should maintain selection
         elif event.key == "ctrl+a":
             self.selection_anchor = Cursor(0, 0)
         elif selection_before is None and "shift" in event.key:
             self.selection_anchor = self.cursor
         elif selection_before is not None and "shift" not in event.key:
             self.selection_anchor = None
 
@@ -103,15 +109,14 @@
             "left_square_bracket",
             "left_curly_bracket",
             "right_parenthesis",
             "right_square_bracket",
             "right_curly_bracket",
         ):
             assert event.character is not None
-            self.log(f"here! {event.character}")
             if selection_before is None:
                 self._insert_closed_character_at_cursor(event.character, self.cursor)
             elif event.key in (
                 "right_parenthesis",
                 "right_square_bracket",
                 "right_curly_bracket",
             ):
@@ -130,14 +135,17 @@
                 x=self.cursor.pos, y=(self.cursor.lno - self._visible_height() + 1)
             )
         elif event.key in ("pagedown", "shift+pagedown"):
             event.stop()
             self.move_cursor(
                 x=self.cursor.pos, y=(self.cursor.lno + self._visible_height() - 1)
             )
+        elif event.key in ("ctrl+up", "ctrl+down"):
+            event.stop()
+            self.post_message(ScrollOne(direction=event.key.split("+")[1]))
         elif any([dir in event.key for dir in ["left", "right", "up", "down"]]):
             event.stop()
             self.cursor = handle_arrow(event.key, self.lines, self.cursor)
         elif event.key in ("home", "shift+home"):
             event.stop()
             self.cursor = Cursor(self.cursor.lno, 0)
         elif event.key in ("end", "shift+end"):
@@ -161,34 +169,81 @@
                     for indent, stripped_line in zip(indents, no_comment_lines)
                 ]
             else:
                 self.lines[first.lno : last.lno + 1] = [
                     f"{' ' * indent}-- {stripped_line}"
                     for indent, stripped_line in zip(indents, stripped_lines)
                 ]
+        elif event.key in ("ctrl+c", "ctrl+x"):
+            event.stop()
+            if selection_before:
+                lines, first, last = self._get_selected_lines(selection_before)
+            else:  # no selection, copy whole line
+                lines, first, last = (
+                    [self.lines[self.cursor.lno], ""],
+                    Cursor(self.cursor.lno, 0),
+                    Cursor(self.cursor.lno, len(self.lines[self.cursor.lno])),
+                )
+            lines[-1] = lines[-1][: last.pos]
+            lines[0] = lines[0][first.pos :]
+            self.clipboard = lines.copy()
+            self.log(f"copied to clipboard: {self.clipboard}")
+            if event.key == "ctrl+x":
+                self._delete_selection(first, last)
+                new_lno = min(first.lno, len(self.lines) - 1)
+                self.cursor = Cursor(
+                    new_lno, min(first.pos, len(self.lines[new_lno]) - 1)
+                )
+        elif event.key == "ctrl+u":
+            event.stop()
+            self._insert_clipboard_at_selection(selection_before, self.cursor)
+        elif event.key == "tab":
+            event.stop()
+            lines, first, last = self._get_selected_lines(selection_before)
+            # in some cases, selections are replaced with four spaces
+            if first.lno == last.lno and (
+                first.pos == last.pos
+                or first.pos != 0
+                or last.pos != len(self.lines[self.cursor.lno]) - 1
+            ):
+                self._delete_selection(first, last)
+                indent = TAB_SIZE - first.pos % TAB_SIZE
+                self._insert_character_at_cursor(" " * indent, first)
+                self.cursor = Cursor(lno=first.lno, pos=first.pos + indent)
+            # usually, selected lines are prepended with four-ish spaces
+            else:
+                self._indent_selection(selection_before, self.cursor, kind="indent")
+        elif event.key == "shift+tab":
+            event.stop()
+            self._indent_selection(selection_before, self.cursor, kind="dedent")
         elif event.key == "enter":
             event.stop()
             old_lines, first, last = self._get_selected_lines(selection_before)
             head = f"{old_lines[0][:first.pos]} "
             tail = f"{old_lines[-1][last.pos:]}"
-            indent = len(old_lines[0]) - len(old_lines[0].lstrip())
+            if old_lines[0].isspace():
+                indent = 0
+            else:
+                indent = len(old_lines[0]) - len(old_lines[0].lstrip())
+
             char_before = self._get_character_before_cursor(first)
             if char_before in BRACKETS and BRACKETS[
                 char_before
             ] == self._get_character_at_cursor(last):
+                new_indent = indent + TAB_SIZE - (indent % TAB_SIZE)
                 self.lines[first.lno : last.lno + 1] = [
                     head,
-                    f"{' ' * (indent+TAB_SIZE)} ",
+                    f"{' ' * new_indent} ",
                     f"{' ' * indent}{tail.lstrip()}",
                 ]
-                self.cursor = Cursor(first.lno + 1, indent + TAB_SIZE)
+                self.cursor = Cursor(first.lno + 1, new_indent)
             else:
                 self.lines[first.lno : last.lno + 1] = [
                     head,
-                    f"{' ' * indent}{tail.lstrip()} ",
+                    f"{' ' * indent}{tail.lstrip() or ' '}",
                 ]
                 self.cursor = Cursor(first.lno + 1, min(first.pos, indent))
         elif event.key == "delete":
             event.stop()
             if selection_before is None:
                 anchor = self.cursor
                 cursor = handle_arrow("right", self.lines, self.cursor)
@@ -239,15 +294,15 @@
                 # rows are 1-indexed
                 (first.lno + 1, first.pos),
                 (second.lno + 1, second.pos),
             )
         return syntax
 
     def _scroll_to_cursor(self) -> None:
-        self.post_message(self.CursorMoved(self.cursor.pos, self.cursor.lno))
+        self.post_message(CursorMoved(self.cursor.pos, self.cursor.lno))
 
     def _visible_height(self) -> int:
         parent = self.parent
         assert isinstance(parent, TextContainer)
         return parent.window_region.height
 
     def _toggle_cursor(self) -> None:
@@ -304,17 +359,75 @@
             ):
                 self._insert_character_at_cursor(CLOSERS[character], self.cursor)
 
     def _delete_selection(self, anchor: Cursor, cursor: Cursor) -> None:
         old_lines, first, last = self._get_selected_lines(anchor, maybe_cursor=cursor)
         head = f"{old_lines[0][:first.pos]}"
         tail = f"{old_lines[-1][last.pos:]}"
-        self.lines[first.lno : last.lno + 1] = [f"{head}{tail}"]
+        if new_line := f"{head}{tail}":
+            self.lines[first.lno : last.lno + 1] = [new_line]
+        else:  # empty str, no line-ending space, delete whole line
+            self.lines[first.lno : last.lno + 1] = []
+            if not self.lines:
+                self.lines = [" "]
         self.cursor = Cursor(first.lno, first.pos)
 
+    def _indent_selection(
+        self, anchor: Union[Cursor, None], cursor: Cursor, kind: str
+    ) -> None:
+        assert kind in ("indent", "dedent")
+        rounder, offset = (ceil, -1) if kind == "dedent" else (floor, 1)
+
+        lines, first, last = self._get_selected_lines(anchor, cursor)
+        leading_spaces = [(len(line) - len(line.lstrip())) for line in lines]
+        leading_tabs = [rounder(space / TAB_SIZE) for space in leading_spaces]
+        new_lines = [
+            f"{' ' * TAB_SIZE * max(0, indent+offset)}{line.lstrip()}"
+            for line, indent in zip(lines, leading_tabs)
+        ]
+        self.lines[first.lno : last.lno + 1] = new_lines
+        if anchor:
+            change_at_anchor_line = len(new_lines[anchor.lno - first.lno]) - len(
+                lines[anchor.lno - first.lno]
+            )
+            self.selection_anchor = (
+                anchor
+                if anchor.pos == 0
+                else Cursor(
+                    anchor.lno,
+                    anchor.pos + change_at_anchor_line,
+                )
+            )
+        change_at_cursor = len(new_lines[cursor.lno - first.lno]) - len(
+            lines[cursor.lno - first.lno]
+        )
+        self.cursor = (
+            cursor
+            if cursor.pos == 0
+            else Cursor(cursor.lno, cursor.pos + change_at_cursor)
+        )
+
+    def _insert_clipboard_at_selection(
+        self, anchor: Union[Cursor, None], cursor: Cursor
+    ) -> None:
+        if anchor:
+            self._delete_selection(anchor, cursor)
+            cursor = self.cursor
+        head = self.lines[cursor.lno][: cursor.pos]
+        tail = self.lines[cursor.lno][cursor.pos :]
+        if (clip_len := len(self.clipboard)) != 0:
+            new_lines = self.clipboard.copy()
+            new_lines[0] = f"{head}{new_lines[0]}"
+            new_lines[-1] = f"{new_lines[-1]}{tail}"
+            self.lines[cursor.lno : cursor.lno + 1] = new_lines
+            self.cursor = Cursor(
+                cursor.lno + clip_len - 1,
+                len(self.lines[cursor.lno + clip_len - 1]) - len(tail),
+            )
+
     def _get_character_at_cursor(self, cursor: Cursor) -> str:
         return self.lines[cursor.lno][cursor.pos]
 
     def _get_character_before_cursor(self, cursor: Cursor) -> Union[str, None]:
         if self.cursor.pos == 0:
             return None
         else:
@@ -375,15 +488,15 @@
         """
         input = self.query_one(TextInput)
         input.cursor_visible = True
         input.blink_timer.reset()
         input.move_cursor(event.x - 1, event.y)
         input.focus()
 
-    def on_text_input_cursor_moved(self, event: TextInput.CursorMoved) -> None:
+    def on_cursor_moved(self, event: CursorMoved) -> None:
         """
         Scrolls the container so the cursor is visible.
         """
         event.stop()
         container = self.query_one(TextContainer)
         x_buffer = container.window_region.width // 4
         y_buffer = container.window_region.height // 4
@@ -404,14 +517,22 @@
             >= container.window_region.y + container.window_region.height - y_buffer
         ):  # scroll down
             container.scroll_to(
                 container.window_region.x,
                 event.cursor_y - container.window_region.height + y_buffer,
             )
 
+    def on_scroll_one(self, event: ScrollOne) -> None:
+        event.stop()
+        offset = 1 if event.direction == "down" else -1
+        container = self.query_one(TextContainer)
+        container.scroll_to(
+            container.window_region.x, container.window_region.y + offset
+        )
+
 
 if __name__ == "__main__":
     from textual.app import App, ComposeResult
 
     class TextApp(App):
         def compose(self) -> ComposeResult:
             yield TextArea()
```

### Comparing `harlequin-0.0.7/src/harlequin/tui/utils.py` & `harlequin-0.0.8/src/harlequin/tui/utils.py`

 * *Files identical despite different names*

### Comparing `harlequin-0.0.7/PKG-INFO` & `harlequin-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: harlequin
-Version: 0.0.7
+Version: 0.0.8
 Summary: A Text User Interface for DuckDB
 License: MIT
 Author: Ted Conbeer
 Author-email: tconbeer@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,57 +25,65 @@
 
 (A Harlequin is also a [pretty duck](https://en.wikipedia.org/wiki/Harlequin_duck).)
 
 ![harlequin duck](harlequin.jpg)
 
 ## Installing Harlequin
 
-Use `pip` or `pipx`:
+After installing Python 3.8 or above, install Harlequin using `pip` or `pipx` with:
 
 ```bash
 pipx install harlequin
 ```
 
 > **Tip:**
 >
 > You can run invoke directly with [`pipx run`](https://pypa.github.io/pipx/examples/#pipx-run-examples) anywhere that `pipx` is installed. For example:
 > - `pipx run harlequin --help`
 > - `pipx run harlequin ./my.duckdb`
 
+
+## Running Harlequin in a Container
+
+Without a database file:
+
+```bash
+docker run ghcr.io/tconbeer/harlequin:latest
+```
+
+Mounting a database file `./foo.db` into the container's working directory, `/data`:
+
+```bash
+docker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db
+```
+
 ## Using Harlequin
 
-To open a DuckDB database file:
+From any shell, to open a DuckDB database file:
 
 ```bash
 harlequin "path/to/duck.db"
 ```
 
 To open an in-memory DuckDB session, run Harlequin with no arguments:
 
 ```bash
 harlequin
 ```
 
-When Harlequin is open, you can view the schema of your DuckDB database in the left sidebar.
-
-To run a query, enter your code in the main textarea, then press Ctrl+Enter. You should see the data appear in the pane below.
+### Viewing the Schema of your Database
 
-You can press Tab or use your mouse to change the focus between the panes.
+When Harlequin is open, you can view the schema of your DuckDB database in the left sidebar. You can use your mouse or the arrow keys + enter to navigate the tree. The tree shows schemas, tables/views and their types, and columns and their types.
 
-When the focus is on the data pane, you can use your arrow keys or mouse to select different cells.
+### Editing a Query
 
-Press Ctrl+c to quit and return to your shell.
+The main query editor is a full-featured text editor, with features including syntax highlighting, auto-formatting with ``ctrl + ` ``, text selection, copy/paste, and more.
 
-### Running Harlequin in a Container
+You can save the query currently in the editor with `ctrl + s`. You can open a query in any text or .sql file with `ctrl + o`.
 
-Without a database file:
-
-```bash
-docker run ghcr.io/tconbeer/harlequin:latest
-```
+### Running a Query and Viewing Results
 
-Mounting a database file `./foo.db` into the container's working directory, `/data`:
+To run a query, press `ctrl + enter`. Up to 50k records will be loaded into the results pane below the query editor. When the focus is on the data pane, you can use your arrow keys or mouse to select different cells.
 
-```bash
-docker run -v $(pwd)/foo.db:/data/bar.db ghcr.io/tconbeer/harlequin:latest harlequin bar.db
-```
+### Exiting Harlequin
 
+Press `ctrl + q` to quit and return to your shell.
```

