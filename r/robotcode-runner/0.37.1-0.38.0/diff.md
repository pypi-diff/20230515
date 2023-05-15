# Comparing `tmp/robotcode_runner-0.37.1.tar.gz` & `tmp/robotcode_runner-0.38.0.tar.gz`

## Comparing `robotcode_runner-0.37.1.tar` & `robotcode_runner-0.38.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3555 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6007 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    18514 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/README.md
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/pyproject.toml
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.37.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6003 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    20426 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/LICENSE.txt
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/README.md
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/pyproject.toml
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 robotcode_runner-0.38.0/PKG-INFO
```

### Comparing `robotcode_runner-0.37.1/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.38.0/src/robotcode/runner/cli/libdoc.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         options, arguments = super().parse_arguments(cli_args)
 
         if self.dry:
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute libdoc with the following options and arguments:\n"
-                f'{line_end.join((*(f"{k} = {repr(v)}" for k, v in options.items()) ,*arguments))}'
+                f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
```

### Comparing `robotcode_runner-0.37.1/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.38.0/src/robotcode/runner/cli/rebot.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         options, arguments = super().parse_arguments(cli_args)
 
         if self.dry:
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute libdoc with the following options and arguments:\n"
-                f'{line_end.join((*(f"{k} = {repr(v)}" for k, v in options.items()) ,*arguments))}'
+                f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
```

### Comparing `robotcode_runner-0.37.1/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.38.0/src/robotcode/runner/cli/robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             arguments = self.paths
 
         if self.dry:
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute robot with the following options and arguments:\n"
-                f'{line_end.join((*(f"{k} = {repr(v)}" for k, v in options.items()) ,*arguments))}'
+                f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
 
 ROBOT_OPTIONS = (
     click.option("--by-longname", type=str, multiple=True, help="Select tests/tasks or suites by longname."),
```

### Comparing `robotcode_runner-0.37.1/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.38.0/src/robotcode/runner/cli/testdoc.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         options, arguments = super().parse_arguments(cli_args)
 
         if self.dry:
             line_end = "\n"
             raise Information(
                 "Dry run, not executing any commands. "
                 f"Would execute testdoc with the followingoptions and arguments:\n"
-                f'{line_end.join((*(f"{k} = {repr(v)}" for k, v in options.items()) ,*arguments))}'
+                f'{line_end.join((*(f"{k} = {v!r}" for k, v in options.items()) ,*arguments))}'
             )
 
         return options, arguments
 
     def main(self, arguments: Any, **options: Any) -> Any:
         if self.root_folder is not None:
             os.chdir(self.root_folder)
```

### Comparing `robotcode_runner-0.37.1/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.38.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import io
 import os
 import re
 import sys
+from collections import defaultdict
 from dataclasses import dataclass
 from io import IOBase
 from pathlib import Path
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import click
 import robot.running.model as running_model
@@ -122,22 +122,22 @@
                     error_message=str(e), name=TestSuite.name_from_source(structure.source), source=structure.source
                 ), TestDefaults(self.parent_defaults)
 
         SuiteStructureParser._build_suite_directory = build_suite_directory
 
     old_get_file = FileReader._get_file
 
-    def get_file(self: FileReader, source: Union[str, Path, IOBase], accept_text: bool) -> Tuple[io.IOBase, bool]:
+    def get_file(self: FileReader, source: Union[str, Path, IOBase], accept_text: bool) -> Any:
         path = self._get_path(source, accept_text)
         if path:
             if _stdin_data is not None and (data := _stdin_data.get(str(path))) is not None:
                 if data is not None:
-                    return old_get_file(self, data, accept_text)  # type: ignore
+                    return old_get_file(self, data, accept_text)
 
-        return old_get_file(self, source, accept_text)  # type: ignore
+        return old_get_file(self, source, accept_text)
 
     FileReader._get_file = get_file
 
 
 @dataclass
 class TestItem:
     type: str
@@ -174,14 +174,15 @@
             name=Path.cwd().name,
             longname=Path.cwd().name,
             uri=str(Uri.from_path(Path.cwd())),
         )
         self._current = self.all
         self.suites: List[TestItem] = []
         self.tests: List[TestItem] = []
+        self.tags: Dict[str, List[TestItem]] = defaultdict(list)
         self.statistics = Statistics()
 
     def visit_suite(self, suite: TestSuite) -> None:
         item = TestItem(
             type="suite",
             id=f"{Path(suite.source).resolve() if suite.source is not None else ''};{suite.longname}",
             name=suite.name,
@@ -225,23 +226,27 @@
             uri=str(Uri.from_path(test.source)) if test.source else None,
             range=Range(
                 start=Position(line=test.lineno - 1, character=0),
                 end=Position(line=test.lineno - 1, character=0),
             ),
             tags=list(test.tags) if test.tags else None,
         )
+        for tag in test.tags:
+            self.tags[str(tag)].append(item)
 
         self.tests.append(item)
         self._current.children.append(item)
 
         self.statistics.tests += 1
 
 
 @click.group(invoke_without_command=False)
-@click.option("--read-from-stdin", is_flag=True, help="Read file contents from stdin. This is an internal option.")
+@click.option(
+    "--read-from-stdin", is_flag=True, help="Read file contents from stdin. This is an internal option.", hidden=True
+)
 @pass_application
 def discover(app: Application, read_from_stdin: bool) -> None:
     """\
     Commands to discover informations about the current project.
 
     \b
     Examples:
@@ -249,15 +254,15 @@
     robotcode discover tests
     robotcode --profile regression discover tests
     ```
     """
     if read_from_stdin:
         global _stdin_data
         _stdin_data = from_json(sys.stdin.buffer.read(), Dict[str, str], strict=True)
-        app.verbose(f"Read data from stdin: {repr(_stdin_data)}")
+        app.verbose(f"Read data from stdin: {_stdin_data!r}")
 
 
 RE_IN_FILE_LINE_MATCHER = re.compile(r".+\sin\sfile\s'(?P<file>.*)'\son\sline\s(?P<line>\d+):(?P<message>.*)")
 RE_PARSING_FAILED_MATCHER = re.compile(r"Parsing\s'(?P<file>.*)'\sfailed:(?P<message>.*)")
 
 
 class DiagnosticsLogger:
@@ -530,7 +535,68 @@
                     yield f"{item.longname}{os.linesep}"
 
             if collector.suites:
                 app.echo_via_pager(print(collector.suites))
 
         else:
             app.print_data(ResultItem(collector.suites, diagnostics), remove_defaults=True)
+
+
+@dataclass
+class TagsResult:
+    tags: Dict[str, List[TestItem]]
+
+
+@discover.command(
+    context_settings={
+        "allow_extra_args": True,
+        "ignore_unknown_options": True,
+    },
+    add_help_option=True,
+    epilog='Use "-- --help" to see `robot` help.',
+)
+@add_options(*ROBOT_OPTIONS)
+@pass_application
+def tags(
+    app: Application,
+    by_longname: Tuple[str, ...],
+    exclude_by_longname: Tuple[str, ...],
+    robot_options_and_args: Tuple[str, ...],
+) -> None:
+    """\
+    Discover tags with the selected configuration, profiles, options and
+    arguments.
+
+    \b
+    Examples:
+    ```
+    robotcode discover tags
+    robotcode --profile regression discover tags
+
+    robotcode --profile regression discover tags -i wip
+    ```
+    """
+
+    suite, diagnostics = handle_options(app, by_longname, exclude_by_longname, robot_options_and_args)
+
+    collector = Collector()
+    suite.visit(collector)
+
+    if collector.all.children:
+        if app.config.output_format is None or app.config.output_format == OutputFormat.TEXT:
+
+            def print(tags: Dict[str, List[TestItem]]) -> Iterable[str]:
+                for tag, items in tags.items():
+                    yield f"{tag}{os.linesep}"
+                    # for item in items:
+                    #     yield f"  {item.longname}{os.linesep}"
+                    #     if item.uri:
+                    #         yield (
+                    #             f" ({Uri(item.uri).to_path()}{f':{item.range.start.line+1}' if item.range else ''})"
+                    #             f"{os.linesep}"
+                    #         )
+
+            if collector.suites:
+                app.echo_via_pager(print(collector.tags))
+
+        else:
+            app.print_data(TagsResult(collector.tags), remove_defaults=True)
```

### Comparing `robotcode_runner-0.37.1/.gitignore` & `robotcode_runner-0.38.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.37.1/LICENSE.txt` & `robotcode_runner-0.38.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.37.1/README.md` & `robotcode_runner-0.38.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.37.1/pyproject.toml` & `robotcode_runner-0.38.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -24,17 +24,17 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-robot==0.37.1",
-  "robotcode-modifiers==0.37.1",
-  "robotcode==0.37.1",
+  "robotcode-robot==0.38.0",
+  "robotcode-modifiers==0.38.0",
+  "robotcode==0.38.0",
 ]
 
 [project.entry-points.robotcode]
 runner = "robotcode.runner.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_runner-0.37.1/PKG-INFO` & `robotcode_runner-0.38.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-runner
-Version: 0.37.1
+Version: 0.38.0
 Summary: RobotCode runner plugin for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,17 +21,17 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-modifiers==0.37.1
-Requires-Dist: robotcode-robot==0.37.1
-Requires-Dist: robotcode==0.37.1
+Requires-Dist: robotcode-modifiers==0.38.0
+Requires-Dist: robotcode-robot==0.38.0
+Requires-Dist: robotcode==0.38.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
```

