# Comparing `tmp/edk2-basetools-0.1.8.tar.gz` & `tmp/edk2-basetools-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edk2-basetools-0.1.8.tar", last modified: Sat Jan 22 09:07:32 2022, max compression
+gzip compressed data, was "edk2-basetools-0.1.9.tar", last modified: Sat Jan 22 09:38:58 2022, max compression
```

## Comparing `edk2-basetools-0.1.8.tar` & `edk2-basetools-0.1.9.tar`

### file list

```diff
@@ -1,375 +1,375 @@
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.136473 edk2-basetools-0.1.8/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.808474 edk2-basetools-0.1.8/.azurepipelines/
--rw-rw-rw-   0        0        0      459 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/azure-pipelines-release.yml
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.815474 edk2-basetools-0.1.8/.azurepipelines/templates/
--rw-rw-rw-   0        0        0      520 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/basic-setup-steps.yml
--rw-rw-rw-   0        0        0      968 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/build-publish-whl-steps.yml
--rw-rw-rw-   0        0        0     1308 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/build-test-job.yml
--rw-rw-rw-   0        0        0      660 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/flake8-test-steps.yml
--rw-rw-rw-   0        0        0      438 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/markdown-lint-steps.yml
--rw-rw-rw-   0        0        0     1692 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/pytest-test-steps.yml
--rw-rw-rw-   0        0        0      486 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/templates/spell-test-steps.yml
--rw-rw-rw-   0        0        0      423 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/ubuntu-test-pr-ci.yml
--rw-rw-rw-   0        0        0      421 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.azurepipelines/windows-test-pr-ci.yml
--rw-rw-rw-   0        0        0     1599 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/.cspell.json
--rw-rw-rw-   0        0        0     2489 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/BasicDevTests.py
--rw-rw-rw-   0        0        0     1429 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/ConfirmVersionAndTag.py
--rw-rw-rw-   0        0        0      102 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     4716 2022-01-22 09:07:32.135472 edk2-basetools-0.1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.817474 edk2-basetools-0.1.8/docs/
--rw-rw-rw-   0        0        0     1797 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/docs/coverage.md
--rw-rw-rw-   0        0        0     1691 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/docs/publishing.md
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.823472 edk2-basetools-0.1.8/edk2_basetools.egg-info/
--rw-rw-rw-   0        0        0     4716 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    12702 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      105 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2022-01-22 09:07:31.000000 edk2-basetools-0.1.8/edk2_basetools.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.828474 edk2-basetools-0.1.8/edk2basetools/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.829473 edk2-basetools-0.1.8/edk2basetools/AmlToC/
--rw-rw-rw-   0        0        0     4677 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AmlToC/AmlToC.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.850475 edk2-basetools-0.1.8/edk2basetools/AutoGen/
--rw-rw-rw-   0        0        0     4646 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/AutoGen.py
--rw-rw-rw-   0        0        0    15154 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/AutoGenWorker.py
--rw-rw-rw-   0        0        0    26598 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/BuildEngine.py
--rw-rw-rw-   0        0        0     7181 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/DataPipe.py
--rw-rw-rw-   0        0        0    94675 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/GenC.py
--rw-rw-rw-   0        0        0    21188 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/GenDepex.py
--rw-rw-rw-   0        0        0    78532 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/GenMake.py
--rw-rw-rw-   0        0        0    72646 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/GenPcdDb.py
--rw-rw-rw-   0        0        0    16258 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/GenVar.py
--rw-rw-rw-   0        0        0     5749 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/IdfClassObject.py
--rw-rw-rw-   0        0        0    14610 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/IncludesAutoGen.py
--rw-rw-rw-   0        0        0     4624 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/InfSectionParser.py
--rw-rw-rw-   0        0        0   109827 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/ModuleAutoGen.py
--rw-rw-rw-   0        0        0    30806 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/ModuleAutoGenHelper.py
--rw-rw-rw-   0        0        0    83657 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/PlatformAutoGen.py
--rw-rw-rw-   0        0        0    22439 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/StrGather.py
--rw-rw-rw-   0        0        0    29657 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/UniClassObject.py
--rw-rw-rw-   0        0        0    10205 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/ValidCheckingInfoObject.py
--rw-rw-rw-   0        0        0    46637 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/WorkspaceAutoGen.py
--rw-rw-rw-   0        0        0      313 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/AutoGen/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.854478 edk2-basetools-0.1.8/edk2basetools/BPDG/
--rw-rw-rw-   0        0        0     6086 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/BPDG/BPDG.py
--rw-rw-rw-   0        0        0    33024 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/BPDG/GenVpd.py
--rw-rw-rw-   0        0        0     3174 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/BPDG/StringTable.py
--rw-rw-rw-   0        0        0      278 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/BPDG/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.857476 edk2-basetools-0.1.8/edk2basetools/Capsule/
--rw-rw-rw-   0        0        0    58579 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Capsule/GenerateCapsule.py
--rw-rw-rw-   0        0        0     5892 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Capsule/GenerateWindowsDriver.py
--rw-rw-rw-   0        0        0     2660 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Capsule/WindowsCapsuleSupportHelper.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.886478 edk2-basetools-0.1.8/edk2basetools/Common/
--rw-rw-rw-   0        0        0     5253 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/BuildToolError.py
--rw-rw-rw-   0        0        0      266 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/BuildVersion.py
--rw-rw-rw-   0        0        0    23720 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/DataType.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.892474 edk2-basetools-0.1.8/edk2basetools/Common/Edk2/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.895474 edk2-basetools-0.1.8/edk2basetools/Common/Edk2/Capsule/
--rw-rw-rw-   0        0        0     3450 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Edk2/Capsule/FmpPayloadHeader.py
--rw-rw-rw-   0        0        0      293 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Edk2/Capsule/__init__.py
--rw-rw-rw-   0        0        0      285 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Edk2/__init__.py
--rw-rw-rw-   0        0        0    12973 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/EdkLogger.py
--rw-rw-rw-   0        0        0    44557 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Expression.py
--rw-rw-rw-   0        0        0     3620 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/GlobalData.py
--rw-rw-rw-   0        0        0     1888 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathOs.py
--rw-rw-rw-   0        0        0     1239 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathOsPath.py
--rw-rw-rw-   0        0        0     1344 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathSupport.py
--rw-rw-rw-   0        0        0    73267 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Misc.py
--rw-rw-rw-   0        0        0     5104 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/MultipleWorkspace.py
--rw-rw-rw-   0        0        0    39051 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Parsing.py
--rw-rw-rw-   0        0        0    25319 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/RangeExpression.py
--rw-rw-rw-   0        0        0    29531 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/StringUtils.py
--rw-rw-rw-   0        0        0     9068 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/TargetTxtClassObject.py
--rw-rw-rw-   0        0        0    12974 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/ToolDefClassObject.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.896900 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.903473 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/
--rw-rw-rw-   0        0        0    17261 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/CapsuleDependency.py
--rw-rw-rw-   0        0        0     7883 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/FmpAuthHeader.py
--rw-rw-rw-   0        0        0    14854 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/FmpCapsuleHeader.py
--rw-rw-rw-   0        0        0     5521 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/UefiCapsuleHeader.py
--rw-rw-rw-   0        0        0      293 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/__init__.py
--rw-rw-rw-   0        0        0      285 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/Uefi/__init__.py
--rw-rw-rw-   0        0        0     1961 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/VariableAttributes.py
--rw-rw-rw-   0        0        0    11682 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/VpdInfoFile.py
--rw-rw-rw-   0        0        0      287 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/__init__.py
--rw-rw-rw-   0        0        0     1320 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Common/caching.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.892474 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/
--rw-rw-rw-   0        0        0     3862 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/CommonClass.py
--rw-rw-rw-   0        0        0    16528 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/DataClass.py
--rw-rw-rw-   0        0        0      530 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/Exceptions.py
--rw-rw-rw-   0        0        0     7612 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/FdfClass.py
--rw-rw-rw-   0        0        0      296 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/CommonDataClass/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.919474 edk2-basetools-0.1.8/edk2basetools/Ecc/
--rw-rw-rw-   0        0        0    17207 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/C.g
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.923473 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/
--rw-rw-rw-   0        0        0    98792 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/CLexer.py
--rw-rw-rw-   0        0        0   698147 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/CParser.py
--rw-rw-rw-   0        0        0        0 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.927474 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/
--rw-rw-rw-   0        0        0    15914 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/C.g4
--rw-rw-rw-   0        0        0    38792 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CLexer.py
--rw-rw-rw-   0        0        0    26606 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CListener.py
--rw-rw-rw-   0        0        0   257504 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CParser.py
--rw-rw-rw-   0        0        0        0 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/__init__.py
--rw-rw-rw-   0        0        0   102733 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Check.py
--rw-rw-rw-   0        0        0     4891 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CodeFragment.py
--rw-rw-rw-   0        0        0    25592 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/CodeFragmentCollector.py
--rw-rw-rw-   0        0        0    23197 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Configuration.py
--rw-rw-rw-   0        0        0    14082 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Database.py
--rw-rw-rw-   0        0        0      432 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/EccGlobalData.py
--rw-rw-rw-   0        0        0    19353 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/EccMain.py
--rw-rw-rw-   0        0        0    14452 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/EccToolError.py
--rw-rw-rw-   0        0        0     2713 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Exception.py
--rw-rw-rw-   0        0        0     1332 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/FileProfile.py
--rw-rw-rw-   0        0        0    10766 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaDataParser.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.932476 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/
--rw-rw-rw-   0        0        0     6200 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaDataTable.py
--rw-rw-rw-   0        0        0   100873 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaFileParser.py
--rw-rw-rw-   0        0        0    13080 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaFileTable.py
--rw-rw-rw-   0        0        0      290 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/__init__.py
--rw-rw-rw-   0        0        0      782 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/ParserWarning.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.934473 edk2-basetools-0.1.8/edk2basetools/Ecc/Xml/
--rw-rw-rw-   0        0        0     7254 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Xml/XmlRoutines.py
--rw-rw-rw-   0        0        0      308 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/Xml/__init__.py
--rw-rw-rw-   0        0        0      284 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/__init__.py
--rw-rw-rw-   0        0        0   113709 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/c.py
--rw-rw-rw-   0        0        0    11328 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/config.ini
--rw-rw-rw-   0        0        0     7951 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Ecc/exception.xml
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.948473 edk2-basetools-0.1.8/edk2basetools/Eot/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.952473 edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/
--rw-rw-rw-   0        0        0    98792 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/CLexer.py
--rw-rw-rw-   0        0        0   698115 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/CParser.py
--rw-rw-rw-   0        0        0        0 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.955474 edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/
--rw-rw-rw-   0        0        0    38794 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CLexer.py
--rw-rw-rw-   0        0        0    26604 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CListener.py
--rw-rw-rw-   0        0        0   257504 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CParser.py
--rw-rw-rw-   0        0        0        0 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/__init__.py
--rw-rw-rw-   0        0        0     5503 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CodeFragment.py
--rw-rw-rw-   0        0        0    16753 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/CodeFragmentCollector.py
--rw-rw-rw-   0        0        0     9735 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/Database.py
--rw-rw-rw-   0        0        0    11283 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/EfiCompressor.pyd
--rw-rw-rw-   0        0        0     3720 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/EotGlobalData.py
--rw-rw-rw-   0        0        0    69058 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/EotMain.py
--rw-rw-rw-   0        0        0      292 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/EotToolError.py
--rw-rw-rw-   0        0        0     1378 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/FileProfile.py
--rw-rw-rw-   0        0        0     1365 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/Identification.py
--rw-rw-rw-   0        0        0     5750 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/InfParserLite.py
--rw-rw-rw-   0        0        0    14875 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/LzmaCompressor.pyd
--rw-rw-rw-   0        0        0    34281 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/Parser.py
--rw-rw-rw-   0        0        0      620 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/ParserWarning.py
--rw-rw-rw-   0        0        0    17383 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/Report.py
--rw-rw-rw-   0        0        0      277 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/__init__.py
--rw-rw-rw-   0        0        0    14082 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Eot/c.py
--rw-rw-rw-   0        0        0      245 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GNUmakefile
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.981473 edk2-basetools-0.1.8/edk2basetools/GenFds/
--rw-rw-rw-   0        0        0     4971 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/AprioriSection.py
--rw-rw-rw-   0        0        0    10484 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Capsule.py
--rw-rw-rw-   0        0        0     7184 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/CapsuleData.py
--rw-rw-rw-   0        0        0     3607 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/CompressSection.py
--rw-rw-rw-   0        0        0     5184 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/DataSection.py
--rw-rw-rw-   0        0        0     5205 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/DepexSection.py
--rw-rw-rw-   0        0        0    15655 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/EfiSection.py
--rw-rw-rw-   0        0        0     7130 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Fd.py
--rw-rw-rw-   0        0        0   194986 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/FdfParser.py
--rw-rw-rw-   0        0        0     1960 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Ffs.py
--rw-rw-rw-   0        0        0     7916 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/FfsFileStatement.py
--rw-rw-rw-   0        0        0    54740 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/FfsInfStatement.py
--rw-rw-rw-   0        0        0    20222 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Fv.py
--rw-rw-rw-   0        0        0     7357 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/FvImageSection.py
--rw-rw-rw-   0        0        0    42610 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/GenFds.py
--rw-rw-rw-   0        0        0    45566 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/GenFdsGlobalVariable.py
--rw-rw-rw-   0        0        0    12718 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/GuidSection.py
--rw-rw-rw-   0        0        0     1127 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/OptRomFileStatement.py
--rw-rw-rw-   0        0        0     5611 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/OptRomInfStatement.py
--rw-rw-rw-   0        0        0     5624 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/OptionRom.py
--rw-rw-rw-   0        0        0    15900 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Region.py
--rw-rw-rw-   0        0        0      474 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Rule.py
--rw-rw-rw-   0        0        0      584 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/RuleComplexFile.py
--rw-rw-rw-   0        0        0      579 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/RuleSimpleFile.py
--rw-rw-rw-   0        0        0     6680 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/Section.py
--rw-rw-rw-   0        0        0     2757 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/UiSection.py
--rw-rw-rw-   0        0        0     2973 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/VerSection.py
--rw-rw-rw-   0        0        0      287 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenFds/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.983474 edk2-basetools-0.1.8/edk2basetools/GenPatchPcdTable/
--rw-rw-rw-   0        0        0     9435 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenPatchPcdTable/GenPatchPcdTable.py
--rw-rw-rw-   0        0        0      290 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/GenPatchPcdTable/__init__.py
--rw-rw-rw-   0        0        0      266 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Makefile
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.985473 edk2-basetools-0.1.8/edk2basetools/PatchPcdValue/
--rw-rw-rw-   0        0        0    10510 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/PatchPcdValue/PatchPcdValue.py
--rw-rw-rw-   0        0        0      287 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/PatchPcdValue/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.994473 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/
--rw-rw-rw-   0        0        0    11244 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/Pkcs7Sign.py
--rw-rw-rw-   0        0        0     6631 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/Readme.md
--rw-rw-rw-   0        0        0     3659 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestCert.pem
--rw-rw-rw-   0        0        0     1530 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestCert.pub.pem
--rw-rw-rw-   0        0        0     1008 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer
--rw-rw-rw-   0        0        0     6099 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer.gEfiSecurityPkgTokenSpaceGuid.PcdPkcs7CertBuffer.inc
--rw-rw-rw-   0        0        0     6133 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer.gFmpDevicePkgTokenSpaceGuid.PcdFmpDevicePkcs7CertBufferXdr.inc
--rw-rw-rw-   0        0        0     3578 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.pem
--rw-rw-rw-   0        0        0     1442 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.pub.pem
--rw-rw-rw-   0        0        0     3285 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestSub.pem
--rw-rw-rw-   0        0        0     1414 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestSub.pub.pem
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.999472 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/
--rw-rw-rw-   0        0        0     6532 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256GenerateKeys.py
--rw-rw-rw-   0        0        0     9193 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256Sign.py
--rw-rw-rw-   0        0        0     1706 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/TestSigningPrivateKey.pem
--rw-rw-rw-   0        0        0       32 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/TestSigningPublicKey.bin
--rw-rw-rw-   0        0        0      194 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/TestSigningPublicKey.txt
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.001473 edk2-basetools-0.1.8/edk2basetools/Split/
--rw-rw-rw-   0        0        0     7189 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Split/Split.py
--rw-rw-rw-   0        0        0      215 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Split/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.013473 edk2-basetools-0.1.8/edk2basetools/Table/
--rw-rw-rw-   0        0        0     2919 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/Table.py
--rw-rw-rw-   0        0        0     3076 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableDataModel.py
--rw-rw-rw-   0        0        0     4635 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableDec.py
--rw-rw-rw-   0        0        0     4619 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableDsc.py
--rw-rw-rw-   0        0        0     3226 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableEotReport.py
--rw-rw-rw-   0        0        0     4749 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableFdf.py
--rw-rw-rw-   0        0        0     3743 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableFile.py
--rw-rw-rw-   0        0        0     4614 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableFunction.py
--rw-rw-rw-   0        0        0     4032 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableIdentifier.py
--rw-rw-rw-   0        0        0     5043 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableInf.py
--rw-rw-rw-   0        0        0     3980 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TablePcd.py
--rw-rw-rw-   0        0        0     2197 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableQuery.py
--rw-rw-rw-   0        0        0     5644 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/TableReport.py
--rw-rw-rw-   0        0        0      286 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Table/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.014473 edk2-basetools-0.1.8/edk2basetools/TargetTool/
--rw-rw-rw-   0        0        0    13876 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/TargetTool/TargetTool.py
--rw-rw-rw-   0        0        0      291 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/TargetTool/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.015473 edk2-basetools-0.1.8/edk2basetools/Trim/
--rw-rw-rw-   0        0        0    26557 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Trim/Trim.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.021472 edk2-basetools-0.1.8/edk2basetools/UPT/
--rw-rw-rw-   0        0        0      305 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/BuildVersion.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.028473 edk2-basetools-0.1.8/edk2basetools/UPT/Core/
--rw-rw-rw-   0        0        0    17446 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/DependencyRules.py
--rw-rw-rw-   0        0        0    11375 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/DistributionPackageClass.py
--rw-rw-rw-   0        0        0     6486 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/FileHook.py
--rw-rw-rw-   0        0        0    33706 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/IpiDb.py
--rw-rw-rw-   0        0        0     8764 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/PackageFile.py
--rw-rw-rw-   0        0        0      319 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Core/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.033473 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/
--rw-rw-rw-   0        0        0    27305 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenDecFile.py
--rw-rw-rw-   0        0        0    46494 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenInfFile.py
--rw-rw-rw-   0        0        0     7386 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenMetaFileMisc.py
--rw-rw-rw-   0        0        0      240 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenXmlFile.py
--rw-rw-rw-   0        0        0      316 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/__init__.py
--rw-rw-rw-   0        0        0    37920 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/InstallPkg.py
--rw-rw-rw-   0        0        0     3789 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/InventoryWs.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.042472 edk2-basetools-0.1.8/edk2basetools/UPT/Library/
--rw-rw-rw-   0        0        0     9411 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/CommentGenerating.py
--rw-rw-rw-   0        0        0    22525 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/CommentParsing.py
--rw-rw-rw-   0        0        0    33789 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/DataType.py
--rw-rw-rw-   0        0        0    18091 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/ExpressionValidate.py
--rw-rw-rw-   0        0        0     1806 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/GlobalData.py
--rw-rw-rw-   0        0        0    31580 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/Misc.py
--rw-rw-rw-   0        0        0    19900 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/ParserValidate.py
--rw-rw-rw-   0        0        0    39944 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/Parsing.py
--rw-rw-rw-   0        0        0    31352 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/StringUtils.py
--rw-rw-rw-   0        0        0    50047 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/UniClassObject.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.044473 edk2-basetools-0.1.8/edk2basetools/UPT/Library/Xml/
--rw-rw-rw-   0        0        0     6937 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/Xml/XmlRoutines.py
--rw-rw-rw-   0        0        0      308 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/Xml/__init__.py
--rw-rw-rw-   0        0        0      312 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Library/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.047472 edk2-basetools-0.1.8/edk2basetools/UPT/Logger/
--rw-rw-rw-   0        0        0     8875 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Logger/Log.py
--rw-rw-rw-   0        0        0    46178 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Logger/StringTable.py
--rw-rw-rw-   0        0        0     5795 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Logger/ToolError.py
--rw-rw-rw-   0        0        0      310 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Logger/__init__.py
--rw-rw-rw-   0        0        0    10209 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/MkPkg.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.048473 edk2-basetools-0.1.8/edk2basetools/UPT/Object/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.053477 edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/
--rw-rw-rw-   0        0        0    25908 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/CommonObject.py
--rw-rw-rw-   0        0        0    16270 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/ModuleObject.py
--rw-rw-rw-   0        0        0     5106 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/PackageObject.py
--rw-rw-rw-   0        0        0      307 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.081471 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/
--rw-rw-rw-   0        0        0    15031 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/DecObject.py
--rw-rw-rw-   0        0        0    33097 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfBinaryObject.py
--rw-rw-rw-   0        0        0     2820 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfBuildOptionObject.py
--rw-rw-rw-   0        0        0     3340 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfCommonObject.py
--rw-rw-rw-   0        0        0     2327 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDefineCommonObject.py
--rw-rw-rw-   0        0        0    41374 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDefineObject.py
--rw-rw-rw-   0        0        0     5147 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDepexObject.py
--rw-rw-rw-   0        0        0    13345 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfGuidObject.py
--rw-rw-rw-   0        0        0     2462 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfHeaderObject.py
--rw-rw-rw-   0        0        0    10541 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfLibraryClassesObject.py
--rw-rw-rw-   0        0        0     3924 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfMisc.py
--rw-rw-rw-   0        0        0     7352 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPackagesObject.py
--rw-rw-rw-   0        0        0    26617 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPcdObject.py
--rw-rw-rw-   0        0        0    12506 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPpiObject.py
--rw-rw-rw-   0        0        0    11092 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfProtocolObject.py
--rw-rw-rw-   0        0        0     8493 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfSoucesObject.py
--rw-rw-rw-   0        0        0     4826 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfUserExtensionObject.py
--rw-rw-rw-   0        0        0      310 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/__init__.py
--rw-rw-rw-   0        0        0      310 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Object/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.099470 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/
--rw-rw-rw-   0        0        0    45165 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/DecParser.py
--rw-rw-rw-   0        0        0    10933 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/DecParserMisc.py
--rw-rw-rw-   0        0        0     9276 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfAsBuiltProcess.py
--rw-rw-rw-   0        0        0     8869 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfBinarySectionParser.py
--rw-rw-rw-   0        0        0     8472 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfBuildOptionSectionParser.py
--rw-rw-rw-   0        0        0     6837 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfDefineSectionParser.py
--rw-rw-rw-   0        0        0     3506 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfDepexSectionParser.py
--rw-rw-rw-   0        0        0    13888 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfGuidPpiProtocolSectionParser.py
--rw-rw-rw-   0        0        0     7663 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfLibrarySectionParser.py
--rw-rw-rw-   0        0        0     4878 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfPackageSectionParser.py
--rw-rw-rw-   0        0        0    27810 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfParser.py
--rw-rw-rw-   0        0        0     6832 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfParserMisc.py
--rw-rw-rw-   0        0        0     7372 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfPcdSectionParser.py
--rw-rw-rw-   0        0        0    20744 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfSectionParser.py
--rw-rw-rw-   0        0        0     5199 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfSourceSectionParser.py
--rw-rw-rw-   0        0        0      310 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Parser/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.104473 edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/
--rw-rw-rw-   0        0        0    44504 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/DecPomAlignment.py
--rw-rw-rw-   0        0        0    49064 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/InfPomAlignment.py
--rw-rw-rw-   0        0        0    11167 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/InfPomAlignmentMisc.py
--rw-rw-rw-   0        0        0      314 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/__init__.py
--rw-rw-rw-   0        0        0     5256 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/ReplacePkg.py
--rw-rw-rw-   0        0        0     9213 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/RmPkg.py
--rw-rw-rw-   0        0        0     3003 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/TestInstall.py
--rw-rw-rw-   0        0        0    14916 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UPT.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.109473 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/
--rw-rw-rw-   0        0        0    39744 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/CommentGeneratingUnitTest.py
--rw-rw-rw-   0        0        0    28032 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/CommentParsingUnitTest.py
--rw-rw-rw-   0        0        0     9975 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/DecParserTest.py
--rw-rw-rw-   0        0        0    18679 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/DecParserUnitTest.py
--rw-rw-rw-   0        0        0     9190 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/InfBinarySectionTest.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.118473 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/
--rw-rw-rw-   0        0        0    44407 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/CommonXml.py
--rw-rw-rw-   0        0        0    11487 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/GuidProtocolPpiXml.py
--rw-rw-rw-   0        0        0    16905 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/IniToXml.py
--rw-rw-rw-   0        0        0    38313 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/ModuleSurfaceAreaXml.py
--rw-rw-rw-   0        0        0    15284 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/PackageSurfaceAreaXml.py
--rw-rw-rw-   0        0        0    23075 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/PcdXml.py
--rw-rw-rw-   0        0        0    38789 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/XmlParser.py
--rw-rw-rw-   0        0        0     2789 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/XmlParserMisc.py
--rw-rw-rw-   0        0        0      308 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/UPT/Xml/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.128472 edk2-basetools-0.1.8/edk2basetools/Workspace/
--rw-rw-rw-   0        0        0    32278 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/BuildClassObject.py
--rw-rw-rw-   0        0        0    21356 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/DecBuildData.py
--rw-rw-rw-   0        0        0   208677 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/DscBuildData.py
--rw-rw-rw-   0        0        0    47800 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/InfBuildData.py
--rw-rw-rw-   0        0        0     8741 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/MetaDataTable.py
--rw-rw-rw-   0        0        0     2117 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileCommentParser.py
--rw-rw-rw-   0        0        0   108696 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileParser.py
--rw-rw-rw-   0        0        0    16472 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileTable.py
--rw-rw-rw-   0        0        0    11498 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/WorkspaceCommon.py
--rw-rw-rw-   0        0        0     7085 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/WorkspaceDatabase.py
--rw-rw-rw-   0        0        0      290 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/Workspace/__init__.py
--rw-rw-rw-   0        0        0      319 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/__init__.py
--rw-rw-rw-   0        0        0      228 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/basetool_tiano_python_path_env.yaml
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.132470 edk2-basetools-0.1.8/edk2basetools/build/
--rw-rw-rw-   0        0        0   112502 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/build/BuildReport.py
--rw-rw-rw-   0        0        0      286 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/build/__init__.py
--rw-rw-rw-   0        0        0   133451 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/build/build.py
--rw-rw-rw-   0        0        0     9200 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/build/buildoptions.py
--rw-rw-rw-   0        0        0      364 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/sitecustomize.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:31.798474 edk2-basetools-0.1.8/edk2basetools/tests/
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.133472 edk2-basetools-0.1.8/edk2basetools/tests/Split/
--rw-rw-rw-   0        0        0     3932 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/tests/Split/test_split.py
-drwxrwxrwx   0        0        0        0 2022-01-22 09:07:32.134472 edk2-basetools-0.1.8/edk2basetools/tests/UPT/
--rw-rw-rw-   0        0        0    18731 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/edk2basetools/tests/UPT/test_decparser.py
--rw-rw-rw-   0        0        0     2778 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/license.txt
--rw-rw-rw-   0        0        0       42 2022-01-22 09:07:32.136473 edk2-basetools-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     3342 2022-01-22 09:04:58.000000 edk2-basetools-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.683410 edk2-basetools-0.1.9/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.453380 edk2-basetools-0.1.9/.azurepipelines/
+-rw-rw-rw-   0        0        0      459 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/azure-pipelines-release.yml
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.457387 edk2-basetools-0.1.9/.azurepipelines/templates/
+-rw-rw-rw-   0        0        0      520 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/basic-setup-steps.yml
+-rw-rw-rw-   0        0        0      968 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/build-publish-whl-steps.yml
+-rw-rw-rw-   0        0        0     1308 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/build-test-job.yml
+-rw-rw-rw-   0        0        0      660 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/flake8-test-steps.yml
+-rw-rw-rw-   0        0        0      438 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/markdown-lint-steps.yml
+-rw-rw-rw-   0        0        0     1692 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/pytest-test-steps.yml
+-rw-rw-rw-   0        0        0      486 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/templates/spell-test-steps.yml
+-rw-rw-rw-   0        0        0      423 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/ubuntu-test-pr-ci.yml
+-rw-rw-rw-   0        0        0      421 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.azurepipelines/windows-test-pr-ci.yml
+-rw-rw-rw-   0        0        0     1599 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/.cspell.json
+-rw-rw-rw-   0        0        0     2489 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/BasicDevTests.py
+-rw-rw-rw-   0        0        0     1429 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/ConfirmVersionAndTag.py
+-rw-rw-rw-   0        0        0      102 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     4716 2022-01-22 09:38:58.683410 edk2-basetools-0.1.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.458387 edk2-basetools-0.1.9/docs/
+-rw-rw-rw-   0        0        0     1797 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/docs/coverage.md
+-rw-rw-rw-   0        0        0     1691 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/docs/publishing.md
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.462391 edk2-basetools-0.1.9/edk2_basetools.egg-info/
+-rw-rw-rw-   0        0        0     4716 2022-01-22 09:38:57.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    12702 2022-01-22 09:38:58.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-22 09:38:57.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      105 2022-01-22 09:38:57.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2022-01-22 09:38:57.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2022-01-22 09:38:57.000000 edk2-basetools-0.1.9/edk2_basetools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.464388 edk2-basetools-0.1.9/edk2basetools/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.464388 edk2-basetools-0.1.9/edk2basetools/AmlToC/
+-rw-rw-rw-   0        0        0     4677 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AmlToC/AmlToC.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.489382 edk2-basetools-0.1.9/edk2basetools/AutoGen/
+-rw-rw-rw-   0        0        0     4646 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/AutoGen.py
+-rw-rw-rw-   0        0        0    15154 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/AutoGenWorker.py
+-rw-rw-rw-   0        0        0    26598 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/BuildEngine.py
+-rw-rw-rw-   0        0        0     7181 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/DataPipe.py
+-rw-rw-rw-   0        0        0    94675 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/GenC.py
+-rw-rw-rw-   0        0        0    21188 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/GenDepex.py
+-rw-rw-rw-   0        0        0    78532 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/GenMake.py
+-rw-rw-rw-   0        0        0    72646 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/GenPcdDb.py
+-rw-rw-rw-   0        0        0    16258 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/GenVar.py
+-rw-rw-rw-   0        0        0     5749 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/IdfClassObject.py
+-rw-rw-rw-   0        0        0    14610 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/IncludesAutoGen.py
+-rw-rw-rw-   0        0        0     4624 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/InfSectionParser.py
+-rw-rw-rw-   0        0        0   109789 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/ModuleAutoGen.py
+-rw-rw-rw-   0        0        0    30806 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/ModuleAutoGenHelper.py
+-rw-rw-rw-   0        0        0    83657 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/PlatformAutoGen.py
+-rw-rw-rw-   0        0        0    22439 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/StrGather.py
+-rw-rw-rw-   0        0        0    29657 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/UniClassObject.py
+-rw-rw-rw-   0        0        0    10205 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/ValidCheckingInfoObject.py
+-rw-rw-rw-   0        0        0    46637 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/WorkspaceAutoGen.py
+-rw-rw-rw-   0        0        0      313 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/AutoGen/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.491409 edk2-basetools-0.1.9/edk2basetools/BPDG/
+-rw-rw-rw-   0        0        0     6086 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/BPDG/BPDG.py
+-rw-rw-rw-   0        0        0    33024 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/BPDG/GenVpd.py
+-rw-rw-rw-   0        0        0     3174 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/BPDG/StringTable.py
+-rw-rw-rw-   0        0        0      278 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/BPDG/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.494408 edk2-basetools-0.1.9/edk2basetools/Capsule/
+-rw-rw-rw-   0        0        0    58579 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Capsule/GenerateCapsule.py
+-rw-rw-rw-   0        0        0     5892 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Capsule/GenerateWindowsDriver.py
+-rw-rw-rw-   0        0        0     2660 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Capsule/WindowsCapsuleSupportHelper.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.508634 edk2-basetools-0.1.9/edk2basetools/Common/
+-rw-rw-rw-   0        0        0     5253 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/BuildToolError.py
+-rw-rw-rw-   0        0        0      266 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/BuildVersion.py
+-rw-rw-rw-   0        0        0    23720 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/DataType.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.513417 edk2-basetools-0.1.9/edk2basetools/Common/Edk2/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.514423 edk2-basetools-0.1.9/edk2basetools/Common/Edk2/Capsule/
+-rw-rw-rw-   0        0        0     3450 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Edk2/Capsule/FmpPayloadHeader.py
+-rw-rw-rw-   0        0        0      293 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Edk2/Capsule/__init__.py
+-rw-rw-rw-   0        0        0      285 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Edk2/__init__.py
+-rw-rw-rw-   0        0        0    12973 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/EdkLogger.py
+-rw-rw-rw-   0        0        0    44557 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Expression.py
+-rw-rw-rw-   0        0        0     3620 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/GlobalData.py
+-rw-rw-rw-   0        0        0     1888 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathOs.py
+-rw-rw-rw-   0        0        0     1239 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathOsPath.py
+-rw-rw-rw-   0        0        0     1344 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathSupport.py
+-rw-rw-rw-   0        0        0    73267 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Misc.py
+-rw-rw-rw-   0        0        0     5104 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/MultipleWorkspace.py
+-rw-rw-rw-   0        0        0    39051 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Parsing.py
+-rw-rw-rw-   0        0        0    25319 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/RangeExpression.py
+-rw-rw-rw-   0        0        0    29531 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/StringUtils.py
+-rw-rw-rw-   0        0        0     9068 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/TargetTxtClassObject.py
+-rw-rw-rw-   0        0        0    12974 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/ToolDefClassObject.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.515400 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.520397 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/
+-rw-rw-rw-   0        0        0    17261 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/CapsuleDependency.py
+-rw-rw-rw-   0        0        0     7883 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/FmpAuthHeader.py
+-rw-rw-rw-   0        0        0    14854 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/FmpCapsuleHeader.py
+-rw-rw-rw-   0        0        0     5521 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/UefiCapsuleHeader.py
+-rw-rw-rw-   0        0        0      293 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/__init__.py
+-rw-rw-rw-   0        0        0      285 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/Uefi/__init__.py
+-rw-rw-rw-   0        0        0     1961 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/VariableAttributes.py
+-rw-rw-rw-   0        0        0    11682 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/VpdInfoFile.py
+-rw-rw-rw-   0        0        0      287 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/__init__.py
+-rw-rw-rw-   0        0        0     1320 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Common/caching.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.512405 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/
+-rw-rw-rw-   0        0        0     3862 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/CommonClass.py
+-rw-rw-rw-   0        0        0    16528 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/DataClass.py
+-rw-rw-rw-   0        0        0      530 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/Exceptions.py
+-rw-rw-rw-   0        0        0     7612 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/FdfClass.py
+-rw-rw-rw-   0        0        0      296 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/CommonDataClass/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.532413 edk2-basetools-0.1.9/edk2basetools/Ecc/
+-rw-rw-rw-   0        0        0    17207 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/C.g
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.534412 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/
+-rw-rw-rw-   0        0        0    98792 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/CLexer.py
+-rw-rw-rw-   0        0        0   698147 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/CParser.py
+-rw-rw-rw-   0        0        0        0 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.538416 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/
+-rw-rw-rw-   0        0        0    15914 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/C.g4
+-rw-rw-rw-   0        0        0    38792 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CLexer.py
+-rw-rw-rw-   0        0        0    26606 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CListener.py
+-rw-rw-rw-   0        0        0   257504 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CParser.py
+-rw-rw-rw-   0        0        0        0 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/__init__.py
+-rw-rw-rw-   0        0        0   102733 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Check.py
+-rw-rw-rw-   0        0        0     4891 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CodeFragment.py
+-rw-rw-rw-   0        0        0    25592 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/CodeFragmentCollector.py
+-rw-rw-rw-   0        0        0    23197 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Configuration.py
+-rw-rw-rw-   0        0        0    14082 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Database.py
+-rw-rw-rw-   0        0        0      432 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/EccGlobalData.py
+-rw-rw-rw-   0        0        0    19353 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/EccMain.py
+-rw-rw-rw-   0        0        0    14452 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/EccToolError.py
+-rw-rw-rw-   0        0        0     2713 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Exception.py
+-rw-rw-rw-   0        0        0     1332 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/FileProfile.py
+-rw-rw-rw-   0        0        0    10766 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaDataParser.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.541417 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/
+-rw-rw-rw-   0        0        0     6200 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaDataTable.py
+-rw-rw-rw-   0        0        0   100873 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaFileParser.py
+-rw-rw-rw-   0        0        0    13080 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaFileTable.py
+-rw-rw-rw-   0        0        0      290 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/__init__.py
+-rw-rw-rw-   0        0        0      782 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/ParserWarning.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.542428 edk2-basetools-0.1.9/edk2basetools/Ecc/Xml/
+-rw-rw-rw-   0        0        0     7254 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Xml/XmlRoutines.py
+-rw-rw-rw-   0        0        0      308 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/Xml/__init__.py
+-rw-rw-rw-   0        0        0      284 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/__init__.py
+-rw-rw-rw-   0        0        0   113709 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/c.py
+-rw-rw-rw-   0        0        0    11328 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/config.ini
+-rw-rw-rw-   0        0        0     7951 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Ecc/exception.xml
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.558392 edk2-basetools-0.1.9/edk2basetools/Eot/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.561391 edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/
+-rw-rw-rw-   0        0        0    98792 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/CLexer.py
+-rw-rw-rw-   0        0        0   698115 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/CParser.py
+-rw-rw-rw-   0        0        0        0 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.563387 edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/
+-rw-rw-rw-   0        0        0    38794 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CLexer.py
+-rw-rw-rw-   0        0        0    26604 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CListener.py
+-rw-rw-rw-   0        0        0   257504 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CParser.py
+-rw-rw-rw-   0        0        0        0 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/__init__.py
+-rw-rw-rw-   0        0        0     5503 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CodeFragment.py
+-rw-rw-rw-   0        0        0    16753 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/CodeFragmentCollector.py
+-rw-rw-rw-   0        0        0     9735 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/Database.py
+-rw-rw-rw-   0        0        0    11283 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/EfiCompressor.pyd
+-rw-rw-rw-   0        0        0     3720 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/EotGlobalData.py
+-rw-rw-rw-   0        0        0    69058 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/EotMain.py
+-rw-rw-rw-   0        0        0      292 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/EotToolError.py
+-rw-rw-rw-   0        0        0     1378 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/FileProfile.py
+-rw-rw-rw-   0        0        0     1365 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/Identification.py
+-rw-rw-rw-   0        0        0     5750 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/InfParserLite.py
+-rw-rw-rw-   0        0        0    14875 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/LzmaCompressor.pyd
+-rw-rw-rw-   0        0        0    34281 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/Parser.py
+-rw-rw-rw-   0        0        0      620 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/ParserWarning.py
+-rw-rw-rw-   0        0        0    17383 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/Report.py
+-rw-rw-rw-   0        0        0      277 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/__init__.py
+-rw-rw-rw-   0        0        0    14082 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Eot/c.py
+-rw-rw-rw-   0        0        0      245 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GNUmakefile
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.581391 edk2-basetools-0.1.9/edk2basetools/GenFds/
+-rw-rw-rw-   0        0        0     4971 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/AprioriSection.py
+-rw-rw-rw-   0        0        0    10484 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Capsule.py
+-rw-rw-rw-   0        0        0     7184 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/CapsuleData.py
+-rw-rw-rw-   0        0        0     3607 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/CompressSection.py
+-rw-rw-rw-   0        0        0     5184 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/DataSection.py
+-rw-rw-rw-   0        0        0     5205 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/DepexSection.py
+-rw-rw-rw-   0        0        0    15655 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/EfiSection.py
+-rw-rw-rw-   0        0        0     7130 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Fd.py
+-rw-rw-rw-   0        0        0   194986 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/FdfParser.py
+-rw-rw-rw-   0        0        0     1960 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Ffs.py
+-rw-rw-rw-   0        0        0     7916 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/FfsFileStatement.py
+-rw-rw-rw-   0        0        0    54740 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/FfsInfStatement.py
+-rw-rw-rw-   0        0        0    20222 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Fv.py
+-rw-rw-rw-   0        0        0     7357 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/FvImageSection.py
+-rw-rw-rw-   0        0        0    42610 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/GenFds.py
+-rw-rw-rw-   0        0        0    45566 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/GenFdsGlobalVariable.py
+-rw-rw-rw-   0        0        0    12718 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/GuidSection.py
+-rw-rw-rw-   0        0        0     1127 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/OptRomFileStatement.py
+-rw-rw-rw-   0        0        0     5611 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/OptRomInfStatement.py
+-rw-rw-rw-   0        0        0     5624 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/OptionRom.py
+-rw-rw-rw-   0        0        0    15900 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Region.py
+-rw-rw-rw-   0        0        0      474 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Rule.py
+-rw-rw-rw-   0        0        0      584 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/RuleComplexFile.py
+-rw-rw-rw-   0        0        0      579 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/RuleSimpleFile.py
+-rw-rw-rw-   0        0        0     6680 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/Section.py
+-rw-rw-rw-   0        0        0     2757 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/UiSection.py
+-rw-rw-rw-   0        0        0     2973 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/VerSection.py
+-rw-rw-rw-   0        0        0      287 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenFds/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.582393 edk2-basetools-0.1.9/edk2basetools/GenPatchPcdTable/
+-rw-rw-rw-   0        0        0     9435 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenPatchPcdTable/GenPatchPcdTable.py
+-rw-rw-rw-   0        0        0      290 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/GenPatchPcdTable/__init__.py
+-rw-rw-rw-   0        0        0      266 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Makefile
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.583392 edk2-basetools-0.1.9/edk2basetools/PatchPcdValue/
+-rw-rw-rw-   0        0        0    10510 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/PatchPcdValue/PatchPcdValue.py
+-rw-rw-rw-   0        0        0      287 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/PatchPcdValue/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.593402 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/
+-rw-rw-rw-   0        0        0    11244 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/Pkcs7Sign.py
+-rw-rw-rw-   0        0        0     6631 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/Readme.md
+-rw-rw-rw-   0        0        0     3659 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestCert.pem
+-rw-rw-rw-   0        0        0     1530 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestCert.pub.pem
+-rw-rw-rw-   0        0        0     1008 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer
+-rw-rw-rw-   0        0        0     6099 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer.gEfiSecurityPkgTokenSpaceGuid.PcdPkcs7CertBuffer.inc
+-rw-rw-rw-   0        0        0     6133 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer.gFmpDevicePkgTokenSpaceGuid.PcdFmpDevicePkcs7CertBufferXdr.inc
+-rw-rw-rw-   0        0        0     3578 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.pem
+-rw-rw-rw-   0        0        0     1442 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.pub.pem
+-rw-rw-rw-   0        0        0     3285 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestSub.pem
+-rw-rw-rw-   0        0        0     1414 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestSub.pub.pem
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.599391 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/
+-rw-rw-rw-   0        0        0     6532 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256GenerateKeys.py
+-rw-rw-rw-   0        0        0     9193 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256Sign.py
+-rw-rw-rw-   0        0        0     1706 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/TestSigningPrivateKey.pem
+-rw-rw-rw-   0        0        0       32 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/TestSigningPublicKey.bin
+-rw-rw-rw-   0        0        0      194 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/TestSigningPublicKey.txt
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.600403 edk2-basetools-0.1.9/edk2basetools/Split/
+-rw-rw-rw-   0        0        0     7189 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Split/Split.py
+-rw-rw-rw-   0        0        0      215 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Split/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.606390 edk2-basetools-0.1.9/edk2basetools/Table/
+-rw-rw-rw-   0        0        0     2919 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/Table.py
+-rw-rw-rw-   0        0        0     3076 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableDataModel.py
+-rw-rw-rw-   0        0        0     4635 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableDec.py
+-rw-rw-rw-   0        0        0     4619 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableDsc.py
+-rw-rw-rw-   0        0        0     3226 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableEotReport.py
+-rw-rw-rw-   0        0        0     4749 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableFdf.py
+-rw-rw-rw-   0        0        0     3743 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableFile.py
+-rw-rw-rw-   0        0        0     4614 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableFunction.py
+-rw-rw-rw-   0        0        0     4032 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableIdentifier.py
+-rw-rw-rw-   0        0        0     5043 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableInf.py
+-rw-rw-rw-   0        0        0     3980 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TablePcd.py
+-rw-rw-rw-   0        0        0     2197 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableQuery.py
+-rw-rw-rw-   0        0        0     5644 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/TableReport.py
+-rw-rw-rw-   0        0        0      286 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Table/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.607392 edk2-basetools-0.1.9/edk2basetools/TargetTool/
+-rw-rw-rw-   0        0        0    13876 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/TargetTool/TargetTool.py
+-rw-rw-rw-   0        0        0      291 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/TargetTool/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.608405 edk2-basetools-0.1.9/edk2basetools/Trim/
+-rw-rw-rw-   0        0        0    26557 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Trim/Trim.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.612399 edk2-basetools-0.1.9/edk2basetools/UPT/
+-rw-rw-rw-   0        0        0      305 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/BuildVersion.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.615385 edk2-basetools-0.1.9/edk2basetools/UPT/Core/
+-rw-rw-rw-   0        0        0    17446 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/DependencyRules.py
+-rw-rw-rw-   0        0        0    11375 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/DistributionPackageClass.py
+-rw-rw-rw-   0        0        0     6486 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/FileHook.py
+-rw-rw-rw-   0        0        0    33706 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/IpiDb.py
+-rw-rw-rw-   0        0        0     8764 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/PackageFile.py
+-rw-rw-rw-   0        0        0      319 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Core/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.619402 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/
+-rw-rw-rw-   0        0        0    27305 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenDecFile.py
+-rw-rw-rw-   0        0        0    46494 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenInfFile.py
+-rw-rw-rw-   0        0        0     7386 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenMetaFileMisc.py
+-rw-rw-rw-   0        0        0      240 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenXmlFile.py
+-rw-rw-rw-   0        0        0      316 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/__init__.py
+-rw-rw-rw-   0        0        0    37920 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/InstallPkg.py
+-rw-rw-rw-   0        0        0     3789 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/InventoryWs.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.625393 edk2-basetools-0.1.9/edk2basetools/UPT/Library/
+-rw-rw-rw-   0        0        0     9411 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/CommentGenerating.py
+-rw-rw-rw-   0        0        0    22525 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/CommentParsing.py
+-rw-rw-rw-   0        0        0    33789 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/DataType.py
+-rw-rw-rw-   0        0        0    18091 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/ExpressionValidate.py
+-rw-rw-rw-   0        0        0     1806 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/GlobalData.py
+-rw-rw-rw-   0        0        0    31580 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/Misc.py
+-rw-rw-rw-   0        0        0    19900 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/ParserValidate.py
+-rw-rw-rw-   0        0        0    39944 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/Parsing.py
+-rw-rw-rw-   0        0        0    31352 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/StringUtils.py
+-rw-rw-rw-   0        0        0    50047 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/UniClassObject.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.626384 edk2-basetools-0.1.9/edk2basetools/UPT/Library/Xml/
+-rw-rw-rw-   0        0        0     6937 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/Xml/XmlRoutines.py
+-rw-rw-rw-   0        0        0      308 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/Xml/__init__.py
+-rw-rw-rw-   0        0        0      312 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Library/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.631398 edk2-basetools-0.1.9/edk2basetools/UPT/Logger/
+-rw-rw-rw-   0        0        0     8875 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Logger/Log.py
+-rw-rw-rw-   0        0        0    46178 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Logger/StringTable.py
+-rw-rw-rw-   0        0        0     5795 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Logger/ToolError.py
+-rw-rw-rw-   0        0        0      310 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Logger/__init__.py
+-rw-rw-rw-   0        0        0    10209 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/MkPkg.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.631398 edk2-basetools-0.1.9/edk2basetools/UPT/Object/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.639393 edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/
+-rw-rw-rw-   0        0        0    25908 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/CommonObject.py
+-rw-rw-rw-   0        0        0    16270 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/ModuleObject.py
+-rw-rw-rw-   0        0        0     5106 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/PackageObject.py
+-rw-rw-rw-   0        0        0      307 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.650393 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/
+-rw-rw-rw-   0        0        0    15031 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/DecObject.py
+-rw-rw-rw-   0        0        0    33097 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfBinaryObject.py
+-rw-rw-rw-   0        0        0     2820 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfBuildOptionObject.py
+-rw-rw-rw-   0        0        0     3340 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfCommonObject.py
+-rw-rw-rw-   0        0        0     2327 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDefineCommonObject.py
+-rw-rw-rw-   0        0        0    41374 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDefineObject.py
+-rw-rw-rw-   0        0        0     5147 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDepexObject.py
+-rw-rw-rw-   0        0        0    13345 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfGuidObject.py
+-rw-rw-rw-   0        0        0     2462 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfHeaderObject.py
+-rw-rw-rw-   0        0        0    10541 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfLibraryClassesObject.py
+-rw-rw-rw-   0        0        0     3924 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfMisc.py
+-rw-rw-rw-   0        0        0     7352 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPackagesObject.py
+-rw-rw-rw-   0        0        0    26617 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPcdObject.py
+-rw-rw-rw-   0        0        0    12506 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPpiObject.py
+-rw-rw-rw-   0        0        0    11092 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfProtocolObject.py
+-rw-rw-rw-   0        0        0     8493 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfSoucesObject.py
+-rw-rw-rw-   0        0        0     4826 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfUserExtensionObject.py
+-rw-rw-rw-   0        0        0      310 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/__init__.py
+-rw-rw-rw-   0        0        0      310 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Object/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.659386 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/
+-rw-rw-rw-   0        0        0    45165 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/DecParser.py
+-rw-rw-rw-   0        0        0    10933 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/DecParserMisc.py
+-rw-rw-rw-   0        0        0     9276 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfAsBuiltProcess.py
+-rw-rw-rw-   0        0        0     8869 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfBinarySectionParser.py
+-rw-rw-rw-   0        0        0     8472 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfBuildOptionSectionParser.py
+-rw-rw-rw-   0        0        0     6837 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfDefineSectionParser.py
+-rw-rw-rw-   0        0        0     3506 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfDepexSectionParser.py
+-rw-rw-rw-   0        0        0    13888 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfGuidPpiProtocolSectionParser.py
+-rw-rw-rw-   0        0        0     7663 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfLibrarySectionParser.py
+-rw-rw-rw-   0        0        0     4878 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfPackageSectionParser.py
+-rw-rw-rw-   0        0        0    27810 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfParser.py
+-rw-rw-rw-   0        0        0     6832 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfParserMisc.py
+-rw-rw-rw-   0        0        0     7372 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfPcdSectionParser.py
+-rw-rw-rw-   0        0        0    20744 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfSectionParser.py
+-rw-rw-rw-   0        0        0     5199 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfSourceSectionParser.py
+-rw-rw-rw-   0        0        0      310 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Parser/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.662405 edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/
+-rw-rw-rw-   0        0        0    44504 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/DecPomAlignment.py
+-rw-rw-rw-   0        0        0    49064 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/InfPomAlignment.py
+-rw-rw-rw-   0        0        0    11167 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/InfPomAlignmentMisc.py
+-rw-rw-rw-   0        0        0      314 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/__init__.py
+-rw-rw-rw-   0        0        0     5256 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/ReplacePkg.py
+-rw-rw-rw-   0        0        0     9213 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/RmPkg.py
+-rw-rw-rw-   0        0        0     3003 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/TestInstall.py
+-rw-rw-rw-   0        0        0    14916 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UPT.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.665388 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/
+-rw-rw-rw-   0        0        0    39744 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/CommentGeneratingUnitTest.py
+-rw-rw-rw-   0        0        0    28032 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/CommentParsingUnitTest.py
+-rw-rw-rw-   0        0        0     9975 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/DecParserTest.py
+-rw-rw-rw-   0        0        0    18679 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/DecParserUnitTest.py
+-rw-rw-rw-   0        0        0     9190 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/InfBinarySectionTest.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.671386 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/
+-rw-rw-rw-   0        0        0    44407 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/CommonXml.py
+-rw-rw-rw-   0        0        0    11487 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/GuidProtocolPpiXml.py
+-rw-rw-rw-   0        0        0    16905 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/IniToXml.py
+-rw-rw-rw-   0        0        0    38313 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/ModuleSurfaceAreaXml.py
+-rw-rw-rw-   0        0        0    15284 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/PackageSurfaceAreaXml.py
+-rw-rw-rw-   0        0        0    23075 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/PcdXml.py
+-rw-rw-rw-   0        0        0    38789 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/XmlParser.py
+-rw-rw-rw-   0        0        0     2789 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/XmlParserMisc.py
+-rw-rw-rw-   0        0        0      308 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/UPT/Xml/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.678403 edk2-basetools-0.1.9/edk2basetools/Workspace/
+-rw-rw-rw-   0        0        0    32176 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/BuildClassObject.py
+-rw-rw-rw-   0        0        0    21356 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/DecBuildData.py
+-rw-rw-rw-   0        0        0   208677 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/DscBuildData.py
+-rw-rw-rw-   0        0        0    47800 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/InfBuildData.py
+-rw-rw-rw-   0        0        0     8741 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/MetaDataTable.py
+-rw-rw-rw-   0        0        0     2117 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileCommentParser.py
+-rw-rw-rw-   0        0        0   108696 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileParser.py
+-rw-rw-rw-   0        0        0    16472 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileTable.py
+-rw-rw-rw-   0        0        0    11498 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/WorkspaceCommon.py
+-rw-rw-rw-   0        0        0     7085 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/WorkspaceDatabase.py
+-rw-rw-rw-   0        0        0      290 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/Workspace/__init__.py
+-rw-rw-rw-   0        0        0      319 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/__init__.py
+-rw-rw-rw-   0        0        0      228 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/basetool_tiano_python_path_env.yaml
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.681405 edk2-basetools-0.1.9/edk2basetools/build/
+-rw-rw-rw-   0        0        0   112502 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/build/BuildReport.py
+-rw-rw-rw-   0        0        0      286 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/build/__init__.py
+-rw-rw-rw-   0        0        0   133363 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/build/build.py
+-rw-rw-rw-   0        0        0     9200 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/build/buildoptions.py
+-rw-rw-rw-   0        0        0      364 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/sitecustomize.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.445459 edk2-basetools-0.1.9/edk2basetools/tests/
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.681405 edk2-basetools-0.1.9/edk2basetools/tests/Split/
+-rw-rw-rw-   0        0        0     3932 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/tests/Split/test_split.py
+drwxrwxrwx   0        0        0        0 2022-01-22 09:38:58.682402 edk2-basetools-0.1.9/edk2basetools/tests/UPT/
+-rw-rw-rw-   0        0        0    18731 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/edk2basetools/tests/UPT/test_decparser.py
+-rw-rw-rw-   0        0        0     2778 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/license.txt
+-rw-rw-rw-   0        0        0       42 2022-01-22 09:38:58.683410 edk2-basetools-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     3342 2022-01-22 09:37:03.000000 edk2-basetools-0.1.9/setup.py
```

### Comparing `edk2-basetools-0.1.8/.azurepipelines/templates/basic-setup-steps.yml` & `edk2-basetools-0.1.9/.azurepipelines/templates/basic-setup-steps.yml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/.azurepipelines/templates/build-publish-whl-steps.yml` & `edk2-basetools-0.1.9/.azurepipelines/templates/build-publish-whl-steps.yml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/.azurepipelines/templates/build-test-job.yml` & `edk2-basetools-0.1.9/.azurepipelines/templates/build-test-job.yml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/.azurepipelines/templates/flake8-test-steps.yml` & `edk2-basetools-0.1.9/.azurepipelines/templates/flake8-test-steps.yml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/.azurepipelines/templates/pytest-test-steps.yml` & `edk2-basetools-0.1.9/.azurepipelines/templates/pytest-test-steps.yml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/.cspell.json` & `edk2-basetools-0.1.9/.cspell.json`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/BasicDevTests.py` & `edk2-basetools-0.1.9/BasicDevTests.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/ConfirmVersionAndTag.py` & `edk2-basetools-0.1.9/ConfirmVersionAndTag.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/PKG-INFO` & `edk2-basetools-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edk2-basetools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python BaseTools supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-basetools
 Author: Tianocore Edk2-BaseTool team
 Author-email: edk2-bugs@lists.01.org
 License: BSD-2-Clause-Patent
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edk2-basetools-0.1.8/docs/coverage.md` & `edk2-basetools-0.1.9/docs/coverage.md`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/docs/publishing.md` & `edk2-basetools-0.1.9/docs/publishing.md`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2_basetools.egg-info/PKG-INFO` & `edk2-basetools-0.1.9/edk2_basetools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edk2-basetools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python BaseTools supporting UEFI EDK2 firmware development
 Home-page: https://github.com/tianocore/edk2-basetools
 Author: Tianocore Edk2-BaseTool team
 Author-email: edk2-bugs@lists.01.org
 License: BSD-2-Clause-Patent
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `edk2-basetools-0.1.8/edk2_basetools.egg-info/SOURCES.txt` & `edk2-basetools-0.1.9/edk2_basetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AmlToC/AmlToC.py` & `edk2-basetools-0.1.9/edk2basetools/AmlToC/AmlToC.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/AutoGen.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/AutoGen.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/AutoGenWorker.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/AutoGenWorker.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/BuildEngine.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/BuildEngine.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/DataPipe.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/DataPipe.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/GenC.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/GenC.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/GenDepex.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/GenDepex.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/GenMake.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/GenMake.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/GenPcdDb.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/GenPcdDb.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/GenVar.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/GenVar.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/IdfClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/IdfClassObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/IncludesAutoGen.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/IncludesAutoGen.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/InfSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/InfSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/ModuleAutoGen.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/ModuleAutoGen.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,14 @@
         self._IntroBuildTargetList    = None
         self._FinalBuildTargetList    = None
         self._FileTypes               = None
 
         self.AutoGenDepSet = set()
         self.ReferenceModules = []
         self.ConstPcd                  = {}
-        self.Makefile         = None
         self.FileDependCache  = {}
 
     def __init_platform_info__(self):
         pinfo = self.DataPipe.Get("P_Info")
         self.WorkspaceDir = pinfo.get("WorkspaceDir")
         self.PlatformInfo = PlatformInfo(self.Workspace,pinfo.get("ActivePlatform"),pinfo.get("Target"),pinfo.get("ToolChain"),pinfo.get("Arch"),self.DataPipe)
     ## hash() operator of ModuleAutoGen
```

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/ModuleAutoGenHelper.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/ModuleAutoGenHelper.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/PlatformAutoGen.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/PlatformAutoGen.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/StrGather.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/StrGather.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/UniClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/UniClassObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/ValidCheckingInfoObject.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/ValidCheckingInfoObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/AutoGen/WorkspaceAutoGen.py` & `edk2-basetools-0.1.9/edk2basetools/AutoGen/WorkspaceAutoGen.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/BPDG/BPDG.py` & `edk2-basetools-0.1.9/edk2basetools/BPDG/BPDG.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/BPDG/GenVpd.py` & `edk2-basetools-0.1.9/edk2basetools/BPDG/GenVpd.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/BPDG/StringTable.py` & `edk2-basetools-0.1.9/edk2basetools/BPDG/StringTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Capsule/GenerateCapsule.py` & `edk2-basetools-0.1.9/edk2basetools/Capsule/GenerateCapsule.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Capsule/GenerateWindowsDriver.py` & `edk2-basetools-0.1.9/edk2basetools/Capsule/GenerateWindowsDriver.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Capsule/WindowsCapsuleSupportHelper.py` & `edk2-basetools-0.1.9/edk2basetools/Capsule/WindowsCapsuleSupportHelper.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/BuildToolError.py` & `edk2-basetools-0.1.9/edk2basetools/Common/BuildToolError.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/DataType.py` & `edk2-basetools-0.1.9/edk2basetools/Common/DataType.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Edk2/Capsule/FmpPayloadHeader.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Edk2/Capsule/FmpPayloadHeader.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/EdkLogger.py` & `edk2-basetools-0.1.9/edk2basetools/Common/EdkLogger.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Expression.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Expression.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/GlobalData.py` & `edk2-basetools-0.1.9/edk2basetools/Common/GlobalData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathOs.py` & `edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathOs.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathOsPath.py` & `edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathOsPath.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/LongFilePathSupport.py` & `edk2-basetools-0.1.9/edk2basetools/Common/LongFilePathSupport.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Misc.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Misc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/MultipleWorkspace.py` & `edk2-basetools-0.1.9/edk2basetools/Common/MultipleWorkspace.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Parsing.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Parsing.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/RangeExpression.py` & `edk2-basetools-0.1.9/edk2basetools/Common/RangeExpression.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/StringUtils.py` & `edk2-basetools-0.1.9/edk2basetools/Common/StringUtils.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/TargetTxtClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/Common/TargetTxtClassObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/ToolDefClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/Common/ToolDefClassObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/CapsuleDependency.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/CapsuleDependency.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/FmpAuthHeader.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/FmpAuthHeader.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/FmpCapsuleHeader.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/FmpCapsuleHeader.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/Uefi/Capsule/UefiCapsuleHeader.py` & `edk2-basetools-0.1.9/edk2basetools/Common/Uefi/Capsule/UefiCapsuleHeader.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/VariableAttributes.py` & `edk2-basetools-0.1.9/edk2basetools/Common/VariableAttributes.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/VpdInfoFile.py` & `edk2-basetools-0.1.9/edk2basetools/Common/VpdInfoFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Common/caching.py` & `edk2-basetools-0.1.9/edk2basetools/Common/caching.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/CommonDataClass/CommonClass.py` & `edk2-basetools-0.1.9/edk2basetools/CommonDataClass/CommonClass.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/CommonDataClass/DataClass.py` & `edk2-basetools-0.1.9/edk2basetools/CommonDataClass/DataClass.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/CommonDataClass/Exceptions.py` & `edk2-basetools-0.1.9/edk2basetools/CommonDataClass/Exceptions.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/CommonDataClass/FdfClass.py` & `edk2-basetools-0.1.9/edk2basetools/CommonDataClass/FdfClass.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/C.g` & `edk2-basetools-0.1.9/edk2basetools/Ecc/C.g`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/CLexer.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/CLexer.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser3/CParser.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser3/CParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/C.g4` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/C.g4`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CLexer.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CLexer.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CListener.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CListener.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CParser4/CParser.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CParser4/CParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/Check.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/Check.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CodeFragment.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CodeFragment.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/CodeFragmentCollector.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/CodeFragmentCollector.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/Configuration.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/Configuration.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/Database.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/Database.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/EccMain.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/EccMain.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/EccToolError.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/EccToolError.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/Exception.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/Exception.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/FileProfile.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/FileProfile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/MetaDataParser.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/MetaDataParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaDataTable.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaDataTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaFileParser.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaFileParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/MetaFileWorkspace/MetaFileTable.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/MetaFileWorkspace/MetaFileTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/ParserWarning.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/ParserWarning.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/Xml/XmlRoutines.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/Xml/XmlRoutines.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/c.py` & `edk2-basetools-0.1.9/edk2basetools/Ecc/c.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/config.ini` & `edk2-basetools-0.1.9/edk2basetools/Ecc/config.ini`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Ecc/exception.xml` & `edk2-basetools-0.1.9/edk2basetools/Ecc/exception.xml`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/CLexer.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/CLexer.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CParser3/CParser.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CParser3/CParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CLexer.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CLexer.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CListener.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CListener.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CParser4/CParser.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CParser4/CParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CodeFragment.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CodeFragment.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/CodeFragmentCollector.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/CodeFragmentCollector.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/Database.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/Database.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/EotGlobalData.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/EotGlobalData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/EotMain.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/EotMain.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/FileProfile.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/FileProfile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/Identification.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/Identification.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/InfParserLite.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/InfParserLite.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/Parser.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/Parser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/ParserWarning.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/ParserWarning.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/Report.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/Report.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Eot/c.py` & `edk2-basetools-0.1.9/edk2basetools/Eot/c.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/AprioriSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/AprioriSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Capsule.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Capsule.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/CapsuleData.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/CapsuleData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/CompressSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/CompressSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/DataSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/DataSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/DepexSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/DepexSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/EfiSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/EfiSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Fd.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Fd.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/FdfParser.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/FdfParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Ffs.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Ffs.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/FfsFileStatement.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/FfsFileStatement.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/FfsInfStatement.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/FfsInfStatement.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Fv.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Fv.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/FvImageSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/FvImageSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/GenFds.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/GenFds.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/GenFdsGlobalVariable.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/GenFdsGlobalVariable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/GuidSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/GuidSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/OptRomFileStatement.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/OptRomFileStatement.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/OptRomInfStatement.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/OptRomInfStatement.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/OptionRom.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/OptionRom.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Region.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Region.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/RuleComplexFile.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/RuleComplexFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/RuleSimpleFile.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/RuleSimpleFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/Section.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/Section.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/UiSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/UiSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenFds/VerSection.py` & `edk2-basetools-0.1.9/edk2basetools/GenFds/VerSection.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/GenPatchPcdTable/GenPatchPcdTable.py` & `edk2-basetools-0.1.9/edk2basetools/GenPatchPcdTable/GenPatchPcdTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/PatchPcdValue/PatchPcdValue.py` & `edk2-basetools-0.1.9/edk2basetools/PatchPcdValue/PatchPcdValue.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/Pkcs7Sign.py` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/Pkcs7Sign.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/Readme.md` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/Readme.md`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestCert.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestCert.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestCert.pub.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestCert.pub.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer.gEfiSecurityPkgTokenSpaceGuid.PcdPkcs7CertBuffer.inc` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer.gEfiSecurityPkgTokenSpaceGuid.PcdPkcs7CertBuffer.inc`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.cer.gFmpDevicePkgTokenSpaceGuid.PcdFmpDevicePkcs7CertBufferXdr.inc` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.cer.gFmpDevicePkgTokenSpaceGuid.PcdFmpDevicePkcs7CertBufferXdr.inc`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestRoot.pub.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestRoot.pub.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestSub.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestSub.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Pkcs7Sign/TestSub.pub.pem` & `edk2-basetools-0.1.9/edk2basetools/Pkcs7Sign/TestSub.pub.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256GenerateKeys.py` & `edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256GenerateKeys.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256Sign.py` & `edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/Rsa2048Sha256Sign.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Rsa2048Sha256Sign/TestSigningPrivateKey.pem` & `edk2-basetools-0.1.9/edk2basetools/Rsa2048Sha256Sign/TestSigningPrivateKey.pem`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Split/Split.py` & `edk2-basetools-0.1.9/edk2basetools/Split/Split.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/Table.py` & `edk2-basetools-0.1.9/edk2basetools/Table/Table.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableDataModel.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableDataModel.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableDec.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableDec.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableDsc.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableDsc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableEotReport.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableEotReport.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableFdf.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableFdf.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableFile.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableFunction.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableFunction.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableIdentifier.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableIdentifier.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableInf.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableInf.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TablePcd.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TablePcd.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableQuery.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableQuery.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Table/TableReport.py` & `edk2-basetools-0.1.9/edk2basetools/Table/TableReport.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/TargetTool/TargetTool.py` & `edk2-basetools-0.1.9/edk2basetools/TargetTool/TargetTool.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Trim/Trim.py` & `edk2-basetools-0.1.9/edk2basetools/Trim/Trim.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Core/DependencyRules.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Core/DependencyRules.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Core/DistributionPackageClass.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Core/DistributionPackageClass.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Core/FileHook.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Core/FileHook.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Core/IpiDb.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Core/IpiDb.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Core/PackageFile.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Core/PackageFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenDecFile.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenDecFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenInfFile.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenInfFile.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/GenMetaFile/GenMetaFileMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/GenMetaFile/GenMetaFileMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/InstallPkg.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/InstallPkg.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/InventoryWs.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/InventoryWs.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/CommentGenerating.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/CommentGenerating.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/CommentParsing.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/CommentParsing.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/DataType.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/DataType.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/ExpressionValidate.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/ExpressionValidate.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/GlobalData.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/GlobalData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/Misc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/Misc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/ParserValidate.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/ParserValidate.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/Parsing.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/Parsing.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/StringUtils.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/StringUtils.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/UniClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/UniClassObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Library/Xml/XmlRoutines.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Library/Xml/XmlRoutines.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Logger/Log.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Logger/Log.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Logger/StringTable.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Logger/StringTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Logger/ToolError.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Logger/ToolError.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/MkPkg.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/MkPkg.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/CommonObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/CommonObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/ModuleObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/ModuleObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/POM/PackageObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/POM/PackageObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/DecObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/DecObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfBinaryObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfBinaryObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfBuildOptionObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfBuildOptionObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfCommonObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfCommonObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDefineCommonObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDefineCommonObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDefineObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDefineObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfDepexObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfDepexObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfGuidObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfGuidObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfHeaderObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfHeaderObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfLibraryClassesObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfLibraryClassesObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPackagesObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPackagesObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPcdObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPcdObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfPpiObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfPpiObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfProtocolObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfProtocolObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfSoucesObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfSoucesObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Object/Parser/InfUserExtensionObject.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Object/Parser/InfUserExtensionObject.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/DecParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/DecParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/DecParserMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/DecParserMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfAsBuiltProcess.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfAsBuiltProcess.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfBinarySectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfBinarySectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfBuildOptionSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfBuildOptionSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfDefineSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfDefineSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfDepexSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfDepexSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfGuidPpiProtocolSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfGuidPpiProtocolSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfLibrarySectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfLibrarySectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfPackageSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfPackageSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfParserMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfParserMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfPcdSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfPcdSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Parser/InfSourceSectionParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Parser/InfSourceSectionParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/DecPomAlignment.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/DecPomAlignment.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/InfPomAlignment.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/InfPomAlignment.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/PomAdapter/InfPomAlignmentMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/PomAdapter/InfPomAlignmentMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/ReplacePkg.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/ReplacePkg.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/RmPkg.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/RmPkg.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/TestInstall.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/TestInstall.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UPT.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UPT.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/CommentGeneratingUnitTest.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/CommentGeneratingUnitTest.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/CommentParsingUnitTest.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/CommentParsingUnitTest.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/DecParserTest.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/DecParserTest.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/DecParserUnitTest.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/DecParserUnitTest.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/UnitTest/InfBinarySectionTest.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/UnitTest/InfBinarySectionTest.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/CommonXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/CommonXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/GuidProtocolPpiXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/GuidProtocolPpiXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/IniToXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/IniToXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/ModuleSurfaceAreaXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/ModuleSurfaceAreaXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/PackageSurfaceAreaXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/PackageSurfaceAreaXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/PcdXml.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/PcdXml.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/XmlParser.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/XmlParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/UPT/Xml/XmlParserMisc.py` & `edk2-basetools-0.1.9/edk2basetools/UPT/Xml/XmlParserMisc.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/BuildClassObject.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/BuildClassObject.py`

 * *Files 0% similar despite different names*

```diff
@@ -586,15 +586,14 @@
 # @var PlatformName:      To store value for PlatformName
 # @var Guid:              To store value for Guid
 # @var Version:           To store value for Version
 # @var DscSpecification:  To store value for DscSpecification
 # @var OutputDirectory:   To store value for OutputDirectory
 # @var FlashDefinition:   To store value for FlashDefinition
 # @var BuildNumber:       To store value for BuildNumber
-# @var MakefileName:      To store value for MakefileName
 # @var SkuIds:            To store value for SkuIds, it is a set structure as
 #                         { 'SkuName' : SkuId, '!include' : includefilename, ...}
 # @var Modules:           To store value for Modules, it is a list structure as
 #                         [ InfFileName, ... ]
 # @var Libraries:         To store value for Libraries, it is a list structure as
 #                         [ InfFileName, ... ]
 # @var LibraryClasses:    To store value for LibraryClasses, it is a set structure as
@@ -610,15 +609,14 @@
         self.PlatformName            = ''
         self.Guid                    = ''
         self.Version                 = ''
         self.DscSpecification        = ''
         self.OutputDirectory         = ''
         self.FlashDefinition         = ''
         self.BuildNumber             = ''
-        self.MakefileName            = ''
 
         self.SkuIds                  = {}
         self.Modules                 = []
         self.LibraryInstances        = []
         self.LibraryClasses          = {}
         self.Libraries               = {}
         self.Pcds                    = {}
```

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/DecBuildData.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/DecBuildData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/DscBuildData.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/DscBuildData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/InfBuildData.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/InfBuildData.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/MetaDataTable.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/MetaDataTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileCommentParser.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileCommentParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileParser.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileParser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/MetaFileTable.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/MetaFileTable.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/WorkspaceCommon.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/WorkspaceCommon.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/Workspace/WorkspaceDatabase.py` & `edk2-basetools-0.1.9/edk2basetools/Workspace/WorkspaceDatabase.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/build/BuildReport.py` & `edk2-basetools-0.1.9/edk2basetools/build/BuildReport.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/build/build.py` & `edk2-basetools-0.1.9/edk2basetools/build/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -2182,16 +2182,14 @@
                     ModuleList.append(Inf)
             Pa.DataPipe.DataContainer = {"FfsCommand":CmdListDict}
             Pa.DataPipe.DataContainer = {"Workspace_timestamp": Wa._SrcTimeStamp}
             Pa.DataPipe.DataContainer = {"CommandTarget": self.Target}
             Pa.CreateLibModuelDirs()
             # Fetch the MakeFileName.
             self.MakeFileName = Pa.MakeFileName
-            if not self.MakeFileName:
-                self.MakeFileName = Pa.MakeFile
 
             Pa.DataPipe.DataContainer = {"LibraryBuildDirectoryList":Pa.LibraryBuildDirectoryList}
             Pa.DataPipe.DataContainer = {"ModuleBuildDirectoryList":Pa.ModuleBuildDirectoryList}
             Pa.DataPipe.DataContainer = {"FdsCommandDict": Wa.GenFdsCommandDict}
             # Prepare the cache share data for multiprocessing
             Pa.DataPipe.DataContainer = {"gPlatformHashFile":GlobalData.gPlatformHashFile}
             ModuleCodaFile = {}
```

### Comparing `edk2-basetools-0.1.8/edk2basetools/build/buildoptions.py` & `edk2-basetools-0.1.9/edk2basetools/build/buildoptions.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/tests/Split/test_split.py` & `edk2-basetools-0.1.9/edk2basetools/tests/Split/test_split.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/edk2basetools/tests/UPT/test_decparser.py` & `edk2-basetools-0.1.9/edk2basetools/tests/UPT/test_decparser.py`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/license.txt` & `edk2-basetools-0.1.9/license.txt`

 * *Files identical despite different names*

### Comparing `edk2-basetools-0.1.8/setup.py` & `edk2-basetools-0.1.9/setup.py`

 * *Files identical despite different names*

