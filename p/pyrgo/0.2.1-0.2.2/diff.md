# Comparing `tmp/pyrgo-0.2.1.tar.gz` & `tmp/pyrgo-0.2.2.tar.gz`

## Comparing `pyrgo-0.2.1.tar` & `pyrgo-0.2.2.tar`

### file list

```diff
@@ -1,41 +1,60 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 pyrgo-0.2.1/.tool-versions
--rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrgo-0.2.1/Makefile
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.2.1/mkdocs.yml
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.2.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrgo-0.2.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.2.1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/__main__.py
--rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/py.typed
--rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/add.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/build.py
--rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/check.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/clean.py
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/fmt.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/lock.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/new.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/remove.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/venv.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/docs/__init__.py
--rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/docs/build.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/docs/new.py
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/docs/root.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/command/docs/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/utilities/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/utilities/command.py
--rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyrgo/utilities/project.py
--rw-r--r--   0        0        0     3673 2020-02-02 00:00:00.000000 pyrgo-0.2.1/requirements/core.lock
--rw-r--r--   0        0        0     3684 2020-02-02 00:00:00.000000 pyrgo-0.2.1/requirements/dev.lock
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.2.1/scripts/new_release.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyrgo-0.2.1/tests/integration/resources/pyproject.toml
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 pyrgo-0.2.1/tests/unit/utilities/test_command.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyrgo-0.2.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.2.1/LICENSE
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrgo-0.2.1/README.md
--rw-r--r--   0        0        0     2186 2020-02-02 00:00:00.000000 pyrgo-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 pyrgo-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pyrgo-0.2.2/.tool-versions
+-rw-r--r--   0        0        0     1497 2020-02-02 00:00:00.000000 pyrgo-0.2.2/Makefile
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 pyrgo-0.2.2/mkdocs.yml
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 pyrgo-0.2.2/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 pyrgo-0.2.2/.github/workflows/test.yml
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 pyrgo-0.2.2/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/__init__.py
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/__main__.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/cli.py
+-rw-r--r--   0        0        0      251 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/__init__.py
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/add.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/build.py
+-rw-r--r--   0        0        0      391 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/check.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/clean.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/fmt.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/init.py
+-rw-r--r--   0        0        0     1043 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/lock.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/new.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/remove.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/sync.py
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/test.py
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/venv.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/docs/__init__.py
+-rw-r--r--   0        0        0     1005 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/docs/build.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/docs/new.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/docs/root.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/cli/commands/docs/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/__init__.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/contants.py
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/models/__init__.py
+-rw-r--r--   0        0        0     2435 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/models/pyproject.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/__init__.py
+-rw-r--r--   0        0        0      397 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/build.py
+-rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/check.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/clean.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/fmt.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/lock.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/sync.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/test.py
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/venv.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/docs/__init__.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/docs/build.py
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/docs/new.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/ops/docs/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/utilities/__init__.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/utilities/command.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyrgo/core/utilities/text.py
+-rw-r--r--   0        0        0     3721 2020-02-02 00:00:00.000000 pyrgo-0.2.2/requirements/core.lock
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pyrgo-0.2.2/requirements/dev.lock
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pyrgo-0.2.2/scripts/new_release.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 pyrgo-0.2.2/tests/unit/utilities/test_text.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 pyrgo-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 pyrgo-0.2.2/LICENSE
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pyrgo-0.2.2/README.md
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 pyrgo-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 pyrgo-0.2.2/PKG-INFO
```

### Comparing `pyrgo-0.2.1/Makefile` & `pyrgo-0.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/.github/workflows/release.yml` & `pyrgo-0.2.2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/.github/workflows/test.yml` & `pyrgo-0.2.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/pyrgo/cli.py` & `pyrgo-0.2.2/pyrgo/cli/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,47 @@
 """Root CLI."""
 
 import click
 
-from pyrgo.command.add import add
-from pyrgo.command.build import build
-from pyrgo.command.check import check
-from pyrgo.command.clean import clean
-from pyrgo.command.docs import docs
-from pyrgo.command.fmt import fmt
-from pyrgo.command.init import init
-from pyrgo.command.lock import lock
-from pyrgo.command.new import new
-from pyrgo.command.remove import remove
-from pyrgo.command.test import test
-from pyrgo.command.venv import venv
-from pyrgo.utils import add_commands
-
-
-@click.group()
-@click.version_option()
-def cli() -> None:
-    """pyrgo. Python package manager."""
+from pyrgo.cli.commands.add import add
+from pyrgo.cli.commands.build import build
+from pyrgo.cli.commands.check import check
+from pyrgo.cli.commands.clean import clean
+from pyrgo.cli.commands.docs import docs
+from pyrgo.cli.commands.fmt import fmt
+from pyrgo.cli.commands.init import init
+from pyrgo.cli.commands.lock import lock
+from pyrgo.cli.commands.new import new
+from pyrgo.cli.commands.remove import remove
+from pyrgo.cli.commands.sync import sync
+from pyrgo.cli.commands.test import test
+from pyrgo.cli.commands.venv import venv
+from pyrgo.cli.utils import add_commands
+
+
+@click.group(
+    context_settings={"help_option_names": ["-h", "--help"]},
+    invoke_without_command=False,
+)
+@click.version_option(prog_name="Pyrgo")
+def root() -> None:
+    """Pyrgo. Python package manager."""
 
 
 add_commands(
-    cli=cli,
+    cli=root,
     commands=[
         check,
         clean,
         fmt,
         init,
         lock,
         new,
         venv,
         add,
         test,
         docs,
         remove,
         build,
+        sync,
     ],
 )
```

### Comparing `pyrgo-0.2.1/pyrgo/command/fmt.py` & `pyrgo-0.2.2/pyrgo/core/ops/sync.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,51 @@
-"""fmt command."""
-
+"""sync operation."""
 import pathlib
 
-import click
+from result import Err, Ok, Result
 
-from pyrgo.utilities.command import (
+from pyrgo.core.errors import RequirementsFolderNotFoundError
+from pyrgo.core.utilities.command import (
     PythonExecCommand,
     inform_and_run_program,
 )
-from pyrgo.utilities.project import extract_relevent_paths, read_pyproject
-
 
-@click.command()
-def fmt() -> None:
-    """Format all files of the current project using `black` and `ruff`."""
-    cwd = pathlib.Path().cwd()
-    content = read_pyproject(cwd=cwd)
-    relevant_paths = extract_relevent_paths(content=content)
 
-    inform_and_run_program(
-        command=PythonExecCommand(program="ruff").add_args(
-            args=["--fix-only", *relevant_paths],
-        ),
-    )
+def execute(
+    *,
+    cwd: pathlib.Path,
+    environment: str,
+    editable: bool,
+) -> Result[None, RequirementsFolderNotFoundError]:
+    """Execute sync operation."""
+    req_path = cwd.joinpath("requirements")
+    if not req_path.exists() and req_path.is_dir():
+        return Err(RequirementsFolderNotFoundError(cwd=cwd))
 
     inform_and_run_program(
-        command=PythonExecCommand(program="black").add_args(
-            args=relevant_paths,
+        command=PythonExecCommand(program="piptools").add_args(
+            args=[
+                "sync",
+                f"{req_path!s}/{environment}.lock",
+            ],
         ),
     )
+    if editable:
+        inform_and_run_program(
+            command=PythonExecCommand(program="pip").add_args(
+                args=[
+                    "install",
+                    "-e",
+                    ".",
+                ],
+            ),
+        )
+    else:
+        inform_and_run_program(
+            command=PythonExecCommand(program="pip").add_args(
+                args=[
+                    "install",
+                    ".",
+                ],
+            ),
+        )
+    return Ok()
```

### Comparing `pyrgo-0.2.1/pyrgo/command/test.py` & `pyrgo-0.2.2/pyrgo/cli/commands/test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,43 @@
 """test command."""
 
 import pathlib
+import sys
 from typing import List, Optional
 
 import click
+from result import Ok
 
-from pyrgo.utilities.command import PythonExecCommand, inform_and_run_program
-from pyrgo.utilities.project import (
-    list_pytest_markers,
-    read_pyproject,
-)
+from pyrgo.core import ops
+from pyrgo.core.models.pyproject import Pyproject
 
 
 def dynamic_marker_choices() -> List[str]:
     """Dynamic markers for options."""
-    cwd = pathlib.Path().cwd()
-    content = read_pyproject(cwd=cwd)
-    return list_pytest_markers(content=content)
+    pyproject = Pyproject(cwd=pathlib.Path().cwd())
+    pyproject.read_pyproject_toml()
+    return pyproject.list_pytest_markers()
 
 
 @click.command()
 @click.option(
     "-m",
     "--marked",
     "marker",
     type=click.Choice(
         choices=dynamic_marker_choices(),
     ),
     default=None,
     help="Run tests based on marks. By default all tests are executed.",
 )
-@click.option(
-    "--no-strict-markers",
-    "no_strict_markers",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Any unknown marks applied with the `@pytest.mark.name_of_mark` decorator will trigger an error.",  # noqa: E501
-)
 def test(
     *,
-    no_strict_markers: bool,
     marker: Optional[str],
 ) -> None:
     """Execute tests using `pytest`."""
-    args_to_add: List[str] = []
-    if not no_strict_markers:
-        args_to_add.append("--strict-markers")
-
-    if marker:
-        args_to_add.extend(["-m", marker])
-
-    inform_and_run_program(
-        command=PythonExecCommand(program="pytest").add_args(
-            args=args_to_add,
-        ),
-    )
+    executed = ops.test.execute(marker=marker)
+
+    if not isinstance(executed, Ok):
+        click.echo(message=executed.err())
+        sys.exit(1)
+
+    sys.exit(0)
```

### Comparing `pyrgo-0.2.1/pyrgo/command/docs/serve.py` & `pyrgo-0.2.2/pyrgo/cli/commands/docs/serve.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 """docs serve command."""
 import sys
-from typing import List
+
+from result import Ok
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 
 import click
 
-from pyrgo.utilities.command import (
-    PythonExecCommand,
-    inform_and_run_program,
-)
+from pyrgo.core import ops
 
 
 @click.command()
 @click.option(
     "-a",
     "--dev-addr",
     "dev_addr",
@@ -49,21 +47,17 @@
         "material",
         "mkdocs",
         "readthedocs",
     ],
     strict: bool,
 ) -> None:
     """Serve project documentation."""
-    args_to_add: List[str] = ["serve"]
-
-    if strict:
-        args_to_add.append("--strict")
-    args_to_add.extend(["--theme", theme])
-    args_to_add.extend(["--dev-addr", dev_addr])
-
-    inform_and_run_program(
-        command=PythonExecCommand(
-            program="mkdocs",
-        ).add_args(
-            args=args_to_add,
-        ),
+    executed = ops.docs.serve.execute(
+        dev_address=dev_addr,
+        theme=theme,
+        strict=strict,
     )
+    if not isinstance(executed, Ok):
+        click.echo(message=executed.err())
+        sys.exit(1)
+
+    sys.exit(0)
```

### Comparing `pyrgo-0.2.1/pyrgo/utilities/command.py` & `pyrgo-0.2.2/pyrgo/core/utilities/command.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 """command utilities."""
 import subprocess
 import sys
 from typing import List
 
-if sys.version_info >= (3, 9):
-    from typing import Literal
-else:
-    from typing_extensions import Literal
-
-
 import click
 from typing_extensions import Self
 
+from pyrgo.core.utilities.text import colorize_text
+
 
 class PythonExecCommand:
     """Command builder."""
 
     def __init__(self, program: str) -> None:
         """Python programs to be executed within current python interpreter."""
         self.program = program
@@ -27,26 +23,14 @@
         return self
 
     def run(self) -> None:
         """Run command."""
         subprocess.run(args=self.args)
 
 
-def colorize_text(
-    *,
-    text: str,
-    color: Literal[
-        "yellow",
-        "red",
-    ],
-) -> str:
-    """Colorize text."""
-    return click.style(text=text, fg=color)
-
-
 def inform_and_run_program(command: PythonExecCommand) -> None:
     """Inform and run program."""
     click.echo(
         message=colorize_text(
             text=f"running {command.program}...",
             color="yellow",
         ),
```

### Comparing `pyrgo-0.2.1/requirements/core.lock` & `pyrgo-0.2.2/requirements/core.lock`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     #   pytest
 ptyprocess==0.7.0
     # via pexpect
 pygments==2.15.1
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==9.11
+pymdown-extensions==10.0
     # via mkdocs-material
 pyperclip==1.8.2
     # via hatch
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via pyrgo (pyproject.toml)
@@ -146,14 +146,16 @@
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.5.5
     # via mkdocs-material
 requests==2.30.0
     # via mkdocs-material
+result==0.10.0
+    # via pyrgo (pyproject.toml)
 rich==13.3.5
     # via hatch
 ruff==0.0.267
     # via pyrgo (pyproject.toml)
 shellingham==1.5.0.post1
     # via hatch
 six==1.16.0
```

### Comparing `pyrgo-0.2.1/requirements/dev.lock` & `pyrgo-0.2.2/requirements/dev.lock`

 * *Files 4% similar despite different names*

```diff
@@ -125,15 +125,15 @@
     #   pytest
 ptyprocess==0.7.0
     # via pexpect
 pygments==2.15.1
     # via
     #   mkdocs-material
     #   rich
-pymdown-extensions==9.11
+pymdown-extensions==10.0
     # via mkdocs-material
 pyperclip==1.8.2
     # via hatch
 pyproject-hooks==1.0.0
     # via build
 pytest==7.3.1
     # via pyrgo (pyproject.toml)
@@ -146,14 +146,16 @@
     #   pyyaml-env-tag
 pyyaml-env-tag==0.1
     # via mkdocs
 regex==2023.5.5
     # via mkdocs-material
 requests==2.30.0
     # via mkdocs-material
+result==0.10.0
+    # via pyrgo (pyproject.toml)
 rich==13.3.5
     # via hatch
 ruff==0.0.267
     # via pyrgo (pyproject.toml)
 shellingham==1.5.0.post1
     # via hatch
 six==1.16.0
```

### Comparing `pyrgo-0.2.1/scripts/new_release.py` & `pyrgo-0.2.2/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/tests/unit/utilities/test_command.py` & `pyrgo-0.2.2/tests/unit/utilities/test_text.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
 import pytest
 
-from pyrgo.utilities.command import colorize_text
+from pyrgo.core.utilities.text import colorize_text
 
 
 @pytest.mark.unit()
 @pytest.mark.parametrize(
     argnames=["color", "expected_text"],
     argvalues=[
         (
```

### Comparing `pyrgo-0.2.1/.gitignore` & `pyrgo-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/LICENSE` & `pyrgo-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrgo-0.2.1/pyproject.toml` & `pyrgo-0.2.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyrgo"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
@@ -17,26 +17,27 @@
     "ruff",
     "mypy",
     "black",
     "pip-tools",
     "pytest",
     "mkdocs-material",
     "hatch",
-    "tomli"
+    "tomli",
+    "result"
 ]
 
 [[project.authors]]
 name = "Tomas Perez Alvarez"
 email = "tomasperezalvarez@gmail.com"
 
 [project.optional-dependencies]
 dev = []
 
 [project.scripts]
-pyrgo = "pyrgo.__main__:cli"
+pyrgo = "pyrgo.cli.__main__:cli"
 
 [project.urls]
 Documentation = "https://github.com/Tomperez98/pyrgo#readme"
 Issues = "https://github.com/Tomperez98/pyrgo/issues"
 Source = "https://github.com/Tomperez98/pyrgo"
 
 [tool.ruff]
```

### Comparing `pyrgo-0.2.1/PKG-INFO` & `pyrgo-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrgo
-Version: 0.2.1
+Version: 0.2.2
 Project-URL: Documentation, https://github.com/Tomperez98/pyrgo#readme
 Project-URL: Issues, https://github.com/Tomperez98/pyrgo/issues
 Project-URL: Source, https://github.com/Tomperez98/pyrgo
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
@@ -13,13 +13,14 @@
 Requires-Dist: black
 Requires-Dist: click
 Requires-Dist: hatch
 Requires-Dist: mkdocs-material
 Requires-Dist: mypy
 Requires-Dist: pip-tools
 Requires-Dist: pytest
+Requires-Dist: result
 Requires-Dist: ruff
 Requires-Dist: tomli
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # pyrgo
```

