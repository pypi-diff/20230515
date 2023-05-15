# Comparing `tmp/sosin-1.1.4.tar.gz` & `tmp/sosin-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosin-1.1.4.tar", last modified: Sun May 14 03:15:01 2023, max compression
+gzip compressed data, was "sosin-1.1.5.tar", last modified: Mon May 15 08:04:26 2023, max compression
```

## Comparing `sosin-1.1.4.tar` & `sosin-1.1.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.485884 sosin-1.1.4/
--rw-rw-rw-   0        0        0     1083 2023-04-17 11:46:46.000000 sosin-1.1.4/LICENSE
--rw-rw-rw-   0        0        0     1268 2023-05-14 03:15:01.483875 sosin-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      863 2023-04-17 11:46:46.000000 sosin-1.1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-14 03:15:01.485884 sosin-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-05-14 01:57:48.000000 sosin-1.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.397470 sosin-1.1.4/sosin/
--rw-rw-rw-   0        0        0      295 2023-05-14 01:57:48.000000 sosin-1.1.4/sosin/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.453484 sosin-1.1.4/sosin/databases/
--rw-rw-rw-   0        0        0     4934 2023-04-24 10:38:48.000000 sosin-1.1.4/sosin/databases/fs.py
--rw-rw-rw-   0        0        0     9763 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/databases/rdb.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.456697 sosin-1.1.4/sosin/rpa/
--rw-rw-rw-   0        0        0    10926 2023-05-14 01:57:48.000000 sosin-1.1.4/sosin/rpa/email_mgr.py
--rw-rw-rw-   0        0        0     3698 2023-05-10 06:56:55.000000 sosin-1.1.4/sosin/rpa/sms_mgr.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.464838 sosin-1.1.4/sosin/utils/
--rw-rw-rw-   0        0        0     1797 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/utils/currency.py
--rw-rw-rw-   0        0        0      304 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/log.py
--rw-rw-rw-   0        0        0      527 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/progress.py
--rw-rw-rw-   0        0        0      385 2023-04-17 11:46:46.000000 sosin-1.1.4/sosin/utils/secret.py
--rw-rw-rw-   0        0        0      885 2023-05-10 06:56:55.000000 sosin-1.1.4/sosin/utils/zip.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.482365 sosin-1.1.4/sosin/web/
--rw-rw-rw-   0        0        0     1055 2023-04-18 14:49:45.000000 sosin-1.1.4/sosin/web/content.py
--rw-rw-rw-   0        0        0     5506 2023-05-14 01:57:26.000000 sosin-1.1.4/sosin/web/session.py
--rw-rw-rw-   0        0        0     1051 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/web/translate.py
--rw-rw-rw-   0        0        0     4394 2023-05-14 01:57:45.000000 sosin-1.1.4/sosin/web/virtual.py
-drwxrwxrwx   0        0        0        0 2023-05-14 03:15:01.450315 sosin-1.1.4/sosin.egg-info/
--rw-rw-rw-   0        0        0     1268 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      471 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-14 03:15:01.000000 sosin-1.1.4/sosin.egg-info/top_level.txt
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.463348 sosin-1.1.5/
+-rwx------   0 sosin      (501) staff       (20)     1083 2023-04-17 11:46:46.000000 sosin-1.1.5/LICENSE
+-rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-15 08:04:26.463136 sosin-1.1.5/PKG-INFO
+-rwx------   0 sosin      (501) staff       (20)      863 2023-04-17 11:46:46.000000 sosin-1.1.5/README.md
+-rw-r--r--   0 sosin      (501) staff       (20)       38 2023-05-15 08:04:26.463416 sosin-1.1.5/setup.cfg
+-rwx------   0 sosin      (501) staff       (20)      984 2023-05-15 08:02:34.000000 sosin-1.1.5/setup.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.458250 sosin-1.1.5/sosin/
+-rwx------   0 sosin      (501) staff       (20)      302 2023-05-15 08:02:38.000000 sosin-1.1.5/sosin/__init__.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459341 sosin-1.1.5/sosin/databases/
+-rwx------   0 sosin      (501) staff       (20)     4934 2023-04-24 10:38:48.000000 sosin-1.1.5/sosin/databases/fs.py
+-rwx------   0 sosin      (501) staff       (20)     9763 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/databases/rdb.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459745 sosin-1.1.5/sosin/rpa/
+-rwx------   0 sosin      (501) staff       (20)    11055 2023-05-15 08:02:12.000000 sosin-1.1.5/sosin/rpa/email_mgr.py
+-rwx------   0 sosin      (501) staff       (20)     3698 2023-05-10 06:56:55.000000 sosin-1.1.5/sosin/rpa/sms_mgr.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.460739 sosin-1.1.5/sosin/utils/
+-rwx------   0 sosin      (501) staff       (20)     1797 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/utils/currency.py
+-rwx------   0 sosin      (501) staff       (20)      304 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/log.py
+-rwx------   0 sosin      (501) staff       (20)      527 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/progress.py
+-rwx------   0 sosin      (501) staff       (20)      385 2023-04-17 11:46:46.000000 sosin-1.1.5/sosin/utils/secret.py
+-rwx------   0 sosin      (501) staff       (20)      885 2023-05-10 06:56:55.000000 sosin-1.1.5/sosin/utils/zip.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.462799 sosin-1.1.5/sosin/web/
+-rwx------   0 sosin      (501) staff       (20)     1055 2023-04-18 14:49:45.000000 sosin-1.1.5/sosin/web/content.py
+-rwx------   0 sosin      (501) staff       (20)     5506 2023-05-14 01:57:26.000000 sosin-1.1.5/sosin/web/session.py
+-rwx------   0 sosin      (501) staff       (20)     1051 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/web/translate.py
+-rwx------   0 sosin      (501) staff       (20)     4394 2023-05-14 01:57:45.000000 sosin-1.1.5/sosin/web/virtual.py
+drwxr-xr-x   0 sosin      (501) staff       (20)        0 2023-05-15 08:04:26.459011 sosin-1.1.5/sosin.egg-info/
+-rw-r--r--   0 sosin      (501) staff       (20)     1250 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/PKG-INFO
+-rw-r--r--   0 sosin      (501) staff       (20)      471 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/SOURCES.txt
+-rw-r--r--   0 sosin      (501) staff       (20)        1 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/dependency_links.txt
+-rw-r--r--   0 sosin      (501) staff       (20)       27 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/requires.txt
+-rw-r--r--   0 sosin      (501) staff       (20)        6 2023-05-15 08:04:26.000000 sosin-1.1.5/sosin.egg-info/top_level.txt
```

### Comparing `sosin-1.1.4/LICENSE` & `sosin-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/PKG-INFO` & `sosin-1.1.5/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.4
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.5
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
+
+
```

### Comparing `sosin-1.1.4/README.md` & `sosin-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/setup.py` & `sosin-1.1.5/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name                                = "sosin",
-    version                             = "1.1.4",
+    version                             = "1.1.5",
     license                             = 'MIT',
     author                              = "Jason Choi",
     author_email                        = "svstar94@gmail.com",
     description                         = "Python utils for general works",
     long_description                    = open('README.md').read(),
     url                                 = "https://github.com/devsosin/sosin",
     install_requires                    = ['requests', 'requests-toolbelt'],
```

### Comparing `sosin-1.1.4/sosin/databases/fs.py` & `sosin-1.1.5/sosin/databases/fs.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/databases/rdb.py` & `sosin-1.1.5/sosin/databases/rdb.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/rpa/email_mgr.py` & `sosin-1.1.5/sosin/rpa/email_mgr.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,15 +206,15 @@
         '''
         메일을 발송하는 함수입니다.
 
         **필수값**
         from_user: 보내는 사람의 이메일 주소
         to_users: 받는 사람의 이메일 주소들 (list)
         subject: 메일 제목
-        content: 메일 내용
+        content: 메일 내용 (list)
 
         **선택**
         attachments: 첨부 파일들 (파일경로 리스트)
         cc_targets: 참조 이메일 주소들 (list)
         '''
 
         try:
@@ -240,14 +240,16 @@
 
             msg['From'] = from_user
             msg['To'] = ','.join(set(to_users))
             if cc_targets:
                 msg['CC'] = ','.join(cc_targets)
             msg['Subject'] = subject
 
+            # if type contents is string -> 552 5.2.3 error
+            if type(contents) == str: contents = [contents]
             for content in contents:
                 # don't care content is str or tuple
                 msg.attach(MIMEText(content))
 
             self.protocol.sendmail(from_user, set(to_users+cc_targets), msg.as_string())
             return True
```

### Comparing `sosin-1.1.4/sosin/rpa/sms_mgr.py` & `sosin-1.1.5/sosin/rpa/sms_mgr.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/utils/currency.py` & `sosin-1.1.5/sosin/utils/currency.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/utils/progress.py` & `sosin-1.1.5/sosin/utils/progress.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/utils/zip.py` & `sosin-1.1.5/sosin/utils/zip.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/web/content.py` & `sosin-1.1.5/sosin/web/content.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/web/session.py` & `sosin-1.1.5/sosin/web/session.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/web/translate.py` & `sosin-1.1.5/sosin/web/translate.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin/web/virtual.py` & `sosin-1.1.5/sosin/web/virtual.py`

 * *Files identical despite different names*

### Comparing `sosin-1.1.4/sosin.egg-info/PKG-INFO` & `sosin-1.1.5/sosin.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-Metadata-Version: 2.1
-Name: sosin
-Version: 1.1.4
-Summary: Python utils for general works
-Home-page: https://github.com/devsosin/sosin
-Author: Jason Choi
-Author-email: svstar94@gmail.com
-License: MIT
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-License-File: LICENSE
-
-# sosin: easy to use Python utils for general works
-
-[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
-[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
-[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
-
-----
-
-## Dependencies
-![Python](https://img.shields.io/badge/python->=3.9-blue)
-![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
-![Chrome](https://img.shields.io/badge/Chrome--red)
-
-## Installation
-```bash
-# PyPI
-pip install sosin
-```
-
-## License
-[MIT](LICENSE)
-
-## Getting Help
-For usage questions, Please contact [me](https://github.com/devsosin)
+Metadata-Version: 2.1
+Name: sosin
+Version: 1.1.5
+Summary: Python utils for general works
+Home-page: https://github.com/devsosin/sosin
+Author: Jason Choi
+Author-email: svstar94@gmail.com
+License: MIT
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+License-File: LICENSE
+
+# sosin: easy to use Python utils for general works
+
+[![PyPI Latest Release](https://img.shields.io/pypi/v/sosin.svg)](https://pypi.org/project/sosin/)
+[![License](https://img.shields.io/pypi/l/sosin.svg)](https://github.com/devsosin/sosin/blob/main/LICENSE)
+[![Downloads](https://static.pepy.tech/personalized-badge/sosin?period=month&units=international_system&left_color=black&right_color=orange&left_text=PyPI%20downloads%20per%20month)](https://pepy.tech/project/sosin)
+
+----
+
+## Dependencies
+![Python](https://img.shields.io/badge/python->=3.9-blue)
+![MariaDB](https://img.shields.io/badge/MariaDB->=10.3-yellow)
+![Chrome](https://img.shields.io/badge/Chrome--red)
+
+## Installation
+```bash
+# PyPI
+pip install sosin
+```
+
+## License
+[MIT](LICENSE)
+
+## Getting Help
+For usage questions, Please contact [me](https://github.com/devsosin)
+
+
```

