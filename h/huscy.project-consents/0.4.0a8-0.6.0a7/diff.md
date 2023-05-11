# Comparing `tmp/huscy.project_consents-0.4.0a8.tar.gz` & `tmp/huscy.project_consents-0.6.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huscy.project_consents-0.4.0a8.tar", last modified: Tue Apr 25 09:19:42 2023, max compression
+gzip compressed data, was "huscy.project_consents-0.6.0a7.tar", last modified: Thu May 11 13:50:56 2023, max compression
```

## Comparing `huscy.project_consents-0.4.0a8.tar` & `huscy.project_consents-0.6.0a7.tar`

### file list

```diff
@@ -1,36 +1,40 @@
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a8/LICENSE
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-24 10:37:15.000000 huscy.project_consents-0.4.0a8/MANIFEST.in
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.4.0a8/README.md
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-04-25 09:19:06.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      435 2023-04-21 12:57:46.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/admin.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/api_urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/apps.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-04-21 08:48:37.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/forms.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2492 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/0001_initial.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/__init__.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1495 2023-04-20 11:49:39.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/models.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/services.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      731 2023-04-21 09:45:41.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/projectconsenttoken.html
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-21 09:36:45.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/urls.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     2937 2023-04-24 14:00:00.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/views.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.4.0a8/huscy/project_consents/viewsets.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.883360 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/PKG-INFO
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      920 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/SOURCES.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/dependency_links.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/requires.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-04-25 09:19:42.000000 huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/top_level.txt
--rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/setup.cfg
--rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-24 10:36:29.000000 huscy.project_consents-0.4.0a8/setup.py
-drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-04-25 09:19:42.887360 huscy.project_consents-0.4.0a8/tests/
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/tests/test_project_consent_category_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.4.0a8/tests/test_project_consent_serializer.py
--rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.4.0a8/tests/test_viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)    34523 2022-12-05 12:04:00.000000 huscy.project_consents-0.6.0a7/LICENSE
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       39 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/MANIFEST.in
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       19 2022-09-12 13:32:12.000000 huscy.project_consents-0.6.0a7/README.md
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       81 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      749 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/admin.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      479 2023-04-21 13:33:05.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/api_urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      194 2022-12-05 12:04:00.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/apps.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1007 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/forms.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     3630 2023-05-11 13:50:53.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/0001_initial.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        0 2022-12-08 10:36:34.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/__init__.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     2352 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/models.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1304 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1171 2023-01-24 10:55:08.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/services.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/
+-rw-r--r--   0 lotus     (1000) lotus     (1000)    20480 2023-05-11 09:49:55.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/.project_consent.html.swp
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     6513 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      737 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      379 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/sign_project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      608 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/signed_project_consent.html
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      430 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/urls.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     4427 2023-05-11 13:50:39.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/views.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1527 2023-01-13 21:29:30.000000 huscy.project_consents-0.6.0a7/huscy/project_consents/viewsets.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.100585 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1101 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/PKG-INFO
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     1221 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/SOURCES.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        1 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/dependency_links.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      115 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/requires.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)        6 2023-05-11 13:50:56.000000 huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/top_level.txt
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)       38 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/setup.cfg
+-rwxrwxr-x   0 lotus     (1000) lotus     (1000)     1673 2023-04-27 11:26:24.000000 huscy.project_consents-0.6.0a7/setup.py
+drwxrwxr-x   0 lotus     (1000) lotus     (1000)        0 2023-05-11 13:50:56.104585 huscy.project_consents-0.6.0a7/tests/
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      760 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/tests/test_project_consent_category_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)      684 2023-01-30 14:04:08.000000 huscy.project_consents-0.6.0a7/tests/test_project_consent_serializer.py
+-rw-rw-r--   0 lotus     (1000) lotus     (1000)     5532 2023-01-24 10:55:08.000000 huscy.project_consents-0.6.0a7/tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a8/LICENSE` & `huscy.project_consents-0.6.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/PKG-INFO` & `huscy.project_consents-0.6.0a7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project_consents
-Version: 0.4.0a8
+Version: 0.6.0a7
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a8/huscy/project_consents/migrations/0001_initial.py` & `huscy.project_consents-0.6.0a7/huscy/project_consents/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-# Generated by Django 4.2 on 2023-04-25 09:19
+# Generated by Django 4.2 on 2023-05-11 13:50
 
+from django.conf import settings
 from django.db import migrations, models
 import django.db.models.deletion
+import huscy.project_consents.models
+import phonenumber_field.modelfields
 import uuid
 
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
+        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
+        ('consents', '0001_initial'),
         ('projects', '0002_alter_membership_options'),
         ('subjects', '0001_squashed_0009_delete_contactold'),
-        ('consents', '0001_initial'),
     ]
 
     operations = [
         migrations.CreateModel(
             name='ProjectConsent',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
@@ -25,31 +29,44 @@
             ],
         ),
         migrations.CreateModel(
             name='ProjectConsentToken',
             fields=[
                 ('id', models.UUIDField(default=uuid.uuid4, primary_key=True, serialize=False)),
                 ('created_at', models.DateTimeField(auto_now_add=True)),
+                ('created_by', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
                 ('project', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
                 ('subject', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='subjects.subject')),
             ],
         ),
         migrations.CreateModel(
             name='ProjectConsentCategory',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
                 ('consent_category', models.OneToOneField(on_delete=django.db.models.deletion.PROTECT, to='consents.consentcategory')),
             ],
         ),
         migrations.CreateModel(
+            name='ContactPerson',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('email', models.EmailField(blank=True, max_length=254, null=True)),
+                ('phone', phonenumber_field.modelfields.PhoneNumberField(blank=True, max_length=128, null=True, region=None)),
+                ('project', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='projects.project')),
+                ('user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to=settings.AUTH_USER_MODEL)),
+            ],
+        ),
+        migrations.CreateModel(
             name='ProjectConsentFile',
             fields=[
                 ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('consent_file', models.OneToOneField(on_delete=django.db.models.deletion.PROTECT, to='consents.consentfile')),
+                ('consent_version', models.PositiveIntegerField(default=1)),
+                ('filehandle', models.FileField(upload_to=huscy.project_consents.models.get_consent_file_upload_path)),
+                ('created_at', models.DateTimeField(auto_now_add=True)),
                 ('project_consent', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='project_consents.projectconsent')),
                 ('subject', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, to='subjects.subject')),
             ],
             options={
-                'unique_together': {('project_consent', 'subject')},
+                'unique_together': {('project_consent', 'subject', 'consent_version')},
             },
         ),
     ]
```

### Comparing `huscy.project_consents-0.4.0a8/huscy/project_consents/serializer.py` & `huscy.project_consents-0.6.0a7/huscy/project_consents/serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/huscy/project_consents/services.py` & `huscy.project_consents-0.6.0a7/huscy/project_consents/services.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/huscy/project_consents/templates/project_consents/projectconsenttoken.html` & `huscy.project_consents-0.6.0a7/huscy/project_consents/templates/project_consents/projectconsenttoken.html`

 * *Files 22% similar despite different names*

```diff
@@ -18,12 +18,12 @@
                 </tr>
             </table>
             <button>submit</button>
         </form>
 
         {% if sign_project_consent_url %}
         {% qr_from_text sign_project_consent_url size="l" %}
-		<a href="{{ sign_project_consent_url }}">sign</a>
+        <a href="{{ sign_project_consent_url }}">sign</a>
         {% endif %}
 
     </body>
 </html>
```

### Comparing `huscy.project_consents-0.4.0a8/huscy/project_consents/viewsets.py` & `huscy.project_consents-0.6.0a7/huscy/project_consents/viewsets.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/PKG-INFO` & `huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huscy.project-consents
-Version: 0.4.0a8
+Version: 0.6.0a7
 Summary: projects_consents
 Home-page: https://bitbucket.org/huscy/project_consents
 Author: Gefan Qian, Stefan Bunde
 Author-email: gefan.qian@gmail.com, stefanbunde+git@posteo.de
 License: AGPLv3+
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `huscy.project_consents-0.4.0a8/huscy.project_consents.egg-info/SOURCES.txt` & `huscy.project_consents-0.6.0a7/huscy.project_consents.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -16,11 +16,15 @@
 huscy/project_consents/serializer.py
 huscy/project_consents/services.py
 huscy/project_consents/urls.py
 huscy/project_consents/views.py
 huscy/project_consents/viewsets.py
 huscy/project_consents/migrations/0001_initial.py
 huscy/project_consents/migrations/__init__.py
+huscy/project_consents/templates/project_consents/.project_consent.html.swp
+huscy/project_consents/templates/project_consents/project_consent.html
 huscy/project_consents/templates/project_consents/projectconsenttoken.html
+huscy/project_consents/templates/project_consents/sign_project_consent.html
+huscy/project_consents/templates/project_consents/signed_project_consent.html
 tests/test_project_consent_category_serializer.py
 tests/test_project_consent_serializer.py
 tests/test_viewsets.py
```

### Comparing `huscy.project_consents-0.4.0a8/setup.py` & `huscy.project_consents-0.6.0a7/setup.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
 
     url='https://bitbucket.org/huscy/project_consents',
 
     packages=find_namespace_packages(include=['huscy.*']),
     include_package_data=True,
 
     install_requires=[
-        'django-qr-code',
         'huscy.consents',
         'huscy.projects',
         'huscy.subjects',
+        'django-qr-code',
     ],
     extras_require={
         'development': ['psycopg2-binary'],
         'testing': ['tox', 'watchdog'],
     },
 
     classifiers=[
```

### Comparing `huscy.project_consents-0.4.0a8/tests/test_project_consent_category_serializer.py` & `huscy.project_consents-0.6.0a7/tests/test_project_consent_category_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/tests/test_project_consent_serializer.py` & `huscy.project_consents-0.6.0a7/tests/test_project_consent_serializer.py`

 * *Files identical despite different names*

### Comparing `huscy.project_consents-0.4.0a8/tests/test_viewsets.py` & `huscy.project_consents-0.6.0a7/tests/test_viewsets.py`

 * *Files identical despite different names*

