# Comparing `tmp/django-webperformers-humans-0.3.2.tar.gz` & `tmp/django-webperformers-humans-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-webperformers-humans-0.3.2.tar", last modified: Mon May 15 07:37:15 2023, max compression
+gzip compressed data, was "django-webperformers-humans-0.3.3.tar", last modified: Mon May 15 08:21:00 2023, max compression
```

## Comparing `django-webperformers-humans-0.3.2.tar` & `django-webperformers-humans-0.3.3.tar`

### file list

```diff
@@ -1,46 +1,42 @@
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/
--rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/LICENSE
--rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/MANIFEST.in
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1121 2023-05-15 06:54:22.000000 django-webperformers-humans-0.3.2/README.rst
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/PKG-INFO
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1078 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/SOURCES.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/dependency_links.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/requires.txt
--rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-15 07:37:15.000000 django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/top_level.txt
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      180 2023-05-15 07:35:41.000000 django-webperformers-humans-0.3.2/humans/admin.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/apps.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/helpers/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/helpers/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      224 2023-05-15 07:08:35.000000 django-webperformers-humans-0.3.2/humans/helpers/generic.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/helpers/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      379 2023-05-15 07:33:03.000000 django-webperformers-humans-0.3.2/humans/helpers/team.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/migrations/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1252 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0001_initial.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      369 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0002_human_position.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      377 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0003_human_twitterurl.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      720 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      555 2023-05-15 07:04:27.000000 django-webperformers-humans-0.3.2/humans/migrations/0005_rename_position_human_role_and_more.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/migrations/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1446 2023-05-15 07:34:34.000000 django-webperformers-humans-0.3.2/humans/models.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/signals/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/signals/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/signals/humans.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      251 2023-05-15 07:12:06.000000 django-webperformers-humans-0.3.2/humans/sitemap.py
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templates/
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templates/humans/
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templates/humans/personPage.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)     3260 2023-05-15 07:07:41.000000 django-webperformers-humans-0.3.2/humans/templates/humans/teamComponent.html
--rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templates/humans/teamPage.html
-drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/humans/templatetags/
--rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templatetags/__init__.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/templatetags/images.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/tests.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/humans/urls.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)     1882 2023-05-15 06:57:26.000000 django-webperformers-humans-0.3.2/humans/views.py
--rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/pyproject.toml
--rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-15 07:37:15.374862 django-webperformers-humans-0.3.2/setup.cfg
--rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.2/setup.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)    35148 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/LICENSE
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      130 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/MANIFEST.in
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1121 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/README.rst
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.788718 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     2186 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/PKG-INFO
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      850 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/SOURCES.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        1 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/dependency_links.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       12 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/requires.txt
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        7 2023-05-15 08:21:00.000000 django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/top_level.txt
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      180 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/admin.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      210 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/apps.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/helpers/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/helpers/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      224 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/helpers/generic.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      825 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/helpers/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      379 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/helpers/team.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/migrations/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1785 2023-05-15 08:19:43.000000 django-webperformers-humans-0.3.3/humans/migrations/0001_initial.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/migrations/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1457 2023-05-15 08:08:59.000000 django-webperformers-humans-0.3.3/humans/models.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/signals/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/signals/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      564 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/signals/humans.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      251 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/sitemap.py
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.788718 django-webperformers-humans-0.3.3/humans/templates/
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/templates/humans/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3844 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templates/humans/personPage.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     3260 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/templates/humans/teamComponent.html
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      127 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templates/humans/teamPage.html
+drwxr-xr-x   0 tadas     (1000) tadas     (1000)        0 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/humans/templatetags/
+-rw-r--r--   0 tadas     (1000) tadas     (1000)        0 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templatetags/__init__.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      870 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/templatetags/images.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       60 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/tests.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      288 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/humans/urls.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)     1882 2023-05-15 07:57:20.000000 django-webperformers-humans-0.3.3/humans/views.py
+-rw-r--r--   0 tadas     (1000) tadas     (1000)       88 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/pyproject.toml
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      939 2023-05-15 08:21:00.798718 django-webperformers-humans-0.3.3/setup.cfg
+-rw-r--r--   0 tadas     (1000) tadas     (1000)      295 2023-05-06 12:33:52.000000 django-webperformers-humans-0.3.3/setup.py
```

### Comparing `django-webperformers-humans-0.3.2/LICENSE` & `django-webperformers-humans-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/PKG-INFO` & `django-webperformers-humans-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-webperformers-humans-0.3.2/README.rst` & `django-webperformers-humans-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/PKG-INFO` & `django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-webperformers-humans
-Version: 0.3.2
+Version: 0.3.3
 Summary: A Django app to expose project team in seo-frienly way.
 Home-page: https://www.webperformers.net/
 Author: Your Name
 Author-email: tadas@webperformers.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-webperformers-humans-0.3.2/django_webperformers_humans.egg-info/SOURCES.txt` & `django-webperformers-humans-0.3.3/django_webperformers_humans.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -18,18 +18,14 @@
 humans/urls.py
 humans/views.py
 humans/helpers/__init__.py
 humans/helpers/generic.py
 humans/helpers/images.py
 humans/helpers/team.py
 humans/migrations/0001_initial.py
-humans/migrations/0002_human_position.py
-humans/migrations/0003_human_twitterurl.py
-humans/migrations/0004_alter_human_linkedinurl_alter_human_twitterurl_and_more.py
-humans/migrations/0005_rename_position_human_role_and_more.py
 humans/migrations/__init__.py
 humans/signals/__init__.py
 humans/signals/humans.py
 humans/templates/humans/personPage.html
 humans/templates/humans/teamComponent.html
 humans/templates/humans/teamPage.html
 humans/templatetags/__init__.py
```

### Comparing `django-webperformers-humans-0.3.2/humans/helpers/images.py` & `django-webperformers-humans-0.3.3/humans/helpers/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/humans/migrations/0001_initial.py` & `django-webperformers-humans-0.3.3/humans/migrations/0001_initial.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Generated by Django 4.1.7 on 2023-05-04 10:15
+# Generated by Django 4.2.1 on 2023-05-15 08:19
 
 import ckeditor_uploader.fields
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
 
@@ -12,21 +12,24 @@
     ]
 
     operations = [
         migrations.CreateModel(
             name='Human',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('image', models.ImageField(default='humansImages/default.webp', upload_to='humansImages/', verbose_name='Your humans image')),
+                ('position', models.SmallIntegerField(default=1, help_text='In which position is person listed', unique=True)),
+                ('image', models.ImageField(default='humansImages/default.webp', upload_to='humansImages/', verbose_name='Person image')),
                 ('name', models.TextField(null=True)),
-                ('smallDescription', ckeditor_uploader.fields.RichTextUploadingField(blank=True, null=True)),
+                ('role', models.TextField(help_text='Role inside of the organization', null=True)),
+                ('shortDescription', ckeditor_uploader.fields.RichTextUploadingField(blank=True, null=True)),
                 ('description', ckeditor_uploader.fields.RichTextUploadingField(blank=True, null=True)),
-                ('isPublished', models.BooleanField(default=False, null=True)),
-                ('customSlug', models.TextField(unique=True, verbose_name='Custom slug')),
-                ('websiteUrl', models.URLField(null=True)),
-                ('linkedInUrl', models.URLField(null=True)),
+                ('isPublished', models.BooleanField(default=False, help_text='After setting Yes, person wil be visible for all users, after setting No - for admins only ', null=True, verbose_name='Published')),
+                ('customSlug', models.TextField(help_text='Slug that will lead to persons page, i.e. yourdomain.com/team/<slug>/', unique=True, verbose_name='Custom slug')),
+                ('websiteUrl', models.URLField(blank=True, null=True)),
+                ('twitterUrl', models.URLField(blank=True, null=True)),
+                ('linkedInUrl', models.URLField(blank=True, null=True)),
             ],
             options={
                 'verbose_name_plural': 'Humans',
             },
         ),
     ]
```

### Comparing `django-webperformers-humans-0.3.2/humans/models.py` & `django-webperformers-humans-0.3.3/humans/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from django.db import models
 from ckeditor_uploader.fields import RichTextUploadingField
 from django.utils.translation import gettext as _
 from django.urls import reverse
 # Create your models here.
 
 class Human(models.Model):
-    position = models.SmallIntegerField(unique=True, help_text="In which position is person listed")
+    position = models.SmallIntegerField(unique=True, help_text="In which position is person listed", default=1)
     image = models.ImageField(upload_to='humansImages/', default='humansImages/default.webp', verbose_name=_("Person image"))
     name = models.TextField(null=True)
     role = models.TextField(null=True, help_text=_("Role inside of the organization"))
     shortDescription = RichTextUploadingField(null=True, blank=True)
     description = RichTextUploadingField(null=True, blank=True)
     isPublished = models.BooleanField(default=False, null=True, verbose_name="Published", help_text=_("After setting Yes, person wil be visible for all users, after setting No - for admins only "))
     customSlug = models.TextField(blank=False, null=False, verbose_name=_("Custom slug"), help_text=_("Slug that will lead to persons page, i.e. yourdomain.com/team/<slug>/"), unique=True)
```

### Comparing `django-webperformers-humans-0.3.2/humans/signals/humans.py` & `django-webperformers-humans-0.3.3/humans/signals/humans.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/humans/templates/humans/personPage.html` & `django-webperformers-humans-0.3.3/humans/templates/humans/personPage.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/humans/templates/humans/teamComponent.html` & `django-webperformers-humans-0.3.3/humans/templates/humans/teamComponent.html`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/humans/templatetags/images.py` & `django-webperformers-humans-0.3.3/humans/templatetags/images.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/humans/views.py` & `django-webperformers-humans-0.3.3/humans/views.py`

 * *Files identical despite different names*

### Comparing `django-webperformers-humans-0.3.2/setup.cfg` & `django-webperformers-humans-0.3.3/setup.cfg`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-webperformers-humans
-version = 0.3.2
+version = 0.3.3
 description = A Django app to expose project team in seo-frienly way.
 url = https://www.webperformers.net/
 author = Your Name
 author_email = tadas@webperformers.net
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
```

