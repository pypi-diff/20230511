# Comparing `tmp/tutor-mfe-15.0.5.tar.gz` & `tmp/tutor-mfe-15.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tutor-mfe-15.0.5.tar", last modified: Thu Jan 26 09:22:15 2023, max compression
+gzip compressed data, was "dist/tutor-mfe-15.0.6.tar", last modified: Thu May 11 13:02:07 2023, max compression
```

## Comparing `tutor-mfe-15.0.5.tar` & `tutor-mfe-15.0.6.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/
--rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/MANIFEST.in
--rw-r--r--   0 ci        (1000) ci        (1000)    15243 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)    14207 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/README.rst
--rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/setup.cfg
--rw-r--r--   0 ci        (1000) ci        (1000)     1849 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/setup.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/
--rw-r--r--   0 ci        (1000) ci        (1000)    15243 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/PKG-INFO
--rw-r--r--   0 ci        (1000) ci        (1000)     1162 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/SOURCES.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/dependency_links.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/entry_points.txt
--rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/requires.txt
--rw-r--r--   0 ci        (1000) ci        (1000)        9 2023-01-26 09:22:14.000000 tutor-mfe-15.0.5/tutor_mfe.egg-info/top_level.txt
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/
--rw-r--r--   0 ci        (1000) ci        (1000)       24 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/__about__.py
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/__init__.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/patches/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/.gitignore
--rw-r--r--   0 ci        (1000) ci        (1000)      333 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      605 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/k8s-deployments
--rw-r--r--   0 ci        (1000) ci        (1000)      168 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/k8s-services
--rw-r--r--   0 ci        (1000) ci        (1000)      130 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/kustomization-configmapgenerator
--rw-r--r--   0 ci        (1000) ci        (1000)      460 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/local-docker-compose-dev-services
--rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/local-docker-compose-prod-services
--rw-r--r--   0 ci        (1000) ci        (1000)      476 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/openedx-cms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/openedx-cms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)      356 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/openedx-lms-common-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3124 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/openedx-lms-development-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     3615 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/patches/openedx-lms-production-settings
--rw-r--r--   0 ci        (1000) ci        (1000)     5356 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/plugin.py
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)      629 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/mfe/Caddyfile
--rw-r--r--   0 ci        (1000) ci        (1000)      749 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/
--rw-r--r--   0 ci        (1000) ci        (1000)     3660 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/Dockerfile
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/i18n/
--rwxr-xr-x   0 ci        (1000) ci        (1000)     1489 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/tasks/
--rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/tasks/.gitignore
-drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-01-26 09:22:15.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/tasks/lms/
--rw-r--r--   0 ci        (1000) ci        (1000)     3717 2023-01-26 09:22:04.000000 tutor-mfe-15.0.5/tutormfe/templates/mfe/tasks/lms/init
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/
+-rw-r--r--   0 ci        (1000) ci        (1000)    34523 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/LICENSE.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       76 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/MANIFEST.in
+-rw-r--r--   0 ci        (1000) ci        (1000)    15467 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)    14405 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/README.rst
+-rw-r--r--   0 ci        (1000) ci        (1000)       38 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/setup.cfg
+-rw-r--r--   0 ci        (1000) ci        (1000)     1849 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/setup.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/
+-rw-r--r--   0 ci        (1000) ci        (1000)    15467 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/PKG-INFO
+-rw-r--r--   0 ci        (1000) ci        (1000)     1174 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/SOURCES.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        1 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/dependency_links.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       40 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/entry_points.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)       22 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/requires.txt
+-rw-r--r--   0 ci        (1000) ci        (1000)        9 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutor_mfe.egg-info/top_level.txt
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)       24 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/__about__.py
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/__init__.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/patches/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/.gitignore
+-rw-r--r--   0 ci        (1000) ci        (1000)      333 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      605 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/k8s-deployments
+-rw-r--r--   0 ci        (1000) ci        (1000)      168 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/k8s-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      130 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/kustomization-configmapgenerator
+-rw-r--r--   0 ci        (1000) ci        (1000)      460 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/local-docker-compose-dev-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      184 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/local-docker-compose-prod-services
+-rw-r--r--   0 ci        (1000) ci        (1000)      476 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-cms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      405 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-cms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)      356 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-common-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3124 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-development-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     3615 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-production-settings
+-rw-r--r--   0 ci        (1000) ci        (1000)     5356 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/plugin.py
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)      629 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/Caddyfile
+-rw-r--r--   0 ci        (1000) ci        (1000)      749 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3700 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/Dockerfile
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/
+-rwxr-xr-x   0 ci        (1000) ci        (1000)     1489 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/
+-rw-r--r--   0 ci        (1000) ci        (1000)        0 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/.gitignore
+drwxr-xr-x   0 ci        (1000) ci        (1000)        0 2023-05-11 13:02:07.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/
+-rw-r--r--   0 ci        (1000) ci        (1000)     3717 2023-05-11 13:01:55.000000 tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/init
```

### Comparing `tutor-mfe-15.0.5/PKG-INFO` & `tutor-mfe-15.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.5
+Version: 15.0.6
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 Micro Frontend base plugin for `Tutor <https://docs.tutor.overhang.io>`__
 =========================================================================
 
 This plugin makes it possible to easily add micro frontend (MFE) applications on top of an Open edX platform that runs with Tutor. To learn more about MFEs, please check the `official Open edX documentation <https://edx.readthedocs.io/projects/edx-developer-docs/en/latest/developers_guide/micro_frontends_in_open_edx.html>`__.
 
 In addition, this plugin comes with a few MFEs which are enabled by default:
@@ -134,15 +135,15 @@
                 "repository": "https://github.com/myorg/mymfe",
                 "port": 2001,
                 "version": "me/my-custom-branch", # optional
             }
         }
     }
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with `tutor images build mfe`. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
 
     tutor config save --set MFE_ACCOUNT_MFE_APP=null
@@ -181,33 +182,35 @@
 ~~~~~~~~~~~~~~~~
 
 To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
-    hooks.Filters.ENV_PATCHES.add_item(
-        (
-            "openedx-lms-development-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
-        (
-            "openedx-lms-production-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
+    hooks.Filters.ENV_PATCHES.add_items(
+        [
+            (
+                "openedx-lms-development-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+            (
+                "openedx-lms-production-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+        ]
     )
 
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
@@ -328,8 +331,8 @@
 ---------------
 
 This Tutor plugin is maintained by Adolfo Brandes from `tCRIL <https://openedx.org>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
-This software is licensed under the terms of the AGPLv3.
+This software is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-mfe/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-mfe-15.0.5/README.rst` & `tutor-mfe-15.0.6/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -108,15 +108,15 @@
                 "repository": "https://github.com/myorg/mymfe",
                 "port": 2001,
                 "version": "me/my-custom-branch", # optional
             }
         }
     }
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with `tutor images build mfe`. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
 
     tutor config save --set MFE_ACCOUNT_MFE_APP=null
@@ -155,33 +155,35 @@
 ~~~~~~~~~~~~~~~~
 
 To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
-    hooks.Filters.ENV_PATCHES.add_item(
-        (
-            "openedx-lms-development-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
-        (
-            "openedx-lms-production-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
+    hooks.Filters.ENV_PATCHES.add_items(
+        [
+            (
+                "openedx-lms-development-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+            (
+                "openedx-lms-production-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+        ]
     )
 
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
@@ -302,8 +304,8 @@
 ---------------
 
 This Tutor plugin is maintained by Adolfo Brandes from `tCRIL <https://openedx.org>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
-This software is licensed under the terms of the AGPLv3.
+This software is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-mfe/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-mfe-15.0.5/setup.py` & `tutor-mfe-15.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutor_mfe.egg-info/PKG-INFO` & `tutor-mfe-15.0.6/tutor_mfe.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tutor-mfe
-Version: 15.0.5
+Version: 15.0.6
 Summary: mfe plugin for Tutor
 Home-page: https://github.com/overhangio/tutor-mfe
 Author: Overhang.IO
 Maintainer: tCRIL
 Maintainer-email: adolfo@tcril.org
 License: AGPLv3
 Project-URL: Code, https://github.com/overhangio/tutor-mfe
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.5
 Description-Content-Type: text/x-rst
+License-File: LICENSE.txt
 
 Micro Frontend base plugin for `Tutor <https://docs.tutor.overhang.io>`__
 =========================================================================
 
 This plugin makes it possible to easily add micro frontend (MFE) applications on top of an Open edX platform that runs with Tutor. To learn more about MFEs, please check the `official Open edX documentation <https://edx.readthedocs.io/projects/edx-developer-docs/en/latest/developers_guide/micro_frontends_in_open_edx.html>`__.
 
 In addition, this plugin comes with a few MFEs which are enabled by default:
@@ -134,15 +135,15 @@
                 "repository": "https://github.com/myorg/mymfe",
                 "port": 2001,
                 "version": "me/my-custom-branch", # optional
             }
         }
     }
 
-The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with `tutor images build mfe`. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
+The MFE assets will then be bundled in the "mfe" Docker image whenever it is rebuilt with ``tutor images build mfe``. Assets will be served at ``http(s)://{{ MFE_HOST }}/{{ MYMFE_MFE_APP["name"] }}``. Developers are free to add extra template patches to their plugins, as usual: for instance LMS setting patches to make sure that the LMS correctly connects to the MFEs.
 
 Disabling individual MFEs
 ~~~~~~~~~~~~~~~~~~~~~~~~~
 
 To disable an existing MFE, set its corresponding configuration setting to "null". For instance, to disable the MFEs that ship with this plugin::
 
     tutor config save --set MFE_ACCOUNT_MFE_APP=null
@@ -181,33 +182,35 @@
 ~~~~~~~~~~~~~~~~
 
 To change the MFEs logos from the default to your own logos, override the corresponding settings in the MFEs environment using patches `openedx-lms-production-settings` and `openedx-lms-development-settings`. For example, using the following plugin:
 ::
 
     from tutor import hooks
 
-    hooks.Filters.ENV_PATCHES.add_item(
-        (
-            "openedx-lms-development-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
-        (
-            "openedx-lms-production-settings",
-            """
-    MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
-    MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
-    MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
-    MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
-    """
-        ),
+    hooks.Filters.ENV_PATCHES.add_items(
+        [
+            (
+                "openedx-lms-development-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+            (
+                "openedx-lms-production-settings",
+                """
+        MFE_CONFIG["LOGO_URL"] = "<URL>/logo.svg"
+        MFE_CONFIG["LOGO_TRADEMARK_URL"] = "<URL>/logo-trademark.svg"
+        MFE_CONFIG["LOGO_WHITE_URL"] = "<URL>/logo-white.svg"
+        MFE_CONFIG["FAVICON_URL"] = "<URL>/favicon.ico"
+        """
+            ),
+        ]
     )
 
 To install custom components for the MFEs, such as the `header <https://github.com/openedx/frontend-component-header>`_ and `footer <https://github.com/openedx/frontend-component-footer>`_, override the components by adding a patch to ``mfe-dockerfile-post-npm-install`` in your plugin:
 ::
 
     from tutor import hooks
 
@@ -328,8 +331,8 @@
 ---------------
 
 This Tutor plugin is maintained by Adolfo Brandes from `tCRIL <https://openedx.org>`__. Community support is available from the official `Open edX forum <https://discuss.openedx.org>`__. Do you need help with this plugin? See the `troubleshooting <https://docs.tutor.overhang.io/troubleshooting.html>`__ section from the Tutor documentation.
 
 License
 -------
 
-This software is licensed under the terms of the AGPLv3.
+This software is licensed under the terms of the `GNU Affero General Public License (AGPL) <https://github.com/overhangio/tutor-mfe/blob/master/LICENSE.txt>`_.
```

### Comparing `tutor-mfe-15.0.5/tutor_mfe.egg-info/SOURCES.txt` & `tutor-mfe-15.0.6/tutor_mfe.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE.txt
 MANIFEST.in
 README.rst
 setup.py
 tutor_mfe.egg-info/PKG-INFO
 tutor_mfe.egg-info/SOURCES.txt
 tutor_mfe.egg-info/dependency_links.txt
 tutor_mfe.egg-info/entry_points.txt
```

### Comparing `tutor-mfe-15.0.5/tutormfe/patches/k8s-deployments` & `tutor-mfe-15.0.6/tutormfe/patches/k8s-deployments`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/patches/openedx-lms-development-settings` & `tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-development-settings`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/patches/openedx-lms-production-settings` & `tutor-mfe-15.0.6/tutormfe/patches/openedx-lms-production-settings`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/plugin.py` & `tutor-mfe-15.0.6/tutormfe/plugin.py`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/mfe/Caddyfile` & `tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/Caddyfile`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js` & `tutor-mfe-15.0.6/tutormfe/templates/mfe/apps/mfe/webpack.dev-tutor.config.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/Dockerfile` & `tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/Dockerfile`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 FROM docker.io/node:16.14-bullseye-slim AS base
 
 RUN apt update \
   && apt install -y git \
     # required for cwebp-bin
     gcc libgl1 libxi6 make \
-    # additionally required for gifsicle, mozjpeg, and optipng (on arm)
+    # required for gifsicle, mozjpeg, and optipng (on arm)
     autoconf libtool pkg-config zlib1g-dev \
-    # additionally required for node-sass (on arm)
-    python g++
+    # required for node-sass (on arm)
+    python g++ \
+    # required for image-webpack-loader (on arm)
+    libpng-dev
 
 RUN mkdir -p /openedx/app /openedx/env
 WORKDIR /openedx/app
 ENV PATH ./node_modules/.bin:${PATH}
 
 ######## i18n strings
 FROM base AS i18n
```

### Comparing `tutor-mfe-15.0.5/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js` & `tutor-mfe-15.0.6/tutormfe/templates/mfe/build/mfe/i18n/i18n-merge.js`

 * *Files identical despite different names*

### Comparing `tutor-mfe-15.0.5/tutormfe/templates/mfe/tasks/lms/init` & `tutor-mfe-15.0.6/tutormfe/templates/mfe/tasks/lms/init`

 * *Files identical despite different names*

