# Comparing `tmp/django-peeringdb-3.0.0.tar.gz` & `tmp/django-peeringdb-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-peeringdb-3.0.0.tar", max compression
+gzip compressed data, was "django-peeringdb-3.0.1.tar", max compression
```

## Comparing `django-peeringdb-3.0.0.tar` & `django-peeringdb-3.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     1303 2022-10-10 13:03:11.610570 django-peeringdb-3.0.0/LICENSE.txt
--rw-r--r--   0        0        0      831 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/README.md
--rw-r--r--   0        0        0     1616 2023-04-11 13:16:39.413699 django-peeringdb-3.0.0/pyproject.toml
--rw-r--r--   0        0        0      175 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/__init__.py
--rw-r--r--   0        0        0      183 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/admin/__init__.py
--rw-r--r--   0        0        0     2505 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/admin/views.py
--rw-r--r--   0        0        0       70 2022-07-15 13:10:53.610434 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/__init__.py
--rw-r--r--   0        0        0     7373 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/backend.py
--rw-r--r--   0        0        0     1103 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/load.py
--rw-r--r--   0        0        0      812 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/setup.py
--rw-r--r--   0        0        0    18324 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/const.py
--rw-r--r--   0        0        0      806 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/default_settings.py
--rw-r--r--   0        0        0     2529 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/fields.py
--rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/__init__.py
--rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/commands/__init__.py
--rw-r--r--   0        0        0      662 2022-07-15 13:10:53.613767 django-peeringdb-3.0.0/src/django_peeringdb/management/commands/pdb_sync.py
--rw-r--r--   0        0        0    31571 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0001_initial.py
--rw-r--r--   0        0        0     1241 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py
--rw-r--r--   0        0        0      563 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py
--rw-r--r--   0        0        0      743 2023-03-08 12:36:10.126224 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py
--rw-r--r--   0        0        0      920 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0005_fac_contacts.py
--rw-r--r--   0        0        0      400 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0006_net_operational.py
--rw-r--r--   0        0        0      365 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0007_add_verbose_names.py
--rw-r--r--   0        0        0     2298 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0008_traffic_levels.py
--rw-r--r--   0        0        0      397 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0009_ixlanprefix_in_dfz.py
--rw-r--r--   0        0        0      820 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py
--rw-r--r--   0        0        0     1089 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py
--rw-r--r--   0        0        0     2156 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py
--rw-r--r--   0        0        0     2783 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py
--rw-r--r--   0        0        0      998 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py
--rw-r--r--   0        0        0     2057 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0015_add_aka_longname.py
--rw-r--r--   0        0        0     1621 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py
--rw-r--r--   0        0        0     2338 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0017_facility_fields.py
--rw-r--r--   0        0        0      990 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0018_add_region_continent_field.py
--rw-r--r--   0        0        0     1050 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0019_ix_add_sales_phone_email.py
--rw-r--r--   0        0        0     1176 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0020_status_dashboard.py
--rw-r--r--   0        0        0      720 2023-03-08 12:36:10.129557 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0021_rir_fields.py
--rw-r--r--   0        0        0     4784 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0022_carriers.py
--rw-r--r--   0        0        0      514 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0023_mtu.py
--rw-r--r--   0        0        0      517 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0024_carrier_website_optional.py
--rw-r--r--   0        0        0     3332 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0025_campus.py
--rw-r--r--   0        0        0     1612 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/migrations/0026_add_social_media.py
--rw-r--r--   0        0        0        0 2022-07-15 13:10:53.620434 django-peeringdb-3.0.0/src/django_peeringdb/migrations/__init__.py
--rw-r--r--   0        0        0      260 2022-07-15 13:10:53.620434 django-peeringdb-3.0.0/src/django_peeringdb/models/__init__.py
--rw-r--r--   0        0        0    18192 2023-04-11 13:16:27.426957 django-peeringdb-3.0.0/src/django_peeringdb/models/abstract.py
--rw-r--r--   0        0        0     5601 2023-03-08 12:36:10.132891 django-peeringdb-3.0.0/src/django_peeringdb/models/concrete.py
--rw-r--r--   0        0        0     1942 2023-04-11 13:17:13.497629 django-peeringdb-3.0.0/setup.py
--rw-r--r--   0        0        0     1974 2023-04-11 13:17:13.498307 django-peeringdb-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1303 2022-10-10 13:03:11.610570 django-peeringdb-3.0.1/LICENSE.txt
+-rw-r--r--   0        0        0      831 2022-07-15 13:10:53.610434 django-peeringdb-3.0.1/README.md
+-rw-r--r--   0        0        0     1616 2023-05-15 13:23:12.533407 django-peeringdb-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0      175 2022-07-15 13:10:53.610434 django-peeringdb-3.0.1/src/django_peeringdb/__init__.py
+-rw-r--r--   0        0        0      183 2022-07-15 13:10:53.610434 django-peeringdb-3.0.1/src/django_peeringdb/admin/__init__.py
+-rw-r--r--   0        0        0     2505 2022-07-15 13:10:53.610434 django-peeringdb-3.0.1/src/django_peeringdb/admin/views.py
+-rw-r--r--   0        0        0       70 2022-07-15 13:10:53.610434 django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/__init__.py
+-rw-r--r--   0        0        0     7373 2023-03-08 12:36:10.126224 django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/backend.py
+-rw-r--r--   0        0        0     1103 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/load.py
+-rw-r--r--   0        0        0      812 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/setup.py
+-rw-r--r--   0        0        0    18324 2023-04-11 13:16:27.426957 django-peeringdb-3.0.1/src/django_peeringdb/const.py
+-rw-r--r--   0        0        0      806 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/default_settings.py
+-rw-r--r--   0        0        0     2490 2023-05-15 13:23:05.893374 django-peeringdb-3.0.1/src/django_peeringdb/fields.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/management/__init__.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/management/commands/__init__.py
+-rw-r--r--   0        0        0      662 2022-07-15 13:10:53.613767 django-peeringdb-3.0.1/src/django_peeringdb/management/commands/pdb_sync.py
+-rw-r--r--   0        0        0    31571 2023-03-08 12:36:10.126224 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1241 2023-03-08 12:36:10.126224 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0002_network_fields_help_text.py
+-rw-r--r--   0        0        0      563 2023-03-08 12:36:10.126224 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0003_never_via_route_servers.py
+-rw-r--r--   0        0        0      743 2023-03-08 12:36:10.126224 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0004_rs_lg_fields.py
+-rw-r--r--   0        0        0      920 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0005_fac_contacts.py
+-rw-r--r--   0        0        0      400 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0006_net_operational.py
+-rw-r--r--   0        0        0      365 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0007_add_verbose_names.py
+-rw-r--r--   0        0        0     2298 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0008_traffic_levels.py
+-rw-r--r--   0        0        0      397 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0009_ixlanprefix_in_dfz.py
+-rw-r--r--   0        0        0      820 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0010_ix_ixf_fields.py
+-rw-r--r--   0        0        0     1089 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py
+-rw-r--r--   0        0        0     2156 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py
+-rw-r--r--   0        0        0     2783 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0013_add_phone_help_text.py
+-rw-r--r--   0        0        0      998 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0014_add_suite_and_floor.py
+-rw-r--r--   0        0        0     2057 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0015_add_aka_longname.py
+-rw-r--r--   0        0        0     1621 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py
+-rw-r--r--   0        0        0     2338 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0017_facility_fields.py
+-rw-r--r--   0        0        0      990 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0018_add_region_continent_field.py
+-rw-r--r--   0        0        0     1050 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0019_ix_add_sales_phone_email.py
+-rw-r--r--   0        0        0     1176 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0020_status_dashboard.py
+-rw-r--r--   0        0        0      720 2023-03-08 12:36:10.129557 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0021_rir_fields.py
+-rw-r--r--   0        0        0     4784 2023-03-08 12:36:10.132891 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0022_carriers.py
+-rw-r--r--   0        0        0      514 2023-03-08 12:36:10.132891 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0023_mtu.py
+-rw-r--r--   0        0        0      517 2023-03-08 12:36:10.132891 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0024_carrier_website_optional.py
+-rw-r--r--   0        0        0     3332 2023-03-08 12:36:10.132891 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0025_campus.py
+-rw-r--r--   0        0        0     1612 2023-04-11 13:16:27.426957 django-peeringdb-3.0.1/src/django_peeringdb/migrations/0026_add_social_media.py
+-rw-r--r--   0        0        0        0 2022-07-15 13:10:53.620434 django-peeringdb-3.0.1/src/django_peeringdb/migrations/__init__.py
+-rw-r--r--   0        0        0      260 2022-07-15 13:10:53.620434 django-peeringdb-3.0.1/src/django_peeringdb/models/__init__.py
+-rw-r--r--   0        0        0    18192 2023-04-11 13:16:27.426957 django-peeringdb-3.0.1/src/django_peeringdb/models/abstract.py
+-rw-r--r--   0        0        0     5601 2023-03-08 12:36:10.132891 django-peeringdb-3.0.1/src/django_peeringdb/models/concrete.py
+-rw-r--r--   0        0        0     1942 2023-05-15 13:23:35.143017 django-peeringdb-3.0.1/setup.py
+-rw-r--r--   0        0        0     1974 2023-05-15 13:23:35.143674 django-peeringdb-3.0.1/PKG-INFO
```

### Comparing `django-peeringdb-3.0.0/LICENSE.txt` & `django-peeringdb-3.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/README.md` & `django-peeringdb-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/pyproject.toml` & `django-peeringdb-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-peeringdb"
-version = "3.0.0"
+version = "3.0.1"
 description = "PeeringDB Django models"
 readme = "README.md"
 repository = "https://github.com/peeringdb/django-peeringdb"
 authors = ["PeeringDB <support@peeringdb.com>"]
 license = "Apache-2.0"
 
 classifiers = [
```

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/admin/views.py` & `django-peeringdb-3.0.1/src/django_peeringdb/admin/views.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/backend.py` & `django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/backend.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/load.py` & `django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/load.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/client_adaptor/setup.py` & `django-peeringdb-3.0.1/src/django_peeringdb/client_adaptor/setup.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/const.py` & `django-peeringdb-3.0.1/src/django_peeringdb/const.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/default_settings.py` & `django-peeringdb-3.0.1/src/django_peeringdb/default_settings.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/fields.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,18 +65,15 @@
 
         return ",".join(picked)
 
     def to_python(self, value):
         if isinstance(value, (list, set, tuple)):
             return value
 
-        if value is None:
-            return value
-
-        if value == "[]":
+        if not value or value == "[]":
             return None
 
         values = self.cleaned_values(value.split(","))
         self.clean_choices(values)
 
         return values
```

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/management/commands/pdb_sync.py` & `django-peeringdb-3.0.1/src/django_peeringdb/management/commands/pdb_sync.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0001_initial.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0002_network_fields_help_text.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0002_network_fields_help_text.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0003_never_via_route_servers.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0003_never_via_route_servers.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0004_rs_lg_fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0004_rs_lg_fields.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0005_fac_contacts.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0005_fac_contacts.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0008_traffic_levels.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0008_traffic_levels.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0010_ix_ixf_fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0010_ix_ixf_fields.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0011_ixlan_ixf_fields.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0012_change_network_prefixes_and_info_type.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0013_add_phone_help_text.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0013_add_phone_help_text.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0014_add_suite_and_floor.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0014_add_suite_and_floor.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0015_add_aka_longname.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0015_add_aka_longname.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0016_add_ix_service_and_terms.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0017_facility_fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0017_facility_fields.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0018_add_region_continent_field.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0018_add_region_continent_field.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0019_ix_add_sales_phone_email.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0019_ix_add_sales_phone_email.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0020_status_dashboard.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0020_status_dashboard.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0021_rir_fields.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0021_rir_fields.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0022_carriers.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0022_carriers.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0023_mtu.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0023_mtu.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0024_carrier_website_optional.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0024_carrier_website_optional.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0025_campus.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0025_campus.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/migrations/0026_add_social_media.py` & `django-peeringdb-3.0.1/src/django_peeringdb/migrations/0026_add_social_media.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/models/abstract.py` & `django-peeringdb-3.0.1/src/django_peeringdb/models/abstract.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/src/django_peeringdb/models/concrete.py` & `django-peeringdb-3.0.1/src/django_peeringdb/models/concrete.py`

 * *Files identical despite different names*

### Comparing `django-peeringdb-3.0.0/setup.py` & `django-peeringdb-3.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'django_inet>=1,<2']
 
 entry_points = \
 {'markdown.extensions': ['pymdgen = pymdgen.md:Extension']}
 
 setup_kwargs = {
     'name': 'django-peeringdb',
-    'version': '3.0.0',
+    'version': '3.0.1',
     'description': 'PeeringDB Django models',
     'long_description': '\n# django-peeringdb\n\n[![PyPI](https://img.shields.io/pypi/v/django_peeringdb.svg?maxAge=2592000)](https://pypi.python.org/pypi/django_peeringdb)\n[![PyPI](https://img.shields.io/pypi/pyversions/django-peeringdb.svg)](https://pypi.python.org/pypi/django-peeringdb)\n[![Tests](https://github.com/peeringdb/django-peeringdb/workflows/tests/badge.svg)](https://github.com/peeringdb/django-peeringdb/actions/workflows/tests.yml)\n[![LGTM Grade](https://img.shields.io/lgtm/grade/python/github/peeringdb/django-peeringdb)](https://lgtm.com/projects/g/peeringdb/django-peeringdb/alerts/)\n[![Codecov](https://img.shields.io/codecov/c/github/peeringdb/django-peeringdb/master.svg?maxAge=2592000)](https://codecov.io/github/peeringdb/django-peeringdb)\n\nDjango models for PeeringDB\n\nSee the docs at http://peeringdb.github.io/django-peeringdb/\n\n',
     'author': 'PeeringDB',
     'author_email': 'support@peeringdb.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/peeringdb/django-peeringdb',
```

### Comparing `django-peeringdb-3.0.0/PKG-INFO` & `django-peeringdb-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-peeringdb
-Version: 3.0.0
+Version: 3.0.1
 Summary: PeeringDB Django models
 Home-page: https://github.com/peeringdb/django-peeringdb
 License: Apache-2.0
 Author: PeeringDB
 Author-email: support@peeringdb.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

