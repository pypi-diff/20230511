# Comparing `tmp/os-brick-6.2.1.tar.gz` & `tmp/os-brick-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "os-brick-6.2.1.tar", last modified: Tue May  2 16:00:58 2023, max compression
+gzip compressed data, was "os-brick-6.2.2.tar", last modified: Thu May 11 09:18:15 2023, max compression
```

## Comparing `os-brick-6.2.1.tar` & `os-brick-6.2.2.tar`

### file list

```diff
@@ -1,292 +1,293 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.477865 os-brick-6.2.1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-02 16:00:25.000000 os-brick-6.2.1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-02 16:00:25.000000 os-brick-6.2.1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-05-02 16:00:25.000000 os-brick-6.2.1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2023-05-02 16:00:25.000000 os-brick-6.2.1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6748 2023-05-02 16:00:58.000000 os-brick-6.2.1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-05-02 16:00:25.000000 os-brick-6.2.1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29923 2023-05-02 16:00:57.000000 os-brick-6.2.1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-02 16:00:25.000000 os-brick-6.2.1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-02 16:00:25.000000 os-brick-6.2.1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-02 16:00:58.477865 os-brick-6.2.1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-05-02 16:00:25.000000 os-brick-6.2.1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2023-05-02 16:00:25.000000 os-brick-6.2.1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.421868 os-brick-6.2.1/doc/source/reference/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/exception.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/doc/source/reference/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/initiator/connector.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/reference/os_brick/initiator/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-05-02 16:00:25.000000 os-brick-6.2.1/doc/source/user/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.409869 os-brick-6.2.1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.409869 os-brick-6.2.1/etc/os-brick/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/etc/os-brick/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-02 16:00:25.000000 os-brick-6.2.1/etc/os-brick/rootwrap.d/os-brick.filters
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-05-02 16:00:25.000000 os-brick-6.2.1/mypy-files.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/os_brick/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/caches/opencas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8404 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/encryptors/nop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.429868 os-brick-6.2.1/os_brick/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8025 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fake.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18094 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4003 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57916 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56888 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20407 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/connectors/vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/initiator_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13100 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32119 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/initiator/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4569 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/initiator/windows/smbfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34702 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/local_dev/lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.437867 os-brick-6.2.1/os_brick/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/rootwrap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/privileged/scaleio.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5513 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/remotefs/windows_remotefs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/caches/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/test_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/caches/test_opencas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.441867 os-brick-6.2.1/os_brick/tests/encryptors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_cryptsetup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11941 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_luks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/encryptors/test_nop.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.445867 os-brick-6.2.1/os_brick/tests/initiator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/initiator/connectors/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38122 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3720 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_huawei.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85008 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_lightos.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_local.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    96258 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13651 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_scaleio.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_storpool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/connectors/test_vmware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13407 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_host_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25343 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxfc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8497 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxrbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64131 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_linuxscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/initiator/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/local_dev/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/fake_lvm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/local_dev/test_brick_lvm.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8114 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_nvmeof.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/privileged/test_rootwrap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.449867 os-brick-6.2.1/os_brick/tests/remotefs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/test_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/remotefs/test_windows_remotefs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_brick.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_executor.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25526 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.453866 os-brick-6.2.1/os_brick/tests/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/fake_win_conn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_base_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_factory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_fibre_channel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_iscsi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_rbd.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/tests/windows/test_smbfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14715 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-05-02 16:00:25.000000 os-brick-6.2.1/os_brick/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.425868 os-brick-6.2.1/os_brick.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10825 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-05-02 16:00:58.000000 os-brick-6.2.1/os_brick.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-05-02 16:00:25.000000 os-brick-6.2.1/pylintrc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.413869 os-brick-6.2.1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.469865 os-brick-6.2.1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/encryption-a642889a82ff9207.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.473865 os-brick-6.2.1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-02 16:00:25.000000 os-brick-6.2.1/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-05-02 16:00:25.000000 os-brick-6.2.1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-05-02 16:00:58.477865 os-brick-6.2.1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-02 16:00:25.000000 os-brick-6.2.1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-05-02 16:00:25.000000 os-brick-6.2.1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-02 16:00:58.477865 os-brick-6.2.1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/generate_connector_list.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/lintstack.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/lintstack.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-05-02 16:00:25.000000 os-brick-6.2.1/tools/mypywrap.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-05-02 16:00:25.000000 os-brick-6.2.1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.674141 os-brick-6.2.2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-05-11 09:17:51.000000 os-brick-6.2.2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2023-05-11 09:17:51.000000 os-brick-6.2.2/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-05-11 09:17:51.000000 os-brick-6.2.2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2023-05-11 09:17:51.000000 os-brick-6.2.2/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6748 2023-05-11 09:18:15.000000 os-brick-6.2.2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      603 2023-05-11 09:17:51.000000 os-brick-6.2.2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29971 2023-05-11 09:18:15.000000 os-brick-6.2.2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 09:17:51.000000 os-brick-6.2.2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-05-11 09:17:51.000000 os-brick-6.2.2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-11 09:18:15.674141 os-brick-6.2.2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-05-11 09:17:51.000000 os-brick-6.2.2/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1884 2023-05-11 09:17:51.000000 os-brick-6.2.2/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.626127 os-brick-6.2.2/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      706 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/reference/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/reference/os_brick/exception.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/reference/os_brick/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/reference/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1101 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/reference/os_brick/initiator/connector.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/reference/os_brick/initiator/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2023-05-11 09:17:51.000000 os-brick-6.2.2/doc/source/user/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.622126 os-brick-6.2.2/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.622126 os-brick-6.2.2/etc/os-brick/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/etc/os-brick/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2023-05-11 09:17:51.000000 os-brick-6.2.2/etc/os-brick/rootwrap.d/os-brick.filters
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2023-05-11 09:17:51.000000 os-brick-6.2.2/mypy-files.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.630128 os-brick-6.2.2/os_brick/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1114 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.634129 os-brick-6.2.2/os_brick/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3377 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4197 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/caches/opencas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.634129 os-brick-6.2.2/os_brick/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5487 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2326 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/encryptors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7531 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/encryptors/cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8404 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/encryptors/luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1605 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/encryptors/nop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      857 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.634129 os-brick-6.2.2/os_brick/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11636 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.642132 os-brick-6.2.2/os_brick/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8025 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2288 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1629 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/fake.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19013 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1979 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4185 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1597 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57916 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13060 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3018 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56888 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18651 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5154 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20407 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10364 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/connectors/vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1182 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9607 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/initiator_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13100 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8202 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32866 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1840 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.642132 os-brick-6.2.2/os_brick/initiator/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4569 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8427 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6727 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5195 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/initiator/windows/smbfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.642132 os-brick-6.2.2/os_brick/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34702 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/local_dev/lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.642132 os-brick-6.2.2/os_brick/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1262 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      947 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3532 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2059 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9466 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/rootwrap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2948 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/privileged/scaleio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.646133 os-brick-6.2.2/os_brick/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11191 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/remotefs/remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5513 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/remotefs/windows_remotefs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.646133 os-brick-6.2.2/os_brick/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4800 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.646133 os-brick-6.2.2/os_brick/tests/caches/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/caches/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4883 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/caches/test_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6700 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/caches/test_opencas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.646133 os-brick-6.2.2/os_brick/tests/encryptors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/encryptors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8054 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/encryptors/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6846 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/encryptors/test_cryptsetup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11941 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/encryptors/test_luks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1611 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/encryptors/test_nop.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.650134 os-brick-6.2.2/os_brick/tests/initiator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.654135 os-brick-6.2.2/os_brick/tests/initiator/connectors/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3984 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_base_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3137 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_base_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44571 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5024 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_gpfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10535 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_huawei.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85008 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3430 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_iser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10989 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_lightos.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2284 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_local.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    96258 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25104 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3323 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13651 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_scaleio.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6831 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_storpool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18260 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/connectors/test_vmware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13407 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_host_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25343 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_linuxfc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8497 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_linuxrbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    66885 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_linuxscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3348 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/initiator/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.654135 os-brick-6.2.2/os_brick/tests/local_dev/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/local_dev/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/local_dev/fake_lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18676 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/local_dev/test_brick_lvm.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.654135 os-brick-6.2.2/os_brick/tests/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8114 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/privileged/test_nvmeof.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3528 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/privileged/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9226 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/privileged/test_rootwrap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.654135 os-brick-6.2.2/os_brick/tests/remotefs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/remotefs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11848 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/remotefs/test_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6632 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/remotefs/test_windows_remotefs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      744 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/test_brick.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2208 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6655 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/test_executor.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25526 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.658136 os-brick-6.2.2/os_brick/tests/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/fake_win_conn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1378 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5795 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_base_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1562 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_factory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11642 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_fibre_channel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9125 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_iscsi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5340 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_rbd.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7736 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/tests/windows/test_smbfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14715 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2023-05-11 09:17:51.000000 os-brick-6.2.2/os_brick/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.634129 os-brick-6.2.2/os_brick.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10886 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2023-05-11 09:18:15.000000 os-brick-6.2.2/os_brick.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-05-11 09:17:51.000000 os-brick-6.2.2/pylintrc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.622126 os-brick-6.2.2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.670140 os-brick-6.2.2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add-luks2-support-13563cfe83aba69c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add-vstorage-protocol-b536f4e21d764801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add-windows-fibre-channel-030c095c149da321.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add-windows-iscsi-15d6b1392695f978.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       55 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add-windows-smbfs-d86edaa003130a31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/add_custom_keyring_for_rbd_connection-eccbaae9ee5f3491.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bp-lightbits-lightos-clustered-nvmetcp-connector-fd8dfd73330973e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1722432-2408dab55c903c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      520 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1492 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1862443-e87ef38b60f9b979.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      620 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1884052-798094496dccf23c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1888675-mpath-resize-6013ce39fa2b8401.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1915678-901a6bd24ecede72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1924652-2323f905f62ef8ba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1929223-powerflex-connector-certificate-validation-cf9ffc98391115d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1938870-af85c420d1a108a9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1944474-55c5ebb3a37801aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-1945323-4140f5aff3558082.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/bug-nvmeof-connector-support-multipath-kernels-ff6f1f27fdea2c8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/default-timeout-26c838af8b7af9fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/delay-legacy-encryption-provider-name-deprecation-c0d07be3f0d92afd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/deprecate-plain-cryptsetup-encryptor-0a279abc0b0d718c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/disconnect-multipath-cfg-changed-637abc5ecf44fb10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/encryption-a642889a82ff9207.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fc-force-disconnect-1a33cf46c233dd04.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/iscsi_manual_scan_support-d64a1c3c8e1986b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/local-attach-in-rbd-connector-c06347fb164b084a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/lock_path-c1c58a253391b41c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/lvm-delete-error-76f2cc9d8dc91f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/multipath-improvements-596c2c6eadfba6ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/multipath-nvme-f77a53eb2717a44c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/no-systool-use-b7bc430de1033670.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      156 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvme-flush-f31ab337224e5d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvme-hostnqn-c2611dc56729183b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvme-rsd-support-d487afd77c534fa1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1740 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvmeof-disconnect-83f9aaf17f8c8988.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvmeof-hide-traceback-a968ab71352684e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/nvmeof-multiple-volumes-within-subsystem-support-05879c1c3bdf52c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/privsep-logs-9e938e5a2aee042e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/rbd-disconnect-failure-9efa6932df40271b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/rbd-non-openstack-support-28ee093d7d3a700e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/rbd-windows-support-ef6e8184842409dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/rbd_check_valid_device-2f50c0639adb8e7c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/rbd_extend_volume-5bc6adc08f662c5b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/refactor_iscsi_connect-dfbb24305a954783.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/refactor_iscsi_disconnect-557f4173bc1ae4ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-aoe-7a97315a73c7b24f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-bug-1633518-workaround-75c2e26843660696.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-disco-0809537ffb8c50eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-drbd-21872230fcac1138.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-hgst-daa7f07c307974d0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-hyperscale-468f1b61bf4dadf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-old-constants-20021f5b30bde890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      205 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/remove-sheepdog-611257b28bc88934.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/scaleio-extend-attached-ec44d3a72395882c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       57 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/start-using-reno-23e8d5f1a30851a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/update-nvmeof-connector-6260a658c15a9a6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      177 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/ussuri-release-979d709dfa7df068.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/veritas-hyperscale-connector-fe56cec68b1947cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/vmware-vmdk-connector-19e6999e6cae43cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/notes/yoga-known-issues-f1248af0e328d63e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.674141 os-brick-6.2.2/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.674141 os-brick-6.2.2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.674141 os-brick-6.2.2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1732 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-05-11 09:17:51.000000 os-brick-6.2.2/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2023-05-11 09:17:51.000000 os-brick-6.2.2/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1329 2023-05-11 09:18:15.678142 os-brick-6.2.2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-05-11 09:17:51.000000 os-brick-6.2.2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2023-05-11 09:17:51.000000 os-brick-6.2.2/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-05-11 09:18:15.674141 os-brick-6.2.2/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2023-05-11 09:17:51.000000 os-brick-6.2.2/tools/fast8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6189 2023-05-11 09:17:51.000000 os-brick-6.2.2/tools/generate_connector_list.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6793 2023-05-11 09:17:51.000000 os-brick-6.2.2/tools/lintstack.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2182 2023-05-11 09:17:51.000000 os-brick-6.2.2/tools/lintstack.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2023-05-11 09:17:51.000000 os-brick-6.2.2/tools/mypywrap.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4604 2023-05-11 09:17:51.000000 os-brick-6.2.2/tox.ini
```

### Comparing `os-brick-6.2.1/.zuul.yaml` & `os-brick-6.2.2/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/AUTHORS` & `os-brick-6.2.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/CONTRIBUTING.rst` & `os-brick-6.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/ChangeLog` & `os-brick-6.2.2/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 CHANGES
 =======
 
+6.2.2
+-----
+
+* Support force disconnect for FC
+
 6.2.1
 -----
 
 * Add Python 3.10 to setup.cfg metadata
 * Update TOX\_CONSTRAINTS\_FILE for stable/2023.1
 * Update .gitreview for stable/2023.1
```

### Comparing `os-brick-6.2.1/LICENSE` & `os-brick-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/PKG-INFO` & `os-brick-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.2.1
+Version: 6.2.2
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
```

### Comparing `os-brick-6.2.1/README.rst` & `os-brick-6.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/bindep.txt` & `os-brick-6.2.2/bindep.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/doc/source/conf.py` & `os-brick-6.2.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/doc/source/contributor/contributing.rst` & `os-brick-6.2.2/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/doc/source/reference/os_brick/exception.rst` & `os-brick-6.2.2/doc/source/reference/os_brick/exception.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/doc/source/reference/os_brick/initiator/connector.rst` & `os-brick-6.2.2/doc/source/reference/os_brick/initiator/connector.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/doc/source/user/tutorial.rst` & `os-brick-6.2.2/doc/source/user/tutorial.rst`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/mypy-files.txt` & `os-brick-6.2.2/mypy-files.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/__init__.py` & `os-brick-6.2.2/os_brick/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/caches/__init__.py` & `os-brick-6.2.2/os_brick/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/caches/opencas.py` & `os-brick-6.2.2/os_brick/caches/opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/encryptors/__init__.py` & `os-brick-6.2.2/os_brick/encryptors/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/encryptors/base.py` & `os-brick-6.2.2/os_brick/encryptors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/encryptors/cryptsetup.py` & `os-brick-6.2.2/os_brick/encryptors/cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/encryptors/luks.py` & `os-brick-6.2.2/os_brick/encryptors/luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/encryptors/nop.py` & `os-brick-6.2.2/os_brick/encryptors/nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/exception.py` & `os-brick-6.2.2/os_brick/exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/executor.py` & `os-brick-6.2.2/os_brick/executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/i18n.py` & `os-brick-6.2.2/os_brick/i18n.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/__init__.py` & `os-brick-6.2.2/os_brick/initiator/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connector.py` & `os-brick-6.2.2/os_brick/initiator/connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/base.py` & `os-brick-6.2.2/os_brick/initiator/connectors/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/base_iscsi.py` & `os-brick-6.2.2/os_brick/initiator/connectors/base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/base_rbd.py` & `os-brick-6.2.2/os_brick/initiator/connectors/base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/fake.py` & `os-brick-6.2.2/os_brick/initiator/connectors/fake.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel.py` & `os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         :param device_info: historical difference, but same as connection_props
         :type device_info: dict
 
         connection_properties for Fibre Channel must include:
         target_wwn - World Wide Name
         target_lun - LUN id of the volume
         """
-
+        exc = exception.ExceptionChainer()
         devices = []
         wwn = None
 
         connection_properties = self._add_targets_to_connection_properties(
             connection_properties)
 
         volume_paths = self.get_volume_paths(connection_properties)
@@ -364,45 +364,63 @@
         for path in volume_paths:
             real_path = self._linuxscsi.get_name_from_path(path)
             if (self.use_multipath and not mpath_path
                     and self.check_valid_device(path)):
                 wwn = self._linuxscsi.get_scsi_wwn(path)
                 mpath_path = self._linuxscsi.find_multipath_device_path(wwn)
                 if mpath_path:
-                    self._linuxscsi.flush_multipath_device(mpath_path)
+                    with exc.context(force, 'Flushing %s failed', mpath_path):
+                        self._linuxscsi.flush_multipath_device(mpath_path)
             real_path = typing.cast(str, real_path)
             dev_info = self._linuxscsi.get_device_info(real_path)
             devices.append(dev_info)
 
+        # If flush failed, then remove it forcefully since force=True
+        if mpath_path and exc:
+            with exc.context(force, 'Removing multipath %s failed',
+                             mpath_path):
+                mpath_name = os.path.basename(os.path.realpath(mpath_path))
+                self._linuxscsi.multipath_del_map(mpath_name)
+
         LOG.debug("devices to remove = %s", devices)
-        self._remove_devices(connection_properties, devices, device_info)
+        self._remove_devices(connection_properties, devices, device_info,
+                             force, exc)
+
+        if exc:  # type: ignore
+            LOG.warning('There were errors removing %s, leftovers may remain '
+                        'in the system', volume_paths)
+            if not ignore_errors:
+                raise exc  # type: ignore
 
     def _remove_devices(self,
                         connection_properties: dict,
                         devices: list,
-                        device_info: dict) -> None:
+                        device_info: dict,
+                        force: bool,
+                        exc) -> None:
         # There may have been more than 1 device mounted
         # by the kernel for this volume.  We have to remove
         # all of them
         path_used = utils.get_dev_path(connection_properties, device_info)
         # NOTE: Due to bug #1897787 device_info may have a real path for some
         # single paths instead of a symlink as it should have, so it'll only
         # be a multipath if it was a symlink (not real path) and it wasn't a
         # single path symlink (those have filenames starting with pci-)
         # We don't use os.path.islink in case the file is no longer there.
         was_symlink = path_used.count(os.sep) > 2
         # We check for /pci because that's the value we return for single
         # paths, whereas for multipaths we have multiple link formats.
         was_multipath = '/pci-' not in path_used and was_symlink
         for device in devices:
-            device_path = device['device']
-            flush = self._linuxscsi.requires_flush(device_path,
-                                                   path_used,
-                                                   was_multipath)
-            self._linuxscsi.remove_scsi_device(device_path, flush=flush)
+            with exc.context(force, 'Removing device %s failed', device):
+                device_path = device['device']
+                flush = self._linuxscsi.requires_flush(device_path,
+                                                       path_used,
+                                                       was_multipath)
+                self._linuxscsi.remove_scsi_device(device_path, flush=flush)
 
     def _get_pci_num(self, hba: Optional[dict]) -> tuple:
         # NOTE(walter-boring)
         # device path is in format of (FC and FCoE) :
         # /sys/devices/pci0000:00/0000:00:03.0/0000:05:00.3/host2/fc_host/host2
         # /sys/devices/pci0000:20/0000:20:03.0/0000:21:00.2/net/ens2f2/ctlr_2
         # /host3/fc_host/host3
```

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_ppc64.py` & `os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/fibre_channel_s390x.py` & `os-brick-6.2.2/os_brick/initiator/connectors/fibre_channel_s390x.py`

 * *Files 5% similar despite different names*

```diff
@@ -82,16 +82,19 @@
                 pci_num, target_wwn, lun),
             # Debian based (e.g. for ds8k)
             "/dev/disk/by-path/ccw-%s-fc-%s-lun-%s" % (
                 pci_num, target_wwn, self._get_lun_string(lun)),
         ]
         return host_device
 
-    def _remove_devices(self, connection_properties, devices, device_info):
+    def _remove_devices(self, connection_properties, devices, device_info,
+                        force, exc):
         hbas = self._linuxfc.get_fc_hbas_info()
         targets = connection_properties['targets']
         possible_devs = self._get_possible_devices(hbas, targets)
         for platform, pci_num, target_wwn, lun in possible_devs:
             target_lun = self._get_lun_string(lun)
-            self._linuxfc.deconfigure_scsi_device(pci_num,
-                                                  target_wwn,
-                                                  target_lun)
+            with exc.context(force, 'Removing device %s:%s:%s failed',
+                             pci_num, target_wwn, target_lun):
+                self._linuxfc.deconfigure_scsi_device(pci_num,
+                                                      target_wwn,
+                                                      target_lun)
```

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/gpfs.py` & `os-brick-6.2.2/os_brick/initiator/connectors/gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/huawei.py` & `os-brick-6.2.2/os_brick/initiator/connectors/huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/iscsi.py` & `os-brick-6.2.2/os_brick/initiator/connectors/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/lightos.py` & `os-brick-6.2.2/os_brick/initiator/connectors/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/local.py` & `os-brick-6.2.2/os_brick/initiator/connectors/local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/nvmeof.py` & `os-brick-6.2.2/os_brick/initiator/connectors/nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/rbd.py` & `os-brick-6.2.2/os_brick/initiator/connectors/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/remotefs.py` & `os-brick-6.2.2/os_brick/initiator/connectors/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/scaleio.py` & `os-brick-6.2.2/os_brick/initiator/connectors/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/storpool.py` & `os-brick-6.2.2/os_brick/initiator/connectors/storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/connectors/vmware.py` & `os-brick-6.2.2/os_brick/initiator/connectors/vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/host_driver.py` & `os-brick-6.2.2/os_brick/initiator/host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/initiator_connector.py` & `os-brick-6.2.2/os_brick/initiator/initiator_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/linuxfc.py` & `os-brick-6.2.2/os_brick/initiator/linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/linuxrbd.py` & `os-brick-6.2.2/os_brick/initiator/linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/linuxscsi.py` & `os-brick-6.2.2/os_brick/initiator/linuxscsi.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,7 +755,25 @@
     def multipath_del_path(self, realpath):
         """Remove a path from multipathd for monitoring."""
         stdout, stderr = self._execute('multipathd', 'del', 'path', realpath,
                                        run_as_root=True, timeout=5,
                                        check_exit_code=False,
                                        root_helper=self._root_helper)
         return stdout.strip() == 'ok'
+
+    @utils.retry((putils.ProcessExecutionError, exception.BrickException),
+                 retries=3)
+    def multipath_del_map(self, mpath):
+        """Stop monitoring a multipath given its device name (eg: dm-7).
+
+        Method ensures that the multipath device mapper actually dissapears
+        from sysfs.
+        """
+        map_name = self.get_dm_name(mpath)
+        if map_name:
+            self._execute('multipathd', 'del', 'map', map_name,
+                          run_as_root=True, timeout=5,
+                          root_helper=self._root_helper)
+
+        if map_name and self.get_dm_name(mpath):
+            raise exception.BrickException("Multipath doesn't go away")
+        LOG.debug('Multipath %s no longer present', mpath)
```

### Comparing `os-brick-6.2.1/os_brick/initiator/utils.py` & `os-brick-6.2.2/os_brick/initiator/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/windows/base.py` & `os-brick-6.2.2/os_brick/initiator/windows/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/windows/fibre_channel.py` & `os-brick-6.2.2/os_brick/initiator/windows/fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/windows/iscsi.py` & `os-brick-6.2.2/os_brick/initiator/windows/iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/windows/rbd.py` & `os-brick-6.2.2/os_brick/initiator/windows/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/initiator/windows/smbfs.py` & `os-brick-6.2.2/os_brick/initiator/windows/smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/local_dev/lvm.py` & `os-brick-6.2.2/os_brick/local_dev/lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/opts.py` & `os-brick-6.2.2/os_brick/opts.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/__init__.py` & `os-brick-6.2.2/os_brick/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/lightos.py` & `os-brick-6.2.2/os_brick/privileged/lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/nvmeof.py` & `os-brick-6.2.2/os_brick/privileged/nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/rbd.py` & `os-brick-6.2.2/os_brick/privileged/rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/rootwrap.py` & `os-brick-6.2.2/os_brick/privileged/rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/privileged/scaleio.py` & `os-brick-6.2.2/os_brick/privileged/scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/remotefs/remotefs.py` & `os-brick-6.2.2/os_brick/remotefs/remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/remotefs/windows_remotefs.py` & `os-brick-6.2.2/os_brick/remotefs/windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/base.py` & `os-brick-6.2.2/os_brick/tests/base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/caches/test_init.py` & `os-brick-6.2.2/os_brick/tests/caches/test_init.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/caches/test_opencas.py` & `os-brick-6.2.2/os_brick/tests/caches/test_opencas.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/encryptors/test_base.py` & `os-brick-6.2.2/os_brick/tests/encryptors/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/encryptors/test_cryptsetup.py` & `os-brick-6.2.2/os_brick/tests/encryptors/test_cryptsetup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/encryptors/test_luks.py` & `os-brick-6.2.2/os_brick/tests/encryptors/test_luks.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/encryptors/test_nop.py` & `os-brick-6.2.2/os_brick/tests/encryptors/test_nop.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_iscsi.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_base_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_base_rbd.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_base_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel.py`

 * *Files 4% similar despite different names*

```diff
@@ -739,25 +739,61 @@
               ('/dev/disk/by-path/pci-1-fc-1-lun-1', False))
     @ddt.unpack
     @mock.patch('os_brick.initiator.linuxscsi.LinuxSCSI.remove_scsi_device')
     @mock.patch('os_brick.initiator.linuxscsi.LinuxSCSI.requires_flush')
     @mock.patch('os_brick.utils.get_dev_path')
     def test__remove_devices(self, path_used, was_multipath, get_dev_path_mock,
                              flush_mock, remove_mock):
+        exc = exception.ExceptionChainer()
         get_dev_path_mock.return_value = path_used
         self.connector._remove_devices(mock.sentinel.con_props,
                                        [{'device': '/dev/sda'}],
-                                       mock.sentinel.device_info)
+                                       mock.sentinel.device_info,
+                                       force=False, exc=exc)
+        self.assertFalse(bool(exc))
         get_dev_path_mock.assert_called_once_with(mock.sentinel.con_props,
                                                   mock.sentinel.device_info)
         flush_mock.assert_called_once_with('/dev/sda', path_used,
                                            was_multipath)
         remove_mock.assert_called_once_with('/dev/sda',
                                             flush=flush_mock.return_value)
 
+    @ddt.data(('/dev/mapper/<WWN>', True),
+              ('/dev/mapper/mpath0', True),
+              # Check real devices are properly detected as non multipaths
+              ('/dev/sda', False),
+              ('/dev/disk/by-path/pci-1-fc-1-lun-1', False))
+    @ddt.unpack
+    @mock.patch('os_brick.initiator.linuxscsi.LinuxSCSI.remove_scsi_device')
+    @mock.patch('os_brick.initiator.linuxscsi.LinuxSCSI.requires_flush')
+    @mock.patch('os_brick.utils.get_dev_path')
+    def test__remove_devices_fails(self, path_used, was_multipath,
+                                   get_dev_path_mock, flush_mock, remove_mock):
+        exc = exception.ExceptionChainer()
+        get_dev_path_mock.return_value = path_used
+        remove_mock.side_effect = Exception
+        self.connector._remove_devices(mock.sentinel.con_props,
+                                       [{'device': '/dev/sda'},
+                                        {'device': '/dev/sdb'}],
+                                       mock.sentinel.device_info,
+                                       force=True, exc=exc)
+        self.assertTrue(bool(exc))
+        get_dev_path_mock.assert_called_once_with(mock.sentinel.con_props,
+                                                  mock.sentinel.device_info)
+
+        expect_flush = [mock.call('/dev/sda', path_used, was_multipath),
+                        mock.call('/dev/sdb', path_used, was_multipath)]
+        self.assertEqual(len(expect_flush), flush_mock.call_count)
+        flush_mock.assert_has_calls(expect_flush)
+
+        expect_remove = [mock.call('/dev/sda', flush=flush_mock.return_value),
+                         mock.call('/dev/sdb', flush=flush_mock.return_value)]
+        self.assertEqual(len(expect_remove), remove_mock.call_count)
+        remove_mock.assert_has_calls(expect_remove)
+
     @mock.patch.object(linuxscsi.LinuxSCSI, 'find_multipath_device')
     @mock.patch.object(linuxscsi.LinuxSCSI, 'wait_for_rw')
     @mock.patch.object(os.path, 'exists', return_value=True)
     @mock.patch.object(os.path, 'realpath', return_value='/dev/sdb')
     @mock.patch.object(linuxfc.LinuxFibreChannel, 'get_fc_hbas')
     @mock.patch.object(linuxfc.LinuxFibreChannel, 'get_fc_hbas_info')
     @mock.patch.object(linuxscsi.LinuxSCSI, 'get_scsi_wwn')
@@ -811,7 +847,98 @@
                                          devices['devices'][0])
         expected_commands = [
             'multipath -f ' + find_mp_device_path_mock.return_value,
             'tee -a /sys/block/sdb/device/delete',
             'tee -a /sys/block/sdc/device/delete',
         ]
         self.assertEqual(expected_commands, self.cmds)
+
+    @ddt.data((False, Exception), (True, Exception), (False, None))
+    @ddt.unpack
+    @mock.patch.object(fibre_channel.FibreChannelConnector, '_remove_devices')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'multipath_del_map')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'flush_multipath_device')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'wait_for_rw')
+    @mock.patch.object(os.path, 'exists', return_value=True)
+    @mock.patch.object(os.path, 'realpath')
+    @mock.patch.object(linuxfc.LinuxFibreChannel, 'get_fc_hbas')
+    @mock.patch.object(linuxfc.LinuxFibreChannel, 'get_fc_hbas_info')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_scsi_wwn')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_device_info')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'find_multipath_device_path')
+    @mock.patch.object(base.BaseLinuxConnector, 'check_valid_device')
+    def test_disconnect_volume_fails(self, ignore_exc, side_effect,
+                                     check_valid_device_mock,
+                                     find_mp_device_path_mock,
+                                     get_device_info_mock,
+                                     get_scsi_wwn_mock,
+                                     get_fc_hbas_info_mock,
+                                     get_fc_hbas_mock,
+                                     realpath_mock,
+                                     exists_mock,
+                                     wait_for_rw_mock,
+                                     flush_mock,
+                                     del_map_mock,
+                                     remove_mock):
+
+        flush_mock.side_effect = side_effect
+        del_map_mock.side_effect = side_effect
+
+        check_valid_device_mock.return_value = True
+        self.connector.use_multipath = True
+        get_fc_hbas_mock.side_effect = self.fake_get_fc_hbas
+        get_fc_hbas_info_mock.side_effect = self.fake_get_fc_hbas_info
+
+        wwn = '360002ac00000000000000b860000741c'
+        multipath_devname = f'/dev/disk/by-id/dm-uuid-mpath-{wwn}'
+        realpath_mock.return_value = '/dev/dm-1'
+        devices = {"device": multipath_devname,
+                   "id": wwn,
+                   "devices": [{'device': '/dev/sdb',
+                                'address': '1:0:0:1',
+                                'host': 1, 'channel': 0,
+                                'id': 0, 'lun': 1},
+                               {'device': '/dev/sdc',
+                                'address': '1:0:0:2',
+                                'host': 1, 'channel': 0,
+                                'id': 0, 'lun': 1}]}
+        get_device_info_mock.side_effect = devices['devices']
+        get_scsi_wwn_mock.return_value = wwn
+
+        location = '10.0.2.15:3260'
+        name = 'volume-00000001'
+        vol = {'id': 1, 'name': name}
+        initiator_wwn = ['1234567890123456', '1234567890123457']
+
+        find_mp_device_path_mock.return_value = '/dev/mapper/mpatha'
+
+        connection_info = self.fibrechan_connection(vol, location,
+                                                    initiator_wwn)
+        if side_effect and not ignore_exc:
+            self.assertRaises(exception.ExceptionChainer,
+                              self.connector.disconnect_volume,
+                              connection_info['data'], devices['devices'][0],
+                              force=True, ignore_errors=ignore_exc)
+        else:
+            self.connector.disconnect_volume(connection_info['data'],
+                                             devices['devices'][0],
+                                             force=True,
+                                             ignore_errors=ignore_exc)
+
+        flush_mock.assert_called_once_with(
+            find_mp_device_path_mock.return_value)
+
+        expected = [
+            mock.call(f'/dev/disk/by-path/pci-0000:05:00.2-fc-0x{wwn}-lun-1')
+            for wwn in initiator_wwn]
+        if side_effect:
+            del_map_mock.assert_called_once_with('dm-1')
+            expected.append(mock.call(find_mp_device_path_mock.return_value))
+        else:
+            del_map_mock.assert_not_called()
+
+        remove_mock.assert_called_once_with(connection_info['data'],
+                                            devices['devices'],
+                                            devices['devices'][0],
+                                            True, mock.ANY)
+        self.assertEqual(len(expected), realpath_mock.call_count)
+        realpath_mock.assert_has_calls(expected)
```

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel_ppc64.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_fibre_channel_s390x.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 from unittest import mock
 
+from os_brick import exception
 from os_brick.initiator.connectors import fibre_channel_s390x
 from os_brick.initiator import linuxfc
 from os_brick.tests.initiator import test_connector
 
 
 class FibreChannelConnectorS390XTestCase(test_connector.ConnectorTestCase):
 
@@ -62,14 +63,36 @@
                        '_get_possible_devices', return_value=[('', 3, 5, 2), ])
     @mock.patch.object(linuxfc.LinuxFibreChannelS390X, 'get_fc_hbas_info',
                        return_value=[])
     @mock.patch.object(linuxfc.LinuxFibreChannelS390X,
                        'deconfigure_scsi_device')
     def test_remove_devices(self, mock_deconfigure_scsi_device,
                             mock_get_fc_hbas_info, mock_get_possible_devices):
+        exc = exception.ExceptionChainer()
         connection_properties = {'targets': [5, 2]}
         self.connector._remove_devices(connection_properties, devices=None,
-                                       device_info=None)
+                                       device_info=None, force=False, exc=exc)
         mock_deconfigure_scsi_device.assert_called_with(3, 5,
                                                         "0x0002000000000000")
         mock_get_fc_hbas_info.assert_called_once_with()
         mock_get_possible_devices.assert_called_once_with([], [5, 2])
+        self.assertFalse(bool(exc))
+
+    @mock.patch.object(fibre_channel_s390x.FibreChannelConnectorS390X,
+                       '_get_possible_devices', return_value=[('', 3, 5, 2), ])
+    @mock.patch.object(linuxfc.LinuxFibreChannelS390X, 'get_fc_hbas_info',
+                       return_value=[])
+    @mock.patch.object(linuxfc.LinuxFibreChannelS390X,
+                       'deconfigure_scsi_device')
+    def test_remove_devices_force(self, mock_deconfigure_scsi_device,
+                                  mock_get_fc_hbas_info,
+                                  mock_get_possible_devices):
+        exc = exception.ExceptionChainer()
+        mock_deconfigure_scsi_device.side_effect = Exception
+        connection_properties = {'targets': [5, 2]}
+        self.connector._remove_devices(connection_properties, devices=None,
+                                       device_info=None, force=True, exc=exc)
+        mock_deconfigure_scsi_device.assert_called_with(3, 5,
+                                                        "0x0002000000000000")
+        mock_get_fc_hbas_info.assert_called_once_with()
+        mock_get_possible_devices.assert_called_once_with([], [5, 2])
+        self.assertTrue(bool(exc))
```

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_gpfs.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_gpfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_huawei.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_huawei.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iscsi.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_iser.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_iser.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_lightos.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_lightos.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_local.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_local.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_nvmeof.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_rbd.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_remotefs.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_scaleio.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_scaleio.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_storpool.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_storpool.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/connectors/test_vmware.py` & `os-brick-6.2.2/os_brick/tests/initiator/connectors/test_vmware.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_connector.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_host_driver.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_host_driver.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_linuxfc.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_linuxfc.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_linuxrbd.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_linuxrbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_linuxscsi.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_linuxscsi.py`

 * *Files 2% similar despite different names*

```diff
@@ -1295,14 +1295,72 @@
         self.linuxscsi.multipath_add_path('/dev/sda')
         self.assertEqual(['multipathd add path /dev/sda'], self.cmds)
 
     def test_multipath_del_path(self):
         self.linuxscsi.multipath_del_path('/dev/sda')
         self.assertEqual(['multipathd del path /dev/sda'], self.cmds)
 
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_dm_name', return_value=None)
+    def test_multipath_del_map_not_present(self, name_mock):
+        self.linuxscsi.multipath_del_map('dm-7')
+        self.assertEqual([], self.cmds)
+        name_mock.assert_called_once_with('dm-7')
+
+    @mock.patch.object(linuxscsi.LinuxSCSI, '_execute')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_dm_name', return_value=None)
+    def test_multipath_del_map(self, name_mock, exec_mock):
+        exec_mock.side_effect = [putils.ProcessExecutionError, None]
+
+        mpath_name = '3600d0230000000000e13955cc3757800'
+        name_mock.side_effect = [mpath_name, mpath_name, None]
+        self.linuxscsi.multipath_del_map('dm-7')
+
+        self.assertEqual(2, exec_mock.call_count)
+        exec_mock.assert_has_calls(
+            [mock.call('multipathd', 'del', 'map', mpath_name,
+                       run_as_root=True, timeout=5,
+                       root_helper=self.linuxscsi._root_helper)] * 2)
+        self.assertEqual(3, name_mock.call_count)
+        name_mock.assert_has_calls([mock.call('dm-7')] * 3)
+
+    @mock.patch.object(linuxscsi.LinuxSCSI, '_execute')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_dm_name')
+    def test_multipath_del_map_retries_cmd_fails(self, name_mock, exec_mock):
+        exec_mock.side_effect = putils.ProcessExecutionError
+        mpath_name = '3600d0230000000000e13955cc3757800'
+        name_mock.return_value = mpath_name
+        self.assertRaises(putils.ProcessExecutionError,
+                          self.linuxscsi.multipath_del_map, 'dm-7')
+
+        self.assertEqual(3, exec_mock.call_count)
+        exec_mock.assert_has_calls(
+            [mock.call('multipathd', 'del', 'map', mpath_name,
+                       run_as_root=True, timeout=5,
+                       root_helper=self.linuxscsi._root_helper)] * 3)
+
+        self.assertEqual(3, name_mock.call_count)
+        name_mock.assert_has_calls([mock.call('dm-7')] * 3)
+
+    @mock.patch.object(linuxscsi.LinuxSCSI, '_execute')
+    @mock.patch.object(linuxscsi.LinuxSCSI, 'get_dm_name')
+    def test_multipath_del_map_retries_remains(self, name_mock, exec_mock):
+        mpath_name = '3600d0230000000000e13955cc3757800'
+        name_mock.return_value = mpath_name
+        self.assertRaises(exception.BrickException,
+                          self.linuxscsi.multipath_del_map, 'dm-7')
+
+        self.assertEqual(3, exec_mock.call_count)
+        exec_mock.assert_has_calls(
+            [mock.call('multipathd', 'del', 'map', mpath_name,
+                       run_as_root=True, timeout=5,
+                       root_helper=self.linuxscsi._root_helper)] * 3)
+
+        self.assertEqual(6, name_mock.call_count)
+        name_mock.assert_has_calls([mock.call('dm-7')] * 6)
+
     @ddt.data(('/dev/sda', '/dev/sda', False, True, None),
               # This checks that we ignore the was_multipath parameter if it
               # doesn't make sense (because the used path is the one we are
               # asking about)
               ('/dev/sda', '/dev/sda', True, True, None),
               ('/dev/sda', '', True, False, None),
               # Check for encrypted volume
```

### Comparing `os-brick-6.2.1/os_brick/tests/initiator/test_utils.py` & `os-brick-6.2.2/os_brick/tests/initiator/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/local_dev/fake_lvm.py` & `os-brick-6.2.2/os_brick/tests/local_dev/fake_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/local_dev/test_brick_lvm.py` & `os-brick-6.2.2/os_brick/tests/local_dev/test_brick_lvm.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/privileged/test_nvmeof.py` & `os-brick-6.2.2/os_brick/tests/privileged/test_nvmeof.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/privileged/test_rbd.py` & `os-brick-6.2.2/os_brick/tests/privileged/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/privileged/test_rootwrap.py` & `os-brick-6.2.2/os_brick/tests/privileged/test_rootwrap.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/remotefs/test_remotefs.py` & `os-brick-6.2.2/os_brick/tests/remotefs/test_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/remotefs/test_windows_remotefs.py` & `os-brick-6.2.2/os_brick/tests/remotefs/test_windows_remotefs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/test_brick.py` & `os-brick-6.2.2/os_brick/tests/test_brick.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/test_exception.py` & `os-brick-6.2.2/os_brick/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/test_executor.py` & `os-brick-6.2.2/os_brick/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/test_utils.py` & `os-brick-6.2.2/os_brick/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/fake_win_conn.py` & `os-brick-6.2.2/os_brick/tests/windows/fake_win_conn.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_base.py` & `os-brick-6.2.2/os_brick/tests/windows/test_base.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_base_connector.py` & `os-brick-6.2.2/os_brick/tests/windows/test_base_connector.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_factory.py` & `os-brick-6.2.2/os_brick/tests/windows/test_factory.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_fibre_channel.py` & `os-brick-6.2.2/os_brick/tests/windows/test_fibre_channel.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_iscsi.py` & `os-brick-6.2.2/os_brick/tests/windows/test_iscsi.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_rbd.py` & `os-brick-6.2.2/os_brick/tests/windows/test_rbd.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/tests/windows/test_smbfs.py` & `os-brick-6.2.2/os_brick/tests/windows/test_smbfs.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/utils.py` & `os-brick-6.2.2/os_brick/utils.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick/version.py` & `os-brick-6.2.2/os_brick/version.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/os_brick.egg-info/PKG-INFO` & `os-brick-6.2.2/os_brick.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: os-brick
-Version: 6.2.1
+Version: 6.2.2
 Summary: OpenStack Cinder brick library for managing local volume attaches
 Home-page: https://docs.openstack.org/os-brick/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: OpenStack Cinder brick library for managing local volume attaches
 Platform: UNKNOWN
```

### Comparing `os-brick-6.2.1/os_brick.egg-info/SOURCES.txt` & `os-brick-6.2.2/os_brick.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -180,14 +180,15 @@
 releasenotes/notes/drop-py2-7dcde3ccd0e167b0.yaml
 releasenotes/notes/drop-python-3-6-and-3-7-1e7190189d415492.yaml
 releasenotes/notes/encryption-a642889a82ff9207.yaml
 releasenotes/notes/extend-encrypted-in-use-ac3f7a1994ec3a38.yaml
 releasenotes/notes/external-locks-9f015988ebdc37d6.yaml
 releasenotes/notes/fc-always-check-single-wwnn-1595689da0eb673b.yaml
 releasenotes/notes/fc-flush-single-path-22ed6cc7b56a6d9b.yaml
+releasenotes/notes/fc-force-disconnect-1a33cf46c233dd04.yaml
 releasenotes/notes/fix-fc-scan-too-broad-3c576e1846b7f05f.yaml
 releasenotes/notes/fix-generate-hostnqn-in-case-old-nvmecli.yaml
 releasenotes/notes/fix-multipath-disconnect-819d01e6e981883e.yaml
 releasenotes/notes/fix-nvme-issues-8dfc15cb691389fe.yaml
 releasenotes/notes/improve-get_sysfs_wwn-df38ea88cdcdcc94.yaml
 releasenotes/notes/improve-iscsi-multipath-detection-f36f28a993f61936.yaml
 releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml
```

### Comparing `os-brick-6.2.1/pylintrc` & `os-brick-6.2.2/pylintrc`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml` & `os-brick-6.2.2/releasenotes/notes/bug-1823200-scaleio-upgrade-3e83b5c9dd148714.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml` & `os-brick-6.2.2/releasenotes/notes/bug-1823200-victoria-b414a1806cba3998.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml` & `os-brick-6.2.2/releasenotes/notes/bug-1865754-ceph-octopus-compatibility-0aa9b8bc1b028301.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml` & `os-brick-6.2.2/releasenotes/notes/introduce-encryption-provider-constants-a7cd0ce58da2bae8.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/lock_path-c1c58a253391b41c.yaml` & `os-brick-6.2.2/releasenotes/notes/lock_path-c1c58a253391b41c.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml` & `os-brick-6.2.2/releasenotes/notes/nvmeof-consolidate-004dbe3a98f6f815.yaml`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/releasenotes/source/conf.py` & `os-brick-6.2.2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/requirements.txt` & `os-brick-6.2.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/setup.cfg` & `os-brick-6.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/setup.py` & `os-brick-6.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/test-requirements.txt` & `os-brick-6.2.2/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/tools/generate_connector_list.py` & `os-brick-6.2.2/tools/generate_connector_list.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/tools/lintstack.py` & `os-brick-6.2.2/tools/lintstack.py`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/tools/lintstack.sh` & `os-brick-6.2.2/tools/lintstack.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/tools/mypywrap.sh` & `os-brick-6.2.2/tools/mypywrap.sh`

 * *Files identical despite different names*

### Comparing `os-brick-6.2.1/tox.ini` & `os-brick-6.2.2/tox.ini`

 * *Files identical despite different names*

