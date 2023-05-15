# Comparing `tmp/docformatter-1.6.5.tar.gz` & `tmp/docformatter-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docformatter-1.6.5.tar", max compression
+gzip compressed data, was "docformatter-1.7.0.tar", max compression
```

## Comparing `docformatter-1.6.5.tar` & `docformatter-1.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.6.5/LICENSE
--rw-r--r--   0        0        0     6593 2023-05-03 00:53:18.139711 docformatter-1.6.5/README.rst
--rw-r--r--   0        0        0     5851 2023-05-03 17:53:43.941376 docformatter-1.6.5/pyproject.toml
--rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.6.5/src/docformatter/__init__.py
--rwxr-xr-x   0        0        0     6095 2023-05-03 00:52:57.971387 docformatter-1.6.5/src/docformatter/__main__.py
--rw-r--r--   0        0        0     1191 2023-05-03 17:53:43.942376 docformatter-1.6.5/src/docformatter/__pkginfo__.py
--rw-r--r--   0        0        0    12789 2023-05-03 00:52:57.971387 docformatter-1.6.5/src/docformatter/configuration.py
--rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.6.5/src/docformatter/encode.py
--rw-r--r--   0        0        0    20851 2023-05-03 17:45:12.943363 docformatter-1.6.5/src/docformatter/format.py
--rw-r--r--   0        0        0     6611 2023-05-02 23:18:37.457940 docformatter-1.6.5/src/docformatter/strings.py
--rw-r--r--   0        0        0    15048 2023-05-03 17:40:52.745753 docformatter-1.6.5/src/docformatter/syntax.py
--rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.6.5/src/docformatter/util.py
--rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 docformatter-1.6.5/setup.py
--rw-r--r--   0        0        0     8254 1970-01-01 00:00:00.000000 docformatter-1.6.5/PKG-INFO
+-rw-r--r--   0        0        0     1061 2022-07-29 13:50:28.414095 docformatter-1.7.0/LICENSE
+-rw-r--r--   0        0        0     6593 2023-05-03 00:53:18.139711 docformatter-1.7.0/README.rst
+-rw-r--r--   0        0        0     6026 2023-05-15 00:27:42.297884 docformatter-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1539 2023-04-12 22:55:21.288454 docformatter-1.7.0/src/docformatter/__init__.py
+-rwxr-xr-x   0        0        0     6095 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/__main__.py
+-rw-r--r--   0        0        0     1191 2023-05-15 00:27:42.297884 docformatter-1.7.0/src/docformatter/__pkginfo__.py
+-rw-r--r--   0        0        0    12789 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/configuration.py
+-rw-r--r--   0        0        0     3654 2023-04-12 22:55:21.317454 docformatter-1.7.0/src/docformatter/encode.py
+-rw-r--r--   0        0        0    20851 2023-05-05 16:25:39.896748 docformatter-1.7.0/src/docformatter/format.py
+-rw-r--r--   0        0        0     6611 2023-05-02 23:18:37.457940 docformatter-1.7.0/src/docformatter/strings.py
+-rw-r--r--   0        0        0    15288 2023-05-15 00:27:42.298884 docformatter-1.7.0/src/docformatter/syntax.py
+-rw-r--r--   0        0        0     4573 2023-04-28 16:27:48.980570 docformatter-1.7.0/src/docformatter/util.py
+-rw-r--r--   0        0        0     7811 1970-01-01 00:00:00.000000 docformatter-1.7.0/setup.py
+-rw-r--r--   0        0        0     8254 1970-01-01 00:00:00.000000 docformatter-1.7.0/PKG-INFO
```

### Comparing `docformatter-1.6.5/LICENSE` & `docformatter-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/README.rst` & `docformatter-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/pyproject.toml` & `docformatter-1.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "docformatter"
-version = "1.6.5"
+version = "1.7.0"
 description = "Formats docstrings to follow PEP 257"
 authors = ["Steven Myint"]
 maintainers = [
     "Doyle Rowland <doyle.rowland@reliaqual.com>",
 ]
 license = "Expat"
 readme = "README.rst"
@@ -245,13 +245,13 @@
     pylint
     rstcheck
     toml
     untokenize
 commands =
     pip install -U pip
     pip install .
-    docformatter --recursive {toxinidir}/src/docformatter
-    pycodestyle --ignore=E203,W503,W504 {toxinidir}/src/docformatter
+    docformatter --black --recursive {toxinidir}/src/docformatter
+    pycodestyle --exclude=.git,.tox,*.pyc,*.pyo,build,dist,*.egg-info,config,docs,locale,tests,tools --ignore=C326,C330,E121,E123,E126,E133,E203,E242,E265,E402,W503,W504 --format=pylint --max-line-length=88 {toxinidir}/src/docformatter
     pydocstyle {toxinidir}/src/docformatter
     pylint --rcfile={toxinidir}/pyproject.toml {toxinidir}/src/docformatter
     rstcheck --report-level=1 {toxinidir}/README.rst
 """
```

### Comparing `docformatter-1.6.5/src/docformatter/__init__.py` & `docformatter-1.7.0/src/docformatter/__init__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/__main__.py` & `docformatter-1.7.0/src/docformatter/__main__.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/__pkginfo__.py` & `docformatter-1.7.0/src/docformatter/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,8 @@
 # NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS
 # BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN
 # ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
 # CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Package information for docformatter."""
 
-__version__ = "1.6.5"
+__version__ = "1.7.0"
```

### Comparing `docformatter-1.6.5/src/docformatter/configuration.py` & `docformatter-1.7.0/src/docformatter/configuration.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/encode.py` & `docformatter-1.7.0/src/docformatter/encode.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/format.py` & `docformatter-1.7.0/src/docformatter/format.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/strings.py` & `docformatter-1.7.0/src/docformatter/strings.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/src/docformatter/syntax.py` & `docformatter-1.7.0/src/docformatter/syntax.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,20 +347,26 @@
                 f"{do_clean_url(text[_idx[0] : _idx[1]], indentation)}"
             )
 
             _text_idx = _idx[1]
 
     # Finally, add everything after the last URL.
     with contextlib.suppress(IndexError):
-        _stripped_text = (
-            text[_text_idx + 1 :].strip(indentation)
+        _text = (
+            text[_text_idx + 1 :]
             if text[_text_idx] == "\n"
-            else text[_text_idx:].strip()
+            else text[_text_idx:]
         )
-        _lines.append(f"{indentation}{_stripped_text}")
+        _text = _text.splitlines()
+        for _idx, _line in enumerate(_text):
+            if _line not in ["", "\n", f"{indentation}"]:
+                _text[_idx] = f"{indentation}{_line.strip()}"
+
+        _lines += _text
+
     return _lines
 
 
 # pylint: disable=line-too-long
 def is_some_sort_of_list(text: str, strict: bool) -> bool:
     """Determine if docstring is a reST list.
 
@@ -406,14 +412,17 @@
             re.match(r"\s*\S+[\-*:=@]\s+", line)
             or
             # "parameter:\n    description"
             re.match(r"\s*\S+:\s*$", line)
             or
             # "parameter -- description"
             re.match(r"\s*\S+\s+--\s+", line)
+            or
+            # "parameter::" <-- Literal block
+            re.match(r"\s*[\S ]*:{2}", line)
         )
         for line in split_lines
     )
 
 
 def is_some_sort_of_code(text: str) -> bool:
     """Return True if text looks like code."""
@@ -491,16 +500,16 @@
     else:
         return summary
 
 
 def wrap_description(text, indentation, wrap_length, force_wrap, strict):
     """Return line-wrapped description text.
 
-    We only wrap simple descriptions. We leave doctests, multi-paragraph
-    text, and bulleted lists alone.
+    We only wrap simple descriptions. We leave doctests, multi-paragraph text, and
+    bulleted lists alone.
     """
     text = strip_leading_blank_lines(text)
 
     # Do not modify doctests at all.
     if ">>>" in text:
         return text
```

### Comparing `docformatter-1.6.5/src/docformatter/util.py` & `docformatter-1.7.0/src/docformatter/util.py`

 * *Files identical despite different names*

### Comparing `docformatter-1.6.5/setup.py` & `docformatter-1.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 {'tomli': ['tomli>=2.0.0,<3.0.0']}
 
 entry_points = \
 {'console_scripts': ['docformatter = docformatter.__main__:main']}
 
 setup_kwargs = {
     'name': 'docformatter',
-    'version': '1.6.5',
+    'version': '1.7.0',
     'description': 'Formats docstrings to follow PEP 257',
     'long_description': '============\ndocformatter\n============\n\n.. |CI| image:: https://img.shields.io/github/actions/workflow/status/PyCQA/docformatter/ci.yml?branch=master\n    :target: https://github.com/PyCQA/docformatter/actions/workflows/ci.yml\n.. |COVERALLS| image:: https://img.shields.io/coveralls/github/PyCQA/docformatter\n    :target: https://coveralls.io/github/PyCQA/docformatter\n.. |CONTRIBUTORS| image:: https://img.shields.io/github/contributors/PyCQA/docformatter\n    :target: https://github.com/PyCQA/docformatter/graphs/contributors\n.. |COMMIT| image:: https://img.shields.io/github/last-commit/PyCQA/docformatter\n.. |BLACK| image:: https://img.shields.io/badge/%20style-black-000000.svg\n    :target: https://github.com/psf/black\n.. |ISORT| image:: https://img.shields.io/badge/%20imports-isort-%231674b1\n    :target: https://pycqa.github.io/isort/\n.. |SELF| image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n    :target: https://github.com/PyCQA/docformatter\n.. |SPHINXSTYLE| image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n    :target: https://www.sphinx-doc.org/en/master/usage/index.html\n.. |NUMPSTYLE| image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n    :target: https://numpydoc.readthedocs.io/en/latest/format.html\n.. |GOOGSTYLE| image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n    :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\n.. |VERSION| image:: https://img.shields.io/pypi/v/docformatter\n.. |LICENSE| image:: https://img.shields.io/pypi/l/docformatter\n.. |PYVERS| image:: https://img.shields.io/pypi/pyversions/docformatter\n.. |PYMAT| image:: https://img.shields.io/pypi/format/docformatter\n.. |DD| image:: https://img.shields.io/pypi/dd/docformatter\n.. |PRE| image:: https://img.shields.io/github/v/release/PyCQA/docformatter?include_prereleases\n\n+----------------+----------------------------------------------------------+\n| **Code**       + |BLACK| |ISORT|                                          +\n+----------------+----------------------------------------------------------+\n| **Docstrings** + |SELF| |NUMPSTYLE|                                       +\n+----------------+----------------------------------------------------------+\n| **GitHub**     + |CI| |CONTRIBUTORS| |COMMIT| |PRE|                       +\n+----------------+----------------------------------------------------------+\n| **PyPi**       + |VERSION| |LICENSE| |PYVERS| |PYMAT| |DD|                +\n+----------------+----------------------------------------------------------+\n\nFormats docstrings to follow `PEP 257`_.\n\n.. _`PEP 257`: http://www.python.org/dev/peps/pep-0257/\n\nFeatures\n========\n\n``docformatter`` automatically formats docstrings to follow a subset of the PEP\n257 conventions. Below are the relevant items quoted from PEP 257.\n\n- For consistency, always use triple double quotes around docstrings.\n- Triple quotes are used even though the string fits on one line.\n- Multi-line docstrings consist of a summary line just like a one-line\n  docstring, followed by a blank line, followed by a more elaborate\n  description.\n- Unless the entire docstring fits on a line, place the closing quotes\n  on a line by themselves.\n\n``docformatter`` also handles some of the PEP 8 conventions.\n\n- Don\'t write string literals that rely on significant trailing\n  whitespace. Such trailing whitespace is visually indistinguishable\n  and some editors (or more recently, reindent.py) will trim them.\n\nSee the the full documentation at `read-the-docs`_, especially the\n`requirements`_ section for a more detailed discussion of PEP 257 and other\nrequirements.\n\n.. _read-the-docs: https://docformatter.readthedocs.io\n.. _requirements: https://docformatter.readthedocs.io/en/latest/requirements.html\n\nInstallation\n============\n\nFrom pip::\n\n    $ pip install --upgrade docformatter\n\nOr, if you want to use pyproject.toml to configure docformatter::\n\n    $ pip install --upgrade docformatter[tomli]\n\nOr, if you want to use a release candidate (or any other tag)::\n\n    $ pip install git+https://github.com/PyCQA/docformatter.git@<RC_TAG>\n\nWhere <RC_TAG> is the release candidate tag you\'d like to install.  Release\ncandidate tags will have the format v1.6.0-rc1  Release candidates will also be\nmade available as a Github Release.\n\nExample\n=======\n\nAfter running::\n\n    $ docformatter --in-place example.py\n\nthis code\n\n.. code-block:: python\n\n    """   Here are some examples.\n\n        This module docstring should be dedented."""\n\n\n    def launch_rocket():\n        """Launch\n    the\n    rocket. Go colonize space."""\n\n\n    def factorial(x):\n        \'\'\'\n\n        Return x factorial.\n\n        This uses math.factorial.\n\n        \'\'\'\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial"""\n        print(factorial(x))\n\n\n    def main():\n        """Main\n        function"""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\n\ngets formatted into this\n\n.. code-block:: python\n\n    """Here are some examples.\n\n    This module docstring should be dedented.\n    """\n\n\n    def launch_rocket():\n        """Launch the rocket.\n\n        Go colonize space.\n        """\n\n\n    def factorial(x):\n        """Return x factorial.\n\n        This uses math.factorial.\n        """\n        import math\n        return math.factorial(x)\n\n\n    def print_factorial(x):\n        """Print x factorial."""\n        print(factorial(x))\n\n\n    def main():\n        """Main function."""\n        print_factorial(5)\n        if factorial(10):\n            launch_rocket()\n\nMarketing\n=========\nDo you use *docformatter*?  What style docstrings do you use?  Add some badges to your project\'s **README** and let everyone know.\n\n|SELF|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20formatter-docformatter-fedcba.svg\n        :target: https://github.com/PyCQA/docformatter\n\n|SPHINXSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-sphinx-0a507a.svg\n        :target: https://www.sphinx-doc.org/en/master/usage/index.html\n\n|NUMPSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-numpy-459db9.svg\n        :target: https://numpydoc.readthedocs.io/en/latest/format.html\n\n|GOOGSTYLE|\n\n.. code-block::\n\n    .. image:: https://img.shields.io/badge/%20style-google-3666d6.svg\n        :target: https://google.github.io/styleguide/pyguide.html#s3.8-comments-and-docstrings\n\nIssues\n======\n\nBugs and patches can be reported on the `GitHub page`_.\n\n.. _`GitHub page`: https://github.com/PyCQA/docformatter/issues\n',
     'author': 'Steven Myint',
     'author_email': 'None',
     'maintainer': 'Doyle Rowland',
     'maintainer_email': 'doyle.rowland@reliaqual.com',
     'url': 'https://github.com/PyCQA/docformatter',
```

### Comparing `docformatter-1.6.5/PKG-INFO` & `docformatter-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docformatter
-Version: 1.6.5
+Version: 1.7.0
 Summary: Formats docstrings to follow PEP 257
 Home-page: https://github.com/PyCQA/docformatter
 License: Expat
 Keywords: PEP 257,pep257,style,formatter,docstrings
 Author: Steven Myint
 Maintainer: Doyle Rowland
 Maintainer-email: doyle.rowland@reliaqual.com
```

