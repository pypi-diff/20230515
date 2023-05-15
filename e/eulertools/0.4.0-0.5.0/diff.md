# Comparing `tmp/eulertools-0.4.0.tar.gz` & `tmp/eulertools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eulertools-0.4.0.tar", max compression
+gzip compressed data, was "eulertools-0.5.0.tar", max compression
```

## Comparing `eulertools-0.4.0.tar` & `eulertools-0.5.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.4.0/README.rst
--rw-r--r--   0        0        0     2694 2023-05-12 16:47:11.900398 eulertools-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.4.0/src/eulertools/__init__.py
--rw-r--r--   0        0        0       22 2023-05-12 16:47:05.636529 eulertools-0.4.0/src/eulertools/__version__.py
--rw-r--r--   0        0        0     1894 2023-05-12 14:14:39.715719 eulertools-0.4.0/src/eulertools/compare.py
--rw-r--r--   0        0        0     1219 2023-05-12 16:45:37.573777 eulertools-0.4.0/src/eulertools/generate.py
--rw-r--r--   0        0        0     3234 2023-05-12 16:45:37.571776 eulertools-0.4.0/src/eulertools/main.py
--rw-r--r--   0        0        0     2527 2023-05-12 16:45:58.269757 eulertools-0.4.0/src/eulertools/run.py
--rw-r--r--   0        0        0     1063 2023-05-12 15:13:14.054136 eulertools-0.4.0/src/eulertools/statement.py
--rw-r--r--   0        0        0     2654 2023-05-12 16:45:37.571618 eulertools-0.4.0/src/eulertools/time.py
--rw-r--r--   0        0        0     6013 2023-05-12 15:13:20.367496 eulertools-0.4.0/src/eulertools/utils.py
--rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-05-09 19:41:34.782813 eulertools-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0      976 2023-05-09 19:41:34.788663 eulertools-0.5.0/README.rst
+-rw-r--r--   0        0        0     2694 2023-05-15 10:13:58.333719 eulertools-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-09 19:41:34.789309 eulertools-0.5.0/src/eulertools/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-15 10:13:58.336742 eulertools-0.5.0/src/eulertools/__version__.py
+-rw-r--r--   0        0        0     2879 2023-05-15 10:13:22.829230 eulertools-0.5.0/src/eulertools/compare.py
+-rw-r--r--   0        0        0     1007 2023-05-15 10:13:22.829663 eulertools-0.5.0/src/eulertools/generate.py
+-rw-r--r--   0        0        0     3234 2023-05-12 18:56:00.902083 eulertools-0.5.0/src/eulertools/main.py
+-rw-r--r--   0        0        0     3067 2023-05-15 10:13:22.830141 eulertools-0.5.0/src/eulertools/run.py
+-rw-r--r--   0        0        0      627 2023-05-15 10:13:22.830519 eulertools-0.5.0/src/eulertools/statement.py
+-rw-r--r--   0        0        0     2586 2023-05-15 10:13:22.830923 eulertools-0.5.0/src/eulertools/time.py
+-rw-r--r--   0        0        0     6485 2023-05-15 10:13:22.831296 eulertools-0.5.0/src/eulertools/utils.py
+-rw-r--r--   0        0        0     1817 1970-01-01 00:00:00.000000 eulertools-0.5.0/PKG-INFO
```

### Comparing `eulertools-0.4.0/LICENSE.txt` & `eulertools-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `eulertools-0.4.0/README.rst` & `eulertools-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `eulertools-0.4.0/pyproject.toml` & `eulertools-0.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 [tool.coverage.report]
 show_missing = true
 skip_covered = true
 skip_empty = true
 
 [tool.poetry]
 name = "eulertools"
-version = "0.4.0"
+version = "0.5.0"
 description = "Multilanguage competitive coding toolbox"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
```

### Comparing `eulertools-0.4.0/src/eulertools/compare.py` & `eulertools-0.5.0/src/eulertools/compare.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-from eulertools.utils import Language, get_timings
+from itertools import chain
+
+from eulertools.utils import Language, get_all_keyed_problems, get_timings
 
 
 class Compare:
     def __init__(self, languages: list[Language], problems: list[str]):
         self.languages = languages
-        self.problems = problems
-        self.pad_length = max(max(len(language.name) for language in languages), 9)
+        self.timings = {language: get_timings(language) for language in languages}
+        self.keyed_problems = self.get_keyed_problems(languages, problems)
+        self.pad_length = self._pad_length()
 
     def run(self) -> None:
         matrix = [
-            ["problem", *self.problems],
+            ["problem", *(f"{problem}/{key}" for problem, key in self.keyed_problems)],
             *(self.get_language_timings(language) for language in self.languages),
         ]
         self.print_table(self.transpose(matrix))
 
     def print_table(self, matrix: list[list[str]]) -> None:
         if len(matrix) == 1:
             raise ValueError("No data to print")
@@ -34,19 +37,44 @@
             )
         print(btm)
 
     def get_language_timings(self, language: Language) -> list[str]:
         timings = get_timings(language)
         return [
             language.name,
-            *(str(timings.get(problem, "N/A")) for problem in self.problems),
+            *(
+                str(timings.get(problem, {}).get(key, "N/A"))
+                for problem, key in self.keyed_problems
+            ),
         ]
 
     @staticmethod
     def transpose(matrix: list[list[str]]) -> list[list[str]]:
         new_lines = (list(row) for row in zip(*matrix, strict=True))
         return [line for line in new_lines if any(item != "N/A" for item in line[1:])]
 
     def padded_print(self, string: str, *, heading: bool) -> str:
         if heading:
             return string.center(self.pad_length)
         return string.rjust(self.pad_length)
+
+    def get_keyed_problems(
+        self, languages: list[Language], problems: list[str]
+    ) -> list[tuple[str, int]]:
+        return [
+            (problem, key)
+            for problem, key in get_all_keyed_problems()
+            if any(
+                problem_key
+                for language in languages
+                for problem_key in self.timings[language].get(problem, {})
+            )
+            and problem in problems
+        ]
+
+    def _pad_length(self) -> int:
+        lengths = chain(
+            (len(problem) + len(str(key)) for problem, key in self.keyed_problems),
+            (len(language.name) for language in self.languages),
+            [len("problem")],
+        )
+        return max(lengths) + 2
```

### Comparing `eulertools-0.4.0/src/eulertools/generate.py` & `eulertools-0.5.0/src/eulertools/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,21 @@
 from pathlib import Path
 
 import jinja2
 
-from eulertools.utils import (
-    Language,
-    get_context,
-    get_solution,
-    get_statement,
-    get_template,
-)
+from eulertools.utils import Language, get_context, get_solution, get_template
 
 
 class Generate:
     def __init__(self, languages: list[Language], problems: list[str]):
         self.languages = languages
         self.problems = problems
 
     def run(self) -> None:
         for problem in self.problems:
-            statement = get_statement(problem)
-            if not statement.exists():
-                raise FileNotFoundError("No problem description found. Aborting...")
-
             for language in self.languages:
                 self.generate_solution(language, problem)
 
     def generate_solution(self, language: Language, problem: str) -> None:
         template = get_template(language)
         solution = get_solution(language, problem)
         if get_solution(language, problem).exists():
```

### Comparing `eulertools-0.4.0/src/eulertools/main.py` & `eulertools-0.5.0/src/eulertools/main.py`

 * *Files identical despite different names*

### Comparing `eulertools-0.4.0/src/eulertools/run.py` & `eulertools-0.5.0/src/eulertools/run.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,47 +16,56 @@
     ):
         self.languages = languages
         self.problems = problems
         self.mode = mode
         self.times = times
         self.verbosity = verbosity
 
-    def run(self) -> None:
+    def run(self) -> dict[Language, dict[str, dict[int, list[int]]]]:
+        output: dict[Language, dict[str, dict[int, list[int]]]] = {}
         for language, problem in product(self.languages, self.problems):
-            self.run_single_problem(language, problem)
+            timings = self.run_single_problem(language, problem)
+            if timings is not None:
+                output.setdefault(language, {})[problem] = timings
+        return output
 
-    def run_single_problem(self, language: Language, problem: str) -> list[int] | None:
+    def run_single_problem(
+        self, language: Language, problem: str
+    ) -> dict[int, list[int]] | None:
         solution = get_solution(language, problem)
         if not solution.exists():
             return None
         raw_output = subprocess.run(
-            [language.runner, problem, self.mode, str(self.times)],  # noqa: S603
+            [language.runner, problem, str(self.times)],  # noqa: S603
             capture_output=True,
         )
         output = raw_output.stdout.decode()
         if self.verbosity > 3:
             print(output)
-        timings = [
-            int(line[6:]) or 1
-            for line in output.splitlines()
-            if line.startswith("Time: ")
-        ]
+        actual_answers: dict[int, set[str]] = {}
+        timings: dict[int, list[int]] = {}
+        for line in output.splitlines():
+            output_type, run_id, value = line.split(maxsplit=2)
+            key = int(run_id)
+            if output_type == "Time":
+                timings.setdefault(key, []).append(int(value) or 1)
+            elif output_type == "Answer":
+                actual_answers.setdefault(key, set()).add(value)
         expected_answers = get_answers(problem)
-        actual_answers: dict[int, str] = {}
-        for line in output.strip().splitlines():
-            if line.startswith("Time: "):
-                continue
-            raw_key, value = line.split(maxsplit=1)
-            key = int(raw_key[:-1])
-            actual_answers[key] = value
         success = True
         if self.mode != Modes.TIMING and len(actual_answers) != len(expected_answers):
             success = False
-            print(f"🔴 Running {problem}...")
-        for key, value in actual_answers.items():
+            print(f"🔴 Running {problem}... Not the expected number of answers.")
+        for key, values in actual_answers.items():
+            if len(values) != 1:
+                success = False
+                print(
+                    f"🔴 Running {language.name}/{problem}/{key}... Not deterministic answer."
+                )
+            value = values.pop()
             if key not in expected_answers:
                 if self.mode != Modes.TIMING:
                     print(
                         f"🟠 Running {language.name}/{problem}/{key}... new response: {value}"
                     )
             elif value != expected_answers[key]:
                 success = False
```

### Comparing `eulertools-0.4.0/src/eulertools/utils.py` & `eulertools-0.5.0/src/eulertools/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -28,163 +28,188 @@
     RUN = "run"
 
 
 @dataclass(frozen=True, slots=True)
 class Timing:
     time: Decimal
     unit: str
+    nanoseconds: int = field(repr=False, compare=False)
 
     @classmethod
-    def from_string(cls, timing: str, old_timing: Timing | None = None) -> Self:
-        match = re.match(TIME_UNIT, timing)
-        if match is None:
-            raise ValueError(f"Invalid timing: {timing}")
-        time, unit = match.groups()
-        if not unit:
-            if old_timing is None:
-                raise ValueError("Missing unit in initial timing")
-            unit = old_timing.unit
-        if unit == "us":
-            unit = "µs"
-        return cls(time=Decimal(time), unit=unit)
-
-    @classmethod
-    def from_nanoseconds(cls, nanoseconds: float) -> Self:
+    def from_nanoseconds(cls, nanoseconds: int) -> Self:
         if nanoseconds < 1000:
-            return cls.from_string(f"{nanoseconds:.0f}ns")
+            return cls(time=Decimal(nanoseconds), unit="ns", nanoseconds=nanoseconds)
         microseconds = nanoseconds / 1000
         if microseconds < 1000:
-            return cls.from_string(f"{microseconds:.1f}µs")
+            return cls(
+                time=Decimal(f"{microseconds:.1f}"), unit="µs", nanoseconds=nanoseconds
+            )
         milliseconds = microseconds / 1000
         if milliseconds < 1000:
-            return cls.from_string(f"{milliseconds:.1f}ms")
+            return cls(
+                time=Decimal(f"{milliseconds:.1f}"), unit="ms", nanoseconds=nanoseconds
+            )
         seconds = milliseconds / 1000
-        return cls.from_string(f"{seconds:.2f}s")
-
-    def to_nanoseconds(self) -> int:
-        if self.unit == "ns":
-            return int(self.time)
-        if self.unit == "µs":
-            return int(self.time * 1000)
-        if self.unit == "ms":
-            return int(self.time * 1000 * 1000)
-        return int(self.time * 1000 * 1000 * 1000)
+        return cls(time=Decimal(f"{seconds:.2f}"), unit="s", nanoseconds=nanoseconds)
 
     def __str__(self) -> str:
-        return f"{self.time} {self.unit}"
+        return f"{self.time}{self.unit}"
 
 
 @dataclass(frozen=True, slots=True, order=True)
 class Language:
     name: str
     extension: str
     runner: Path = field(repr=False, compare=False)
 
     @classmethod
     def from_settings(cls, name: str) -> Self:
-        project_root = get_project_root()
+        project_root = _get_project_root()
         settings = get_settings()
         language = settings["languages"][name]
         return cls(
             name=language["name"],
             extension=language["extension"],
             runner=project_root.joinpath(language["runner"]),
         )
 
 
-def get_project_root() -> Path:
+def _get_project_root() -> Path:
     cwd = Path.cwd().resolve()
     while not cwd.joinpath("leet.toml").exists():
         if cwd.as_posix() == "/":
             raise RuntimeError("Could not find project root")
         cwd = cwd.parent
     return cwd
 
 
-def get_settings() -> dict[str, Any]:
-    return SettingsParser(get_project_root().joinpath("leet.toml")).data
+def _get_settings() -> Path:
+    return _get_project_root().joinpath("leet.toml")
 
 
-def get_answers(problem: str) -> dict[int, str]:
-    answers = get_project_root().joinpath("common", "answers.txt")
-    output: dict[int, str] = {}
-    for line in answers.read_text().splitlines():
-        if line.startswith(problem):
-            problem_part, mode_id, answer = line.split(maxsplit=2)
-            output[int(mode_id[:-1])] = answer
-    return output
+def _get_answers() -> Path:
+    return _get_project_root().joinpath("common", "answers.txt")
 
 
-def get_timings(language: Language) -> dict[str, Timing]:
-    timings = get_project_root().joinpath(language.name, "timings.txt")
-    output: dict[str, Timing] = {}
-    for line in timings.read_text().splitlines():
-        problem, timing = line.split(maxsplit=1)
-        output[problem] = Timing.from_string(timing)
-    return output
+def _get_timings(language: Language) -> Path:
+    return _get_project_root().joinpath(language.name, ".leet", "timings.txt")
 
 
-def update_timings(language: Language, timings: dict[str, Timing]) -> None:
-    timings_path = get_project_root().joinpath(language.name, "timings.txt")
-    with timings_path.open("w") as file:
-        for key in sorted(timings):
-            timing = timings[key]
-            file.write(" ".join([key, str(timing.time), timing.unit]) + "\n")
+def _get_statements_dir() -> Path:
+    return _get_project_root().joinpath("common", "statements")
 
 
-def get_average(values: list[int]) -> float:
-    if len(values) >= 3:
-        values = sorted(values)[1:-1]
-    return sum(values) // len(values)
-
-
-def get_statement(problem: str) -> Path:
-    return get_project_root().joinpath("common", "statements", f"{problem}.txt")
-
+def _get_statement(problem: str) -> Path:
+    statement = _get_statements_dir().joinpath(f"{problem}.txt")
+    if not statement.exists():
+        raise FileNotFoundError("No problem description found. Aborting...")
 
-def get_signature(language: Language, problem: str) -> str:
-    statement = get_project_root().joinpath("common", "statements", f"{problem}.txt")
-    with statement.open() as file:
-        for line in file.readlines():
-            if line.startswith(f"::{language.name}::"):
-                return line.split("::")[2].strip()
-
-    return ""
+    return statement
 
 
 def get_template(language: Language) -> Path:
-    return get_project_root().joinpath(language.name, ".leet", "template")
+    return _get_project_root().joinpath(language.name, ".leet", "solution.jinja")
 
 
 def get_solution(language: Language, problem: str) -> Path:
-    return get_project_root().joinpath(
+    return _get_project_root().joinpath(
         language.name, "src", "solutions", f"{problem}.{language.extension}"
     )
 
 
+def get_statement(problem: str) -> dict[str, list[str]]:
+    output: dict[str, list[str]] = {
+        "title": [],
+        "description": [],
+    }
+    title = True
+    for line in _get_statement(problem).read_text().splitlines():
+        if line.startswith("::"):
+            _, language, path = line.split("::")
+            output[language.strip()] = [path.strip()]
+        elif title:
+            output["title"] = [line.strip()]
+            title = False
+        else:
+            output["description"].append(line.strip())
+
+    return output
+
+
+def get_settings() -> dict[str, Any]:
+    return SettingsParser(_get_settings()).data
+
+
+def get_answers(problem: str) -> dict[int, str]:
+    answers = _get_answers()
+    output: dict[int, str] = {}
+    for line in answers.read_text().splitlines():
+        if line.startswith(problem):
+            problem_part, mode_id, answer = line.split(maxsplit=2)
+            output[int(mode_id)] = answer
+    return output
+
+
+def get_timings(language: Language) -> dict[str, dict[int, Timing]]:
+    timings = _get_timings(language)
+    output: dict[str, dict[int, Timing]] = {}
+    for line in timings.read_text().splitlines():
+        problem, key, timing = line.split()
+        output.setdefault(problem, {})[int(key)] = Timing.from_nanoseconds(int(timing))
+    return output
+
+
 def get_context(language: Language, problem: str) -> dict[str, str]:
-    signature = get_signature(language, problem)
-    regex_list = get_settings()["languages"][language.name].get("regex", [])
-    context = {"problem": problem}
-    for regex in regex_list:
-        if regex_match := re.search(regex, signature):
-            context |= regex_match.groupdict()
+    statement = get_statement(problem)
+    parser = get_settings()["languages"][language.name].get("parser", {})
+    context = {"problem": problem, "title": statement["title"][0]}
+
+    try:
+        signature = statement[language.name][0]
+    except KeyError:
+        return context
+
+    for name, regex in parser.items():
+        if regex_match := re.findall(regex["regex"], signature):
+            context |= {name: regex.get("join", "").join(regex_match)}
     return context
 
 
+def update_timings(language: Language, timings: dict[str, dict[int, Timing]]) -> None:
+    timings_path = _get_timings(language)
+    with timings_path.open("w") as file:
+        for problem in sorted(timings):
+            for key in sorted(timings[problem]):
+                timing = timings[problem][key]
+                file.write(f"{problem} {key} {timing.nanoseconds}\n")
+
+
+def get_average(values: list[int]) -> int:
+    if len(values) >= 3:
+        values = sorted(values)[1:-1]
+    return sum(values) // len(values)
+
+
 def get_all_languages() -> list[str]:
     languages = get_settings()["languages"]
     return sorted(languages)
 
 
 def get_all_problems() -> list[str]:
-    statement_dir = get_project_root().joinpath("common", "statements")
+    statement_dir = _get_statements_dir()
     return sorted(file.stem for file in statement_dir.glob("*.txt"))
 
 
+def get_all_keyed_problems() -> list[tuple[str, int]]:
+    output = [
+        (problem, key) for problem in get_all_problems() for key in get_answers(problem)
+    ]
+    return sorted(output)
+
+
 def filter_languages(parsed_languages: list[str]) -> list[Language]:
     language_strings = get_all_languages()
     return [
         Language.from_settings(language)
         for language in language_strings
         if language in parsed_languages
     ]
```

### Comparing `eulertools-0.4.0/PKG-INFO` & `eulertools-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eulertools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Multilanguage competitive coding toolbox
 Home-page: https://eulertools.readthedocs.io/en/latest/
 License: LGPL-3.0+
 Keywords: leetcode,topcoder,project_euler
 Author: Stephanos Kuma
 Author-email: stephanos@kuma.ai
 Requires-Python: >=3.11,<4.0
```

