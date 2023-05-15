# Comparing `tmp/ttrace-0.1.6.tar.gz` & `tmp/ttrace-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttrace-0.1.6.tar", max compression
+gzip compressed data, was "ttrace-0.1.7.tar", max compression
```

## Comparing `ttrace-0.1.6.tar` & `ttrace-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     2632 2023-03-05 10:05:35.397583 ttrace-0.1.6/Readme.md
--rw-r--r--   0        0        0     1741 2023-03-05 10:07:22.683714 ttrace-0.1.6/pyproject.toml
--rwxr-xr-x   0        0        0    20327 2023-03-05 10:05:35.407583 ttrace-0.1.6/ttrace/__init__.py
--rw-r--r--   0        0        0        0 2023-03-05 10:05:35.407583 ttrace-0.1.6/ttrace/utils/__init__.py
--rw-r--r--   0        0        0     4895 2023-03-05 10:05:35.408583 ttrace-0.1.6/ttrace/utils/treestuff.py
--rw-r--r--   0        0        0     3543 1970-01-01 00:00:00.000000 ttrace-0.1.6/setup.py
--rw-r--r--   0        0        0     3215 1970-01-01 00:00:00.000000 ttrace-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     2778 2023-04-26 09:09:07.923462 ttrace-0.1.7/Readme.md
+-rw-r--r--   0        0        0     1753 2023-04-26 09:06:58.455095 ttrace-0.1.7/pyproject.toml
+-rwxr-xr-x   0        0        0    25478 2023-05-15 13:57:36.185804 ttrace-0.1.7/ttrace/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-01 06:28:10.240369 ttrace-0.1.7/ttrace/utils/__init__.py
+-rw-r--r--   0        0        0     4941 2023-05-15 13:57:36.053811 ttrace-0.1.7/ttrace/utils/treestuff.py
+-rw-r--r--   0        0        0     3361 1970-01-01 00:00:00.000000 ttrace-0.1.7/PKG-INFO
```

### Comparing `ttrace-0.1.6/Readme.md` & `ttrace-0.1.7/Readme.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 # ttrace - strace as a tree
 
 Uses `strace` to trace a program call and displays what's going on in a human
 friendly manner.
 
 [Project page](https://projects.om-office.de/frans/ttrace)
 
-## Usage
 
-Currently you just run
+## Installation and Usage
 
+Install `ttrace` via pip:
 ```
-ttrace.py <CMD>
+[<python executable> -m] pip install [-U] ttrace
 ```
-as you would with `strace` but without any arguments to `ttrace` (`strace` will
-be called with a bunch of arguments automatically).
 
-See next section to see what's coming.
+A new executable is then provided which can be used instead of `strace`:
+```
+ttrace [<ARGS>] <CMD>
+```
+Note that you would'nt provide `strace` arguments since `ttrace` provides them
+automatically.
+
+Alternatively you can clone and use the current development tree, see below.
+
 
 ## Intended interface
 
 The following commands and outputs reflect the current development plan:
 
 ```sh
 ttrace <CMD|LOGFILE>
@@ -63,43 +69,50 @@
 * strace console
 * console with only warning character (whatever that means)
 
 ```sh
 ttrace --timing <CMD>
 ```
 
+### ToDo for v1.0
+
+* trace process termination
+* output growing process tree
+* report / visualize abnormal process termination
+* report / visualize file access
+* optionally turn PIDs into PID counters for comparability
+* optionally print timestamp, pid, line number
+* no color
+* logging
+
 
 ### Other ideas
 
+* compare trace files on abstract level
 * trace changes environment
 * trace docker image usage
 * highlight failed processes
 
-## Installation
 
 ## Development & Contribution
 
 ```
 pip3 install -U poetry pre-commit
 git clone --recurse-submodules https://projects.om-office.de/frans/ttrace.git
 cd ttrace
 pre-commit install
 # if you need a specific version of Python inside your dev environment
-poetry env use /home/frafue/.pyenv/versions/3.10.4/bin/python3
+poetry env use ~/.pyenv/versions/3.10.4/bin/python3
 poetry install
 ```
 
-## License
 
-For all code contained in this repository the rules of GPLv3 apply unless
-otherwise noted. That means that you can do what you want with the source
-code as long as you make the files with their original copyright notice
-and all modifications available.
+## License
 
-See [GNU / GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) for details.
+See `License.md`
 
 
 ## Read
 
 * [The Difference Between fork(), vfork(), exec() and clone()](https://www.baeldung.com/linux/fork-vfork-exec-clone)
 * [HN: The Magic of strace](https://news.ycombinator.com/item?id=7155799)
 * [The Magic of strace (archive.org)](https://web.archive.org/web/20160116001752/http://chadfowler.com/blog/2014/01/26/the-magic-of-strace/)
```

### Comparing `ttrace-0.1.6/pyproject.toml` & `ttrace-0.1.7/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ttrace"
-version = "0.1.6"
+version = "0.1.7"
 description = "Makes use of strace"
 authors = ["Frans Fürst <frans.fuerst+gitlab@protonmail.com>"]
 repository = "https://projects.om-office.de/frans/ttrace.git"
 readme = "Readme.md"
 packages = [
   {include = "ttrace"}
 ]
@@ -40,14 +40,15 @@
 include = '\.pyi?$'
 fast = true
 exclude = '''
 (
   /(                        # exclude a few common directories in the
     \.git                   # root of the project
     | \.pytest_cache
+    | untracked
     | \.venv
   ))
 '''
 
 [tool.isort]
 profile = "black"
 
@@ -58,20 +59,19 @@
 no_implicit_optional = "True"
 check_untyped_defs = "True"
 warn_return_any = "True"
 warn_unused_ignores = "True"
 show_error_codes = "True"
 exclude = [
     '\.venv',
+    'untracked',
 ]
 
 [tool.pylint]
-extension-pkg-whitelist="pygame"
-
-ignore = [".venv"]
+ignore = [".venv", "untracked"]
 
 # Files or directories matching the regular expression patterns are skipped. The
 # regex matches against base names, not paths. The default value ignores Emacs
 # file locks
 ignore-patterns = ["^\\.#"]
 
 # Use multiple processes to speed up Pylint. Specifying 0 will auto-detect the
```

### Comparing `ttrace-0.1.6/ttrace/__init__.py` & `ttrace-0.1.7/ttrace/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,57 +22,69 @@
 from dataclasses import dataclass
 from itertools import chain
 from pathlib import Path
 from typing import Any, ClassVar, NoReturn, Protocol, TextIO, Type, TypeVar
 
 import aiofiles
 
-from .utils.treestuff import attributed_tree, colored, get_node, insert
+from ttrace.utils.treestuff import attributed_tree, colored, get_node, insert
 
-PPID = r"\d*"
+PPID = r"\d+"
 PTIME = r"\d{10}\.\d{6}"
-PFNAME = r"([a-z0-9_]*|\?*)"
-PHEX = r"0x[0-9a-f]*"
+PFNAME = r"([a-z0-9_]+|\?+)"
+PHEX = r"0x[0-9a-f]+"
 PCOMMENT = r"\/\*\s(.*)\s\*\/"
-PRESULT = rf"(\?|-?\d*|{PHEX})( [A-Z]*)?( \(.*\))?( {PCOMMENT})?"
+PRESULT = rf"(\?|-?\d+|{PHEX})( [A-Z_]+)?( \(.*\))?( {PCOMMENT})?"
 PPATH = r".*"
-PFLAGS = r"[A-Z_\|]*"
-PCONST = r"([A-Z_]*|\d*)"
+PFLAGS = r"[A-Z_\|]+"
+PCONST = r"([A-Z_]+|\d+)"
 PPERMISSION = r"0[0-7]{3}|000"
 PANYTHING = r".*"
 
+# All functions ttrace can somehow make use of
+IMPLEMENTED_COMMANDS = set("execve openat vfork clone clone3 exit_group exited write".split())
+
+# All function names I've stumbled upon so far
 ALL_COMMANDS = set(
     "exited "
-    "execve openat vfork clone clone3 "
+    "execve openat vfork clone clone3 exit_group "
     "getrusage fstatfs dup getegid rt_sigaction rmdir close rt_sigprocmask "
     "getrandom pipe2 write getcwd lseek munmap getppid unlinkat clock_nanosleep "
     "mprotect getpid readlink getpgrp setresuid sched_getaffinity fcntl umask "
     "gettid wait4 getuid rt_sigreturn sysinfo getdents64 sigaltstack "
-    "geteuid chmod exit_group set_tid_address setresgid brk uname access "
+    "geteuid chmod set_tid_address setresgid brk uname access "
     "fsetxattr mkdir pread64 set_robust_list rseq faccessat2 ioctl getgid "
     "renameat2 newfstatat tgkill mmap statx unlink splice prlimit64 dup2 "
-    "getgroups kill arch_prctl read statfs rename chdir symlinkat fadvise64".split()
+    "getgroups kill arch_prctl read statfs rename chdir symlinkat fadvise64 "
+    "futex socket connect readlinkat getpeername bind close_range epoll_create1 "
+    "fchdir poll lstat clock_getres socketpair renameat recvmmsg sched_yield fchownat "
+    "fgetxattr epoll_ctl accept4 eventfd2 timerfd_settime restart_syscall getsockname "
+    "recvmsg dup3 stat epoll_create prctl ftruncate writev sendmmsg setuid mremap "
+    "getsockopt fchown setitimer rt_sigtimedwait pselect6 fchmod fstat utimensat sendto "
+    "alarm setsid capget setsockopt sendmsg shutdown symlink madvise timerfd_create "
+    "epoll_wait fchmodat fallocate listen recvfrom times capset".split()
 )
 
 
 def parse_args(args: Sequence[str] | None = None) -> tuple[Namespace, Sequence[str]]:
     """Returns parsed arguments until the first
     >>> parse_args(["-v", "--grep", "abc", "foo", "-v", "bar"])
-    (Namespace(verbose=True, record=None, grep='abc'), ['foo', '-v', 'bar'])
+    (Namespace(verbose=True, no_color=False, record=None, grep='abc'), ['foo', '-v', 'bar'])
     """
 
     class MyArgumentParser(ArgumentParser):
         """Argument parser which not exits on error but raises an exception"""
 
         def error(self, message: str) -> NoReturn:
             """Just raises an error we can catch"""
             raise RuntimeError(message)
 
     parser = MyArgumentParser()
     parser.add_argument("--verbose", "-v", action="store_true")
+    parser.add_argument("--no-color", "-n", action="store_true")
     parser.add_argument("--record", "-r", type=Path)
     parser.add_argument("--grep", "-g", type=str)
 
     all_args = args or sys.argv[1:]
     for split_at in (i for i, e in reversed(list(enumerate(all_args))) if not e.startswith("-")):
         try:
             return parser.parse_args(all_args[:split_at]), all_args[split_at:]
@@ -101,32 +113,38 @@
     pid: int
     timestamp: str
     fname: str
     args: str
     result: str
     result_nr: int | None
     PATTERN: ClassVar[str] = (
-        rf"^({PPID})\s({PTIME})\s("
+        rf"^({PPID})\s+({PTIME})\s("
         rf"(({PFNAME})\(({PANYTHING})\)\s=\s({PRESULT}))"
-        rf"|(\+\+\+ (exited) with (-?\d*) \+\+\+)"
+        rf"|(\+\+\+ (exited) with (-?\d+) \+\+\+)"
         rf")$"
     )
 
     def __init__(self, args: tuple[str, ...]) -> None:
         self.pid = int(args[0])
         assert self.pid
         self.timestamp = args[1]
         self.fname = args[4] or args[14]
         assert self.fname
         self.args = args[6]
         self.result = args[7] or args[13]
         assert self.result
         result_nr_str = args[8] or args[15]
         assert result_nr_str is not None
-        self.result_nr = int(result_nr_str) if result_nr_str != "?" else None
+        self.result_nr = (
+            None
+            if result_nr_str == "?"
+            else int(result_nr_str, 16)
+            if result_nr_str.startswith("0x")
+            else int(result_nr_str)
+        )
         self.comment = args[12]
 
     def __repr__(self) -> str:
         return (
             f"strace<pid={self.pid}"
             f", t={self.timestamp}"
             f", cmd={self.fname}"
@@ -147,15 +165,15 @@
     """
 
     line: str
     pid: int
 
     PATTERN: ClassVar[
         str
-    ] = rf"^(({PPID})\s{PTIME}\s{PFNAME}\({PANYTHING})\s<unfinished\s\.\.\.>{PANYTHING}$"
+    ] = rf"^(({PPID})\s+{PTIME}\s{PFNAME}\({PANYTHING})\s<unfinished\s\.\.\.>{PANYTHING}$"
 
     def __init__(self, args: tuple[str, ...]) -> None:
         self.line = args[0]
         self.pid = int(args[1])
 
     def __repr__(self) -> str:
         return f"unfinished<pid={self.pid}>"
@@ -167,15 +185,15 @@
     line needed to stitch it to the previous `unfinished` element.
     >>> parse(ResumedType, "727862 1676908243.255635 <... wait4 resumed>blabla) = 727863")
     resumed<pid=727862>
     """
 
     pid: int
     line: str
-    PATTERN: ClassVar[str] = rf"^({PPID})\s{PTIME}\s<\.\.\. {PFNAME} resumed>({PANYTHING})$"
+    PATTERN: ClassVar[str] = rf"^({PPID})\s+{PTIME}\s<\.\.\. {PFNAME} resumed>({PANYTHING})$"
 
     def __init__(self, args: tuple[str, ...]) -> None:
         self.pid = int(args[0])
         self.line = args[2]
 
     def __repr__(self) -> str:
         return f"resumed<pid={self.pid}>"
@@ -211,26 +229,47 @@
     >>> parse(OpenatType, 'AT_FDCWD, "/usr/bin/print", O_RDONLY|O_CLOEXEC')
     openat<path='/usr/bin/print'>
     """
 
     position: str
     path: str
     flags: str
-    PATTERN: ClassVar[str] = rf'^([A-Z_]*|\d*),\s"({PANYTHING})", ({PFLAGS})(, ({PPERMISSION}))?$'
+    PATTERN: ClassVar[str] = rf'^([A-Z_]+|\d+),\s"({PANYTHING})", ({PFLAGS})(, ({PPERMISSION}))?$'
 
     def __init__(self, args: tuple[str, ...]) -> None:
         self.position = args[0]
         self.path = args[1]
         self.flags = args[2]
 
     def __repr__(self) -> str:
         return f"openat<path={self.path!r}>"
 
 
 @dataclass
+class WriteType:
+    """Content of a write() call,
+    >>> parse(OpenatType, 'AT_FDCWD, "/usr/bin/print", O_RDONLY|O_CLOEXEC')
+    openat<path='/usr/bin/print'>
+    """
+
+    filep: int
+    string: str
+    length: int
+    PATTERN: ClassVar[str] = rf'^(\d+),\s"({PANYTHING})"(\.\.\.)?,\s(\d+)$'
+
+    def __init__(self, args: tuple[str, ...]) -> None:
+        self.filep = int(args[0])
+        self.string = args[1]
+        self.length = int(args[3])
+
+    def __repr__(self) -> str:
+        return f"write<fp={self.filep}, string={self.string!r}>"
+
+
+@dataclass
 class VforkType:
     """Content of an vfork() call
     >>> parse(VforkType, '')
     vfork<>
     """
 
     PATTERN: ClassVar[str] = r"^$"
@@ -268,29 +307,29 @@
             f", flags={self.flags!r}, child_tidptr={self.child_tidptr!r}>"
         )
 
 
 @dataclass
 class Clone3Type:
     """Content of an clone3() call
-    >> parse(Clone3Type, '{flags=FOO, exit_signal=SIGCHLD, stack=0x123, stack_size=0x90}, 88')
+    >>> parse(Clone3Type, '{flags=FOO, exit_signal=SIGCHLD, stack=0x123, stack_size=0x90}, 88')
     clone3<flags=['FOO'], parent_tid_comment=None>
     >>> parse(Clone3Type,
     ...     '{flags=FOO|BAR, child_tid=0x123, parent_tid=0x345'
     ...     ', exit_signal=0, stack=0x234, stack_size=0x54, tls=0x2345}'
     ...     ' => {parent_tid=[1869 /* 1803473 in strace\\'s PID NS */]}, 88')
     clone3<flags=['FOO', 'BAR'], parent_tid_comment="1803473 in strace's PID NS">
     """
 
     flags: Sequence[str]
     parent_tid_comment: str
     PATTERN: ClassVar[str] = (
         rf"^\{{flags=({PFLAGS})(, child_tid={PHEX})?(, parent_tid={PHEX})?"
         rf"(, exit_signal={PCONST})?, stack={PHEX}, stack_size={PHEX}(, tls={PHEX})?\}}"
-        rf"( => \{{parent_tid=\[(\d*)( {PCOMMENT})?\]\}})?, \d*$"
+        rf"( => \{{parent_tid=\[(\d+)( {PCOMMENT})?\]\}})?, \d+$"
     )
 
     def __init__(self, args: tuple[str, ...]) -> None:
         self.flags = args[0].split("|")
         self.parent_tid_comment = args[9]
 
     def __repr__(self) -> str:
@@ -306,209 +345,330 @@
     def __init__(self, args: tuple[str, ...]) -> None:
         ...
 
 
 Parsable = TypeVar("Parsable", bound=ParsableBase)
 
 
-def parse(
-    result_type: Type[Parsable], line: str, raise_on_mismatch: bool = True
-) -> Parsable | None:
+def maybe_parse(result_type: Type[Parsable], src: str | StraceType) -> Parsable | None:
     """Returns an element of given class from parsed line
-    >>> parse(StraceType, '012345 1234567890.123456 abc(a, b, c) = 1')
+    >>> maybe_parse(StraceType, '012345 1234567890.123456 abc(a, b, c) = 1')
     strace<pid=12345, t=1234567890.123456, cmd=abc, res_nr=1, comment=None>
     """
-    if (match := re.match(result_type.PATTERN, line)) is None:
-        if raise_on_mismatch:
-            raise RuntimeError(
-                f"Could not parse a {result_type.__name__} from {line!r} with pattern"
-                f" {result_type.PATTERN}"
-            )
+    if not (match := re.match(result_type.PATTERN, src if isinstance(src, str) else src.args)):
         return None
     return result_type(match.groups())
 
 
-async def sanatized_strace_lines(filename: Path) -> AsyncIterable[tuple[str, StraceType]]:
+def parse(result_type: Type[Parsable], src: str | StraceType) -> Parsable:
+    """Wrapper for maybe_parse() which raises on non-matching input"""
+    if not (result := maybe_parse(result_type, src)):
+        raise RuntimeError(
+            f"Could not parse a {result_type.__name__}"
+            f" from {src if isinstance(src, str) else src.args!r} with pattern"
+            f" {result_type.PATTERN}"
+        )
+    return result
+
+
+async def sanatized_strace_lines(
+    in_stream: AsyncIterable[str],
+) -> AsyncIterable[tuple[int, str, StraceType]]:
     """Returns fully usable strace entries"""
     # pylint: disable=too-many-branches
 
     resume_state: MutableMapping[int, UnfinishedType] = {}
     pid_gen = {"clone", "clone3", "vfork"}
     line_stack_open: MutableSequence[tuple[str, StraceType]] = []
     line_stack: MutableSequence[tuple[str, StraceType]] = []
+    line_nr = 0
+    raw_line_nr = 0
 
     try:
-        async with aiofiles.open(filename) as afp:
-            # https://github.com/Tinche/aiofiles/issues/105
-            async for line in afp:  # type: ignore[attr-defined]
-                if strace := parse(StraceType, line, raise_on_mismatch=False):
-                    if "<unfinished ...>" in line:
-                        print(line)
-                        print(StraceType.PATTERN)
-                        raise SystemExit(1)
-                    assert " resumed>" not in line
-                    if strace.fname == "exited" and strace.pid in resume_state:
-                        del resume_state[strace.pid]
-
-                    if resume_state:
-                        (line_stack_open if strace.fname in pid_gen else line_stack).append(
-                            (line.rstrip(), strace)
-                        )
-                    else:
-                        yield line.rstrip(), strace
-                    continue
-
-                if unfinished := parse(UnfinishedType, line, raise_on_mismatch=False):
-                    assert unfinished.pid not in resume_state
-                    resume_state[unfinished.pid] = unfinished
-                    continue
-
-                if resumed := parse(ResumedType, line, raise_on_mismatch=False):
-                    if resumed.pid not in resume_state:
-                        raise RuntimeError(
-                            f"'resumed' without corresponding 'unfinished' found: {line}"
-                        )
-                    continued_line = resume_state[resumed.pid].line + resumed.line
-                    del resume_state[resumed.pid]
+        async for line in in_stream:
+            # we don't have enumerate() here
+            raw_line_nr += 1
+
+            if strace := maybe_parse(StraceType, line):
+                if "<unfinished ...>" in line or " resumed>" in line:
+                    print(line)
+                    print(StraceType.PATTERN)
+                    raise SystemExit(1)
+
+                if strace.fname == "exited" and strace.pid in resume_state:
+                    del resume_state[strace.pid]
+
+                if resume_state:
+                    (line_stack_open if strace.fname in pid_gen else line_stack).append(
+                        (line.rstrip(), strace)
+                    )
+                else:
+                    yield line_nr, line.rstrip(), strace
+                    line_nr += 1
 
-                    if not (continued_strace := parse(StraceType, continued_line)):
-                        raise RuntimeError()
+                continue
+
+            if unfinished := maybe_parse(UnfinishedType, line):
+                line_nr += 1
+                assert unfinished.pid not in resume_state
+                resume_state[unfinished.pid] = unfinished
+                # print("++++++UNFINISHED++++++", len(resume_state), raw_line_nr, line_nr)
+                continue
 
-                    (line_stack_open if continued_strace.fname in pid_gen else line_stack).append(
-                        (continued_line.rstrip(), continued_strace)
+            if resumed := maybe_parse(ResumedType, line):
+                if resumed.pid not in resume_state:
+                    raise RuntimeError(
+                        f"'resumed' without corresponding 'unfinished' found: {line}"
                     )
+                continued_line = resume_state[resumed.pid].line + resumed.line
+                del resume_state[resumed.pid]
+                # print("++++++RESUME++++++", len(resume_state), raw_line_nr, line_nr)
+
+                continued_strace = parse(StraceType, continued_line)
+
+                assert (
+                    "<unfinished ...>" not in continued_line or continued_strace.result_nr is None
+                )
+
+                (line_stack_open if continued_strace.fname in pid_gen else line_stack).append(
+                    (continued_line.rstrip(), continued_strace)
+                )
+
+                if not resume_state:
+                    for element in sorted(line_stack_open, key=lambda e: e[1].timestamp):
+                        yield line_nr, *element
+                        line_nr += 1
+                    line_stack_open.clear()
+                    for element in line_stack:
+                        yield line_nr, *element
+                        line_nr += 1
+                    line_stack.clear()
+                    assert line_nr == raw_line_nr
+                continue
+
+            line_nr += 1
+            if "+++ killed" in line:
+                # print(line)
+                continue
+            if "--- SIGCHLD " in line:
+                # print(line)
+                continue
+
+            if "--- SIGSEGV " in line:
+                continue
+
+            if "--- SIGTERM " in line:
+                # print(line)
+                continue
 
-                    if not resume_state:
-                        for element in line_stack_open:
-                            yield element
-                        line_stack_open.clear()
-                        for element in line_stack:
-                            yield element
-                        line_stack.clear()
-                    continue
+            if "--- SIGUSR2 " in line:
+                # print(line)
+                continue
 
-                if any(s in line for s in ("+++ killed ", " --- ")):
-                    continue
+            print(line)
 
-                # Should raise
-                parse(StraceType, line)
+            if any(s in line for s in ("+++ killed ", " --- ")):
+                # TODO: we want to track this, too
+                # line_nr += 1
+                continue
+
+            # Should raise
+            parse(StraceType, line)
 
     finally:
         assert not resume_state
 
 
-async def read_strace(filename: Path, args: Namespace) -> None:
-    """Reads strace log from a file (e.g. a named pipe) and handles all entries"""
-    # this will become a generator similar to sanatized_strace_lines but for PID tracking
-    # until then we accept 'too-many-branches' and 'too-many-statements'
-    # pylint: disable=too-many-branches
-    # pylint: disable=too-many-statements
+async def exctract_process_info(
+    sane_strace_stream: AsyncIterable[tuple[int, str, StraceType]],
+) -> AsyncIterable[tuple[int, str, StraceType]]:
+    """This generator function takes sanatized (i.e. ordered and stitched together) strace
+    lines and handles only the process relevant stuff, i.e. forking/cloning and execve instructions
+    """
+
+    # maps PIDs to their parents
+    pid_path: MutableMapping[int, tuple[int, Sequence[int]]] = {}
+
+    async for line_nr, line, strace in sane_strace_stream:
+
+        if strace.result_nr is None:
+            # sometimes we get an '?' instead of a result which always seems to be result
+            # of an unfinished fork due to process termination
+            # once we trace process termination we should assert the associated pid to be gone
+            if strace.fname not in {
+                "vfork",
+                "clone",
+                "clone3",
+                "futex",
+                "exit",
+                "exit_group",
+                "pselect6",
+                "epoll_wait",
+            }:
+                print(f"found a {strace.fname}() call not returning a valid value:")
+                print(line)
+            continue
+
+        if len(pid_path) == 0:
+            # this is the first call. make sure we register the PID even though we have no
+            # fork type yet
+            assert strace.fname == "execve"
+            pid_path[strace.pid] = 0, [strace.pid]
+
+        if strace.pid not in pid_path:
+            print(f">>> {line_nr}: {line}")
+            print(colored(f"{strace}", "yellow_bold"))
+            assert strace.pid in pid_path, f"{strace.pid} not in `pid_path`"
+
+        if strace.fname not in ALL_COMMANDS:
+            print(f"fname not yet considered: '{strace.fname}'")
+
+        if strace.fname not in IMPLEMENTED_COMMANDS:
+            # skip stuff we can't use anyway
+            continue
+
+        if strace.fname in {"vfork", "clone", "clone3"}:
+            new_pid = int(strace.comment.split()[0]) if strace.comment else strace.result_nr
+            if new_pid > 0:
+                assert new_pid not in pid_path, f"{line_nr}: {line} => {new_pid=}"
+                pid_path[new_pid] = len(pid_path), list(chain(pid_path[strace.pid][1], [new_pid]))
+
+        yield line_nr, line, strace, pid_path[strace.pid][1]
+
+
+def print_strace(line_nr: int, strace: StraceType) -> None:
+    """Write out a nice colored pre-formatted strace line"""
+    print(
+        colored(
+            f"{line_nr}" f"|{strace.pid}" f"|{strace.fname}  " f"|{strace.result_nr}"
+            # f"|{strace.command}"
+            "|",
+            {
+                "vfork": "blue_bold",
+                "clone": "blue_bold",
+                "clone3": "blue_bold",
+                "execve": "green_bold",
+            }[strace.fname],
+        )
+    )
+
+
+async def process_strace(
+    in_stream: AsyncIterable[tuple[int, str, StraceType]], args: Namespace
+) -> None:
+    """Crawls through pre-digested strace data and handles operations readily associated
+    to processes"""
 
-    # maps PIDs to a fork type - maybe we can get rid of this in the future in favor of `ptree`
-    pid_path: MutableMapping[str | int, Sequence[int]] = {}
     ptree: MutableMapping[str | int, Any] = {}
 
     try:
-        async for line, strace in sanatized_strace_lines(filename):
-            if strace.result_nr is None:
-                assert strace.fname in {"vfork", "clone", "clone3"}
-                continue
-
+        async for line_nr, line, strace, pid_path in in_stream:
             if args.grep and re.findall(args.grep, line):
                 print(line)
 
-            assert strace.fname in ALL_COMMANDS, f"{strace.fname}"
+            # print(line_nr, strace, pid_path)
 
-            if len(pid_path) == 0:
-                # this is the first call. make sure we register the PID even though we have no
-                # fork type yet
-                assert strace.fname == "execve"
-                pid_path[strace.pid] = [strace.pid]
+            if strace.fname in {"vfork", "clone", "clone3"}:
+                if args.verbose:
+                    print_strace(
+                        line_nr,
+                        parse(
+                            {
+                                "vfork": VforkType,
+                                "clone": CloneType,
+                                "clone3": Clone3Type,
+                            }[strace.fname],
+                            strace.args,
+                        ),
+                    )
                 insert(
                     ptree,
-                    path=[],
-                    name=strace.pid,
-                    # display_name=execve.fname[0],
+                    path=pid_path,
+                    name=strace.result_nr,
                     attrs={
-                        "tags": [],
+                        "tags": [strace.fname],
                     },
                 )
+            elif strace.fname == "exited":
+                # print(strace.result_nr)
+                get_node(ptree, pid_path).setdefault("__attrs__", {})["color"] = (
+                    "green" if strace.result_nr == 0 else "red"
+                )
 
-            if strace.pid not in pid_path:
-                print(">>>", line)
-                print(colored(f"{strace}", "yellow_bold"))
-                assert strace.pid in pid_path, f"{strace.pid} not in `pid_path`"
+            elif strace.fname == "execve":
+                assert strace.result_nr is not None
 
-            if strace.fname == "execve":
                 if strace.result_nr >= 0:
                     execve = parse(ExecveType, strace.args)
                     assert execve
                     if args.verbose:
-                        print(
-                            colored(
-                                f"{strace.pid}|execve |"
-                                # f"execve |{'.'.join(pid_path[strace.pid][0])}.{strace.pid}|"
-                                f"{strace.result}| {execve.command}",
-                                "green_bold",
-                            )
+                        print_strace(line_nr, strace)
+                    if line_nr == 0:
+                        insert(
+                            ptree,
+                            path=[],
+                            name=strace.pid,
+                            display_name=execve.command[0],
+                            attrs={
+                                "tags": [strace.fname],
+                            },
                         )
-                    get_node(ptree, pid_path[strace.pid]).setdefault("__attrs__", {}).setdefault(
-                        "tags", []
-                    ).append(execve.command[0])
-
-            elif strace.fname in {"vfork", "clone", "clone3"}:
-                new_pid = int(strace.comment.split()[0]) if strace.comment else strace.result_nr
-                assert new_pid not in pid_path
-                pid_path[new_pid] = list(chain(pid_path[strace.pid], [new_pid]))
-
-                if args.verbose:
-                    if strace.fname == "vfork":
-                        vfork = parse(VforkType, strace.args)
-                        assert vfork
-                        print(colored(f"{strace.pid}|vfork  |{strace.result_nr}|", "blue_bold"))
-
-                    elif strace.fname == "clone":
-                        clone = parse(CloneType, strace.args)
-                        assert clone
-                        print(colored(f"{strace.pid}|clone  |{strace.result_nr}|", "blue_bold"))
-
-                    elif strace.fname == "clone3":
-                        clone3 = parse(Clone3Type, strace.args)
-                        assert clone3
-                        print(colored(f"{strace.pid}|clone3 |{strace.result_nr}|", "blue_bold"))
 
-                insert(
-                    ptree,
-                    path=pid_path[strace.pid],
-                    name=new_pid,
-                    ## display_name=execve.command[0],
-                    attrs={
-                        "tags": [strace.fname],
-                    },
-                )
+                tags = get_node(ptree, pid_path).setdefault("__attrs__", {}).setdefault("tags", [])
+                cmd = (
+                    " ".join(execve.command)
+                    if isinstance(execve.command, (list, tuple))
+                    else str(execve.command)
+                )[:70].replace("\n", "\\n")
+                if cmd not in tags:
+                    tags.append(cmd)
 
             elif strace.fname == "openat":
                 openat = parse(OpenatType, strace.args)
                 assert openat
                 if not strace.result.startswith("-1"):
                     if (
                         args.verbose
                         and openat.path not in {".", "/proc/filesystems", "/dev/null"}
                         and ".so" not in openat.path
                         and not any(openat.path.endswith(s) for s in (".h", ".c", ".o", ".a", ".s"))
                     ):
                         print(
                             colored(
-                                f"{strace.pid}|openat |{strace.result}| {openat.path}", "blue_bold"
+                                f"{line_nr}|{strace.pid}|openat |{strace.result}| {openat.path}",
+                                "blue_bold",
                             )
                         )
+            elif strace.fname == "write":
+                if (write := parse(WriteType, strace.args)).filep in {1, 2}:
+                    string = write.string[:168].strip(" \n").replace("\n", "\\n")
+                    insert(
+                        ptree,
+                        path=pid_path,
+                        name=f"'{string}'",
+                        display_name="xxx",
+                        attrs={
+                            "color": "yellow" if write.filep == 2 else "blue",
+                        },
+                    )
     finally:
         print(attributed_tree(ptree))
 
 
+async def process_strace_file(filename: Path, args: Namespace) -> None:
+    """For testability: provides content of a file to process_strace()"""
+    async with aiofiles.open(filename) as afp:
+        await process_strace(
+            exctract_process_info(
+                sanatized_strace_lines(afp),
+            ),
+            args,
+        )
+
+
 async def buffer_stream(stream: StreamReader, out_file: TextIO) -> None:
     """Records a given stream to a buffer line by line along with the source"""
     while line := (await stream.readline()).decode():
         out_file.write(line)
 
 
 @contextmanager
@@ -526,15 +686,15 @@
 
 
 async def main_invoke(cmd: Sequence[str], args: Namespace) -> None:
     """Runs a program using strace"""
     with strace_output_path(args.record) as output_file_path:
         full_cmd = (
             "strace",
-            "--trace=fork,vfork,clone,clone3,execve,openat",
+            "--trace=fork,vfork,clone,clone3,execve,openat,write",
             "--decode-pids=pidns",
             "--timestamps=unix,us",
             "--follow-forks",
             "--columns=0",
             "--abbrev=none",
             "-s",
             "65536",
@@ -553,29 +713,29 @@
 
         await gather(
             *(
                 awaitable
                 for awaitable in (
                     buffer_stream(process.stdout, sys.stdout),
                     buffer_stream(process.stderr, sys.stderr),
-                    None if args.record else read_strace(output_file_path, args),
+                    None if args.record else process_strace_file(output_file_path, args),
                     process.wait(),
                 )
                 if awaitable
             )
         )
         raise SystemExit(process.returncode)
 
 
 def main() -> int:
     """Main entrypoint"""
     args, command = parse_args()
 
     if command[0].endswith(".log"):
-        run(read_strace(Path(command[0]), args))
+        run(process_strace_file(Path(command[0]), args))
     else:
         run(main_invoke(command, args))
     return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `ttrace-0.1.6/ttrace/utils/treestuff.py` & `ttrace-0.1.7/ttrace/utils/treestuff.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 __all__ = ["attributed_tree", "traverse", "insert", "colored"]
 
 
 def colored(text: str, color: str) -> str:
     """Returns @color formatted @text"""
     return (
         text
-        if color is None or not sys.stdout.isatty() or "COLORTERM" not in os.environ
+        if False  # color is None or not sys.stdout.isatty() or "COLORTERM" not in os.environ
         else {
             "none": "%s",
             "green": "\033[0;32m%s\033[0m",
             "green_bold": "\033[1;32m%s\033[0m",
             "red": "\033[0;31m%s\033[0m",
             "red_bold": "\033[1;31m%s\033[0m",
             "black": "\033[0;30m%s\033[0m",
@@ -120,14 +120,15 @@
 
 
 def insert(
     tree: MutableMapping[str | int, Any],
     path: Sequence[str | int],
     *,
     name: str | int | None = None,
+    display_name: str | None = None,
     data: Mapping[str, Any] | None = None,
     attrs: Mapping[str, Any] | None = None,
     insert_missing: bool = False,
 ) -> Mapping[str, Any]:
     """Inserts a new element with provided @data and @attrs at position @path
     into @tree"""
     iterator = tree
```

### Comparing `ttrace-0.1.6/PKG-INFO` & `ttrace-0.1.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttrace
-Version: 0.1.6
+Version: 0.1.7
 Summary: Makes use of strace
 Home-page: https://projects.om-office.de/frans/ttrace.git
 Author: Frans Fürst
 Author-email: frans.fuerst+gitlab@protonmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -17,25 +17,31 @@
 # ttrace - strace as a tree
 
 Uses `strace` to trace a program call and displays what's going on in a human
 friendly manner.
 
 [Project page](https://projects.om-office.de/frans/ttrace)
 
-## Usage
 
-Currently you just run
+## Installation and Usage
 
+Install `ttrace` via pip:
 ```
-ttrace.py <CMD>
+[<python executable> -m] pip install [-U] ttrace
 ```
-as you would with `strace` but without any arguments to `ttrace` (`strace` will
-be called with a bunch of arguments automatically).
 
-See next section to see what's coming.
+A new executable is then provided which can be used instead of `strace`:
+```
+ttrace [<ARGS>] <CMD>
+```
+Note that you would'nt provide `strace` arguments since `ttrace` provides them
+automatically.
+
+Alternatively you can clone and use the current development tree, see below.
+
 
 ## Intended interface
 
 The following commands and outputs reflect the current development plan:
 
 ```sh
 ttrace <CMD|LOGFILE>
@@ -79,43 +85,50 @@
 * strace console
 * console with only warning character (whatever that means)
 
 ```sh
 ttrace --timing <CMD>
 ```
 
+### ToDo for v1.0
+
+* trace process termination
+* output growing process tree
+* report / visualize abnormal process termination
+* report / visualize file access
+* optionally turn PIDs into PID counters for comparability
+* optionally print timestamp, pid, line number
+* no color
+* logging
+
 
 ### Other ideas
 
+* compare trace files on abstract level
 * trace changes environment
 * trace docker image usage
 * highlight failed processes
 
-## Installation
 
 ## Development & Contribution
 
 ```
 pip3 install -U poetry pre-commit
 git clone --recurse-submodules https://projects.om-office.de/frans/ttrace.git
 cd ttrace
 pre-commit install
 # if you need a specific version of Python inside your dev environment
-poetry env use /home/frafue/.pyenv/versions/3.10.4/bin/python3
+poetry env use ~/.pyenv/versions/3.10.4/bin/python3
 poetry install
 ```
 
-## License
 
-For all code contained in this repository the rules of GPLv3 apply unless
-otherwise noted. That means that you can do what you want with the source
-code as long as you make the files with their original copyright notice
-and all modifications available.
+## License
 
-See [GNU / GPLv3](https://www.gnu.org/licenses/gpl-3.0.en.html) for details.
+See `License.md`
 
 
 ## Read
 
 * [The Difference Between fork(), vfork(), exec() and clone()](https://www.baeldung.com/linux/fork-vfork-exec-clone)
 * [HN: The Magic of strace](https://news.ycombinator.com/item?id=7155799)
 * [The Magic of strace (archive.org)](https://web.archive.org/web/20160116001752/http://chadfowler.com/blog/2014/01/26/the-magic-of-strace/)
```

