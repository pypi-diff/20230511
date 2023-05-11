# Comparing `tmp/os-traits-2.9.0.tar.gz` & `tmp/os-traits-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-traits-2.9.0.tar", last modified: Fri Aug 26 17:09:01 2022, max compression
+gzip compressed data, was "os-traits-3.0.0.tar", last modified: Thu May 11 09:13:36 2023, max compression
```

## Comparing `os-traits-2.9.0.tar` & `os-traits-3.0.0.tar`

### file list

```diff
@@ -1,113 +1,113 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.153655 os-traits-2.9.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2022-08-26 17:08:18.000000 os-traits-2.9.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2022-08-26 17:08:18.000000 os-traits-2.9.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2082 2022-08-26 17:09:00.000000 os-traits-2.9.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2022-08-26 17:08:18.000000 os-traits-2.9.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5430 2022-08-26 17:09:00.000000 os-traits-2.9.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2022-08-26 17:08:18.000000 os-traits-2.9.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-08-26 17:08:18.000000 os-traits-2.9.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2022-08-26 17:08:18.000000 os-traits-2.9.0/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2022-08-26 17:09:01.153655 os-traits-2.9.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2022-08-26 17:08:18.000000 os-traits-2.9.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/ext/traits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2484 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2022-08-26 17:08:18.000000 os-traits-2.9.0/doc/source/user/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.137655 os-traits-2.9.0/os_traits/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5695 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2274 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/arch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/config_drive.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/ephemeral.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/firmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/graphics.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/image.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/migrate.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/security.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/storage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/viommu.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/compute/volume.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/hw/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/arch.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/hw/cpu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/aarch64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/amd.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/hw/cpu/ppc64le/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/ppc64le/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/hw/cpu/x86/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/x86/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/x86/amd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/cpu/x86/intel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.145655 os-traits-2.9.0/os_traits/hw/gpu/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/gpu/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/gpu/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/gpu/cuda.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/gpu/max_display_heads.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/gpu/resolution.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/hw/nic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/nic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/nic/accel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/nic/dcb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/nic/offload.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/nic/sriov.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/hw/numa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/hw/numa/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/misc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1775 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/misc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/owner/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/owner/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/storage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/storage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/storage/disk.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/os_traits/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/tests/test_cuda.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5159 2022-08-26 17:08:18.000000 os-traits-2.9.0/os_traits/tests/test_os_traits.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.141655 os-traits-2.9.0/os_traits.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1878 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2022-08-26 17:09:01.000000 os-traits-2.9.0/os_traits.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.133655 os-traits-2.9.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.149655 os-traits-2.9.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/notes/add-owner-trait-f33e0e038961cbbd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/notes/add-suffix-get_traits-d1d91edcf7f65188.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/notes/drop-python2-support-d11499973c50713b.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.153655 os-traits-2.9.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.153655 os-traits-2.9.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:09:01.153655 os-traits-2.9.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2022-08-26 17:08:18.000000 os-traits-2.9.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2022-08-26 17:08:18.000000 os-traits-2.9.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      890 2022-08-26 17:09:01.153655 os-traits-2.9.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-08-26 17:08:18.000000 os-traits-2.9.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2022-08-26 17:08:18.000000 os-traits-2.9.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1348 2022-08-26 17:08:18.000000 os-traits-2.9.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.642694 os-traits-3.0.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       50 2023-05-11 09:13:08.000000 os-traits-3.0.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-05-11 09:13:08.000000 os-traits-3.0.0/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2023-05-11 09:13:36.000000 os-traits-3.0.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2023-05-11 09:13:08.000000 os-traits-3.0.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5711 2023-05-11 09:13:36.000000 os-traits-3.0.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-11 09:13:08.000000 os-traits-3.0.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 09:13:08.000000 os-traits-3.0.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2023-05-11 09:13:08.000000 os-traits-3.0.0/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2023-05-11 09:13:36.642694 os-traits-3.0.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2023-05-11 09:13:08.000000 os-traits-3.0.0/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.622688 os-traits-3.0.0/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.622688 os-traits-3.0.0/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/ext/traits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2484 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      693 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3693 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1532 2023-05-11 09:13:08.000000 os-traits-3.0.0/doc/source/user/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/os_traits/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5695 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.630690 os-traits-3.0.0/os_traits/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2525 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      864 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/arch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/config_drive.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/ephemeral.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/firmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      933 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/graphics.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/image.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      762 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/migrate.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/security.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/storage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      891 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/viommu.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      966 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/compute/volume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.630690 os-traits-3.0.0/os_traits/hw/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1241 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/arch.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.630690 os-traits-3.0.0/os_traits/hw/cpu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2289 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/aarch64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/amd.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.630690 os-traits-3.0.0/os_traits/hw/cpu/ppc64le/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      612 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/ppc64le/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/hw/cpu/x86/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/x86/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/x86/amd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/cpu/x86/intel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/hw/gpu/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/gpu/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/gpu/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5602 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/gpu/cuda.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/gpu/max_display_heads.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1025 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/gpu/resolution.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/hw/nic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      915 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/nic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      834 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/nic/accel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      765 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/nic/dcb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1399 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/nic/offload.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1134 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/nic/sriov.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/hw/numa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      924 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/hw/numa/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/misc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1775 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/misc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/owner/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/owner/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.634692 os-traits-3.0.0/os_traits/storage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/storage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      645 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/storage/disk.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.638693 os-traits-3.0.0/os_traits/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      794 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1516 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/tests/test_cuda.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5159 2023-05-11 09:13:08.000000 os-traits-3.0.0/os_traits/tests/test_os_traits.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.626689 os-traits-3.0.0/os_traits.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2319 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       19 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-05-11 09:13:36.000000 os-traits-3.0.0/os_traits.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.618687 os-traits-3.0.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.638693 os-traits-3.0.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/notes/add-owner-trait-f33e0e038961cbbd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/notes/add-suffix-get_traits-d1d91edcf7f65188.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/notes/drop-python2-support-d11499973c50713b.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.638693 os-traits-3.0.0/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.638693 os-traits-3.0.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:36.642694 os-traits-3.0.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2166 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:13:08.000000 os-traits-3.0.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-05-11 09:13:08.000000 os-traits-3.0.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      852 2023-05-11 09:13:36.642694 os-traits-3.0.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:13:08.000000 os-traits-3.0.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-05-11 09:13:08.000000 os-traits-3.0.0/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2023-05-11 09:13:08.000000 os-traits-3.0.0/tox.ini
```

### Comparing `os-traits-2.9.0/AUTHORS` & `os-traits-3.0.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Andreas Jaeger <aj@suse.com>
 Artom Lifshitz <alifshit@redhat.com>
 Balazs Gibizer <gibi@redhat.com>
 Charles Short <chucks@redhat.com>
 Chris Dent <cdent@anticdent.org>
 Corey Bryant <corey.bryant@canonical.com>
 Dan Smith <dansmith@redhat.com>
+Danylo Vodopianov <dvo-plv@napatech.com>
 Dmitrii Shcherbakov <dmitrii.shcherbakov@canonical.com>
 Doug Hellmann <doug@doughellmann.com>
 EdLeafe <ed@leafe.com>
 Edan David <edand@mellanox.com>
 Eric Fried <efried@us.ibm.com>
 Eric Fried <openstack@fried.cc>
 Ghanshyam Mann <gmann@ghanshyammann.com>
@@ -20,14 +21,15 @@
 Kashyap Chamarthy <kchamart@redhat.com>
 Kevin Zhao <kevin.zhao@arm.com>
 Konstantinos Samaras-Tsakiris <konstantinos.samaras-tsakiris@cern.ch>
 Lee Yarwood <lyarwood@redhat.com>
 Lin Yang <lin.a.yang@intel.com>
 Matt Riedemann <mriedem.os@gmail.com>
 Michael Davies <michael@the-davies.net>
+Nobuhiro MIKI <nmiki@yahoo-corp.jp>
 OpenStack Release Bot <infra-root@openstack.org>
 Paul-Emile Element <Paul-Emile.Element@windriver.com>
 René Ribaud <rribaud@redhat.com>
 Rico Lin <rlin@vexxhost.com>
 Rodolfo Alonso Hernandez <rodolfo.alonso.hernandez@intel.com>
 Ruby Loo <ruby.loo@intel.com>
 Sean Mooney <work@seanmooney.info>
```

### Comparing `os-traits-2.9.0/CONTRIBUTING.rst` & `os-traits-3.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/ChangeLog` & `os-traits-3.0.0/ChangeLog`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,35 @@
 CHANGES
 =======
 
+3.0.0
+-----
+
+* Comment to the trait was added
+* Add 'COMPUTE\_NET\_VIRTIO\_PACKED'
+
+2.10.0
+------
+
+* Add 'COMPUTE\_SHARE\_LOCAL\_FS'
+* Add new 'COMPUTE\_ADDRESS\_SPACE\_\*' traits
+* Update python classifier for python 3.10
+
 2.9.0
 -----
 
 * add new trait for config drive regeneration
 
 2.8.0
 -----
 
 * Add traits for vIOMMU
 * Add COMPUTE\_MANAGED\_PCI\_DEVICE trait
 * Add 'COMPUTE\_STORAGE\_VIRTIO\_FS', 'COMPUTE\_MEM\_BACKING\_FILE'
+* Update python testing as per zed cycle testing runtime
 * Add nova and cyborg owner traits for resources
 * Remove unnecessary unicode prefixes
 * Update CI to use unversioned jobs template
 
 2.7.0
 -----
```

### Comparing `os-traits-2.9.0/LICENSE` & `os-traits-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/PKG-INFO` & `os-traits-3.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-traits
-Version: 2.9.0
+Version: 3.0.0
 Summary: A library containing standardized trait strings
 Home-page: https://docs.openstack.org/os-traits/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =========
         os-traits
@@ -30,14 +30,13 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
```

### Comparing `os-traits-2.9.0/README.rst` & `os-traits-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/ext/traits.py` & `os-traits-3.0.0/doc/ext/traits.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/source/conf.py` & `os-traits-3.0.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/source/contributor/index.rst` & `os-traits-3.0.0/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/source/index.rst` & `os-traits-3.0.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/source/reference/index.rst` & `os-traits-3.0.0/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/doc/source/user/index.rst` & `os-traits-3.0.0/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/__init__.py` & `os-traits-3.0.0/os_traits/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/__init__.py` & `os-traits-3.0.0/os_traits/compute/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,8 +40,14 @@
     'REMOTE_MANAGED_PORTS',
     # The compute manager is configured to support file-backed memory.
     # https://docs.openstack.org/nova/latest/admin/file-backed-memory.html
     'MEM_BACKING_FILE',
     # Nova use this to indicate that an RP has inventories of PCI device(s)
     # managed by the nova-compute service
     'MANAGED_PCI_DEVICE',
+    # The virt driver supports pass-through or emulated modes for guest
+    # physical address bits.
+    'ADDRESS_SPACE_PASSTHROUGH',
+    'ADDRESS_SPACE_EMULATED',
+    # The compute manager supports share local fs (via virtiofs)
+    'SHARE_LOCAL_FS',
 ]
```

### Comparing `os-traits-2.9.0/os_traits/compute/arch.py` & `os-traits-3.0.0/os_traits/compute/arch.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/config_drive.py` & `os-traits-3.0.0/os_traits/compute/config_drive.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/ephemeral.py` & `os-traits-3.0.0/os_traits/compute/ephemeral.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/firmware.py` & `os-traits-3.0.0/os_traits/compute/firmware.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/graphics.py` & `os-traits-3.0.0/os_traits/compute/graphics.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/image.py` & `os-traits-3.0.0/os_traits/compute/image.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/migrate.py` & `os-traits-3.0.0/os_traits/compute/migrate.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/net.py` & `os-traits-3.0.0/os_traits/compute/net.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 
 TRAITS = [
     # The virt driver supports attaching a network interface after boot
     'ATTACH_INTERFACE',
     # The virt driver supports attaching a network interface after boot and
     # specifying a device tag for the interface
     'ATTACH_INTERFACE_WITH_TAG',
-
+    # The virt driver supports Packed virtqueue format
+    'VIRTIO_PACKED',
     # traits corresponding to the allowed values of "hw_vif_model"
     # image metadata property
     # https://github.com/openstack/nova/blob/1f74441/nova/network/model.py#L136-L149
     'VIF_MODEL_E1000',
     'VIF_MODEL_E1000E',
     'VIF_MODEL_LAN9118',
     'VIF_MODEL_NETFRONT',
```

### Comparing `os-traits-2.9.0/os_traits/compute/security.py` & `os-traits-3.0.0/os_traits/compute/security.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/status.py` & `os-traits-3.0.0/os_traits/compute/status.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/storage.py` & `os-traits-3.0.0/os_traits/compute/storage.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/viommu.py` & `os-traits-3.0.0/os_traits/compute/viommu.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/compute/volume.py` & `os-traits-3.0.0/os_traits/compute/volume.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/arch.py` & `os-traits-3.0.0/os_traits/hw/arch.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/__init__.py` & `os-traits-3.0.0/os_traits/hw/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/aarch64.py` & `os-traits-3.0.0/os_traits/hw/cpu/aarch64.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/amd.py` & `os-traits-3.0.0/os_traits/hw/cpu/amd.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/ppc64le/__init__.py` & `os-traits-3.0.0/os_traits/hw/cpu/ppc64le/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/x86/__init__.py` & `os-traits-3.0.0/os_traits/hw/cpu/x86/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/x86/amd.py` & `os-traits-3.0.0/os_traits/hw/cpu/x86/amd.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/cpu/x86/intel.py` & `os-traits-3.0.0/os_traits/hw/cpu/x86/intel.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/gpu/api.py` & `os-traits-3.0.0/os_traits/hw/gpu/api.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/gpu/cuda.py` & `os-traits-3.0.0/os_traits/hw/gpu/cuda.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/gpu/max_display_heads.py` & `os-traits-3.0.0/os_traits/hw/gpu/max_display_heads.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/gpu/resolution.py` & `os-traits-3.0.0/os_traits/hw/gpu/resolution.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/nic/__init__.py` & `os-traits-3.0.0/os_traits/hw/nic/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/nic/accel.py` & `os-traits-3.0.0/os_traits/hw/nic/accel.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/nic/dcb.py` & `os-traits-3.0.0/os_traits/hw/nic/dcb.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/nic/offload.py` & `os-traits-3.0.0/os_traits/hw/nic/offload.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/nic/sriov.py` & `os-traits-3.0.0/os_traits/hw/nic/sriov.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/hw/numa/__init__.py` & `os-traits-3.0.0/os_traits/hw/numa/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/misc/__init__.py` & `os-traits-3.0.0/os_traits/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/owner/__init__.py` & `os-traits-3.0.0/os_traits/owner/__init__.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/storage/disk.py` & `os-traits-3.0.0/os_traits/storage/disk.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/tests/base.py` & `os-traits-3.0.0/os_traits/tests/base.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/tests/test_cuda.py` & `os-traits-3.0.0/os_traits/tests/test_cuda.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits/tests/test_os_traits.py` & `os-traits-3.0.0/os_traits/tests/test_os_traits.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/os_traits.egg-info/PKG-INFO` & `os-traits-3.0.0/os_traits.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-traits
-Version: 2.9.0
+Version: 3.0.0
 Summary: A library containing standardized trait strings
 Home-page: https://docs.openstack.org/os-traits/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =========
         os-traits
@@ -30,14 +30,13 @@
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
+Requires-Python: >=3.8
```

### Comparing `os-traits-2.9.0/os_traits.egg-info/SOURCES.txt` & `os-traits-3.0.0/os_traits.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/releasenotes/source/conf.py` & `os-traits-3.0.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/setup.cfg` & `os-traits-3.0.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 name = os-traits
 summary = A library containing standardized trait strings
 description_file = 
 	README.rst
 author = OpenStack
 author_email = openstack-discuss@lists.openstack.org
 home_page = https://docs.openstack.org/os-traits/latest/
-python_requires = >=3.6
+python_requires = >=3.8
 classifier = 
 	Environment :: OpenStack
 	Intended Audience :: Information Technology
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Operating System :: POSIX :: Linux
 	Programming Language :: Python
 	Programming Language :: Python :: 3
-	Programming Language :: Python :: 3.6
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: Implementation :: CPython
 
 [files]
 packages = 
 	os_traits
```

### Comparing `os-traits-2.9.0/setup.py` & `os-traits-3.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `os-traits-2.9.0/tox.ini` & `os-traits-3.0.0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 minversion = 3.18.0
-envlist = py39,pep8
+envlist = py3,pep8
 ignore_basepython_conflict = true
 
 [testenv]
 basepython = python3
 allowlist_externals =
   rm
 deps =
```

