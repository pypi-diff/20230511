# Comparing `tmp/mxops-1.0.0.tar.gz` & `tmp/mxops-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxops-1.0.0.tar", last modified: Thu Mar  9 07:56:53 2023, max compression
+gzip compressed data, was "mxops-1.1.0.tar", last modified: Thu May 11 16:43:03 2023, max compression
```

## Comparing `mxops-1.0.0.tar` & `mxops-1.1.0.tar`

### file list

```diff
@@ -1,53 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.099530 mxops-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-03-09 07:56:15.000000 mxops-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-09 07:56:53.099530 mxops-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-09 07:56:15.000000 mxops-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.095529 mxops-1.0.0/mxops/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.095529 mxops-1.0.0/mxops/config/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/config/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.095529 mxops-1.0.0/mxops/data/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4526 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/data/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10794 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/data/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/data/path.py
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     5955 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.099530 mxops-1.0.0/mxops/execution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/contract_interactions.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/msc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     3749 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/scene.py
--rw-r--r--   0 runner    (1001) docker     (123)     8530 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/execution/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.099530 mxops-1.0.0/mxops/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/resources/data_parser_help.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/resources/default_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/resources/parser_help.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.099530 mxops-1.0.0/mxops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-09 07:56:15.000000 mxops-1.0.0/mxops/utils/msc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.095529 mxops-1.0.0/mxops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-09 07:56:53.000000 mxops-1.0.0/mxops.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-03-09 07:56:15.000000 mxops-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-09 07:56:15.000000 mxops-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-03-09 07:56:53.099530 mxops-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 07:56:53.099530 mxops-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     8833 2023-03-09 07:56:15.000000 mxops-1.0.0/tests/test_check_transfers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-03-09 07:56:15.000000 mxops-1.0.0/tests/test_execution_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-03-09 07:56:15.000000 mxops-1.0.0/tests/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-03-09 07:56:15.000000 mxops-1.0.0/tests/test_raise_tx_errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.820605 mxops-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-11 16:42:27.000000 mxops-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-11 16:43:03.820605 mxops-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-11 16:42:27.000000 mxops-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.812605 mxops-1.1.0/mxops/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.816605 mxops-1.1.0/mxops/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/config/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5225 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.816605 mxops-1.1.0/mxops/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/data/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15893 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/data/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/data/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.816605 mxops-1.1.0/mxops/execution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11925 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/contract_interactions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/msc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9018 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/scene.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30282 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/token_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/token_management_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9267 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/execution/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.820605 mxops-1.1.0/mxops/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/resources/data_parser_help.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/resources/default_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/resources/parser_help.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.820605 mxops-1.1.0/mxops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-11 16:42:27.000000 mxops-1.1.0/mxops/utils/msc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.816605 mxops-1.1.0/mxops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 16:43:03.000000 mxops-1.1.0/mxops.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-11 16:42:27.000000 mxops-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-11 16:42:27.000000 mxops-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-11 16:43:03.820605 mxops-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 16:43:03.820605 mxops-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_core_builders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_data_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_execution_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_raise_tx_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_token_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-05-11 16:42:27.000000 mxops-1.1.0/tests/test_transfers_extraction.py
```

### Comparing `mxops-1.0.0/LICENSE` & `mxops-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/PKG-INFO` & `mxops-1.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mxops
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package to automate MultiversX smart contracts deployment and contract interactions in general
 Author: Etienne Wallet
 Project-URL: Homepage, https://github.com/Catenscia/MxOps
 Keywords: elrond,multiversx,smart-contract,devops,tests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MxOps
 
-MxOps is a python package created to automate MultiversX smart contracts deployments, calls and queries.
-Inspired from DevOps tools, it aims to ease and make reproducible any set of these interactions with smart-contracts.
+MxOps is a python package created to automate MultiversX transactions: be it smart contracts deployments, calls, queries or just simple transfers. Inspired from DevOps tools and built on top of [mxpy](https://github.com/multiversx/mx-sdk-py-cli), it aims to ease and make reproducible any set of these interactions with the blockchain.
 
 MxOps aims to be useful in these situations:
 
 - deployment automation
 - on-chain integration tests
 - contract interaction automation
 
@@ -30,8 +29,8 @@
 ## Contribution
 
 This tool is an humble proposal by [Catenscia](https://catenscia.com/) to have a standard way of writing deployment files, integration tests and others.
 If you want this tool to improve, please tell us your issues and proposals!
 
 And if you're motivated, we will always welcome hepling hands onboard :grin: !
 
-Read the [contribution guidelines](./CONTRIBUTING.md) for more :wink:
+Read the [contribution guidelines](https://github.com/Catenscia/MxOps/blob/main/CONTRIBUTING.md) for more :wink:
```

### Comparing `mxops-1.0.0/README.md` & `mxops-1.1.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # MxOps
 
-MxOps is a python package created to automate MultiversX smart contracts deployments, calls and queries.
-Inspired from DevOps tools, it aims to ease and make reproducible any set of these interactions with smart-contracts.
+MxOps is a python package created to automate MultiversX transactions: be it smart contracts deployments, calls, queries or just simple transfers. Inspired from DevOps tools and built on top of [mxpy](https://github.com/multiversx/mx-sdk-py-cli), it aims to ease and make reproducible any set of these interactions with the blockchain.
 
 MxOps aims to be useful in these situations:
 
 - deployment automation
 - on-chain integration tests
 - contract interaction automation
 
@@ -16,8 +15,8 @@
 ## Contribution
 
 This tool is an humble proposal by [Catenscia](https://catenscia.com/) to have a standard way of writing deployment files, integration tests and others.
 If you want this tool to improve, please tell us your issues and proposals!
 
 And if you're motivated, we will always welcome hepling hands onboard :grin: !
 
-Read the [contribution guidelines](./CONTRIBUTING.md) for more :wink:
+Read the [contribution guidelines](https://github.com/Catenscia/MxOps/blob/main/CONTRIBUTING.md) for more :wink:
```

### Comparing `mxops-1.0.0/mxops/__main__.py` & `mxops-1.1.0/mxops/__main__.py`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/config/cli.py` & `mxops-1.1.0/mxops/config/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 author: Etienne Wallet
 
 This module contains the cli for the config subpackage
 """
 from argparse import _SubParsersAction, Namespace, RawDescriptionHelpFormatter
 import json
 
-from mxops.enums import NetworkEnum
+from mxops.enums import parse_network_enum
 from mxops.config.config import Config, dump_default_config
 
 
 def add_subparser(subparsers_action: _SubParsersAction):
     """
     Add the steps subparser to a parser
 
@@ -20,15 +20,15 @@
     config_parser = subparsers_action.add_parser('config',
                                                  formatter_class=RawDescriptionHelpFormatter,
                                                  )
 
     config_parser.add_argument('-n',
                                '--network',
                                help='Name of the network to use',
-                               type=NetworkEnum)
+                               type=parse_network_enum)
 
     config_parser.add_argument('-o',
                                '--options',
                                action='store_true',
                                help=('list of options in the config for the '
                                      'specified network'))
```

### Comparing `mxops-1.0.0/mxops/config/config.py` & `mxops-1.1.0/mxops/config/config.py`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/data/cli.py` & `mxops-1.1.0/mxops/data/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from argparse import _SubParsersAction, ArgumentError, Namespace, RawDescriptionHelpFormatter
 from importlib import resources
 import json
 
 from mxops.data import path
 from mxops.config.config import Config
 from mxops.data.data import ScenarioData, delete_scenario_data
-from mxops.enums import NetworkEnum
+from mxops.enums import parse_network_enum
 
 
 def add_subparser(subparsers_action: _SubParsersAction):
     """
     Add the data subparser to a parser
 
     :param subparsers_action: subparsers interface for the parent parser
@@ -31,15 +31,15 @@
 
     # add get command
     get_parser = data_subparsers_actions.add_parser('get')
 
     get_parser.add_argument('-n',
                             '--network',
                             help='Name of the network to use',
-                            type=NetworkEnum,
+                            type=parse_network_enum,
                             required=True)
 
     get_parser.add_argument('-p',
                             '--path',
                             action='store_true',
                             help='Display the root path for the user data')
 
@@ -55,15 +55,15 @@
 
     # add delete command
     delete_parser = data_subparsers_actions.add_parser('delete')
 
     delete_parser.add_argument('-n',
                                '--network',
                                help='Name of the network to use',
-                               type=NetworkEnum,
+                               type=parse_network_enum,
                                required=True)
 
     delete_parser.add_argument('-s',
                                '--scenario',
                                help='Name of the scenario for the data deletion')
 
     delete_parser.add_argument('-a',
```

### Comparing `mxops-1.0.0/mxops/data/data.py` & `mxops-1.1.0/mxops/data/data.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,109 @@
 """
 author: Etienne Wallet
 
 This module contains the functions to load, write and update contracts data
 """
 from __future__ import annotations
-from dataclasses import dataclass
+from dataclasses import asdict, dataclass, field, is_dataclass
 import json
 import os
 from pathlib import Path
 import time
 from typing import Any, Dict, Optional
+
 from mxops.config.config import Config
 from mxops.data.path import get_scenario_file_path
-
-from mxops.enums import NetworkEnum
+from mxops import enums as mxops_enums
 from mxops import errors
 from mxops.utils.logger import get_logger
 
 
 LOGGER = get_logger('data')
 
 
 @dataclass
-class ContractData:
+class SavedValuesData:
     """
-    Dataclass representing the data that can be locally saved for a contract
+    Dataclass representing an object that can store values for the environment
     """
-    contract_id: str
-    address: str
     saved_values: Dict[str, Any]
 
     def set_value(self, value_key: str, value: Any):
         """
         Set the a value under a specified key
 
         :param value_key: key to save the value
         :type value_key: str
         :param value: value to save
         :type value: Any
         """
-        if value_key == 'address':
-            self.address = value
-        else:
-            self.saved_values[value_key] = value
+        self.saved_values[value_key] = value
+
+    def get_value(self, value_key: str) -> Any:
+        """
+        Fetch a value from the attribute of the class or from the saved value
+
+        :param value_key: key for the value
+        :type value_key: str
+        :return: value saved under the attribute or the the key provided
+        :rtype: Any
+        """
+        try:
+            return getattr(self, value_key)
+        except AttributeError:
+            pass
+        return self.get_saved_value(value_key)
 
     def get_saved_value(self, value_key: str) -> Any:
         """
-        Fetch a value saved under a key for this contract
+        Fetch a value saved under a key
 
         :param value_key: key for the value
         :type value_key: str
         :return: value saved under the key
         :rtype: Any
         """
         try:
             return self.saved_values[value_key]
         except KeyError as err:
             raise ValueError(
-                f'Unkown key: {value_key} for contract {self.contract_id}') from err
+                f'Unkown key: {value_key} for data object {self}') from err
+
+
+@dataclass
+class ContractData(SavedValuesData):
+    """
+    Dataclass representing the data that can be locally saved for a contract
+    """
+    contract_id: str
+    address: str
+
+    def set_value(self, value_key: str, value: Any):
+        """
+        Set the a value under a specified key
+
+        :param value_key: key to save the value
+        :type value_key: str
+        :param value: value to save
+        :type value: Any
+        """
+        if value_key == 'address':
+            self.address = value
+        else:
+            super().set_value(value_key, value)
 
     def to_dict(self) -> Dict:
         """
         Convert this instance to a dictionary
 
         :return: this instance as a dictionary
         :rtype: Dict
         """
-        self_dict = {**self.__dict__}
-        # avoid shallow copy (warning: not nested proof)
-        self_dict['saved_values'] = dict(self_dict['saved_values'])
+        self_dict = asdict(self)
         # add attribute to indicate internal/external
         self_dict['is_external'] = isinstance(self, ExternalContractData)
         return self_dict
 
 
 @dataclass
 class InternalContractData(ContractData):
@@ -90,65 +121,61 @@
     """
     Dataclass representing the data that can be locally saved for a contract
     not managed by MxOps
     """
 
 
 @dataclass
-class _ScenarioData:
+class TokenData(SavedValuesData):
     """
-    Dataclass representing the data that can be locally saved for a scenario
+    Dataclass representing a token issued on MultiversX
     """
     name: str
-    network: NetworkEnum
-    creation_time: int
-    last_update_time: int
-    contracts_data: Dict[str, ContractData]
+    ticker: str
+    identifier: str
+    type: mxops_enums.TokenTypeEnum
 
-    @staticmethod
-    def load_from_file(scenario_name: str) -> _ScenarioData:
+    def to_dict(self) -> Dict:
         """
-        Retrieve the locally saved scenario data and instantiate it
+        Transform this instance to a dictionnary
 
-        :param scenario_name: name of the scenario to load
-        :type scenario_name: str
-        :return: loaded scenario data
-        :rtype: _ScenarioData
+        :return: dictionary representing this instance
+        :rtype: Dict
         """
-        scenario_path = get_scenario_file_path(scenario_name)
-        with open(scenario_path.as_posix(), 'r', encoding='utf-8') as file:
-            return _ScenarioData(**json.load(file))
+        self_dict = asdict(self)
+        self_dict['type'] = self.type.value
+        return self_dict
 
-    def __post_init__(self):
-        """
-        After the initialisation of an instance, if the contracts data are found to be Dict,
-        will try to convert them to ContractData instances.
-        Will also try to convert string network to NetworkEnum.
-        Usefull for easy loading from json files
+    @classmethod
+    def from_dict(cls, data: Dict) -> TokenData:
         """
-        checked_data = {}
-        for contract_id, contract_data in self.contracts_data.items():
-            if isinstance(contract_data, Dict):
-                try:
-                    is_external = contract_data.pop('is_external')
-                except KeyError:
-                    is_external = False
-                if is_external:
-                    checked_data[contract_id] = ExternalContractData(**contract_data)
-                else:
-                    checked_data[contract_id] = InternalContractData(**contract_data)
-            elif isinstance(contract_data, ContractData):
-                checked_data[contract_id] = contract_data
-            else:
-                raise TypeError(('Unexpected contract data '
-                                 f'type {type(contract_data)}'))
-        self.contracts_data = checked_data
+        Create an instance of TokenData from a dictionary
 
-        if isinstance(self.network, str):
-            self.network = NetworkEnum(self.network)
+        :param data: dictionary to transform into TokenData
+        :type data: Dict
+        :return: instance from the input dictionary
+        :rtype: TokenData
+        """
+        formated_data = {
+            'type': mxops_enums.parse_token_type_enum(data['type'])
+        }
+        return cls(**{**data, **formated_data})
+
+
+@dataclass
+class _ScenarioData:
+    """
+    Dataclass representing the data that can be locally saved for a scenario
+    """
+    name: str
+    network: mxops_enums.NetworkEnum
+    creation_time: int
+    last_update_time: int
+    contracts_data: Dict[str, ContractData] = field(default_factory=dict)
+    tokens_data: Dict[str, TokenData] = field(default_factory=dict)
 
     def get_contract_value(self, contract_id: str, value_key: str) -> Any:
         """
         Return the value of a contract for a given key
 
         :param contract_id: unique id of the contract in the scenario
         :type contract_id: str
@@ -157,51 +184,113 @@
         :return: value saved under the given key
         :rtype: Any
         """
         try:
             contract = self.contracts_data[contract_id]
         except KeyError as err:
             raise errors.UnknownContract(self.name, contract_id) from err
-        try:
-            return getattr(contract, value_key)
-        except AttributeError:
-            pass
-        return contract.get_saved_value(value_key)
+        return contract.get_value(value_key)
 
     def set_contract_value(self, contract_id: str, value_key: str, value: Any):
         """
         Set the value of a contract for a given key
 
         :param contract_id: unique id of the contract in the scenario
         :type contract_id: str
-        :param value_key: key for the value to fetch
+        :param value_key: key for the value to set
         :type value_key: str
-        :return: value saved under the given key
-        :rtype: Any
         """
-        self.last_update_time = int(time.time())
+        self._set_update_time()
         try:
             contract = self.contracts_data[contract_id]
         except KeyError as err:
             raise errors.UnknownContract(self.name, contract_id) from err
         contract.set_value(value_key, value)
         self.save()
 
     def add_contract_data(self, contract_data: ContractData):
         """
         Add a contract data to the scenario
 
         :param contract_data: data to add to the scenario
         :type contract_data: ContractData
         """
-        self.last_update_time = int(time.time())
+        self._set_update_time()
         if contract_data.contract_id in self.contracts_data:
             raise errors.ContractIdAlreadyExists(contract_data.contract_id)
         self.contracts_data[contract_data.contract_id] = contract_data
 
+    def get_token_value(self, token_name: str, value_key: str) -> Any:
+        """
+        Return the value of a token for a given key
+
+        :param token_name: unique name of the token in the scenario
+        :type token_name: str
+        :param value_key: key for the value to fetch
+        :type value_key: str
+        :return: value saved under the given key
+        :rtype: Any
+        """
+        try:
+            token_data = self.tokens_data[token_name]
+        except KeyError as err:
+            raise errors.UnknownToken(self.name, token_name) from err
+        return token_data.get_value(value_key)
+
+    def set_token_value(self, token_name: str, value_key: str, value: Any):
+        """
+        Set the value of a contract for a given key
+
+        :param token_name: unique name of the token in the scenario
+        :type token_name: str
+        :param value_key: key for the value to set
+        :type value_key: str
+        """
+        self._set_update_time()
+        try:
+            token_data = self.tokens_data[token_name]
+        except KeyError as err:
+            raise errors.UnknownToken(self.name, token_name) from err
+        token_data.set_value(value_key, value)
+        self.save()
+
+    def add_token_data(self, token_data: TokenData):
+        """
+        Add a token data to the scenario
+
+        :param contract_data: data to add to the scenario
+        :type contract_data: ContractData
+        """
+        self._set_update_time()
+        if token_data.name in self.tokens_data:
+            raise errors.TokenNameAlreadyExists(token_data.name)
+        self.tokens_data[token_data.name] = token_data
+
+    def get_value(self, root_name: str, value_key: str) -> Any:
+        """
+        Search within tokens data and contracts data the value saved under the provided key
+
+        :param root_name: contract id or token name that hosts the value
+        :type root_name: str
+        :param value_key: key under which the value is savedd
+        :type value_key: str
+        :return: value saved
+        :rtype: Any
+        """
+        try:
+            return self.get_contract_value(root_name, value_key)
+        except errors.UnknownContract:
+            pass
+
+        try:
+            return self.get_token_value(root_name, value_key)
+        except errors.UnknownToken:
+            pass
+        raise errors.UnknownRootName(self.name, root_name)
+
     def save(self):
         """
         Save this scenario data where it belongs.
         Overwrite any existing file
         """
         scenario_path = get_scenario_file_path(self.name)
         with open(scenario_path.as_posix(), 'w', encoding='utf-8') as file:
@@ -211,20 +300,96 @@
         """
         Convert this instance to a dictionary
 
         :return: this instance as a dictionary
         :rtype: Dict
         """
         self_dict = {**self.__dict__}
-        self_dict['network'] = self.network.name
-        self_dict['contracts_data'] = {}
-        for contract_id, contract_data in self.contracts_data.items():
-            self_dict['contracts_data'][contract_id] = contract_data.to_dict()
+        for key, value in self_dict.items():
+            if isinstance(value, dict):
+                self_dict[key] = {}
+                for sub_key, sub_value in value.items():
+                    try:
+                        self_dict[key][sub_key] = sub_value.to_dict()
+                        continue
+                    except AttributeError:
+                        pass
+                    if is_dataclass(sub_value):
+                        self_dict[key][sub_key] = asdict(sub_value)
+                    else:
+                        self_dict[key][sub_key] = sub_value
+        self_dict['network'] = self.network.value
         return self_dict
 
+    def _set_update_time(self):
+        """
+        Set the last update time to now
+        """
+        self.last_update_time = int(time.time())
+
+    @classmethod
+    def load_from_name(cls, scenario_name: str) -> _ScenarioData:
+        """
+        Retrieve the locally saved scenario data and instantiate it
+
+        :param scenario_name: name of the scenario to load
+        :type scenario_name: str
+        :return: loaded scenario data
+        :rtype: _ScenarioData
+        """
+        scenario_path = get_scenario_file_path(scenario_name)
+        return cls.load_from_path(scenario_path)
+
+    @classmethod
+    def load_from_path(cls, scenario_path: Path) -> _ScenarioData:
+        """
+        Retrieve the locally saved scenario data and instantiate it
+
+        :param scenario_path: path to the scenario to load
+        :type scenario_path: Path
+        :return: loaded scenario data
+        :rtype: _ScenarioData
+        """
+        with open(scenario_path.as_posix(), 'r', encoding='utf-8') as file:
+            raw_content = json.load(file)
+        return cls.from_dict(raw_content)
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> _ScenarioData:
+        """
+        Create an instance of _ScenarioData from a dict
+
+        :param data: data with the needed attributes and values
+        :type data: Dict[str, Any]
+        :return: _ScenarioData instance corresponding to the provided data
+        :rtype: ScenarioData
+        """
+        contracts_data = {}
+        for contract_id, contract_data in data['contracts_data'].items():
+            if isinstance(contract_data, Dict):
+                try:
+                    is_external = contract_data.pop('is_external')
+                except KeyError:
+                    is_external = False
+                if is_external:
+                    contracts_data[contract_id] = ExternalContractData(**contract_data)
+                else:
+                    contracts_data[contract_id] = InternalContractData(**contract_data)
+
+        tokens_data = data.get('tokens_data', {})
+        tokens_data = {k: TokenData.from_dict(v) for k, v in tokens_data.items()}
+
+        formated_data = {
+            'contracts_data': contracts_data,
+            'tokens_data': tokens_data,
+            'network': mxops_enums.parse_network_enum(data['network'])
+        }
+
+        return cls(**{**data, **formated_data})
+
 
 class ScenarioData:  # pylint: disable=too-few-public-methods
     """
     Shell class that implement the singleton logic for the _ScenarioData
     class.
     Only one scenario should be loaded by execution.
     """
@@ -250,21 +415,21 @@
 
         :param scenario_name: name of the scenario to load
         :type scenario_name: str
         """
         if cls._instance is not None:
             raise errors.UnloadedScenario
         try:
-            cls._instance = _ScenarioData.load_from_file(scenario_name)
+            cls._instance = _ScenarioData.load_from_name(scenario_name)
         except FileNotFoundError as err:
             raise errors.UnknownScenario(scenario_name) from err
         config = Config.get_config()
         network = config.get_network()
         LOGGER.info((f'Scenario {scenario_name} loaded for '
-                     f'network {network.name}'))
+                     f'network {network.value}'))
 
     @classmethod
     def create_scenario(cls, scenario_name: str):
         """
         Create a scenario data while checking for a pre existing instance.
 
         :param scenario_name: name of the scenario to create
@@ -281,15 +446,15 @@
         current_timestamp = int(time.time())
         cls._instance = _ScenarioData(scenario_name,
                                       network,
                                       current_timestamp,
                                       current_timestamp,
                                       {})
         LOGGER.info((f'Scenario {scenario_name} created for '
-                     f'network {network.name}'))
+                     f'network {network.value}'))
 
 
 def check_scenario_file(scenario_name: str) -> bool:
     """
     Check if a file exists for a given scenario name
 
     :param scenario_name: name of the scenario to check
@@ -316,10 +481,11 @@
         message = (f'Confirm the deletion of the scenario {scenario_name} '
                    f'located at {scenario_path.as_posix()}. (y/n)')
         if input(message).lower() not in ('y', 'yes'):
             print('User aborted deletion')
             return
     try:
         os.remove(scenario_path.as_posix())
+        LOGGER.info(f'The data of the scenario {scenario_name} has been deleted')
     except FileNotFoundError:
         LOGGER.warning((f'The scenario {scenario_name} does'
                         ' not have any data recorded'))
```

### Comparing `mxops-1.0.0/mxops/data/path.py` & `mxops-1.1.0/mxops/data/path.py`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/errors.py` & `mxops-1.1.0/mxops/errors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 author: Etienne Wallet
 
 Errors used in the MxOps package
 """
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, List
+from typing import Any, Dict, List
 
 from multiversx_sdk_network_providers.transactions import TransactionOnNetwork
 
 from mxops.utils.msc import get_tx_link
 
 
 #############################################################
@@ -25,17 +25,24 @@
     """
 
     def __init__(self, raw_object: Any, parsing_target: str, ) -> None:
         message = f"Could not parse {raw_object} as {parsing_target}"
         super().__init__(message)
 
 
+class NewTokenIdentifierNotFound(Exception):
+    """
+    To be raised when the token identifier of newly issued token was not found in the results
+    of the transaction
+    """
+
+
 #############################################################
 #
-#                   Data Managment Errors
+#                   Data Management Errors
 #
 #############################################################
 
 
 class UnknownScenario(Exception):
     """
     To be raised when a specified scenario is not found
@@ -83,14 +90,46 @@
     """
 
     def __init__(self, contract_id: str) -> None:
         message = f'Contract id {contract_id} already exists'
         super().__init__(message)
 
 
+class UnknownToken(Exception):
+    """
+    To be raised when a specified token is not found is a scenario
+    """
+
+    def __init__(self, scenario_name: str, token_name: str) -> None:
+        message = (f'Token named {token_name} is unkown in '
+                   f'scenario {scenario_name}')
+        super().__init__(message)
+
+
+class TokenNameAlreadyExists(Exception):
+    """
+    To be raised when there is a conflict with token name
+    """
+
+    def __init__(self, token_name: str) -> None:
+        message = f'Token named {token_name} already exists'
+        super().__init__(message)
+
+
+class UnknownRootName(Exception):
+    """
+    To be raised when a specified root name is not found is a scenario
+    """
+
+    def __init__(self, scenario_name: str, root_name: str) -> None:
+        message = (f'Root named {root_name} is unkown in '
+                   f'scenario {scenario_name}')
+        super().__init__(message)
+
+
 class ScenarioNameAlreadyExists(Exception):
     """
     To be raised when there is a conflict with scenario name
     """
 
     def __init__(self, scenario_name: str) -> None:
         message = f'Scenario name {scenario_name} already exists'
@@ -210,14 +249,47 @@
 #############################################################
 
 class CheckFailed(Exception):
     """
     To be raised when an on-chain transaction check fails
     """
 
-    def __init__(self, check: dataclass, tx: TransactionOnNetwork, *args: object) -> None:
+    def __init__(self, check: dataclass, tx: TransactionOnNetwork) -> None:
         self.check = check
         self.tx = tx
-        super().__init__(*args)()
+        super().__init__()
 
     def __str__(self) -> str:
         return f'Check failed on transaction {get_tx_link(self.tx.hash)}\nCheck: {self.check}'
+
+
+#############################################################
+#
+#                   User Errors
+#
+#############################################################
+
+class UnkownStep(Exception):
+    """
+    to be raised when the user provide a step name that is unkown
+    """
+
+    def __init__(self, step_name: str) -> None:
+        self.step_name = step_name
+        super().__init__()
+
+    def __str__(self) -> str:
+        return f'Unkown Step name: {self.step_name}'
+
+
+class InvalidStepDefinition(Exception):
+    """
+    to be raised when the arguments provided by the user for a Step are not valid
+    """
+
+    def __init__(self, step_name: str, parameters: Dict) -> None:
+        self.step_name = step_name
+        self.parameters = parameters
+        super().__init__()
+
+    def __str__(self) -> str:
+        return f'Step {self.step_name} received invalid parameters {self.parameters}'
```

### Comparing `mxops-1.0.0/mxops/execution/account.py` & `mxops-1.1.0/mxops/execution/account.py`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/execution/cli.py` & `mxops-1.1.0/mxops/execution/cli.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 This module contains the cli for the execution subpackage
 """
 from argparse import _SubParsersAction, Namespace
 import os
 from pathlib import Path
 from mxops.config.config import Config
 from mxops.data import path
-from mxops.data.data import ScenarioData
+from mxops.data.data import ScenarioData, delete_scenario_data
 
-from mxops.enums import NetworkEnum
+from mxops.enums import parse_network_enum
 from mxops.execution.scene import execute_directory, execute_scene
 from mxops import errors
 
 
 def add_subparser(subparsers_action: _SubParsersAction):
     """
     Add the data subparser to a parser
@@ -27,18 +27,28 @@
                                  '--scenario',
                                  type=str,
                                  required=True,
                                  help=('Name of the scenario in which the '
                                        'scene(s) will be executed'))
     scenario_parser.add_argument('-n',
                                  '--network',
-                                 type=NetworkEnum,
+                                 type=parse_network_enum,
                                  required=True,
                                  help=('Name of the network in which the '
                                        'scene(s) will be executed'))
+    scenario_parser.add_argument('-d',
+                                 '--delete',
+                                 action='store_true',
+                                 required=False,
+                                 help='delete the scenario data after the execution')
+    scenario_parser.add_argument('-c',
+                                 '--clean',
+                                 action='store_true',
+                                 required=False,
+                                 help='clean the scenario data before the execution')
     scenario_parser.add_argument('elements',
                                  nargs='+',
                                  type=str,
                                  help='Path to scene file and/or scene directory')
 
 
 def execute_cli(args: Namespace):
@@ -49,21 +59,28 @@
     :type args: Namespace
     """
     if args.command != 'execute':
         raise ValueError(f'Command execute was expected, found {args.command}')
 
     path.initialize_data_folder()
     Config.set_network(args.network)
+
+    if args.clean:
+        delete_scenario_data(args.scenario, False)
+
     try:
         ScenarioData.load_scenario(args.scenario)
     except errors.UnknownScenario:
         ScenarioData.create_scenario(args.scenario)
         ScenarioData.get().save()
 
     for element in args.elements:
-        element_path = Path('./' + element)
+        element_path = Path(element)
         if os.path.isfile(element_path):
             execute_scene(element_path)
         elif os.path.isdir(element_path):
             execute_directory(element_path)
         else:
             raise ValueError(f'{element_path} is not a file nor a directory')
+
+    if args.delete:
+        delete_scenario_data(args.scenario, False)
```

### Comparing `mxops-1.0.0/mxops/execution/contract_interactions.py` & `mxops-1.1.0/mxops/execution/contract_interactions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 """
-Module with deploy functions for the contracts
+Module with deploy, call and queries functions for the contracts
 """
 from pathlib import Path
 from typing import List, Tuple
 
 from multiversx_sdk_cli import config as mxpy_config
 from multiversx_sdk_cli.accounts import Account
 from multiversx_sdk_cli.contracts import CodeMetadata, SmartContract, QueryResult
-from multiversx_sdk_cli.transactions import Transaction
+from multiversx_sdk_cli.transactions import Transaction as CliTransaction
 from multiversx_sdk_cli import utils as mxpy_utils
 from multiversx_sdk_network_providers import ProxyNetworkProvider
 
 from mxops.config.config import Config
 from mxops.execution.msc import EsdtTransfer
 from mxops.execution import utils
 
 
 def get_contract_deploy_tx(
     wasm_file: Path,
     metadata: CodeMetadata,
     gas_limit: int,
     contract_args: List,
     sender: Account
-) -> Tuple[Transaction, SmartContract]:
+) -> Tuple[CliTransaction, SmartContract]:
     """
     Contruct the contract instance and the transaction used to deploy a contract.
     The transaction is not relayed to the proxy,
     this has to be done with the result of this function.
 
     :param wasm_file: path to the wasm file of the contract
     :type wasm_file: Path
@@ -35,15 +35,15 @@
     :param gas_limit: gas limit for the transaction
     :type gas_limit: int
     :param contract_args: list of arguments to pass to the deploy method
     :type contract_args: List
     :param sender: account to use for this transaction
     :type sender: Account
     :return: deploy transaction and contract instance created
-    :rtype: Tuple[Transaction, SmartContract]
+    :rtype: Tuple[CliTransaction, SmartContract]
     """
     config = Config.get_config()
 
     bytecode = mxpy_utils.read_binary_file(wasm_file).hex()
     contract = SmartContract(bytecode=bytecode, metadata=metadata)
     formated_args = utils.format_tx_arguments(contract_args)
 
@@ -56,15 +56,15 @@
 def get_contract_value_call_tx(
     contract_str: str,
     endpoint: str,
     gas_limit: int,
     arguments: List,
     value: int,
     sender: Account
-) -> Transaction:
+) -> CliTransaction:
     """
     Contruct the transaction for a contract call with value provision.
     The transaction is not relayed to the proxy, this has to be done with
     the result of this function.
 
     :param contract_str: designation of the contract to call (bech32 or mxops value)
     :type contract_str: str
@@ -75,15 +75,15 @@
     :param arguments: argument for endpoint
     :type arguments: List
     :param value: value to send during the call
     :type value: int
     :param sender: sender of the transaction
     :type sender: Account
     :return: call transaction to send
-    :rtype: Transaction
+    :rtype: CliTransaction
     """
     config = Config.get_config()
 
     contract = utils.get_contract_instance(contract_str)
 
     formated_args = utils.format_tx_arguments(arguments)
     if isinstance(value, str):
@@ -106,15 +106,15 @@
 def get_contract_single_esdt_call_tx(
     contract_str: str,
     endpoint: str,
     gas_limit: int,
     arguments: List,
     esdt_transfer: EsdtTransfer,
     sender: Account
-) -> Transaction:
+) -> CliTransaction:
     """
     Contruct the transaction for a contract call with an esdt transfer.
     The transaction is not relayed to the proxy, this has to be done with
     the result of this function.
 
     :param contract_str: designation of the contract to call (bech32 or mxops value)
     :type contract_str: str
@@ -125,15 +125,15 @@
     :param arguments: argument for endpoint
     :type arguments: List
     :param esdt_transfer: transfer to be made with the endpoint call
     :type esdt_transfer: EsdtTransfer
     :param sender: sender of the transaction
     :type sender: Account
     :return: call transaction to send
-    :rtype: Transaction
+    :rtype: CliTransaction
     """
     config = Config.get_config()
 
     contract = utils.get_contract_instance(contract_str)
 
     tx_arguments = [
         esdt_transfer.token_identifier,
@@ -160,15 +160,15 @@
 def get_contract_single_nft_call_tx(
     contract_str: str,
     endpoint: str,
     gas_limit: int,
     arguments: List,
     nft_transfer: EsdtTransfer,
     sender: Account
-) -> Transaction:
+) -> CliTransaction:
     """
     Contruct the transaction for a contract call with an nft transfer (NFT, SFT and Meta ESDT).
     The transaction is not relayed to the proxy, this has to be done with
     the result of this function.
 
     :param contract_str: designation of the contract to call (bech32 or mxops value)
     :type contract_str: str
@@ -179,15 +179,15 @@
     :param arguments: argument for endpoint
     :type arguments: List
     :param nft_transfer: transfer to be made with the endpoint call
     :type nft_transfer: EsdtTransfer
     :param sender: sender of the transaction
     :type sender: Account
     :return: call transaction to send
-    :rtype: Transaction
+    :rtype: CliTransaction
     """
     config = Config.get_config()
     self_contract = SmartContract(sender.address)
 
     contract = utils.get_contract_instance(contract_str)
 
     tx_arguments = [
@@ -217,15 +217,15 @@
 def get_contract_multiple_esdt_call_tx(
     contract_str: str,
     endpoint: str,
     gas_limit: int,
     arguments: List,
     esdt_transfers: List[EsdtTransfer],
     sender: Account
-) -> Transaction:
+) -> CliTransaction:
     """
     Contruct the transaction for a contract call with multiple esdt transfers.
     The transaction is not relayed to the proxy, this has to be done with
     the result of this function.
 
     :param contract_str: designation of the contract to call (bech32 or mxops value)
     :type contract_str: str
@@ -236,15 +236,15 @@
     :param arguments: argument for endpoint
     :type arguments: List
     :param esdt_transfers: transfers to be made with the endpoint call
     :type esdt_transfers: List[EsdtTransfer]
     :param sender: sender of the transaction
     :type sender: Account
     :return: call transaction to send
-    :rtype: Transaction
+    :rtype: CliTransaction
     """
     config = Config.get_config()
 
     self_contract = SmartContract(sender.address)
     contract = utils.get_contract_instance(contract_str)
 
     tx_arguments = [
@@ -279,15 +279,15 @@
     contract_str: str,
     endpoint: str,
     gas_limit: int,
     arguments: List,
     value: int,
     esdt_transfers: List[EsdtTransfer],
     sender: Account
-) -> Transaction:
+) -> CliTransaction:
     """
     Contruct the transaction for a contract call
     The transaction is not relayed to the proxy, this has to be done with
     the result of this function.
 
     :param contract_str: designation of the contract to call (bech32 or mxops value)
     :type contract_str: str
@@ -300,15 +300,15 @@
     :param value: value to send during the call
     :type value: int
     :param esdt_transfers: transfers to be made with the endpoint call
     :type esdt_transfers: List[EsdtTransfer]
     :param sender: sender of the transaction
     :type sender: Account
     :return: call transaction to send
-    :rtype: Transaction
+    :rtype: CliTransaction
     """
     n_transfers = len(esdt_transfers)
 
     if n_transfers == 0:
         tx = get_contract_value_call_tx(contract_str,
                                         endpoint,
                                         gas_limit,
```

### Comparing `mxops-1.0.0/mxops/execution/network.py` & `mxops-1.1.0/mxops/execution/network.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,67 @@
 """
 author: Etienne Wallet
 
 This module contains the functions to pass transactions to the proxy and to monitor them
 """
-from typing import List
+import time
+from typing import List, Union
 
-from multiversx_sdk_cli.transactions import Transaction
-from multiversx_sdk_cli.accounts import Address
+from multiversx_sdk_cli.transactions import Transaction as CliTransaction
+from multiversx_sdk_cli.accounts import Address as CliAddress
+from multiversx_sdk_core import Transaction
 from multiversx_sdk_network_providers import ProxyNetworkProvider
 from multiversx_sdk_network_providers.transactions import TransactionOnNetwork
 
 from mxops.config.config import Config
 from mxops import errors
 from mxops.execution.msc import OnChainTransfer
 
 
-def send(tx: Transaction) -> str:
+def send(tx: Union[CliTransaction, Transaction]) -> str:
     """
     Send a transaction through the proxy without waiting for a return
 
     :param tx: transaction to send
-    :type tx: Transaction
+    :type tx: Union[CliTransaction, Transaction]
     :return: hash of the transaction
     :rtype: str
     """
     config = Config.get_config()
     proxy = ProxyNetworkProvider(config.get('PROXY'))
-    return tx.send(proxy)
+    return proxy.send_transaction(tx)
 
 
-def send_and_wait_for_result(tx: Transaction) -> Transaction:
+def send_and_wait_for_result(tx: Union[CliTransaction, Transaction]) -> TransactionOnNetwork:
     """
     Transmit a transaction to a proxy constructed with the config.
     Wait for the result of the transaction and return the on-chainfinalised transaction.
 
     :param tx: transaction to send
-    :type tx: Transaction
+    :type tx: Union[CliTransaction, Transaction]
     :return: on chain finalised transaction
-    :rtype: Transaction
+    :rtype: TransactionOnNetwork
     """
     config = Config.get_config()
     proxy = ProxyNetworkProvider(config.get('PROXY'))
+
     timeout = int(config.get('TX_TIMEOUT'))
-    return tx.send_wait_result(proxy, timeout)
+    refresh_period = int(config.get('TX_REFRESH_PERIOD'))
+
+    tx_hash = proxy.send_transaction(tx)
+    num_periods_to_wait = int(timeout / refresh_period)
+
+    for _ in range(0, num_periods_to_wait):
+        time.sleep(refresh_period)
+
+        on_chain_tx = proxy.get_transaction(tx_hash)
+        if on_chain_tx.is_completed:
+            return on_chain_tx
+
+    raise errors.UnfinalizedTransactionException(on_chain_tx)
 
 
 def raise_on_errors(on_chain_tx: TransactionOnNetwork):
     """
     Raise an error if the transaction contains any of the following:
 
     - failed tx
@@ -86,21 +101,21 @@
     :return: Transfer found in the data
     :rtype: OnChainTransfer
     """
     if not data.startswith('ESDTTransfer@'):
         raise ValueError(f'Data does not describe a simple ESDT transfer: {data}')
 
     try:
-        _, token, amount, *_ = data.split('@')
-        token = bytearray.fromhex(token).decode()
+        _, token_identifier, amount, *_ = data.split('@')
+        token_identifier = bytearray.fromhex(token_identifier).decode()
         amount = str(int(amount, 16))
     except Exception as err:
         raise errors.ParsingError(data, 'ESDTTransfer') from err
 
-    return OnChainTransfer(sender, receiver, token, amount)
+    return OnChainTransfer(sender, receiver, token_identifier, amount)
 
 
 def extract_nft_transfer(sender: str, receiver: str, data: str) -> OnChainTransfer:
     """
     Extract a nft transfer from a smart contract result data.
 
     :param sender: address of the sender of the data in bech32
@@ -112,21 +127,21 @@
     :return: Transfer found in the data
     :rtype: OnChainTransfer
     """
     if not data.startswith('ESDTNFTTransfer@'):
         raise ValueError(f'Data does not describe a nft transfer: {data}')
 
     try:
-        _, token, nonce, amount, *_ = data.split('@')
-        token = bytearray.fromhex(token).decode() + '-' + nonce
+        _, token_identifier, nonce, amount, *_ = data.split('@')
+        token_identifier = bytearray.fromhex(token_identifier).decode() + '-' + nonce
         amount = str(int(amount, 16))
     except Exception as err:
         raise errors.ParsingError(data, 'ESDTNFTTransfer') from err
 
-    return OnChainTransfer(sender, receiver, token, amount)
+    return OnChainTransfer(sender, receiver, token_identifier, amount)
 
 
 def extract_multi_transfer(sender: str, data: str) -> List[OnChainTransfer]:
     """
     Extract a multi transfer from smart contract result data
 
     :param sender: address of the sender of the data in bech32
@@ -138,29 +153,29 @@
     """
     if not data.startswith('MultiESDTNFTTransfer@'):
         raise ValueError(f'Data does not describe a multi transfer: {data}')
 
     try:
         _, receiver, n_transfers, *details = data.split('@')
         n_transfers = int(n_transfers, base=16)
-        receiver = Address(receiver).bech32()
+        receiver = CliAddress(receiver).bech32()
     except Exception as err:
         raise errors.ParsingError(data, 'MultiESDTNFTTransfer') from err
 
     transfers = []
     for i in range(n_transfers):
         try:
-            token, nonce, amount = details[3*i:3*(i+1)]
-            token = bytearray.fromhex(token).decode()
+            token_identifier, nonce, amount = details[3*i:3*(i+1)]
+            token_identifier = bytearray.fromhex(token_identifier).decode()
             amount = str(int(amount, 16))
         except Exception as err:
             raise errors.ParsingError(data, 'MultiESDTNFTTransfer') from err
         if nonce != '':
-            token += f'-{nonce}'
-        transfers.append(OnChainTransfer(sender, receiver, token, amount))
+            token_identifier += f'-{nonce}'
+        transfers.append(OnChainTransfer(sender, receiver, token_identifier, amount))
 
     return transfers
 
 
 def get_transfers_from_data(sender: str, receiver: str, data: str) -> List[OnChainTransfer]:
     """
     Try to extract token transfers from the data of a transaction or asmart contract result.
@@ -189,21 +204,26 @@
         return extract_multi_transfer(sender, data)
     except ValueError:
         pass
 
     return []
 
 
-def get_on_chain_transfers(on_chain_tx: TransactionOnNetwork) -> List[OnChainTransfer]:
+def get_on_chain_transfers(
+        on_chain_tx: TransactionOnNetwork,
+        include_refund: bool = False
+) -> List[OnChainTransfer]:
     """
     Extract from an on-chain transaction the tokens transfers that were operated in this
     transaction.
 
     :param on_chain_tx: on-chain transaction to inspect
     :type on_chain_tx: TransactionOnNetwork
+    :param include_refund: if gas refund should be included in the transfers returned
+    :type include_refund: bool, default to False
     :return: list of executed transfer
     :rtype: List[OnChainTransfer]
     """
     transfers = []
     sender = on_chain_tx.sender.bech32()
     receiver = on_chain_tx.receiver.bech32()
     amount = str(on_chain_tx.value)
@@ -224,15 +244,15 @@
             transfers.extend(extract_multi_transfer(sender, on_chain_tx.data))
         except errors.ParsingError:
             pass
 
     for result in on_chain_tx.contract_results.items:
         sender, receiver = result.sender.bech32(), result.receiver.bech32()
         amount = str(result.value)
-        if amount != "0" and not result.is_refund:
+        if amount != "0" and (include_refund or not result.is_refund):
             transfers.append(OnChainTransfer(
                 sender,
                 receiver,
                 'EGLD',
                 amount
             ))
         else:
```

### Comparing `mxops-1.0.0/mxops/execution/scene.py` & `mxops-1.1.0/mxops/execution/scene.py`

 * *Files 13% similar despite different names*

```diff
@@ -70,18 +70,18 @@
     scene = load_scene(scene_path)
     scenario_data = ScenarioData.get()
 
     config = Config.get_config()
     network = config.get_network()
 
     # check network authorization
-    if network.name not in scene.allowed_networks:
+    if network.name not in scene.allowed_networks and network.value not in scene.allowed_networks:
         raise errors.ForbiddenSceneNetwork(
             scene_path,
-            network.name,
+            network.value,
             scene.allowed_networks
         )
 
     # check scenario authorizations
     match_found = False
     for scenario_pattern in scene.allowed_scenario:
         if re.match(scenario_pattern, scenario_data.name) is not None:
@@ -102,15 +102,20 @@
     # load external contracts addresses
     for contract_id, address in scene.external_contracts.items():
         try:
             # try to update the contract address while keeping data intact
             scenario_data.set_contract_value(contract_id, 'address', address)
         except errors.UnknownContract:
             # otherwise create the contract data
-            scenario_data.add_contract_data(ExternalContractData(contract_id, address, {}))
+            scenario_data.add_contract_data(ExternalContractData(
+                contract_id=contract_id,
+                address=address,
+                saved_values={}
+            )
+            )
 
     # execute steps
     for step in scene.steps:
         step.execute()
         scenario_data.save()
```

### Comparing `mxops-1.0.0/mxops/execution/utils.py` & `mxops-1.1.0/mxops/execution/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 author: Etienne Wallet
 
 This module contains some utilities functions for the execution sub package
 """
 import os
 from typing import Any, List, Optional, Tuple
 
-from multiversx_sdk_cli.accounts import Address
+from multiversx_sdk_cli.accounts import Address as CliAddress
 from multiversx_sdk_cli.contracts import QueryResult, SmartContract
 from multiversx_sdk_cli.errors import BadAddressFormatError
+from multiversx_sdk_core.address import Address
+from multiversx_sdk_core.errors import ErrBadAddress
 
 from mxops.config.config import Config
 from mxops.data.data import ScenarioData
 from mxops import errors
 from mxops.execution.account import AccountsManager
 
 
@@ -85,72 +87,99 @@
     retrieved_value = config.get(inner_arg[1:].upper())
     return convert_arg(retrieved_value, desired_type)
 
 
 def retrieve_value_from_scenario_data(arg: str) -> str:
     """
     Retrieve the value of an argument from scenario data.
-    the argument must formated like this: %<contract_id>%<attribute>
+    the argument must formated like this: %<root_name>%<attribute>
 
     :param arg: name of the variable formated as above
     :type arg: str
     :return: value saved in the config
     :rtype: str
     """
     inner_arg, desired_type = retrieve_specified_type(arg)
     try:
-        contract_id, value_key = inner_arg[1:].split('%')
+        root_name, value_key = inner_arg[1:].split('%')
     except Exception as err:
         raise errors.WrongScenarioDataReference from err
 
     scenario_data = ScenarioData.get()
-    retrieved_value = scenario_data.get_contract_value(contract_id, value_key)
+    retrieved_value = scenario_data.get_value(root_name, value_key)
     return convert_arg(retrieved_value, desired_type)
 
 
-def retrieve_address_from_account(arg: str) -> str:
+def retrieve_address_from_account(arg: str) -> CliAddress:
     """
     Retrieve an address from the accounts manager.
     the argument must formated like this: [user]
 
     :param arg: name of the variable formated as above
     :type arg: str
     :return: address from the scenario
-    :rtype: str
+    :rtype: CliAddress
     """
     try:
         arg = arg[1:-1]
     except Exception as err:
         raise errors.WrongScenarioDataReference from err
 
     account = AccountsManager.get_account(arg)
-    return account.address.bech32()
+    return account.address
 
 
 def retrieve_value_from_string(arg: str) -> Any:
     """
     Check if a string argument is intended to be an env var, a config var or a data var.
     If Nonce of the previous apply, return the string unchanged
 
     :param arg: argument to check
     :type arg: str
     :return: untouched argument or retrieved value
     :rtype: Any
     """
     if arg.startswith('['):
-        return retrieve_address_from_account(arg)
+        return retrieve_address_from_account(arg).bech32()
     if arg.startswith('$'):
         return retrieve_value_from_env(arg)
     if arg.startswith('&'):
         return retrieve_value_from_config(arg)
     if arg.startswith('%'):
         return retrieve_value_from_scenario_data(arg)
     return arg
 
 
+def retrieve_values_from_strings(args: List[str]) -> List[Any]:
+    """
+    Dynamically evaluate the value of each element of the provided list
+
+    :param args: args to evaluate
+    :type args: List[str]
+    :return: evaluated arguments
+    :rtype: List[Any]
+    """
+    return [retrieve_value_from_string(arg) for arg in args]
+
+
+def retrieve_value_from_any(arg: Any) -> Any:
+    """
+    Dynamically evaluate the provided argument depending on its type.
+    Otherwise it will be returned itself
+
+    :param arg: argument to evaluate
+    :type arg: Any
+    :return: evaluated argument
+    :rtype: Any
+    """
+    if isinstance(arg, str):
+        return retrieve_value_from_string(arg)
+    return arg
+
+
 def format_tx_arguments(arguments: List[Any]) -> List[Any]:
     """
     Transform the arguments so they can be recognised by mxpy
 
     :param arguments: list of arguments to be supplied to a endpoint
     :type arguments: List[Any]
     :return: formatted arguments
@@ -159,18 +188,18 @@
     formated_arguments = []
     for arg in arguments:
         if isinstance(arg, str):  # done a first time as int arg can be entered as string
             arg = retrieve_value_from_string(arg)
         formated_arg = arg
         if isinstance(arg, str):
             if arg.startswith('erd') and len(arg) == 62:
-                formated_arg = '0x' + Address(arg).hex()
+                formated_arg = '0x' + CliAddress(arg).hex()
             elif not arg.startswith('0x'):
                 formated_arg = 'str:' + arg
-        elif isinstance(arg, Address):
+        elif isinstance(arg, CliAddress):
             formated_arg = '0x' + arg.hex()
 
         formated_arguments.append(formated_arg)
     return formated_arguments
 
 
 def get_contract_instance(contract_str: str) -> SmartContract:
@@ -182,32 +211,69 @@
     :param contract_str: contract address or mxops value
     :type contract_str: str
     :return: smart contract corresponding to the address
     :rtype: SmartContract
     """
     # try to see if the string is a valid address
     try:
-        return SmartContract(Address(contract_str))
+        return SmartContract(CliAddress(contract_str))
     except BadAddressFormatError:
         pass
     # otherwise try to parse it as a mxops value
     contract_address = retrieve_value_from_string(contract_str)
     try:
-        return SmartContract(Address(contract_address))
+        return SmartContract(CliAddress(contract_address))
     except BadAddressFormatError:
         pass
     # lastly try to see if it is a valid contract id
     contract_address = retrieve_value_from_string(f'%{contract_str}%address')
     try:
-        return SmartContract(Address(contract_address))
+        return SmartContract(CliAddress(contract_address))
     except BadAddressFormatError:
         pass
     raise errors.ParsingError(contract_str, 'contract address')
 
 
+def get_address_instance(address_str: str) -> Address:
+    """
+    From a string return an Address instance.
+    The input will be parsed to dynamically evaluate values from the environment, the config, saved
+    data or from the defined contracts or accounts.
+
+    :param address_str: raw address or address entity designation
+    :type address_str: str
+    :return: address instance corresponding to the input
+    :rtype: Address
+    """
+    # try to see if the string is a valid address
+    try:
+        return Address.from_bech32(address_str)
+    except ErrBadAddress:
+        pass
+    # otherwise try to parse it as a mxops value
+    evaluated_address_str = retrieve_value_from_string(address_str)
+    try:
+        return Address.from_bech32(evaluated_address_str)
+    except ErrBadAddress:
+        pass
+    # else try to see if it is a valid contract id
+    try:
+        evaluated_address_str = retrieve_value_from_string(f'%{address_str}%address')
+        return Address.from_bech32(evaluated_address_str)
+    except (ErrBadAddress, errors.UnknownRootName):
+        pass
+    # finally try to see if it designate a defined account
+    try:
+        account = AccountsManager.get_account(address_str)
+        return Address.from_bech32(account.address.bech32())
+    except errors.UnknownAccount:
+        pass
+    raise errors.ParsingError(address_str, 'address_str address')
+
+
 def parse_query_result(result: QueryResult, expected_return: str) -> Any:
     """
     Take the return of a query and tries to parse it in the specified return type
 
     :param result: result of a query
     :type result: QueryResult
     :param expected_return: expected return of the query
```

### Comparing `mxops-1.0.0/mxops/resources/data_parser_help.txt` & `mxops-1.1.0/mxops/resources/data_parser_help.txt`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 
 mxops data [SUBCOMMAND] [OPTIONS]
 
 Available sub-commands:
 
     get     ->  Print recorded contract data for the current env
                 Required:
-                    -n, --network           name of the network to consider (MAIN, DEV, TEST, LOCAL)
+                    -n, --network           name of the network to consider (mainnet, devnet, testnet, localnet)
                 Options:
                     -p, --path              display the root path for the user data
                     -l, --list              print all the scenarios names
                     -s, --scenario          print the data saved for a scenario
 
     delete  ->  Delete locally saved data for a specified network
                 Required:
-                    -n, --network           name of the network to consider (MAIN, DEV, TEST, LOCAL)
+                    -n, --network           name of the network to consider (mainnet, devnet, testnet, localnet)
                 Options:
                     -s, --scenario          name of the scenario to delete
                     -a, --all               delete all scenarios for the specified network
                     -y, --yes               skip confirmation step
```

### Comparing `mxops-1.0.0/mxops/resources/parser_help.txt` & `mxops-1.1.0/mxops/resources/parser_help.txt`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/utils/logger.py` & `mxops-1.1.0/mxops/utils/logger.py`

 * *Files identical despite different names*

### Comparing `mxops-1.0.0/mxops/utils/msc.py` & `mxops-1.1.0/mxops/utils/msc.py`

 * *Files 10% similar despite different names*

```diff
@@ -67,7 +67,23 @@
     file_hash = hashlib.sha256()
     with open(file_path.as_posix(), 'rb') as file:
         file_block = file.read(block_size)
         while len(file_block) > 0:
             file_hash.update(file_block)
             file_block = file.read(block_size)
     return file_hash.hexdigest()
+
+
+def int_to_pair_hex(number: int) -> str:
+    """
+    Transform an integer into its hex representation (without the 0x) and
+    ensure that there is an even number of characters by filling with 0 if necessary
+
+    :param number: number to conver
+    :type number: int
+    :return: hex representation of the number
+    :rtype: str
+    """
+    hex_str = hex(number)[2:]
+    if len(hex_str) % 2:
+        return '0' + hex_str
+    return hex_str
```

### Comparing `mxops-1.0.0/mxops.egg-info/PKG-INFO` & `mxops-1.1.0/mxops.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mxops
-Version: 1.0.0
+Version: 1.1.0
 Summary: Python package to automate MultiversX smart contracts deployment and contract interactions in general
 Author: Etienne Wallet
 Project-URL: Homepage, https://github.com/Catenscia/MxOps
 Keywords: elrond,multiversx,smart-contract,devops,tests
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MxOps
 
-MxOps is a python package created to automate MultiversX smart contracts deployments, calls and queries.
-Inspired from DevOps tools, it aims to ease and make reproducible any set of these interactions with smart-contracts.
+MxOps is a python package created to automate MultiversX transactions: be it smart contracts deployments, calls, queries or just simple transfers. Inspired from DevOps tools and built on top of [mxpy](https://github.com/multiversx/mx-sdk-py-cli), it aims to ease and make reproducible any set of these interactions with the blockchain.
 
 MxOps aims to be useful in these situations:
 
 - deployment automation
 - on-chain integration tests
 - contract interaction automation
 
@@ -30,8 +29,8 @@
 ## Contribution
 
 This tool is an humble proposal by [Catenscia](https://catenscia.com/) to have a standard way of writing deployment files, integration tests and others.
 If you want this tool to improve, please tell us your issues and proposals!
 
 And if you're motivated, we will always welcome hepling hands onboard :grin: !
 
-Read the [contribution guidelines](./CONTRIBUTING.md) for more :wink:
+Read the [contribution guidelines](https://github.com/Catenscia/MxOps/blob/main/CONTRIBUTING.md) for more :wink:
```

### Comparing `mxops-1.0.0/mxops.egg-info/SOURCES.txt` & `mxops-1.1.0/mxops.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -25,19 +25,25 @@
 mxops/execution/checks.py
 mxops/execution/cli.py
 mxops/execution/contract_interactions.py
 mxops/execution/msc.py
 mxops/execution/network.py
 mxops/execution/scene.py
 mxops/execution/steps.py
+mxops/execution/token_management.py
+mxops/execution/token_management_builders.py
 mxops/execution/utils.py
 mxops/resources/__init__.py
 mxops/resources/data_parser_help.txt
 mxops/resources/default_config.ini
 mxops/resources/parser_help.txt
 mxops/utils/__init__.py
 mxops/utils/logger.py
 mxops/utils/msc.py
-tests/test_check_transfers.py
+tests/test_checks.py
+tests/test_core_builders.py
+tests/test_data_io.py
 tests/test_execution_utils.py
 tests/test_instantiate.py
-tests/test_raise_tx_errors.py
+tests/test_raise_tx_errors.py
+tests/test_token_management.py
+tests/test_transfers_extraction.py
```

### Comparing `mxops-1.0.0/pyproject.toml` & `mxops-1.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "mxops"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   {name="Etienne Wallet"},
 ]
 description = "Python package to automate MultiversX smart contracts deployment and contract interactions in general"
 readme = "README.md"
 keywords = ["elrond", "multiversx", "smart-contract", "devops", "tests"]
 classifiers = [
```

### Comparing `mxops-1.0.0/tests/test_check_transfers.py` & `mxops-1.1.0/tests/test_transfers_extraction.py`

 * *Files 9% similar despite different names*

```diff
@@ -102,14 +102,54 @@
             'RIDE-7d18e9',
             '37'),
     ]
 
     assert transfers == expected_result
 
 
+def test_add_liquidity_with_refund(test_data_folder_path: Path):
+    # Given
+    with open(test_data_folder_path / 'api_responses' / 'add_liquidity.json') as file:
+        tx = TransactionOnNetwork.from_proxy_http_response(**json.load(file))
+
+    # When
+    transfers = ntk.get_on_chain_transfers(tx, True)
+
+    # Then
+    expected_result = [
+        OnChainTransfer(
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'erd1qqqqqqqqqqqqqpgqav09xenkuqsdyeyy5evqyhuusvu4gl3t2jpss57g8x',
+            'WEGLD-bd4d79',
+            '2662383390769244262'),
+        OnChainTransfer(
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'erd1qqqqqqqqqqqqqpgqav09xenkuqsdyeyy5evqyhuusvu4gl3t2jpss57g8x',
+            'RIDE-7d18e9',
+            '1931527217545745197301'),
+        OnChainTransfer(
+            'erd1qqqqqqqqqqqqqpgqav09xenkuqsdyeyy5evqyhuusvu4gl3t2jpss57g8x',
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'EGLDRIDE-7bd51a',
+            '1224365948567992620'),
+        OnChainTransfer(
+            'erd1qqqqqqqqqqqqqpgqav09xenkuqsdyeyy5evqyhuusvu4gl3t2jpss57g8x',
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'RIDE-7d18e9',
+            '37'),
+        OnChainTransfer(
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'erd1n775edthxhyrhntcutmqfspanmjvscumxuydmm83xumlahz75kfsgp62ss',
+            'EGLD',
+            '14546790000000'),
+    ]
+
+    assert transfers == expected_result
+
+
 def test_claim(test_data_folder_path: Path):
     # Given
     with open(test_data_folder_path / 'api_responses' / 'claim.json') as file:
         tx = TransactionOnNetwork.from_proxy_http_response(**json.load(file))
 
     # When
     transfers = ntk.get_on_chain_transfers(tx)
```

### Comparing `mxops-1.0.0/tests/test_execution_utils.py` & `mxops-1.1.0/tests/test_execution_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,11 +88,11 @@
     address = 'erd1qyu5wthldzr8wx5c9ucg8kjagg0jfs53s8nr3zpz3hypefsdd8ssycr6th'
     account_name = 'alice'
     account = Account(address)
     AccountsManager._accounts[account_name] = account
 
     # When
     arg = f'[{account_name}]'
-    retrieved_value = utils.retrieve_address_from_account(arg)
+    retrieved_value = utils.retrieve_address_from_account(arg).bech32()
 
     # Then
     assert retrieved_value == address
```

### Comparing `mxops-1.0.0/tests/test_instantiate.py` & `mxops-1.1.0/tests/test_instantiate.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,9 +52,9 @@
             print_results=True
         )
     ]
 
     assert expected_steps == loaded_steps
     assert scene.accounts == [
         {'account_name': 'owner', 'pem_path': 'wallets/local_owner.pem'}]
-    assert scene.allowed_networks == ['LOCAL']
+    assert scene.allowed_networks == ['localnet']
     assert scene.allowed_scenario == ['.*']
```

### Comparing `mxops-1.0.0/tests/test_raise_tx_errors.py` & `mxops-1.1.0/tests/test_raise_tx_errors.py`

 * *Files identical despite different names*

