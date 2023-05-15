# Comparing `tmp/file_validator-1.0.5.tar.gz` & `tmp/file_validator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-bu9hge84\file_validator-1.0.5.tar", last modified: Sun May 14 21:26:04 2023, max compression
+gzip compressed data, was "F:\Progamming Project\file-validator\dist\.tmp-vh05ocbu\file_validator-1.0.6.tar", last modified: Sun May 14 22:38:34 2023, max compression
```

## Comparing `file_validator-1.0.5.tar` & `file_validator-1.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.150998 file_validator-1.0.5/
--rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.5/AUTHORS.md
--rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.5/CONTRIBUTING.md
--rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.5/HISTORY.md
--rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     8148 2023-05-14 21:26:04.150998 file_validator-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     6289 2023-05-14 21:22:48.000000 file_validator-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.140994 file_validator-1.0.5/file_validator/
--rw-rw-rw-   0        0        0      136 2023-05-14 21:24:59.000000 file_validator-1.0.5/file_validator/__init__.py
--rw-rw-rw-   0        0        0     2765 2023-03-30 15:19:51.000000 file_validator-1.0.5/file_validator/constants.py
--rw-rw-rw-   0        0        0     3978 2023-03-30 15:19:51.000000 file_validator-1.0.5/file_validator/exceptions.py
--rw-rw-rw-   0        0        0      807 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/forms.py
--rw-rw-rw-   0        0        0    13267 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/models.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.008122 file_validator-1.0.5/file_validator/templates/
-drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.149992 file_validator-1.0.5/file_validator/templates/file_validator/
--rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.5/file_validator/templates/file_validator/file_input_widget.html
--rw-rw-rw-   0        0        0     4204 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/utils.py
--rw-rw-rw-   0        0        0    16723 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/validators.py
--rw-rw-rw-   0        0        0      214 2023-05-14 21:22:48.000000 file_validator-1.0.5/file_validator/widgets.py
-drwxrwxrwx   0        0        0        0 2023-05-14 21:26:04.148997 file_validator-1.0.5/file_validator.egg-info/
--rw-rw-rw-   0        0        0     8148 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-14 21:26:04.000000 file_validator-1.0.5/file_validator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      206 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-14 21:26:03.000000 file_validator-1.0.5/file_validator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      846 2023-05-14 21:26:04.152994 file_validator-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2774 2023-05-14 21:24:59.000000 file_validator-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.796372 file_validator-1.0.6/
+-rw-rw-rw-   0        0        0      115 2023-03-23 16:55:55.000000 file_validator-1.0.6/AUTHORS.md
+-rw-rw-rw-   0        0        0     2474 2023-03-23 16:55:55.000000 file_validator-1.0.6/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0      162 2023-03-23 16:55:55.000000 file_validator-1.0.6/HISTORY.md
+-rw-rw-rw-   0        0        0     1091 2023-03-23 16:55:55.000000 file_validator-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      310 2023-03-23 16:55:55.000000 file_validator-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     8148 2023-05-14 22:38:34.797362 file_validator-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     6289 2023-05-14 21:22:48.000000 file_validator-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.767360 file_validator-1.0.6/file_validator/
+-rw-rw-rw-   0        0        0      136 2023-05-14 22:19:37.000000 file_validator-1.0.6/file_validator/__init__.py
+-rw-rw-rw-   0        0        0     2765 2023-03-30 15:19:51.000000 file_validator-1.0.6/file_validator/constants.py
+-rw-rw-rw-   0        0        0     3978 2023-03-30 15:19:51.000000 file_validator-1.0.6/file_validator/exceptions.py
+-rw-rw-rw-   0        0        0      807 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/forms.py
+-rw-rw-rw-   0        0        0    12995 2023-05-14 22:32:47.000000 file_validator-1.0.6/file_validator/models.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.675359 file_validator-1.0.6/file_validator/templates/
+drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.782368 file_validator-1.0.6/file_validator/templates/file_validator/
+-rw-rw-rw-   0        0        0      127 2023-03-23 16:55:55.000000 file_validator-1.0.6/file_validator/templates/file_validator/file_input_widget.html
+-rw-rw-rw-   0        0        0     4204 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/utils.py
+-rw-rw-rw-   0        0        0    16723 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/validators.py
+-rw-rw-rw-   0        0        0      214 2023-05-14 21:22:48.000000 file_validator-1.0.6/file_validator/widgets.py
+drwxrwxrwx   0        0        0        0 2023-05-14 22:38:34.779378 file_validator-1.0.6/file_validator.egg-info/
+-rw-rw-rw-   0        0        0     8148 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      206 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-14 22:38:34.000000 file_validator-1.0.6/file_validator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      846 2023-05-14 22:38:34.798359 file_validator-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2774 2023-05-14 22:19:37.000000 file_validator-1.0.6/setup.py
```

### Comparing `file_validator-1.0.5/CONTRIBUTING.md` & `file_validator-1.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/LICENSE` & `file_validator-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/PKG-INFO` & `file_validator-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file_validator
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
```

### Comparing `file_validator-1.0.5/README.md` & `file_validator-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/file_validator/constants.py` & `file_validator-1.0.6/file_validator/constants.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/file_validator/exceptions.py` & `file_validator-1.0.6/file_validator/exceptions.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/file_validator/forms.py` & `file_validator-1.0.6/file_validator/forms.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/file_validator/models.py` & `file_validator-1.0.6/file_validator/validators.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,318 +1,412 @@
-"""In this module, there are file validators and field for Django.
-
-and it is made using external libraries such as (filetype, python-magic,
-pure_magic, mimetypes) and native libraries such as (mimetypes), and
-there is a method to perform validation operations using all three
-libraries It is called safe mode
-"""
-
-from django.core.exceptions import ValidationError
-from django.core.files.uploadedfile import TemporaryUploadedFile
-from django.db.models import FileField
-from django.utils.deconstruct import deconstructible
+"""In this module, there is a file validator for python, and it uses different
+libraries such as filetype, python-magic, mimetypes, and files are validated
+based on mimes, extensions, and magic numbers; The termcolor library is also
+used to color the error messages."""
+
+import os
+import platform
+from mimetypes import guess_type
+from pathlib import Path
+
+import magic
+import puremagic
+from dotenv import load_dotenv
+from filetype import guess
 from humanize import naturalsize
+from puremagic import PureError
 from termcolor import colored
 
 from file_validator.constants import (
-    ALL,
+    DJANGO,
+    ERROR_MESSAGE_FOR_EXTENSION_VALIDATION,
+    ERROR_MESSAGE_FOR_MIME_VALIDATION,
+    ERROR_MESSAGE_FOR_TYPE_VALIDATION,
     FILE_SIZE_IS_NOT_VALID,
     FILETYPE,
-    MAX_UPLOAD_SIZE_IS_EMPTY,
+    MIME_NOT_VALID,
     MIMETYPES,
+    OK,
     PURE_MAGIC,
     PYTHON_MAGIC,
+    SIZE,
+    SUPPORTED_TYPES,
+    TYPE_NOT_SUPPORTED,
 )
 from file_validator.exceptions import (
     error_message,
     FileValidationException,
     SizeValidationException,
+    TypeNotSupportedException,
 )
-from file_validator.utils import (
-    all_mimes_is_equal,
-    is_library_supported,
-    is_type_supported,
-    parameters_are_empty,
-    set_the_acceptable_mimes,
-    set_the_library,
-)
-from file_validator.validators import FileValidator
-
-
-class ValidatedFileField(FileField):
-    """
-    :return: If everything is OK, it will return None, otherwise it will
-        return a ValidationError.
-    """
-
-    def __init__(self, **kwargs):
-        """
-        :type acceptable_mimes: list
-        :param acceptable_mimes: The mimes you want the file to be checked
-            based on, example: image/png
-        :type acceptable_types: list
-        :param acceptable_types: The types you want the file to be checked based on, example: font,
-            audio, video, image, archive
-        :type max_upload_file_size: int, optional
-        :param max_upload_file_size: If you want the file size to be checked,
-            the file size must be in bytes,
-            example: file_size=1048576 (1MB), defaults to 0, optional
-        :type libraries: list, optional
-        :param libraries: The value of libraries should be a list of libraries
-            with which you want to perform the validation operation, example:
-            libraries=["filetype","python_magic"] defaults If you do not select
-            any library, it will perform the validation operation with django by
-            default, Supported libraries for validation operations:
-            python_magic, pure_magic, filetype, mimetypes, all, default
-        :raises ValueError: If the mime list is empty, raised a value error
-        :raises ValueError: If the library you entered is not supported,
-            raised a value error, Supported library: filetype, mimetypes,
-            pure_magic, python_magic
-        :raises ValidationError: if file not valid
-        """
-        self.max_upload_file_size: int = kwargs.get("max_upload_file_size")
-        self.acceptable_mimes: list = kwargs.get("acceptable_mimes")
-        self.acceptable_types: list = kwargs.get("acceptable_types")
-        libraries: list = kwargs.get("libraries")
-
-        parameters_are_empty(
-            acceptable_mimes=self.acceptable_mimes,
-            acceptable_types=self.acceptable_types,
-        )
-
-        all_mimes_is_equal(self.acceptable_mimes)
-
-        self.acceptable_mimes = set_the_acceptable_mimes(self.acceptable_mimes)
-
-        self.libraries = set_the_library(libraries)
-
-        is_type_supported(acceptable_types=self.acceptable_types)
-
-        super().__init__()
-
-    def deconstruct(self):
-        name, path, args, kwargs = super().deconstruct()
-        kwargs["acceptable_mimes"] = self.acceptable_mimes
-        kwargs["acceptable_types"] = self.acceptable_types
-        kwargs["libraries"] = self.libraries
-        kwargs["max_upload_file_size"] = self.max_upload_file_size
-        return name, path, args, kwargs
-
-    def clean(self, *args, **kwargs):
-        data = super().clean(*args, **kwargs)
-        current_file = data.file
-        try:
-            file_mime_guessed_by_django = current_file.content_type
-        except AttributeError:
-            file_mime_guessed_by_django = None
-        file_size = data.size
-        file_path = TemporaryUploadedFile.temporary_file_path(current_file)
-        try:
-            file_validator = FileValidator(
-                file_path=file_path,
-                libraries=self.libraries,
-                acceptable_mimes=self.acceptable_mimes,
-                acceptable_types=self.acceptable_types,
-                max_upload_file_size=self.max_upload_file_size,
-                file_mime_guessed_by_django=file_mime_guessed_by_django,
-            )
-            if self.acceptable_mimes is not None:
-                for library in self.libraries:
-                    if library == ALL:
-                        file_validator.validate()
-                    elif library == PYTHON_MAGIC:
-                        file_validator.python_magic()
-                    elif library == PURE_MAGIC:
-                        file_validator.pure_magic()
-                    elif library == MIMETYPES:
-                        file_validator.mimetypes()
-                    elif library == FILETYPE:
-                        file_validator.filetype()
-                    else:
-                        file_validator.django()
-            if self.acceptable_types is not None:
-                file_validator.validate_type()
-            if self.max_upload_file_size is not None:
-                file_validator.validate_size()
-        except (FileValidationException, SizeValidationException) as error:
-            raise ValidationError(
-                error_message(
-                    acceptable_mimes=self.acceptable_mimes,
-                    acceptable_types=self.acceptable_types,
-                    current_file_name=current_file.name,
-                    current_file_size=naturalsize(file_size),
-                    current_file_mime=file_mime_guessed_by_django,
-                    max_file_size=naturalsize(self.max_upload_file_size)
-                    if self.max_upload_file_size is not None
-                    else 0,
-                ),
-            ) from error
-        setattr(data, "validation_data", file_validator.result_of_validation)
-        return data
+from file_validator.utils import generate_information_about_file, guess_the_type
 
 
-@deconstructible
-class DjangoFileValidator:
-    """File validator for django."""
+class FileValidator:
+    """File validator."""
 
+    # pylint: disable=too-many-instance-attributes
+    # Eight are reasonable in this case.
     def __init__(
         self,
+        file_path: str = None,
         libraries: list = None,
         acceptable_mimes: list = None,
-        acceptable_types: list = None,
         max_upload_file_size: int = None,
+        **kwargs
     ):
-        """
-        :type acceptable_mimes: list
-        :param acceptable_mimes: The mimes you want the file to be checked
-            based on, example: image/png
-        :type acceptable_types: list
-        :param acceptable_types: The types you want the file to be checked based on, example: font,
-            audio, video, image, archive
-        :type max_upload_file_size: int, optional
-        :param max_upload_file_size: If you want the file size to be checked,
-            the file size must be in bytes,
-            example: file_size=1048576 (1MB), defaults to 0, optional
-        :type libraries: list, optional
-        :param libraries: The value of libraries should be a list of libraries
-            with which you want to perform the validation operation, example:
-            libraries=["filetype","python_magic"] defaults If you do not select
-            any library, it will perform the validation operation with django by
-            default, Supported libraries for validation operations:
-            python_magic, pure_magic, filetype, mimetypes, all, default
-        :raises ValueError: If the mime list is empty, raised a value error
-        :raises ValueError: If the library you entered is not supported,
-            raised a value error, Supported library: filetype, mimetypes,
-            pure_magic, python_magic
-        :return: If everything is OK, it will return None, otherwise it will
-            return a ValidationError.
-        """
-        self.max_upload_file_size = None
-        self.acceptable_types: list = acceptable_types
-        self.libraries = set_the_library(libraries)
-
-        if max_upload_file_size is not None:
-            self.max_upload_file_size = max_upload_file_size
-
-        parameters_are_empty(
-            acceptable_mimes=acceptable_mimes,
-            acceptable_types=acceptable_types,
-        )
-
-        all_mimes_is_equal(acceptable_mimes)
-
-        self.acceptable_mimes = set_the_acceptable_mimes(acceptable_mimes)
-
-        is_type_supported(acceptable_types=self.acceptable_types)
-
-    def __call__(self, value):
-        current_file = value.file
-        file_size = value.size
-        file_path = TemporaryUploadedFile.temporary_file_path(current_file)
-        try:
-            file_mime_guessed_by_django = current_file.content_type
-        except AttributeError:
-            file_mime_guessed_by_django = None
-        try:
-            file_validator = FileValidator(
-                file_path=file_path,
-                libraries=self.libraries,
-                acceptable_mimes=self.acceptable_mimes,
-                acceptable_types=self.acceptable_types,
-                max_upload_file_size=self.max_upload_file_size,
-                file_mime_guessed_by_django=file_mime_guessed_by_django,
+        self.file_mime_guessed_by_django = kwargs.get("file_mime_guessed_by_django")
+        self.acceptable_extensions = kwargs.get("acceptable_extensions")
+        self.result_of_validation = {}
+        self.max_upload_file_size = max_upload_file_size
+        self.acceptable_mimes = acceptable_mimes
+        self.acceptable_types = kwargs.get("acceptable_types")
+        self.file_path = file_path
+        self.libraries = libraries
+
+    def validate_extension(self):
+        """This method for validating the extension of file."""
+        current_file = Path(self.file_path)
+        file_extension = current_file.suffix
+        if file_extension not in self.acceptable_extensions:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_name=current_file.name,
+                        current_file_extension=file_extension,
+                        acceptable_extensions=self.acceptable_extensions,
+                        message=ERROR_MESSAGE_FOR_EXTENSION_VALIDATION,
+                    ),
+                    "red",
+                ),
             )
-            if self.acceptable_mimes is not None:
-                for library in self.libraries:
-                    is_library_supported(library)
-                    if library == ALL:
-                        file_validator.validate()
-                    elif library == PYTHON_MAGIC:
-                        file_validator.python_magic()
-                    elif library == PURE_MAGIC:
-                        file_validator.pure_magic()
-                    elif library == MIMETYPES:
-                        file_validator.mimetypes()
-                    elif library == FILETYPE:
-                        file_validator.filetype()
-                    else:
-                        file_validator.django()
-            if self.acceptable_types is not None:
-                file_validator.validate_type()
-            if self.max_upload_file_size is not None:
-                file_validator.validate_size()
-        except (FileValidationException, SizeValidationException) as error:
-            raise ValidationError(
+        result_of_validation = {
+            "file_extension": file_extension,
+        }
+        self.result_of_validation.update({SIZE: result_of_validation})
+        return result_of_validation
+
+    def validate_size(self):
+        """This method for validating the size of file."""
+        file_size = os.path.getsize(self.file_path)
+        current_file = Path(self.file_path)
+        if (
+            self.max_upload_file_size is not None
+            and file_size > self.max_upload_file_size
+        ):
+            raise SizeValidationException(
                 error_message(
-                    acceptable_mimes=self.acceptable_mimes,
-                    acceptable_types=self.acceptable_types,
-                    current_file_name=current_file.name,
                     current_file_size=naturalsize(file_size),
-                    current_file_mime=file_mime_guessed_by_django,
-                    max_file_size=naturalsize(self.max_upload_file_size)
-                    if self.max_upload_file_size is not None
-                    else 0,
+                    current_file_name=current_file.name,
+                    max_file_size=naturalsize(self.max_upload_file_size),
+                    message=FILE_SIZE_IS_NOT_VALID,
+                ),
+            )
+        result_of_validation = {
+            "file_size": naturalsize(file_size),
+            "max_upload_file_size": naturalsize(self.max_upload_file_size)
+            if self.max_upload_file_size is not None
+            else 0,
+        }
+        self.result_of_validation.update({SIZE: result_of_validation})
+        return result_of_validation
+
+    def validate_type(self):
+        """This method for validating the type of file."""
+        current_file = Path(self.file_path)
+        for acceptable_type in self.acceptable_types:
+            if acceptable_type.lower() not in SUPPORTED_TYPES:
+                raise TypeNotSupportedException(colored(TYPE_NOT_SUPPORTED, "red"))
+        file_type = guess_the_type(self.file_path)
+        if file_type not in self.acceptable_types:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_name=current_file.name,
+                        current_file_type=file_type,
+                        acceptable_mimes=self.acceptable_mimes,
+                        message=ERROR_MESSAGE_FOR_TYPE_VALIDATION,
+                    ),
+                    "red",
+                ),
+            )
+        current_file = Path(self.file_path)
+        result_of_validation = generate_information_about_file(
+            status=OK,
+            library=FILETYPE,
+            file_name=current_file.name,
+            file_type=file_type,
+            file_extension=current_file.suffix,
+        )
+        return result_of_validation
+
+    def validate_mime(self):
+        """This method for validating the mime of file."""
+        load_dotenv()
+        current_file = Path(self.file_path)
+        operating_system_name = platform.system()
+        path_magic_file = os.environ.get("path_magic_file")
+        if path_magic_file and operating_system_name == "Windows":
+            with open(self.file_path, "rb") as file:
+                magic.Magic(magic_file=path_magic_file)
+                guessed_mime_by_python_magic = magic.from_buffer(
+                    file.read(2048),
+                    mime=True,
+                )
+        else:
+            with open(self.file_path, "rb") as file:
+                guessed_mime_by_python_magic = magic.from_buffer(
+                    file.read(2048),
+                    mime=True,
+                )
+
+        with open(self.file_path, "rb") as file:
+            file_signatures = puremagic.magic_stream(file)
+            file_mimes_by_pure_magic = []
+            for file_signature in file_signatures:
+                file_mimes_by_pure_magic.append(file_signature.mime_type)
+        guessed_mime_by_pure_magic = file_mimes_by_pure_magic[0]
+        guessed_mime_by_mimetypes = guess_type(self.file_path)[0]
+        guessed_mime_by_filetype = guess(self.file_path).MIME
+        guessed_mimes = [
+            guessed_mime_by_python_magic,
+            guessed_mime_by_pure_magic,
+            guessed_mime_by_mimetypes,
+            guessed_mime_by_filetype,
+        ]
+        for file_mime in guessed_mimes:
+            if file_mime not in self.acceptable_mimes:
+                raise FileValidationException(
+                    colored(
+                        error_message(
+                            current_file_name=current_file.name,
+                            current_file_mime=file_mime,
+                            acceptable_mimes=self.acceptable_mimes,
+                            message=ERROR_MESSAGE_FOR_MIME_VALIDATION,
+                        ),
+                        "red",
+                    ),
+                )
+
+    def validate(self):
+        """This method for validating file based on mime using all
+        libraries."""
+        validation_data = {}
+
+        validation_data_filetype = self.filetype()
+        validation_data.update({FILETYPE: validation_data_filetype})
+
+        validation_data_mimetypes = self.mimetypes()
+        validation_data.update({MIMETYPES: validation_data_mimetypes})
+
+        validation_data_pure_magic = self.pure_magic()
+        validation_data.update({PURE_MAGIC: validation_data_pure_magic})
+
+        validation_data_python_magic = self.python_magic()
+        validation_data.update({PYTHON_MAGIC: validation_data_python_magic})
+
+        if self.file_mime_guessed_by_django is not None:
+            validation_data_django = self.django()
+            validation_data.update({DJANGO: validation_data_django})
+
+        return validation_data
+
+    def python_magic(self):
+        """This method for validating file based on mime using python-magic
+        library."""
+        load_dotenv()
+        operating_system_name = platform.system()
+        path_magic_file = os.environ.get("path_magic_file")
+        current_file = Path(self.file_path)
+        file_name = current_file.name
+        file_extension = current_file.suffix
+        if path_magic_file and operating_system_name == "Windows":
+            with open(self.file_path, "rb") as file:
+                magic.Magic(magic_file=path_magic_file)
+                file_mime = magic.from_buffer(file.read(2048), mime=True)
+        else:
+            with open(self.file_path, "rb") as file:
+                file_mime = magic.from_buffer(file.read(2048), mime=True)
+        file_type = file_mime.split("/")[0]
+        if file_mime not in self.acceptable_mimes:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_extension=current_file.suffix,
+                        current_file_name=current_file.name,
+                        current_file_mime=file_mime,
+                        current_file_type=file_type,
+                        acceptable_mimes=self.acceptable_mimes,
+                        acceptable_types=self.acceptable_types,
+                        acceptable_extensions=self.acceptable_extensions,
+                    ),
+                    "red",
                 ),
-            ) from error
+            )
 
-    def __eq__(self, other):
-        return (
-            isinstance(other, self.__class__)
-            and self.libraries == other.libraries
-            and self.acceptable_mimes == other.acceptable_mimes
-            and self.acceptable_types == other.acceptable_types
-            and self.max_upload_file_size == other.max_upload_file_size
+        result_of_validation = generate_information_about_file(
+            status=OK,
+            library=PYTHON_MAGIC,
+            file_name=file_name,
+            file_mime=file_mime,
+            file_type=file_type,
+            file_extension=file_extension,
         )
+        self.result_of_validation.update({PYTHON_MAGIC: result_of_validation})
+        return result_of_validation
 
-    def __hash__(self):
-        return hash(self.max_upload_file_size)
+    def pure_magic(self):
+        """This method for validating file based on mime using the pure-magic
+        library."""
+        current_file = Path(self.file_path)
+        try:
+            with open(self.file_path, "rb") as file:
+                file_signatures = puremagic.magic_stream(file)
+                file_mimes = []
+                for file_signature in file_signatures:
+                    file_mimes.append(file_signature.mime_type)
+        except PureError as error:
+            raise FileValidationException(colored(MIME_NOT_VALID, "red")) from error
+
+        file_mime = file_mimes[0]
+        file_type = file_mime.split("/")[0]
+        if file_mime not in self.acceptable_mimes:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_extension=current_file.suffix,
+                        current_file_name=current_file.name,
+                        current_file_mime=file_mime,
+                        current_file_type=file_type,
+                        acceptable_mimes=self.acceptable_mimes,
+                        acceptable_types=self.acceptable_types,
+                        acceptable_extensions=self.acceptable_extensions,
+                    ),
+                    "red",
+                ),
+            )
 
+        result_of_validation = generate_information_about_file(
+            status=OK,
+            library=PURE_MAGIC,
+            file_name=current_file.name,
+            file_mime=file_mime,
+            file_type=file_type,
+            file_extension=current_file.suffix,
+        )
+        self.result_of_validation.update({PURE_MAGIC: result_of_validation})
+        return result_of_validation
 
-@deconstructible
-class FileSizeValidator:
-    """Size validator for django."""
+    def mimetypes(self):
+        """This method for validating file based on mime using the mimetypes
+        library."""
+        current_file = Path(self.file_path)
+        file_mime = guess_type(self.file_path)[0]
+        if file_mime is None:
+            raise FileValidationException(colored(MIME_NOT_VALID, "red"))
+        file_type = file_mime.split("/")[0]
+
+        if file_mime not in self.acceptable_mimes:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_extension=current_file.suffix,
+                        current_file_name=current_file.name,
+                        current_file_mime=file_mime,
+                        current_file_type=file_type,
+                        acceptable_mimes=self.acceptable_mimes,
+                        acceptable_types=self.acceptable_types,
+                        acceptable_extensions=self.acceptable_extensions,
+                    ),
+                    "red",
+                ),
+            )
 
-    def __init__(
-        self,
-        max_upload_file_size: int = None,
-    ):
-        """
-        :type max_upload_file_size: int
-        :param max_upload_file_size: If you want the file size to be checked,
-            the file size must be in bytes,
-            example: file_size=1048576 (1MB), defaults to 0, optional
-        :return: If everything is OK, it will return None, otherwise it will
-            return a ValidationError.
-        """
-        if max_upload_file_size is None:
-            raise SizeValidationException(colored(MAX_UPLOAD_SIZE_IS_EMPTY, "red"))
+        result_of_validation = generate_information_about_file(
+            status=OK,
+            library=MIMETYPES,
+            file_name=current_file.name,
+            file_mime=file_mime,
+            file_type=file_type,
+            file_extension=current_file.suffix,
+        )
+        self.result_of_validation.update({MIMETYPES: result_of_validation})
+        return result_of_validation
 
-        self.max_upload_file_size = max_upload_file_size
+    def filetype(self):
+        """This method for validating file based on mime using the filetype
+        library."""
+        current_file = Path(self.file_path)
 
-    def __call__(self, value):
-        current_file = value.file
-        file_size = value.size
-        file_path = TemporaryUploadedFile.temporary_file_path(current_file)
         try:
-            file_validator = FileValidator(
-                file_path=file_path,
-                max_upload_file_size=self.max_upload_file_size,
-            )
-            file_validator.validate_size()
-        except SizeValidationException as error:
-            raise ValidationError(
-                error_message(
-                    current_file_name=current_file.name,
-                    current_file_size=naturalsize(file_size),
-                    max_file_size=naturalsize(self.max_upload_file_size),
-                    message=FILE_SIZE_IS_NOT_VALID,
+            file_mime = guess(self.file_path).MIME
+            file_type = file_mime.split("/")[0]
+        except AttributeError as error:
+            raise FileValidationException(colored(MIME_NOT_VALID, "red")) from error
+
+        if file_mime not in self.acceptable_mimes:
+            raise FileValidationException(
+                colored(
+                    error_message(
+                        current_file_extension=current_file.suffix,
+                        current_file_name=current_file.name,
+                        current_file_mime=file_mime,
+                        current_file_type=file_type,
+                        acceptable_mimes=self.acceptable_mimes,
+                        acceptable_types=self.acceptable_types,
+                        acceptable_extensions=self.acceptable_extensions,
+                    ),
+                    "red",
                 ),
-            ) from error
+            )
 
-    def __eq__(self, other):
-        return (
-            isinstance(other, self.__class__)
-            and self.max_upload_file_size == other.max_upload_file_size
+        result_of_validation = generate_information_about_file(
+            status=OK,
+            library=FILETYPE,
+            file_name=current_file.name,
+            file_mime=file_mime,
+            file_type=file_type,
+            file_extension=current_file.suffix,
         )
+        self.result_of_validation.update({FILETYPE: result_of_validation})
+        return result_of_validation
 
-    def __hash__(self):
-        return hash(self.max_upload_file_size)
+    def django(self):
+        """This method for validating file based on mime using data from
+        django."""
+        try:
+            current_file = Path(self.file_path)
+            file_type = self.file_mime_guessed_by_django.split("/")[0]
+            if self.file_mime_guessed_by_django not in self.acceptable_mimes:
+                raise FileValidationException(
+                    colored(
+                        error_message(
+                            current_file_extension=current_file.suffix,
+                            current_file_name=current_file.name,
+                            current_file_mime=self.file_mime_guessed_by_django,
+                            current_file_type=file_type,
+                            acceptable_mimes=self.acceptable_mimes,
+                            acceptable_types=self.acceptable_types,
+                            acceptable_extensions=self.acceptable_extensions,
+                        ),
+                        "red",
+                    ),
+                )
+            result_of_validation = generate_information_about_file(
+                status=OK,
+                file_name=current_file.name,
+                file_mime=self.file_mime_guessed_by_django,
+                file_type=file_type,
+                file_extension=current_file.suffix,
+            )
+            self.result_of_validation.update({DJANGO: result_of_validation})
+            return result_of_validation
+        except AttributeError:
+            result_of_validation = generate_information_about_file(
+                status="Fail",
+                file_name=current_file.name,
+                file_mime="NOT_FOUND",
+                file_type="NOT_FOUND",
+                file_extension=current_file.suffix,
+            )
+            self.result_of_validation.update({DJANGO: result_of_validation})
+            return result_of_validation
```

### Comparing `file_validator-1.0.5/file_validator/utils.py` & `file_validator-1.0.6/file_validator/utils.py`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/file_validator.egg-info/PKG-INFO` & `file_validator-1.0.6/file_validator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-validator
-Version: 1.0.5
+Version: 1.0.6
 Summary: Python validation library to validate files using type, mime, extension, magic numbers and size ✅
 Home-page: https://github.com/file-validator/file-validator
 Author: Reza Shakeri
 Author-email: rzashakeri@outlook.com
 License: MIT license
 Project-URL: Documentation, https://file-validator.github.io/
 Project-URL: Homepage, https://github.com/file-validator
```

### Comparing `file_validator-1.0.5/file_validator.egg-info/SOURCES.txt` & `file_validator-1.0.6/file_validator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file_validator-1.0.5/setup.cfg` & `file_validator-1.0.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.0.5
+current_version = 1.0.6
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `file_validator-1.0.5/setup.py` & `file_validator-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         "django",
     ],
     name="file_validator",
     packages=find_packages(include=["file_validator", "file_validator.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/file-validator/file-validator",
-    version="1.0.5",
+    version="1.0.6",
     zip_safe=False,
     project_urls={
         "Documentation": "https://file-validator.github.io/",
         "Homepage": "https://github.com/file-validator",
         "Issue tracker": "https://github.com/file-validator/file-validator/issues",
         "Release notes": "https://github.com/file-validator/file-validator/releases",
         "Source": "https://github.com/file-validator/file-validator",
```

