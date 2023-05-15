# Comparing `tmp/section-to-course-0.2.0.tar.gz` & `tmp/section-to-course-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "section-to-course-0.2.0.tar", last modified: Wed May 10 17:49:03 2023, max compression
+gzip compressed data, was "section-to-course-0.3.0.tar", last modified: Mon May 15 15:00:23 2023, max compression
```

## Comparing `section-to-course-0.2.0.tar` & `section-to-course-0.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-10 17:48:59.000000 section-to-course-0.2.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-10 17:48:59.000000 section-to-course-0.2.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-10 17:48:59.000000 section-to-course-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-05-10 17:49:03.667816 section-to-course-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-05-10 17:48:59.000000 section-to-course-0.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.663816 section-to-course-0.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-10 17:48:59.000000 section-to-course-0.2.0/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-10 17:48:59.000000 section-to-course-0.2.0/requirements/constraints.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/
--rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14125 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      398 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/api/views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     4763 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/management/commands/section_to_course.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/settings/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/settings/common.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.663816 section-to-course-0.2.0/section_to_course/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.663816 section-to-course-0.2.0/section_to_course/static/section_to_course/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course/static/section_to_course/js/
--rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/static/section_to_course/js/admin-tools.js
--rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-10 17:48:59.000000 section-to-course-0.2.0/section_to_course/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-10 17:49:03.667816 section-to-course-0.2.0/section_to_course.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5840 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-10 17:49:03.000000 section-to-course-0.2.0/section_to_course.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-10 17:49:03.667816 section-to-course-0.2.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (122)     5320 2023-05-10 17:48:59.000000 section-to-course-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-15 15:00:16.000000 section-to-course-0.3.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    35139 2023-05-15 15:00:16.000000 section-to-course-0.3.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      212 2023-05-15 15:00:16.000000 section-to-course-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-05-15 15:00:23.911131 section-to-course-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6207 2023-05-15 15:00:16.000000 section-to-course-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-15 15:00:16.000000 section-to-course-0.3.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)      562 2023-05-15 15:00:16.000000 section-to-course-0.3.0/requirements/constraints.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14154 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      398 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2944 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1326 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4820 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2066 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/management/commands/section_to_course.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1612 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1354 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/settings/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      275 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/settings/common.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.903130 section-to-course-0.3.0/section_to_course/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.903130 section-to-course-0.3.0/section_to_course/static/section_to_course/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.911131 section-to-course-0.3.0/section_to_course/static/section_to_course/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     2526 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/static/section_to_course/js/admin-tools.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2692 2023-05-15 15:00:16.000000 section-to-course-0.3.0/section_to_course/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 15:00:23.907130 section-to-course-0.3.0/section_to_course.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     7803 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1039 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      119 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-15 15:00:23.000000 section-to-course-0.3.0/section_to_course.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      176 2023-05-15 15:00:23.911131 section-to-course-0.3.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5320 2023-05-15 15:00:16.000000 section-to-course-0.3.0/setup.py
```

### Comparing `section-to-course-0.2.0/CHANGELOG.rst` & `section-to-course-0.3.0/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -12,14 +12,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-12
+********************
+
+Changed
+=======
+
+* New section-based courses are self-paced.
+
 [0.2.0] - 2023-05-10
 ********************
 
 Added
 =====
 
 * Admin views for creating new section-based courses.
```

### Comparing `section-to-course-0.2.0/LICENSE.txt` & `section-to-course-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/PKG-INFO` & `section-to-course-0.3.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: section-to-course
-Version: 0.2.0
+Version: 0.3.0
 Summary: Factors sections from Open edX courses into their own new course.
 Home-page: https://github.com/open-craft/section-to-course
 Author: OpenCraft
 Author-email: help@opencraft.com
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -67,22 +67,51 @@
 
 .. code-block:: bash
 
     make dev.shell.studio
     cd /edx/src/section-to-course
     pip install -e .
 
+Configuration (optional)
+************************
+
+New courses are self-paced. If you want to set relative deadlines in them, follow the next steps:
+
+#. Add the following `Waffle Flags`_ (with ``Everyone: Yes``) in Django admin:
+
+    #. `studio.custom_relative_dates`_
+    #. `course_experience.relative_dates`_
+    #. `course_experience.relative_dates_disable_reset`_
+#. Go to `Django admin -> Course_Date_Signals -> Self paced relative dates`_ configs and add a config with ``Enabled: Yes``.
+
+.. _Waffle Flags: http://localhost:18000/admin/waffle/flag/
+.. _studio.custom_relative_dates: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-studio.custom_relative_dates
+.. _course_experience.relative_dates: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-course_experience.relative_dates
+.. _course_experience.relative_dates_disable_reset: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-course_experience.relative_dates_disable_reset
+.. _Django admin -> Course_Date_Signals -> Self paced relative dates: http://localhost:18000/admin/course_date_signals/selfpacedrelativedatesconfig/
+
 
 Usage
 *****
 
 Once installed, the plugin should automatically register itself within Django. Be sure to run database migrations.
 
 The admin views are in the Django admin, under the "Section to Course" section. From there, you can create a new section to course link, which will create a new course with the same content as the section you selected. You can also view the list of existing section to course links, refresh them, and delete them.
 
+**Note:** The start date of a newly created course is in the future, so you will likely want to modify it in the "Schedule & Details" section in Studio.
+
+Relative due dates (optional)
+=============================
+
+If you want to configure relative deadlines in your course, follow these steps:
+
+#. Mark a subsection in the newly created course as graded (otherwise, deadlines will be enforced but learners will not see these dates in the LMS).
+#. Enter the number of weeks in the subsection's "Due in" field.
+#. You may also want to adjust the new course's grading policy to change the weight of the section.
+
 Refreshing a Course
 ===================
 
 There are two ways to refresh a course:
 
 1. Use the admin action from the changelist view. This will allow you to refresh several courses at once.
 2. Use the refresh button on the detail view for a single course, shown here:
@@ -152,14 +181,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-12
+********************
+
+Changed
+=======
+
+* New section-based courses are self-paced.
+
 [0.2.0] - 2023-05-10
 ********************
 
 Added
 =====
 
 * Admin views for creating new section-based courses.
```

### Comparing `section-to-course-0.2.0/requirements/constraints.txt` & `section-to-course-0.3.0/requirements/constraints.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/admin.py` & `section-to-course-0.3.0/section_to_course/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -248,14 +248,15 @@
         run = cleaned_data['new_course_run']
         course = create_course(
             user=self.user,
             org=org,
             number=number,
             run=run,
             display_name=cleaned_data['new_course_name'],
+            self_paced=True,
         )
         return paste_from_template(
             destination_course_key=course.id,
             source_block_usage_key=cleaned_data['source_section_id'],
             user=self.user,
         )
```

### Comparing `section-to-course-0.2.0/section_to_course/api/views.py` & `section-to-course-0.3.0/section_to_course/api/views.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/apps.py` & `section-to-course-0.3.0/section_to_course/apps.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/compat.py` & `section-to-course-0.3.0/section_to_course/compat.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,27 @@
 def create_course(
     *,
     user,
     org: str,
     number: str,
     run: str,
     display_name: str,
+    self_paced: bool = False,
 ):
     """
     Create a course to match a specific course key.
     """
     # Defer this import to avoid invoking cms startup code during module import.
     from cms.djangoapps.contentstore.views.course import create_new_course
     return create_new_course(
         user,
         org=org,
         number=number,
         run=run,
-        fields={'display_name': display_name}
+        fields={'display_name': display_name, 'self_paced': self_paced},
     )
 
 
 def organization_options():
     """
     Return a Django choice tuple of organizations that can be used to create a course.
     """
```

### Comparing `section-to-course-0.2.0/section_to_course/management/commands/section_to_course.py` & `section-to-course-0.3.0/section_to_course/management/commands/section_to_course.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/migrations/0001_initial.py` & `section-to-course-0.3.0/section_to_course/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/models.py` & `section-to-course-0.3.0/section_to_course/models.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/static/section_to_course/js/admin-tools.js` & `section-to-course-0.3.0/section_to_course/static/section_to_course/js/admin-tools.js`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course/utils.py` & `section-to-course-0.3.0/section_to_course/utils.py`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/section_to_course.egg-info/PKG-INFO` & `section-to-course-0.3.0/section_to_course.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: section-to-course
-Version: 0.2.0
+Version: 0.3.0
 Summary: Factors sections from Open edX courses into their own new course.
 Home-page: https://github.com/open-craft/section-to-course
 Author: OpenCraft
 Author-email: help@opencraft.com
 License: AGPL 3.0
 Keywords: Python edx
 Classifier: Development Status :: 3 - Alpha
@@ -67,22 +67,51 @@
 
 .. code-block:: bash
 
     make dev.shell.studio
     cd /edx/src/section-to-course
     pip install -e .
 
+Configuration (optional)
+************************
+
+New courses are self-paced. If you want to set relative deadlines in them, follow the next steps:
+
+#. Add the following `Waffle Flags`_ (with ``Everyone: Yes``) in Django admin:
+
+    #. `studio.custom_relative_dates`_
+    #. `course_experience.relative_dates`_
+    #. `course_experience.relative_dates_disable_reset`_
+#. Go to `Django admin -> Course_Date_Signals -> Self paced relative dates`_ configs and add a config with ``Enabled: Yes``.
+
+.. _Waffle Flags: http://localhost:18000/admin/waffle/flag/
+.. _studio.custom_relative_dates: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-studio.custom_relative_dates
+.. _course_experience.relative_dates: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-course_experience.relative_dates
+.. _course_experience.relative_dates_disable_reset: https://edx.readthedocs.io/projects/edx-platform-technical/en/latest/featuretoggles.html#featuretoggle-course_experience.relative_dates_disable_reset
+.. _Django admin -> Course_Date_Signals -> Self paced relative dates: http://localhost:18000/admin/course_date_signals/selfpacedrelativedatesconfig/
+
 
 Usage
 *****
 
 Once installed, the plugin should automatically register itself within Django. Be sure to run database migrations.
 
 The admin views are in the Django admin, under the "Section to Course" section. From there, you can create a new section to course link, which will create a new course with the same content as the section you selected. You can also view the list of existing section to course links, refresh them, and delete them.
 
+**Note:** The start date of a newly created course is in the future, so you will likely want to modify it in the "Schedule & Details" section in Studio.
+
+Relative due dates (optional)
+=============================
+
+If you want to configure relative deadlines in your course, follow these steps:
+
+#. Mark a subsection in the newly created course as graded (otherwise, deadlines will be enforced but learners will not see these dates in the LMS).
+#. Enter the number of weeks in the subsection's "Due in" field.
+#. You may also want to adjust the new course's grading policy to change the weight of the section.
+
 Refreshing a Course
 ===================
 
 There are two ways to refresh a course:
 
 1. Use the admin action from the changelist view. This will allow you to refresh several courses at once.
 2. Use the refresh button on the detail view for a single course, shown here:
@@ -152,14 +181,22 @@
 .. There should always be an "Unreleased" section for changes pending release.
 
 Unreleased
 **********
 
 *
 
+[0.3.0] - 2023-05-12
+********************
+
+Changed
+=======
+
+* New section-based courses are self-paced.
+
 [0.2.0] - 2023-05-10
 ********************
 
 Added
 =====
 
 * Admin views for creating new section-based courses.
```

### Comparing `section-to-course-0.2.0/section_to_course.egg-info/SOURCES.txt` & `section-to-course-0.3.0/section_to_course.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `section-to-course-0.2.0/setup.py` & `section-to-course-0.3.0/setup.py`

 * *Files identical despite different names*

