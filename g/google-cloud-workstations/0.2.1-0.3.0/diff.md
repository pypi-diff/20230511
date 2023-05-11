# Comparing `tmp/google-cloud-workstations-0.2.1.tar.gz` & `tmp/google-cloud-workstations-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-workstations-0.2.1.tar", last modified: Tue Apr 11 16:32:42 2023, max compression
+gzip compressed data, was "google-cloud-workstations-0.3.0.tar", last modified: Thu May 11 18:37:01 2023, max compression
```

## Comparing `google-cloud-workstations-0.2.1.tar` & `google-cloud-workstations-0.3.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4600 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3682 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/workstations/
--rw-rw-r--   0 root         (0)     1003     3048 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.467257 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/
--rw-rw-r--   0 root         (0)     1003     2904 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     8908 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129387 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   140606 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27340 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20457 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    42986 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43817 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142624 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54336 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003     2908 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003     8916 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      653 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       86 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.471258 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/
--rw-rw-r--   0 root         (0)     1003      761 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/__init__.py
--rw-rw-r--   0 root         (0)     1003   129831 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/async_client.py
--rw-rw-r--   0 root         (0)     1003   141050 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/client.py
--rw-rw-r--   0 root         (0)     1003    27504 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20465 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py
--rw-rw-r--   0 root         (0)     1003    43078 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    43909 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   142768 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/
--rw-rw-r--   0 root         (0)     1003     2643 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    54080 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/
--rw-r--r--   0 root         (0)     1003     4600 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     2717 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      352 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-11 16:32:42.000000 google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2994 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.475259 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   567497 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/test_workstations.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-11 16:32:42.479260 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/
--rw-rw-r--   0 root         (0)     1003      600 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/__init__.py
--rw-rw-r--   0 root         (0)     1003   567385 2023-04-11 16:30:19.000000 google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4600 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3682 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.395266 google-cloud-workstations-0.3.0/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.395266 google-cloud-workstations-0.3.0/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations/
+-rw-rw-r--   0 root         (0)     1003     3048 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003     2904 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8908 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129566 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   140785 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27340 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20457 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43040 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43871 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142624 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.399266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    55514 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003     2908 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8916 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      653 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       86 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/
+-rw-rw-r--   0 root         (0)     1003      761 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/__init__.py
+-rw-rw-r--   0 root         (0)     1003   129831 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/async_client.py
+-rw-rw-r--   0 root         (0)     1003   141050 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/client.py
+-rw-rw-r--   0 root         (0)     1003    27504 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20465 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    43078 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    43909 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   142768 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.403266 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/
+-rw-rw-r--   0 root         (0)     1003     2643 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    54080 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/
+-rw-r--r--   0 root         (0)     1003     4600 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     2717 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-11 18:37:01.000000 google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2994 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   568245 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/test_workstations.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-11 18:37:01.407266 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/
+-rw-rw-r--   0 root         (0)     1003      600 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/__init__.py
+-rw-rw-r--   0 root         (0)     1003   567385 2023-05-11 18:34:19.000000 google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/test_workstations.py
```

### Comparing `google-cloud-workstations-0.2.1/LICENSE` & `google-cloud-workstations-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/MANIFEST.in` & `google-cloud-workstations-0.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/PKG-INFO` & `google-cloud-workstations-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.2.1/README.rst` & `google-cloud-workstations-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations/gapic_version.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_metadata.json` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/gapic_version.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/async_client.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -976,16 +976,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationConfigsAsyncPager:
-        r"""Returns all WorkstationConfigs in the specified
-        cluster.
+        r"""Returns all workstation configurations in the
+        specified cluster.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1277,15 +1277,17 @@
                 should not be set.
             workstation_config (:class:`google.cloud.workstations_v1.types.WorkstationConfig`):
                 Required. Config to create.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             workstation_config_id (:class:`str`):
-                Required. ID to use for the config.
+                Required. ID to use for the
+                workstation configuration.
+
                 This corresponds to the ``workstation_config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1404,15 +1406,16 @@
             workstation_config (:class:`google.cloud.workstations_v1.types.WorkstationConfig`):
                 Required. Config to update.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1526,16 +1529,16 @@
                 print(response)
 
         Args:
             request (Optional[Union[google.cloud.workstations_v1.types.DeleteWorkstationConfigRequest, dict]]):
                 The request object. Message for deleting a workstation
                 configuration.
             name (:class:`str`):
-                Required. Name of the config to
-                delete.
+                Required. Name of the workstation
+                configuration to delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1717,15 +1720,16 @@
         request: Optional[Union[workstations.ListWorkstationsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationsAsyncPager:
-        r"""Returns all Workstations using the specified config.
+        r"""Returns all Workstations using the specified
+        workstation configuration.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1840,16 +1844,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUsableWorkstationsAsyncPager:
-        r"""Returns all Workstations using the specified config
-        on which the caller has the
+        r"""Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
@@ -2142,15 +2146,16 @@
             workstation (:class:`google.cloud.workstations_v1.types.Workstation`):
                 Required. Workstation to update.
                 This corresponds to the ``workstation`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (:class:`google.protobuf.field_mask_pb2.FieldMask`):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/client.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1230,16 +1230,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationConfigsPager:
-        r"""Returns all WorkstationConfigs in the specified
-        cluster.
+        r"""Returns all workstation configurations in the
+        specified cluster.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -1515,15 +1515,17 @@
                 should not be set.
             workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
                 Required. Config to create.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             workstation_config_id (str):
-                Required. ID to use for the config.
+                Required. ID to use for the
+                workstation configuration.
+
                 This corresponds to the ``workstation_config_id`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
             metadata (Sequence[Tuple[str, str]]): Strings which should be
@@ -1644,15 +1646,16 @@
             workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
                 Required. Config to update.
                 This corresponds to the ``workstation_config`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1768,16 +1771,16 @@
                 print(response)
 
         Args:
             request (Union[google.cloud.workstations_v1.types.DeleteWorkstationConfigRequest, dict]):
                 The request object. Message for deleting a workstation
                 configuration.
             name (str):
-                Required. Name of the config to
-                delete.
+                Required. Name of the workstation
+                configuration to delete.
 
                 This corresponds to the ``name`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
@@ -1952,15 +1955,16 @@
         request: Optional[Union[workstations.ListWorkstationsRequest, dict]] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListWorkstationsPager:
-        r"""Returns all Workstations using the specified config.
+        r"""Returns all Workstations using the specified
+        workstation configuration.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
             # - It may require correct/in-range values for request initialization.
@@ -2066,16 +2070,16 @@
         ] = None,
         *,
         parent: Optional[str] = None,
         retry: OptionalRetry = gapic_v1.method.DEFAULT,
         timeout: Union[float, object] = gapic_v1.method.DEFAULT,
         metadata: Sequence[Tuple[str, str]] = (),
     ) -> pagers.ListUsableWorkstationsPager:
-        r"""Returns all Workstations using the specified config
-        on which the caller has the
+        r"""Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         .. code-block:: python
 
             # This snippet has been automatically generated and should be regarded as a
             # code template only.
             # It will require modifications to work:
@@ -2359,15 +2363,16 @@
             workstation (google.cloud.workstations_v1.types.Workstation):
                 Required. Workstation to update.
                 This corresponds to the ``workstation`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             update_mask (google.protobuf.field_mask_pb2.FieldMask):
                 Required. Mask specifying which
-                fields in the config should be updated.
+                fields in the workstation configuration
+                should be updated.
 
                 This corresponds to the ``update_mask`` field
                 on the ``request`` instance; if ``request`` is provided, this
                 should not be set.
             retry (google.api_core.retry.Retry): Designation of what errors, if any,
                 should be retried.
             timeout (float): The timeout for this request.
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/pagers.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/base.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,16 +422,16 @@
         self,
     ) -> Callable[
         [workstations.ListWorkstationConfigsRequest],
         workstations.ListWorkstationConfigsResponse,
     ]:
         r"""Return a callable for the list workstation configs method over gRPC.
 
-        Returns all WorkstationConfigs in the specified
-        cluster.
+        Returns all workstation configurations in the
+        specified cluster.
 
         Returns:
             Callable[[~.ListWorkstationConfigsRequest],
                     ~.ListWorkstationConfigsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -595,15 +595,16 @@
     def list_workstations(
         self,
     ) -> Callable[
         [workstations.ListWorkstationsRequest], workstations.ListWorkstationsResponse
     ]:
         r"""Return a callable for the list workstations method over gRPC.
 
-        Returns all Workstations using the specified config.
+        Returns all Workstations using the specified
+        workstation configuration.
 
         Returns:
             Callable[[~.ListWorkstationsRequest],
                     ~.ListWorkstationsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -624,16 +625,16 @@
         self,
     ) -> Callable[
         [workstations.ListUsableWorkstationsRequest],
         workstations.ListUsableWorkstationsResponse,
     ]:
         r"""Return a callable for the list usable workstations method over gRPC.
 
-        Returns all Workstations using the specified config
-        on which the caller has the
+        Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         Returns:
             Callable[[~.ListUsableWorkstationsRequest],
                     ~.ListUsableWorkstationsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/grpc_asyncio.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,16 +432,16 @@
         self,
     ) -> Callable[
         [workstations.ListWorkstationConfigsRequest],
         Awaitable[workstations.ListWorkstationConfigsResponse],
     ]:
         r"""Return a callable for the list workstation configs method over gRPC.
 
-        Returns all WorkstationConfigs in the specified
-        cluster.
+        Returns all workstation configurations in the
+        specified cluster.
 
         Returns:
             Callable[[~.ListWorkstationConfigsRequest],
                     Awaitable[~.ListWorkstationConfigsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -611,15 +611,16 @@
         self,
     ) -> Callable[
         [workstations.ListWorkstationsRequest],
         Awaitable[workstations.ListWorkstationsResponse],
     ]:
         r"""Return a callable for the list workstations method over gRPC.
 
-        Returns all Workstations using the specified config.
+        Returns all Workstations using the specified
+        workstation configuration.
 
         Returns:
             Callable[[~.ListWorkstationsRequest],
                     Awaitable[~.ListWorkstationsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
@@ -640,16 +641,16 @@
         self,
     ) -> Callable[
         [workstations.ListUsableWorkstationsRequest],
         Awaitable[workstations.ListUsableWorkstationsResponse],
     ]:
         r"""Return a callable for the list usable workstations method over gRPC.
 
-        Returns all Workstations using the specified config
-        on which the caller has the
+        Returns all workstations using the specified
+        workstation configuration on which the caller has the
         "workstations.workstations.use" permission.
 
         Returns:
             Callable[[~.ListUsableWorkstationsRequest],
                     Awaitable[~.ListUsableWorkstationsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/services/workstations/transports/rest.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1/types/workstations.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/workstations.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.workstations.v1",
+    package="google.cloud.workstations.v1beta",
     manifest={
         "WorkstationCluster",
         "WorkstationConfig",
         "Workstation",
         "GetWorkstationClusterRequest",
         "ListWorkstationClustersRequest",
         "ListWorkstationClustersResponse",
@@ -101,15 +101,15 @@
             in which instances associated with this cluster
             will be created.
         subnetwork (str):
             Immutable. Name of the Compute Engine
             subnetwork in which instances associated with
             this cluster will be created. Must be part of
             the subnetwork specified for this cluster.
-        private_cluster_config (google.cloud.workstations_v1.types.WorkstationCluster.PrivateClusterConfig):
+        private_cluster_config (google.cloud.workstations_v1beta.types.WorkstationCluster.PrivateClusterConfig):
             Configuration for private cluster.
         degraded (bool):
             Output only. Whether this resource is in degraded mode, in
             which case it may require user action to restore full
             functionality. Details can be found in the ``conditions``
             field.
         conditions (MutableSequence[google.rpc.status_pb2.Status]):
@@ -278,24 +278,24 @@
             Defaults to 20 minutes.
         running_timeout (google.protobuf.duration_pb2.Duration):
             How long to wait before automatically stopping a workstation
             after it started. A value of 0 indicates that workstations
             using this configuration should never time out. Must be
             greater than 0 and less than 24 hours if encryption_key is
             set. Defaults to 12 hours.
-        host (google.cloud.workstations_v1.types.WorkstationConfig.Host):
+        host (google.cloud.workstations_v1beta.types.WorkstationConfig.Host):
             Runtime host for the workstation.
-        persistent_directories (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory]):
+        persistent_directories (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory]):
             Directories to persist across workstation
             sessions.
-        container (google.cloud.workstations_v1.types.WorkstationConfig.Container):
+        container (google.cloud.workstations_v1beta.types.WorkstationConfig.Container):
             Container that will be run for each
             workstation using this configuration when that
             workstation is started.
-        encryption_key (google.cloud.workstations_v1.types.WorkstationConfig.CustomerEncryptionKey):
+        encryption_key (google.cloud.workstations_v1beta.types.WorkstationConfig.CustomerEncryptionKey):
             Encrypts resources of this workstation
             configuration using a customer-managed
             encryption key.
             If specified, the boot disk of the Compute
             Engine instance and the persistent disk are
             encrypted using this encryption key. If this
             field is not set, the disks are encrypted using
@@ -308,68 +308,66 @@
             Be sure to keep older versions of the key until
             the persistent disk is recreated. Otherwise,
             data on the persistent disk will be lost.
             If the encryption key is revoked, the
             workstation session will automatically be
             stopped within 7 hours.
         degraded (bool):
-            Output only. Whether this resource is degraded, in which
-            case it may require user action to restore full
-            functionality. See also the ``conditions`` field.
+            Output only. Whether this resource is in degraded mode, in
+            which case it may require user action to restore full
+            functionality. Details can be found in the ``conditions``
+            field.
         conditions (MutableSequence[google.rpc.status_pb2.Status]):
             Output only. Status conditions describing the
             current resource state.
     """
 
     class Host(proto.Message):
         r"""Runtime host for a workstation.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
-            gce_instance (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance):
+            gce_instance (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance):
                 Specifies a Compute Engine instance as the
                 host.
 
                 This field is a member of `oneof`_ ``config``.
         """
 
         class GceInstance(proto.Message):
             r"""A runtime using a Compute Engine instance.
 
             Attributes:
                 machine_type (str):
                     The name of a Compute Engine machine type.
                 service_account (str):
-                    Email address of the service account that
-                    will be used on VM instances used to support
-                    this config. If not set, VMs will run with a
-                    Google-managed service account. This service
-                    account must have permission to pull the
-                    specified container image, otherwise the image
-                    must be publicly accessible.
+                    Email address of the service account used on
+                    VM instances used to support this configuration.
+                    If not set, VMs run with a Google-managed
+                    service account. This service account must have
+                    permission to pull the specified container
+                    image; otherwise, the image must be publicly
+                    accessible.
                 tags (MutableSequence[str]):
                     Network tags to add to the Compute Engine
                     machines backing the Workstations.
                 pool_size (int):
                     Number of instances to pool for faster
                     workstation starup.
                 disable_public_ip_addresses (bool):
                     Whether instances have no public IP address.
-                enable_nested_virtualization (bool):
-                    Whether to enable nested virtualization on
-                    instances.
-                shielded_instance_config (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig):
+                shielded_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig):
                     A set of Compute Engine Shielded instance
                     options.
-                confidential_instance_config (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig):
+                confidential_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig):
                     A set of Compute Engine Confidential VM
                     instance options.
                 boot_disk_size_gb (int):
-                    Size of the boot disk in GB. Defaults to 50.
+                    Size of the boot disk in GB.
             """
 
             class GceShieldedInstanceConfig(proto.Message):
                 r"""A set of Compute Engine Shielded instance options.
 
                 Attributes:
                     enable_secure_boot (bool):
@@ -424,18 +422,14 @@
                 proto.INT32,
                 number=5,
             )
             disable_public_ip_addresses: bool = proto.Field(
                 proto.BOOL,
                 number=6,
             )
-            enable_nested_virtualization: bool = proto.Field(
-                proto.BOOL,
-                number=7,
-            )
             shielded_instance_config: "WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig" = proto.Field(
                 proto.MESSAGE,
                 number=8,
                 message="WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig",
             )
             confidential_instance_config: "WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig" = proto.Field(
                 proto.MESSAGE,
@@ -456,43 +450,42 @@
 
     class PersistentDirectory(proto.Message):
         r"""A directory to persist across workstation sessions.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
-            gce_pd (google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk):
+            mount_path (str):
+                Location of this directory in the running
+                workstation.
+            gce_pd (google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk):
                 A PersistentDirectory backed by a Compute
                 Engine persistent disk.
 
                 This field is a member of `oneof`_ ``directory_type``.
-            mount_path (str):
-                Location of this directory in the running
-                workstation.
         """
 
         class GceRegionalPersistentDisk(proto.Message):
             r"""A PersistentDirectory backed by a Compute Engine regional
             persistent disk.
 
             Attributes:
                 size_gb (int):
                     Size of the disk in GB. Must be empty if source_snapshot is
-                    set. Defaults to 200.
+                    set.
                 fs_type (str):
                     Type of file system that the disk should be formatted with.
                     The workstation image must support this file system type.
-                    Must be empty if source_snapshot is set. Defaults to ext4.
+                    Must be empty if source_snapshot is set.
                 disk_type (str):
-                    Type of the disk to use. Defaults to
-                    pd-standard.
+                    Type of the disk to use.
                 source_snapshot (str):
                     Name of the snapshot to use as the source for the disk. If
                     set, size_gb and fs_type must be empty.
-                reclaim_policy (google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy):
+                reclaim_policy (google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy):
                     What should happen to the disk after the
                     workstation is deleted. Defaults to DELETE.
             """
 
             class ReclaimPolicy(proto.Enum):
                 r"""Value representing what should happen to the disk after the
                 workstation is deleted.
@@ -530,24 +523,24 @@
             )
             reclaim_policy: "WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy" = proto.Field(
                 proto.ENUM,
                 number=4,
                 enum="WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy",
             )
 
+        mount_path: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
         gce_pd: "WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk" = proto.Field(
             proto.MESSAGE,
             number=2,
             oneof="directory_type",
             message="WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk",
         )
-        mount_path: str = proto.Field(
-            proto.STRING,
-            number=1,
-        )
 
     class Container(proto.Message):
         r"""A Docker container.
 
         Attributes:
             image (str):
                 Docker image defining the container. This
@@ -740,15 +733,15 @@
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
             on update and delete requests to ensure that the
             client has an up-to-date value before
             proceeding.
-        state (google.cloud.workstations_v1.types.Workstation.State):
+        state (google.cloud.workstations_v1beta.types.Workstation.State):
             Output only. Current state of the
             workstation.
         host (str):
             Output only. Host to which clients can send HTTPS traffic
             that will be received by the workstation. Authorized traffic
             will be received to the workstation as HTTP on port 80. To
             send traffic to a different port, clients may prefix the
@@ -878,15 +871,15 @@
     )
 
 
 class ListWorkstationClustersResponse(proto.Message):
     r"""Response message for ListWorkstationClusters.
 
     Attributes:
-        workstation_clusters (MutableSequence[google.cloud.workstations_v1.types.WorkstationCluster]):
+        workstation_clusters (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationCluster]):
             The requested workstation clusters.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -916,15 +909,15 @@
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_cluster_id (str):
             Required. ID to use for the workstation
             cluster.
-        workstation_cluster (google.cloud.workstations_v1.types.WorkstationCluster):
+        workstation_cluster (google.cloud.workstations_v1beta.types.WorkstationCluster):
             Required. Workstation cluster to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -946,15 +939,15 @@
     )
 
 
 class UpdateWorkstationClusterRequest(proto.Message):
     r"""Request message for UpdateWorkstationCluster.
 
     Attributes:
-        workstation_cluster (google.cloud.workstations_v1.types.WorkstationCluster):
+        workstation_cluster (google.cloud.workstations_v1beta.types.WorkstationCluster):
             Required. Workstation cluster to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask that specifies which fields in
             the workstation cluster should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
@@ -1065,15 +1058,15 @@
     )
 
 
 class ListWorkstationConfigsResponse(proto.Message):
     r"""Response message for ListWorkstationConfigs.
 
     Attributes:
-        workstation_configs (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig]):
+        workstation_configs (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig]):
             The requested configs.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1125,15 +1118,15 @@
     )
 
 
 class ListUsableWorkstationConfigsResponse(proto.Message):
     r"""Response message for ListUsableWorkstationConfigs.
 
     Attributes:
-        workstation_configs (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig]):
+        workstation_configs (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig]):
             The requested configs.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1162,15 +1155,15 @@
     r"""Message for creating a CreateWorkstationConfig.
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_config_id (str):
             Required. ID to use for the config.
-        workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
+        workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
             Required. Config to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -1192,15 +1185,15 @@
     )
 
 
 class UpdateWorkstationConfigRequest(proto.Message):
     r"""Request message for UpdateWorkstationConfig.
 
     Attributes:
-        workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
+        workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
             Required. Config to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
             config should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
@@ -1307,15 +1300,15 @@
     )
 
 
 class ListWorkstationsResponse(proto.Message):
     r"""Response message for ListWorkstations.
 
     Attributes:
-        workstations (MutableSequence[google.cloud.workstations_v1.types.Workstation]):
+        workstations (MutableSequence[google.cloud.workstations_v1beta.types.Workstation]):
             The requested workstations.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1367,15 +1360,15 @@
     )
 
 
 class ListUsableWorkstationsResponse(proto.Message):
     r"""Response message for ListUsableWorkstations.
 
     Attributes:
-        workstations (MutableSequence[google.cloud.workstations_v1.types.Workstation]):
+        workstations (MutableSequence[google.cloud.workstations_v1beta.types.Workstation]):
             The requested workstations.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1404,15 +1397,15 @@
     r"""Message for creating a CreateWorkstation.
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_id (str):
             Required. ID to use for the workstation.
-        workstation (google.cloud.workstations_v1.types.Workstation):
+        workstation (google.cloud.workstations_v1beta.types.Workstation):
             Required. Workstation to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -1434,15 +1427,15 @@
     )
 
 
 class UpdateWorkstationRequest(proto.Message):
     r"""Request message for UpdateWorkstation.
 
     Attributes:
-        workstation (google.cloud.workstations_v1.types.Workstation):
+        workstation (google.cloud.workstations_v1beta.types.Workstation):
             Required. Workstation to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
             config should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
@@ -1565,14 +1558,17 @@
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
+        workstation (str):
+            Required. Name of the workstation for which
+            the access token should be generated.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Desired expiration time of the access token.
             This value must be at most 24 hours in the
             future. If a value is not specified, the token's
             expiration time will be set to a default value
             of 1 hour in the future.
 
@@ -1580,35 +1576,32 @@
         ttl (google.protobuf.duration_pb2.Duration):
             Desired lifetime duration of the access
             token. This value must be at most 24 hours. If a
             value is not specified, the token's lifetime
             will be set to a default value of 1 hour.
 
             This field is a member of `oneof`_ ``expiration``.
-        workstation (str):
-            Required. Name of the workstation for which
-            the access token should be generated.
     """
 
+    workstation: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
     expire_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="expiration",
         message=timestamp_pb2.Timestamp,
     )
     ttl: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="expiration",
         message=duration_pb2.Duration,
     )
-    workstation: str = proto.Field(
-        proto.STRING,
-        number=1,
-    )
 
 
 class GenerateAccessTokenResponse(proto.Message):
     r"""Response message for GenerateAccessToken.
 
     Attributes:
         access_token (str):
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_metadata.json` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/gapic_version.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/gapic_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
-__version__ = "0.2.1"  # {x-release-please-version}
+__version__ = "0.3.0"  # {x-release-please-version}
```

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/async_client.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/client.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/pagers.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/base.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/services/workstations/transports/rest.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/services/workstations/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/__init__.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1beta/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/google/cloud/workstations_v1beta/types/workstations.py` & `google-cloud-workstations-0.3.0/google/cloud/workstations_v1/types/workstations.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from google.protobuf import duration_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 from google.rpc import status_pb2  # type: ignore
 import proto  # type: ignore
 
 __protobuf__ = proto.module(
-    package="google.cloud.workstations.v1beta",
+    package="google.cloud.workstations.v1",
     manifest={
         "WorkstationCluster",
         "WorkstationConfig",
         "Workstation",
         "GetWorkstationClusterRequest",
         "ListWorkstationClustersRequest",
         "ListWorkstationClustersResponse",
@@ -89,27 +89,34 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
         network (str):
             Immutable. Name of the Compute Engine network
             in which instances associated with this cluster
             will be created.
         subnetwork (str):
             Immutable. Name of the Compute Engine
             subnetwork in which instances associated with
             this cluster will be created. Must be part of
             the subnetwork specified for this cluster.
-        private_cluster_config (google.cloud.workstations_v1beta.types.WorkstationCluster.PrivateClusterConfig):
+        control_plane_ip (str):
+            Output only. The private IP address of the
+            control plane for this cluster. Workstation VMs
+            need access to this IP address to work with the
+            service, so make sure that your firewall rules
+            allow egress from the workstation VMs to this
+            address.
+        private_cluster_config (google.cloud.workstations_v1.types.WorkstationCluster.PrivateClusterConfig):
             Configuration for private cluster.
         degraded (bool):
             Output only. Whether this resource is in degraded mode, in
             which case it may require user action to restore full
             functionality. Details can be found in the ``conditions``
             field.
         conditions (MutableSequence[google.rpc.status_pb2.Status]):
@@ -213,14 +220,18 @@
         proto.STRING,
         number=10,
     )
     subnetwork: str = proto.Field(
         proto.STRING,
         number=11,
     )
+    control_plane_ip: str = proto.Field(
+        proto.STRING,
+        number=16,
+    )
     private_cluster_config: PrivateClusterConfig = proto.Field(
         proto.MESSAGE,
         number=12,
         message=PrivateClusterConfig,
     )
     degraded: bool = proto.Field(
         proto.BOOL,
@@ -263,42 +274,42 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
         idle_timeout (google.protobuf.duration_pb2.Duration):
             How long to wait before automatically
             stopping an instance that hasn't received any
             user traffic. A value of 0 indicates that this
             instance should never time out due to idleness.
             Defaults to 20 minutes.
         running_timeout (google.protobuf.duration_pb2.Duration):
             How long to wait before automatically stopping a workstation
             after it started. A value of 0 indicates that workstations
             using this configuration should never time out. Must be
             greater than 0 and less than 24 hours if encryption_key is
             set. Defaults to 12 hours.
-        host (google.cloud.workstations_v1beta.types.WorkstationConfig.Host):
+        host (google.cloud.workstations_v1.types.WorkstationConfig.Host):
             Runtime host for the workstation.
-        persistent_directories (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory]):
+        persistent_directories (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory]):
             Directories to persist across workstation
             sessions.
-        container (google.cloud.workstations_v1beta.types.WorkstationConfig.Container):
+        container (google.cloud.workstations_v1.types.WorkstationConfig.Container):
             Container that will be run for each
             workstation using this configuration when that
             workstation is started.
-        encryption_key (google.cloud.workstations_v1beta.types.WorkstationConfig.CustomerEncryptionKey):
-            Encrypts resources of this workstation
-            configuration using a customer-managed
-            encryption key.
+        encryption_key (google.cloud.workstations_v1.types.WorkstationConfig.CustomerEncryptionKey):
+            Immutable. Encrypts resources of this
+            workstation configuration using a
+            customer-managed encryption key.
             If specified, the boot disk of the Compute
             Engine instance and the persistent disk are
             encrypted using this encryption key. If this
             field is not set, the disks are encrypted using
             a generated key. Customer-managed encryption
             keys do not protect disk metadata.
             If the customer-managed encryption key is
@@ -307,31 +318,33 @@
             persistent disk with the new version of the key.
             Be sure to keep older versions of the key until
             the persistent disk is recreated. Otherwise,
             data on the persistent disk will be lost.
             If the encryption key is revoked, the
             workstation session will automatically be
             stopped within 7 hours.
+
+            Immutable after the workstation configuration is
+            created.
         degraded (bool):
-            Output only. Whether this resource is in degraded mode, in
-            which case it may require user action to restore full
-            functionality. Details can be found in the ``conditions``
-            field.
+            Output only. Whether this resource is degraded, in which
+            case it may require user action to restore full
+            functionality. See also the ``conditions`` field.
         conditions (MutableSequence[google.rpc.status_pb2.Status]):
             Output only. Status conditions describing the
             current resource state.
     """
 
     class Host(proto.Message):
         r"""Runtime host for a workstation.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
-            gce_instance (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance):
+            gce_instance (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance):
                 Specifies a Compute Engine instance as the
                 host.
 
                 This field is a member of `oneof`_ ``config``.
         """
 
         class GceInstance(proto.Message):
@@ -349,25 +362,32 @@
                     image; otherwise, the image must be publicly
                     accessible.
                 tags (MutableSequence[str]):
                     Network tags to add to the Compute Engine
                     machines backing the Workstations.
                 pool_size (int):
                     Number of instances to pool for faster
-                    workstation starup.
+                    workstation startup.
+                pooled_instances (int):
+                    Output only. Number of instances currently
+                    available in the pool for faster workstation
+                    startup.
                 disable_public_ip_addresses (bool):
                     Whether instances have no public IP address.
-                shielded_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig):
+                enable_nested_virtualization (bool):
+                    Whether to enable nested virtualization on
+                    instances.
+                shielded_instance_config (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig):
                     A set of Compute Engine Shielded instance
                     options.
-                confidential_instance_config (google.cloud.workstations_v1beta.types.WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig):
+                confidential_instance_config (google.cloud.workstations_v1.types.WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig):
                     A set of Compute Engine Confidential VM
                     instance options.
                 boot_disk_size_gb (int):
-                    Size of the boot disk in GB.
+                    Size of the boot disk in GB. Defaults to 50.
             """
 
             class GceShieldedInstanceConfig(proto.Message):
                 r"""A set of Compute Engine Shielded instance options.
 
                 Attributes:
                     enable_secure_boot (bool):
@@ -418,18 +438,26 @@
                 proto.STRING,
                 number=4,
             )
             pool_size: int = proto.Field(
                 proto.INT32,
                 number=5,
             )
+            pooled_instances: int = proto.Field(
+                proto.INT32,
+                number=12,
+            )
             disable_public_ip_addresses: bool = proto.Field(
                 proto.BOOL,
                 number=6,
             )
+            enable_nested_virtualization: bool = proto.Field(
+                proto.BOOL,
+                number=7,
+            )
             shielded_instance_config: "WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig" = proto.Field(
                 proto.MESSAGE,
                 number=8,
                 message="WorkstationConfig.Host.GceInstance.GceShieldedInstanceConfig",
             )
             confidential_instance_config: "WorkstationConfig.Host.GceInstance.GceConfidentialInstanceConfig" = proto.Field(
                 proto.MESSAGE,
@@ -450,42 +478,43 @@
 
     class PersistentDirectory(proto.Message):
         r"""A directory to persist across workstation sessions.
 
         .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
         Attributes:
-            mount_path (str):
-                Location of this directory in the running
-                workstation.
-            gce_pd (google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk):
+            gce_pd (google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk):
                 A PersistentDirectory backed by a Compute
                 Engine persistent disk.
 
                 This field is a member of `oneof`_ ``directory_type``.
+            mount_path (str):
+                Location of this directory in the running
+                workstation.
         """
 
         class GceRegionalPersistentDisk(proto.Message):
             r"""A PersistentDirectory backed by a Compute Engine regional
             persistent disk.
 
             Attributes:
                 size_gb (int):
                     Size of the disk in GB. Must be empty if source_snapshot is
-                    set.
+                    set. Defaults to 200.
                 fs_type (str):
                     Type of file system that the disk should be formatted with.
                     The workstation image must support this file system type.
-                    Must be empty if source_snapshot is set.
+                    Must be empty if source_snapshot is set. Defaults to ext4.
                 disk_type (str):
-                    Type of the disk to use.
+                    Type of the disk to use. Defaults to
+                    pd-standard.
                 source_snapshot (str):
                     Name of the snapshot to use as the source for the disk. If
                     set, size_gb and fs_type must be empty.
-                reclaim_policy (google.cloud.workstations_v1beta.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy):
+                reclaim_policy (google.cloud.workstations_v1.types.WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy):
                     What should happen to the disk after the
                     workstation is deleted. Defaults to DELETE.
             """
 
             class ReclaimPolicy(proto.Enum):
                 r"""Value representing what should happen to the disk after the
                 workstation is deleted.
@@ -523,41 +552,41 @@
             )
             reclaim_policy: "WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy" = proto.Field(
                 proto.ENUM,
                 number=4,
                 enum="WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk.ReclaimPolicy",
             )
 
-        mount_path: str = proto.Field(
-            proto.STRING,
-            number=1,
-        )
         gce_pd: "WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk" = proto.Field(
             proto.MESSAGE,
             number=2,
             oneof="directory_type",
             message="WorkstationConfig.PersistentDirectory.GceRegionalPersistentDisk",
         )
+        mount_path: str = proto.Field(
+            proto.STRING,
+            number=1,
+        )
 
     class Container(proto.Message):
         r"""A Docker container.
 
         Attributes:
             image (str):
                 Docker image defining the container. This
-                image must be accessible by the config's service
-                account.
+                image must be accessible by the service account
+                specified in the workstation configuration.
             command (MutableSequence[str]):
                 If set, overrides the default ENTRYPOINT
                 specified by the image.
             args (MutableSequence[str]):
                 Arguments passed to the entrypoint.
             env (MutableMapping[str, str]):
                 Environment variables passed to the
-                container.
+                container's entrypoint.
             working_dir (str):
                 If set, overrides the default DIR specified
                 by the image.
             run_as_user (int):
                 If set, overrides the USER specified in the
                 image with the given uid.
         """
@@ -590,21 +619,22 @@
 
     class CustomerEncryptionKey(proto.Message):
         r"""A customer-managed encryption key for the Compute Engine
         resources of this workstation configuration.
 
         Attributes:
             kms_key (str):
-                The name of the Google Cloud KMS encryption key. For
-                example,
+                Immutable. The name of the Google Cloud KMS encryption key.
+                For example,
                 ``projects/PROJECT_ID/locations/REGION/keyRings/KEY_RING/cryptoKeys/KEY_NAME``.
             kms_key_service_account (str):
-                The service account to use with the specified KMS key. We
-                recommend that you use a separate service account and follow
-                KMS best practices. For more information, see `Separation of
+                Immutable. The service account to use with the specified KMS
+                key. We recommend that you use a separate service account
+                and follow KMS best practices. For more information, see
+                `Separation of
                 duties <https://cloud.google.com/kms/docs/separation-of-duties>`__
                 and ``gcloud kms keys add-iam-policy-binding``
                 ```--member`` <https://cloud.google.com/sdk/gcloud/reference/kms/keys/add-iam-policy-binding#--member>`__.
         """
 
         kms_key: str = proto.Field(
             proto.STRING,
@@ -730,18 +760,18 @@
             Output only. Time when this resource was most
             recently updated.
         delete_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. Time when this resource was
             soft-deleted.
         etag (str):
             Checksum computed by the server. May be sent
-            on update and delete requests to ensure that the
-            client has an up-to-date value before
+            on update and delete requests to make sure that
+            the client has an up-to-date value before
             proceeding.
-        state (google.cloud.workstations_v1beta.types.Workstation.State):
+        state (google.cloud.workstations_v1.types.Workstation.State):
             Output only. Current state of the
             workstation.
         host (str):
             Output only. Host to which clients can send HTTPS traffic
             that will be received by the workstation. Authorized traffic
             will be received to the workstation as HTTP on port 80. To
             send traffic to a different port, clients may prefix the
@@ -871,15 +901,15 @@
     )
 
 
 class ListWorkstationClustersResponse(proto.Message):
     r"""Response message for ListWorkstationClusters.
 
     Attributes:
-        workstation_clusters (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationCluster]):
+        workstation_clusters (MutableSequence[google.cloud.workstations_v1.types.WorkstationCluster]):
             The requested workstation clusters.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -909,15 +939,15 @@
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_cluster_id (str):
             Required. ID to use for the workstation
             cluster.
-        workstation_cluster (google.cloud.workstations_v1beta.types.WorkstationCluster):
+        workstation_cluster (google.cloud.workstations_v1.types.WorkstationCluster):
             Required. Workstation cluster to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -939,15 +969,15 @@
     )
 
 
 class UpdateWorkstationClusterRequest(proto.Message):
     r"""Request message for UpdateWorkstationCluster.
 
     Attributes:
-        workstation_cluster (google.cloud.workstations_v1beta.types.WorkstationCluster):
+        workstation_cluster (google.cloud.workstations_v1.types.WorkstationCluster):
             Required. Workstation cluster to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask that specifies which fields in
             the workstation cluster should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
@@ -986,15 +1016,15 @@
             delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation cluster on the
-            server does not have this etag.
+            server does not have this ETag.
         force (bool):
             If set, any workstation configurations and
             workstations in the workstation cluster are also
             deleted. Otherwise, the request only works if
             the workstation cluster has no configurations or
             workstations.
     """
@@ -1058,15 +1088,15 @@
     )
 
 
 class ListWorkstationConfigsResponse(proto.Message):
     r"""Response message for ListWorkstationConfigs.
 
     Attributes:
-        workstation_configs (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig]):
+        workstation_configs (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig]):
             The requested configs.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1118,15 +1148,15 @@
     )
 
 
 class ListUsableWorkstationConfigsResponse(proto.Message):
     r"""Response message for ListUsableWorkstationConfigs.
 
     Attributes:
-        workstation_configs (MutableSequence[google.cloud.workstations_v1beta.types.WorkstationConfig]):
+        workstation_configs (MutableSequence[google.cloud.workstations_v1.types.WorkstationConfig]):
             The requested configs.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1154,16 +1184,17 @@
 class CreateWorkstationConfigRequest(proto.Message):
     r"""Message for creating a CreateWorkstationConfig.
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_config_id (str):
-            Required. ID to use for the config.
-        workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
+            Required. ID to use for the workstation
+            configuration.
+        workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
             Required. Config to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -1185,25 +1216,26 @@
     )
 
 
 class UpdateWorkstationConfigRequest(proto.Message):
     r"""Request message for UpdateWorkstationConfig.
 
     Attributes:
-        workstation_config (google.cloud.workstations_v1beta.types.WorkstationConfig):
+        workstation_config (google.cloud.workstations_v1.types.WorkstationConfig):
             Required. Config to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
-            config should be updated.
+            workstation configuration should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         allow_missing (bool):
-            If set, and the config is not found, a new config will be
-            created. In this situation, update_mask is ignored.
+            If set and the workstation configuration is not found, a new
+            workstation configuration will be created. In this
+            situation, update_mask is ignored.
     """
 
     workstation_config: "WorkstationConfig" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="WorkstationConfig",
     )
@@ -1223,26 +1255,28 @@
 
 
 class DeleteWorkstationConfigRequest(proto.Message):
     r"""Message for deleting a workstation configuration.
 
     Attributes:
         name (str):
-            Required. Name of the config to delete.
+            Required. Name of the workstation
+            configuration to delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
-            If set, the request will be rejected if the
-            latest version of the config on the server does
-            not have this etag.
+            If set, the request is rejected if the latest
+            version of the workstation configuration on the
+            server does not have this ETag.
         force (bool):
-            If set, any Workstations in the config will
-            also be deleted. Otherwise, the request will
-            work only if the config has no workstations.
+            If set, any workstations in the workstation
+            configuration are also deleted. Otherwise, the
+            request works only if the workstation
+            configuration has no workstations.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1300,15 +1334,15 @@
     )
 
 
 class ListWorkstationsResponse(proto.Message):
     r"""Response message for ListWorkstations.
 
     Attributes:
-        workstations (MutableSequence[google.cloud.workstations_v1beta.types.Workstation]):
+        workstations (MutableSequence[google.cloud.workstations_v1.types.Workstation]):
             The requested workstations.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1360,15 +1394,15 @@
     )
 
 
 class ListUsableWorkstationsResponse(proto.Message):
     r"""Response message for ListUsableWorkstations.
 
     Attributes:
-        workstations (MutableSequence[google.cloud.workstations_v1beta.types.Workstation]):
+        workstations (MutableSequence[google.cloud.workstations_v1.types.Workstation]):
             The requested workstations.
         next_page_token (str):
             Token to retrieve the next page of results,
             or empty if there are no more results in the
             list.
         unreachable (MutableSequence[str]):
             Unreachable resources.
@@ -1397,15 +1431,15 @@
     r"""Message for creating a CreateWorkstation.
 
     Attributes:
         parent (str):
             Required. Parent resource name.
         workstation_id (str):
             Required. ID to use for the workstation.
-        workstation (google.cloud.workstations_v1beta.types.Workstation):
+        workstation (google.cloud.workstations_v1.types.Workstation):
             Required. Workstation to create.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
     """
 
     parent: str = proto.Field(
@@ -1427,25 +1461,26 @@
     )
 
 
 class UpdateWorkstationRequest(proto.Message):
     r"""Request message for UpdateWorkstation.
 
     Attributes:
-        workstation (google.cloud.workstations_v1beta.types.Workstation):
+        workstation (google.cloud.workstations_v1.types.Workstation):
             Required. Workstation to update.
         update_mask (google.protobuf.field_mask_pb2.FieldMask):
             Required. Mask specifying which fields in the
-            config should be updated.
+            workstation configuration should be updated.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         allow_missing (bool):
-            If set, and the config is not found, a new config will be
-            created. In this situation, update_mask is ignored.
+            If set and the workstation configuration is not found, a new
+            workstation configuration is created. In this situation,
+            update_mask is ignored.
     """
 
     workstation: "Workstation" = proto.Field(
         proto.MESSAGE,
         number=1,
         message="Workstation",
     )
@@ -1472,15 +1507,15 @@
             Required. Name of the workstation to delete.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1501,15 +1536,15 @@
             Required. Name of the workstation to start.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1530,15 +1565,15 @@
             Required. Name of the workstation to stop.
         validate_only (bool):
             If set, validate the request and preview the
             review, but do not actually apply it.
         etag (str):
             If set, the request will be rejected if the
             latest version of the workstation on the server
-            does not have this etag.
+            does not have this ETag.
     """
 
     name: str = proto.Field(
         proto.STRING,
         number=1,
     )
     validate_only: bool = proto.Field(
@@ -1558,17 +1593,14 @@
     For each oneof, at most one member field can be set at the same time.
     Setting any member of the oneof automatically clears all other
     members.
 
     .. _oneof: https://proto-plus-python.readthedocs.io/en/stable/fields.html#oneofs-mutually-exclusive-fields
 
     Attributes:
-        workstation (str):
-            Required. Name of the workstation for which
-            the access token should be generated.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Desired expiration time of the access token.
             This value must be at most 24 hours in the
             future. If a value is not specified, the token's
             expiration time will be set to a default value
             of 1 hour in the future.
 
@@ -1576,42 +1608,45 @@
         ttl (google.protobuf.duration_pb2.Duration):
             Desired lifetime duration of the access
             token. This value must be at most 24 hours. If a
             value is not specified, the token's lifetime
             will be set to a default value of 1 hour.
 
             This field is a member of `oneof`_ ``expiration``.
+        workstation (str):
+            Required. Name of the workstation for which
+            the access token should be generated.
     """
 
-    workstation: str = proto.Field(
-        proto.STRING,
-        number=1,
-    )
     expire_time: timestamp_pb2.Timestamp = proto.Field(
         proto.MESSAGE,
         number=2,
         oneof="expiration",
         message=timestamp_pb2.Timestamp,
     )
     ttl: duration_pb2.Duration = proto.Field(
         proto.MESSAGE,
         number=3,
         oneof="expiration",
         message=duration_pb2.Duration,
     )
+    workstation: str = proto.Field(
+        proto.STRING,
+        number=1,
+    )
 
 
 class GenerateAccessTokenResponse(proto.Message):
     r"""Response message for GenerateAccessToken.
 
     Attributes:
         access_token (str):
             The generated bearer access token. To use this token,
             include it in an Authorization header of an HTTP request
-            sent to the associated workstation's hostname, for example,
+            sent to the associated workstation's hostname—for example,
             ``Authorization: Bearer <access_token>``.
         expire_time (google.protobuf.timestamp_pb2.Timestamp):
             Time at which the generated token will
             expire.
     """
 
     access_token: str = proto.Field(
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/PKG-INFO` & `google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-workstations
-Version: 0.2.1
+Version: 0.3.0
 Summary: Google Cloud Workstations API client library
 Home-page: https://github.com/googleapis/google-cloud-python
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-workstations-0.2.1/google_cloud_workstations.egg-info/SOURCES.txt` & `google-cloud-workstations-0.3.0/google_cloud_workstations.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/setup.py` & `google-cloud-workstations-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/__init__.py` & `google-cloud-workstations-0.3.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/unit/__init__.py` & `google-cloud-workstations-0.3.0/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/unit/gapic/__init__.py` & `google-cloud-workstations-0.3.0/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/__init__.py` & `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1/test_workstations.py` & `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/test_workstations.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.workstations_v1.services.workstations import (
+from google.cloud.workstations_v1beta.services.workstations import (
     WorkstationsAsyncClient,
     WorkstationsClient,
     pagers,
     transports,
 )
-from google.cloud.workstations_v1.types import workstations
+from google.cloud.workstations_v1beta.types import workstations
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -620,15 +620,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_workstations_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsGrpcTransport.__init__"
+        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = WorkstationsClient(client_options={"api_endpoint": "squid.clam.whelk"})
         grpc_transport.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host="squid.clam.whelk",
@@ -6966,15 +6966,15 @@
         client.get_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -7255,15 +7255,15 @@
         client.list_workstation_clusters(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*}/workstationClusters"
+            "%s/v1beta/{parent=projects/*/locations/*}/workstationClusters"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstation_clusters_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -7681,15 +7681,15 @@
         client.create_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*}/workstationClusters"
+            "%s/v1beta/{parent=projects/*/locations/*}/workstationClusters"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8043,15 +8043,15 @@
         client.update_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{workstation_cluster.name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1beta/{workstation_cluster.name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8330,15 +8330,15 @@
         client.delete_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8614,15 +8614,15 @@
         client.get_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8907,15 +8907,15 @@
         client.list_workstation_configs(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstation_configs_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9268,15 +9268,15 @@
         client.list_usable_workstation_configs(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs:listUsable"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs:listUsable"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_usable_workstation_configs_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9394,34 +9394,33 @@
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
                 "disable_public_ip_addresses": True,
-                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
+                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
-                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -9675,34 +9674,33 @@
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
                 "disable_public_ip_addresses": True,
-                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
+                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
-                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -9775,15 +9773,15 @@
         client.create_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9843,34 +9841,33 @@
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
                 "disable_public_ip_addresses": True,
-                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
+                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
-                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -10106,34 +10103,33 @@
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
                 "disable_public_ip_addresses": True,
-                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
+                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
-                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -10207,15 +10203,15 @@
         client.update_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{workstation_config.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1beta/{workstation_config.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -10494,15 +10490,15 @@
         client.delete_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -10780,15 +10776,15 @@
         client.get_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11071,15 +11067,15 @@
         client.list_workstations(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstations_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11423,15 +11419,15 @@
         client.list_usable_workstations(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations:listUsable"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations:listUsable"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_usable_workstations_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11816,15 +11812,15 @@
         client.create_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
+            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12140,15 +12136,15 @@
         client.update_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{workstation.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1beta/{workstation.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12425,15 +12421,15 @@
         client.delete_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12695,15 +12691,15 @@
         client.start_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:start"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:start"
             % client.transport._host,
             args[1],
         )
 
 
 def test_start_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12965,15 +12961,15 @@
         client.stop_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:stop"
+            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:stop"
             % client.transport._host,
             args[1],
         )
 
 
 def test_stop_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -13240,15 +13236,15 @@
         client.generate_access_token(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1/{workstation=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:generateAccessToken"
+            "%s/v1beta/{workstation=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:generateAccessToken"
             % client.transport._host,
             args[1],
         )
 
 
 def test_generate_access_token_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -13396,15 +13392,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_workstations_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport.__init__"
+        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.WorkstationsTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -13460,15 +13456,15 @@
 
 
 def test_workstations_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
+        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.WorkstationsTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -13479,15 +13475,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_workstations_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
+        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.WorkstationsTransport()
         adc.assert_called_once()
```

### Comparing `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/__init__.py` & `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1beta/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-workstations-0.2.1/tests/unit/gapic/workstations_v1beta/test_workstations.py` & `google-cloud-workstations-0.3.0/tests/unit/gapic/workstations_v1/test_workstations.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,21 +57,21 @@
 from grpc.experimental import aio
 from proto.marshal.rules import wrappers
 from proto.marshal.rules.dates import DurationRule, TimestampRule
 import pytest
 from requests import PreparedRequest, Request, Response
 from requests.sessions import Session
 
-from google.cloud.workstations_v1beta.services.workstations import (
+from google.cloud.workstations_v1.services.workstations import (
     WorkstationsAsyncClient,
     WorkstationsClient,
     pagers,
     transports,
 )
-from google.cloud.workstations_v1beta.types import workstations
+from google.cloud.workstations_v1.types import workstations
 
 
 def client_cert_source_callback():
     return b"cert bytes", b"key bytes"
 
 
 # If default endpoint is localhost, then default mtls endpoint will be the same.
@@ -620,15 +620,15 @@
             always_use_jwt_access=True,
             api_audience=None,
         )
 
 
 def test_workstations_client_client_options_from_dict():
     with mock.patch(
-        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsGrpcTransport.__init__"
+        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsGrpcTransport.__init__"
     ) as grpc_transport:
         grpc_transport.return_value = None
         client = WorkstationsClient(client_options={"api_endpoint": "squid.clam.whelk"})
         grpc_transport.assert_called_once_with(
             credentials=None,
             credentials_file=None,
             host="squid.clam.whelk",
@@ -734,14 +734,15 @@
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             network="network_value",
             subnetwork="subnetwork_value",
+            control_plane_ip="control_plane_ip_value",
             degraded=True,
         )
         response = client.get_workstation_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
@@ -752,14 +753,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 def test_get_workstation_cluster_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = WorkstationsClient(
@@ -801,14 +803,15 @@
                 name="name_value",
                 display_name="display_name_value",
                 uid="uid_value",
                 reconciling=True,
                 etag="etag_value",
                 network="network_value",
                 subnetwork="subnetwork_value",
+                control_plane_ip="control_plane_ip_value",
                 degraded=True,
             )
         )
         response = await client.get_workstation_cluster(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
@@ -820,14 +823,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 @pytest.mark.asyncio
 async def test_get_workstation_cluster_async_from_dict():
     await test_get_workstation_cluster_async(request_type=dict)
 
@@ -6735,14 +6739,15 @@
             name="name_value",
             display_name="display_name_value",
             uid="uid_value",
             reconciling=True,
             etag="etag_value",
             network="network_value",
             subnetwork="subnetwork_value",
+            control_plane_ip="control_plane_ip_value",
             degraded=True,
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         pb_return_value = workstations.WorkstationCluster.pb(return_value)
@@ -6757,14 +6762,15 @@
     assert response.name == "name_value"
     assert response.display_name == "display_name_value"
     assert response.uid == "uid_value"
     assert response.reconciling is True
     assert response.etag == "etag_value"
     assert response.network == "network_value"
     assert response.subnetwork == "subnetwork_value"
+    assert response.control_plane_ip == "control_plane_ip_value"
     assert response.degraded is True
 
 
 def test_get_workstation_cluster_rest_required_fields(
     request_type=workstations.GetWorkstationClusterRequest,
 ):
     transport_class = transports.WorkstationsRestTransport
@@ -6966,15 +6972,15 @@
         client.get_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -7255,15 +7261,15 @@
         client.list_workstation_clusters(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*}/workstationClusters"
+            "%s/v1/{parent=projects/*/locations/*}/workstationClusters"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstation_clusters_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -7367,14 +7373,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7611,14 +7618,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7681,15 +7689,15 @@
         client.create_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*}/workstationClusters"
+            "%s/v1/{parent=projects/*/locations/*}/workstationClusters"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -7742,14 +7750,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -7970,14 +7979,15 @@
         "labels": {},
         "create_time": {"seconds": 751, "nanos": 543},
         "update_time": {},
         "delete_time": {},
         "etag": "etag_value",
         "network": "network_value",
         "subnetwork": "subnetwork_value",
+        "control_plane_ip": "control_plane_ip_value",
         "private_cluster_config": {
             "enable_private_endpoint": True,
             "cluster_hostname": "cluster_hostname_value",
             "service_attachment_uri": "service_attachment_uri_value",
             "allowed_projects": ["allowed_projects_value1", "allowed_projects_value2"],
         },
         "degraded": True,
@@ -8043,15 +8053,15 @@
         client.update_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{workstation_cluster.name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1/{workstation_cluster.name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8330,15 +8340,15 @@
         client.delete_workstation_cluster(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_cluster_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8614,15 +8624,15 @@
         client.get_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -8907,15 +8917,15 @@
         client.list_workstation_configs(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstation_configs_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9268,15 +9278,15 @@
         client.list_usable_workstation_configs(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs:listUsable"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs:listUsable"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_usable_workstation_configs_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9393,34 +9403,36 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
+                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
-                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
+                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -9673,34 +9685,36 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
+                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
-                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
+                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -9773,15 +9787,15 @@
         client.create_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*}/workstationConfigs"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -9840,34 +9854,36 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
+                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
-                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
+                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -10102,34 +10118,36 @@
         "running_timeout": {},
         "host": {
             "gce_instance": {
                 "machine_type": "machine_type_value",
                 "service_account": "service_account_value",
                 "tags": ["tags_value1", "tags_value2"],
                 "pool_size": 980,
+                "pooled_instances": 1706,
                 "disable_public_ip_addresses": True,
+                "enable_nested_virtualization": True,
                 "shielded_instance_config": {
                     "enable_secure_boot": True,
                     "enable_vtpm": True,
                     "enable_integrity_monitoring": True,
                 },
                 "confidential_instance_config": {"enable_confidential_compute": True},
                 "boot_disk_size_gb": 1792,
             }
         },
         "persistent_directories": [
             {
-                "mount_path": "mount_path_value",
                 "gce_pd": {
                     "size_gb": 739,
                     "fs_type": "fs_type_value",
                     "disk_type": "disk_type_value",
                     "source_snapshot": "source_snapshot_value",
                     "reclaim_policy": 1,
                 },
+                "mount_path": "mount_path_value",
             }
         ],
         "container": {
             "image": "image_value",
             "command": ["command_value1", "command_value2"],
             "args": ["args_value1", "args_value2"],
             "env": {},
@@ -10203,15 +10221,15 @@
         client.update_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{workstation_config.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1/{workstation_config.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -10490,15 +10508,15 @@
         client.delete_workstation_config(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_config_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -10776,15 +10794,15 @@
         client.get_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_get_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11067,15 +11085,15 @@
         client.list_workstations(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_workstations_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11419,15 +11437,15 @@
         client.list_usable_workstations(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations:listUsable"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations:listUsable"
             % client.transport._host,
             args[1],
         )
 
 
 def test_list_usable_workstations_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -11812,15 +11830,15 @@
         client.create_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
+            "%s/v1/{parent=projects/*/locations/*/workstationClusters/*/workstationConfigs/*}/workstations"
             % client.transport._host,
             args[1],
         )
 
 
 def test_create_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12136,15 +12154,15 @@
         client.update_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{workstation.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1/{workstation.name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_update_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12421,15 +12439,15 @@
         client.delete_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}"
             % client.transport._host,
             args[1],
         )
 
 
 def test_delete_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12691,15 +12709,15 @@
         client.start_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:start"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:start"
             % client.transport._host,
             args[1],
         )
 
 
 def test_start_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -12961,15 +12979,15 @@
         client.stop_workstation(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:stop"
+            "%s/v1/{name=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:stop"
             % client.transport._host,
             args[1],
         )
 
 
 def test_stop_workstation_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -13236,15 +13254,15 @@
         client.generate_access_token(**mock_args)
 
         # Establish that the underlying call was made with the expected
         # request object values.
         assert len(req.mock_calls) == 1
         _, args, _ = req.mock_calls[0]
         assert path_template.validate(
-            "%s/v1beta/{workstation=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:generateAccessToken"
+            "%s/v1/{workstation=projects/*/locations/*/workstationClusters/*/workstationConfigs/*/workstations/*}:generateAccessToken"
             % client.transport._host,
             args[1],
         )
 
 
 def test_generate_access_token_rest_flattened_error(transport: str = "rest"):
     client = WorkstationsClient(
@@ -13392,15 +13410,15 @@
             credentials_file="credentials.json",
         )
 
 
 def test_workstations_base_transport():
     # Instantiate the base transport.
     with mock.patch(
-        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport.__init__"
+        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport.__init__"
     ) as Transport:
         Transport.return_value = None
         transport = transports.WorkstationsTransport(
             credentials=ga_credentials.AnonymousCredentials(),
         )
 
     # Every method on the transport should just blindly
@@ -13456,15 +13474,15 @@
 
 
 def test_workstations_base_transport_with_credentials_file():
     # Instantiate the base transport with a credentials file
     with mock.patch.object(
         google.auth, "load_credentials_from_file", autospec=True
     ) as load_creds, mock.patch(
-        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
+        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         load_creds.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.WorkstationsTransport(
             credentials_file="credentials.json",
             quota_project_id="octopus",
         )
@@ -13475,15 +13493,15 @@
             quota_project_id="octopus",
         )
 
 
 def test_workstations_base_transport_with_adc():
     # Test the default credentials are used if credentials and credentials_file are None.
     with mock.patch.object(google.auth, "default", autospec=True) as adc, mock.patch(
-        "google.cloud.workstations_v1beta.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
+        "google.cloud.workstations_v1.services.workstations.transports.WorkstationsTransport._prep_wrapped_messages"
     ) as Transport:
         Transport.return_value = None
         adc.return_value = (ga_credentials.AnonymousCredentials(), None)
         transport = transports.WorkstationsTransport()
         adc.assert_called_once()
```

