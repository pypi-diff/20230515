# Comparing `tmp/justpass-me-django-0.0.1.tar.gz` & `tmp/justpass-me-django-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justpass-me-django-0.0.1.tar", last modified: Mon May 15 15:48:48 2023, max compression
+gzip compressed data, was "justpass-me-django-0.1.0.tar", last modified: Mon May 15 15:51:50 2023, max compression
```

## Comparing `justpass-me-django-0.0.1.tar` & `justpass-me-django-0.1.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:48:48.988693 justpass-me-django-0.0.1/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 15:42:36.000000 justpass-me-django-0.0.1/LICENSE
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4737 2023-05-15 15:48:48.988693 justpass-me-django-0.0.1/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3378 2023-05-15 15:44:07.000000 justpass-me-django-0.0.1/README.md
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:48:48.988693 justpass-me-django-0.0.1/justpass_me_django.egg-info/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4737 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/PKG-INFO
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      445 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/SOURCES.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/dependency_links.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/not-zip-safe
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       39 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/requires.txt
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-15 15:48:48.000000 justpass-me-django-0.0.1/justpass_me_django.egg-info/top_level.txt
-drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:48:48.988693 justpass-me-django-0.0.1/justpassme/
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6696 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/OIDC_CLIENT.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/__init__.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/admin.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 15:13:26.000000 justpass-me-django-0.0.1/justpassme/apps.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1013 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/helpers.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      557 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/urls.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 15:07:58.000000 justpass-me-django-0.0.1/justpassme/utils.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      945 2023-05-15 15:13:03.000000 justpass-me-django-0.0.1/justpassme/views.py
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-15 15:48:48.988693 justpass-me-django-0.0.1/setup.cfg
--rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1772 2023-05-15 15:22:22.000000 justpass-me-django-0.0.1/setup.py
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:51:50.720700 justpass-me-django-0.1.0/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1067 2023-05-15 15:42:36.000000 justpass-me-django-0.1.0/LICENSE
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4737 2023-05-15 15:51:50.720700 justpass-me-django-0.1.0/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     3378 2023-05-15 15:50:10.000000 justpass-me-django-0.1.0/README.md
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:51:50.720700 justpass-me-django-0.1.0/justpass_me_django.egg-info/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     4737 2023-05-15 15:51:50.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/PKG-INFO
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      445 2023-05-15 15:51:50.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/SOURCES.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:51:50.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/dependency_links.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        1 2023-05-15 15:48:48.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/not-zip-safe
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       39 2023-05-15 15:51:50.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/requires.txt
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       11 2023-05-15 15:51:50.000000 justpass-me-django-0.1.0/justpass_me_django.egg-info/top_level.txt
+drwxrwxr-x   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:51:50.720700 justpass-me-django-0.1.0/justpassme/
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     6696 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/OIDC_CLIENT.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)        0 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/__init__.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       63 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/admin.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      152 2023-05-15 15:13:26.000000 justpass-me-django-0.1.0/justpassme/apps.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1013 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/helpers.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      557 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/urls.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      168 2023-05-15 15:07:58.000000 justpass-me-django-0.1.0/justpassme/utils.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)      945 2023-05-15 15:13:03.000000 justpass-me-django-0.1.0/justpassme/views.py
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)       38 2023-05-15 15:51:50.720700 justpass-me-django-0.1.0/setup.cfg
+-rw-rw-r--   0 mohamed   (1000) mohamed   (1000)     1772 2023-05-15 15:51:49.000000 justpass-me-django-0.1.0/setup.py
```

### Comparing `justpass-me-django-0.0.1/LICENSE` & `justpass-me-django-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `justpass-me-django-0.0.1/PKG-INFO` & `justpass-me-django-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 0.0.1
+Version: 0.1.0
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
 Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
@@ -88,33 +88,33 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-4. Write a function to start registration and add it to your `urls.py`
+3. Write a function to start registration and add it to your `urls.py`
 
    ```python
    def start_reg(request):
        from justpassme.helpers import start_reg
        return start_reg(request)
    ```
 
-5. Write a function to start login and add it to your `urls.py`
+4. Write a function to start login and add it to your `urls.py`
 
    **Note:** The function expects the user username to be in `request.session["base_username"]`
 
    ```python
    def start_login(request):
        from justpassme.helpers import start_oidc_sign
        return start_oidc_sign(request)
    ```
 
-6. Write 4 functions that handle the success and failure of registration and login. 
+5. Write 4 functions that handle the success and failure of registration and login. 
 You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
```

### Comparing `justpass-me-django-0.0.1/README.md` & `justpass-me-django-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -53,33 +53,33 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-4. Write a function to start registration and add it to your `urls.py`
+3. Write a function to start registration and add it to your `urls.py`
 
    ```python
    def start_reg(request):
        from justpassme.helpers import start_reg
        return start_reg(request)
    ```
 
-5. Write a function to start login and add it to your `urls.py`
+4. Write a function to start login and add it to your `urls.py`
 
    **Note:** The function expects the user username to be in `request.session["base_username"]`
 
    ```python
    def start_login(request):
        from justpassme.helpers import start_oidc_sign
        return start_oidc_sign(request)
    ```
 
-6. Write 4 functions that handle the success and failure of registration and login. 
+5. Write 4 functions that handle the success and failure of registration and login. 
 You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
```

### Comparing `justpass-me-django-0.0.1/justpass_me_django.egg-info/PKG-INFO` & `justpass-me-django-0.1.0/justpass_me_django.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justpass-me-django
-Version: 0.0.1
+Version: 0.1.0
 Summary: Django Integration with JustPass.me
 Home-page: https://github.com/justpass-me/justpass-me-django
 Download-URL: https://github.com/justpass-me/justpass-me-django
 Author: JustPassMe
 Author-email: sameh@justpass.me
 License: MIT
 Classifier: Development Status :: 4 - Beta
@@ -88,33 +88,33 @@
 Break your login function, Usually your login function will check for username and password, log the user in if the username and password are correct and create the user session, to support justpass.me, this has to change
    
    * authenticate the user
    * if username and password are correct , check if the user has mfa or not
        * if user has mfa then redirect to justpass.me
        * if user doesn't have mfa then call your function to create the user session
 
-4. Write a function to start registration and add it to your `urls.py`
+3. Write a function to start registration and add it to your `urls.py`
 
    ```python
    def start_reg(request):
        from justpassme.helpers import start_reg
        return start_reg(request)
    ```
 
-5. Write a function to start login and add it to your `urls.py`
+4. Write a function to start login and add it to your `urls.py`
 
    **Note:** The function expects the user username to be in `request.session["base_username"]`
 
    ```python
    def start_login(request):
        from justpassme.helpers import start_oidc_sign
        return start_oidc_sign(request)
    ```
 
-6. Write 4 functions that handle the success and failure of registration and login. 
+5. Write 4 functions that handle the success and failure of registration and login. 
 You can use the four functions below as a reference.
 
    ```python
    def auth_success(request):
       return redirect('home')
          
    def auth_failure(request):
```

### Comparing `justpass-me-django-0.0.1/justpassme/OIDC_CLIENT.py` & `justpass-me-django-0.1.0/justpassme/OIDC_CLIENT.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-0.0.1/justpassme/helpers.py` & `justpass-me-django-0.1.0/justpassme/helpers.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-0.0.1/justpassme/urls.py` & `justpass-me-django-0.1.0/justpassme/urls.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-0.0.1/justpassme/views.py` & `justpass-me-django-0.1.0/justpassme/views.py`

 * *Files identical despite different names*

### Comparing `justpass-me-django-0.0.1/setup.py` & `justpass-me-django-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name='justpass-me-django',
-    version='0.0.1',
+    version='0.1.0',
     description='Django Integration with JustPass.me',
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author='JustPassMe',
     author_email = 'sameh@justpass.me',
     url = 'https://github.com/justpass-me/justpass-me-django',
     download_url='https://github.com/justpass-me/justpass-me-django',
```

