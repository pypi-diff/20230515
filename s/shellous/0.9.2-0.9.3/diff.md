# Comparing `tmp/shellous-0.9.2.tar.gz` & `tmp/shellous-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellous-0.9.2.tar", max compression
+gzip compressed data, was "shellous-0.9.3.tar", max compression
```

## Comparing `shellous-0.9.2.tar` & `shellous-0.9.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11347 2021-11-04 23:59:45.892344 shellous-0.9.2/LICENSE
--rw-r--r--   0        0        0     8260 2021-11-04 23:59:55.976433 shellous-0.9.2/README.md
--rw-r--r--   0        0        0     1466 2021-11-04 23:59:45.892344 shellous-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      653 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/__init__.py
--rw-r--r--   0        0        0    21229 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/command.py
--rw-r--r--   0        0        0     6621 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/harvest.py
--rw-r--r--   0        0        0     6737 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/log.py
--rw-r--r--   0        0        0     4871 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/pipeline.py
--rw-r--r--   0        0        0     7528 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/pty_util.py
--rw-r--r--   0        0        0     6883 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/redirect.py
--rw-r--r--   0        0        0     3348 2021-11-04 23:59:45.892344 shellous-0.9.2/shellous/result.py
--rw-r--r--   0        0        0    34439 2021-11-04 23:59:45.896344 shellous-0.9.2/shellous/runner.py
--rw-r--r--   0        0        0     4214 2021-11-04 23:59:45.896344 shellous-0.9.2/shellous/util.py
--rw-r--r--   0        0        0    10066 2021-11-04 23:59:45.896344 shellous-0.9.2/shellous/watcher.py
--rw-r--r--   0        0        0     9279 2021-11-04 23:59:56.958024 shellous-0.9.2/setup.py
--rw-r--r--   0        0        0     9026 2021-11-04 23:59:56.959192 shellous-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11347 2021-11-10 18:11:43.811179 shellous-0.9.3/LICENSE
+-rw-r--r--   0        0        0     8268 2021-11-10 18:11:54.023505 shellous-0.9.3/README.md
+-rw-r--r--   0        0        0     1466 2021-11-10 18:11:43.811179 shellous-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      653 2021-11-10 18:11:43.811179 shellous-0.9.3/shellous/__init__.py
+-rw-r--r--   0        0        0    21402 2021-11-10 18:11:43.811179 shellous-0.9.3/shellous/command.py
+-rw-r--r--   0        0        0     6621 2021-11-10 18:11:43.811179 shellous-0.9.3/shellous/harvest.py
+-rw-r--r--   0        0        0     6737 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/log.py
+-rw-r--r--   0        0        0     4875 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/pipeline.py
+-rw-r--r--   0        0        0     7528 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/pty_util.py
+-rw-r--r--   0        0        0     6883 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/redirect.py
+-rw-r--r--   0        0        0     3348 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/result.py
+-rw-r--r--   0        0        0    34446 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/runner.py
+-rw-r--r--   0        0        0     4214 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/util.py
+-rw-r--r--   0        0        0    10066 2021-11-10 18:11:43.815179 shellous-0.9.3/shellous/watcher.py
+-rw-r--r--   0        0        0     9287 2021-11-10 18:11:55.194970 shellous-0.9.3/setup.py
+-rw-r--r--   0        0        0     9034 2021-11-10 18:11:55.195791 shellous-0.9.3/PKG-INFO
```

### Comparing `shellous-0.9.2/LICENSE` & `shellous-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/README.md` & `shellous-0.9.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -193,15 +193,15 @@
 'README.md\n'
 ```
 
 Use ~ to write to a command instead.
 
 ```pycon
 >>> buf = bytearray()
->>> cmd = sh("ls") | sh("tee", ~sh("grep", "README") | buf) | shellous.DEVNULL
+>>> cmd = sh("ls") | sh("tee", sh("grep", "README").writable | buf) | shellous.DEVNULL
 >>> await cmd
 ''
 >>> buf
 bytearray(b'README.md\n')
 ```
 
 Async With & For
```

### Comparing `shellous-0.9.2/pyproject.toml` & `shellous-0.9.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shellous"
-version = "0.9.2"
+version = "0.9.3"
 description = "Async Processes and Pipelines"
 license = "Apache-2.0"
 authors = ["Bill Fisher <william.w.fisher@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/byllyfish/shellous"
 classifiers = [
   "Development Status :: 4 - Beta",
```

### Comparing `shellous-0.9.2/shellous/__init__.py` & `shellous-0.9.3/shellous/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 .. include:: ../README.md
 """
 __docformat__ = "restructuredtext"
 
-__version__ = "0.9.2"
+__version__ = "0.9.3"
 
 # pylint: disable=cyclic-import
 from .command import CmdContext, Command, Options  # noqa: F401
 from .pipeline import Pipeline  # noqa: F401
 from .pty_util import cbreak, cooked, raw  # noqa: F401
 from .redirect import Redirect
 from .result import PipeResult, Result, ResultError  # noqa: F401
```

### Comparing `shellous-0.9.2/shellous/command.py` & `shellous-0.9.3/shellous/command.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
     pass_fds: Iterable[int] = ()
     "File descriptors to pass to the command."
 
     pass_fds_close: bool = False
     "True if pass_fds should be closed after subprocess launch."
 
-    write_mode: bool = False
+    writable: bool = False
     "True if using process substitution in write mode."
 
     _start_new_session: bool = False
     "True if child process should start a new session with setsid()."
 
     _preexec_fn: _Preexec_Fn_T = None
     "Function to call in child process after fork from parent."
@@ -225,15 +225,15 @@
         exit_codes=_UNSET,
         timeout=_UNSET,
         cancel_timeout=_UNSET,
         cancel_signal=_UNSET,
         alt_name=_UNSET,
         pass_fds=_UNSET,
         pass_fds_closed=_UNSET,
-        write_mode=_UNSET,
+        writable=_UNSET,
         _start_new_session=_UNSET,
         _preexec_fn=_UNSET,
         pty=_UNSET,
         close_fds=_UNSET,
         audit_callback=_UNSET,
     ) -> "CmdContext":
         """Return new context with custom options set.
@@ -367,15 +367,15 @@
         exit_codes: Unset[Optional[set]] = _UNSET,
         timeout: Unset[Optional[float]] = _UNSET,
         cancel_timeout: Unset[float] = _UNSET,
         cancel_signal: Unset[Optional[signal.Signals]] = _UNSET,
         alt_name: Unset[Optional[str]] = _UNSET,
         pass_fds: Unset[Iterable[int]] = _UNSET,
         pass_fds_close: Unset[bool] = _UNSET,
-        write_mode: Unset[bool] = _UNSET,
+        writable: Unset[bool] = _UNSET,
         _start_new_session: Unset[bool] = _UNSET,
         _preexec_fn: Unset[_Preexec_Fn_T] = _UNSET,
         pty: Unset[bool] = _UNSET,
         close_fds: Unset[bool] = _UNSET,
         audit_callback: Unset[_Audit_Fn_T] = _UNSET,
     ) -> "Command":
         """Return new command with custom options set.
@@ -433,15 +433,15 @@
         **pass_fds** (Iterable[int]) default=()<br>
         Specify open file descriptors to pass to the subprocess.
 
         **pass_fds_close** (bool) default=False<br>
         Close the file descriptors in `pass_fds` immediately in the current
         process immediately after launching the subprocess.
 
-        **write_mode** (bool) default=False<br>
+        **writable** (bool) default=False<br>
         Used to indicate process substitution is writing.
 
         **_start_new_session** (bool) default=False<br>
         Provided for testing purposes only.
 
         **_preexec_fn** (Callable() | None) default=None<br>
         Provided for testing purposes only.
@@ -571,15 +571,22 @@
 
     def __rshift__(self, rhs):
         "Right shift operator is used to build pipelines."
         if isinstance(rhs, STDOUT_APPEND_TYPES):
             return self.stdout(rhs, append=True)
         return NotImplemented
 
-    def __invert__(self):
-        "Unary ~ operator sets write_mode to True."
-        return self.set(write_mode=True)
+    def __mod__(self, rhs):
+        "Modulo operator is used to concatenate commands."
+        if isinstance(rhs, Command):
+            return self(rhs.args)
+        return NotImplemented
+
+    @property
+    def writable(self):
+        "Set `writable` to True."
+        return self.set(writable=True)
 
 
 def _check_args(out, append):
     if append and not isinstance(out, STDOUT_APPEND_TYPES):
         raise TypeError(f"{type(out)} does not support append")
```

### Comparing `shellous-0.9.2/shellous/harvest.py` & `shellous-0.9.3/shellous/harvest.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/log.py` & `shellous-0.9.3/shellous/log.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/pipeline.py` & `shellous-0.9.3/shellous/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,17 +49,17 @@
 
     def stderr(self, error, *, append=False, close=False) -> "Pipeline":
         "Set stderr on the last command of the pipeline."
         new_last = self.commands[-1].stderr(error, append=append, close=close)
         new_commands = self.commands[0:-1] + (new_last,)
         return dataclasses.replace(self, commands=new_commands)
 
-    def _set_write_mode(self):
+    def _set_writable(self):
         "Set write_mode=True on last command of the pipeline."
-        new_last = self.commands[-1].set(write_mode=True)
+        new_last = self.commands[-1].set(writable=True)
         new_commands = self.commands[0:-1] + (new_last,)
         return dataclasses.replace(self, commands=new_commands)
 
     def coro(self):
         "Return coroutine object for pipeline."
         return PipeRunner.run_pipeline(self)
 
@@ -113,17 +113,18 @@
         return NotImplemented
 
     def __rshift__(self, rhs):
         if isinstance(rhs, STDOUT_APPEND_TYPES):
             return self.stdout(rhs, append=True)
         return NotImplemented
 
-    def __invert__(self):
-        "Set write_mode=True option on last command of pipeline."
-        return self._set_write_mode()
+    @property
+    def writable(self):
+        "Set writable=True option on last command of pipeline."
+        return self._set_writable()
 
     def __await__(self):
         return self.coro().__await__()
 
     async def __aenter__(self):
         "Enter the async context manager."
         return await context_aenter(id(self), self.run())
```

### Comparing `shellous-0.9.2/shellous/pty_util.py` & `shellous-0.9.3/shellous/pty_util.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/redirect.py` & `shellous-0.9.3/shellous/redirect.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/result.py` & `shellous-0.9.3/shellous/result.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/runner.py` & `shellous-0.9.3/shellous/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     return isinstance(ex, asyncio.CancelledError)
 
 
 def _is_cmd(cmd):
     return isinstance(cmd, (shellous.Command, shellous.Pipeline))
 
 
-def _is_write_mode(cmd):
-    "Return true if command/pipeline has write_mode set."
+def _is_writable(cmd):
+    "Return true if command/pipeline has `writable` set."
     if isinstance(cmd, shellous.Pipeline):
         # Pipelines need to check both the last/first commands.
-        return cmd.options.write_mode or cmd[0].options.write_mode
-    return cmd.options.write_mode
+        return cmd.options.writable or cmd[0].options.writable
+    return cmd.options.writable
 
 
 def _split(encoding):
     if encoding is None:
         raise TypeError("when encoding is None, input must be bytes")
     return encoding.split(maxsplit=1)
 
@@ -111,15 +111,15 @@
 
         for arg in self.command.args:
             if not _is_cmd(arg):
                 new_args.append(arg)
                 continue
 
             (read_fd, write_fd) = os.pipe()
-            if _is_write_mode(arg):
+            if _is_writable(arg):
                 new_args.append(f"/dev/fd/{write_fd}")
                 pass_fds.append(write_fd)
                 subcmd = arg.stdin(read_fd, close=True)
             else:
                 new_args.append(f"/dev/fd/{read_fd}")
                 pass_fds.append(read_fd)
                 subcmd = arg.stdout(write_fd, close=True)
@@ -441,15 +441,15 @@
 
         except (asyncio.CancelledError, asyncio.TimeoutError) as ex:
             LOGGER.warning("Runner.kill %r (ex)=%r", self, ex)
             if _is_cancelled(ex):
                 self._set_cancelled()
             await self._kill_wait()
 
-        except Exception as ex:
+        except (Exception, GeneratorExit) as ex:
             LOGGER.warning("Runner.kill %r ex=%r", self, ex)
             await self._kill_wait()
             raise
 
     def _send_signal(self, sig):
         "Send a signal to the process."
```

### Comparing `shellous-0.9.2/shellous/util.py` & `shellous-0.9.3/shellous/util.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/shellous/watcher.py` & `shellous-0.9.3/shellous/watcher.py`

 * *Files identical despite different names*

### Comparing `shellous-0.9.2/setup.py` & `shellous-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['immutables>=0.16,<0.17']
 
 setup_kwargs = {
     'name': 'shellous',
-    'version': '0.9.2',
+    'version': '0.9.3',
     'description': 'Async Processes and Pipelines',
-    'long_description': 'Async Processes and Pipelines\n=============================\n\n[![docs](https://img.shields.io/badge/-documentation-informational)](https://byllyfish.github.io/shellous/shellous.html) [![PyPI](https://img.shields.io/pypi/v/shellous)](https://pypi.org/project/shellous/) [![CI](https://github.com/byllyfish/shellous/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/shellous/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/shellous/branch/main/graph/badge.svg?token=W44NZE89AW)](https://codecov.io/gh/byllyfish/shellous) [![Downloads](https://pepy.tech/badge/shellous)](https://pepy.tech/project/shellous)\n\nshellous provides a concise API for running subprocesses using asyncio. It is \nsimilar to and inspired by [sh](https://pypi.org/project/sh/).\n\n```python\nimport asyncio\nimport shellous\n\nsh = shellous.context()\n\nasync def main():\n    result = await (sh("ls") | sh("grep", "README"))\n    print(result)\n\nasyncio.run(main())\n```\n\nBenefits\n--------\n\n- Run programs asychronously in a single line.\n- Easily capture output or redirect stdin, stdout and stderr to files, memory buffers or loggers.\n- Easily construct [pipelines](https://en.wikipedia.org/wiki/Pipeline_(Unix)) and use [process substitution](https://en.wikipedia.org/wiki/Process_substitution).\n- Run a program with a pseudo-terminal (pty).\n- Runs on Linux, MacOS, FreeBSD and Windows.\n- Monitor processes being started and stopped with `audit_callback` API.\n\nRequirements\n------------\n\n- Requires Python 3.9 or later.\n- Requires an asyncio event loop.\n- Process substitution requires a Unix system with /dev/fd support.\n- Pseudo-terminals require a Unix system. Pty\'s do not work on [uvloop](https://github.com/MagicStack/uvloop).\n- [FastChildWatcher](https://docs.python.org/3/library/asyncio-policy.html#asyncio.FastChildWatcher) is not supported.\n\nBasic Usage\n-----------\n\nStart the asyncio REPL by typing `python3 -m asyncio`, and import the **shellous** module:\n\n```pycon\n>>> import shellous\n```\n\nBefore we can do anything else, we need to create a **context**. Store the context in a \nshort variable name like `sh` because we\'ll be typing it a lot.\n\n```pycon\n>>> sh = shellous.context()\n```\n\nNow, we\'re ready to run our first command. Here\'s one that runs `echo "hello, world"`.\n\n```pycon\n>>> await sh("echo", "hello, world")\n\'hello, world\\n\'\n```\n\nThe first argument is the program name. It is followed by zero or more separate arguments.\n\nA command does not run until you `await` it. Here, we create our own echo command with "-n"\nto omit the newline. Note, `echo("abc")` is the same as `echo -n "abc"`.\n\n```pycon\n>>> echo = sh("echo", "-n")\n>>> await echo("abc")\n\'abc\'\n```\n\n\nResults and Exit Codes\n----------------------\n\nWhen you `await` a command, it captures the standard output and returns it. You can optionally have the\ncommand return a `Result` object. The `Result` object will contain more information about the command \nexecution including the `exit_code`. To return a result object, set `return_result` option to `True`.\n\n```pycon\n>>> await echo("abc").set(return_result=True)\nResult(output_bytes=b\'abc\', exit_code=0, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\nThe above command had an exit_code of 0.\n\nIf a command exits with a non-zero exit code, it raises a `ResultError` exception that contains\nthe `Result` object.\n\n```pycon\n>>> await sh("cat", "does_not_exist")\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=1, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\n\nRedirecting Standard Input\n--------------------------\n\nYou can change the standard input of a command by using the `|` operator.\n\n```pycon\n>>> cmd = "abc" | sh("wc", "-c")\n>>> await cmd\n\'       3\\n\'\n```\n\nTo redirect stdin using a file\'s contents, use a `Path` object from `pathlib`.\n\n```pycon\n>>> from pathlib import Path\n>>> cmd = Path("LICENSE") | sh("wc", "-l")\n>>> await cmd\n\'     201\\n\'\n```\n\n\nRedirecting Standard Output\n---------------------------\n\nTo redirect standard output, use the `|` operator.\n\n```pycon\n>>> output_file = Path("/tmp/output_file")\n>>> cmd = sh("echo", "abc") | output_file\n>>> await cmd\n\'\'\n>>> output_file.read_bytes()\nb\'abc\\n\'\n```\n\nTo redirect standard output with append, use the `>>` operator.\n\n```pycon\n>>> cmd = sh("echo", "def") >> output_file\n>>> await cmd\n\'\'\n>>> output_file.read_bytes()\nb\'abc\\ndef\\n\'\n```\n\n\nRedirecting Standard Error\n--------------------------\n\nBy default, standard error is not captured. To redirect standard error, use the `stderr`\nmethod.\n\n```pycon\n>>> cmd = sh("cat", "does_not_exist").stderr(shellous.STDOUT)\n>>> await cmd.set(exit_codes={0,1})\n\'cat: does_not_exist: No such file or directory\\n\'\n```\n\nYou can redirect standard error to a file or path. \n\nTo redirect standard error to the hosting program\'s `sys.stderr`, use the INHERIT redirect\noption.\n\n```pycon\n>>> cmd = sh("cat", "does_not_exist").stderr(shellous.INHERIT)\n>>> await cmd\ncat: does_not_exist: No such file or directory\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=1, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\n\nPipelines\n---------\n\nYou can create a pipeline by combining commands using the `|` operator.\n\n```pycon\n>>> pipe = sh("ls") | sh("grep", "README")\n>>> await pipe\n\'README.md\\n\'\n```\n\nProcess Substitution (Unix Only)\n--------------------------------\n\nYou can pass a shell command as an argument to another.\n\n```pycon\n>>> cmd = sh("grep", "README", sh("ls"))\n>>> await cmd\n\'README.md\\n\'\n```\n\nUse ~ to write to a command instead.\n\n```pycon\n>>> buf = bytearray()\n>>> cmd = sh("ls") | sh("tee", ~sh("grep", "README") | buf) | shellous.DEVNULL\n>>> await cmd\n\'\'\n>>> buf\nbytearray(b\'README.md\\n\')\n```\n\nAsync With & For\n----------------\n\nYou can loop over a command\'s output by using the context manager as an iterator.\n\n```pycon\n>>> async with pipe as run:\n...   async for line in run:\n...     print(line.rstrip())\n... \nREADME.md\n```\n\n> <span style="font-size:1.5em;">⚠️ </span> You can also acquire an async iterator directly from\n> the command or pipeline object. This is discouraged because you will have less control over the final\n> clean up of the command invocation than with a context manager.\n\n```pycon\n>>> async for line in pipe:   # Use caution!\n...   print(line.rstrip())\n... \nREADME.md\n```\n\nYou can use `async with` to interact with the process streams directly. You have to be careful; you\nare responsible for correctly reading and writing multiple streams at the same time.\n\n```pycon\n>>> async with pipe as run:\n...   data = await run.stdout.readline()\n...   print(data)\n... \nb\'README.md\\n\'\n```\n\nCancellation\n------------\n\nWhen a command is cancelled, shellous terminates the process and raises a `CancelledError`.\n\nYou can retrieve the partial result by setting `incomplete_result` to True. Shellous will return a\n`ResultError` when the specified command is cancelled.\n\n```pycon\n>>> sleep = sh("sleep", 60).set(incomplete_result=True)\n>>> t = asyncio.create_task(sleep.coro())\n>>> t.cancel()\nTrue\n>>> await t\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=-15, cancelled=True, encoding=\'utf-8\', extra=None)\n```\n\nWhen you use `incomplete_result`, your code should respect the `cancelled` attribute in the Result object. \nOtherwise, your code may swallow the CancelledError.\n\nPseudo-Terminal Support (Unix Only)\n-----------------------------------\n\nTo run a command through a pseudo-terminal, set the `pty` option to True. Alternatively, you can pass\na function to configure the tty mode and size.\n\n```pycon\n>>> ls = sh("ls").set(pty=shellous.cooked(cols=40, rows=10, echo=False))\n>>> await ls("README.md", "CHANGELOG.md")\n\'CHANGELOG.md\\tREADME.md\\r\\n\'\n```\n\nContext Objects\n---------------\n\nYou can specify shared command settings in a context object. Context objects are immutable,\nso you must store the result of your changes in a new variable.\n\n```pycon\n>>> auditor = lambda phase, info: print(phase, info["runner"].name)\n>>> sh1 = sh.set(audit_callback=auditor)\n```\n\nNow all commands run with `sh1` will log their progress using the audit callback.\n\n```pycon\n>>> await sh1("echo", "goodbye")\nstart echo\nstop echo\n\'goodbye\\n\'\n```\n',
+    'long_description': 'Async Processes and Pipelines\n=============================\n\n[![docs](https://img.shields.io/badge/-documentation-informational)](https://byllyfish.github.io/shellous/shellous.html) [![PyPI](https://img.shields.io/pypi/v/shellous)](https://pypi.org/project/shellous/) [![CI](https://github.com/byllyfish/shellous/actions/workflows/ci.yml/badge.svg)](https://github.com/byllyfish/shellous/actions/workflows/ci.yml) [![codecov](https://codecov.io/gh/byllyfish/shellous/branch/main/graph/badge.svg?token=W44NZE89AW)](https://codecov.io/gh/byllyfish/shellous) [![Downloads](https://pepy.tech/badge/shellous)](https://pepy.tech/project/shellous)\n\nshellous provides a concise API for running subprocesses using asyncio. It is \nsimilar to and inspired by [sh](https://pypi.org/project/sh/).\n\n```python\nimport asyncio\nimport shellous\n\nsh = shellous.context()\n\nasync def main():\n    result = await (sh("ls") | sh("grep", "README"))\n    print(result)\n\nasyncio.run(main())\n```\n\nBenefits\n--------\n\n- Run programs asychronously in a single line.\n- Easily capture output or redirect stdin, stdout and stderr to files, memory buffers or loggers.\n- Easily construct [pipelines](https://en.wikipedia.org/wiki/Pipeline_(Unix)) and use [process substitution](https://en.wikipedia.org/wiki/Process_substitution).\n- Run a program with a pseudo-terminal (pty).\n- Runs on Linux, MacOS, FreeBSD and Windows.\n- Monitor processes being started and stopped with `audit_callback` API.\n\nRequirements\n------------\n\n- Requires Python 3.9 or later.\n- Requires an asyncio event loop.\n- Process substitution requires a Unix system with /dev/fd support.\n- Pseudo-terminals require a Unix system. Pty\'s do not work on [uvloop](https://github.com/MagicStack/uvloop).\n- [FastChildWatcher](https://docs.python.org/3/library/asyncio-policy.html#asyncio.FastChildWatcher) is not supported.\n\nBasic Usage\n-----------\n\nStart the asyncio REPL by typing `python3 -m asyncio`, and import the **shellous** module:\n\n```pycon\n>>> import shellous\n```\n\nBefore we can do anything else, we need to create a **context**. Store the context in a \nshort variable name like `sh` because we\'ll be typing it a lot.\n\n```pycon\n>>> sh = shellous.context()\n```\n\nNow, we\'re ready to run our first command. Here\'s one that runs `echo "hello, world"`.\n\n```pycon\n>>> await sh("echo", "hello, world")\n\'hello, world\\n\'\n```\n\nThe first argument is the program name. It is followed by zero or more separate arguments.\n\nA command does not run until you `await` it. Here, we create our own echo command with "-n"\nto omit the newline. Note, `echo("abc")` is the same as `echo -n "abc"`.\n\n```pycon\n>>> echo = sh("echo", "-n")\n>>> await echo("abc")\n\'abc\'\n```\n\n\nResults and Exit Codes\n----------------------\n\nWhen you `await` a command, it captures the standard output and returns it. You can optionally have the\ncommand return a `Result` object. The `Result` object will contain more information about the command \nexecution including the `exit_code`. To return a result object, set `return_result` option to `True`.\n\n```pycon\n>>> await echo("abc").set(return_result=True)\nResult(output_bytes=b\'abc\', exit_code=0, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\nThe above command had an exit_code of 0.\n\nIf a command exits with a non-zero exit code, it raises a `ResultError` exception that contains\nthe `Result` object.\n\n```pycon\n>>> await sh("cat", "does_not_exist")\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=1, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\n\nRedirecting Standard Input\n--------------------------\n\nYou can change the standard input of a command by using the `|` operator.\n\n```pycon\n>>> cmd = "abc" | sh("wc", "-c")\n>>> await cmd\n\'       3\\n\'\n```\n\nTo redirect stdin using a file\'s contents, use a `Path` object from `pathlib`.\n\n```pycon\n>>> from pathlib import Path\n>>> cmd = Path("LICENSE") | sh("wc", "-l")\n>>> await cmd\n\'     201\\n\'\n```\n\n\nRedirecting Standard Output\n---------------------------\n\nTo redirect standard output, use the `|` operator.\n\n```pycon\n>>> output_file = Path("/tmp/output_file")\n>>> cmd = sh("echo", "abc") | output_file\n>>> await cmd\n\'\'\n>>> output_file.read_bytes()\nb\'abc\\n\'\n```\n\nTo redirect standard output with append, use the `>>` operator.\n\n```pycon\n>>> cmd = sh("echo", "def") >> output_file\n>>> await cmd\n\'\'\n>>> output_file.read_bytes()\nb\'abc\\ndef\\n\'\n```\n\n\nRedirecting Standard Error\n--------------------------\n\nBy default, standard error is not captured. To redirect standard error, use the `stderr`\nmethod.\n\n```pycon\n>>> cmd = sh("cat", "does_not_exist").stderr(shellous.STDOUT)\n>>> await cmd.set(exit_codes={0,1})\n\'cat: does_not_exist: No such file or directory\\n\'\n```\n\nYou can redirect standard error to a file or path. \n\nTo redirect standard error to the hosting program\'s `sys.stderr`, use the INHERIT redirect\noption.\n\n```pycon\n>>> cmd = sh("cat", "does_not_exist").stderr(shellous.INHERIT)\n>>> await cmd\ncat: does_not_exist: No such file or directory\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=1, cancelled=False, encoding=\'utf-8\', extra=None)\n```\n\n\nPipelines\n---------\n\nYou can create a pipeline by combining commands using the `|` operator.\n\n```pycon\n>>> pipe = sh("ls") | sh("grep", "README")\n>>> await pipe\n\'README.md\\n\'\n```\n\nProcess Substitution (Unix Only)\n--------------------------------\n\nYou can pass a shell command as an argument to another.\n\n```pycon\n>>> cmd = sh("grep", "README", sh("ls"))\n>>> await cmd\n\'README.md\\n\'\n```\n\nUse ~ to write to a command instead.\n\n```pycon\n>>> buf = bytearray()\n>>> cmd = sh("ls") | sh("tee", sh("grep", "README").writable | buf) | shellous.DEVNULL\n>>> await cmd\n\'\'\n>>> buf\nbytearray(b\'README.md\\n\')\n```\n\nAsync With & For\n----------------\n\nYou can loop over a command\'s output by using the context manager as an iterator.\n\n```pycon\n>>> async with pipe as run:\n...   async for line in run:\n...     print(line.rstrip())\n... \nREADME.md\n```\n\n> <span style="font-size:1.5em;">⚠️ </span> You can also acquire an async iterator directly from\n> the command or pipeline object. This is discouraged because you will have less control over the final\n> clean up of the command invocation than with a context manager.\n\n```pycon\n>>> async for line in pipe:   # Use caution!\n...   print(line.rstrip())\n... \nREADME.md\n```\n\nYou can use `async with` to interact with the process streams directly. You have to be careful; you\nare responsible for correctly reading and writing multiple streams at the same time.\n\n```pycon\n>>> async with pipe as run:\n...   data = await run.stdout.readline()\n...   print(data)\n... \nb\'README.md\\n\'\n```\n\nCancellation\n------------\n\nWhen a command is cancelled, shellous terminates the process and raises a `CancelledError`.\n\nYou can retrieve the partial result by setting `incomplete_result` to True. Shellous will return a\n`ResultError` when the specified command is cancelled.\n\n```pycon\n>>> sleep = sh("sleep", 60).set(incomplete_result=True)\n>>> t = asyncio.create_task(sleep.coro())\n>>> t.cancel()\nTrue\n>>> await t\nTraceback (most recent call last):\n  ...\nshellous.result.ResultError: Result(output_bytes=b\'\', exit_code=-15, cancelled=True, encoding=\'utf-8\', extra=None)\n```\n\nWhen you use `incomplete_result`, your code should respect the `cancelled` attribute in the Result object. \nOtherwise, your code may swallow the CancelledError.\n\nPseudo-Terminal Support (Unix Only)\n-----------------------------------\n\nTo run a command through a pseudo-terminal, set the `pty` option to True. Alternatively, you can pass\na function to configure the tty mode and size.\n\n```pycon\n>>> ls = sh("ls").set(pty=shellous.cooked(cols=40, rows=10, echo=False))\n>>> await ls("README.md", "CHANGELOG.md")\n\'CHANGELOG.md\\tREADME.md\\r\\n\'\n```\n\nContext Objects\n---------------\n\nYou can specify shared command settings in a context object. Context objects are immutable,\nso you must store the result of your changes in a new variable.\n\n```pycon\n>>> auditor = lambda phase, info: print(phase, info["runner"].name)\n>>> sh1 = sh.set(audit_callback=auditor)\n```\n\nNow all commands run with `sh1` will log their progress using the audit callback.\n\n```pycon\n>>> await sh1("echo", "goodbye")\nstart echo\nstop echo\n\'goodbye\\n\'\n```\n',
     'author': 'Bill Fisher',
     'author_email': 'william.w.fisher@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/byllyfish/shellous',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `shellous-0.9.2/PKG-INFO` & `shellous-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellous
-Version: 0.9.2
+Version: 0.9.3
 Summary: Async Processes and Pipelines
 Home-page: https://github.com/byllyfish/shellous
 License: Apache-2.0
 Author: Bill Fisher
 Author-email: william.w.fisher@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -214,15 +214,15 @@
 'README.md\n'
 ```
 
 Use ~ to write to a command instead.
 
 ```pycon
 >>> buf = bytearray()
->>> cmd = sh("ls") | sh("tee", ~sh("grep", "README") | buf) | shellous.DEVNULL
+>>> cmd = sh("ls") | sh("tee", sh("grep", "README").writable | buf) | shellous.DEVNULL
 >>> await cmd
 ''
 >>> buf
 bytearray(b'README.md\n')
 ```
 
 Async With & For
```

