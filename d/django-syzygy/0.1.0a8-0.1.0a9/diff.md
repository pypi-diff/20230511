# Comparing `tmp/django-syzygy-0.1.0a8.tar.gz` & `tmp/django-syzygy-0.1.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-syzygy-0.1.0a8.tar", last modified: Thu Apr 29 00:35:43 2021, max compression
+gzip compressed data, was "dist/django-syzygy-0.1.0a9.tar", last modified: Fri May  7 15:28:58 2021, max compression
```

## Comparing `django-syzygy-0.1.0a8.tar` & `django-syzygy-0.1.0a9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/
--rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/LICENSE
--rwxr-xr-x   0 runner    (1001) docker     (121)     1249 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)      355 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      680 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8427 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/django_syzygy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5908 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8427 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/syzygy/
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/syzygy/management/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/syzygy/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)     8520 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/management/commands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/management/commands/makemigrations.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     8165 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/operations.py
--rw-r--r--   0 runner    (1001) docker     (121)      109 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)      401 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     5893 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/plan.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/syzygy/quorum/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:43.000000 django-syzygy-0.1.0a8/syzygy/quorum/backends/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/quorum/backends/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/quorum/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/quorum/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/quorum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      520 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8362 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/autodetector.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2021-04-29 00:35:29.000000 django-syzygy-0.1.0a8/syzygy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/
+-rw-r--r--   0 runner    (1001) docker     (121)     8433 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      355 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1059 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/syzygy/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9160 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/operations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13439 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/autodetector.py
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/syzygy/management/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/syzygy/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)     8750 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/management/commands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/management/commands/makemigrations.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      401 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2288 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)      520 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/syzygy/quorum/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/syzygy/quorum/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/quorum/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1966 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/quorum/backends/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/quorum/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1888 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/quorum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5893 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/plan.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1301 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/syzygy/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8433 2021-05-07 15:28:57.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      680 2021-05-07 15:28:58.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2021-05-07 15:28:57.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-07 15:28:57.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2021-05-07 15:28:57.000000 django-syzygy-0.1.0a9/django_syzygy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5914 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/README.rst
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1249 2021-05-07 15:28:42.000000 django-syzygy-0.1.0a9/setup.py
```

### Comparing `django-syzygy-0.1.0a8/LICENSE` & `django-syzygy-0.1.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/setup.py` & `django-syzygy-0.1.0a9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import find_packages, setup
 
 with open("README.rst") as file_:
     long_description = file_.read()
 
 setup(
     name="django-syzygy",
-    version="0.1.0a8",
+    version="0.1.0a9",
     description="",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/charettes/django-syzygy",
     author="Simon Charette",
     author_email="charette.s@gmail.com",
     install_requires=["Django>=2.2"],
```

### Comparing `django-syzygy-0.1.0a8/django_syzygy.egg-info/SOURCES.txt` & `django-syzygy-0.1.0a9/django_syzygy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/django_syzygy.egg-info/PKG-INFO` & `django-syzygy-0.1.0a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-syzygy
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: UNKNOWN
 Home-page: https://github.com/charettes/django-syzygy
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
 Description: django-syzygy
         =============
@@ -159,32 +159,32 @@
         To circumvent this limitation Syzygy introduces a ``--quorum <N:int>`` flag to the
         ``migrate`` command that allow clusters coordination to take place.
         
         When specified the ``migrate --quorum <N:int>`` command will wait for at least
         ``N`` number invocations of ``migrate`` for the planned migrations before proceeding
         with applying them once and blocking on all callers until the operation completes.
         
-        In order to use the ``--quorum`` feature you must configure the ``MIGRATE_QUORUM_BACKEND``
+        In order to use the ``--quorum`` feature you must configure the ``MIGRATION_QUORUM_BACKEND``
         setting to point to a quorum backend such as cache based one provided by Sygyzy
         
         .. code:: python
         
-            MIGRATE_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
+            MIGRATION_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
         
         or
         
         .. code:: python
         
             CACHES = {
                 ...,
                 'quorum': {
                     ...
                 },
             }
-            MIGRATE_QUORUM_BACKEND = {
+            MIGRATION_QUORUM_BACKEND = {
                 'backend': 'syzygy.quorum.backends.cache.CacheQuorum',
                 'alias': 'quorum',
             }
         
         .. note::
         
           In order for ``CacheQuorum`` to work properly in a distributed environment it
```

### Comparing `django-syzygy-0.1.0a8/README.rst` & `django-syzygy-0.1.0a9/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -151,32 +151,32 @@
 To circumvent this limitation Syzygy introduces a ``--quorum <N:int>`` flag to the
 ``migrate`` command that allow clusters coordination to take place.
 
 When specified the ``migrate --quorum <N:int>`` command will wait for at least
 ``N`` number invocations of ``migrate`` for the planned migrations before proceeding
 with applying them once and blocking on all callers until the operation completes.
 
-In order to use the ``--quorum`` feature you must configure the ``MIGRATE_QUORUM_BACKEND``
+In order to use the ``--quorum`` feature you must configure the ``MIGRATION_QUORUM_BACKEND``
 setting to point to a quorum backend such as cache based one provided by Sygyzy
 
 .. code:: python
 
-    MIGRATE_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
+    MIGRATION_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
 
 or
 
 .. code:: python
 
     CACHES = {
         ...,
         'quorum': {
             ...
         },
     }
-    MIGRATE_QUORUM_BACKEND = {
+    MIGRATION_QUORUM_BACKEND = {
         'backend': 'syzygy.quorum.backends.cache.CacheQuorum',
         'alias': 'quorum',
     }
 
 .. note::
 
   In order for ``CacheQuorum`` to work properly in a distributed environment it
```

### Comparing `django-syzygy-0.1.0a8/PKG-INFO` & `django-syzygy-0.1.0a9/django_syzygy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-syzygy
-Version: 0.1.0a8
+Version: 0.1.0a9
 Summary: UNKNOWN
 Home-page: https://github.com/charettes/django-syzygy
 Author: Simon Charette
 Author-email: charette.s@gmail.com
 License: MIT License
 Description: django-syzygy
         =============
@@ -159,32 +159,32 @@
         To circumvent this limitation Syzygy introduces a ``--quorum <N:int>`` flag to the
         ``migrate`` command that allow clusters coordination to take place.
         
         When specified the ``migrate --quorum <N:int>`` command will wait for at least
         ``N`` number invocations of ``migrate`` for the planned migrations before proceeding
         with applying them once and blocking on all callers until the operation completes.
         
-        In order to use the ``--quorum`` feature you must configure the ``MIGRATE_QUORUM_BACKEND``
+        In order to use the ``--quorum`` feature you must configure the ``MIGRATION_QUORUM_BACKEND``
         setting to point to a quorum backend such as cache based one provided by Sygyzy
         
         .. code:: python
         
-            MIGRATE_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
+            MIGRATION_QUORUM_BACKEND = 'syzygy.quorum.backends.cache.CacheQuorum'
         
         or
         
         .. code:: python
         
             CACHES = {
                 ...,
                 'quorum': {
                     ...
                 },
             }
-            MIGRATE_QUORUM_BACKEND = {
+            MIGRATION_QUORUM_BACKEND = {
                 'backend': 'syzygy.quorum.backends.cache.CacheQuorum',
                 'alias': 'quorum',
             }
         
         .. note::
         
           In order for ``CacheQuorum`` to work properly in a distributed environment it
```

### Comparing `django-syzygy-0.1.0a8/syzygy/checks.py` & `django-syzygy-0.1.0a9/syzygy/checks.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/syzygy/management/commands/migrate.py` & `django-syzygy-0.1.0a9/syzygy/management/commands/migrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,14 +148,21 @@
         started_at = time.monotonic()
         while not poll_quorum(namespace, quorum):
             if (time.monotonic() - started_at) > quorum_timeout:
                 raise RuntimeError("Migration plan quorum timeout")
             time.sleep(1)
         return time.monotonic() - started_at
 
+    def _join_or_poll_until_quorum(
+        self, namespace: str, quorum: int, quorum_timeout: int
+    ) -> float:
+        if join_quorum(namespace, quorum):
+            return 0
+        return self._poll_until_quorum(namespace, quorum, quorum_timeout)
+
     @contextmanager
     def _handle_quorum(
         self, quorum: int, quorum_timeout: int, options: dict
     ) -> Iterator[bool]:
         """
         Context manager that handles migration application quorum by only
         allowing a single caller to proceed with application and preventing
@@ -179,32 +186,34 @@
         post_namespace = f"post:{database}:{plan_hash}"
         if join_quorum(pre_namespace, quorum):
             if verbosity:
                 self.stdout.write(
                     "Reached pre-migrate quorum, proceeding with planned migrations..."
                 )
             yield True
-            join_quorum(post_namespace, quorum)
             if verbosity:
                 self.stdout.write("Waiting for post-migrate quorum...")
-            duration = self._poll_until_quorum(post_namespace, quorum, quorum_timeout)
+            duration = self._join_or_poll_until_quorum(
+                post_namespace, quorum, quorum_timeout
+            )
             if verbosity:
                 self.stdout.write(
                     f"Reached post-migrate quorum after {duration:.2f}s..."
                 )
             return
         yield False
         if verbosity:
             self.stdout.write("Waiting for pre-migrate quorum...")
         duration = self._poll_until_quorum(pre_namespace, quorum, quorum_timeout)
         if verbosity:
             self.stdout.write(f"Reached pre-migrate quorum after {duration:.2f}s...")
             self.stdout.write("Waiting for migrations to be applied by remote party...")
-        join_quorum(post_namespace, quorum)
-        duration = self._poll_until_quorum(post_namespace, quorum, quorum_timeout)
+        duration = self._join_or_poll_until_quorum(
+            post_namespace, quorum, quorum_timeout
+        )
         if verbosity:
             self.stdout.write(f"Reached post-migrate quorum after {duration:.2f}s...")
             self.stdout.write("Migrations applied by remote party")
         return
 
     def handle(  # type: ignore
         self,
```

### Comparing `django-syzygy-0.1.0a8/syzygy/management/commands/makemigrations.py` & `django-syzygy-0.1.0a9/syzygy/management/commands/makemigrations.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import partial
+
 from django.core.management.commands import makemigrations  # type: ignore
 
 from syzygy.autodetector import MigrationAutodetector
 
 
 class Command(makemigrations.Command):
     def add_arguments(self, parser):
@@ -17,12 +19,14 @@
 
     def handle(self, *args, disable_syzygy, **options):
         if disable_syzygy:
             return super().handle(*args, **options)
         # Monkey-patch makemigrations.MigrationAutodetector since the command
         # doesn't allow it to be overridden in any other way.
         MigrationAutodetector_ = makemigrations.MigrationAutodetector
-        makemigrations.MigrationAutodetector = MigrationAutodetector
+        makemigrations.MigrationAutodetector = partial(
+            MigrationAutodetector, style=self.style
+        )
         try:
             super().handle(*args, **options)
         finally:
             makemigrations.MigrationAutodetector = MigrationAutodetector_
```

### Comparing `django-syzygy-0.1.0a8/syzygy/conf.py` & `django-syzygy-0.1.0a9/syzygy/conf.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/syzygy/operations.py` & `django-syzygy-0.1.0a9/syzygy/operations.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from contextlib import contextmanager
 
-from django.db import migrations
+from django.db.migrations import operations
 from django.db.models.fields import NOT_PROVIDED
 
 from .constants import Stage
 
 
 def _alter_field_db_default_sql_params(schema_editor, model, name, drop=False):
     field = model._meta.get_field(name)
@@ -57,15 +57,15 @@
     try:
         with _force_field_alteration(schema_editor):
             yield
     finally:
         schema_editor.column_sql = column_sql_
 
 
-class PreRemoveField(migrations.AlterField):
+class PreRemoveField(operations.AlterField):
     """
     Perform database operations required to make sure an application with a
     rolling deployment won't crash prior to a field removal.
 
     If the field has a `default` value defined its corresponding column is
     altered to use it until the field is removed otherwise the field is made
     NULL'able if it's not already.
@@ -91,15 +91,15 @@
                         app_label, schema_editor, from_state, to_state
                     )
             else:
                 _alter_field_db_default(schema_editor, model, self.name)
         else:
             nullable_field = field.clone()
             nullable_field.null = True
-            operation = migrations.AlterField(
+            operation = operations.AlterField(
                 self.model_name, self.name, nullable_field
             )
             operation.state_forwards(app_label, to_state)
             operation.database_forwards(app_label, schema_editor, from_state, to_state)
 
     @property
     def migration_name_fragment(self):
@@ -118,15 +118,15 @@
             return "Set database DEFAULT of field %s on %s" % (
                 self.name,
                 self.model_name,
             )
         return "Set field %s of %s NULLable" % (self.name, self.model_name)
 
 
-class AddField(migrations.AddField):
+class AddField(operations.AddField):
     """
     Subclass of `AddField` that preserves the database default on database
     application.
     """
 
     @contextmanager
     def _prevent_drop_default(self, schema_editor, model):
@@ -163,15 +163,15 @@
         # Defer the removal of DEFAUT to `PostAddField`
         with self._preserve_column_default(schema_editor, model):
             return super().database_forwards(
                 app_label, schema_editor, from_state, to_state
             )
 
 
-class PostAddField(migrations.AlterField):
+class PostAddField(operations.AlterField):
     """
     Elidable operation that drops a previously preserved database default.
     """
 
     stage = Stage.POST_DEPLOY
 
     def state_forwards(self, app_label, state):
@@ -212,7 +212,40 @@
         )
 
     def describe(self):
         return "Drop database DEFAULT of field %s on %s" % (
             self.name,
             self.model_name,
         )
+
+
+class StagedOperation(operations.base.Operation):
+    stage: Stage
+
+    def __init__(self, *args, **kwargs):
+        self.stage = kwargs.pop("stage")
+        super().__init__(*args, **kwargs)
+
+    @classmethod
+    def for_stage(cls, operation: operations.base.Operation, stage: Stage):
+        _, args, kwargs = operation.deconstruct()
+        kwargs["stage"] = stage
+        return cls(*args, **kwargs)
+
+    def deconstruct(self):
+        name, args, kwargs = super().deconstruct()
+        kwargs["stage"] = self.stage
+        return name, args, kwargs
+
+
+class RenameField(StagedOperation, operations.RenameField):
+    """
+    Subclass of ``RenameField`` that explicitly defines a stage for the rare
+    instances where a rename operation is safe to perform.
+    """
+
+
+class RenameModel(StagedOperation, operations.RenameModel):
+    """
+    Subclass of ``RenameModel`` that explicitly defines a stage for the rare
+    instances where a rename operation is safe to perform.
+    """
```

### Comparing `django-syzygy-0.1.0a8/syzygy/plan.py` & `django-syzygy-0.1.0a9/syzygy/plan.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/syzygy/quorum/__init__.py` & `django-syzygy-0.1.0a9/syzygy/quorum/__init__.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/syzygy/compat.py` & `django-syzygy-0.1.0a9/syzygy/compat.py`

 * *Files identical despite different names*

### Comparing `django-syzygy-0.1.0a8/syzygy/autodetector.py` & `django-syzygy-0.1.0a9/syzygy/autodetector.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,20 +7,27 @@
 )
 from django.db.migrations.operations.base import Operation
 from django.db.migrations.questioner import InteractiveMigrationQuestioner
 from django.db.models.fields import NOT_PROVIDED
 from django.utils.functional import cached_property
 
 from .compat import get_model_state_field
+from .constants import Stage
 from .exceptions import AmbiguousStage
-from .operations import AddField, PostAddField, PreRemoveField
+from .operations import (
+    AddField,
+    PostAddField,
+    PreRemoveField,
+    RenameField,
+    RenameModel,
+)
 from .plan import partition_operations
 
 
-class Stage(Operation):
+class OperationStage(Operation):
     """
     Fake operation that serves as a placeholder to break operations into
     multiple migrations.
     """
 
 
 class MigrationAutodetector(_MigrationAutodetector):
@@ -31,39 +38,132 @@
     It works by inserting fake `Stage` operations into a fake __stage__
     application since `_build_migration_list` will only split operations of a
     single application into multiple migrations if it has external
     dependencies.
 
     By creating a chain of external application dependencies between operations::
 
-        app.FirstOperation -> __stage__.Stage -> app.SecondOperation
+        app.FirstOperation -> __stage__.OperationStage -> app.SecondOperation
 
     The auto-detector will generate a sequence of migrations of the form::
 
         app.Migration1(operations=[FirstOperation])
-        __stage__.Migration1(operations=[Stage])
+        __stage__.Migration1(operations=[OperationStage])
         app.Migration2(operations=[FirstOperation])
 
     And automatically remove the __stage__ migrations since it's a not
     an existing application.
     """
 
     STAGE_SPLIT = "__stage__"
 
+    def __init__(self, *args, **kwargs):
+        self.style = kwargs.pop("style", None)
+        super().__init__(*args, **kwargs)
+
     @cached_property
     def has_interactive_questionner(self) -> bool:
         return not self.questioner.dry_run and isinstance(
             self.questioner, InteractiveMigrationQuestioner
         )
 
+    def add_operation(self, app_label, operation, dependencies=None, beginning=False):
+        if isinstance(operation, operations.RenameField):
+            print(
+                self.style.WARNING(
+                    "Renaming a column from a database table actively relied upon might cause downtime "
+                    "during deployment.",
+                ),
+                file=sys.stderr,
+            )
+            choice = self.questioner.defaults.get("ask_rename_field_stage", 0)
+            if self.has_interactive_questionner:
+                choice = self.questioner._choice_input(
+                    "Please choose an appropriate action to take:",
+                    [
+                        (
+                            f"Quit, and let me add a new {operation.model_name}.{operation.new_name} field meant "
+                            f"to be backfilled with {operation.model_name}.{operation.old_name} values"
+                        ),
+                        (
+                            f"Assume the currently deployed code doesn't reference {app_label}.{operation.model_name} "
+                            f"on reachable code paths and mark the operation to be applied before deployment. "
+                            + self.style.MIGRATE_LABEL(
+                                "This might cause downtime if your assumption is wrong",
+                            )
+                        ),
+                        (
+                            f"Assume the newly deployed code doesn't reference {app_label}.{operation.model_name} on "
+                            "reachable code paths and mark the operation to be applied after deployment. "
+                            + self.style.MIGRATE_LABEL(
+                                "This might cause downtime if your assumption is wrong",
+                            )
+                        ),
+                    ],
+                )
+            if choice == 0:
+                sys.exit(3)
+            else:
+                stage = Stage.PRE_DEPLOY if choice == 1 else Stage.POST_DEPLOY
+                operation = RenameField.for_stage(operation, stage)
+        if isinstance(operation, operations.RenameModel):
+            from_db_table = (
+                self.from_state.models[app_label, operation.old_name_lower].options.get(
+                    "db_table"
+                )
+                or f"{app_label}_{operation.old_name_lower}"
+            )
+            to_db_table = self.to_state.models[
+                app_label, operation.new_name_lower
+            ].options.get("db_table")
+            if from_db_table != to_db_table:
+                print(
+                    self.style.WARNING(
+                        "Renaming an actively relied on database table might cause downtime during deployment."
+                    ),
+                    file=sys.stderr,
+                )
+                choice = self.questioner.defaults.get("ask_rename_model_stage", 0)
+                if self.has_interactive_questionner:
+                    choice = self.questioner._choice_input(
+                        "Please choose an appropriate action to take:",
+                        [
+                            (
+                                f"Quit, and let me manually set {app_label}.{operation.new_name}.Meta.db_table to "
+                                f'"{from_db_table}" to avoid renaming its underlying table'
+                            ),
+                            (
+                                f"Assume the currently deployed code doesn't reference "
+                                f"{app_label}.{operation.old_name} on reachable code paths and mark the operation to "
+                                "be applied before the deployment. "
+                                + self.style.MIGRATE_LABEL(
+                                    "This might cause downtime if your assumption is wrong",
+                                )
+                            ),
+                            (
+                                f"Assume the newly deployed code doesn't reference {app_label}.{operation.new_name} "
+                                "on reachable code paths and mark the operation to be applied after the deployment. "
+                                + self.style.MIGRATE_LABEL(
+                                    "This might cause downtime if your assumption is wrong",
+                                )
+                            ),
+                        ],
+                    )
+                if choice == 0:
+                    sys.exit(3)
+                else:
+                    stage = Stage.PRE_DEPLOY if choice == 1 else Stage.POST_DEPLOY
+                    operation = RenameModel.for_stage(operation, stage)
+        super().add_operation(app_label, operation, dependencies, beginning)
+
     def _generate_added_field(self, app_label, model_name, field_name):
         super()._generate_added_field(app_label, model_name, field_name)
         add_field = self.generated_operations[app_label][-1]
         add_field.__class__ = AddField
-        stage = Stage()
+        stage = OperationStage()
         self.add_operation(
             self.STAGE_SPLIT,
             stage,
             dependencies=[(app_label, self.STAGE_SPLIT, add_field)],
         )
         post_add_field = PostAddField(
             model_name=model_name, name=field_name, field=add_field.field
@@ -112,15 +212,15 @@
             if remove_default is not NOT_PROVIDED:
                 field = field.clone()
                 field.default = remove_default
         pre_remove_field = PreRemoveField(
             model_name=model_name, name=field_name, field=field
         )
         self.add_operation(app_label, pre_remove_field)
-        stage = Stage()
+        stage = OperationStage()
         self.add_operation(
             self.STAGE_SPLIT,
             stage,
             dependencies=[
                 (app_label, self.STAGE_SPLIT, self.generated_operations[app_label][-1])
             ],
         )
@@ -179,15 +279,15 @@
                             ),
                         ],
                     )
                     if not choice:
                         sys.exit(3)
                 continue
             if pre_operations and post_operations:
-                stage = Stage()
+                stage = OperationStage()
                 self.add_operation(
                     self.STAGE_SPLIT,
                     stage,
                     dependencies=[(app_label, self.STAGE_SPLIT, pre_operations[-1])],
                 )
                 post_operations[0]._auto_deps.append((self.STAGE_SPLIT, stage))
                 # Assign updated operations as they might have be re-ordered by
```

