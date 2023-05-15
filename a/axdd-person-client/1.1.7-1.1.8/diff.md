# Comparing `tmp/axdd-person-client-1.1.7.tar.gz` & `tmp/axdd-person-client-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axdd-person-client-1.1.7.tar", last modified: Fri May 12 17:49:54 2023, max compression
+gzip compressed data, was "axdd-person-client-1.1.8.tar", last modified: Mon May 15 16:09:45 2023, max compression
```

## Comparing `axdd-person-client-1.1.7.tar` & `axdd-person-client-1.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/axdd_person_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-12 17:49:54.000000 axdd-person-client-1.1.7/axdd_person_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/conf/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/conf/settings.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/clients/
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27342 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/clients/mock_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3588 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/components.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/databases/
--rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/postgres.py
--rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/databases/uwpds.py
--rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:54.364961 axdd-person-client-1.1.7/uw_person_client/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_components.py
--rw-r--r--   0 runner    (1001) docker     (122)    35548 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_core_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-12 17:49:44.000000 axdd-person-client-1.1.7/uw_person_client/tests/test_mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/axdd_person_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      662 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      779 2023-05-15 16:09:45.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       48 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-15 16:09:44.000000 axdd-person-client-1.1.8/axdd_person_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/conf/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      869 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/conf/settings.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1509 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/uw_person_client/
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.262085 axdd-person-client-1.1.8/uw_person_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27839 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4733 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/clients/mock_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/components.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/uw_person_client/databases/
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6038 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/databases/uwpds.py
+-rw-r--r--   0 runner    (1001) docker     (122)      194 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      349 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:45.266085 axdd-person-client-1.1.8/uw_person_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      501 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35780 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_core_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3881 2023-05-15 16:09:31.000000 axdd-person-client-1.1.8/uw_person_client/tests/test_mock_client.py
```

### Comparing `axdd-person-client-1.1.7/LICENSE` & `axdd-person-client-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/PKG-INFO` & `axdd-person-client-1.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.7
+Version: 1.1.8
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.7/README.md` & `axdd-person-client-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/axdd_person_client.egg-info/PKG-INFO` & `axdd-person-client-1.1.8/axdd_person_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: axdd-person-client
-Version: 1.1.7
+Version: 1.1.8
 Summary: A library for connecting to and querying the uw-person-datastore
 Home-page: https://github.com/uw-it-aca/axdd-person-client
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `axdd-person-client-1.1.7/axdd_person_client.egg-info/SOURCES.txt` & `axdd-person-client-1.1.8/axdd_person_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/conf/settings.py` & `axdd-person-client-1.1.8/conf/settings.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/setup.py` & `axdd-person-client-1.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/clients/__init__.py` & `axdd-person-client-1.1.8/uw_person_client/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/clients/core_client.py` & `axdd-person-client-1.1.8/uw_person_client/clients/core_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,18 +193,14 @@
         student.application_status_desc = sqla_student.application_status_desc
         student.application_type_code = sqla_student.application_type_code
         student.application_type_desc = sqla_student.application_type_desc
         student.applied_to_graduate_yr_qtr_desc = \
             sqla_student.applied_to_graduate_yr_qtr_desc
         student.applied_to_graduate_yr_qtr_id = \
             sqla_student.applied_to_graduate_yr_qtr_id
-        student.assigned_ethnic_code = sqla_student.assigned_ethnic_code
-        student.assigned_ethnic_desc = sqla_student.assigned_ethnic_desc
-        student.assigned_ethnic_group_desc = \
-            sqla_student.assigned_ethnic_group_desc
         student.asuwind = sqla_student.asuwind
         student.birth_city = sqla_student.birth_city
         student.birth_country = sqla_student.birth_country
         student.birth_state = sqla_student.birth_state
         student.birthdate = sqla_student.birthdate
         student.campus_code = sqla_student.campus_code
         student.campus_desc = sqla_student.campus_desc
@@ -218,24 +214,36 @@
         student.emergency_email = sqla_student.emergency_email
         student.emergency_name = sqla_student.emergency_name
         student.emergency_phone = sqla_student.emergency_phone
         student.enroll_status_code = sqla_student.enroll_status_code
         student.enroll_status_request_code = \
             sqla_student.enroll_status_request_code
         student.enroll_status_desc = sqla_student.enroll_status_desc
+        student.ethnic_code = sqla_student.ethnic_code
+        student.ethnic_desc = sqla_student.ethnic_desc
+        student.ethnic_long_desc = sqla_student.ethnic_long_desc
+        student.ethnic_group_code = sqla_student.ethnic_group_code
+        student.ethnic_group_desc = Student.ETHNIC_GROUP_DESCRIPTIONS.get(
+            sqla_student.ethnic_group_code)
         student.exemption_code = sqla_student.exemption_code
         student.exemption_desc = sqla_student.exemption_desc
         student.external_email = sqla_student.external_email
         student.first_generation_4yr_ind = \
             sqla_student.first_generation_4yr_ind
         student.first_generation_ind = sqla_student.first_generation_ind
         student.gender = sqla_student.gender
         student.high_school_gpa = sqla_student.high_school_gpa
         student.high_school_graduation_date = \
             sqla_student.high_school_graduation_date
+        student.hispanic_code = sqla_student.hispanic_code
+        student.hispanic_desc = sqla_student.hispanic_desc
+        student.hispanic_long_desc = sqla_student.hispanic_long_desc
+        student.hispanic_group_code = sqla_student.hispanic_group_code
+        student.hispanic_group_desc = Student.ETHNIC_GROUP_DESCRIPTIONS.get(
+            sqla_student.hispanic_group_code)
         student.honors_program_code = sqla_student.honors_program_code
         student.honors_program_ind = sqla_student.honors_program_ind
         student.iss_perm_resident_country = \
             sqla_student.iss_perm_resident_country
         student.jr_col_gpa = sqla_student.jr_col_gpa
         student.last_enrolled_yr_qtr_desc = \
             sqla_student.last_enrolled_yr_qtr_desc
```

### Comparing `axdd-person-client-1.1.7/uw_person_client/clients/mock_client.py` & `axdd-person-client-1.1.8/uw_person_client/clients/mock_client.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/components.py` & `axdd-person-client-1.1.8/uw_person_client/components.py`

 * *Files 9% similar despite different names*

```diff
@@ -87,15 +87,24 @@
 
 
 class Person(AbstractBase):
     pass
 
 
 class Student(AbstractBase):
-    pass
+    ETHNIC_GROUP_DESCRIPTIONS = {
+        "1": "African American",
+        "2": "American Indian",
+        "3": "White",
+        "4": "Hispanic/Latino",
+        "5": "Asian American",
+        "6": "Hawaiian/Pacific Islander",
+        "7": "Not Indicated",
+        "99": "International",
+    }
 
 
 class Employee(AbstractBase):
     pass
 
 
 class Transcript(AbstractBase):
```

### Comparing `axdd-person-client-1.1.7/uw_person_client/databases/__init__.py` & `axdd-person-client-1.1.8/uw_person_client/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/databases/postgres.py` & `axdd-person-client-1.1.8/uw_person_client/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/databases/uwpds.py` & `axdd-person-client-1.1.8/uw_person_client/databases/uwpds.py`

 * *Files identical despite different names*

### Comparing `axdd-person-client-1.1.7/uw_person_client/tests/test_core_client.py` & `axdd-person-client-1.1.8/uw_person_client/tests/test_core_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -380,17 +380,14 @@
         mock_student.student_number = MagicMock()
         mock_student.application_status_code = MagicMock()
         mock_student.application_status_desc = MagicMock()
         mock_student.application_type_code = MagicMock()
         mock_student.application_type_desc = MagicMock()
         mock_student.applied_to_graduate_yr_qtr_desc = MagicMock()
         mock_student.applied_to_graduate_yr_qtr_id = MagicMock()
-        mock_student.assigned_ethnic_code = MagicMock()
-        mock_student.assigned_ethnic_desc = MagicMock()
-        mock_student.assigned_ethnic_group_desc = MagicMock()
         mock_student.asuwind = MagicMock()
         mock_student.birth_city = MagicMock()
         mock_student.birth_country = MagicMock()
         mock_student.birth_state = MagicMock()
         mock_student.birthdate = MagicMock()
         mock_student.campus_code = MagicMock()
         mock_student.campus_desc = MagicMock()
@@ -403,22 +400,30 @@
         mock_student.disability_ind = MagicMock()
         mock_student.emergency_email = MagicMock()
         mock_student.emergency_name = MagicMock()
         mock_student.emergency_phone = MagicMock()
         mock_student.enroll_status_code = MagicMock()
         mock_student.enroll_status_request_code = MagicMock()
         mock_student.enroll_status_desc = MagicMock()
+        mock_student.ethnic_code = MagicMock()
+        mock_student.ethnic_desc = MagicMock()
+        mock_student.ethnic_long_desc = MagicMock()
+        mock_student.ethnic_group_code = MagicMock()
         mock_student.exemption_code = MagicMock()
         mock_student.exemption_desc = MagicMock()
         mock_student.external_email = MagicMock()
         mock_student.first_generation_4yr_ind = MagicMock()
         mock_student.first_generation_ind = MagicMock()
         mock_student.gender = MagicMock()
         mock_student.high_school_gpa = MagicMock()
         mock_student.high_school_graduation_date = MagicMock()
+        mock_student.hispanic_code = MagicMock()
+        mock_student.hispanic_desc = MagicMock()
+        mock_student.hispanic_long_desc = MagicMock()
+        mock_student.hispanic_group_code = MagicMock()
         mock_student.honors_program_code = MagicMock()
         mock_student.honors_program_ind = MagicMock()
         mock_student.iss_perm_resident_country = MagicMock()
         mock_student.jr_col_gpa = MagicMock()
         mock_student.last_enrolled_yr_qtr_desc = MagicMock()
         mock_student.last_enrolled_yr_qtr_id = MagicMock()
         mock_student.local_addr_4digit_zip = MagicMock()
```

### Comparing `axdd-person-client-1.1.7/uw_person_client/tests/test_mock_client.py` & `axdd-person-client-1.1.8/uw_person_client/tests/test_mock_client.py`

 * *Files identical despite different names*

