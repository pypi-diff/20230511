# Comparing `tmp/tap-impact-1.0.0.tar.gz` & `tmp/tap-impact-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-impact-1.0.0.tar", last modified: Tue Sep  1 20:17:58 2020, max compression
+gzip compressed data, was "dist/tap-impact-1.0.1.tar", last modified: Thu May 11 12:11:46 2023, max compression
```

## Comparing `tap-impact-1.0.0.tar` & `tap-impact-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 aerlich    (503) staff       (20)        0 2020-09-01 20:17:58.639605 tap-impact-1.0.0/
--rw-r--r--   0 aerlich    (503) staff       (20)    34523 2020-09-01 20:13:18.000000 tap-impact-1.0.0/LICENSE
--rw-r--r--   0 aerlich    (503) staff       (20)       49 2020-09-01 20:13:18.000000 tap-impact-1.0.0/MANIFEST.in
--rw-r--r--   0 aerlich    (503) staff       (20)      327 2020-09-01 20:17:58.639320 tap-impact-1.0.0/PKG-INFO
--rw-r--r--   0 aerlich    (503) staff       (20)    19254 2020-09-01 20:13:18.000000 tap-impact-1.0.0/README.md
--rw-r--r--   0 aerlich    (503) staff       (20)       38 2020-09-01 20:17:58.639694 tap-impact-1.0.0/setup.cfg
--rw-r--r--   0 aerlich    (503) staff       (20)      834 2020-09-01 20:17:44.000000 tap-impact-1.0.0/setup.py
-drwxr-xr-x   0 aerlich    (503) staff       (20)        0 2020-09-01 20:17:58.623278 tap-impact-1.0.0/tap_impact/
--rw-r--r--   0 aerlich    (503) staff       (20)     1327 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/__init__.py
--rw-r--r--   0 aerlich    (503) staff       (20)     6545 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/client.py
--rw-r--r--   0 aerlich    (503) staff       (20)     1013 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/discover.py
--rw-r--r--   0 aerlich    (503) staff       (20)     1341 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schema.py
-drwxr-xr-x   0 aerlich    (503) staff       (20)        0 2020-09-01 20:17:58.638689 tap-impact-1.0.0/tap_impact/schemas/
--rw-r--r--   0 aerlich    (503) staff       (20)     2214 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/action_inquiries.json
--rw-r--r--   0 aerlich    (503) staff       (20)     1877 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/action_updates.json
--rw-r--r--   0 aerlich    (503) staff       (20)     2745 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/actions.json
--rw-r--r--   0 aerlich    (503) staff       (20)     6842 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/ads.json
--rw-r--r--   0 aerlich    (503) staff       (20)     1042 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/api_submissions.json
--rw-r--r--   0 aerlich    (503) staff       (20)     5323 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/campaigns.json
--rw-r--r--   0 aerlich    (503) staff       (20)     4879 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/catalog_items.json
--rw-r--r--   0 aerlich    (503) staff       (20)      762 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/catalogs.json
--rw-r--r--   0 aerlich    (503) staff       (20)     2511 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/clicks.json
--rw-r--r--   0 aerlich    (503) staff       (20)     4363 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/company_information.json
--rw-r--r--   0 aerlich    (503) staff       (20)     1976 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/contacts.json
--rw-r--r--   0 aerlich    (503) staff       (20)     9160 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/conversion_paths.json
--rw-r--r--   0 aerlich    (503) staff       (20)     4332 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/deals.json
--rw-r--r--   0 aerlich    (503) staff       (20)      502 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/exception_list_items.json
--rw-r--r--   0 aerlich    (503) staff       (20)     1185 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/exception_lists.json
--rw-r--r--   0 aerlich    (503) staff       (20)      793 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/ftp_file_submissions.json
--rw-r--r--   0 aerlich    (503) staff       (20)     2119 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/invoices.json
--rw-r--r--   0 aerlich    (503) staff       (20)      870 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/media_partner_groups.json
--rw-r--r--   0 aerlich    (503) staff       (20)     3305 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/media_partners.json
--rw-r--r--   0 aerlich    (503) staff       (20)      910 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/notes.json
--rw-r--r--   0 aerlich    (503) staff       (20)      652 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/phone_numbers.json
--rw-r--r--   0 aerlich    (503) staff       (20)     5146 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/promo_codes.json
--rw-r--r--   0 aerlich    (503) staff       (20)     1459 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/report_metadata.json
--rw-r--r--   0 aerlich    (503) staff       (20)      365 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/reports.json
--rw-r--r--   0 aerlich    (503) staff       (20)     7122 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/tracking_value_requests.json
--rw-r--r--   0 aerlich    (503) staff       (20)      899 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/schemas/unique_urls.json
--rw-r--r--   0 aerlich    (503) staff       (20)     8588 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/streams.py
--rw-r--r--   0 aerlich    (503) staff       (20)    19020 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/sync.py
--rw-r--r--   0 aerlich    (503) staff       (20)     3454 2020-09-01 20:13:18.000000 tap-impact-1.0.0/tap_impact/transform.py
-drwxr-xr-x   0 aerlich    (503) staff       (20)        0 2020-09-01 20:17:58.625612 tap-impact-1.0.0/tap_impact.egg-info/
--rw-r--r--   0 aerlich    (503) staff       (20)      327 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/PKG-INFO
--rw-r--r--   0 aerlich    (503) staff       (20)     1368 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/SOURCES.txt
--rw-r--r--   0 aerlich    (503) staff       (20)        1 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/dependency_links.txt
--rw-r--r--   0 aerlich    (503) staff       (20)       72 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/entry_points.txt
--rw-r--r--   0 aerlich    (503) staff       (20)       85 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/requires.txt
--rw-r--r--   0 aerlich    (503) staff       (20)       11 2020-09-01 20:17:58.000000 tap-impact-1.0.0/tap_impact.egg-info/top_level.txt
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 12:11:46.000000 tap-impact-1.0.1/
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 12:11:46.000000 tap-impact-1.0.1/tap_impact/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3454 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/transform.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6545 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/client.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 12:11:46.000000 tap-impact-1.0.1/tap_impact/schemas/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1042 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/api_submissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     7122 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/tracking_value_requests.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1185 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/exception_lists.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      899 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/unique_urls.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4363 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/company_information.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      502 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/exception_list_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      652 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/phone_numbers.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     3305 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/media_partners.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      870 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/media_partner_groups.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      910 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/notes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1976 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/contacts.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1877 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/action_updates.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     9160 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/conversion_paths.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5146 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/promo_codes.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2119 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/invoices.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2511 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/clicks.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      365 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/reports.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4879 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/catalog_items.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2745 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/actions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     4332 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/deals.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5323 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/campaigns.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      793 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/ftp_file_submissions.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2214 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/action_inquiries.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     6842 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/ads.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1459 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/report_metadata.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      762 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schemas/catalogs.json
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     8588 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/streams.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1341 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/schema.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1327 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19014 2023-05-11 12:10:50.000000 tap-impact-1.0.1/tap_impact/sync.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1013 2023-05-11 12:09:24.000000 tap-impact-1.0.1/tap_impact/discover.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2023-05-11 12:09:24.000000 tap-impact-1.0.1/MANIFEST.in
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2023-05-11 12:11:46.000000 tap-impact-1.0.1/tap_impact.egg-info/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       79 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       72 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1368 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       11 2023-05-11 12:11:45.000000 tap-impact-1.0.1/tap_impact.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       59 2023-05-11 12:11:46.000000 tap-impact-1.0.1/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      329 2023-05-11 12:11:46.000000 tap-impact-1.0.1/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      828 2023-05-11 12:10:50.000000 tap-impact-1.0.1/setup.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    34523 2023-05-11 12:09:24.000000 tap-impact-1.0.1/LICENSE
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    19254 2023-05-11 12:09:24.000000 tap-impact-1.0.1/README.md
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `tap-impact-1.0.0/LICENSE` & `tap-impact-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/README.md` & `tap-impact-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/setup.py` & `tap-impact-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 setup(name='tap-impact',
-      version='1.0.0',
+      version='1.0.1',
       description='Singer.io tap for extracting data from the Impact Advertiser, Partner, Agency APIs',
       author='jeff.huth@bytecode.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_impact'],
       install_requires=[
           'backoff==1.8.0',
           'requests==2.22.0',
           'singer-python==5.8.1'
       ],
       extras_require={
           'dev': [
-              'ipdb==0.11',
+              'ipdb',
               'pylint==2.5.3'
           ]
       },
       entry_points='''
           [console_scripts]
           tap-impact=tap_impact:main
       ''',
```

### Comparing `tap-impact-1.0.0/tap_impact/__init__.py` & `tap-impact-1.0.1/tap_impact/__init__.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/client.py` & `tap-impact-1.0.1/tap_impact/client.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/discover.py` & `tap-impact-1.0.1/tap_impact/discover.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schema.py` & `tap-impact-1.0.1/tap_impact/schema.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/action_inquiries.json` & `tap-impact-1.0.1/tap_impact/schemas/action_inquiries.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/action_updates.json` & `tap-impact-1.0.1/tap_impact/schemas/action_updates.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/actions.json` & `tap-impact-1.0.1/tap_impact/schemas/actions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/ads.json` & `tap-impact-1.0.1/tap_impact/schemas/ads.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/api_submissions.json` & `tap-impact-1.0.1/tap_impact/schemas/api_submissions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/campaigns.json` & `tap-impact-1.0.1/tap_impact/schemas/campaigns.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/catalog_items.json` & `tap-impact-1.0.1/tap_impact/schemas/catalog_items.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/catalogs.json` & `tap-impact-1.0.1/tap_impact/schemas/catalogs.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/clicks.json` & `tap-impact-1.0.1/tap_impact/schemas/clicks.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/company_information.json` & `tap-impact-1.0.1/tap_impact/schemas/company_information.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/contacts.json` & `tap-impact-1.0.1/tap_impact/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/conversion_paths.json` & `tap-impact-1.0.1/tap_impact/schemas/conversion_paths.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/deals.json` & `tap-impact-1.0.1/tap_impact/schemas/deals.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/exception_lists.json` & `tap-impact-1.0.1/tap_impact/schemas/exception_lists.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/ftp_file_submissions.json` & `tap-impact-1.0.1/tap_impact/schemas/ftp_file_submissions.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/invoices.json` & `tap-impact-1.0.1/tap_impact/schemas/invoices.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/media_partner_groups.json` & `tap-impact-1.0.1/tap_impact/schemas/media_partner_groups.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/media_partners.json` & `tap-impact-1.0.1/tap_impact/schemas/media_partners.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/notes.json` & `tap-impact-1.0.1/tap_impact/schemas/notes.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/phone_numbers.json` & `tap-impact-1.0.1/tap_impact/schemas/phone_numbers.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/promo_codes.json` & `tap-impact-1.0.1/tap_impact/schemas/promo_codes.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/report_metadata.json` & `tap-impact-1.0.1/tap_impact/schemas/report_metadata.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/tracking_value_requests.json` & `tap-impact-1.0.1/tap_impact/schemas/tracking_value_requests.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/schemas/unique_urls.json` & `tap-impact-1.0.1/tap_impact/schemas/unique_urls.json`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/streams.py` & `tap-impact-1.0.1/tap_impact/streams.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact/sync.py` & `tap-impact-1.0.1/tap_impact/sync.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,18 +283,18 @@
                 stream_name, record_count))
 
             # Loop thru parent batch records for each children objects (if should stream)
             children = endpoint_config.get('children')
             if children:
                 for child_stream_name, child_endpoint_config in children.items():
                     if child_stream_name in selected_streams:
-                        model_id = config.get('model_id', '')
+                        model_id = config.get('model_id')
                         process_child = True
                         # conversion_paths endpoint requires model_id tap config param
-                        if child_stream_name == 'conversion_paths' and model_id == '':
+                        if child_stream_name == 'conversion_paths' and not model_id:
                             process_child = False
                         if process_child:
                             write_schema(catalog, child_stream_name)
                             # For each parent record
                             for record in transformed_data:
                                 i = 0
                                 # Set parent_id
```

### Comparing `tap-impact-1.0.0/tap_impact/transform.py` & `tap-impact-1.0.1/tap_impact/transform.py`

 * *Files identical despite different names*

### Comparing `tap-impact-1.0.0/tap_impact.egg-info/SOURCES.txt` & `tap-impact-1.0.1/tap_impact.egg-info/SOURCES.txt`

 * *Files identical despite different names*

