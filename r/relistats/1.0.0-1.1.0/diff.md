# Comparing `tmp/relistats-1.0.0.tar.gz` & `tmp/relistats-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relistats-1.0.0.tar", last modified: Sat Apr  8 21:14:07 2023, max compression
+gzip compressed data, was "relistats-1.1.0.tar", last modified: Sun May 14 23:01:10 2023, max compression
```

## Comparing `relistats-1.0.0.tar` & `relistats-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 sanjay     (503) staff       (20)        0 2023-04-08 21:14:07.246864 relistats-1.0.0/
--rw-r--r--   0 sanjay     (503) staff       (20)     1075 2023-02-26 11:35:04.000000 relistats-1.0.0/LICENSE
--rw-r--r--   0 sanjay     (503) staff       (20)     2874 2023-04-08 21:14:07.247073 relistats-1.0.0/PKG-INFO
--rw-r--r--   0 sanjay     (503) staff       (20)     2607 2023-04-08 21:07:11.000000 relistats-1.0.0/README.rst
-drwxr-xr-x   0 sanjay     (503) staff       (20)        0 2023-04-08 21:14:07.243627 relistats-1.0.0/relistats/
--rw-r--r--   0 sanjay     (503) staff       (20)       23 2023-03-04 14:14:04.000000 relistats-1.0.0/relistats/__init__.py
--rw-r--r--   0 sanjay     (503) staff       (20)      193 2023-02-16 02:17:40.000000 relistats-1.0.0/relistats/__main__.py
--rw-r--r--   0 sanjay     (503) staff       (20)     5123 2023-04-08 21:05:40.000000 relistats-1.0.0/relistats/binomial.py
-drwxr-xr-x   0 sanjay     (503) staff       (20)        0 2023-04-08 21:14:07.245533 relistats-1.0.0/relistats.egg-info/
--rw-r--r--   0 sanjay     (503) staff       (20)     2874 2023-04-08 21:14:07.000000 relistats-1.0.0/relistats.egg-info/PKG-INFO
--rw-r--r--   0 sanjay     (503) staff       (20)      306 2023-04-08 21:14:07.000000 relistats-1.0.0/relistats.egg-info/SOURCES.txt
--rw-r--r--   0 sanjay     (503) staff       (20)        1 2023-04-08 21:14:07.000000 relistats-1.0.0/relistats.egg-info/dependency_links.txt
--rw-r--r--   0 sanjay     (503) staff       (20)        6 2023-04-08 21:14:07.000000 relistats-1.0.0/relistats.egg-info/requires.txt
--rw-r--r--   0 sanjay     (503) staff       (20)       15 2023-04-08 21:14:07.000000 relistats-1.0.0/relistats.egg-info/top_level.txt
--rw-r--r--   0 sanjay     (503) staff       (20)      689 2023-04-08 21:14:07.247932 relistats-1.0.0/setup.cfg
--rw-r--r--   0 sanjay     (503) staff       (20)       38 2023-02-16 02:05:37.000000 relistats-1.0.0/setup.py
-drwxr-xr-x   0 sanjay     (503) staff       (20)        0 2023-04-08 21:14:07.246475 relistats-1.0.0/test/
--rw-r--r--   0 sanjay     (503) staff       (20)        0 2023-02-16 01:49:25.000000 relistats-1.0.0/test/__init__.py
--rw-r--r--   0 sanjay     (503) staff       (20)     3339 2023-02-16 02:08:21.000000 relistats-1.0.0/test/test_binomial.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:01:10.110759 relistats-1.1.0/
+-rw-rw-rw-   0        0        0     1095 2023-05-14 13:07:05.000000 relistats-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2947 2023-05-14 23:01:10.110759 relistats-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2669 2023-05-14 13:07:05.000000 relistats-1.1.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-14 23:01:10.077394 relistats-1.1.0/relistats/
+-rw-rw-rw-   0        0        0       81 2023-05-14 23:00:25.000000 relistats-1.1.0/relistats/__init__.py
+-rw-rw-rw-   0        0        0      201 2023-05-14 13:07:05.000000 relistats-1.1.0/relistats/__main__.py
+-rw-rw-rw-   0        0        0     4681 2023-05-14 23:00:25.000000 relistats-1.1.0/relistats/binom_fin.py
+-rw-rw-rw-   0        0        0     5285 2023-05-14 13:16:43.000000 relistats-1.1.0/relistats/binomial.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:01:10.104380 relistats-1.1.0/relistats.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-05-14 23:01:10.000000 relistats-1.1.0/relistats.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2023-05-14 23:01:10.000000 relistats-1.1.0/relistats.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 23:01:10.000000 relistats-1.1.0/relistats.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-14 23:01:10.000000 relistats-1.1.0/relistats.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 23:01:10.000000 relistats-1.1.0/relistats.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      729 2023-05-14 23:01:10.122753 relistats-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-05-14 13:07:05.000000 relistats-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 23:01:10.108761 relistats-1.1.0/test/
+-rw-rw-rw-   0        0        0        0 2023-05-14 13:07:05.000000 relistats-1.1.0/test/__init__.py
+-rw-rw-rw-   0        0        0     3819 2023-05-14 23:00:25.000000 relistats-1.1.0/test/test_binom_fin.py
+-rw-rw-rw-   0        0        0     3449 2023-05-14 23:00:25.000000 relistats-1.1.0/test/test_binomial.py
```

### Comparing `relistats-1.0.0/LICENSE` & `relistats-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright 2023 Sanjay M. Joshi
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the “Software”),
-to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense,
-and/or sell copies of the Software, and to permit persons to whom the
-Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
-FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+MIT License
+
+Copyright 2023 Sanjay M. Joshi
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the “Software”),
+to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense,
+and/or sell copies of the Software, and to permit persons to whom the
+Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
+FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
 DEALINGS IN THE SOFTWARE.
```

### Comparing `relistats-1.0.0/PKG-INFO` & `relistats-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-Metadata-Version: 2.1
-Name: relistats
-Version: 1.0.0
-Summary: Reliability Statistics
-Home-page: https://github.com/sanjaymjoshi/relistats
-Author: Sanjay Joshi
-Author-email: sanjaymjoshi@iitbombay.org
-License: MIT License
-Requires-Python: >=3.7
-License-File: LICENSE
-
-Reliability Statistics
-======================
-
-Reliability engineering deals with estimating parameters or qualities of a product or
-process or experiment. For simplicity, we assume that all units of a product or results
-of an experiment are random variables. Collectively, let's call them samples.
-We assume that the samples are independent (one sample has no effect on another
-sample) and identically distributed (the reliability or properties of underlying
-random variable stay the same for each sample).
-
-Concepts
---------
-- Reliability is probability of success. The math assumes infinite number of samples,
-  but we can get access to only a finite number of samples. Therefore, we can compute
-  only an estimate of the actual reliability. Based on the number of samples, we
-  qualify the quality of this estimate using *confidence*.
-
-- Confidence in reliability is probability that the actual reliability of the
-  population is at least the provided reliability level. 
-  For example, we can say "If we see zero failures in 10 samples of a success-failure
-  experiment, we have 95% confidence that the reliability is at least about 74%".
-
-- Assurance simplifies reliability and confidence by setting both of them the same.
-  The result is just one number that is easier to communicate. For example, 90%
-  assurance means 90% reliability with 90% confidence. Given the number of samples
-  and number of failures, assurance is just one number.
-
-This library provides methods to calculate these statistics.
-
-Example usage in a python file:
-
-.. code-block:: python
-
-   from relistats.binomial import assurance
-   
-   n = 22
-   a = assurance(n, 0) or 0
-   print(f"Assurance at {n} good samples: {a*100:.1f}%")
-
-See
-
-- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
-  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
-
-- Jupyter notebook showing how to use this library:
-  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
-
-- Interactive online version of the Jupyter notebook on
-  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
-
-Additional documentation:
-
-- `Usage <docs/source/usage.rst>`_ for installation and how to use.
-
-- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
-
-Credits
-----------
-This package was created with Cookiecutter and the
-`sourcery-ai/python-best-practices-cookiecutter
-<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
-project template.
+Metadata-Version: 2.1
+Name: relistats
+Version: 1.1.0
+Summary: Reliability Statistics
+Home-page: https://github.com/sanjaymjoshi/relistats
+Author: Sanjay Joshi
+Author-email: sanjaymjoshi@iitbombay.org
+License: MIT License
+Requires-Python: >=3.7
+License-File: LICENSE
+
+Reliability Statistics
+======================
+
+Reliability engineering deals with estimating parameters or qualities of a product or
+process or experiment. For simplicity, we assume that all units of a product or results
+of an experiment are random variables. Collectively, let's call them samples.
+We assume that the samples are independent (one sample has no effect on another
+sample) and identically distributed (the reliability or properties of underlying
+random variable stay the same for each sample).
+
+Concepts
+--------
+- Reliability is probability of success. The math assumes infinite number of samples,
+  but we can get access to only a finite number of samples. Therefore, we can compute
+  only an estimate of the actual reliability. Based on the number of samples, we
+  qualify the quality of this estimate using *confidence*.
+
+- Confidence in reliability is probability that the actual reliability of the
+  population is at least the provided reliability level. 
+  For example, we can say "If we see zero failures in 10 samples of a success-failure
+  experiment, we have 95% confidence that the reliability is at least about 74%".
+
+- Assurance simplifies reliability and confidence by setting both of them the same.
+  The result is just one number that is easier to communicate. For example, 90%
+  assurance means 90% reliability with 90% confidence. Given the number of samples
+  and number of failures, assurance is just one number.
+
+This library provides methods to calculate these statistics.
+
+Example usage in a python file:
+
+.. code-block:: python
+
+   from relistats.binomial import assurance
+   
+   n = 22
+   a = assurance(n, 0) or 0
+   print(f"Assurance at {n} good samples: {a*100:.1f}%")
+
+See
+
+- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
+  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
+
+- Jupyter notebook showing how to use this library:
+  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
+
+- Interactive online version of the Jupyter notebook on
+  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
+
+Additional documentation:
+
+- `Usage <docs/source/usage.rst>`_ for installation and how to use.
+
+- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
+
+Credits
+----------
+This package was created with Cookiecutter and the
+`sourcery-ai/python-best-practices-cookiecutter
+<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
+project template.
```

### Comparing `relistats-1.0.0/README.rst` & `relistats-1.1.0/README.rst`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-Reliability Statistics
-======================
-
-Reliability engineering deals with estimating parameters or qualities of a product or
-process or experiment. For simplicity, we assume that all units of a product or results
-of an experiment are random variables. Collectively, let's call them samples.
-We assume that the samples are independent (one sample has no effect on another
-sample) and identically distributed (the reliability or properties of underlying
-random variable stay the same for each sample).
-
-Concepts
---------
-- Reliability is probability of success. The math assumes infinite number of samples,
-  but we can get access to only a finite number of samples. Therefore, we can compute
-  only an estimate of the actual reliability. Based on the number of samples, we
-  qualify the quality of this estimate using *confidence*.
-
-- Confidence in reliability is probability that the actual reliability of the
-  population is at least the provided reliability level. 
-  For example, we can say "If we see zero failures in 10 samples of a success-failure
-  experiment, we have 95% confidence that the reliability is at least about 74%".
-
-- Assurance simplifies reliability and confidence by setting both of them the same.
-  The result is just one number that is easier to communicate. For example, 90%
-  assurance means 90% reliability with 90% confidence. Given the number of samples
-  and number of failures, assurance is just one number.
-
-This library provides methods to calculate these statistics.
-
-Example usage in a python file:
-
-.. code-block:: python
-
-   from relistats.binomial import assurance
-   
-   n = 22
-   a = assurance(n, 0) or 0
-   print(f"Assurance at {n} good samples: {a*100:.1f}%")
-
-See
-
-- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
-  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
-
-- Jupyter notebook showing how to use this library:
-  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
-
-- Interactive online version of the Jupyter notebook on
-  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
-
-Additional documentation:
-
-- `Usage <docs/source/usage.rst>`_ for installation and how to use.
-
-- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
-
-Credits
-----------
-This package was created with Cookiecutter and the
-`sourcery-ai/python-best-practices-cookiecutter
-<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
-project template.
+Reliability Statistics
+======================
+
+Reliability engineering deals with estimating parameters or qualities of a product or
+process or experiment. For simplicity, we assume that all units of a product or results
+of an experiment are random variables. Collectively, let's call them samples.
+We assume that the samples are independent (one sample has no effect on another
+sample) and identically distributed (the reliability or properties of underlying
+random variable stay the same for each sample).
+
+Concepts
+--------
+- Reliability is probability of success. The math assumes infinite number of samples,
+  but we can get access to only a finite number of samples. Therefore, we can compute
+  only an estimate of the actual reliability. Based on the number of samples, we
+  qualify the quality of this estimate using *confidence*.
+
+- Confidence in reliability is probability that the actual reliability of the
+  population is at least the provided reliability level. 
+  For example, we can say "If we see zero failures in 10 samples of a success-failure
+  experiment, we have 95% confidence that the reliability is at least about 74%".
+
+- Assurance simplifies reliability and confidence by setting both of them the same.
+  The result is just one number that is easier to communicate. For example, 90%
+  assurance means 90% reliability with 90% confidence. Given the number of samples
+  and number of failures, assurance is just one number.
+
+This library provides methods to calculate these statistics.
+
+Example usage in a python file:
+
+.. code-block:: python
+
+   from relistats.binomial import assurance
+   
+   n = 22
+   a = assurance(n, 0) or 0
+   print(f"Assurance at {n} good samples: {a*100:.1f}%")
+
+See
+
+- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
+  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
+
+- Jupyter notebook showing how to use this library:
+  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
+
+- Interactive online version of the Jupyter notebook on
+  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
+
+Additional documentation:
+
+- `Usage <docs/source/usage.rst>`_ for installation and how to use.
+
+- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
+
+Credits
+----------
+This package was created with Cookiecutter and the
+`sourcery-ai/python-best-practices-cookiecutter
+<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
+project template.
```

### Comparing `relistats-1.0.0/relistats/binomial.py` & `relistats-1.1.0/relistats/binomial.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,162 +1,162 @@
-""" Reliability Engineering Statistics for Binomial Distributions
-
-Also known as Bernoulli Trials.
-
-Reference:
-S.M. Joshi, "Computation of Reliability Statistics for
-Success-Failure Experiments," arXiv:2303.03167 [stat.ME], March 2023.
-https://doi.org/10.48550/arXiv.2303.03167
-"""
-from math import sqrt
-from typing import Optional
-
-import scipy.optimize as opt
-import scipy.stats as st
-
-
-def confidence(n: int, f: int, r: float) -> Optional[float]:
-    """Confidence [0, 1] in reliability r using closed-form expression.
-
-    :param n: number of samples
-    :type n: int, >=0
-    :param f: number of failures
-    :type f: int, >=0
-    :param r: reliability level
-    :type r: float, [0, 1]
-    :return: Confidence or None if it could not be computed
-    :rtype: float, optional
-    """
-    if n <= 0 or f < 0 or r < 0 or r > 1:
-        return None
-    # Scipy's binom object provides 'survival function', which is 1 - CDF.
-    prob_failure = 1 - r
-    return st.binom.sf(f, n, prob_failure)
-
-
-def _wilson_center(p, n, c):
-    """Center of Wilson score interval. See reference below."""
-    z = st.norm.ppf(c)
-    return (p + z * z / (2 * n)) / (1 + z * z / n)
-
-
-def _wilson_lower(p, n, c):
-    """Lower bound of Wilson score interval. See reference below."""
-    z = st.norm.ppf(c)
-    p50 = _wilson_center(p, n, c)
-    part2 = z / (1 + z * z / n) * sqrt(p * (1 - p) / n + z * z / (4 * n * n))
-    return p50 - part2
-
-
-def _wilson_lower_corrected(p, n, c):
-    """Lower bound of Wilson score interval, with continuity correction."""
-    return _wilson_lower(max(p - 1 / (2 * n), 0), n, c)
-
-
-def reliability_closed(n: int, f: int, c: float) -> Optional[float]:
-    """Approximate minimum reliability [0, 1] at confidence level c.
-    The approximation is within about 5% of actual reliability and uses
-    closed-form expression for computation called 'Wilson Score Interval
-    with Continuity Correction' [Wallis, Sean A. (2013). "Binomial
-    confidence intervals and contingency tests: mathematical fundamentals
-    and the evaluation of alternative methods". Journal of Quantitative
-    Linguistics. 20 (3): 178–208].
-
-    :param n: number of samples
-    :type n: int, >=0
-    :param f: number of failures
-    :type f: int, >=0
-    :param c: confidence level
-    :type c: float, [0, 1]
-    :return: Reliability or None if it could not be computed
-    :rtype: float, optional
-    """
-    if n <= 0 or f < 0 or c < 0 or c > 1:
-        return None
-
-    return _wilson_lower_corrected((n - f) / n, n, c)
-
-
-def _reliability_fn(x: float, n: int, f: int, c: float) -> float:
-    """Function to find roots of c = confidence(n, f, x)"""
-    c_hat = confidence(n, f, x) or 0
-    return c_hat - c
-
-
-def reliability_optim(n: int, f: int, c: float, tol=0.001) -> Optional[float]:
-    """Minimum reliability [0, 1] at confidence level c using numerical
-    optimization (Brent's method). The approximation is within specified
-    tolerance limit.
-
-    :param n: number of samples
-    :type n: int, >=0
-    :param f: number of failures
-    :type f: int, >=0
-    :param c: confidence level
-    :type c: float, [0, 1]
-    :param tol: accuracy tolerance
-    :type tol: float, optional
-
-    :return: Reliability or None if it could not be computed
-    :rtype: float, optional
-    """
-    if n <= 0 or f < 0 or c < 0 or c > 1:
-        return None
-
-    # Use numerical optimization to find real root of the confidence equation
-    # c - confidence(n, f, r)
-    return opt.brentq(
-        _reliability_fn,
-        a=0,  # Lowest possible value
-        b=1,  # Highest possible value
-        args=(n, f, c),
-        xtol=tol,
-    )
-
-
-def reliability(n: int, f: int, c: float) -> Optional[float]:
-    """Minimum reliability at confidence level c
-
-    :param n: number of samples
-    :type n: int, >=0
-    :param f: number of failures
-    :type f: int, >=0
-    :param c: confidence level
-    :type c: float, [0, 1]
-    :return: Reliability or None if it could not be computed
-    :rtype: float, optional
-    """
-    return reliability_optim(n, f, c)
-
-
-def _assurance_fn(x: float, n: int, f: int) -> float:
-    """Function to find roots of x = confidence(n, f, x)"""
-    c = confidence(n, f, x) or 0
-    return x - c
-
-
-def assurance(n: int, f: int, tol=0.001) -> Optional[float]:
-    """Assurance [0, 1], i.e., confidence = reliability. For example,
-    90% assurance means 90% confidence in 90% reliability (at n=22, f=0).
-    This method uses numerical approach of Brent's method to compute
-    the solution within the specified tolerance.
-
-    :param n: number of samples
-    :type n: int, >=0
-    :param f: number of failures
-    :type f: int, >=0
-    :param tol: accuracy tolerance
-    :type tol: float, optional
-    :return: Assurance or None if it could not be computed
-    :rtype: float, optional
-    """
-    if n <= 0 or f < 0:
-        return None
-    # Use brentq method to find real root of the assurance equation
-    # a = c = r. Meaning a = confidence(n, f, a)
-    return opt.brentq(
-        _assurance_fn,
-        a=0,  # Lowest possible value
-        b=1,  # Highest possible value
-        args=(n, f),
-        xtol=tol,
-    )
+""" Reliability Engineering Statistics for Binomial Distributions
+
+Also known as Bernoulli Trials.
+
+Reference:
+S.M. Joshi, "Computation of Reliability Statistics for
+Success-Failure Experiments," arXiv:2303.03167 [stat.ME], March 2023.
+https://doi.org/10.48550/arXiv.2303.03167
+"""
+from math import sqrt
+from typing import Optional
+
+import scipy.optimize as opt
+import scipy.stats as st
+
+
+def confidence(n: int, f: int, r: float) -> Optional[float]:
+    """Confidence [0, 1] in reliability r using closed-form expression.
+
+    :param n: number of samples
+    :type n: int, >=0
+    :param f: number of failures
+    :type f: int, >=0
+    :param r: reliability level
+    :type r: float, [0, 1]
+    :return: Confidence or None if it could not be computed
+    :rtype: float, optional
+    """
+    if n <= 0 or f < 0 or r < 0 or r > 1:
+        return None
+    # Scipy's binom object provides 'survival function', which is 1 - CDF.
+    prob_failure = 1 - r
+    return st.binom.sf(f, n, prob_failure)
+
+
+def _wilson_center(p, n, c):
+    """Center of Wilson score interval. See reference below."""
+    z = st.norm.ppf(c)
+    return (p + z * z / (2 * n)) / (1 + z * z / n)
+
+
+def _wilson_lower(p, n, c):
+    """Lower bound of Wilson score interval. See reference below."""
+    z = st.norm.ppf(c)
+    p50 = _wilson_center(p, n, c)
+    part2 = z / (1 + z * z / n) * sqrt(p * (1 - p) / n + z * z / (4 * n * n))
+    return p50 - part2
+
+
+def _wilson_lower_corrected(p, n, c):
+    """Lower bound of Wilson score interval, with continuity correction."""
+    return _wilson_lower(max(p - 1 / (2 * n), 0), n, c)
+
+
+def reliability_closed(n: int, f: int, c: float) -> Optional[float]:
+    """Approximate minimum reliability [0, 1] at confidence level c.
+    The approximation is within about 5% of actual reliability and uses
+    closed-form expression for computation called 'Wilson Score Interval
+    with Continuity Correction' [Wallis, Sean A. (2013). "Binomial
+    confidence intervals and contingency tests: mathematical fundamentals
+    and the evaluation of alternative methods". Journal of Quantitative
+    Linguistics. 20 (3): 178–208].
+
+    :param n: number of samples
+    :type n: int, >=0
+    :param f: number of failures
+    :type f: int, >=0
+    :param c: confidence level
+    :type c: float, [0, 1]
+    :return: Reliability or None if it could not be computed
+    :rtype: float, optional
+    """
+    if n <= 0 or f < 0 or c < 0 or c > 1:
+        return None
+
+    return _wilson_lower_corrected((n - f) / n, n, c)
+
+
+def _reliability_fn(x: float, n: int, f: int, c: float) -> float:
+    """Function to find roots of c = confidence(n, f, x)"""
+    c_hat = confidence(n, f, x) or 0
+    return c_hat - c
+
+
+def reliability_optim(n: int, f: int, c: float, tol=0.001) -> Optional[float]:
+    """Minimum reliability [0, 1] at confidence level c using numerical
+    optimization (Brent's method). The approximation is within specified
+    tolerance limit.
+
+    :param n: number of samples
+    :type n: int, >=0
+    :param f: number of failures
+    :type f: int, >=0
+    :param c: confidence level
+    :type c: float, [0, 1]
+    :param tol: accuracy tolerance
+    :type tol: float, optional
+
+    :return: Reliability or None if it could not be computed
+    :rtype: float, optional
+    """
+    if n <= 0 or f < 0 or c < 0 or c > 1:
+        return None
+
+    # Use numerical optimization to find real root of the confidence equation
+    # c - confidence(n, f, r)
+    return opt.brentq(
+        _reliability_fn,
+        a=0,  # Lowest possible value
+        b=1,  # Highest possible value
+        args=(n, f, c),
+        xtol=tol,
+    )
+
+
+def reliability(n: int, f: int, c: float) -> Optional[float]:
+    """Minimum reliability at confidence level c
+
+    :param n: number of samples
+    :type n: int, >=0
+    :param f: number of failures
+    :type f: int, >=0
+    :param c: confidence level
+    :type c: float, [0, 1]
+    :return: Reliability or None if it could not be computed
+    :rtype: float, optional
+    """
+    return reliability_optim(n, f, c)
+
+
+def _assurance_fn(x: float, n: int, f: int) -> float:
+    """Function to find roots of x = confidence(n, f, x)"""
+    c = confidence(n, f, x) or 0
+    return x - c
+
+
+def assurance(n: int, f: int, tol=0.001) -> Optional[float]:
+    """Assurance [0, 1], i.e., confidence = reliability. For example,
+    90% assurance means 90% confidence in 90% reliability (at n=22, f=0).
+    This method uses numerical approach of Brent's method to compute
+    the solution within the specified tolerance.
+
+    :param n: number of samples
+    :type n: int, >=0
+    :param f: number of failures
+    :type f: int, >=0
+    :param tol: accuracy tolerance
+    :type tol: float, optional
+    :return: Assurance or None if it could not be computed
+    :rtype: float, optional
+    """
+    if n <= 0 or f < 0:
+        return None
+    # Use brentq method to find real root of the assurance equation
+    # a = c = r. Meaning a = confidence(n, f, a)
+    return opt.brentq(
+        _assurance_fn,
+        a=0,  # Lowest possible value
+        b=1,  # Highest possible value
+        args=(n, f),
+        xtol=tol,
+    )
```

### Comparing `relistats-1.0.0/relistats.egg-info/PKG-INFO` & `relistats-1.1.0/relistats.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-Metadata-Version: 2.1
-Name: relistats
-Version: 1.0.0
-Summary: Reliability Statistics
-Home-page: https://github.com/sanjaymjoshi/relistats
-Author: Sanjay Joshi
-Author-email: sanjaymjoshi@iitbombay.org
-License: MIT License
-Requires-Python: >=3.7
-License-File: LICENSE
-
-Reliability Statistics
-======================
-
-Reliability engineering deals with estimating parameters or qualities of a product or
-process or experiment. For simplicity, we assume that all units of a product or results
-of an experiment are random variables. Collectively, let's call them samples.
-We assume that the samples are independent (one sample has no effect on another
-sample) and identically distributed (the reliability or properties of underlying
-random variable stay the same for each sample).
-
-Concepts
---------
-- Reliability is probability of success. The math assumes infinite number of samples,
-  but we can get access to only a finite number of samples. Therefore, we can compute
-  only an estimate of the actual reliability. Based on the number of samples, we
-  qualify the quality of this estimate using *confidence*.
-
-- Confidence in reliability is probability that the actual reliability of the
-  population is at least the provided reliability level. 
-  For example, we can say "If we see zero failures in 10 samples of a success-failure
-  experiment, we have 95% confidence that the reliability is at least about 74%".
-
-- Assurance simplifies reliability and confidence by setting both of them the same.
-  The result is just one number that is easier to communicate. For example, 90%
-  assurance means 90% reliability with 90% confidence. Given the number of samples
-  and number of failures, assurance is just one number.
-
-This library provides methods to calculate these statistics.
-
-Example usage in a python file:
-
-.. code-block:: python
-
-   from relistats.binomial import assurance
-   
-   n = 22
-   a = assurance(n, 0) or 0
-   print(f"Assurance at {n} good samples: {a*100:.1f}%")
-
-See
-
-- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
-  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
-
-- Jupyter notebook showing how to use this library:
-  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
-
-- Interactive online version of the Jupyter notebook on
-  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
-
-Additional documentation:
-
-- `Usage <docs/source/usage.rst>`_ for installation and how to use.
-
-- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
-
-Credits
-----------
-This package was created with Cookiecutter and the
-`sourcery-ai/python-best-practices-cookiecutter
-<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
-project template.
+Metadata-Version: 2.1
+Name: relistats
+Version: 1.1.0
+Summary: Reliability Statistics
+Home-page: https://github.com/sanjaymjoshi/relistats
+Author: Sanjay Joshi
+Author-email: sanjaymjoshi@iitbombay.org
+License: MIT License
+Requires-Python: >=3.7
+License-File: LICENSE
+
+Reliability Statistics
+======================
+
+Reliability engineering deals with estimating parameters or qualities of a product or
+process or experiment. For simplicity, we assume that all units of a product or results
+of an experiment are random variables. Collectively, let's call them samples.
+We assume that the samples are independent (one sample has no effect on another
+sample) and identically distributed (the reliability or properties of underlying
+random variable stay the same for each sample).
+
+Concepts
+--------
+- Reliability is probability of success. The math assumes infinite number of samples,
+  but we can get access to only a finite number of samples. Therefore, we can compute
+  only an estimate of the actual reliability. Based on the number of samples, we
+  qualify the quality of this estimate using *confidence*.
+
+- Confidence in reliability is probability that the actual reliability of the
+  population is at least the provided reliability level. 
+  For example, we can say "If we see zero failures in 10 samples of a success-failure
+  experiment, we have 95% confidence that the reliability is at least about 74%".
+
+- Assurance simplifies reliability and confidence by setting both of them the same.
+  The result is just one number that is easier to communicate. For example, 90%
+  assurance means 90% reliability with 90% confidence. Given the number of samples
+  and number of failures, assurance is just one number.
+
+This library provides methods to calculate these statistics.
+
+Example usage in a python file:
+
+.. code-block:: python
+
+   from relistats.binomial import assurance
+   
+   n = 22
+   a = assurance(n, 0) or 0
+   print(f"Assurance at {n} good samples: {a*100:.1f}%")
+
+See
+
+- Paper: S.M. Joshi, "Computation of Reliability Statistics for Success-Failure Experiments,"
+  `arXiv:2303.03167 [stat.ME] <https://doi.org/10.48550/arXiv.2303.03167>`_, March 2023.
+
+- Jupyter notebook showing how to use this library:
+  `relistats_notebook <https://github.com/sanjaymjoshi/relistats_notebook>`_
+
+- Interactive online version of the Jupyter notebook on
+  `Google Colab <https://colab.research.google.com/github/sanjaymjoshi/relistats_notebook/blob/main/relistats_binomial.ipynb>`_.
+
+Additional documentation:
+
+- `Usage <docs/source/usage.rst>`_ for installation and how to use.
+
+- `Background <docs/source/background.rst>`_ for concepts and mathematical background.
+
+Credits
+----------
+This package was created with Cookiecutter and the
+`sourcery-ai/python-best-practices-cookiecutter
+<https://github.com/sourcery-ai/python-best-practices-cookiecutter>`_
+project template.
```

### Comparing `relistats-1.0.0/test/test_binomial.py` & `relistats-1.1.0/test/test_binomial.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,112 +1,111 @@
-from dataclasses import asdict, dataclass
-
-import pytest
-
-from relistats.binomial import (
-    assurance,
-    confidence,
-    reliability,
-    reliability_closed,
-    reliability_optim,
-)
-
-
-@dataclass
-class NFRC:
-    n: int
-    f: int
-    r: float
-    c: float
-
-
-test_nfrc = (
-    NFRC(1, 0, 0.5, 0.5),
-    NFRC(2, 0, 0.5, 0.75),
-    NFRC(2, 1, 0.5, 0.25),
-    NFRC(8, 0, 0.7, 0.942),
-    NFRC(8, 0, 0.9, 0.570),
-    NFRC(10, 9, 0.1, 0.349),
-    NFRC(100, 10, 0.9, 0.417),
-    NFRC(1000, 100, 0.9, 0.473),
-    NFRC(10000, 1000, 0.9, 0.492),
-)
-
-
-def test_confidence() -> None:
-
-    # Confidence computation is exact, so set the tolerance tight
-    ABS_TOL_CONFIDENCE = 0.001
-    for x in test_nfrc:
-        print(f"Testing confidence: {asdict(x)}")
-        assert confidence(x.n, x.f, x.r) == pytest.approx(x.c, abs=ABS_TOL_CONFIDENCE)
-
-    assert confidence(2, 2, 0.5) == 0
-    assert confidence(2, 3, 0.5) == 0
-    assert confidence(20, 0, 0) == 1
-    assert confidence(20, 0, 1) == 0
-
-    assert confidence(2, 0, 2) is None
-    assert confidence(2, -2, 0.5) is None
-    assert confidence(-2, 0, 0.5) is None
-    assert confidence(2, 0, -0.5) is None
-
-
-def test_reliability_closed() -> None:
-    # Reliability closed form computation is approximate, so set the tolerance loose
-    ABS_TOL_RELIABILITY_CLOSED = 0.03
-
-    for x in test_nfrc:
-        print(f"Testing reliability: {asdict(x)}")
-        c1 = confidence(x.n, x.f, x.r)
-        if c1 is None:
-            c1 = 0
-        assert reliability_closed(x.n, x.f, c1) == pytest.approx(
-            x.r, abs=ABS_TOL_RELIABILITY_CLOSED
-        )
-
-    assert reliability_closed(2, 0, 2) is None
-    assert reliability_closed(2, -2, 0.5) is None
-    assert reliability_closed(-2, 0, 0.5) is None
-    assert reliability_closed(2, 0, -0.5) is None
-
-
-def test_reliability_optim() -> None:
-    # Reliability computation via optimization is more accurate, so set the tolerance tight
-    ABS_TOL_RELIABILITY_OPTIM = 0.001
-    for x in test_nfrc:
-        print(f"Testing reliability: {asdict(x)}")
-        c1 = confidence(x.n, x.f, x.r)
-        if c1 is None:
-            c1 = 0
-        assert reliability_optim(x.n, x.f, c1) == pytest.approx(
-            x.r, abs=ABS_TOL_RELIABILITY_OPTIM
-        )
-
-    assert reliability_optim(20, 0, 0.9, 0.0001) == pytest.approx(0.8912, abs=0.0001)
-
-    assert reliability_optim(2, 0, 2) is None
-    assert reliability_optim(2, -2, 0.5) is None
-    assert reliability_optim(-2, 0, 0.5) is None
-    assert reliability_optim(2, 0, -0.5) is None
-
-
-def test_reliability() -> None:
-    # Reliability computation should be accurate, so set the tolerance tight
-    ABS_TOL_RELIABILITY = 0.001
-    for x in test_nfrc:
-        print(f"Testing reliability: {asdict(x)}")
-        c1 = confidence(x.n, x.f, x.r)
-        if c1 is None:
-            c1 = 0
-        assert reliability(x.n, x.f, c1) == pytest.approx(x.r, abs=ABS_TOL_RELIABILITY)
-
-
-def test_assurance() -> None:
-    assert assurance(22, 0) == pytest.approx(0.9, abs=0.001)
-    assert assurance(59, 0) == pytest.approx(0.95, abs=0.001)
-    assert assurance(22, 2) == pytest.approx(0.812, abs=0.001)
-    assert assurance(59, 6) == pytest.approx(0.842, abs=0.001)
-    assert assurance(59, 10, 0.0001) == pytest.approx(0.7798, abs=0.0001)
-
-    assert assurance(2, -2) is None
-    assert assurance(-2, 0) is None
+from dataclasses import asdict, dataclass
+
+import pytest
+
+from relistats.binomial import (
+    assurance,
+    confidence,
+    reliability,
+    reliability_closed,
+    reliability_optim,
+)
+
+
+@dataclass
+class NFRC:
+    n: int
+    f: int
+    r: float
+    c: float
+
+
+test_nfrc = (
+    NFRC(1, 0, 0.5, 0.5),
+    NFRC(2, 0, 0.5, 0.75),
+    NFRC(2, 1, 0.5, 0.25),
+    NFRC(8, 0, 0.7, 0.942),
+    NFRC(8, 0, 0.9, 0.570),
+    NFRC(10, 9, 0.1, 0.349),
+    NFRC(100, 10, 0.9, 0.417),
+    NFRC(1000, 100, 0.9, 0.473),
+    NFRC(10000, 1000, 0.9, 0.492),
+)
+
+
+def test_confidence() -> None:
+    # Confidence computation is exact, so set the tolerance tight
+    ABS_TOL_CONFIDENCE = 0.001
+    for x in test_nfrc:
+        print(f"Testing confidence: {asdict(x)}")
+        assert confidence(x.n, x.f, x.r) == pytest.approx(x.c, abs=ABS_TOL_CONFIDENCE)
+
+    assert confidence(2, 2, 0.5) == 0
+    assert confidence(2, 3, 0.5) == 0
+    assert confidence(20, 0, 0) == 1
+    assert confidence(20, 0, 1) == 0
+
+    assert confidence(2, 0, 2) is None
+    assert confidence(2, -2, 0.5) is None
+    assert confidence(-2, 0, 0.5) is None
+    assert confidence(2, 0, -0.5) is None
+
+
+def test_reliability_closed() -> None:
+    # Reliability closed form computation is approximate, so set the tolerance loose
+    ABS_TOL_RELIABILITY_CLOSED = 0.03
+
+    for x in test_nfrc:
+        print(f"Testing reliability: {asdict(x)}")
+        c1 = confidence(x.n, x.f, x.r)
+        if c1 is None:
+            c1 = 0
+        assert reliability_closed(x.n, x.f, c1) == pytest.approx(
+            x.r, abs=ABS_TOL_RELIABILITY_CLOSED
+        )
+
+    assert reliability_closed(2, 0, 2) is None
+    assert reliability_closed(2, -2, 0.5) is None
+    assert reliability_closed(-2, 0, 0.5) is None
+    assert reliability_closed(2, 0, -0.5) is None
+
+
+def test_reliability_optim() -> None:
+    # Reliability computation via optimization is more accurate, so set the tolerance tight
+    ABS_TOL_RELIABILITY_OPTIM = 0.001
+    for x in test_nfrc:
+        print(f"Testing reliability: {asdict(x)}")
+        c1 = confidence(x.n, x.f, x.r)
+        if c1 is None:
+            c1 = 0
+        assert reliability_optim(x.n, x.f, c1) == pytest.approx(
+            x.r, abs=ABS_TOL_RELIABILITY_OPTIM
+        )
+
+    assert reliability_optim(20, 0, 0.9, 0.0001) == pytest.approx(0.8912, abs=0.0001)
+
+    assert reliability_optim(2, 0, 2) is None
+    assert reliability_optim(2, -2, 0.5) is None
+    assert reliability_optim(-2, 0, 0.5) is None
+    assert reliability_optim(2, 0, -0.5) is None
+
+
+def test_reliability() -> None:
+    # Reliability computation should be accurate, so set the tolerance tight
+    ABS_TOL_RELIABILITY = 0.001
+    for x in test_nfrc:
+        print(f"Testing reliability: {asdict(x)}")
+        c1 = confidence(x.n, x.f, x.r)
+        if c1 is None:
+            c1 = 0
+        assert reliability(x.n, x.f, c1) == pytest.approx(x.r, abs=ABS_TOL_RELIABILITY)
+
+
+def test_assurance() -> None:
+    assert assurance(22, 0) == pytest.approx(0.9, abs=0.001)
+    assert assurance(59, 0) == pytest.approx(0.95, abs=0.001)
+    assert assurance(22, 2) == pytest.approx(0.812, abs=0.001)
+    assert assurance(59, 6) == pytest.approx(0.842, abs=0.001)
+    assert assurance(59, 10, 0.0001) == pytest.approx(0.7798, abs=0.0001)
+
+    assert assurance(2, -2) is None
+    assert assurance(-2, 0) is None
```

