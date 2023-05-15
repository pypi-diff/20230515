# Comparing `tmp/djangoldp_tzcld-1.0.6.tar.gz` & `tmp/djangoldp_tzcld-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/djangoldp_tzcld-1.0.6.tar", last modified: Mon May 15 09:28:58 2023, max compression
+gzip compressed data, was "dist/djangoldp_tzcld-1.0.7.tar", last modified: Mon May 15 09:48:48 2023, max compression
```

## Comparing `djangoldp_tzcld-1.0.6.tar` & `djangoldp_tzcld-1.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/
--rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/README.md
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)     1682 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/
--rw-rw-rw-   0 root         (0) root         (0)    18317 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/models.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/permissions.py
--rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/admin.py
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-15 09:28:56.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:28:58.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
--rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
--rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
--rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
--rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
--rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
--rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
--rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
--rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
--rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
--rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
--rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
--rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
--rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-15 09:28:39.000000 djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/
+-rw-rw-rw-   0 root         (0) root         (0)       65 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      505 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)     1682 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/
+-rw-rw-rw-   0 root         (0) root         (0)    18337 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/permissions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2347 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-05-15 09:48:46.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-15 09:48:48.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     5896 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py
+-rw-rw-rw-   0 root         (0) root         (0)      836 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py
+-rw-rw-rw-   0 root         (0) root         (0)     9812 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py
+-rw-rw-rw-   0 root         (0) root         (0)     1889 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py
+-rw-rw-rw-   0 root         (0) root         (0)      501 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0014_auto_20230330_1258.py
+-rw-rw-rw-   0 root         (0) root         (0)     1099 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py
+-rw-rw-rw-   0 root         (0) root         (0)      431 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0002_tzcldcommunity_contact_job.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-15 09:48:31.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1033 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)    18022 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py
+-rw-rw-rw-   0 root         (0) root         (0)     4403 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py
+-rw-rw-rw-   0 root         (0) root         (0)      706 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0022_tzcldcommunity_membership_organisation_name.py
+-rw-rw-rw-   0 root         (0) root         (0)      632 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py
+-rw-rw-rw-   0 root         (0) root         (0)     1816 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py
+-rw-rw-rw-   0 root         (0) root         (0)      653 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py
+-rw-rw-rw-   0 root         (0) root         (0)     1750 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py
+-rw-rw-rw-   0 root         (0) root         (0)     1270 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2023-05-15 09:48:30.000000 djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py
```

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld.egg-info/SOURCES.txt` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/models.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,18 +395,18 @@
 def create_user_tzcld_profile(sender, instance, created, **kwargs):
     if not Model.is_external(instance) and created:
         tzcld_profile = TzcldProfile.objects.create(user=instance)
         profile_job = TzcldProfileJob.objects.create(profile=tzcld_profile)
         TzcldContactEmail.objects.create(job=profile_job)
         TzcldContactPhone.objects.create(job=profile_job)
 
-        # Add user to tzcld community
-        tzcld_community = Community.objects.get(id=1)
-        tzcld_community.members.add(instance)
-        tzcld_community.save()
+        # add the user to the first (tzcld) community
+        community = Community.objects.order_by('id').first()
+        if community:
+            community.members.create(user=instance)
 
 # Create tzcld community profile, job instance and contact email/phone when community is created
 @receiver(post_save, sender=Community)
 def create_tzcld_community(instance, created, **kwargs):
     if not Model.is_external(instance) and created:
         tzCommunity = TzcldCommunity.objects.create(community=instance)
         territory_location = TzcldTerritoryLocation.objects.create(name=instance.name + " Location", community=tzCommunity)
```

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/permissions.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/permissions.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/admin.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/admin.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0004_tzcldprofilejob_tzcldprofilejobemail_tzcldprofilejobphone.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0007_auto_20230327_1451.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0001_initial.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0013_auto_20230330_1246.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0016_tzcldcontactmember.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0019_auto_20230414_1634.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0021_auto_20230510_1232.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0012_auto_20230330_1233.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0003_auto_20220720_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0006_auto_20230327_1449.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0005_auto_20230325_1335.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0011_auto_20230328_1045.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0018_auto_20230406_1755.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0017_tzcldcontactmember_community.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0015_auto_20230330_1439.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0010_auto_20230327_1629.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0020_auto_20230417_1242.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0009_auto_20230327_1623.py`

 * *Files identical despite different names*

### Comparing `djangoldp_tzcld-1.0.6/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py` & `djangoldp_tzcld-1.0.7/djangoldp_tzcld/migrations/0008_auto_20230327_1602.py`

 * *Files identical despite different names*

