# Comparing `tmp/Exegol-4.2.0.tar.gz` & `tmp/Exegol-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Exegol-4.2.0.tar", last modified: Wed May 10 03:26:51 2023, max compression
+gzip compressed data, was "Exegol-4.2.1.tar", last modified: Thu May 11 01:24:38 2023, max compression
```

## Comparing `Exegol-4.2.0.tar` & `Exegol-4.2.1.tar`

### file list

```diff
@@ -1,421 +1,421 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.695214 Exegol-4.2.0/Exegol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-10 03:26:51.000000 Exegol-4.2.0/Exegol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-10 03:26:24.000000 Exegol-4.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-10 03:26:51.767214 Exegol-4.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-10 03:26:24.000000 Exegol-4.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.695214 Exegol-4.2.0/exegol/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/ConstantConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/DataCache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/EnvInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/UserConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ConsoleFormat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ExegolProgress.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/ExegolPrompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/LayerTextColumn.py
--rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/MetaGitProgress.py
--rw-r--r--   0 runner    (1001) docker     (123)    25668 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/TUI.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/ExegolCompleter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/ParametersManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/console/cli/actions/
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/Command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/ExegolParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/GenericParameters.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/console/cli/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/exceptions/ExegolExceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/manager/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/ExegolController.py
--rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/ExegolManager.py
--rw-r--r--   0 runner    (1001) docker     (123)    19735 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/UpdateManager.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/manager/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.763214 Exegol-4.2.0/exegol/model/
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/CacheModels.py
--rw-r--r--   0 runner    (1001) docker     (123)    59376 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ContainerConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolContainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolContainerTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)    32609 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolImage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/ExegolModules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/MetaImages.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/SelectableInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/model/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/exegol/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/DataFileUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28822 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/DockerUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/ExeLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/FsUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/GitUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/GuiUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/MetaSingleton.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/WebUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-10 03:26:24.000000 Exegol-4.2.0/exegol/utils/argParse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/ad.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/debug.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/light.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/osint.dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/config.json
--rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/bloodhound/customqueries.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/crackmapexec/
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/crackmapexec/cme.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/build_pipeline_tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/load_supported_setups.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.699215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/keys.list
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/packages.list
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/apt/sources.list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/firefox/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/firefox/addons.txt
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/load_user_setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/python3/
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/python3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/supported_setups.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/aliases
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/history
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/zsh/zshrc
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/exegol/start.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.703215 Exegol-4.2.0/exegol-docker-build/sources/firefox/
--rw-r--r--   0 runner    (1001) docker     (123)  1703936 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/places.sqlite
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/firefox/user-setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/grc/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.cme
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.describeTicket
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.getgpppassword
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.krbrelayx
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.ntlmrelayx
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.rbcd
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/conf.secretsdump
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/grc/grc.conf
--rw-r--r--   0 runner    (1001) docker     (123)   180784 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/install.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/logrotate/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/logrotate/exegol_vpn
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/patches/
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/proxychains/
--rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/proxychains/proxychains.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.707214 Exegol-4.2.0/exegol-docker-build/sources/tmux/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/tmux/tmux.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.711214 Exegol-4.2.0/exegol-docker-build/sources/trilium/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)  1470464 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db
--rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-shm
--rw-r--r--   0 runner    (1001) docker     (123)  4169472 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-wal
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.715214 Exegol-4.2.0/exegol-docker-build/sources/zsh/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.739214 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/PassTheCert
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/arsenal
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bettercap
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/blazy
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/bolt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/burpsuite
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/corscanner
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/dnschef
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/donpapi
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/eaphammer
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/emacs-nox
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/empire
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/enyx
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/eyewitness
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/finalrecon
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/fuxploider
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/fzf
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gdb
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ghidra
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ghunt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/git-dumper
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gittools
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gopherus
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/gpp-decrypt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/grc
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/h2csmuggler
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ida
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/impacket
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/infoga
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jd-gui
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jdwp-shellifier
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/joomscan
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/jwt_tool
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/kraken
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/libmspack
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/linkfinder
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/nmap
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/nosqlmap
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/oneforall
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pcredz
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/photon
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/php
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/php_filter_chain_generator
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/phpggc
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/polenum
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/powershell
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxychains
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pwnedornot
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pygpoabuse
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pykek
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/python3
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/recondog
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/responder
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/routersploit
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/rsactftool
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smali
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smbmap
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/soapui
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ssrfmap
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/starkiller
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/symfony-exploits
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/testssl
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/tomcatwardeployer
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/toutatis
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/trid
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/trilium
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/username-anarchy
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/volatility2
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/vulny-code-static-analysis
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xmllint
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xsel
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/xsstrike
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/ysoserial
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.759214 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/adidnsdump
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/aircrack-ng
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/amber
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/assetfinder
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/autorecon
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-import
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bloodhound-quickwin
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/bqm
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/brakeman
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/buster
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/carbon14
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/certipy
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cewl
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cloudfail
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/clusterd
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cmsmap
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/coercer
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackhound
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackmapexec
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ctf-party
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/curl
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/cypheroth
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/darkarmour
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dfscoerce
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dirb
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dirsearch
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/divideandscan
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dnsutils
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/dnsx
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/donpapi
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/enum4linux-ng
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/enyx
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/evil-winrm
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/exif
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/exiv2
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/faketime
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fcrackzip
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fdisk
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/feroxbuster
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ffuf
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/fierce
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/finduncommonshares
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/github-email
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gmsadumper
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gobuster
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/goldencopy
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gosecretsdump
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/goshs
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/gowitness
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/h8mail
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/haiti
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hakrawler
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hakrevdns
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hashcat
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hcxdumptool
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hcxtools
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hexedit
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/holehe
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/httpmethods
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/httpx
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/impacket
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/infoga
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ipinfo
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/jackit
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/jadx
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/john-the-ripper
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kadimus
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kerbrute
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kiterunner
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kraken
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/krbrelayx
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapdomaindump
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldaprelayscan
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapsearch
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldapsearch-ad
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ldeep
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/libnfc
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/libnfc-crypto1-crack
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/linkedin2username
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/lnkup
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/lsassy
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/maigret
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/manspider
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/masscan
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mfdread
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mfoc
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mitm6
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/moodlescan
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/mousejack
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/name-that-hash
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nbtscan
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/neo4j
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/netdiscover
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ngrok
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nmap
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/notify
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ntlmv1-multi
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ntpdate
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nuclei
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/oaburl
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/objection
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/onesixtyone
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pass-station
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/petitpotam
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/phoneinfoga
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pkinittools
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/polenum
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/prips
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/privexchange
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/proxmark3
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pth-tools
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pwndb
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pyftpdlib
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pylaps
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pypykatz
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pywhisker
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/pywsus
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/responder
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/rlwrap
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/robotstester
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ruler
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/rusthound
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/samba
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/semgrep
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shadowcoerce
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shellerator
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/shuffledns
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/simplyemail
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smartbrute
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smbclient
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smbmap
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smtp-user-enum
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/smuggler
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/snmp
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/spiderfoot
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sprayhound
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sqlmap
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/ssh
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sslyze
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/subfinder
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/sublist3r
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/swaks
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tailscale
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/targetedkerberoast
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/testdisk
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/theharvester
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tls-map
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tls-scanner
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/toutatis
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/twint
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/updog
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/volatility3
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/waybackurls
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/webclientservicescanner
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wfuzz
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/whatportis
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/windapsearch
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wpscan
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/xfreerdp
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/zerologon
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/sources/zsh/zshrc
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-10 03:26:28.000000 Exegol-4.2.0/exegol-docker-build/web.dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 03:26:51.767214 Exegol-4.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-10 03:26:24.000000 Exegol-4.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 03:26:51.767214 Exegol-4.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 03:26:24.000000 Exegol-4.2.0/tests/test_exegol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.107931 Exegol-4.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.047931 Exegol-4.2.1/Exegol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18613 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-11 01:24:38.000000 Exegol-4.2.1/Exegol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-11 01:24:11.000000 Exegol-4.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6482 2023-05-11 01:24:38.107931 Exegol-4.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-11 01:24:11.000000 Exegol-4.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.047931 Exegol-4.2.1/exegol/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/config/ConstantConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/config/DataCache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/config/EnvInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6552 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/config/UserConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol/console/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/ConsoleFormat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/ExegolProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/ExegolPrompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/LayerTextColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/MetaGitProgress.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25668 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/TUI.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol/console/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/ExegolCompleter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/ParametersManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol/console/cli/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/actions/Command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13777 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/actions/ExegolParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16057 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/actions/GenericParameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/console/cli/actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/exceptions/ExegolExceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.107931 Exegol-4.2.1/exegol/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/manager/ExegolController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30595 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/manager/ExegolManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19735 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/manager/UpdateManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.107931 Exegol-4.2.1/exegol/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/CacheModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59390 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/ContainerConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13096 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/ExegolContainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/ExegolContainerTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32739 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/ExegolImage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/ExegolModules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/MetaImages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/SelectableInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/model/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.107931 Exegol-4.2.1/exegol/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     7869 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/DataFileUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29033 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/DockerUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/ExeLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/FsUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/GitUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18137 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/GuiUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/MetaSingleton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/WebUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-05-11 01:24:11.000000 Exegol-4.2.1/exegol/utils/argParse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/ad.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/debug.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/light.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/osint.dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/bloodhound/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/bloodhound/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    37672 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/bloodhound/customqueries.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/crackmapexec/
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/crackmapexec/cme.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/build_pipeline_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3456 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/load_supported_setups.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/apt/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/apt/keys.list
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/apt/packages.list
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/apt/sources.list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/firefox/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/firefox/addons.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/load_user_setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/python3/
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/python3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/supported_setups.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.051931 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/zsh/aliases
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/zsh/history
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/exegol/start.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/firefox/
+-rw-r--r--   0 runner    (1001) docker     (123)  1703936 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/firefox/places.sqlite
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/firefox/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/firefox/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/firefox/user-setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/grc/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.cme
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.describeTicket
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.getgpppassword
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.ntlmrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.rbcd
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/conf.secretsdump
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/grc/grc.conf
+-rw-r--r--   0 runner    (1001) docker     (123)   180784 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/install.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/logrotate/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/logrotate/exegol_vpn
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/proxychains/
+-rw-r--r--   0 runner    (1001) docker     (123)     5593 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/proxychains/proxychains.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.055931 Exegol-4.2.1/exegol-docker-build/sources/tmux/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/tmux/tmux.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.059931 Exegol-4.2.1/exegol-docker-build/sources/trilium/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/trilium/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)  1470464 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db
+-rw-r--r--   0 runner    (1001) docker     (123)    32768 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db-shm
+-rw-r--r--   0 runner    (1001) docker     (123)  4169472 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db-wal
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.063931 Exegol-4.2.1/exegol-docker-build/sources/zsh/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.079931 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/PassTheCert
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/arsenal
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/bettercap
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/blazy
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/bolt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/burpsuite
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/corscanner
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/dnschef
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/eaphammer
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/emacs-nox
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/empire
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/eyewitness
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/finalrecon
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/fuxploider
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/fzf
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/gdb
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ghidra
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ghunt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/git-dumper
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/gittools
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/gopherus
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/gpp-decrypt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/grc
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/h2csmuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ida
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/jd-gui
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/jdwp-shellifier
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/joomscan
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/jwt_tool
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/libmspack
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/linkfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/nosqlmap
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/oneforall
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pcredz
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/photon
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/php
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/php_filter_chain_generator
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/phpggc
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/powershell
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/proxychains
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pwnedornot
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pygpoabuse
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pykek
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/python3
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/recondog
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/responder
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/routersploit
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/rsactftool
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/smali
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/soapui
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ssrfmap
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/starkiller
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/symfony-exploits
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/testssl
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/tomcatwardeployer
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/trid
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/trilium
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/username-anarchy
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/volatility2
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/vulny-code-static-analysis
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/xmllint
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/xsel
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/xsstrike
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/ysoserial
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.103932 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/adidnsdump
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/aircrack-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/amber
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/assetfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/autorecon
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/bloodhound-import
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/bloodhound-py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/bloodhound-quickwin
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/bqm
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/brakeman
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/buster
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/carbon14
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/certipy
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/cewl
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/cloudfail
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/clusterd
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/cmsmap
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/coercer
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/crackhound
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/crackmapexec
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ctf-party
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/curl
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/cypheroth
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/darkarmour
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/dfscoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/dirb
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/dirsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/divideandscan
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/dnsutils
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/dnsx
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/donpapi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/enum4linux-ng
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/enyx
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/evil-winrm
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/exif
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/exiv2
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/faketime
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/fcrackzip
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/fdisk
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/feroxbuster
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ffuf
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/fierce
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/finduncommonshares
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/github-email
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/gmsadumper
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/gobuster
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/goldencopy
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/gosecretsdump
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/goshs
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/gowitness
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/h8mail
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/haiti
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hakrawler
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hakrevdns
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hashcat
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hcxdumptool
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hcxtools
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hexedit
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/holehe
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/httpmethods
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/httpx
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/impacket
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/infoga
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ipinfo
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/jackit
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/jadx
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/john-the-ripper
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/kadimus
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/kerbrute
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/kiterunner
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/kraken
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/krbrelayx
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ldapdomaindump
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ldaprelayscan
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ldapsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ldapsearch-ad
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ldeep
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/libnfc
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/libnfc-crypto1-crack
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/linkedin2username
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/lnkup
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/lsassy
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/maigret
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/manspider
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/masscan
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/mfdread
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/mfoc
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/mitm6
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/moodlescan
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/mousejack
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/name-that-hash
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/nbtscan
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/neo4j
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/netdiscover
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ngrok
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/nmap
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/notify
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ntlmv1-multi
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ntpdate
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/nuclei
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/oaburl
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/objection
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/onesixtyone
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pass-station
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/petitpotam
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/phoneinfoga
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pkinittools
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/polenum
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/prips
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/privexchange
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/proxmark3
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pth-tools
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pwndb
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pyftpdlib
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pylaps
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pypykatz
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pywhisker
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/pywsus
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/responder
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/rlwrap
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/robotstester
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ruler
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/rusthound
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/samba
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/semgrep
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/shadowcoerce
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/shellerator
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/shuffledns
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/simplyemail
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/smartbrute
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/smbclient
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/smbmap
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/smtp-user-enum
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/smuggler
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/snmp
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/spiderfoot
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/sprayhound
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/sqlmap
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/ssh
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/sslyze
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/subfinder
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/sublist3r
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/swaks
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/tailscale
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/targetedkerberoast
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/testdisk
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/theharvester
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/tls-map
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/tls-scanner
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/toutatis
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/twint
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/updog
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/volatility3
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/waybackurls
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/webclientservicescanner
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/wfuzz
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/whatportis
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/windapsearch
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/wpscan
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/xfreerdp
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/zerologon
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/sources/zsh/zshrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-11 01:24:14.000000 Exegol-4.2.1/exegol-docker-build/web.dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 01:24:38.107931 Exegol-4.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-11 01:24:11.000000 Exegol-4.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 01:24:38.107931 Exegol-4.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-11 01:24:11.000000 Exegol-4.2.1/tests/test_exegol.py
```

### Comparing `Exegol-4.2.0/Exegol.egg-info/PKG-INFO` & `Exegol-4.2.1/Exegol.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
```

### Comparing `Exegol-4.2.0/Exegol.egg-info/SOURCES.txt` & `Exegol-4.2.1/Exegol.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/LICENSE` & `Exegol-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/PKG-INFO` & `Exegol-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Exegol
-Version: 4.2.0
+Version: 4.2.1
 Summary: Python wrapper to use Exegol, a container based fully featured and community-driven hacking environment.
 Home-page: https://github.com/ThePorgs/Exegol
 Author: Shutdown & Dramelac
 Author-email: nwodtuhs@pm.me
 License: GNU (GPLv3)
 Project-URL: Bug Reports, https://github.com/ThePorgs/Exegol/issues
 Project-URL: Source, https://github.com/ThePorgs/Exegol
```

### Comparing `Exegol-4.2.0/README.md` & `Exegol-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/config/ConstantConfig.py` & `Exegol-4.2.1/exegol/config/ConstantConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import site
 from pathlib import Path
 
 
 class ConstantConfig:
     """Constant parameters information"""
     # Exegol Version
-    version: str = "4.2.0"
+    version: str = "4.2.1"
 
     # Exegol documentation link
     documentation: str = "https://exegol.rtfd.io/"
     discord: str = "https://discord.gg/cXThyp7D6P"
     # OS Dir full root path of exegol project
     src_root_path_obj: Path = Path(__file__).parent.parent.parent.resolve()
     # Path of the Dockerfile
```

### Comparing `Exegol-4.2.0/exegol/config/DataCache.py` & `Exegol-4.2.1/exegol/config/DataCache.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/config/EnvInfo.py` & `Exegol-4.2.1/exegol/config/EnvInfo.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/config/UserConfig.py` & `Exegol-4.2.1/exegol/config/UserConfig.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/ConsoleFormat.py` & `Exegol-4.2.1/exegol/console/ConsoleFormat.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/ExegolProgress.py` & `Exegol-4.2.1/exegol/console/ExegolProgress.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/LayerTextColumn.py` & `Exegol-4.2.1/exegol/console/LayerTextColumn.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/MetaGitProgress.py` & `Exegol-4.2.1/exegol/console/MetaGitProgress.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/TUI.py` & `Exegol-4.2.1/exegol/console/TUI.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/cli/ExegolCompleter.py` & `Exegol-4.2.1/exegol/console/cli/ExegolCompleter.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/cli/ParametersManager.py` & `Exegol-4.2.1/exegol/console/cli/ParametersManager.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/cli/actions/Command.py` & `Exegol-4.2.1/exegol/console/cli/actions/Command.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/cli/actions/ExegolParameters.py` & `Exegol-4.2.1/exegol/console/cli/actions/ExegolParameters.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/console/cli/actions/GenericParameters.py` & `Exegol-4.2.1/exegol/console/cli/actions/GenericParameters.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/manager/ExegolController.py` & `Exegol-4.2.1/exegol/manager/ExegolController.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/manager/ExegolManager.py` & `Exegol-4.2.1/exegol/manager/ExegolManager.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/manager/UpdateManager.py` & `Exegol-4.2.1/exegol/manager/UpdateManager.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/model/CacheModels.py` & `Exegol-4.2.1/exegol/model/CacheModels.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/model/ContainerConfig.py` & `Exegol-4.2.1/exegol/model/ContainerConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -797,15 +797,15 @@
             try:
                 if not (path.is_file() or path.is_dir()):
                     if must_exist:
                         raise CancelOperation(f"{host_path} does not exist on your host.")
                     else:
                         # If the directory is created by exegol, bypass user preference and enable shared perms (if available)
                         execute_update_fs = force_sticky_group or enable_sticky_group
-                        path.mkdir(exist_ok=True)
+                        path.mkdir(parents=True, exist_ok=True)
             except PermissionError:
                 logger.error("Unable to create the volume folder on the filesystem locally.")
                 logger.critical(f"Insufficient permissions to create the folder: {host_path}")
             except FileExistsError:
                 # The volume targets a file that already exists on the file system
                 pass
             # Update FS don't work on Windows and only for directory
```

### Comparing `Exegol-4.2.0/exegol/model/ExegolContainer.py` & `Exegol-4.2.1/exegol/model/ExegolContainer.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/model/ExegolContainerTemplate.py` & `Exegol-4.2.1/exegol/model/ExegolContainerTemplate.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/model/ExegolImage.py` & `Exegol-4.2.1/exegol/model/ExegolImage.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,17 @@
             self.__initFromDockerImage()
         else:
             self.__setImageId(image_id)
             if dockerhub_data:
                 self.__is_remote = True
                 self.__setArch(MetaImages.parseArch(dockerhub_data))
                 self.__dl_size = self.__processSize(dockerhub_data.get("size", 0))
-            if meta_img:
+            if meta_img and meta_img.meta_id is not None:
                 self.__setDigest(meta_img.meta_id)
+                self.__setLatestRemoteId(meta_img.meta_id)  # Meta id is always the latest one
         logger.debug(f"└── {self.__name}\t→ ({self.getType()}) {self.__digest}")
 
     def __initFromDockerImage(self):
         """Parse Docker object to set up self configuration on creation."""
         assert self.__image is not None
         # If docker object exists, image is already installed
         self.__is_install = True
@@ -193,15 +194,15 @@
         self.__setLatestVersion(meta.version)
         if meta.meta_id:
             self.__setLatestRemoteId(meta.meta_id)
         # Check if local image is sync with remote digest id (check up-to-date status)
         self.__is_update = self.__digest == self.__profile_digest
         if not self.__digest and meta.is_latest and meta.meta_id:
             # If the digest is lost (multiple same image installed locally) fallback to meta id (only if latest)
-            self.__digest = meta.meta_id
+            self.__setDigest(meta.meta_id)
         # Refresh status after metadata update
         self.syncStatus()
 
     def setAsDiscontinued(self):
         logger.debug(f"The image '{self.getName()}' (digest: {self.getRemoteId()}) has not been found remotely, "
                      f"considering it as discontinued.")
         # If there are still remote images but the image has not found any match it is because it has been deleted/discontinued
```

### Comparing `Exegol-4.2.0/exegol/model/ExegolModules.py` & `Exegol-4.2.1/exegol/model/ExegolModules.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/model/MetaImages.py` & `Exegol-4.2.1/exegol/model/MetaImages.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/DataFileUtils.py` & `Exegol-4.2.1/exegol/utils/DataFileUtils.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def __load_file(self):
         """
         Function to load the file and the corresponding parameters
         :return:
         """
         if not self._file_path.parent.is_dir():
             logger.verbose(f"Creating config folder: {self._file_path.parent}")
-            self._file_path.parent.mkdir()
+            self._file_path.parent.mkdir(parents=True, exist_ok=True)
         if not self._file_path.is_file():
             logger.verbose(f"Creating default file: {self._file_path}")
             self._create_config_file()
         else:
             self._parse_config()
             if self.__config_upgrade:
                 logger.verbose("Upgrading config file")
```

### Comparing `Exegol-4.2.0/exegol/utils/DockerUtils.py` & `Exegol-4.2.1/exegol/utils/DockerUtils.py`

 * *Files 3% similar despite different names*

```diff
@@ -392,16 +392,20 @@
         # Remove duplication (version specific / latest release)
         return remote_results
 
     @classmethod
     def __findImageMatch(cls, remote_image: ExegolImage):
         """From a Remote ExegolImage, try to find a local match (using Remote DigestID).
         This method is useful if the image repository name is also lost"""
+        remote_id = remote_image.getLatestRemoteId()
+        if not remote_id:
+            logger.debug("Latest remote id is not available... Falling back to the current remote id.")
+            remote_id = remote_image.getRemoteId()
         try:
-            docker_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_image.getLatestRemoteId()}")
+            docker_image = cls.__client.images.get(f"{ConstantConfig.IMAGE_NAME}@{remote_id}")
         except ImageNotFound:
             raise ObjectNotFound
         remote_image.resetDockerImage()
         remote_image.setDockerObject(docker_image)
 
     @classmethod
     def downloadImage(cls, image: ExegolImage, install_mode: bool = False) -> bool:
```

### Comparing `Exegol-4.2.0/exegol/utils/ExeLog.py` & `Exegol-4.2.1/exegol/utils/ExeLog.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/FsUtils.py` & `Exegol-4.2.1/exegol/utils/FsUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/GitUtils.py` & `Exegol-4.2.1/exegol/utils/GitUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/GuiUtils.py` & `Exegol-4.2.1/exegol/utils/GuiUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/MetaSingleton.py` & `Exegol-4.2.1/exegol/utils/MetaSingleton.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/WebUtils.py` & `Exegol-4.2.1/exegol/utils/WebUtils.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol/utils/argParse.py` & `Exegol-4.2.1/exegol/utils/argParse.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/Dockerfile` & `Exegol-4.2.1/exegol-docker-build/Dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/ad.dockerfile` & `Exegol-4.2.1/exegol-docker-build/ad.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/debug.dockerfile` & `Exegol-4.2.1/exegol-docker-build/debug.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/light.dockerfile` & `Exegol-4.2.1/exegol-docker-build/light.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/osint.dockerfile` & `Exegol-4.2.1/exegol-docker-build/osint.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/bloodhound/config.json` & `Exegol-4.2.1/exegol-docker-build/sources/bloodhound/config.json`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/bloodhound/customqueries.json` & `Exegol-4.2.1/exegol-docker-build/sources/bloodhound/customqueries.json`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/build_pipeline_tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/entrypoint.sh` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/load_supported_setups.sh` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/load_supported_setups.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/README.md` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/README.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/load_user_setup.sh` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/load_user_setup.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/skel/supported_setups.md` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/skel/supported_setups.md`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/exegol/start.sh` & `Exegol-4.2.1/exegol-docker-build/sources/exegol/start.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/firefox/places.sqlite` & `Exegol-4.2.1/exegol-docker-build/sources/firefox/places.sqlite`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/firefox/setup.py` & `Exegol-4.2.1/exegol-docker-build/sources/firefox/setup.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/firefox/user-setup.py` & `Exegol-4.2.1/exegol-docker-build/sources/firefox/user-setup.py`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.getgpppassword` & `Exegol-4.2.1/exegol-docker-build/sources/grc/conf.getgpppassword`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.ntlmrelayx` & `Exegol-4.2.1/exegol-docker-build/sources/grc/conf.ntlmrelayx`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.rbcd` & `Exegol-4.2.1/exegol-docker-build/sources/grc/conf.rbcd`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/grc/conf.secretsdump` & `Exegol-4.2.1/exegol-docker-build/sources/grc/conf.secretsdump`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/grc/grc.conf` & `Exegol-4.2.1/exegol-docker-build/sources/grc/grc.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/install.sh` & `Exegol-4.2.1/exegol-docker-build/sources/install.sh`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch` & `Exegol-4.2.1/exegol-docker-build/sources/patches/undefined-symbol-aesni-key.patch`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/proxychains/proxychains.conf` & `Exegol-4.2.1/exegol-docker-build/sources/proxychains/proxychains.conf`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/trilium/config.ini` & `Exegol-4.2.1/exegol-docker-build/sources/trilium/config.ini`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db` & `Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-shm` & `Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db-shm`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/trilium/document.db-wal` & `Exegol-4.2.1/exegol-docker-build/sources/trilium/document.db-wal`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/proxmark3` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/proxmark3`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/aliases.d/responder` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/aliases.d/responder`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/crackmapexec` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/crackmapexec`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/hashcat` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/hashcat`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/impacket` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/impacket`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/kiterunner` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/kiterunner`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/krbrelayx` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/krbrelayx`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/nmap` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/nmap`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/tls-map` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/tls-map`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/volatility3` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/volatility3`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/history.d/wfuzz` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/history.d/wfuzz`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/sources/zsh/zshrc` & `Exegol-4.2.1/exegol-docker-build/sources/zsh/zshrc`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/exegol-docker-build/web.dockerfile` & `Exegol-4.2.1/exegol-docker-build/web.dockerfile`

 * *Files identical despite different names*

### Comparing `Exegol-4.2.0/setup.py` & `Exegol-4.2.1/setup.py`

 * *Files identical despite different names*

