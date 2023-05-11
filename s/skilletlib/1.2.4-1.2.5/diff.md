# Comparing `tmp/skilletlib-1.2.4.tar.gz` & `tmp/skilletlib-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skilletlib-1.2.4.tar", last modified: Thu Apr  7 16:09:08 2022, max compression
+gzip compressed data, was "skilletlib-1.2.5.tar", last modified: Thu May 11 16:51:37 2023, max compression
```

## Comparing `skilletlib-1.2.4.tar` & `skilletlib-1.2.5.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.286114 skilletlib-1.2.4/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    11357 2021-12-03 17:18:16.000000 skilletlib-1.2.4/LICENSE
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)       37 2021-12-03 17:18:16.000000 skilletlib-1.2.4/MANIFEST.in
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     6750 2022-04-07 16:09:08.286293 skilletlib-1.2.4/PKG-INFO
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     6231 2021-12-03 17:18:16.000000 skilletlib-1.2.4/README.md
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)       99 2022-04-07 16:09:08.287045 skilletlib-1.2.4/setup.cfg
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1179 2022-04-07 16:05:22.000000 skilletlib-1.2.4/setup.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.251712 skilletlib-1.2.4/skilletlib/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      206 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/__init__.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.255033 skilletlib-1.2.4/skilletlib/assets/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/__init__.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.243289 skilletlib-1.2.4/skilletlib/assets/panorama/
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.256051 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_81/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1827 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_81/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     3269 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_81/baseline_81.xml
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.257667 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_90/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1827 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_90/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     3537 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panorama/baseline_90/baseline_90.xml
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.244700 skilletlib-1.2.4/skilletlib/assets/panos/
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.258804 skilletlib-1.2.4/skilletlib/assets/panos/baseline_80/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      977 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_80/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    12663 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_80/baseline_80.xml
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.259773 skilletlib-1.2.4/skilletlib/assets/panos/baseline_81/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1356 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_81/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    12663 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_81/baseline_81.xml
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.260907 skilletlib-1.2.4/skilletlib/assets/panos/baseline_90/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1354 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_90/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    12898 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_90/baseline_90.xml
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.262764 skilletlib-1.2.4/skilletlib/assets/panos/baseline_91/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1354 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_91/.meta-cnc.yaml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    12898 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/assets/panos/baseline_91/baseline_91.xml
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      725 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/exceptions.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    85767 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/panoply.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.264137 skilletlib-1.2.4/skilletlib/remotes/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/remotes/__init__.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     5235 2021-12-03 17:25:12.000000 skilletlib-1.2.4/skilletlib/remotes/git.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.275351 skilletlib-1.2.4/skilletlib/skillet/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      271 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/__init__.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      904 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/app.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    25968 2022-02-15 15:26:41.000000 skilletlib-1.2.4/skilletlib/skillet/base.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     3438 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/docker.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     5409 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/pan_validation.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    13266 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/panos.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1380 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/python3.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     3749 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/rest.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     2365 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/template.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1058 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/terraform.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     3363 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skillet/workflow.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    44028 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/skilletLoader.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.283769 skilletlib-1.2.4/skilletlib/snippet/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/__init__.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    55761 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/base.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     9374 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/docker.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     2648 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/pan_validation.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)    14966 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/panos.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      767 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/python3.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     4447 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/rest.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1405 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/template.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     4840 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/snippet/workflow.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.285372 skilletlib-1.2.4/skilletlib/utils/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/utils/__init__.py
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      161 2021-12-03 17:18:16.000000 skilletlib-1.2.4/skilletlib/utils/testing_utils.py
-drwxr-xr-x   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        0 2022-04-07 16:09:08.254592 skilletlib-1.2.4/skilletlib.egg-info/
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     6750 2022-04-07 16:09:08.000000 skilletlib-1.2.4/skilletlib.egg-info/PKG-INFO
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)     1695 2022-04-07 16:09:08.000000 skilletlib-1.2.4/skilletlib.egg-info/SOURCES.txt
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)        1 2022-04-07 16:09:08.000000 skilletlib-1.2.4/skilletlib.egg-info/dependency_links.txt
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)      152 2022-04-07 16:09:08.000000 skilletlib-1.2.4/skilletlib.egg-info/requires.txt
--rw-r--r--   0 nembery  (934317215) PALOALTONETWORK\Domain Users (192360288)       11 2022-04-07 16:09:08.000000 skilletlib-1.2.4/skilletlib.egg-info/top_level.txt
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.775364 skilletlib-1.2.5/
+-rw-r--r--   0 nembery  (934317215) 192360288    11357 2021-12-03 17:18:16.000000 skilletlib-1.2.5/LICENSE
+-rw-r--r--   0 nembery  (934317215) 192360288       37 2021-12-03 17:18:16.000000 skilletlib-1.2.5/MANIFEST.in
+-rw-r--r--   0 nembery  (934317215) 192360288     6750 2023-05-11 16:51:37.775579 skilletlib-1.2.5/PKG-INFO
+-rw-r--r--   0 nembery  (934317215) 192360288     6231 2021-12-03 17:18:16.000000 skilletlib-1.2.5/README.md
+-rw-r--r--   0 nembery  (934317215) 192360288       99 2023-05-11 16:51:37.776314 skilletlib-1.2.5/setup.cfg
+-rw-r--r--   0 nembery  (934317215) 192360288     1179 2023-05-11 16:51:05.000000 skilletlib-1.2.5/setup.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.729597 skilletlib-1.2.5/skilletlib/
+-rw-r--r--   0 nembery  (934317215) 192360288      206 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/__init__.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.734853 skilletlib-1.2.5/skilletlib/assets/
+-rw-r--r--   0 nembery  (934317215) 192360288        0 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/__init__.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.719764 skilletlib-1.2.5/skilletlib/assets/panorama/
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.736223 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_81/
+-rw-r--r--   0 nembery  (934317215) 192360288     1827 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_81/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288     3269 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_81/baseline_81.xml
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.737730 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_90/
+-rw-r--r--   0 nembery  (934317215) 192360288     1827 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_90/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288     3537 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panorama/baseline_90/baseline_90.xml
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.720971 skilletlib-1.2.5/skilletlib/assets/panos/
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.739118 skilletlib-1.2.5/skilletlib/assets/panos/baseline_80/
+-rw-r--r--   0 nembery  (934317215) 192360288      977 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_80/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288    12663 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_80/baseline_80.xml
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.740634 skilletlib-1.2.5/skilletlib/assets/panos/baseline_81/
+-rw-r--r--   0 nembery  (934317215) 192360288     1356 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_81/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288    12663 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_81/baseline_81.xml
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.742608 skilletlib-1.2.5/skilletlib/assets/panos/baseline_90/
+-rw-r--r--   0 nembery  (934317215) 192360288     1354 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_90/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288    12898 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_90/baseline_90.xml
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.744332 skilletlib-1.2.5/skilletlib/assets/panos/baseline_91/
+-rw-r--r--   0 nembery  (934317215) 192360288     1354 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_91/.meta-cnc.yaml
+-rw-r--r--   0 nembery  (934317215) 192360288    12898 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/assets/panos/baseline_91/baseline_91.xml
+-rw-r--r--   0 nembery  (934317215) 192360288      725 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/exceptions.py
+-rw-r--r--   0 nembery  (934317215) 192360288    86398 2023-05-11 16:50:47.000000 skilletlib-1.2.5/skilletlib/panoply.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.746128 skilletlib-1.2.5/skilletlib/remotes/
+-rw-r--r--   0 nembery  (934317215) 192360288        0 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/remotes/__init__.py
+-rw-r--r--   0 nembery  (934317215) 192360288     5235 2021-12-03 17:25:12.000000 skilletlib-1.2.5/skilletlib/remotes/git.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.762151 skilletlib-1.2.5/skilletlib/skillet/
+-rw-r--r--   0 nembery  (934317215) 192360288      271 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/__init__.py
+-rw-r--r--   0 nembery  (934317215) 192360288      904 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/app.py
+-rw-r--r--   0 nembery  (934317215) 192360288    25968 2022-02-15 15:26:41.000000 skilletlib-1.2.5/skilletlib/skillet/base.py
+-rw-r--r--   0 nembery  (934317215) 192360288     3438 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/docker.py
+-rw-r--r--   0 nembery  (934317215) 192360288     5409 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/pan_validation.py
+-rw-r--r--   0 nembery  (934317215) 192360288    13266 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/panos.py
+-rw-r--r--   0 nembery  (934317215) 192360288     1380 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/python3.py
+-rw-r--r--   0 nembery  (934317215) 192360288     3749 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/rest.py
+-rw-r--r--   0 nembery  (934317215) 192360288     2365 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/template.py
+-rw-r--r--   0 nembery  (934317215) 192360288     1058 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/terraform.py
+-rw-r--r--   0 nembery  (934317215) 192360288     3363 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skillet/workflow.py
+-rw-r--r--   0 nembery  (934317215) 192360288    44028 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/skilletLoader.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.772337 skilletlib-1.2.5/skilletlib/snippet/
+-rw-r--r--   0 nembery  (934317215) 192360288        0 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/__init__.py
+-rw-r--r--   0 nembery  (934317215) 192360288    55761 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/base.py
+-rw-r--r--   0 nembery  (934317215) 192360288     9374 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/docker.py
+-rw-r--r--   0 nembery  (934317215) 192360288     2648 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/pan_validation.py
+-rw-r--r--   0 nembery  (934317215) 192360288    14966 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/panos.py
+-rw-r--r--   0 nembery  (934317215) 192360288      767 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/python3.py
+-rw-r--r--   0 nembery  (934317215) 192360288     4447 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/rest.py
+-rw-r--r--   0 nembery  (934317215) 192360288     1405 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/template.py
+-rw-r--r--   0 nembery  (934317215) 192360288     4840 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/snippet/workflow.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.774427 skilletlib-1.2.5/skilletlib/utils/
+-rw-r--r--   0 nembery  (934317215) 192360288        0 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/utils/__init__.py
+-rw-r--r--   0 nembery  (934317215) 192360288      161 2021-12-03 17:18:16.000000 skilletlib-1.2.5/skilletlib/utils/testing_utils.py
+drwxr-xr-x   0 nembery  (934317215) 192360288        0 2023-05-11 16:51:37.734047 skilletlib-1.2.5/skilletlib.egg-info/
+-rw-r--r--   0 nembery  (934317215) 192360288     6750 2023-05-11 16:51:37.000000 skilletlib-1.2.5/skilletlib.egg-info/PKG-INFO
+-rw-r--r--   0 nembery  (934317215) 192360288     1695 2023-05-11 16:51:37.000000 skilletlib-1.2.5/skilletlib.egg-info/SOURCES.txt
+-rw-r--r--   0 nembery  (934317215) 192360288        1 2023-05-11 16:51:37.000000 skilletlib-1.2.5/skilletlib.egg-info/dependency_links.txt
+-rw-r--r--   0 nembery  (934317215) 192360288      152 2023-05-11 16:51:37.000000 skilletlib-1.2.5/skilletlib.egg-info/requires.txt
+-rw-r--r--   0 nembery  (934317215) 192360288       11 2023-05-11 16:51:37.000000 skilletlib-1.2.5/skilletlib.egg-info/top_level.txt
```

### Comparing `skilletlib-1.2.4/LICENSE` & `skilletlib-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/PKG-INFO` & `skilletlib-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilletlib
-Version: 1.2.4
+Version: 1.2.5
 Summary: Tools for working with PAN-OS Skillets in Python 3
 Home-page: https://github.com/paloaltonetworks/skilletlib
 Author: Nathan Embery
 Author-email: nembery@paloaltonetworks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skilletlib-1.2.4/README.md` & `skilletlib-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/setup.py` & `skilletlib-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="skilletlib",
-    version="1.2.4",
+    version="1.2.5",
     author="Nathan Embery",
     author_email="nembery@paloaltonetworks.com",
     description="Tools for working with PAN-OS Skillets in Python 3",
     license='Apache 2.0',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/paloaltonetworks/skilletlib",
```

### Comparing `skilletlib-1.2.4/skilletlib/assets/panorama/baseline_81/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panorama/baseline_81/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panorama/baseline_81/baseline_81.xml` & `skilletlib-1.2.5/skilletlib/assets/panorama/baseline_81/baseline_81.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panorama/baseline_90/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panorama/baseline_90/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panorama/baseline_90/baseline_90.xml` & `skilletlib-1.2.5/skilletlib/assets/panorama/baseline_90/baseline_90.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_80/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_80/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_80/baseline_80.xml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_80/baseline_80.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_81/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_81/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_81/baseline_81.xml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_81/baseline_81.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_90/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_90/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_90/baseline_90.xml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_90/baseline_90.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_91/.meta-cnc.yaml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_91/.meta-cnc.yaml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/assets/panos/baseline_91/baseline_91.xml` & `skilletlib-1.2.5/skilletlib/assets/panos/baseline_91/baseline_91.xml`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/exceptions.py` & `skilletlib-1.2.5/skilletlib/exceptions.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/panoply.py` & `skilletlib-1.2.5/skilletlib/panoply.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,43 +457,54 @@
             self.xapi.ad_hoc(qs=qs, modify_qs=True)
 
         except PanXapiError as e:
             raise PanoplyException(f"Could not execute query_set: {qs}: {e}")
 
         return self.xapi.xml_document
 
-    def fetch_license(self, auth_code: str) -> bool:
+    def fetch_license(self, auth_code: str, force_fetch_license: bool = False) -> bool:
         """
         Fetch and install licenses for PAN-OS NGFW
 
         :param auth_code: Authorization code to use to license the NGFW
+        :param force_fetch_license: Fetch licenses even if NGFW is already licensed
         :return: True when license installation succeeds / False otherwise
         """
 
         if self.facts.get("family", "") == "vm":
 
-            if self.facts.get("vm-license", "none") != "none":
+            if force_fetch_license:
+                logger.debug("force_fetch_license is set. Not checking if device is already licensed.")
+            elif self.facts.get("vm-license", "none") != "none":
                 logger.debug("This VM is already licensed")
                 return True
 
         try:
             cmd = f"<request><license><fetch><auth-code>{auth_code}</auth-code></fetch></license></request>"
             logger.debug(f"Using request cmd: {cmd}")
             self.xapi.op(cmd=cmd)
             results = self.xapi.xml_result()
             logger.debug(f"fetch_license results: {results}")
 
             if "License installed" in results:
                 return True
+            # If VMseries is already licensed but auth_code adds more features it will return <licenses />
+            # containting all the licenses installed
+            if "<licenses>" in results:
+                return True
 
             else:
                 logger.warning("Unexpected Results from fetch_license")
                 logger.warning(results)
                 return False
 
+        except RemoteDisconnected:
+            logger.info("PAN-OS dropped the connection due to licensing request")
+            return True
+
         except PanXapiError as pxe:
             # bug present in 9.0.4 that returns content-type of xml but the content is only text.
             # this causes a ParseError to be thrown, however, the operation was actually successful
 
             if "ParseError" in str(pxe):
 
                 if self.xapi.xml_document is not None and "License installed" in self.xapi.xml_document:
```

### Comparing `skilletlib-1.2.4/skilletlib/remotes/git.py` & `skilletlib-1.2.5/skilletlib/remotes/git.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/app.py` & `skilletlib-1.2.5/skilletlib/skillet/app.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/base.py` & `skilletlib-1.2.5/skilletlib/skillet/base.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/docker.py` & `skilletlib-1.2.5/skilletlib/skillet/docker.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/pan_validation.py` & `skilletlib-1.2.5/skilletlib/skillet/pan_validation.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/panos.py` & `skilletlib-1.2.5/skilletlib/skillet/panos.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/python3.py` & `skilletlib-1.2.5/skilletlib/skillet/python3.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/rest.py` & `skilletlib-1.2.5/skilletlib/skillet/rest.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/template.py` & `skilletlib-1.2.5/skilletlib/skillet/template.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/terraform.py` & `skilletlib-1.2.5/skilletlib/skillet/terraform.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skillet/workflow.py` & `skilletlib-1.2.5/skilletlib/skillet/workflow.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/skilletLoader.py` & `skilletlib-1.2.5/skilletlib/skilletLoader.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/base.py` & `skilletlib-1.2.5/skilletlib/snippet/base.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/docker.py` & `skilletlib-1.2.5/skilletlib/snippet/docker.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/pan_validation.py` & `skilletlib-1.2.5/skilletlib/snippet/pan_validation.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/panos.py` & `skilletlib-1.2.5/skilletlib/snippet/panos.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/python3.py` & `skilletlib-1.2.5/skilletlib/snippet/python3.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/rest.py` & `skilletlib-1.2.5/skilletlib/snippet/rest.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/template.py` & `skilletlib-1.2.5/skilletlib/snippet/template.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib/snippet/workflow.py` & `skilletlib-1.2.5/skilletlib/snippet/workflow.py`

 * *Files identical despite different names*

### Comparing `skilletlib-1.2.4/skilletlib.egg-info/PKG-INFO` & `skilletlib-1.2.5/skilletlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skilletlib
-Version: 1.2.4
+Version: 1.2.5
 Summary: Tools for working with PAN-OS Skillets in Python 3
 Home-page: https://github.com/paloaltonetworks/skilletlib
 Author: Nathan Embery
 Author-email: nembery@paloaltonetworks.com
 License: Apache 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `skilletlib-1.2.4/skilletlib.egg-info/SOURCES.txt` & `skilletlib-1.2.5/skilletlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

