# Comparing `tmp/pytest_smtpd-0.1.0.tar.gz` & `tmp/pytest-smtpd-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pytest-smtpd-0.1.0a0.tar", last modified: Fri May  5 23:07:39 2023, max compression
```

## Comparing `pytest_smtpd-0.1.0.tar` & `pytest-smtpd-0.1.0a0.tar`

### file list

```diff
@@ -1,6 +1,19 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/src/pytest_smtpd/__init__.py
--rw-r--r--   0        0        0     1825 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/LICENSE
--rw-r--r--   0        0        0     6618 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/README.md
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7962 2020-02-02 00:00:00.000000 pytest_smtpd-0.1.0/PKG-INFO
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-05 23:07:39.113151 pytest-smtpd-0.1.0a0/
+-rw-r--r--   0 james     (1000) james     (1000)     1068 2023-05-04 23:55:36.000000 pytest-smtpd-0.1.0a0/LICENSE
+-rw-r--r--   0 james     (1000) james     (1000)     7962 2023-05-05 23:07:39.113151 pytest-smtpd-0.1.0a0/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)     6838 2023-05-05 21:46:39.000000 pytest-smtpd-0.1.0a0/README.md
+-rw-r--r--   0 james     (1000) james     (1000)       94 2023-05-04 21:47:32.000000 pytest-smtpd-0.1.0a0/pyproject.toml
+-rw-r--r--   0 james     (1000) james     (1000)     1773 2023-05-05 23:07:39.123151 pytest-smtpd-0.1.0a0/setup.cfg
+-rw-r--r--   0 james     (1000) james     (1000)       38 2023-05-04 21:47:32.000000 pytest-smtpd-0.1.0a0/setup.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-05 23:07:39.093151 pytest-smtpd-0.1.0a0/src/
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-05 23:07:39.113151 pytest-smtpd-0.1.0a0/src/pytest_smtpd/
+-rw-r--r--   0 james     (1000) james     (1000)      148 2023-05-05 23:07:10.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd/__init__.py
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-05 23:07:39.113151 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/
+-rw-r--r--   0 james     (1000) james     (1000)     7962 2023-05-05 23:07:39.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/PKG-INFO
+-rw-r--r--   0 james     (1000) james     (1000)      340 2023-05-05 23:07:39.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/SOURCES.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2023-05-05 23:07:39.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/dependency_links.txt
+-rw-r--r--   0 james     (1000) james     (1000)        1 2023-05-05 19:58:37.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/not-zip-safe
+-rw-r--r--   0 james     (1000) james     (1000)       45 2023-05-05 23:07:39.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/requires.txt
+-rw-r--r--   0 james     (1000) james     (1000)       13 2023-05-05 23:07:39.000000 pytest-smtpd-0.1.0a0/src/pytest_smtpd.egg-info/top_level.txt
+drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-05-05 23:07:39.113151 pytest-smtpd-0.1.0a0/tests/
+-rw-r--r--   0 james     (1000) james     (1000)      258 2023-05-05 21:10:49.000000 pytest-smtpd-0.1.0a0/tests/test_fixture.py
```

### Comparing `pytest_smtpd-0.1.0/LICENSE` & `pytest-smtpd-0.1.0a0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 James Warne
+Copyright (c) 2020 James Warne
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `pytest_smtpd-0.1.0/README.md` & `pytest-smtpd-0.1.0a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 This fixture is intended to address cases where to test an application that sends an email, it needs to be intercepted for subsequent processing. For example, sending an email with a code for password reset or two-factor authentication. This fixture allows a test to trigger the email being sent, ensure that it's sent, and read the email.
 
 ## Installing
 
 To install using pip, first upgrade pip to the latest version to avoid any issues installing `cryptography`:
 
 ```bash
-python -m pip install --upgrade pip
-pip install pytest-smtpd
+$ python -m pip install --upgrade pip
+$ pip install pytest-smtpd
 ```
 
 Or, if you're using setuptools, it can be included in the `extras_require` argument of a `setup.py` file:
 
 ```python
 setup(
     ...
@@ -26,16 +26,16 @@
     },
 )
 ```
 
 and then installed with pip (-e assumes that you want your project to be editable):
 
 ```bash
-python -m pip install --upgrade pip
-pip install -e .[test]
+$ python -m pip install --upgrade pip
+$ pip install -e .[test]
 ```
 
 ## Using
 
 The `SMTPDFix` plugin, `smtpd`, automatically registers for use with pytest when you install smtpdfix. To use it simply add to your test method.
 
 ```python
@@ -115,50 +115,55 @@
 `login_password` | `SMTPD_LOGIN_PASSWORD` | `password`           | Password for default authentication.
 `use_ssl`        | `SMTPD_USE_SSL`        | `False`              | Whether the fixture should use fixed TLS/SSL for transactions. If using smtplib requires that `SMTP_SSL` be used instead of `SMTP`.
 `use_starttls`   | `SMTPD_USE_STARTTLS`   | `False`              | Whether the fixture should use StartTLS to encrypt the connections. If using `smtplib` requires that `SMTP.starttls()` is called before other commands are issued. Overrides `use_tls` as the preferred method for securing communications with the client.
 `enforce_auth`   | `SMTPD_ENFORCE_AUTH`   | `False`              | If set to true then the fixture refuses MAIL, RCPT, DATA commands until authentication is completed.
 `ssl_cert_path`  | `SMTPD_SSL_CERTS_PATH` | `./certs/`           | The path to the key and certificate in PEM format for encryption with SSL/TLS or StartTLS.
 `ssl_cert_files` | `SMTPD_SSL_CERT_FILE` and `SMTPD_SSL_KEY_FILE` | `("cert.pem", None)` | A tuple of the path for the certificate file and key file in PEM format.
 
+
+
 ## Alternatives
 
 Many libraries for sending email have built-in methods for testing and using these methods should generally be prefered over pytest-smtpd. Some known solutions:
 
 + **fastapi-mail**: has a `record_messsages()` method to intercept the mail. Instructions on how to suppress the sending of mail and implement it can be seen at [https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail](https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail)
 + **flask-mail**: has a method to suppress sending and capture the email for testing purposes. [Instructions](https://pythonhosted.org/Flask-Mail/#unit-tests-and-suppressing-emails)
 
 ## Developing
 
 To develop and test smtpdfix you will need to install [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests, [isort](https://pycqa.github.io/isort/) to sort imports and [flake8](https://flake8.pycqa.org/en/latest/) to lint. To install in a virtual environment for development:
 
 ```bash
-python -m venv venv
-./venv/scripts/activate
-pip install -e .[dev]
+$ python -m venv venv
+$ ./venv/scripts/activate
+$ pip install -e .[dev]
 ```
 
 Code is tested using tox:
 
 ```bash
-tox
+$ tox
 ```
 
 Quick tests can be handled by running pytest directly:
 
 ```bash
-pytest
+$ pytest
 ```
 
 We include a [pre-commit](https://pre-commit.com/) configuration file to automate checks and clean up imports before pushing code. In order to install pre-commit git hooks:
 
 ```bash
-pip install pre-commit
-pre-commit install
+$ pip install pre-commit
+$ pre-commit install
 ```
 
 ## Known Issues
 
 + Firewalls may interfere with the operation of the smtp server.
-+ Authenticating with LOGIN and PLAIN mechanisms fails over TLS/SSL, but works with STARTTLS. [smtpdfix Issue #10](https://github.com/bebleo/smtpdfix/issues/10)
-+ Currently no support for termination through signals. [smtpdfix Issue #4](https://github.com/bebleo/smtpdfix/issues/4)
++ Authenticating with LOGIN and PLAIN mechanisms fails over TLS/SSL, but works with STARTTLS. [Issue #10](https://github.com/bebleo/smtpdfix/issues/10)
++ Currently no support for termination through signals. [Issue #4](https://github.com/bebleo/smtpdfix/issues/4)
++ If the fixture start exceeds the `ready_timeout` and aborts the host and port are not consistently released and subsequent uses may result in an error. [Issue #80](https://github.com/bebleo/smtpdfix/issues/80)
 
 Written with ☕ and ❤ in Montreal, QC
+
+
```

### Comparing `pytest_smtpd-0.1.0/PKG-INFO` & `pytest-smtpd-0.1.0a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,48 @@
 Metadata-Version: 2.1
 Name: pytest-smtpd
-Version: 0.1.0
-Summary: An SMTP server for testing built on aiosmtpd
+Version: 0.1.0a0
+Summary: package_description
+Author: James Warne
+Author-email: bebleo@yahoo.com
+License: MIT
+Project-URL: Source, https://github.com/bebleo/pytest-smtpd
 Project-URL: Documentation, https://github.com/bebleo/pytest-smtpd#readme
 Project-URL: Issues, https://github.com/bebleo/pytest-smtpd/issues
-Project-URL: Source, https://github.com/bebleo/pytest-smtpd
-Author-email: James Warne <bebleo@yahoo.com>
-License-Expression: MIT
-License-File: LICENSE
-Keywords: email,pytest,smtp,testing
+Keywords: smtp,testing,pytest,email
 Classifier: Framework :: Pytest
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: <4,>=3.7
-Requires-Dist: pytest
-Requires-Dist: smtpdfix
-Provides-Extra: dev
-Requires-Dist: flake8; extra == 'dev'
-Requires-Dist: isort; extra == 'dev'
-Requires-Dist: mypy; extra == 'dev'
-Requires-Dist: tox; extra == 'dev'
 Description-Content-Type: text/markdown
+Provides-Extra: dev
+License-File: LICENSE
 
 # pytest-smtpd
 
 ⚠ **Not intended for use with production systems.** ⚠
 
 This fixture is intended to address cases where to test an application that sends an email, it needs to be intercepted for subsequent processing. For example, sending an email with a code for password reset or two-factor authentication. This fixture allows a test to trigger the email being sent, ensure that it's sent, and read the email.
 
 ## Installing
 
 To install using pip, first upgrade pip to the latest version to avoid any issues installing `cryptography`:
 
 ```bash
-python -m pip install --upgrade pip
-pip install pytest-smtpd
+$ python -m pip install --upgrade pip
+$ pip install pytest-smtpd
 ```
 
 Or, if you're using setuptools, it can be included in the `extras_require` argument of a `setup.py` file:
 
 ```python
 setup(
     ...
@@ -59,16 +54,16 @@
     },
 )
 ```
 
 and then installed with pip (-e assumes that you want your project to be editable):
 
 ```bash
-python -m pip install --upgrade pip
-pip install -e .[test]
+$ python -m pip install --upgrade pip
+$ pip install -e .[test]
 ```
 
 ## Using
 
 The `SMTPDFix` plugin, `smtpd`, automatically registers for use with pytest when you install smtpdfix. To use it simply add to your test method.
 
 ```python
@@ -148,50 +143,55 @@
 `login_password` | `SMTPD_LOGIN_PASSWORD` | `password`           | Password for default authentication.
 `use_ssl`        | `SMTPD_USE_SSL`        | `False`              | Whether the fixture should use fixed TLS/SSL for transactions. If using smtplib requires that `SMTP_SSL` be used instead of `SMTP`.
 `use_starttls`   | `SMTPD_USE_STARTTLS`   | `False`              | Whether the fixture should use StartTLS to encrypt the connections. If using `smtplib` requires that `SMTP.starttls()` is called before other commands are issued. Overrides `use_tls` as the preferred method for securing communications with the client.
 `enforce_auth`   | `SMTPD_ENFORCE_AUTH`   | `False`              | If set to true then the fixture refuses MAIL, RCPT, DATA commands until authentication is completed.
 `ssl_cert_path`  | `SMTPD_SSL_CERTS_PATH` | `./certs/`           | The path to the key and certificate in PEM format for encryption with SSL/TLS or StartTLS.
 `ssl_cert_files` | `SMTPD_SSL_CERT_FILE` and `SMTPD_SSL_KEY_FILE` | `("cert.pem", None)` | A tuple of the path for the certificate file and key file in PEM format.
 
+
+
 ## Alternatives
 
 Many libraries for sending email have built-in methods for testing and using these methods should generally be prefered over pytest-smtpd. Some known solutions:
 
 + **fastapi-mail**: has a `record_messsages()` method to intercept the mail. Instructions on how to suppress the sending of mail and implement it can be seen at [https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail](https://sabuhish.github.io/fastapi-mail/example/#unittests-using-fastapimail)
 + **flask-mail**: has a method to suppress sending and capture the email for testing purposes. [Instructions](https://pythonhosted.org/Flask-Mail/#unit-tests-and-suppressing-emails)
 
 ## Developing
 
 To develop and test smtpdfix you will need to install [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to run asynchronous tests, [isort](https://pycqa.github.io/isort/) to sort imports and [flake8](https://flake8.pycqa.org/en/latest/) to lint. To install in a virtual environment for development:
 
 ```bash
-python -m venv venv
-./venv/scripts/activate
-pip install -e .[dev]
+$ python -m venv venv
+$ ./venv/scripts/activate
+$ pip install -e .[dev]
 ```
 
 Code is tested using tox:
 
 ```bash
-tox
+$ tox
 ```
 
 Quick tests can be handled by running pytest directly:
 
 ```bash
-pytest
+$ pytest
 ```
 
 We include a [pre-commit](https://pre-commit.com/) configuration file to automate checks and clean up imports before pushing code. In order to install pre-commit git hooks:
 
 ```bash
-pip install pre-commit
-pre-commit install
+$ pip install pre-commit
+$ pre-commit install
 ```
 
 ## Known Issues
 
 + Firewalls may interfere with the operation of the smtp server.
-+ Authenticating with LOGIN and PLAIN mechanisms fails over TLS/SSL, but works with STARTTLS. [smtpdfix Issue #10](https://github.com/bebleo/smtpdfix/issues/10)
-+ Currently no support for termination through signals. [smtpdfix Issue #4](https://github.com/bebleo/smtpdfix/issues/4)
++ Authenticating with LOGIN and PLAIN mechanisms fails over TLS/SSL, but works with STARTTLS. [Issue #10](https://github.com/bebleo/smtpdfix/issues/10)
++ Currently no support for termination through signals. [Issue #4](https://github.com/bebleo/smtpdfix/issues/4)
++ If the fixture start exceeds the `ready_timeout` and aborts the host and port are not consistently released and subsequent uses may result in an error. [Issue #80](https://github.com/bebleo/smtpdfix/issues/80)
 
 Written with ☕ and ❤ in Montreal, QC
+
+
```

