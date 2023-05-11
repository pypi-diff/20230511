# Comparing `tmp/steam-sdk-2023.4.3.tar.gz` & `tmp/steam-sdk-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.4.3.tar", last modified: Mon Apr 24 13:26:58 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.5.0.tar", last modified: Thu May 11 15:26:41 2023, max compression
```

## Comparing `steam-sdk-2023.4.3.tar` & `steam-sdk-2023.5.0.tar`

### file list

```diff
@@ -1,207 +1,211 @@
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.552091 steam-sdk-2023.4.3/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.4.3/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.4.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-04-24 13:26:58.551093 steam-sdk-2023.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.4.3/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/mkdocs.yaml
--rw-rw-rw-   0        0        0     1686 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-24 13:26:58.552091 steam-sdk-2023.4.3/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-04-24 13:24:31.000000 steam-sdk-2023.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.368581 steam-sdk-2023.4.3/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.378588 steam-sdk-2023.4.3/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   103257 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.378588 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.380554 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.387530 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.389526 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.393514 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.395509 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.399498 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.401494 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.418448 steam-sdk-2023.4.3/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   160973 2023-01-17 16:22:36.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    32791 2023-04-13 17:03:42.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    33654 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.4.3/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.419445 steam-sdk-2023.4.3/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.421440 steam-sdk-2023.4.3/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.424432 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.427424 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.429418 steam-sdk-2023.4.3/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.432413 steam-sdk-2023.4.3/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.460336 steam-sdk-2023.4.3/steam_sdk/data/
--rw-rw-rw-   0        0        0    10087 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8004 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.4.3/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     3169 2023-01-20 13:20:13.000000 steam-sdk-2023.4.3/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35441 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2620 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.4.3/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.4.3/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.472317 steam-sdk-2023.4.3/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     7741 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.474298 steam-sdk-2023.4.3/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.503222 steam-sdk-2023.4.3/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10602 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.504219 steam-sdk-2023.4.3/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.4.3/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.511200 steam-sdk-2023.4.3/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    54678 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    59090 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    59958 2023-04-03 16:34:32.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.4.3/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.512197 steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2204 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.517184 steam-sdk-2023.4.3/steam_sdk/plotters/
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2022-12-02 17:12:04.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0    17127 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/plotters/PlotterSIGMA.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.519178 steam-sdk-2023.4.3/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.540123 steam-sdk-2023.4.3/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.4.3/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0    11647 2023-04-24 13:20:15.000000 steam-sdk-2023.4.3/steam_sdk/utils/builder_SIGMA_helpers.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.4.3/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     6908 2023-04-20 15:50:04.000000 steam-sdk-2023.4.3/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.544112 steam-sdk-2023.4.3/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.4.3/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.546107 steam-sdk-2023.4.3/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.547103 steam-sdk-2023.4.3/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.549099 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.550096 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.4.3/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-04-24 13:26:58.374566 steam-sdk-2023.4.3/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7314 2023-04-24 13:26:57.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1597 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-24 13:26:30.000000 steam-sdk-2023.4.3/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.680715 steam-sdk-2023.5.0/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.5.0/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.5.0/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-05-11 15:26:41.679718 steam-sdk-2023.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.5.0/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.5.0/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1685 2023-05-11 15:14:30.000000 steam-sdk-2023.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 15:26:41.680715 steam-sdk-2023.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-05-11 15:21:42.000000 steam-sdk-2023.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.496401 steam-sdk-2023.5.0/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.504144 steam-sdk-2023.5.0/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   119712 2023-05-11 15:13:46.000000 steam-sdk-2023.5.0/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.505311 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.506312 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.516285 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.518279 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.522282 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.524264 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.528252 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.530247 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.541241 steam-sdk-2023.5.0/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162619 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    34260 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.5.0/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.5.0/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.542239 steam-sdk-2023.5.0/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.544233 steam-sdk-2023.5.0/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.548224 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.551216 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.553210 steam-sdk-2023.5.0/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.555205 steam-sdk-2023.5.0/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.582135 steam-sdk-2023.5.0/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10171 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8040 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.5.0/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.5.0/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35546 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.5.0/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.5.0/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.5.0/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.5.0/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.5.0/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.5.0/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.591868 steam-sdk-2023.5.0/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     2832 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.5.0/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.595858 steam-sdk-2023.5.0/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.620875 steam-sdk-2023.5.0/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-11 15:23:35.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.5.0/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.621872 steam-sdk-2023.5.0/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.5.0/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.628854 steam-sdk-2023.5.0/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61593 2023-05-11 11:02:01.000000 steam-sdk-2023.5.0/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    70148 2023-05-11 15:13:46.000000 steam-sdk-2023.5.0/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    47683 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.5.0/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.630848 steam-sdk-2023.5.0/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2329 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.638827 steam-sdk-2023.5.0/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8053 2023-05-11 15:13:46.000000 steam-sdk-2023.5.0/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20399 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2023-05-11 15:23:13.000000 steam-sdk-2023.5.0/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.640823 steam-sdk-2023.5.0/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.665755 steam-sdk-2023.5.0/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.5.0/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.5.0/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.5.0/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.5.0/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.5.0/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 10:23:04.000000 steam-sdk-2023.5.0/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.669745 steam-sdk-2023.5.0/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.5.0/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.671748 steam-sdk-2023.5.0/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.673737 steam-sdk-2023.5.0/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.674732 steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.676727 steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.5.0/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 15:26:41.502149 steam-sdk-2023.5.0/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-05-11 15:26:12.000000 steam-sdk-2023.5.0/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7480 2023-05-11 15:26:40.000000 steam-sdk-2023.5.0/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 15:26:12.000000 steam-sdk-2023.5.0/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-05-11 15:26:12.000000 steam-sdk-2023.5.0/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 15:26:12.000000 steam-sdk-2023.5.0/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.4.3/.gitignore` & `steam-sdk-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/.gitlab-ci.yml` & `steam-sdk-2023.5.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/PKG-INFO` & `steam-sdk-2023.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.4.3
+Version: 2023.5.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: API,SDK,CERN,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.4.3/Readme.md` & `steam-sdk-2023.5.0/Readme.md`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/mkdocs.yaml` & `steam-sdk-2023.5.0/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/requirements.txt` & `steam-sdk-2023.5.0/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.4.15
+steam-pysigma==2023.5.6
```

### Comparing `steam-sdk-2023.4.3/setup.py` & `steam-sdk-2023.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.4.3",
+    version="2023.5.0",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,40 +3,44 @@
 import os
 import pathlib
 import shutil
 import importlib
 import importlib.util
 import pandas as pd
 import pickle
+import csv
+import re
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
+from steam_sdk.plotters.PlotterMap2d import export_B_field_txt_to_map2d_SIGMA
 from steam_sdk.data.DataSettings import DataSettings
 from steam_sdk.builders.BuilderModel import BuilderModel
 from steam_sdk.data.DataAnalysis import DataAnalysis, ModifyModel, ModifyModelMultipleVariables, ParametricSweep, LoadCircuitParameters, WriteStimulusFile
 from steam_sdk.drivers.DriverFiQuS import DriverFiQuS
 from steam_sdk.drivers.DriverLEDET import DriverLEDET
 from steam_sdk.drivers.DriverPSPICE import DriverPSPICE
 from steam_sdk.drivers.DriverPyBBQ import DriverPyBBQ
-from steam_sdk.drivers.DriverSIGMA import DriverSIGMA
+from steam_sdk.drivers.DriverSIGMA import DriverSIGMA_new
 from steam_sdk.drivers.DriverXYCE import DriverXYCE
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.parsims.ParsimConductor import ParsimConductor
 from steam_sdk.parsims.ParsimEventCircuit import ParsimEventCircuit
 from steam_sdk.parsims.ParsimEventMagnet import ParsimEventMagnet
 from steam_sdk.utils import parse_str_to_list
 from steam_sdk.postprocs.PostprocsMetrics import PostprocsMetrics
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
 from steam_sdk.utils.rgetattr import rgetattr
 from steam_sdk.utils.sgetattr import rsetattr
 from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.viewers.Viewer import Viewer
 from steam_sdk.parsers.ParserPSPICE import writeStimuliFromInterpolation
+from steam_sdk.plotters.PlotterMap2d import generate_report_from_map2d
 
 
 class AnalysisSTEAM:
     """
         Class to run analysis based on STEAM_SDK
     """
 
@@ -422,16 +426,16 @@
                     flag_yaml = True  # Hard-coded for the moment
                     BM.buildLEDET()
                     self.setup_sim_LEDET(simulation_name=step.simulation_name, sim_number=simulation_number,
                                          flag_yaml=flag_yaml, flag_json=flag_json)
                 if 'SIGMA' in step.software:
                     for sim_num in step.simulation_numbers:
                         make_folder_if_not_existing(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}") )#ADDED
-                        BM.buildSIGMA(output_path=os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}"))
-                    #self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=simulation_number)
+                        BM.buildSIGMA(f"{step.simulation_name}_{sim_num}")
+                    self.setup_sim_SIGMA(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PyBBQ' in step.software:
                     BM.buildPyBBQ()
                     self.setup_sim_PyBBQ(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'PSPICE' in step.software:
                     BM.buildPSPICE()
                     self.setup_sim_PSPICE(simulation_name=step.simulation_name, sim_number=simulation_number)
                 if 'XYCE' in step.software:
@@ -544,16 +548,34 @@
             if verbose:
                 print('Running simulation of model {} #{} using {}.'.format(simulation_name, sim_number, software))
             # Run simulation
             self.run_sim(software, sim_name, sim_number, simFileType, verbose)
 
     def step_postprocess(self, step, verbose: bool = False):
         if verbose: print('postprocessing')
-        print('Not implemented yet.')
-        pass
+        if step.software and 'SIGMA' in step.software:
+            for sim_num in step.simulation_numbers:
+                # Check if files exist
+                path_result_txt_Bx = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'mf.Bx.txt')
+                path_result_txt_By = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'mf.By.txt')
+                path_new_file = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", 'B_field_map2d.map2d')
+                path_reference_roxie = os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}", f"{step.simulation_name}_ROXIE_REFERENCE.map2d")
+
+                if not os.path.exists(path_result_txt_Bx):
+                    raise Warning("No Bx file is found, please check that simulation ran successfully.")
+                elif not os.path.exists(path_result_txt_By):
+                    raise Warning("No By file is found, please check that simulation ran successfully.")
+                elif not os.path.exists(path_reference_roxie):
+                    raise Warning("No Roxie reference file is found, please check model_data.yaml in options_sigma that key map2d is specified.")
+                else:
+                    export_B_field_txt_to_map2d_SIGMA(path_reference_roxie, path_result_txt_Bx, path_result_txt_By,
+                                                path_new_file)
+                    generate_report_from_map2d(os.path.join(self.settings.local_SIGMA_folder, f"{step.simulation_name}_{sim_num}"), path_reference_roxie, "Roxie Data", path_new_file, "SIGMA DATA", "coil", save=True)
+        else:
+            print('Not implemented yet.')
 
     def step_setup_folder(self, step, verbose: bool = False):
         """
         Set up simulation working folder.
         The function applies a different logic for each simulation software.
         """
         list_software = step.software
@@ -588,28 +610,28 @@
                 # Copy csv files from the output folder
                 list_csv_files = [entry for entry in os.listdir(self.output_path) if
                                   (simulation_name in entry) and ('.csv' in entry)]
                 for csv_file in list_csv_files:
                     file_to_copy = os.path.join(self.output_path, csv_file)
                     file_copied = os.path.join(Path(local_LEDET_folder / simulation_name / 'Input').resolve(), csv_file)
                     shutil.copyfile(file_to_copy, file_copied)
-                    if verbose: print('Csv file {} copied to {}.'.format(file_to_copy, file_copied))
+                    if verbose: print(f'Csv file {file_to_copy} copied to {file_copied}.')
 
                 # Make magnet field-map folder
                 field_maps_folder = Path(local_LEDET_folder / '..' / 'Field maps' / simulation_name).resolve()
                 make_folder_if_not_existing(field_maps_folder, verbose=verbose)
 
                 # Copy field-map files from the output folder
                 list_field_maps = [entry for entry in os.listdir(self.output_path) if
                                    (simulation_name in entry) and ('.map2d' in entry)]
                 for field_map in list_field_maps:
                     file_to_copy = os.path.join(self.output_path, field_map)
                     file_copied = os.path.join(field_maps_folder, field_map)
                     shutil.copyfile(file_to_copy, file_copied)
-                    if verbose: ('Field map file {} copied to {}.'.format(file_to_copy, file_copied))
+                    if verbose: print(f'Field map file {file_to_copy} copied to {file_copied}.')
 
             elif 'PSPICE' in software:
                 local_PSPICE_folder = Path(self.settings.local_PSPICE_folder)
                 local_model_folder = Path(local_PSPICE_folder / simulation_name).resolve()
                 # Make magnet input folder
                 make_folder_if_not_existing(local_model_folder, verbose=verbose)
 
@@ -1255,19 +1277,19 @@
             dPSPICE.run_PSPICE(simulation_name, suffix='')
         elif software == 'XYCE':
             local_model_folder = Path(
                 Path(self.settings.local_XYCE_folder) / simulation_name / str(sim_number)).resolve()
             dXYCE = DriverXYCE(path_exe=self.settings.XYCE_path, path_folder_XYCE=local_model_folder, verbose=verbose)
             dXYCE.run_XYCE(simulation_name, suffix='')
         elif software == 'SIGMA':
-            simulation_name_temp = simulation_name + f"_{str(sim_number)}"
-            local_model_folder = Path(
-                Path(self.settings.local_SIGMA_folder) / simulation_name_temp).resolve()
-            ds = DriverSIGMA(simulation_name, path_folder_SIGMA=local_model_folder)
-            ds.run_SIGMA()
+            local_analysis_folder = simulation_name + '_' + str(sim_number)
+            ds = DriverSIGMA_new(path_folder_SIGMA=self.settings.local_SIGMA_folder,
+                                 path_folder_SIGMA_input=os.path.join(self.settings.local_SIGMA_folder,
+                                                                      local_analysis_folder), local_analysis_folder=local_analysis_folder, system_settings=self.settings, verbose=verbose)
+            ds.run_SIGMA(simulation_name)
         else:
             raise Exception(f'Software {software} not supported for automated running.')
 
 
     def write_stimuli_from_interpolation(self, step, verbose: bool = False):
         '''
         Function to write a resistance stimuli for n apertures of a magnet for any current level. Resistance will be interpolated
@@ -1371,52 +1393,145 @@
             # TODO: parse Conductor Data - but what are the names in Quenchdict? (Parsim Sweep can handly conductor changes)
 
             # Write a .csv file that can be used to run a STEAM Viewer analysis
             for current_software, current_path_viewer_csv in zip(software, path_output_viewer_csv):
                 pem.set_up_viewer(current_path_viewer_csv, default_keys, simulation_numbers, simulation_name, current_software)
                 if verbose: print(f'File {current_path_viewer_csv} written. It can be used to run a STEAM Viewer analysis.')
         elif case_model == 'circuit':
+            # Read input file and run the ParsimEvent analysis
             pec = ParsimEventCircuit(ref_model=self.list_models[model_name], verbose=verbose)
             pec.read_from_input(path_input_file=input_file, flag_append=False)
             pec.write_event_file(simulation_name=simulation_name, simulation_numbers=simulation_numbers,
                                  path_outputfile_event_csv=path_output_event_csv)
-            for event_number in range(len(pec.list_events)):
+
+            quenching_magnet_list = []  # required for families where multiple magnets can quench like RB
+
+            for event_number in range(len(pec.list_events)):  # reading through each row of the event file
+                # get circuit specific information
                 circuit_name = pec.list_events[event_number].GeneralParameters.name
                 circuit_family_name = self.__get_circuit_family_name(circuit_name)
                 magnet_name = self.__get_magnet_name(circuit_name)
                 circuit_type = self.__get_circuit_type(circuit_name)
                 number_of_magnets = self.__get_number_of_magnets(circuit_name)
                 number_of_apertures = self.__get_number_of_apertures(circuit_name)
                 current_level = pec.list_events[event_number].PoweredCircuits[circuit_name].current_at_discharge
                 magnets_list = self.__get_magnets_list(number_of_magnets)
                 t_PC_off = pec.list_events[event_number].PoweredCircuits[circuit_name].delta_t_FGC_PIC
                 magnet_types = self.__get_magnet_types_list(number_of_magnets)
+
+                # load circuit parameters step
                 if circuit_family_name == "RQ":
                     circuit_name_1 = circuit_name.replace(".", "D_")
                     circuit_name_2 = circuit_name.replace(".", "F_")
-                    load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
+                    position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
+                    quenching_magnet = [self.__get_quenching_magnet_number(position, circuit_family_name)]
+                    # modify model diode step used to change diodes across the quenching magnets with heating
+                    modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RQ_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
+                elif circuit_type == "RCBX":
+                    circuit_name_1 = circuit_name.replace("X", "XH")
+                    circuit_name_2 = circuit_name.replace("X", "XV")
+                    load_circuit_parameters_step_1 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_1)
+                    load_circuit_parameters_step_2 = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name_2)
                 else:
                     load_circuit_parameters_step = LoadCircuitParameters(type='LoadCircuitParameters', model_name=model_name, path_file_circuit_parameters=os.path.join(f"../../tests/builders/model_library/circuits/circuit_parameters/{circuit_family_name}_circuit_parameters.csv"), selected_circuit_name=circuit_name)
+
+                # choosing stimulus output file location
                 if circuit_family_name == "IPD":
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_family_name}', f'{event_number + 1}', 'coil_resistances.stl')
+                elif circuit_family_name == "RQ":
+                    stimulus_output_file_1 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets', f'{event_number + 1}', 'coil_resistances.stl')
+                    stimulus_output_file_2 = os.path.join(default_keys.path_output, f'{circuit_type}_47magnets',f'{event_number + 2}', 'coil_resistances.stl')
+                elif circuit_type == "RCBX":
+                    stimulus_output_file_1 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 1}', 'coil_resistances.stl')
+                    stimulus_output_file_2 = os.path.join(default_keys.path_output, 'RCBX', f'{event_number + 2}', 'coil_resistances.stl')
+                elif simulation_name.startswith("IPQ"):
+                    stimulus_output_file = os.path.join(default_keys.path_output, f'{simulation_name}', f'{event_number + 1}', 'coil_resistances.stl')
+                elif circuit_name.startswith("RCBY"):
+                    stimulus_output_file = os.path.join(default_keys.path_output, 'RCBY', f'{event_number + 1}', 'coil_resistances.stl')
                 else:
                     stimulus_output_file = os.path.join(default_keys.path_output, f'{circuit_type}', f'{event_number + 1}', 'coil_resistances.stl')
+
+                # making appropriate directory if it doesn't exist for the stimulus output file
+                if circuit_family_name == "RQ" or circuit_type == "RCBX":
+                    for file_path in [stimulus_output_file_1, stimulus_output_file_2]:
+                        directory = os.path.dirname(file_path)
+                        if not os.path.exists(directory):
+                            os.makedirs(directory)
+                else:
+                    directory = os.path.dirname(stimulus_output_file)
+                    if not os.path.exists(directory):
+                        os.makedirs(directory)
+
+                # write stimulus file step
                 if circuit_family_name == "RQ":
-                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=quenching_magnet, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type == "RCBX":
+                    write_stimuli_file_step_1 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_1, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off[0]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                    write_stimuli_file_step_2 = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file_2, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off[1]], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 elif circuit_family_name == "RQX":
                     current_level = [current_level[0]+current_level[1], current_level[0]+current_level[2], current_level[0]+current_level[2], current_level[0]]
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_family_name == "IPQ" and number_of_magnets == 2:
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=current_level, magnets=magnets_list, t_offset=[t_PC_off]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_family_name == "IPQ" and number_of_magnets == 1:
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level[0]], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type in ["RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"]:
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[0]}.csv'), os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name[1]}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level]*number_of_magnets, magnets=magnets_list, t_offset=[t_PC_off[0]]*number_of_magnets, interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
+                elif circuit_type == "RB":
+                    position = pec.list_events[event_number].QuenchEvents[circuit_name].magnet_electrical_position
+                    quenching_magnet = [self.__get_quenching_magnet_number(position, circuit_family_name)]
+                    quenching_magnet_list.append(quenching_magnet[0])
+                    quenching_magnet_list.sort()
+                    # modify model diode step used to change diodes across the quenching magnets with heating
+                    modify_model_diode_step = ModifyModel(type='ModifyModel', model_name=model_name, variable_to_change=f'Netlist.x_D{quenching_magnet[0]}.value', variable_value=["RB_Protection_Diode"], simulation_numbers=[], simulation_name=simulation_name, software=software)
+                    write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file=stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level]*(event_number + 1), magnets=quenching_magnet_list, t_offset=[t_PC_off]*(event_number + 1), interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
                 else:
                     write_stimuli_file_step = WriteStimulusFile(type='WriteStimulusFile', output_file= stimulus_output_file, path_interpolation_file=[os.path.join(f'../../tests/builders/model_library/circuits/coil_resistances_to_interpolate/interpolation_resistance_{magnet_name}.csv')], n_total_magnets=number_of_magnets, n_apertures=number_of_apertures, current_level=[current_level], magnets=magnets_list, t_offset=[t_PC_off], interpolation_type='Linear', type_file_writing='w', n_sampling=1, magnet_types=magnet_types)
-                # start parsim sweep step with newly created event file
-                parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
-                                                    model_name=model_name, case_model=case_model, software=software, verbose=verbose)
-                self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
-                self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
-                self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
+
+                # parsim sweep step with newly created event file
+                if circuit_family_name == "RQ" or circuit_type == "RCBX":
+                    output_files = self.__split_csv(path_output_event_csv)
+                    parsim_sweep_step_1 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[0],
+                                                        model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+                    parsim_sweep_step_2 = ParametricSweep(type='ParametricSweep', input_sweep_file=output_files[1],
+                                                        model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+                else:
+                    parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_event_csv,
+                                                        model_name=model_name, case_model=case_model, software=software, verbose=verbose)
+
+                # run all the steps together
+                if circuit_family_name == "RQ":
+                    self.load_circuit_parameters(load_circuit_parameters_step_1, verbose=verbose)
+                    self.write_stimuli_from_interpolation(write_stimuli_file_step_1, verbose=verbose)
+                    self.step_modify_model(modify_model_diode_step, verbose=verbose)
+                    self.run_parsim_sweep(parsim_sweep_step_1, verbose=verbose)
+                    self.load_circuit_parameters(load_circuit_parameters_step_2, verbose=verbose)
+                    self.write_stimuli_from_interpolation(write_stimuli_file_step_2, verbose=verbose)
+                    self.step_modify_model(modify_model_diode_step, verbose=verbose)
+                    self.run_parsim_sweep(parsim_sweep_step_2, verbose=verbose)
+                elif circuit_type == "RCBX":
+                    self.load_circuit_parameters(load_circuit_parameters_step_1, verbose=verbose)
+                    self.write_stimuli_from_interpolation(write_stimuli_file_step_1, verbose=verbose)
+                    self.run_parsim_sweep(parsim_sweep_step_1, verbose=verbose)
+                    self.load_circuit_parameters(load_circuit_parameters_step_2, verbose=verbose)
+                    self.write_stimuli_from_interpolation(write_stimuli_file_step_2, verbose=verbose)
+                    self.run_parsim_sweep(parsim_sweep_step_2, verbose=verbose)
+                elif circuit_type == "RB":
+                    self.step_modify_model(modify_model_diode_step, verbose=verbose)  # diode is changed for each row of the event file
+                    if event_number == len(pec.list_events)-1:  # the simulation runs correctly only at the end
+                        self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
+                        self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
+                        self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
+                else:
+                    self.load_circuit_parameters(load_circuit_parameters_step, verbose=verbose)
+                    self.write_stimuli_from_interpolation(write_stimuli_file_step, verbose=verbose)
+                    self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
 
             # Write a .csv file that can be used to run a STEAM Viewer analysis #TODO consider adding set_up_viewer() method
             # for current_software, current_path_viewer_csv in zip(software, path_output_viewer_csv):
             #     pec.set_up_viewer(current_path_viewer_csv, default_keys, simulation_numbers, simulation_name, current_software)
             #     if verbose: print(f'File {current_path_viewer_csv} written. It can be used to run a STEAM Viewer analysis.')
         else:
             raise Exception(f'case_model {case_model} not supported by ParsimEvent.')
@@ -1432,15 +1547,16 @@
         :param verbose: if true displays more information
         '''
         # Unpack inputs
         model_name = step.model_name
         case_model = step.case_model
         software = step.software
         groups_to_coils = step.groups_to_coils
-        groups_to_coil_length = step.groups_to_coil_length
+        length_to_coil = step.length_to_coil
+        if not length_to_coil: length_to_coil = {}  # optimize coillen
         simulation_number = step.simulation_number
         input_file = step.input_file
         path_output_sweeper_csv = step.path_output_sweeper_csv
         strand_critical_current_measurements = step.strand_critical_current_measurements
 
         # check if crucial variables are not None
         if not path_output_sweeper_csv:
@@ -1450,18 +1566,14 @@
 
         # check if all groups are defined in the group dictionaries
         highest_group_index = max([max(values) for values in groups_to_coils.values()])
         expected_group_numbers = list(range(1, highest_group_index + 1))
         all_group_numbers_in_dict = [num for sublist in groups_to_coils.values() for num in sublist]
         if sorted(all_group_numbers_in_dict) != expected_group_numbers:
             raise Exception(f'Invalid groups_to_coils entry in step definition. \nSorted groups given by the user: {sorted(all_group_numbers_in_dict)}')
-        all_group_numbers_in_dict = [num for sublist in groups_to_coil_length.values() for num in sublist]
-        if sorted(all_group_numbers_in_dict) != expected_group_numbers:
-            raise Exception(f'Invalid groups_to_coil_length entry in step definition. \nSorted groups given by the user: {sorted(all_group_numbers_in_dict)}')
-
 
         # make a copy of the respective conductor for every coil and store it in the magnet model
         # NOTE: if a coil consists of 2 different conductors the user has to treat them as 2 different coils (so a coil is not always a coil but rather a subcoil with the same conductor)
         new_conductors = [None] * len(groups_to_coils)
         dict_coilname_to_conductorindex = {}
         new_conductor_to_group = [None] * len(self.list_models[model_name].model_data.CoilWindings.conductor_to_group)
         for idx, (coil_name, group_numbers) in enumerate(groups_to_coils.items()):
@@ -1496,35 +1608,36 @@
         del new_conductors, new_conductor_to_group
 
 
         if case_model == 'magnet':
             # create instance of ParsimConductor
             pc = ParsimConductor(verbose=verbose, model_data=self.list_models[model_name].model_data,
                                  dict_coilName_to_conductorIndex=dict_coilname_to_conductorindex,
-                                 groups_to_coils=groups_to_coils, groups_to_coil_length=groups_to_coil_length)
+                                 groups_to_coils=groups_to_coils, length_to_coil=length_to_coil,
+                                 path_input_dir=Path(self.list_models[step.model_name].file_model_data).parent)
             # read the conductor database
-            pc.read_from_input(path_input_file=input_file, magnet_name=self.list_models[model_name].model_data.GeneralParameters.magnet_name,
+            pc.read_from_input(path_input_file=input_file, magnet_name=self.data_analysis.GeneralParameters.model.name,
                                strand_critical_current_measurements=strand_critical_current_measurements)
             # write a sweeper csv file
-            pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name,
+            pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name, # TODO simulation_name should be step variable in definition, model_name ist not step name
                                               simulation_number=simulation_number)
 
             # create parsim sweep step with newly created sweeper csv file and run it
             parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_sweeper_csv, # TODO rename teh class to ParametricSweepStep? ParsimConductor is no step class and ParametricSweep is
                                                 model_name=model_name, case_model=case_model, software=software, verbose=verbose)
-            self.run_parsim_sweep(parsim_sweep_step, verbose=verbose)
+            self.run_parsim_sweep(parsim_sweep_step, verbose=verbose, revert=False)
         else:
             raise Exception(f'Case_model "{case_model}" not supported by ParsimConductor.')
 
-    def run_parsim_sweep(self, step, verbose: bool = False):
+    def run_parsim_sweep(self, step, verbose: bool = False, revert: bool = True):
         '''
         Function to generate steps based on list of models read from external file
         :param step:
         :param verbose: if true displays more information
-        :return:
+        :param revert: if true the changes to the BM object are reverted after setting up the simulation files row by row
         '''
         # Unpack inputs
         input_sweep_file = step.input_sweep_file
         default_model_name = step.model_name
         case_model = step.case_model
         software = step.software
         verbose = step.verbose
@@ -1547,31 +1660,15 @@
             try:
                 # number has to be present & has to be an int (or be parsable into one) for the rest of the code to work
                 simulation_number = int(row['simulation_number'])
             except:
                 raise Exception(f'ERROR: no simulation_number provided in csv file {input_sweep_file}.')
             if verbose: print(f'changing these fields row # {i + 1}: {row}')
 
-            # save the earliest starting time of Quench Heaters to definitely start the simulation beforehand
-            if case_model == 'magnet':
-                new_start_time = self.__get_earliest_QH_starting_time(row)
-
-            # set simulation start time 50 ms before the start time of the first Quench Heater
             dict_variables_to_change = dict()
-            if case_model == 'magnet' and 'LEDET' in software:
-                time_vec = rgetattr(self.list_models[model_name].model_data,'Options_LEDET.time_vector.time_vector_params')
-                if new_start_time:
-                    # shift all times in time_vector by the difference by which the simulation has to start earlier
-                    diff = new_start_time - time_vec[0]
-                    # time_vec structure is: [start_val1, step_size1, end_val1, start_val2, step_size2, end_val2, ...]
-                    # all values of time should be shifted in space by the difference (all start and end values)
-                    for i in range(int(len(time_vec)/3)):
-                        time_vec[0+3*i] = time_vec[0+3*i] + diff
-                        time_vec[2+3*i] = time_vec[2+3*i] + diff
-                dict_variables_to_change['Options_LEDET.time_vector.time_vector_params'] = time_vec
 
             # unpack model_data
             if case_model == 'magnet':
                 model_data = self.list_models[model_name].model_data
                 next_simulation_name = model_data.GeneralParameters.magnet_name
             elif case_model == 'circuit':
                 model_data = self.list_models[model_name].circuit_data
@@ -1638,103 +1735,183 @@
                 elif case_model == 'conductor':
                     dict_variables_to_change['GeneralParameters.conductor_name'] = rgetattr(model_data, 'GeneralParameters.conductor_name')
                 else:
                     raise Exception(f'case_model {case_model} not supported by ParsimSweep.')
 
 
             # copy original model to reset changes that step_modify_model_multiple_variables does
-            local_model_copy = deepcopy(self.list_models[model_name])
+            if revert: local_model_copy = deepcopy(self.list_models[model_name])
 
             # make step ModifyModelMultipleVariables and alter all values found before
             next_step = ModifyModelMultipleVariables(type='ModifyModelMultipleVariables')
             next_step.model_name = model_name
             next_step.simulation_name = next_simulation_name
             next_step.variables_value = [[val] for val in dict_variables_to_change.values()]
             next_step.variables_to_change = list(dict_variables_to_change.keys())
             next_step.simulation_numbers = [simulation_number]
             next_step.software = software
             self.step_modify_model_multiple_variables(next_step, verbose=verbose)
 
-            # reset changes to the model in self
-            self.list_models[model_name] = deepcopy(local_model_copy)
-        del local_model_copy
+            # reset changes to the model in self if revert flag is set
+            if revert:
+                self.list_models[model_name] = deepcopy(local_model_copy)
+                del local_model_copy
 
         if verbose:
             print(f'Parsim Event called using input file {input_sweep_file}.')
 
-    def __get_earliest_QH_starting_time(self, row: pd.Series, t_before_QH_start: float = 0.05,
-                                        t_earliest_starting_time: float = -10, t_latest_starting_time: float = 10):
-        if 'Quench_Protection.Quench_Heaters.t_trigger' in row:
-            min_value = (min(parse_str_to_list(row['Quench_Protection.Quench_Heaters.t_trigger'])))
-            # if all QH fire after a specified time (default 1sec), it is likely that they are switched off - so dont change default simulation starting time
-            if min_value > t_latest_starting_time: return None
-            # start simulation t_before_QH_start seconds before the first Quench Heater starts
-            return max(min_value - t_before_QH_start, t_earliest_starting_time)  # no values smaller then t_earliest_starting_time make sense
-        else:
-            if self.verbose:
-                print('No start time for Quench Heaters found in csv file. Using default simulation time.')
-            return None
-
     def __get_circuit_family_name(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "60A"
         elif circuit_name.startswith("RD"):
             return "IPD"
         elif circuit_name.startswith("RQX"):
             return "RQX"
+        elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
+            return "IPQ"
+        elif circuit_name.startswith(("RQT12", "RQT13", "RQS", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RCBX", "RQSX3", "RCS", "ROD", "ROF", "RQ6", "RSD", "RSF", "RQTL9", "RQTD", "RQTF")):
+            return "600A"
         elif circuit_name.startswith("RQ"):
             return "RQ"
+        elif circuit_name.startswith(("RCBY", "RCBC", "RCTX")):
+            return "80-120A"
+        elif circuit_name.startswith("RB"):
+            return "RB"
+
 
     def __get_magnet_name(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "MCBH"
         elif circuit_name.startswith("RD"):
             circuit_type = self.__get_circuit_type(circuit_name)
             magnet_dict = {"RD1": "MBX", "RD2": "MBRC", "RD3": "MBRS", "RD4": "MBRB"}
             return magnet_dict.get(circuit_type, "")
         elif circuit_name.startswith("RQX"):
             return ["MQXA", "MQXB"]
+        elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
+            magnet_dict = {"IPQ_RQ4_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ4_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ5_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ5_2_2xRPHH_2xMQY": "MQY", "IPQ_RQ5_4_2xRPHGB_4xMQM": ["MQM", "MQM"], "IPQ_RQ5_4_2xRPHH_4xMQY": ["MQY", "MQY"], "IPQ_RQ6_2_2xRPHGB_2xMQML": "MQML", "IPQ_RQ6_2_2xRPHGB_2xMQY": "MQY", "IPQ_RQ6_4_2xRPHGB_2xMQM_2xMQML": ["MQM", "MQML"], "IPQ_RQ7_2_2xRPHGA_2xMQM": "MQM", "IPQ_RQ7_4_2xRPHGA_4xMQM": ["MQM", "MQM"], "IPQ_RQ8_2_2xRPHGA_2xMQML": "MQML", "IPQ_RQ9_4_2xRPHGA_2xMQM_2xMQMC": ["MQM", "MQMC"], "IPQ_RQ10_2_2xRPHGA_2xMQML": "MQML"}
+            return magnet_dict.get(self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name, "")
         elif circuit_name.startswith("RQ"):
             return "MQ"
+        elif circuit_name.startswith("RCBY"):
+            return "MCBYH"
+        elif circuit_name.startswith("RCBC"):
+            return "MCBCH"
+        elif circuit_name.startswith("RQT12"):
+            return "MQT"
+        elif circuit_name.startswith("RCS"):
+            return ["MCS", "MCS_quenchback"]
+        elif circuit_name.startswith("RB"):
+            return "MB"
+        elif circuit_name.startswith("RCBX"):
+            return ["MCBXH", "MCBXV"]
 
     def __get_number_of_magnets(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
-        if circuit_family_name in ["60A", "IPD"]:
+        circuit_type = self.__get_circuit_type(circuit_name)
+        if circuit_type in ["RCS", "RB"]:
+            return 154
+        elif circuit_family_name in ["60A", "IPD", "80-120A", "600A"]: #RCO (77) out of ambit
             return 1
         elif circuit_family_name == "RQ":
             return 47  # deal with 51 later
         elif circuit_family_name == "RQX":
             return 4
+        elif circuit_family_name == "IPQ":
+            return int(int(re.search(r'_(\d+)_', self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name).group(1))/2)
 
     def __get_number_of_apertures(self, circuit_name: str):
         circuit_family_name = self.__get_circuit_family_name(circuit_name)
-        if circuit_family_name == "IPQ":
+        if circuit_family_name in ["IPQ", "RB"]:
             return 2
         else:
             return 1
 
     def __get_magnets_list(self, number_of_magnets: int):
         list = []
         for i in range(1, number_of_magnets+1):
             list.append(i)
         return list
 
     def __get_magnet_types_list(self, number_of_magnets: int):
         list = []
         if number_of_magnets == 4: #to be improved
             list = [1, 2, 2, 1]
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name.startswith("IPQ") and number_of_magnets == 2:
+            list = [1, 2]
+        elif self.data_analysis.AnalysisStepDefinition['runParsimEvent'].simulation_name.startswith("RB"):
+            for i in range(1, number_of_magnets+1):
+                list.append(1)
+        elif number_of_magnets in [154, 13, 8, 77, 6, 12, 11, 10, 9]:
+            list = [1] + [2] * (number_of_magnets - 1)
         else:
             for i in range(1, number_of_magnets+1):
                 list.append(1)
         return list
 
     def __get_circuit_type(self, circuit_name: str):
         if circuit_name.startswith("RCBH") or circuit_name.startswith("RCBV"):
             return "RCB"
         elif circuit_name.startswith(("RD1", "RD2", "RD3", "RD4")):
             return {"RD1": "RD1", "RD2": "RD2", "RD3": "RD3", "RD4": "RD4"}.get(circuit_name[:3], "No match found")
         elif circuit_name.startswith("RQX"):
             return "RQX"
+        elif circuit_name.startswith(("RQ4", "RQ5", "RQ6", "RQ7", "RQ8", "RQ9", "RQ10")):
+            return circuit_name.split(".")[0]
+        elif circuit_name.startswith("RQT12"):
+            return "RQT12"
         elif circuit_name.startswith("RQ"):
             return "RQ"
+        elif circuit_name.startswith("RCS"):
+            return "RCS"
+        elif circuit_name.startswith("RB"):
+            return "RB"
+        elif circuit_name.startswith("RCBX"):
+            return "RCBX"
+
+    def __get_quenching_magnet_number(self, position: str, circuit_family_name: str):
+        df = pd.read_csv(os.path.join(f"../../tests/analyses/input/run_parsim_event_circuit/{circuit_family_name}_LayoutDetails.csv"))
+        mask = df['Magnet'].str.split('.').str[1] == position
+        result = df.loc[mask, '#Electric_circuit'].iloc[0]
+        return result
+
+
+    def __split_csv(self, input_file_name):
+        # Create empty lists to hold the odd and even rows
+        odd_rows = []
+        even_rows = []
+
+        # Open the input CSV file and read in the rows
+        with open(input_file_name, 'r') as input_file:
+            reader = csv.reader(input_file)
+
+            # Save the header row
+            header = next(reader)
+
+            # Loop over the remaining rows and append them to the odd or even list
+            for i, row in enumerate(reader):
+                if i % 2 == 0:
+                    even_rows.append(row)
+                else:
+                    odd_rows.append(row)
+
+        # Write the odd and even rows to separate output files
+        output_odd_file_name = 'output_odd.csv'
+        with open(output_odd_file_name, 'w', newline='') as output_odd_file:
+            writer_odd = csv.writer(output_odd_file)
+            writer_odd.writerow(header)
+            writer_odd.writerows(odd_rows)
+
+        output_even_file_name = 'output_even.csv'
+        with open(output_even_file_name, 'w', newline='') as output_even_file:
+            writer_even = csv.writer(output_even_file)
+            writer_even.writerow(header)
+            writer_even.writerows(even_rows)
+
+        # Return a list of the output file names
+        return [output_even_file_name, output_odd_file_name]
+
+
+
+
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.5.0/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.5.0/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/builders/BuilderLEDET.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import numpy as np
 import pandas as pd
 import openpyxl
 import csv
 from pathlib import Path
 from operator import itemgetter
+from typing import List
 
 from steam_sdk.data.DataLEDET import LEDETInputs, LEDETOptions, LEDETPlots, LEDETVariables, LEDETAuxiliary
 from steam_sdk.data.DataRoxieParser import RoxieData
 from steam_sdk.data import DataModelMagnet, DataModelConductor
 from steam_sdk.data import DictionaryLEDET
 from steam_sdk.configs.tools_defaults.ToolDefaultReader import ToolDefaultReader
 from steam_sdk.builders.geometricFunctions import close_pairs_ckdtree
@@ -91,15 +92,15 @@
                 if self.input_map2d:
                     # Read ROXIE-generated .map2d file, load some conductor parameters, and calculate other parameters
                     self.loadParametersFromMap2d(path_map2d=self.input_map2d, flag_plot=self.flag_plot_all)
                 else:
                     if verbose: print('Map2d file not defined. Some geometry parameters will be read from the input yaml file.')
                     self.loadParametersFromDataModel()
 
-                    # Load conductor data from DataModelMagnet keys
+                # Load conductor data from DataModelMagnet keys
                 if self.model_data.GeneralParameters.magnet_type in ['multipole', 'busbar']:
                     self.loadConductorData()
 
                 # Calculate electrical order of the half-turns
                 self.calcElectricalOrder(flag_plot=self.flag_plot_all)
 
                 # Calculate thermal connections, i.e. pairs of half-turns that are in thermal contact
@@ -112,14 +113,17 @@
                 else:
                     if self.Auxiliary.iContactAlongHeight_pairs_to_add or self.Auxiliary.iContactAlongWidth_pairs_to_add:   # only if any of these are specified
                         self.addThermalConnectionsCCT()
 
                 # Remove thermal connections which where manually set
                 self.removeThermalConnections(flag_plot=self.flag_plot_all)
 
+                # If needed, convert QH parameters from strings to integers
+                self.convert_QH_parameters()
+
                 # Calculate self-mutual inductances between magnet coil sections and turns
                 if self.Auxiliary.flag_calculate_inductance:
                     self.calculateSelfMutualInductance(csv_write_path=self.smic_write_path)
                 else:
                     self.setSelfMutualInductances()
 
                 if self.model_data.GeneralParameters.magnet_type == 'CCT_straight':
@@ -1296,14 +1300,42 @@
             if self.verbose: print('Selected thermal links are removed.')
 
         if flag_plot:
             PM = PlotterModel(self.roxie_data)
             PM.plot_heat_connections(iContactAlongHeight_From, iContactAlongHeight_To, iContactAlongWidth_From, iContactAlongWidth_To, self.Auxiliary.x_strands, self.Auxiliary.y_strands, self.Auxiliary.strandToHalfTurn, self.model_data)
 
 
+    def convert_QH_parameters(self, list_vars_to_convert: List[str] = ['type_ins_QH', 'type_ins_QH_He']):
+        '''
+        The material type of QH insulation layers can be defined either as string or as integer.
+        If it is defined as string, this method will convert the values into integers.
+        Values that are already numeric will not be converted.
+        :param list_vars_to_convert: List of variables to convert. Bu default, the QH insulation layers on both sides
+        are included.
+        '''
+        for var_name in list_vars_to_convert:
+            var_value = getattr(self.Inputs, var_name)
+
+            if isinstance(var_value[0], list):  # case 1: list of lists of strings
+                for row, row_values in enumerate(var_value):
+                    for col, col_value in enumerate(row_values):
+                        if col_value.isnumeric():
+                            var_value[row][col] = int(col_value)
+                        else:
+                            var_value[row][col] = DictionaryLEDET.lookupInsulation(col_value)
+            else:  # case 2: list of strings
+                for col, col_value in enumerate(var_value):
+                    if col_value.isnumeric():
+                        var_value[col] = int(col_value)
+                    else:
+                        var_value[col] = DictionaryLEDET.lookupInsulation(col_value)
+
+            self.setAttribute(self.Inputs, var_name, np.array(var_value, np.int32))
+
+
     def calculateSelfMutualInductance(self, csv_write_path: str = ''):
         """
             Calculate the self-mutual inductance matrix
             Calculation based on the SMIC code (https://cernbox.cern.ch/index.php/s/37F87v3oeI2Gkp3)
         """
         # TODO: since many parameters, maybe access as .self when used instead of unpacking
         # TODO: however, should be stated, e.g. in docstring, which parameters needed from the outside in order to run
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.5.0/steam_sdk/builders/BuilderModel.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,23 +12,24 @@
 from steam_sdk.builders.BuilderLEDET import BuilderLEDET
 from steam_sdk.builders.BuilderProteCCT import BuilderProteCCT
 from steam_sdk.builders.BuilderSIGMA import BuilderSIGMA
 from steam_sdk.parsers.ParserCsv import find_by_position, find_column_list
 from steam_sdk.parsers.ParserFiQuS import ParserFiQuS
 from steam_sdk.parsers.ParserLEDET import ParserLEDET, copy_modified_map2d_ribbon_cable, copy_map2d
 from steam_sdk.parsers.ParserPSPICE import ParserPSPICE
+from steam_sdk.parsers.ParserSIGMA import ParserSIGMA
 from steam_sdk.parsers.ParserXYCE import ParserXYCE
 from steam_sdk.parsers.ParserProteCCT import ParserProteCCT
 from steam_sdk.parsers.ParserProtePyBBQ import ParserPyBBQ
 from steam_sdk.parsers.ParserRoxie import ParserRoxie
 from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
 from steam_sdk.parsers.ParserYAML import dict_to_yaml, yaml_to_data
 from steam_sdk.plotters import PlotterRoxie
 from steam_sdk.plotters.PlotterModel import PlotterModel
-
+from steam_sdk.utils.create_coordinate_file_SIGMA import create_coordinate_file
 
 class BuilderModel:
     """
         Class to generate STEAM models, which can be later on written to input files of supported programs
     """
 
     def __init__(self,
@@ -522,27 +523,40 @@
                                      verbose=self.verbose)
 
         # Write output yaml file
         parser_PyBBQ = ParserPyBBQ(builder_PyBBQ)
         nameFilePyBBQ = os.path.join(self.output_path, conductor_name + '.yaml')  # full path of the PyBBQ input file to write
         parser_PyBBQ.writePyBBQ2yaml(full_path_file_name=nameFilePyBBQ, verbose=self.verbose)
 
-    def buildSIGMA(self, output_path = None):
-        """
-            Building a SIGMA model
+    def buildSIGMA(self, simulation_name = None):
         """
-        file_working_directory = os.getcwd()
-        if not output_path:
-            output_path = self.output_path
-
-        BuilderSIGMA(input_model_data=self.model_data, input_roxie_data=self.roxie_data, bh_curve_database=self.path_bh,
-                     settings_dict=self.settings_dict, output_path=output_path,
-                     flag_build=self.flag_build, verbose=self.verbose)
-        os.chdir(file_working_directory)
+                  Building a FiQuS model
+                  :param simulation_name: This is used in analysis steam to change yaml name from magnet name to simulation name
+              """
+        if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source == None:
+            if self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d != None:
+                path_map2d = os.path.join(Path(self.path_bh).parent, self.model_data.GeneralParameters.magnet_name, 'input', self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.map2d )
+                destination_map2d = os.path.join(self.output_path, self.model_data.GeneralParameters.magnet_name + "_ROXIE_REFERENCE.map2d")
+                # Copy map2d file
+                shutil.copyfile(path_map2d, destination_map2d)
+                coordinate_file_path = os.path.join(self.output_path, self.model_data.GeneralParameters.magnet_name + "_ROXIE_COORD.csv")
+                # Create coordinate file
+                create_coordinate_file(path_map2d, coordinate_file_path)
+                # Set file as coordinate_source
+                self.model_data.Options_SIGMA.postprocessing.out_2D_at_points.coordinate_source = coordinate_file_path
+
+        builder_SIGMA = BuilderSIGMA(model_data=self.model_data, roxie_data=self.roxie_data,
+                                     flag_build=self.flag_build, flag_plot_all=self.flag_plot_all, verbose=self.verbose)
+
+        # if map2d specified then copy to working folder,
 
+        # Write output files
+        self.parser_SIGMA = ParserSIGMA(builder_SIGMA, verbose=self.verbose)
+        self.parser_SIGMA.writeSIGMA2yaml(output_path=self.output_path, simulation_name=simulation_name,
+                                          append_str_to_magnet_name='_SIGMA')
 
     def load_circuit_parameters_from_csv(self, input_file_name: str, selected_circuit_name: str = None):
         '''
             Load circuit parameters from a csv file into a case=circuit object
             :param input_file_name: full path to the csv file
             :param selected_circuit_name: name of the circuit name whose parameters will be loaded
         '''
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.5.0/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.5.0/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.5.0/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.5.0/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml` & `steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.5.0/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataAnalysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,17 @@
 
 
 class PostProcess(BaseModel):
     """
         Level 2: Analysis step to run a simulation file
     """
     type: Literal['PostProcess']
-
+    software: str = None
+    simulation_name: str = None
+    simulation_numbers: List[int] = []
 
 class RunCustomPyFunction(BaseModel):
     """
         Level 2: Analysis step to run a custom Python function
     """
     type: Literal['RunCustomPyFunction']
     flag_enable: bool = None
@@ -261,15 +263,15 @@
     model_name: str = None
     case_model: str = None
     input_file: str = None
     software: List[str] = []
     simulation_number: int = None
     strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement] = []
     groups_to_coils: Dict[str, List[int]] = {}
-    groups_to_coil_length: Dict[float, List[int]] = {}
+    length_to_coil: Dict[str, float] = {}
     path_output_sweeper_csv: str = None
 
 # class AnalysisStep(BaseModel):
 #     """
 #         Level 1: Class for information on the analysis step
 #         Objects of this class will be defined in AnalysisStepDefinition
 #     """
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     material_inner_voids: str = None
     material_outer_voids: str = None
     material_core: str = None
 
 
 class Ribbon(BaseModel):
     """
-        Mono cable type: This is basically type of cable consisting of one strand - not really a cable
+        Mono cable type: This is basically type of cable consisting of one strand - not really a cable # TODO copy error, this is not MONO
     """
     type: Literal['Ribbon']
     n_strands: int = None  # This defines the number of "strands" in the ribbon cable, which are physically glued but electrically in series
     bare_cable_width: float = None
     bare_cable_height_low: float = None
     bare_cable_height_high: float = None
     bare_cable_height_mean: float = None
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataModelMagnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,18 +177,18 @@
     N_strips: int = None                              # nHeaterStrips
     t_trigger: List[float] = []                        # tQH
     U0: List[float] = []
     C: List[float] = []
     R_warm: List[float] = []
     w: List[float] = []                             # In Sigma this
     h: List[float] = []
-    s_ins: List[float] = []
-    type_ins: List[int] = []
-    s_ins_He: List[float] = []
-    type_ins_He: List[int] = []
+    s_ins: Union[List[float], List[List[float]]] = []
+    type_ins: Union[List[str], List[List[str]]] = []
+    s_ins_He: Union[List[float], List[List[float]]] = []
+    type_ins_He: Union[List[str], List[List[str]]] = []
     l: List[float] = []
     l_copper: List[float] = []
     l_stainless_steel: List[float] = []
     f_cover: List[float] = []
     iQH_toHalfTurn_From: List[int] = []
     iQH_toHalfTurn_To: List[int] = []
 
@@ -925,15 +925,15 @@
     nbr_elements_mesh_width: int = None
     nbr_elements_mesh_height: int = None
 
 class PhysicsSIGMA(BaseModel):
     """
         Level 2: Class for physics parameters in SIGMA
     """
-    FLAG_M_pers: float = None # change to int
+    FLAG_M_pers: int = None
     FLAG_ifcc: int = None
     FLAG_iscc_crossover: int = None
     FLAG_iscc_adjw: int = None
     FLAG_iscc_adjn: int = None
     tauCC_PE: float = None
 
 
@@ -949,14 +949,15 @@
     quench_init_HT: List[str] = None
     quench_stop_temp: float = None
 
 class Out2DAtPointsSIGMA(BaseModel):
     coordinate_source: str = None
     variables: List[str] = None
     time: List[List[float]] = None
+    map2d: str = None
 
 
 class Out1DVsTimeSIGMA(BaseModel):
     variables: List[str] = None
     time: List[List[float]] = None
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataParsimConductor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from typing import (List, Dict, Union, Literal)
+from typing import (List, Dict)
 from pydantic import BaseModel
 
 ############################
 # General parameters
 class GeneralParameters(BaseModel):
     magnet_name: str = None
-    circuit_name: str = None
-    state: str = None  # measured, deduced from short-samples, deduced from design
+    circuit_name: str = None  # TODO currenty unused
+    state: str = None  # measured, deduced from short-samples, deduced from design  # TODO currenty unused
 
 ############################
 # Magnet
 class Magnet(BaseModel):
     coils: List[str] = []
-    measured_inductance_versus_current: List[List[float]] = []   # TODO why is this needed?
+    measured_inductance_versus_current: List[List[float]] = []   # TODO currenty unused
 
 ############################
 # Coils
 class IcMeasurement(BaseModel):
     """
         Level 1: Class for parameters of a critical current measurement to adjust Jc fit parameters
     """
@@ -32,43 +32,42 @@
     """
     diameter: float = None
     bare_width: float = None
     bare_height: float = None
 
 
 class ConductorSample(BaseModel):
-    # ID: str = None
-    # Ra: float = None
-    # Rc: float = None
+    ID: str = None  # TODO currenty unused
+    Ra: float = None
+    Rc: float = None
     number_of_strands: int = None
     width: float = None
     height: float = None
     strand_twist_pitch: float = None
     filament_twist_pitch: float = None
     RRR: float = None
     Cu_noCu: float = None
     # critical current measurement attributes
     Tc0: float = None
     Bc20: float = None
-    f_rho_eff: float = None  # TODO unused
+    f_rho_eff: float = None
     Ic_measurements: List[IcMeasurement] = []
     strand_geometry: StrandGeometry = StrandGeometry()
 
 
 
 class Coil(BaseModel):
-    ID: str = None  # TODO unused
-    cable_ID: str = None  # TODO unused
-    coil_length: float = None  # TODO unused
+    ID: str = None  # TODO currenty unused
+    cable_ID: str = None  # TODO currenty unused
     # Resistance measurement attributes
     coil_resistance_room_T: float = None
     Cu_noCu_resistance_meas: float = None
-    total_conductor_length: float = None
+    B_resistance_meas: float = None
     T_ref_coil_resistance: float = None
-    T_ref_RRR_low: float = None
+    T_ref_RRR_low: float = None  # TODO do i have to write this in modelData? there would be such an entry
     T_ref_RRR_high: float = None
     # list of conductor samples and weight factor
     conductorSamples: List[ConductorSample] = []
     weight_factors: List[float] = []
 
 
 
@@ -80,8 +79,7 @@
 
         :return: DataParsimConductor object
     '''
 
     GeneralParameters: GeneralParameters = GeneralParameters()
     Magnet: Magnet = Magnet()
     Coils: Dict[str, Coil] = {}  # Datastructure representing one row in the csv file
-    # ConductorSamples: Dict[str, ConductorSample] = {}
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.5.0/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.5.0/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/temp/postLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/temp/postLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/temp/runLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/temp/runLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/drivers/temp/simLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/drivers/temp/simLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserMat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import warnings
 
 import numpy as np
 import pandas as pd
 import h5py
-
+from scipy.io import loadmat
 
 def getSignalMat(path_sim, simNumber, list_Signals):
 
     simulationSignalsToPlot = pd.DataFrame()
 
     for i in range(len(simNumber)):
         path_simulationSignals = os.path.join(path_sim + str(simNumber[i]) + '.mat')
@@ -180,14 +180,18 @@
         self.t = np.array(self.data.get('time_vector')).T[0]
 
     def data_0D(self, var_name):
         return np.array(self.data.get(var_name))[0, 0]
 
     def data_1D(self, var_name, op='max'):
         data = np.array(self.data.get(var_name))
+        if data.dtype == object:
+            # https://stackoverflow.com/questions/17316880/reading-v-7-3-mat-file-in-python
+            list_of_pointers = [r and self.data.get(self.data[r].name, self.data[r].name) for r in data.flat][0]
+            return np.array(list_of_pointers).T
         if data.shape[0] == 1:
             return data[0]          # get first column
         elif data.shape[1] == 1:
             return data.T[0]        # transpose and get first column
         elif data.shape[0] == self.t.shape[0]:
             if op == 'min':
                 return data.min(axis=1)
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.5.0/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsers/templates/template_Dakota.in` & `steam-sdk-2023.5.0/steam_sdk/parsers/templates/template_Dakota.in`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.5.0/steam_sdk/parsims/ParsimConductor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,178 +1,228 @@
 import csv
 import warnings
 import math
-from scipy.optimize import fsolve
 import numpy as np
 import pandas as pd
 import steammaterials
-from steammaterials.STEAM_materials import STEAM_materials
 import os
 import yaml
-from typing import List, Dict
+from scipy.optimize import fsolve
+from steammaterials.STEAM_materials import STEAM_materials
+from pathlib import Path
+from typing import List, Dict, Any
 
-from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement, Coil
+from steam_sdk.data.DataParsimConductor import DataParsimConductor, IcMeasurement, Coil, StrandGeometry
+from steam_sdk.data.DataAnalysis import StrandCriticalCurrentMeasurement
 from steam_sdk.parsers.ParserMap2d import getParametersFromMap2d
 from steam_sdk.utils.get_attribute_type import get_attribute_type
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.rhasattr import rhasattr
 from steam_sdk.utils.sgetattr import rsetattr, rgetattr
 from steam_sdk.data.DataParsimConductor import ConductorSample
 from steam_sdk.utils.parse_str_to_list import parse_str_to_list
-
+from steam_sdk.data.DataModelMagnet import DataModelMagnet
+from steam_sdk.data.DataConductor import Conductor
 
 class ParsimConductor:
     """
+    class to assist running a ParsimConductor step
 
+    This class is used to:
+     - read_from_input: reading input table where every row represents one coil of a magent
+     - write_conductor_parameter_file: calculates all conductor parameters to change and writes them in a csv file for a ParsimSweeper step
     """
 
-    def __init__(self, model_data, groups_to_coils, groups_to_coil_length, dict_coilName_to_conductorIndex, verbose: bool = True):
-        """
-        If verbose is read to True, additional information will be displayed
-        """
+    def __init__(self, path_input_dir: Path, model_data: DataModelMagnet, groups_to_coils: Dict[str, List[int]],
+                 length_to_coil: Dict[str, float], dict_coilName_to_conductorIndex: Dict[str, int], verbose: bool = True):
+        '''
+        Initializes the ParsimConductor with the required input data and configurations.
+
+        :param path_input_dir: The path of the magnet directory in steam_models
+        :param model_data: The original model data of the magnet
+        :param groups_to_coils: A dictionary mapping coil name (key) to their respective groups (values).
+        :param length_to_coil: A dictionary mapping coil names to their lengths (if None or empty, length will be optimized - if coil length is known, fraction of copper will be optimized)
+        :param dict_coilName_to_conductorIndex: A dictionary mapping coil names to their respective conductor indices in BuilderModel
+        :param verbose: A boolean indicating whether to display additional information (default is True).
+        '''
         # Unpack arguments
         self.verbose: bool = verbose
         self.model_data = model_data
+        self.path_input_dir = path_input_dir
         self.dict_coilName_to_conductorIndex = dict_coilName_to_conductorIndex
         self.groups_to_coils = groups_to_coils
-
-        # groups_to_coil_length is either None (coil_length will be optimized) or dict (fCu will be optimized)
         self.number_of_groups = max([max(values) for values in self.groups_to_coils.values()])
-        if groups_to_coil_length and type(groups_to_coil_length) == float:
-            expected_group_numbers = list(range(1, self.number_of_groups + 1))
-            self.groups_to_coil_length = {groups_to_coil_length: expected_group_numbers}
-        else:
-            self.groups_to_coil_length = groups_to_coil_length
 
-        # check input: coil names in groups_to_coils and dict_coilName_to_conductorIndex have to be the same
+        # length_to_coil is either empty/None (coil_length will be optimized) or filled with {coilname: length} (fCu will be optimized)
+        if length_to_coil is None: length_to_coil = {}  # optimize coillength if not specified by the user
+        if not isinstance(length_to_coil, dict):
+            raise Exception(f'length_to_coil parameter of ParsimConductor step has to be a dict! Leave it empty if you dont know the values, otherwise specify the length for every coil.')
+        if length_to_coil != {}:
+            if not set(groups_to_coils.keys()) == set(length_to_coil.keys()):
+                raise Exception(f'Coils of input dictionaries dont have the same names.\ngroups_to_coils= {groups_to_coils.keys()}\nlength_to_coil= {length_to_coil.keys()}')
+        self.length_to_coil = length_to_coil
+
+        # check input: coil names in the input dicts have to be the same
         if not set(groups_to_coils.keys()) == set(dict_coilName_to_conductorIndex.keys()):
-            raise Exception(f'Coils of input dictionaries dont have the same names.')
+            raise Exception(f'Coils of input dictionaries dont have the same names.\ngroups_to_coils= {groups_to_coils.keys()}\ndict_coilName_to_conductorIndex= {dict_coilName_to_conductorIndex.keys()}')
 
-        # DataParsimConductor object that will hold all the information from the input csv file
+        # DataParsimConductor object that will hold all the information from the input csv file when reading it
         self.data_parsim_conductor = DataParsimConductor()
 
-    def read_from_input(self, path_input_file: str, magnet_name: str, strand_critical_current_measurements: Dict[str, Dict]):
+    def read_from_input(self, path_input_file: str, magnet_name: str, strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement]):
         '''
-        Read a .csv file and assign its content to a instance of DataParsimConductor().
+        Reads a .csv or .xlsx file containing magnet and coil data, and assigns its content to an instance of DataParsimConductor.
 
-        Parameters:
-            path_input_file: Path to the .csv file to read
-            magnet_name: name of the magnet that should be changed
-            strand_critical_current_measurements: dict of all the critical current measurements details specified by the user
+        :param path_input_file: The path to the .csv or .xlsx file to read.
+        :param magnet_name: The name of the magnet for which data should be processed.
+        :param strand_critical_current_measurements: A dictionary containing the critical current measurements details specified by the user.
         '''
 
         # read table into pandas dataframe
         if path_input_file.endswith('.csv'):
             df_coils = pd.read_csv(path_input_file)
         elif path_input_file.endswith('.xlsx'):
             df_coils = pd.read_excel(path_input_file)
         else:
             raise Exception(f'The extension of the file {path_input_file} is not supported. Use either csv or xlsx.')
         df_coils = df_coils.dropna(axis=1, how='all')
 
         # read dict for reading columns into local dataclass
+        # to add new column names the code does not have to be changed, just add the new colunm names to this yaml file
         yaml_path = os.path.join(os.path.dirname(os.path.abspath(__file__)), "translation_dicts", "conductor_column_names.yaml")
         with open(yaml_path, 'r') as file:
-            dict_attribute_to_column = yaml.safe_load(file) # TODO discuss with mariusz and implement also in ParsimEventMagnet
+            # this dict now holds the attribute names as keys and a list of possible column names as values
+            dict_attribute_to_column = yaml.safe_load(file)
 
         # set magnet name to local model
         rsetattr(self.data_parsim_conductor, 'GeneralParameters.magnet_name', magnet_name)
 
         # get column name of coil and magnet
         parsed_columns = []  # list containing the column names that were parsed
         column_name_magnets, column_name_coils = self.__get_and_check_main_column_names(df_coils, parsed_columns, dict_attribute_to_column['MainColumnNames'])
 
         # delete all rows of dataframe that don't belong to the magnet
         mask = df_coils[column_name_magnets] != magnet_name  # create a boolean mask for the rows that do not have the value in the column
         df_coils = df_coils.drop(df_coils[mask].index)  # drop the rows that do not have the value in the column
 
         # Assign the content to a dataclass structure - loop over all the coils of the magnet in the database
         for _, row in df_coils.iterrows():
+            # in case coilname is only a number, convert it to str
+            if isinstance(row[column_name_coils], (int, float)): row[column_name_coils] = str(row[column_name_coils])
+            # if the coil name is not present in the userinput dictionary, don't read it
+            if row[column_name_coils] not in self.dict_coilName_to_conductorIndex.keys():
+                warnings.warn(f'The coil {row[column_name_coils]} is present in the conductor database but is not used.')
+                continue
             self.__read_magnet(row, column_name_coils, parsed_columns)
             self.__read_coils(row, column_name_coils, parsed_columns, dict_attribute_to_column['Coil'])
             self.__read_conductors(row, column_name_coils, parsed_columns, strand_critical_current_measurements,
                                    dict_attribute_to_column['ConductorSample'])
 
+        # check if all needed coils could be found in the conductor database
+        for need_coil_name in self.dict_coilName_to_conductorIndex.keys():
+            if need_coil_name not in self.data_parsim_conductor.Coils.keys():
+                raise Exception(f'The coil {need_coil_name} for the magnet {magnet_name} could not be found in the conductor database. Please check the input dictionaries.')
+
         # show the user all the columns that where ignored by the code
         ignored_column_names = list(set(df_coils.columns) - set(parsed_columns))
         if self.verbose: print(f'Names of ignored columns: {ignored_column_names}')
 
-    def write_conductor_parameter_file(self, path_output_file: str, simulation_name: str, simulation_number: int):
+    def write_conductor_parameter_file(self, path_output_file: str, simulation_name: str, simulation_number: int, rel_warning_limit: float = 0.1):
         """
-        Write the Parsim Conductor information to a CSV file, that can be used to run a ParsimSweep Step.
+        Calculates and writes the conductor parameters to change from the DataParsimConductor instance to a csv file
+        for running a ParsimSweep step.
 
-        Parameters:
-            path_output_file (str): path to the output file
-            groups_to_coil_length: None, float or dict
+        :param path_output_file: The path to the output file
+        :param simulation_name: The name of the simulation
+        :param simulation_number: The number of the simulation
+        :param rel_warning_limit: function raises warning in console when values are changed for more/less then this relative value
         """
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_output_file))
 
         # save all conductor parameters in a dict
         dict_sweeper = dict()
         dict_sweeper['simulation_name'] = simulation_name
         dict_sweeper['simulation_number'] = int(simulation_number)
 
         # write all the ConductorSample data to
-        if self.groups_to_coil_length:
+        if self.length_to_coil != {}:
             # if groups_to_coil_length is specified, optimize the fraction of superconductor
-            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=True)
+            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=True, rel_warning_limit=rel_warning_limit)
         else:
             # if no groups_to_coil_length is specified, optimize the length of the magnet
-            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=False)
-            # self.__write_parsweep_optimized_ht_length(dict_sweeper)
+            self.__write_parsweep_conductors(dict_sweeper, flag_optimize_fCu=False, rel_warning_limit=rel_warning_limit)
+            self.__write_parsweep_optimized_ht_length(dict_sweeper)
 
         # open file in writing mode and write the dict of the parameters as a row in the sweeper csv file
         with open(path_output_file, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=dict_sweeper.keys())
             writer.writeheader()
             writer.writerow(dict_sweeper)
 
     ################ HELPERS
 
-    def __get_and_check_main_column_names(self, df_coils, parsed_columns, dict_attr_to_colname):
+    def __get_and_check_main_column_names(self, df_coils: pd.DataFrame, parsed_columns: List[str], dict_attr_to_colname: Dict[str, List[str]]):
         '''
-            TODO refactoring and docstrings
+        function checking the main columns "magnet name" and "coil name" and returning their column name
+
+        :param df_coils: dataframe where every row represents one coil
+        :param parsed_columns: A list of column names that have already been parsed (parsed columns are added)
+        :param dict_attr_to_colname: A dictionary mapping attribute names of the coil (key) to possible column names (values)
         '''
         # allowed names for the magnet
         csv_column_names_for_magnet_name = dict_attr_to_colname['magnet_name']
         csv_column_names_for_coil_name = dict_attr_to_colname['coil_name']
 
         # find out what name is being used for the magnet and coil column
         column_name_magnets, column_name_coils = None, None
         for col_name_magnet in csv_column_names_for_magnet_name:
             if col_name_magnet in df_coils.keys():
                 column_name_magnets = col_name_magnet
         for col_name_coil in csv_column_names_for_coil_name:
             if col_name_coil in df_coils.keys():
                 column_name_coils = col_name_coil
-        # TODO do i check later if coilnames are valid?
 
         # check if there is a column for magnet and coil
         if not column_name_magnets:
             raise Exception(f'No column for the magnet name could be found in the input table. Make sure this column is present.\nAllowed values :{csv_column_names_for_magnet_name}')
         if not column_name_coils:
             raise Exception(f'No column for the coil names could be found in the input table. Make sure this columns are present.\nAllowed values:{csv_column_names_for_coil_name}')
 
         # check if magnet name is present in the xlsx file
         if not any(df_coils[column_name_magnets] == self.data_parsim_conductor.GeneralParameters.magnet_name):
-            raise Exception(f'The magnet "{self.data_parsim_conductor.GeneralParameters.magnet_name}" is not present in the conductor database. ')
+            raise Exception(f'The magnet "{self.data_parsim_conductor.GeneralParameters.magnet_name}" is not present in the conductor database. Please change the GeneralParameters.model.name in the analysis input file.')
 
         # mark columns as parsed
         parsed_columns.append(column_name_magnets)
         parsed_columns.append(column_name_coils)
 
         return column_name_magnets, column_name_coils
 
-    def __read_magnet(self, row, column_name_coils, parsed_columns):
+    def __read_magnet(self, row: pd.Series, column_name_coils: str, parsed_columns: List[str]):
+        '''
+        Adds the coil name from the given row to the Magnet's list of coils in the DataParsimConductor instance.
+
+        :param row: A pandas Series object representing a row in the input table where a row is a coil of the magnet
+        :param column_name_coils: The name of the column containing the coil names in the input table
+        :param parsed_columns: A list of column names that have already been parsed (parsed columns are added)
+        '''
         # add coil name to Coils list
         self.data_parsim_conductor.Magnet.coils.append(row[column_name_coils])
         
-    def __read_coils(self, row, column_name_coils, parsed_columns, dict_attr_to_colname):
+    def __read_coils(self, row: pd.Series, column_name_coils: str, parsed_columns: List[str], dict_attr_to_colname: Dict[str, List[str]]):
+        '''
+        Reads coil related data for a row in the table into a new Coil instance, and adds it to the DataParsimConductor instance
+
+        :param row: A pandas Series object representing a row in the input table where a row is a coil of the magnet
+        :param column_name_coils: The name of the column containing the coil names in the input table
+        :param parsed_columns: A list of column names that have already been parsed (parsed columns are added)
+        :param dict_attr_to_colname: A dictionary mapping attribute names of the coil (key) to possible column names (values)
+        '''
         # create new coil instance
         coil_name = row[column_name_coils]
         new_Coil = Coil()
 
         # change parameters of coil instance according to yaml translation file
         for attribute_name, column_names in dict_attr_to_colname.items():
             # check if only one column for the attribute can be found
@@ -180,15 +230,15 @@
             if len(used_column_names) == 1:
                 used_column_name = used_column_names[0]
             elif len(used_column_names) == 0:
                 warnings.warn(f'No column for Coil attribute "{attribute_name}" found.')
                 continue
             else: raise ValueError(f"More then one column for the ConductorSample attribute '{attribute_name}' found.")
 
-            # check dimension of input column to convert number into SI unit
+            # extract unit of the value from the column name - unit is given in squared brackets (e.g. "voltage [V]")
             dim = used_column_name[used_column_name.find('[') + 1:used_column_name.find(']')] if '[' in used_column_name else ''
             # check if value is set in csv file
             if not pd.isna(row[used_column_name]):
                 # if input is a float list in string format, parse it into a float list
                 if get_attribute_type(new_Coil, attribute_name)[0] == List[float]:
                     if isinstance(row[used_column_name], str):
                         float_list = parse_str_to_list(row[used_column_name], only_float_list=True)
@@ -197,22 +247,33 @@
                     rsetattr(new_Coil, attribute_name, [make_value_SI(val, dim) for val in float_list])
                 else:
                     # change parameter and convert number into SI unit
                     rsetattr(new_Coil, attribute_name, make_value_SI(row[used_column_name], dim))
                 # mark column as parsed
                 if used_column_name not in parsed_columns: parsed_columns.append(used_column_name)
 
+        # normalize weight factors if not normalized
+        if new_Coil.weight_factors and sum(new_Coil.weight_factors) != 1.0:
+            weight_sum = sum(new_Coil.weight_factors)
+            new_Coil.weight_factors = [w / weight_sum for w in new_Coil.weight_factors]
+
+        # add new coil to local DataParsimConductor dataclass
         self.data_parsim_conductor.Coils[coil_name] = new_Coil
 
-    def __read_conductors(self, row, column_name_coils, parsed_columns, strand_critical_current_measurements, dict_attr_to_colname):
+    def __read_conductors(self, row: pd.Series, column_name_coils: str, parsed_columns: List[str],
+                          strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement],
+                          dict_attr_to_colname: Dict[str, List[str]]):
         '''
-        Function to read ConductorSamples of ParsimConductors
+        Reads conductor related data for a row in the table into ConductorSample instances and adds them to the corresponding Coil instance.
 
-        :param row: Series of parameters (read from csv file)
-        :param parsed_columns: list of parsed table columns names
+        :param row: A pandas Series object representing a row in the input table where a row is a coil of the magnet
+        :param column_name_coils: The name of the column containing the coil names in the input table
+        :param parsed_columns: A list of column names that have already been parsed (parsed columns are added)
+        :param strand_critical_current_measurements: A dictionary of critical current measurements provided by the user
+        :param dict_attr_to_colname: A dictionary mapping attribute names of the conductor samples (key) to possible column names (values)
         '''
         coil_name = row[column_name_coils]
 
         # read how many conductor samples there are in the database for this coil
         n_conductor_samples_found = []
         all_col_names = [string for string_list in dict_attr_to_colname.values() for string in string_list]
         # add column names for Ic measurements
@@ -221,15 +282,16 @@
                 all_col_names.append(meas.column_name_I_critical)
                 all_col_names.append(meas.column_name_CuNoCu_short_sample)
         for col_name in all_col_names:
             if col_name in row and not pd.isna(row[col_name]) and isinstance(row[col_name], str):
                 float_list = parse_str_to_list(row[col_name], only_float_list=True)
                 n_conductor_samples_found.append(len(float_list))
         if all(element == n_conductor_samples_found[0] for element in n_conductor_samples_found):
-            n_conductor_samples = n_conductor_samples_found[0]
+            if len(n_conductor_samples_found)==0: n_conductor_samples = 1
+            else: n_conductor_samples = n_conductor_samples_found[0]
         else:
             raise Exception(f'Different number of Conductor Samples found for Coil "{coil_name}".')
 
         # check length of weight factors
         if self.data_parsim_conductor.Coils[coil_name].weight_factors:
             if len(self.data_parsim_conductor.Coils[coil_name].weight_factors) != n_conductor_samples:
                 raise Exception(f'Length of weight factor for coil {coil_name} is not similar to number of Conductor samples. Please correct the length to {n_conductor_samples} or delete entry (the average of the values will then be calculated)')
@@ -245,24 +307,23 @@
                     raise Exception(f'Invalid column name for I_critical. "{meas.column_name_I_critical}" already used for the attribute "{attr_name}". Please change.')
                 if meas.column_name_CuNoCu_short_sample in col_names:
                     raise Exception(f'Invalid column name for I_critical. "{meas.column_name_CuNoCu_short_sample}" already used for the attribute "{attr_name}". Please change.')
 
             if coil_name in meas.coil_names:
                 # create new IcMeasurement instances, add all values and append it to the measurement list of the conductor
                 new_Ic_measurements = [IcMeasurement() for _ in range(n_conductor_samples)]
-                  # TODO falsch - ConductorSample braucht list of IcMeasurement
                 # add temperature and magnetic flux of the measurements (directly given in step definition)
                 for Ic_meas in new_Ic_measurements:
                     rsetattr(Ic_meas, 'B_ref_Ic', meas.reference_mag_field)
                     rsetattr(Ic_meas, 'T_ref_Ic', meas.reference_temperature)
                 # read critical current form csv file
                 if meas.column_name_I_critical in row and not pd.isna(row[meas.column_name_I_critical]):
                     setattr_to_list(new_Ic_measurements, row, meas.column_name_I_critical, 'Ic')
                 else:
-                    raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty for coil {coil_name}.')
+                    raise Exception(f'Provided column name for Ic measurement "{meas.column_name_I_critical}" was not found in the conductor database or is empty for coil {coil_name}.')
                 # read CuNoCu ratio of the short sample measurement
                 if meas.column_name_CuNoCu_short_sample in row and not pd.isna(row[meas.column_name_CuNoCu_short_sample]):
                     setattr_to_list(new_Ic_measurements, row, meas.column_name_CuNoCu_short_sample, 'Cu_noCu_sample')
                 else:
                     raise Exception(f'Provided coulumn name for Ic measurement "{meas.column_name_CuNoCu_short_sample}" was not found in the conductor database or is empty.')
                 # append the new Ic measurements to a conductor sample
                 for cond, Ic_meas in zip(new_Conductors, new_Ic_measurements):
@@ -283,140 +344,175 @@
             if not pd.isna(row[used_column_name]):
                 setattr_to_list(new_Conductors, row, used_column_name, attribute_name)
             # mark column as parsed
             if used_column_name not in parsed_columns: parsed_columns.append(used_column_name)
 
         # check if only either diameter or bare w/h is set and check if original conductor type is the right one
         original_conductor_type = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]].strand.type
-        if not original_conductor_type: raise Exception(f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
+        if not original_conductor_type: raise Exception(f'Strand type of conductor for coil {coil_name} is not specified in modelData.')
         for cond in new_Conductors:
             if original_conductor_type == 'Round':
                 if cond.strand_geometry.bare_width or cond.strand_geometry.bare_height:
-                    raise Exception(f'Tried to change bare with/height of Round coil named {coil_name}')
+                    raise Exception(f'Tried to change bare with/height of Round conductor in coil {coil_name}')
             elif original_conductor_type == 'Rectangular':
                 if cond.strand_geometry.diameter:
-                    raise Exception(f'Tried to change diameter of Rectangular coil named {coil_name}')
+                    raise Exception(f'Tried to change diameter of Rectangular conductor in coil {coil_name}')
             else:
-                raise Exception(f'Unknown conductor type {original_conductor_type} for for coil {coil_name}.')
+                raise Exception(f'Unknown conductor type {original_conductor_type} for coil {coil_name}.')
 
         # append new conductor instance to Conductors dictionary of ParsimConductor
         self.data_parsim_conductor.Coils[coil_name].conductorSamples = new_Conductors
 
 
-    def __write_parsweep_optimized_ht_length(self, dict_sweeper):
-        # create empty list to later fill with optimized values
-        half_turn_length = [None for _ in range(self.number_of_groups)]
+    def __write_parsweep_optimized_ht_length(self, dict_sweeper: Dict[str, Any]):
+        """
+        Optimizes the half-turn length for each conductor sample in each coil and calculates the average for each group.
+
+        :param dict_sweeper: The dictionary where the optimized half-turn length will be stored, in the format {attributeNameDataModelMagnet: newValue}
+        """
+        ht_len = [0.0 for _ in range(self.number_of_groups)]
 
-        # looping through the coil list
+        # looping through the coils
         for coil_name, coil in self.data_parsim_conductor.Coils.items():
+            if not coil.coil_resistance_room_T:
+                warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Using default value from modelData.')
+                continue
             original_conductor = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]]
+            # calculate the optimized coil length for every group in the conductor sample separately
+            for sample in coil.conductorSamples:
+                # optimize the length for this coil with one conductor
+                L = self.__optimize_coil_length_with_resistance_meas(sample, coil_name, original_conductor, coil)
+                # for every conductorSamples add the optimized lengths together (to later make the average)
+                for group_number in self.groups_to_coils[coil_name]:
+                    ht_len[group_number - 1] = ht_len[group_number - 1] + L
+            # divide the sum of all the length with the number of conductorSamples do get the average value
             for index in self.groups_to_coils[coil_name]:
-                for sample in coil.conductorSamples:
-                    half_turn_length[index-1] = self.optimize_coil_length_with_resistance_meas(sample, original_conductor, dict_sweeper)
+                ht_len[index-1] = ht_len[index-1] / len(coil.conductorSamples)
 
-        # raise Exception if there is still a None value in half_turn_length
-        if not all(item is not None for item in half_turn_length):
-            raise Exception('Something went wrong when calculating the half_turn_length. Not every list entry could be calculated.')
-
-        # add the list to the sweeper dict as a string
-        dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in half_turn_length) + ']'  # TODO test if this works with ParsimSweeper in AnalysisSTEAM
-
-    # TODO correction factor strand twist-pitch: f_twist_pitch = sqrt(wBare^2+(Lp_s/2)^2)/(Lp_s/2) , where w=wBare cable width, Lp_s=strand twist-pitch; if set to 2, take into account the increases of electrical resistance, ohmic loss per unit length, inter-filament and inter-strand coupling loss per unit length, and fractions of superconductor and stabilizer in the cable bare cross-section due to strand twist-pitch (default=0)
-    # R = C_rho_Cu_NIST_fit with the coil_resistance_room_T, T_ref_coil_resistance and RRR (between 273 and 4) - most people take between RT and 4K
-
-
-    # def optimize_coil_length_with_resistance_meas(self, conductor_sample, conductor_samples, weight_factors, original_conductor):
-    #     # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-    #     bare_cable_width = getattr_from_list(conductor_samples, 'bare_cable_width', weight_factors=weight_factors)
-    #     if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
-    #
-    #     f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, conductor_samples, original_conductor)
-    #
-    #     # get number of half turns from map2d file if present
-    #     if self.model_data.Sources.magnetic_field_fromROXIE:
-    #         path_map2d = self.model_data.Sources.magnetic_field_fromROXIE
-    #         number_of_ht, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d) # TODO test this in AnalysisSTEAM
-    #     else:
-    #         number_of_ht = self.model_data.CoilWindings.n_half_turn_in_group
-    #
-    #     # define function to solve
-    #     def resistance_as_function_of_L(L, *args):
-    #         fCu, A_cond, temperature, mag_field, RRR, Tup_RRR  = args  # unpack arguments
-    #         rho_parameters = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
-    #         matpath = os.path.dirname(steammaterials.__file__)
-    #         CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', rho_parameters.shape[0], rho_parameters.shape[1], matpath)
-    #         rho = CFUN_rhoCuNIST.evaluate(rho_parameters)[0]
-    #         return rho * L / (fCu * A_cond) * f_twist_pitch  # TODO solve it analytically
-    #
-    #     # define parameters needed for function
-    #     fCu = conductor_sample.Cu_noCu_resistance_meas / (1 + conductor_sample.Cu_noCu_resistance_meas)  # TODO if not present modeldata
-    #     key_RRR = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].strand.RRR'
-    #     if key_RRR in dict_sweeper:
-    #         RRR = dict_sweeper[key_RRR]  # use RRR from database - if not existing use modelData
-    #         Tup_RRR  = ...#TODO Cond.T_ref_RRR_high if not use 293.0
-    #     else:
-    #         if not original_conductor.strand.RRR: raise Exception('TODO')
-    #         if not original_conductor.strand.T_ref_RRR_high: raise Exception('TODO')
-    #         RRR = original_conductor.strand.RRR
-    #         Tup_RRR = original_conductor.strand.T_ref_RRR_high
-    #     A_cond = calc_strand_area(strand_geometry=conductor_sample.strand_geometry, original_conductor=original_conductor) # TODO is this right? * n_strands
-    #     temperature = ...#TODO Cond.coil_resistance_room_T if not 293.0  # TODO
-    #     mag_field = 0
-    #       # TODO if measured find in column
-    #
-    #     # solve equation for magnetic length
-    #     args = (fCu, A_cond, temperature, mag_field, RRR, Tup_RRR)
-    #     if self.model_data.GeneralParameters.magnetic_length:
-    #         initial_guess = [self.model_data.GeneralParameters.magnetic_length]
-    #     else: initial_guess = [10]
-    #     L = fsolve(func=resistance_as_function_of_L, x0=initial_guess, args=args)
-    #     L_ht = L[0] / number_of_ht
-    #     return L_ht
-    #
-    def calculate_f_twist_pitch(self, conductor_sample, dict_sweeper, original_conductor):
-        # get the bare_cable_width from the database if it has been changed, if not: use the default one from model_data
-        key_bare_cable_width = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].cable.bare_cable_width'
-        if key_bare_cable_width in dict_sweeper:
-            bare_cable_width = dict_sweeper[key_bare_cable_width]
+        # if half_turn_length from modelData has correct length, and some values in ht_len were calculated, combine the 2
+        ht_len_modelData = self.model_data.CoilWindings.half_turn_length
+        if ht_len_modelData and len(ht_len_modelData) == self.number_of_groups and any(l != 0.0 for l in ht_len):
+            # use the values from modelData if no value could be calculated
+            ht_len = [ht_len_modelData[i] if ht_len[i] == 0.0 else ht_len[i] for i in range(len(ht_len))]
+
+        # if some values could not be calculated or been taken from modeldata, inform the user that calculation was skipped
+        if any(l in [None, 0.0] for l in ht_len):
+            warnings.warn(f'Length optimization was skipped. Not all ht lengths could be calculated from measurements or read from modelData.')
         else:
-            bare_cable_width = original_conductor.cable.bare_cable_width
+            # add the list to the sweeper dict as a string
+            dict_sweeper[f'CoilWindings.half_turn_length'] = '[' + ', '.join(str(x) for x in ht_len) + ']'
 
-        # get the strand_twist_pitch from the database if it has been changed, if not: use the default one from model_data
-        key_strand_twist_pitch = f'Conductors[{conductor_sample.index_of_conductor_in_modelData}].cable.strand_twist_pitch'
-        if key_strand_twist_pitch in dict_sweeper:
-            strand_twist_pitch = dict_sweeper[key_strand_twist_pitch]
-        else:
-            strand_twist_pitch = original_conductor.cable.strand_twist_pitch
-            
-        # calculate correction factor strand twist-pitch
-        f_twist_pitch = np.sqrt(bare_cable_width ** 2 + (strand_twist_pitch / 2) ** 2) / (strand_twist_pitch / 2)  # TODO should be around 1.03-1.05
-        return f_twist_pitch
+    def __optimize_coil_length_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
+                                                    original_conductor: Conductor, coil: Coil):
+        """
+        Optimizes the coil length using the room temperature resistance measurements using the formula:
+        R_RT = rho * L / (fCu * A_cond) * f_twist_pitch -> solving for length L
+
+        :param conductor_sample: A ConductorSample object containing sample data for the conductor
+        :param coil_name: The name of the coil
+        :param original_conductor: The original conductor object, needed for getting parameters if they are not beeing changed, meaning not present in conductor_sample
+        :param coil: The Coil object to get the RT resistance measurement values
+        """
 
+        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+        bare_cable_width = conductor_sample.width
+        if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
+        if not bare_cable_width: raise Exception('Could not find bare cable width in conductor database and in original conductor.')
+        strand_twist_pitch = conductor_sample.strand_twist_pitch
+        if not strand_twist_pitch: strand_twist_pitch = original_conductor.cable.strand_twist_pitch
+        if not strand_twist_pitch: raise Exception('Could not find strand twist pitch in conductor database and in original conductor.')
+        f_twist_pitch = np.sqrt(bare_cable_width ** 2 + (strand_twist_pitch / 2) ** 2) / (strand_twist_pitch / 2)
+
+        # get number of half turns from map2d file if present, else check in modelData
+        number_of_hts = self.__read_num_ht_per_group()
+        number_of_ht = sum([number_of_hts[i-1] for i in self.groups_to_coils[coil_name]])  # add all the halfturns for the coil together
+
+        # define needed parameters - check if they are present in sample and if not use default values form in modelData
+        R_RT = coil.coil_resistance_room_T
+        if not R_RT: raise Exception(f'No room temperature measurement provided for coil {coil_name}')
+        Cu_noCu = coil.Cu_noCu_resistance_meas
+        if not Cu_noCu: Cu_noCu = conductor_sample.Cu_noCu
+        if not Cu_noCu: Cu_noCu = original_conductor.strand.Cu_noCu_in_strand
+        if not Cu_noCu: raise Exception('Could not find copper-non-copper-ratio in conductor database (nor general nor measurement specific) and in original conductor.')
+        fCu = Cu_noCu / (1+Cu_noCu)
+        A_strand = calc_strand_area(conductor_sample.strand_geometry, original_conductor)
+        n_strands = conductor_sample.number_of_strands
+        if not n_strands: n_strands = original_conductor.cable.n_strands
+        if not n_strands: Exception('Could not find number of strands in conductor database and in original conductor.')
+        A_cond = A_strand * n_strands
+
+        # calculate rho with c function
+        temperature = coil.T_ref_coil_resistance
+        if not temperature: temperature = 293.0
+        mag_field = coil.B_resistance_meas
+        if not mag_field: mag_field = 0.0
+        RRR = conductor_sample.RRR
+        if not RRR: RRR = original_conductor.strand.RRR
+        if not RRR: raise Exception('Could not find RRR in conductor database and in original conductor.')
+        Tup_RRR = coil.T_ref_RRR_high
+        if not Tup_RRR: Tup_RRR = original_conductor.strand.T_ref_RRR_high
+        if not Tup_RRR: Tup_RRR = 293.0
+        rho_param = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+        CFUN_path = os.path.dirname(steammaterials.__file__)  # get path to steam materials library
+        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', rho_param.shape[0], rho_param.shape[1], CFUN_path)
+        rho = CFUN_rhoCuNIST.evaluate(rho_param)[0]  # evaluate rho function with the parameters
+
+        # calculate the length
+        L = R_RT * fCu * A_cond / (rho * f_twist_pitch)
+        L_ht = L / number_of_ht
+        return L_ht
 
-    def __write_parsweep_conductors(self, dict_sweeper, flag_optimize_fCu: bool):
+    def __read_num_ht_per_group(self):
         """
-        Writes the Conductor parameter for a sweeper csv file to a dict.
+        Reads the number of half-turns per group either from the map2d file or from the model_data's CoilWindings attribute.
+        If neither is available, raises an exception.
+
+        :return: A list containing the number of half-turns for each group.
+        """
+        if self.model_data.Sources.magnetic_field_fromROXIE:
+            path_map2d = Path(self.path_input_dir, self.model_data.Sources.magnetic_field_fromROXIE).resolve()
+            # number_of_ht has as many elements as groups. Each element defines the number of half-turns in that group
+            number_of_hts, _, _, _, _, _, _, _ = getParametersFromMap2d(map2dFile=path_map2d)
+            if len(number_of_hts) != self.number_of_groups: raise Exception(
+                f'The number of groups given to ParsimConductor ({self.number_of_groups}) is different then the number of groups specified in the map2d file "{path_map2d}" ({len(number_of_hts)})')
+        else:
+            number_of_hts = self.model_data.CoilWindings.n_half_turn_in_group
+            if not number_of_hts: raise Exception(
+                'Number of half turns per group could not be specified. CoilWindings.n_half_turn_in_group is empty in modelData.')
+            if len(number_of_hts) != self.number_of_groups: raise Exception(
+                'The number of groups given to ParsimConductor is different then the length of CoilWindings.n_half_turn_in_group in modelData.')
+        return number_of_hts
 
-        Parameters:
-        - dict_sweeper (dict): input dict where the sweeper entries will be stored  int the format {columnName: value}
-        - flag_optimize_fCu (bool): TODO
+    def __write_parsweep_conductors(self, dict_sweeper: Dict[str, Any], flag_optimize_fCu: bool, rel_warning_limit: float):
+        """
+        Writes the Conductor parameters for a sweeper CSV file to a dictionary.
 
+        :param dict_sweeper: The input dictionary where the sweeper entries will be stored in the format {attributeNameDataModelMagnet: newValue}.
+        :param flag_optimize_fCu: If set to True, fCu will be optimized with the coil resistance measurement at room temperature.
+        :param rel_warning_limit: function raises warning in console when values are changed for more/less then this relative value
         """
         # parameter dict for creating the column names of sweeper csv file
         dict_param = {
             # format {attribute_name_of_ConductorSample_object: attribute_name_of_Conductor_from_DataModelMagnet_object}
             'strand_geometry.diameter': 'strand.diameter',
             'strand_geometry.bare_width': 'strand.bare_width',
             'strand_geometry.bare_height': 'strand.bare_height',
+            'width': 'cable.width_core',  # TODO: is this correct? or bare_cable_width?
+            'height': 'cable.height_core',  # TODO: is this correct?
+            'f_rho_eff': 'strand.f_Rho_effective',
+            'Ra': 'cable.Ra',
+            'Rc': 'cable.Rc',
             'RRR': 'strand.RRR',
+            'Bc20': 'Jc_fit.Tc0_CUDI1',
+            'Tc0': 'Jc_fit.Bc20_CUDI1',
+            'number_of_strands': 'cable.n_strands',
             'Cu_noCu': 'strand.Cu_noCu_in_strand',
             'width': 'cable.bare_cable_width',
             'filament_twist_pitch': 'strand.fil_twist_pitch',
             'strand_twist_pitch': 'cable.strand_twist_pitch',
-# TODO name the attribute_name_of_ConductorSample_object identical to attribute_name_of_Conductor_from_DataModelMagnet_object to not need this dict?
         }
 
         # looping through the coil list
         for coil_name, coil in self.data_parsim_conductor.Coils.items():
             idx = self.dict_coilName_to_conductorIndex[coil_name]
             sweeper_cond_name = f'Conductors[{idx}].'
 
@@ -430,330 +526,281 @@
                     # append value to sweeper dict
                     dict_sweeper[sweeper_cond_name + conductor_attribute_name] = val
 
             # insert Jc fit value(s) depending on their fitting function (usual Bottura, CUDI1, CUDI3 for NbTi and Summers, Bordini for Nb3Sn)
             Jc_dict_list = []
             for conductor_sample in coil.conductorSamples:
                 # calculate the parameters for Jc fit for every conductor sample of this coil
-                Jc_dict = get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], coil_name=coil_name,
+                Jc_dict = self.__get_Jc_fit_params(original_conductor=self.model_data.Conductors[idx], coil_name=coil_name,
                                   strand_geometry=conductor_sample.strand_geometry, Bc20=conductor_sample.Bc20,
-                                  Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0)
+                                  Ic_measurements=conductor_sample.Ic_measurements, Tc0=conductor_sample.Tc0,
+                                  n_strand=conductor_sample.number_of_strands, Cu_nCu=conductor_sample.Cu_noCu)
                 Jc_dict_list.append(Jc_dict)
             # Calculate the average of values for each key across all dictionaries in the list
-            Jc_avg_dict = {key: sum(d[key] for d in Jc_dict_list) / len(Jc_dict_list) for key in Jc_dict_list[0]}
+            Jc_avg_dict = average_dicts(Jc_dict_list)
             for name, val in Jc_avg_dict.items():
-                if val: dict_sweeper[sweeper_cond_name + 'Jc_fit.' + name] = val
+                dict_sweeper[sweeper_cond_name + 'Jc_fit.' + name] = val
 
             # optimize the fraction of copper with the resistance measurement at room temperature
-            # if flag_optimize_fCu:
-                # list_optimized_Cu_noCu = []
-                # for conductor_sample in coil.conductorSamples:
-                #     list_optimized_Cu_noCu.append(self.optimize_fCu_with_resistance_meas(coil.conductorSamples, self.model_data.Conductors[idx], dict_sweeper))
-                # dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = val
-
-    def optimize_fCu_with_resistance_meas(self, conductor_samples, original_conductor, dict_sweeper):
-        # # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
-        # f_twist_pitch = self.calculate_f_twist_pitch(conductor_sample, dict_sweeper, original_conductor)
-        #
-        # # define function to solve
-        # def resistance_as_function_of_fCu(fCu, *args):
-        #     L, A_cond, temperature, mag_field, RRR, RRR_ref = args  # unpack arguments
-        #     numpy2d = np.vstack((temperature, mag_field, RRR, RRR_ref))  # create parameter v stack for c function
-        #     matpath = os.path.dirname(steammaterials.__file__)
-        #     CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', numpy2d.shape[0], numpy2d.shape[1], matpath)
-        #     rho = CFUN_rhoCuNIST.evaluate(numpy2d)  # TODO check dimension (1x1 array)
-        #     return rho * L / (fCu * A_cond) * f_twist_pitch
-        #
-        # # solve equation for fraction of Copper
-        # args = (1, 0.2, 273, 0, 100, 1)  # TODO: copy from optimize_L_with_resistance_meas if working
-        # if original_conductor.strand.Cu_noCu_in_strand:
-        #     initial_guess = [original_conductor.strand.Cu_noCu_in_strand]
-        # else: initial_guess = [0.1]
-        # fCu = fsolve(func=resistance_as_function_of_fCu, x0=initial_guess, args=args)
-        # Cu_noCu = fCu[0] / (1 - fCu[0])
-        # if Cu_noCu < 0.01:
-        #     Cu_noCu = 0.01  # TODO delete this and find cause of problem
-        # return Cu_noCu
-        pass
-
-
-def get_Jc_fit_params(original_conductor, strand_geometry, Tc0, Bc20, Ic_measurements, coil_name):
-    # TODO: use C-python-wrapper functions(see steam-materials-library) - ask Mariusz how to set it up (when it is implemented)
-    if original_conductor.Jc_fit.type == 'Summers':
-        # check inputs
-        if not original_conductor.strand.type: raise Exception(
-            f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
-        if len(Ic_measurements) > 1:
-            # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
-            raise Exception(
-                f'More then one Measurement for Summers fit provided for coil {coil_name}. Please only provide 1 or 0.')
-        elif len(Ic_measurements) < 1:
-            warnings.warn(
-                f'No Measurement for Summers fit provided for coil {coil_name}. Calculation of new Summers parameters will be skipped.')
-            return {}
-        else:
-            Ic_measurement = Ic_measurements[0]
-            if not Ic_measurement.Ic: raise Exception(
-                f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not Ic_measurement.B_ref_Ic: raise Exception(
-                f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
-            if not Ic_measurement.T_ref_Ic: raise Exception(
-                f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
-            if not Ic_measurement.Cu_noCu_sample: raise Exception(
-                f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-
-        # use parameters of modelData if they are not changed with the conductor database
-        if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_Summers
-        if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_Summers
-
-        # calculate critical current density from critical current by using the area of
-        fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample + 1)
-        A = calc_strand_area(strand_geometry, original_conductor)
-        A_noCu = A * (1 - fCu)
-        Jc_Tref_Bref = Ic_measurement.Ic / A_noCu
-
-        # search for the best C0  # TODO use np.linalg.solve?
-        tol = 1e-6  # hardcoded
-        if original_conductor.Jc_fit.Jc0_Summers:
-            val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
-            print(val_range)
-        else:
-            val_range = [1e6, 1e14]
-        n_iterations = math.ceil(
-            np.log((val_range[1] - val_range[0]) / tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
-        for _ in range(n_iterations):
-            try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
-            tryJc_Summers = np.zeros(len(try_CO_Summers))
-            # calculate Jc for every selected C0 value
-            for j in range(len(try_CO_Summers)):
-                tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic,
-                                                       try_CO_Summers[j], Tc0, Bc20)
-            # find indices of the list values that are higher than Jc_Tref_Bref
-            tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
-            if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
-            # set new value range for net iteration
-            val_range = [try_CO_Summers[tempIdx[0] - 1], try_CO_Summers[tempIdx[0]]]
-            C0 = try_CO_Summers[tempIdx[0] - 1]
-
-        return {
-            'Jc0_Summers': C0,
-            'Tc0_Summers': Tc0,
-            'Bc20_Summers': Bc20,
-        }
-    elif original_conductor.Jc_fit.type == 'Bordini':
-        # TODO use C-function when wrapper is available
-        return {
-            'C0_Bordini': todo(),
-            'alpha_Bordini': todo(),
-            'Tc0_Bordini': todo(),
-            'Bc20_Bordini': todo(),
-        }
-    elif original_conductor.Jc_fit.type == 'CUDI1':
-        # general equation for CUDI1: Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59)
+            if flag_optimize_fCu:
+                # check if RT measurement is defined
+                if not coil.coil_resistance_room_T:
+                    warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database.')
+                    continue
+                # calculate Cu_noCu for every conductor sample and use mean value
+                list_optimized_Cu_noCu = []
+                for sample in coil.conductorSamples:
+                    list_optimized_Cu_noCu.append(self.__optimize_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx], coil))
+                dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = np.mean(list_optimized_Cu_noCu)
 
-        # depending on the number of critical current measurements, use different ways to calculate C1 and C2 parameter
-        if len(Ic_measurements) not in [0, 1, 2]:
-            # TODO we could solve the overdetermined system of equations with Least Squares algorithms, like numpy.linalg.lstsq
-            raise Exception(
-                f'More then two measurements for CUDI1 fit provided in coil {coil_name}. Please only provide 2, 1 or 0 measurements.')
-        elif len(Ic_measurements) == 2:
-            # if two measurements are specified, we have 2 equations and 2 unknowns -> system can be solved
-
-            # check inputs and use parameters of modelData if they are not changed with the conductor database
-            for Ic_measurement in Ic_measurements:
-                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-                # if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not original_conductor.cable.n_strands: raise Exception(
-                'No number of strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception(
-                'No Tc0 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception(
-                'No Bc02 specified in modelData of the conductor that should be changed.')
-            if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
-            if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
-
-            # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable1 = Ic_measurements[0].Ic  # TODO * original_conductor.cable.n_strands
-            Ic_cable2 = Ic_measurements[1].Ic  # TODO * original_conductor.cable.n_strands
-
-            # # # solve system of linear equations: A*x = b - redundant way
-            # A = np.array([[1, Ic_measurements[0].B_ref_Ic], [1, Ic_measurements[1].B_ref_Ic]])
-            # b_1 = Ic_cable1 / (1 - Ic_measurements[0].T_ref_Ic / Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** -0.59)
-            # b_2 = Ic_cable2 / (1 - Ic_measurements[1].T_ref_Ic / Tc0 * (1 - Ic_measurements[1].B_ref_Ic / Bc20) ** -0.59)
-            # b = np.array([b_1, b_2])
-            # x = np.linalg.solve(A, b,)
-
-            def CUDI1_equation_fixed_ratio(C, *args):
-                C1, C2 = C
-                Ic1, Ic2, T1, T2, Tc0, B1, B2, Bc20 = args
-
-                eq1 = Ic1 - (C1 + C2 * B1) * (1 - T1 / (Tc0 * (1 - B1 / Bc20) ** 0.59))
-                eq2 = Ic2 - (C1 + C2 * B2) * (1 - T2 / (Tc0 * (1 - B2 / Bc20) ** 0.59))
-
-                return [eq1, eq2]
-
-            initial_values = [787.327,
-                              -63.073]  # values come from magnet "MQML" in csv file "Strand and cable characteristics"
-            args = (Ic_cable1, Ic_cable2, Ic_measurements[0].T_ref_Ic, Ic_measurements[1].T_ref_Ic, Tc0,
-                    Ic_measurements[0].B_ref_Ic, Ic_measurements[1].B_ref_Ic, Bc20)
-            x = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_values, args=args)
+    def __optimize_fCu_with_resistance_meas(self, conductor_sample: ConductorSample, coil_name: str,
+                                            original_conductor: Conductor, coil: Coil):
+        """
+        Optimizes the fraction of copper (fCu) using the room temperature resistance measurements using the formula:
+        R_RT = rho * L / (fCu * A_cond) * f_twist_pitch -> solving for fCu
 
-            if len(x) == 2:
-                C1, C2 = x
-            else:
-                raise Exception(
-                    f'No valid solution for CUDI1 fitting parameters C1 and C2 could be found for coil {coil_name}.')
-        elif len(Ic_measurements) == 1:
-            # if only one measurement is provided use one equation and the ratio of C1 and C2 according to modelData and warn the user
-            warnings.warn(
-                f'Only one Measurement for CUDI1 fit provided for coil {coil_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
-
-            # check inputs and use parameters of modelData if they are not changed with the conductor database
-            if not Ic_measurements[0].Ic: raise Exception(
-                f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not Ic_measurements[0].B_ref_Ic: raise Exception(
-                f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-            if not Ic_measurements[0].T_ref_Ic: raise Exception(
-                f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
-            # if not Ic_measurements[0].Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-            if not original_conductor.cable.n_strands: raise Exception(
-                'No number of strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Tc0_CUDI1: raise Exception(
-                'No Tc0 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.Bc20_CUDI1: raise Exception(
-                'No Bc02 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.C1_CUDI1: raise Exception(
-                'No C1_CUDI1 specified in modelData of the conductor that should be changed.')
-            if not original_conductor.Jc_fit.C2_CUDI1: raise Exception(
-                'No C2_CUDI1 specified in modelData of the conductor that should be changed.')
-            if not Tc0: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
-            if not Bc20: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
-
-            # convert critical current of strand to critical current of conductor by multiplying with number of strands
-            Ic_cable = Ic_measurements[
-                0].Ic  # TODO why delete this "* original_conductor.cable.n_strands" - in csv we only use n_strands=1
-
-            # try to read C1 over C2 ratio from modelData - if not existing use usual ratio for NbTi superconductors
-            if not original_conductor.Jc_fit.C1_CUDI1 or not original_conductor.Jc_fit.C2_CUDI1:
-                warnings.warn(
-                    f'No C1 or C2 parameter defined in modelData for coil {coil_name}. Using usual ratio for NbTi superconductors.')
-                # 787.327 and -63.073 are hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
-                # saving signed angle instead of ratio to keep track of signs - tan(angle_C1_C2) = C1/C2
-                angle_C1_C2 = math.atan2(787.327,
-                                         -63.073)  # atan2 is a tangens calcualtion that also saves the sign of the angle depending on the quadrant
-                initial_guess = [787.327, -63.073]
-            else:
-                angle_C1_C2 = math.atan2(original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1)
-                initial_guess = [original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1]
+        :param conductor_sample: A ConductorSample object containing sample data for the conductor
+        :param coil_name: The name of the coil
+        :param original_conductor: The original conductor object, needed for getting parameters if they are not being changed, meaning not present in conductor_sample
+        :param coil: The Coil object to get the RT resistance measurement values
+        """
 
-            def CUDI1_equation_fixed_ratio(C, *args):
-                C1, C2 = C
-                Ic, T, Tc0, B, Bc20, angle_C1_C2 = args
-
-                eq1 = Ic - (C1 + C2 * B) * (1 - T / (Tc0 * (1 - B / Bc20) ** 0.59))
-                eq2 = C1 - C2 * math.tan(angle_C1_C2)
-
-                return [eq1, eq2]
-
-            # Solve the equation system
-            args = (Ic_cable, Ic_measurements[0].T_ref_Ic, Tc0, Ic_measurements[0].B_ref_Ic, Bc20, angle_C1_C2)
-            C = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_guess, args=args)
-            C1, C2 = C[0], C[1]
-
-            # old approach with analytical solution
-            # # Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59) where only C1 and C2 are unknown - second equation: tan(angle_C1_C2) = C1/C2
-            # C2 = Ic_cable / (1 - Ic_measurements[0].T_ref_Ic / (Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** 0.59)) / (Ic_measurements[0].B_ref_Ic + math.tan(angle_C1_C2))
-            # C1 = C2 * math.tan(angle_C1_C2)
-        elif len(Ic_measurements) == 0:
-            # if no measurement is provided use the usual ratio for NbTi superconductors and scale that value by cross section of superconductor and warn the user
-            warnings.warn(
-                f'No Measurement for CUDI1 fit provided for coil {coil_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
+        # calculate correction factor strand twist-pitch with bare cable width and strand twist pitch
+        bare_cable_width = conductor_sample.width
+        if not bare_cable_width: bare_cable_width = original_conductor.cable.bare_cable_width
+        if not bare_cable_width: raise Exception('Could not find bare cable width in conductor database and in original conductor.')
+        strand_twist_pitch = conductor_sample.strand_twist_pitch
+        if not strand_twist_pitch: strand_twist_pitch = original_conductor.cable.strand_twist_pitch
+        if not strand_twist_pitch: raise Exception('Could not find strand twist pitch in conductor database and in original conductor.')
+        f_twist_pitch = np.sqrt(bare_cable_width ** 2 + (strand_twist_pitch / 2) ** 2) / (strand_twist_pitch / 2)
+
+        # define needed parameters - check if they are present in sample and if not use default values form in modelData
+        L_coil = self.length_to_coil[coil_name]
+        R_RT = coil.coil_resistance_room_T
+        if not R_RT: raise Exception(f'No room temperature measurement provided for coil {coil_name}')
+        A_strand = calc_strand_area(conductor_sample.strand_geometry, original_conductor)
+        n_strands = conductor_sample.number_of_strands
+        if not n_strands: n_strands = original_conductor.cable.n_strands
+        if not n_strands: raise Exception('Could not find number of strands in conductor database and in original conductor.')
+        A_cond = A_strand * n_strands
+
+        # calculate rho with c function
+        temperature = coil.T_ref_coil_resistance
+        if not temperature: temperature = 293.0
+        mag_field = coil.B_resistance_meas
+        if not mag_field: mag_field = 0.0
+        RRR = conductor_sample.RRR
+        if not RRR: RRR = original_conductor.strand.RRR
+        if not RRR: raise Exception('Could not find RRR in conductor database and in original conductor.')
+        Tup_RRR = coil.T_ref_RRR_high
+        if not Tup_RRR: Tup_RRR = original_conductor.strand.T_ref_RRR_high
+        if not Tup_RRR: Tup_RRR = 293.0
+        rho_param = np.vstack((temperature, mag_field, RRR, Tup_RRR))  # create parameter v stack for c function
+        CFUN_path = os.path.dirname(steammaterials.__file__)  # get path to steam materials library
+        CFUN_rhoCuNIST = STEAM_materials('CFUN_rhoCuNIST', rho_param.shape[0], rho_param.shape[1], CFUN_path)
+        rho = CFUN_rhoCuNIST.evaluate(rho_param)[0]  # evaluate rho function with the parameters
+
+        # calculte fCu
+        fCu = L_coil * rho * f_twist_pitch / (R_RT * A_cond)
+        Cu_noCu_new = fCu / (1 - fCu)
+
+        # compare new value with old one
+        Cu_noCu_old = coil.Cu_noCu_resistance_meas
+        if not Cu_noCu_old: Cu_noCu_old = conductor_sample.Cu_noCu
+        if not Cu_noCu_old: Cu_noCu_old = original_conductor.strand.Cu_noCu_in_strand
+        if self.verbose: print(f'Copper-non-Copper-ratio optimized form {Cu_noCu_old} to {Cu_noCu_new}.')
 
-            # check inputs
-            if not original_conductor.cable.n_strands: raise Exception(
-                'No n_strands specified in modelData of the conductor that should be changed.')
-            if not original_conductor.strand.Cu_noCu_in_strand: raise Exception(
-                'No n_strands specified in modelData of the conductor that should be changed.')
-
-            # hardcoded values come from magnet "MQML" in csv file "Strand and cable characteristics"
-            # NOTE: cab...cable, str...strand, C1_cab = C1_str * nStrands  and  C1_str = C1_str_MB / A_MB * A_thisMagnet
-            C1_per_square_meter_of_NbTi = 787.327 / 6.580e-08  # C1_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
-            C2_per_square_meter_of_NbTi = -63.073 / 6.580e-08  # C2_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu)
-
-            # scale it with the cross-section of superconductor
-            strand_cross_section = calc_strand_area(strand_geometry, original_conductor)
-            fraction_of_superconductor = 1 / (original_conductor.strand.Cu_noCu_in_strand + 1)
-            total_NbTi_area = fraction_of_superconductor * strand_cross_section  # TODO why do i have to delete this? "* original_conductor.cable.n_strands" (AH97)
-            C1 = C1_per_square_meter_of_NbTi * total_NbTi_area
-            C2 = C2_per_square_meter_of_NbTi * total_NbTi_area
-
-        # check if values are real and not imaginary (e.g. when Bc20 is bigger than B_ref_Ic)
-        if np.iscomplex(complex(C1)) or np.iscomplex(complex(C2)):
-            raise Exception(
-                f'When calculating CUDI1 parameters (C1, C2) the values turned out to have an imaginary part. Please check the inputs.')
-
-        return {
-            # TODO: shall we add a plausibility check - e.g. if the value will be changed by many orders of magnitude
-            'Tc0_CUDI1': Tc0,
-            'Bc20_CUDI1': Bc20,
-            'C1_CUDI1': C1,
-            'C2_CUDI1': C2,
-        }
-    else:
-        raise Exception(
-            f'No implementation for fit type "{original_conductor.Jc_fit.type}" defined in ParsimConductor.')
+        # calculate fCu
+        return Cu_noCu_new
+    
+    def __get_Jc_fit_params(self, original_conductor: Conductor, strand_geometry: StrandGeometry, n_strand: int,
+                            Cu_nCu: float, Tc0: float, Bc20: float, Ic_measurements: List[IcMeasurement], coil_name: str):
+        """
+        Calculate Jc fit parameters for a coil based using the variables to change, the original conductor's properties
+        and the provided critical current measurements.
 
+        :param original_conductor: The original conductor object, needed for getting parameters if they are not being changed, meaning not present in conductor_sample
+        :param strand_geometry: geometry of the conductor sample
+        :param n_strand: number of strands
+        :param Cu_nCu: copper non copper ratio
+        :param Tc0: Tc0 parameter for Jc fitting function
+        :param Bc20: Bc20 parameter for Jc fitting function
+        :param Ic_measurements: list of critical current measurements for this conductorSample
+        :param coil_name: name of the coil
 
-def calc_C0_summers(new_conductor, original_conductor, coil_name):
-    # check inputs
-    Ic_measurement = new_conductor.Ic_measurements[0]
-    if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-    if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
-    if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
-    if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
-
-    # use parameters of modelData if they are not changed with the conductor database
-    Tc0 = new_conductor.Tc0  # TODO should this be done like this with Tc0, or shall i take the avg before the calculation?
-    Bc20 = new_conductor.Bc20
-    if not Tc0:
-        Tc0 = original_conductor.Jc_fit.Tc0_Summers
-    if not Bc20:
-        Bc20 = original_conductor.Jc_fit.Bc20_Summers
-
-    # calculate critical current density from critical current
-    fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample + 1)
-    A = calc_strand_area(new_conductor.strand_geometry, original_conductor)
-    A_noCu = A * (1 - fCu)
-    Jc_Tref_Bref = Ic_measurement.Ic / A_noCu
-
-    # search for the best C0  # TODO use np.linalg.solve or method to use Jc c-func more easily
-    tol = 1e-6  # hardcoded
-    if original_conductor.Jc_fit.Jc0_Summers:
-        val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
-        print(val_range)
-    else:
-        val_range = [1e6, 1e14]
-    n_iterations = math.ceil(
-        np.log((val_range[1] - val_range[0]) / tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
-    for _ in range(n_iterations):
-        try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
-        tryJc_Summers = np.zeros(len(try_CO_Summers))
-        # calculate Jc for every selected C0 value
-        for j in range(len(try_CO_Summers)):
-            tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic, try_CO_Summers[j], Tc0, Bc20)
-        # find indices of the list values that are higher than Jc_Tref_Bref
-        tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
-        if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
-        # set new value range for net iteration
-        val_range = [try_CO_Summers[tempIdx[0] - 1], try_CO_Summers[tempIdx[0]]]
-        C0 = try_CO_Summers[tempIdx[0] - 1]
-    return C0
+        returns: dictionary containing the calculated Jc fit parameters in format {attributeNameJcInDataModelMagnet: value}
+        """
+        Jc_dict = {}
+        # TODO: use C-python-wrapper functions(see steam-materials-library) when implemented
+        if original_conductor.Jc_fit.type == 'Summers':
+            # check inputs
+            if not original_conductor.strand.type: raise Exception(f'Strand type of conductor in coil {coil_name} is not specified in modelData.')
+            if len(Ic_measurements) > 1:
+                raise Exception(f'More then one Measurement for Summers fit provided for coil {coil_name}. Please only provide 1 or 0.')
+            elif len(Ic_measurements) < 1:
+                warnings.warn(f'No Measurement for Summers fit provided for coil {coil_name}. Calculation of new Summers parameters will be skipped.')
+                return {}
+            else:
+                Ic_measurement = Ic_measurements[0]
+                if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+                if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for Summers fit provided for coil {coil_name}.')
+                if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for Summers fit provided for coil {coil_name}.')
+                if not Ic_measurement.Cu_noCu_sample: raise Exception(f'No Cu-nCu-ratio of critical current measurement for Summers fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+    
+            # use parameters of modelData if they are not changed with the conductor database
+            if Tc0:
+                Jc_dict['Tc0_Summers'] = Tc0
+            else: Tc0 = original_conductor.Jc_fit.Tc0_Summers
+            if not Tc0: raise Exception(f'No Tc0 specified in modelData or the conductor database for coil {coil_name}.')
+            if Bc20:
+                Jc_dict['Bc20_Summers'] = Bc20
+            else: Bc20 = original_conductor.Jc_fit.Bc20_Summers
+            if not Bc20: raise Exception(f'No Bc20 specified in modelData or the conductor database for coil {coil_name}.')
+    
+            # calculate critical current density from critical current by using the area of
+            fCu = Ic_measurement.Cu_noCu_sample / (Ic_measurement.Cu_noCu_sample + 1)
+            A = calc_strand_area(strand_geometry, original_conductor)
+            A_noCu = A * (1 - fCu)
+            Jc_Tref_Bref = Ic_measurement.Ic / A_noCu
+    
+            # search for the best C0  # TODO use CFUN when available
+            tol = 1e-6  # hardcoded
+            if original_conductor.Jc_fit.Jc0_Summers:
+                val_range = [original_conductor.Jc_fit.Jc0_Summers / 1000, original_conductor.Jc_fit.Jc0_Summers * 1000]
+            else:
+                val_range = [1e6, 1e14]
+            n_iterations = math.ceil(np.log((val_range[1] - val_range[0]) / tol) / np.log(10))  # from formula: width/(10**n_iterations) = tol
+            C0 = None
+            for _ in range(n_iterations):
+                try_CO_Summers = np.linspace(val_range[0], val_range[1], 10)
+                tryJc_Summers = np.zeros(len(try_CO_Summers))
+                # calculate Jc for every selected C0 value
+                for j in range(len(try_CO_Summers)):
+                    tryJc_Summers[j] = Jc_Nb3Sn_Summer_new(Ic_measurement.T_ref_Ic, Ic_measurement.B_ref_Ic, try_CO_Summers[j], Tc0, Bc20)
+                # find indices of the list values that are higher than Jc_Tref_Bref
+                tempIdx = np.where(np.array(tryJc_Summers) >= Jc_Tref_Bref)[0]
+                if len(tempIdx) == 0: raise Exception('No C0 for Jc Summers fit could be found in specified value range.')
+                # set new value range for net iteration
+                val_range = [try_CO_Summers[tempIdx[0] - 1], try_CO_Summers[tempIdx[0]]]
+                C0 = try_CO_Summers[tempIdx[0] - 1]
+    
+            Jc_dict['Jc0_Summers'] = C0
+    
+            return Jc_dict
+        # elif original_conductor.Jc_fit.type == 'Bordini':
+        #     # TODO use C-function when wrapper is available
+        #     Jc_dict['C0_Bordini'] = 0
+        #     Jc_dict['alpha_Bordini'] = 0
+        #     Jc_dict['Tc0_Bordini'] = 0
+        #     Jc_dict['Bc20_Bordini'] = 0
+        #     return Jc_dict
+        elif original_conductor.Jc_fit.type == 'CUDI1':
+            # general equation for CUDI1: Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59)
+    
+            # use parameters of modelData if they are not changed with the conductor database
+            if Tc0: Jc_dict['Tc0_CUDI1'] = Tc0
+            else: Tc0 = original_conductor.Jc_fit.Tc0_CUDI1
+            if Bc20: Jc_dict['Bc20_CUDI1'] = Bc20
+            else: Bc20 = original_conductor.Jc_fit.Bc20_CUDI1
+            if not n_strand: n_strand = original_conductor.cable.n_strands
+            if not n_strand: raise Exception(f'Number of strands for coil {coil_name} unknown. CUDI parameter calculation not possible.')
+    
+            # depending on the number of critical current measurements, use different ways to calculate C1 and C2 parameter
+            if len(Ic_measurements) == 2:
+                # if two measurements are specified, we have 2 equations and 2 unknowns -> system can be solved
+    
+                # check inputs
+                for Ic_measurement in Ic_measurements:
+                    if not Ic_measurement.Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+                    if not Ic_measurement.B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                    if not Ic_measurement.T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                if not Tc0: raise Exception(f'No Tc0 specified in modelData or the conductor database for coil {coil_name}.')
+                if not Bc20: raise Exception(f'No Bc02 specified in modelData or the conductor database for coil {coil_name}.')
+    
+                # solve system of linear equations: A*x = b
+                A = np.array([[1, Ic_measurements[0].B_ref_Ic], [1, Ic_measurements[1].B_ref_Ic]])
+                b_1 = Ic_measurements[0].Ic / (1 - Ic_measurements[0].T_ref_Ic / Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** -0.59)
+                b_2 = Ic_measurements[1].Ic / (1 - Ic_measurements[1].T_ref_Ic / Tc0 * (1 - Ic_measurements[1].B_ref_Ic / Bc20) ** -0.59)
+                b = np.array([b_1, b_2])
+                x = np.linalg.solve(A, b)
+                C1_str, C2_str = x
+            elif len(Ic_measurements) == 1:
+                # if only one measurement is provided use one equation and the ratio of C1 and C2 according to modelData and warn the user
+                warnings.warn(f'Only one Measurement for CUDI1 fit provided for coil {coil_name}. Ratio of C1 and C2 from modelData is used as a second equation.')
+    
+                # check inputs and use parameters of modelData if they are not changed with the conductor database
+                if not Ic_measurements[0].Ic: raise Exception(f'No measured critical current (Ic) for CUDI1 fit could be found in conductor database for coil {coil_name}. Please check column name in step definition.')
+                if not Ic_measurements[0].B_ref_Ic: raise Exception(f'No reference magnetic field of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                if not Ic_measurements[0].T_ref_Ic: raise Exception(f'No reference temperature of critical current measurement for CUDI1 fit provided for coil {coil_name}.')
+                if not Tc0: raise Exception(f'No Tc0 specified in modelData or the conductor database for coil {coil_name}.')
+                if not Bc20: raise Exception(f'No Bc02 specified in modelData or the conductor database for coil {coil_name}.')
+    
+                # try to read C1 over C2 ratio from modelData - if not existing use usual ratio for NbTi superconductors
+                if not original_conductor.Jc_fit.C1_CUDI1 or not original_conductor.Jc_fit.C2_CUDI1:
+                    print(f'No C1 or C2 parameter defined in modelData for coil {coil_name}. Using usual ratio for NbTi superconductors.')
+                    # 787.327 and -63.073 are hardcoded values come from magnet "MB inner layer" in csv file "Strand and cable characteristics"
+                    # saving signed angle instead of ratio to keep track of signs - tan(angle_C1_C2) = C1/C2
+                    angle_C1_C2 = math.atan2(3448.573, -257.289)  # atan2 is a tangens calcualtion that also saves the sign of the angle depending on the quadrant
+                    initial_guess = [3448.573, -257.289]
+                else:
+                    angle_C1_C2 = math.atan2(original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1)
+                    initial_guess = [original_conductor.Jc_fit.C1_CUDI1, original_conductor.Jc_fit.C2_CUDI1]
+    
+                def CUDI1_equation_fixed_ratio(C, *args):
+                    # function defining the equation system to solve
+                    C1, C2 = C
+                    Ic, T, Tc0, B, Bc20, angle_C1_C2 = args
 
+                    return [Ic - (C1 + C2 * B) * (1 - T / (Tc0 * (1 - B / Bc20) ** 0.59)),
+                            C1 - C2 * math.tan(angle_C1_C2)]
+    
+                # Solve the equation system
+                args = (Ic_measurements[0].Ic, Ic_measurements[0].T_ref_Ic, Tc0, Ic_measurements[0].B_ref_Ic, Bc20, angle_C1_C2)
+                C = fsolve(func=CUDI1_equation_fixed_ratio, x0=initial_guess, args=args)
+                C1_str = C[0]
+                C2_str = C[1]
+    
+                # old approach with analytical solution (not used because of problem with sign of C1&C2)
+                # # Ic = (C1 + C2*B) * (1 - T/Tc0*(1-B/Bc20)^-.59) where only C1 and C2 are unknown - second equation: tan(angle_C1_C2) = C1/C2
+                # C2 = Ic_measurements[0].Ic / (1 - Ic_measurements[0].T_ref_Ic / (Tc0 * (1 - Ic_measurements[0].B_ref_Ic / Bc20) ** 0.59)) / (Ic_measurements[0].B_ref_Ic + math.tan(angle_C1_C2))
+                # C1 = C2 * math.tan(angle_C1_C2)
+            elif len(Ic_measurements) == 0:
+                # if no measurement is provided use the usual ratio for NbTi superconductors and scale that value by cross section of superconductor and warn the user
+                warnings.warn(f'No Measurement for CUDI1 fit provided for coil {coil_name}. Usual ratio for NbTi superconductors of C1 and C2 is used and scaled by cross section of superconductor. Copper-non-copper ratio of magnet model will be used.')
+    
+                # get Copper to non Copper ratio
+                if not Cu_nCu: Cu_nCu = original_conductor.strand.Cu_noCu_in_strand
+                if not Cu_nCu: raise Exception(f'No Copper-to-non-copper ratio could be found in conductor database or modeldata for coil {coil_name}.')
+    
+                # hardcoded values come from magnet "MB inner layer" in csv file "Strand and cable characteristics"
+                # NOTE: cab...cable, str...strand, C1_cab = C1_str * nStrands  and  C1_str = C1_str_MB / A_MB * A_thisMagnet
+                C1_per_square_meter_of_NbTi = 3448.573 / 3.362E-07  # C1_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu) # MB inner layer
+                C2_per_square_meter_of_NbTi = -257.289 / 3.362E-07  # C2_cab/(Cable Section NbTi) #  = strandArea * nStrands * (1-fCu) # MB inner layer
+    
+                # scale it with the cross-section of superconductor
+                strand_cross_section = calc_strand_area(strand_geometry, original_conductor)
+                fraction_of_superconductor = 1 / (Cu_nCu + 1)
+                strand_NbTi_area = fraction_of_superconductor * strand_cross_section
+                C1_str = C1_per_square_meter_of_NbTi * strand_NbTi_area
+                C2_str = C2_per_square_meter_of_NbTi * strand_NbTi_area
+            else:
+                raise Exception(f'More then two measurements for CUDI1 fit provided in coil {coil_name}. Please only provide 2, 1 or 0 measurements.')
+    
+            # calculate cable parameters by multiplying with number of strands
+            Jc_dict['C1_CUDI1'] = C1_str * n_strand
+            Jc_dict['C2_CUDI1'] = C2_str * n_strand
+    
+            # check if values are real and not imaginary (e.g. when Bc20 is bigger than B_ref_Ic)
+            if np.iscomplex(complex(Jc_dict['C2_CUDI1'])) or np.iscomplex(complex(Jc_dict['C1_CUDI1'])):
+                raise Exception(f'When calculating CUDI1 parameters (C1, C2) the values turned out to have an imaginary part. Please check the inputs for coil {coil_name}.')
+    
+            return Jc_dict
+        else:
+            raise Exception(f'No implementation for fit type "{original_conductor.Jc_fit.type}" defined in ParsimConductor.')
+    
 
 def calc_strand_area(strand_geometry, original_conductor):
     # check inputs
     if not original_conductor.strand.type: raise Exception(f'Strand type is not specified in modelData.')
     
     if original_conductor.strand.type == 'Round':
 
@@ -786,106 +833,116 @@
     Bc2 = Bc20 * (1 - frac_T ** 2) * (1 - 0.31 * frac_T ** 2 * (1 - 1.77 * np.log(frac_T)))
     frac_B = B / Bc2
     if frac_B > 1: frac_B = 1
     Jc = C / np.sqrt(B) * (1 - frac_B) ** 2 * (1 - frac_T ** 2)**2
     return Jc
 
 
-def Jc_Nb3Sn_Bordini(T, B, C0, Tc0_Nb3Sn, Bc20_Nb3Sn, alpha):
-    # Critical current density in a Nb3Sn strand, Bordini fit
-
-    # % % % Check all inputs are scalars or vectors
-    if not (np.isscalar(T) or np.isscalar(B) or np.isscalar(C0) or np.isscalar(Tc0_Nb3Sn) or np.isscalar(Bc20_Nb3Sn) or np.isscalar(alpha)):
-        if not (len(T) == len(B) == len(C0) == len(Tc0_Nb3Sn) == len(Bc20_Nb3Sn) == len(alpha)):
-            raise ValueError('All inputs must be scalars or vectors with the same number of elements.')
-
-    nElements = max([len(T), len(B), len(C0), len(Tc0_Nb3Sn), len(Bc20_Nb3Sn), len(alpha)])
-
-    # % % % Check all inputs are scalars or vectors with the same number of elements
-    if ((len(T) > 1 and len(T) != nElements) or (len(B) > 1 and len(B) != nElements) or
-            (len(C0) > 1 and len(C0) != nElements) or
-            (len(Tc0_Nb3Sn) > 1 and len(Tc0_Nb3Sn) != nElements) or
-            (len(Bc20_Nb3Sn) > 1 and len(Bc20_Nb3Sn) != nElements) or
-            (len(alpha) > 1 and len(alpha) != nElements)):
-        raise ValueError('All inputs must be scalars or vectors with the same number of elements.')
-
-    # Modify the input magnetic field
-    B = np.abs(B)
-    B[B < 0] *= -1
-    B[np.abs(B) < 0.001] = 0.001  # very small magnetic field causes numerical problems
-
-    f_T_T0 = T / Tc0_Nb3Sn
-    f_T_T0[f_T_T0 > 1] = 1  # avoid values higher than 1
-    Bc2 = Bc20_Nb3Sn * (1 - f_T_T0 ** 1.52)
-    f_B_Bc2 = B / Bc2
-    f_B_Bc2[f_B_Bc2 > 1] = 1  # avoid values higher than 1
-    C = C0 * (1 - f_T_T0 ** 1.52) ** alpha * (1 - f_T_T0 ** 2) ** alpha
-
-    Jc_T_B = C / B * f_B_Bc2 ** 0.5 * (1 - f_B_Bc2) ** 2  # [A/m^2]
-    return Jc_T_B
-
-
-def todo():
-    #TODO make functions whereever this function is used
-    return None
-
 def make_value_SI(val: float, dim: str):
     if dim in ['mm', 'mOhm', 'mV']:
         return val / 1000
     elif dim in ['m', 'T', 'K', 'Ohm', 'V', '', ' ', '-']:
         return val
     elif dim in ['kA', 'kV', 'km']:
         return val * 1000
     elif dim in ['degC']:
         return val + 273.15
     else:
         raise Exception(f'unknown physical unit "{dim}".')
 
-def setattr_to_list(list_instances, row, col_name, attr_name):
+def setattr_to_list(list_instances: List[Any], row: pd.Series, col_name: str, attr_name: str):
+    """
+    Sets an attribute of a list of instances to a value derived from a specified column in a CSV row.
+
+    :param list_instances: a list of instances to modify
+    :param row: a row of data from a CSV file
+    :param col_name: the name of the CSV column to get values from
+    :param attr_name: the name of the attribute to set on each instance
+    """
     # get dimension from csv column name
     dim = col_name[col_name.find('[') + 1:col_name.find(']')] if '[' in col_name else ''
 
     # parse str into list or make single float to
     if isinstance(row[col_name], str):
         val_list = parse_str_to_list(row[col_name], only_float_list=True)
     elif type(row[col_name]) in [float, int]:
         val_list = [row[col_name] for _ in range(len(list_instances))]
     else:
         raise Exception(f'Unknown datatype in column "{col_name}".')
 
     for val, instance in zip(val_list, list_instances):
         rsetattr(instance, attr_name, make_value_SI(val, dim))
 
-def getattr_from_list(conductor_samples, sample_attribute_name, weight_factors):
-    # check if attribute is either set in all of the conductor_samples (return weighted values) or in none (return None)
+def getattr_from_list(list_instances: List[Any], attribute_name: str, weight_factors: List[float]):
+    """
+    returns the weighted attribute value from a list of instances
+
+    :param list_instances: list of instances to get the attribute value from
+    :param attribute_name: attribute name
+    :param weight_factors: list of weight factors
+    """
+    # check if attribute is either set in all of the instances (return weighted values) or in none (return None)
     attr_present = []
-    for con in conductor_samples:
-        if rgetattr(con, sample_attribute_name): attr_present.append(True)
+    for instance in list_instances:
+        if rgetattr(instance, attribute_name): attr_present.append(True)
         else: attr_present.append(False)
     if True in attr_present and False in attr_present:
-        raise Exception(f'The attribute "{sample_attribute_name}" is only set in a few instances of the ConductorSample list.')
+        raise Exception(f'The attribute "{attribute_name}" is only set in a few instances of the ConductorSample list.')
     if not all(attr_present):
         return None
 
-    # read the values for the specific attribute for all the ConductorSample instances and store them in a list
+    # read the values for the specific attribute for all the instances and store them in a list
     val_list = []
-    for con in conductor_samples:
-        val_list.append(rgetattr(con, sample_attribute_name))
+    for instance in list_instances:
+        val_list.append(rgetattr(instance, attribute_name))
 
     # if there is no weight_factors specified, weight them equally (average)
     if not weight_factors:
-        weight_factors = [1.0 for _ in range(len(conductor_samples))]
+        weight_factors = [1.0/len(list_instances) for _ in range(len(list_instances))]
 
     # check if length is the same
     if len(weight_factors) != len(val_list):
         raise Exception(f'The length of the weight factors {len(weight_factors)} is not the same as the number of conductor samples {len(val_list)}.')
 
-    # Normalize the weight_factors
-    weight_sum = sum(weight_factors)
-    normalized_weights = [w / weight_sum for w in weight_factors]
+    # check if weight factors is normalized
+    if sum(weight_factors) != 1.0:
+        weight_factors = [w / sum(weight_factors) for w in weight_factors]
 
     # calculate weighting
-    return sum([v * w for v, w in zip(val_list, normalized_weights)])
+    return sum([v * w for v, w in zip(val_list, weight_factors)])
+
+
+def average_dicts(dict_list: List[Dict[str, Any]]):
+    """
+    Returns a dictionary with the same keys as the list of input dicts, and makes the average for all the values in the list
+
+    :param dict_list: a list of dictionaries (with the same keys)
+    """
+    if not dict_list or dict_list == {}:
+        return {}
+
+    # check if all dicts have the same keys
+    first_dict_keys = set(dict_list[0].keys())
+    for d in dict_list[1:]:
+        if set(d.keys()) != first_dict_keys:
+            raise Exception('Input dictionaries do not have the same keys.')
+
+    avg_dict = {}
+    num_dicts = len(dict_list)
+
+    # Sum the values for each key
+    for d in dict_list:
+        for key, value in d.items():
+            # init dict value if not existing
+            if key not in avg_dict: avg_dict[key] = 0
+            if value is None or avg_dict[key] is None:
+                avg_dict[key] = None
+            else:
+                avg_dict[key] += value
 
+    # Divide the summed values by the number of dictionaries
+    for key in avg_dict:
+        avg_dict[key] /= num_dicts
 
+    return avg_dict
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.5.0/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.5.0/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from steam_sdk.data.DataEventCircuit import DataEventCircuit
 from steam_sdk.data.DataEventCircuit import Powering, General, QuenchEvent, EnergyExtraction
 from steam_sdk.utils.make_folder_if_not_existing import make_folder_if_not_existing
 from steam_sdk.utils.rgetattr import rgetattr
 from steam_sdk.utils.sgetattr import rsetattr
 from steam_sdk.utils.utils_PC import calculate_t_PC_off
 
-
 class ParsimEventCircuit:
     """
 
     """
 
     def __init__(self, ref_model: BuilderModel = None, verbose: bool = True):
         """
@@ -73,38 +72,41 @@
 
         # Assign the content to a dataclass structure
         list_events = []
         parsed_columns = []  # list containing the column names that were parsed
         for index, event_info in df_events.iterrows():
             new_event = DataEventCircuit()
             circuit_type = event_info["Circuit Family"]
+            circuit_name = event_info["Circuit Name"]
             rsetattr(new_event, 'GeneralParameters.circuit_type', circuit_type)
 
             if self.verbose:
                 print(f"circuit type: {circuit_type}")
             if circuit_type in ["RCBH", "RCBV"]:
-                parsed_columns += self.__read_RCB(event_info, new_event)
+                parsed_columns += self.__read_60A(event_info, new_event)
             elif circuit_type == "RQX":
                 parsed_columns += self.__read_RQX(event_info, new_event)
-            elif circuit_type in ["RQ4", "RQ5",  "RQ6", "RQ7", "RQ8", "RQ9", "RQ10"]:
+            elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
                 parsed_columns += self.__read_IPQ(event_info, new_event)
             elif circuit_type in ["RD1", "RD2", "RD3", "RD4"]:
                 parsed_columns += self.__read_IPD(event_info, new_event)
-            elif circuit_type == "RCS":
-                parsed_columns += self.__read_RCS(event_info, new_event)
+            elif circuit_type in ["RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
+                parsed_columns += self.__read_600A_with_EE(event_info, new_event)
             elif circuit_type == "RCD":
                 parsed_columns += self.__read_RCD(event_info, new_event)
             elif circuit_type == "RCBX":
                 parsed_columns += self.__read_RCBX(event_info, new_event)
-            elif circuit_type in ["RCBCH", "RCBCV"]:
-                parsed_columns += self.__read_RCBC(event_info, new_event)
+            elif circuit_type in ["RCBCH", "RCBCV", "RCBYH", "RCBYV"]:
+                parsed_columns += self.__read_80_120A(event_info, new_event)
             elif circuit_type == "RQ":
                 parsed_columns += self.__read_RQ(event_info, new_event)
             elif circuit_type == "RB":
                 parsed_columns += self.__read_RB(event_info, new_event)
+            elif circuit_type in ["RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3"]: #RQS common to EE and no EE case
+                parsed_columns += self.__read_600A_no_EE(event_info, new_event)
             else:
                 raise Exception(f"circuit type not supported {circuit_type}")
             list_events.append(new_event)
 
         # print out all the names of the ignored columns
         ignored_column_names = list(set(df_events.columns) - set(parsed_columns))
         if self.verbose:
@@ -127,15 +129,19 @@
             path_outputfile_event_csv (str): Path to the output event CSV file.
 
         Raises:
             Exception: If the length of input simulation numbers differs from length of events found in the input file.
 
         """
         # check inputs
-        if len(simulation_numbers) != len(self.list_events):
+        if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"]:
+            if len(simulation_numbers) != 2 * len(self.list_events):
+                raise Exception(
+                    f'length of input simulation numbers ({len(simulation_numbers)}) is not double of length of events found in the input file ({len(self.list_events)}) for RQ type circuit')
+        elif len(simulation_numbers) != len(self.list_events):
             raise Exception(
                 f'length of input simulation numbers ({len(simulation_numbers)}) differs from length of events found in the input file ({len(self.list_events)})')
 
         # Make target folder if it is missing
         make_folder_if_not_existing(os.path.dirname(path_outputfile_event_csv))
 
         # open file in writing mode
@@ -143,37 +149,92 @@
         list_paramerers = []
 
         # Loop trough each element of self.list_events and write parameters to csv
         for i, event in enumerate(self.list_events):
             print(i, event)
             new_row = {'simulation_name': simulation_name, 'simulation_number': simulation_numbers[i]}
             event_data = self.__write_event(event)
+            event_data_counter = 0
             if isinstance(event_data, list):
                 for data in event_data:
                     new_row.update(data)
+                    if simulation_name in ["RQ_47magnets", "RQ_51magnets", "RCBX"] and event_data_counter % 2 != 0:
+                        new_row['simulation_number'] = 2
                     all_rows.append(new_row.copy())
                     list_paramerers = list(set(list_paramerers + list(new_row.keys())))
+                    event_data_counter = event_data_counter + 1
             else:
                 new_row.update(event_data)
                 all_rows.append(new_row)
                 list_paramerers = list(set(list_paramerers + list(new_row.keys())))
 
         # TODO reorder the columns
         # Write file
         with open(path_outputfile_event_csv, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=list_paramerers)
             writer.writeheader()
             for new_row in all_rows:
                 writer.writerow(new_row)
 
     ### Helper functions ###
+    def __read_600A_no_EE(self, event_info: pd.Series, new_event: DataEventCircuit):
+        '''
+        Function to read 600A circuit family with no EE parameters
+
+        :param event_info: Series of parameters
+        :param new_event: DataEventCircuit object to update
+        :return: new_event
+        '''
+        circuit_name = event_info["Circuit Name"]
+        dict_params_GeneralParameters = {
+            'Circuit Name': 'GeneralParameters.name',
+            "Period": 'GeneralParameters.period',
+            "Date (FGC)": 'GeneralParameters.date',
+            "Time (FGC)": 'GeneralParameters.time',
+            'Circuit Family': 'GeneralParameters.circuit_type'
+        }
+        dict_params_Powering = {
+            "Circuit Name": 'circuit_name',
+            "Circuit Family": 'circuit_type',
+            'I_Q_circ': 'current_at_discharge',
+            "Ramp rate": 'dI_dt_at_discharge',
+            "Plateau duration": 'plateau_duration',
+            "Delta_t(FGC-PIC)": 'delta_t_FGC_PIC',
+            "FPA Reason": 'cause_FPA'
+        }
+        dict_params_QuenchEvents = {
+            'I_Q_circ': 'current_at_quench',
+            'Type of Quench': 'quench_cause',
+            "Delta_t(QPS-PIC)": 'delta_t_iQPS_PIC',
+            "dU_QPS/dt": 'dU_iQPS_dt',
+            "QDS trigger origin": "QDS_trigger_origin"
+        }
+        # Assign General parameters
+        new_event.GeneralParameters = General()
+        for param in dict_params_GeneralParameters:
+            if param in event_info:
+                rsetattr(new_event, dict_params_GeneralParameters[param], event_info[param])
+
+        # Assign powering parameters
+        new_event.PoweredCircuits[circuit_name] = Powering()
+        for param in dict_params_Powering:
+            if param in event_info:
+                rsetattr(new_event.PoweredCircuits[circuit_name], dict_params_Powering[param], event_info[param])
+
+        # Assign quench event parameters
+        new_event.QuenchEvents[circuit_name] = QuenchEvent()
+        for param in dict_params_QuenchEvents:
+            if param in event_info:
+                rsetattr(new_event.QuenchEvents[circuit_name], dict_params_QuenchEvents[param], event_info[param])
 
-    def __read_RCB(self, event_info: pd.Series, new_event: DataEventCircuit):
+        return_list = list(dict_params_Powering.keys()) + list(dict_params_QuenchEvents.keys()) + list(dict_params_GeneralParameters.keys())
+        return return_list
+    def __read_60A(self, event_info: pd.Series, new_event: DataEventCircuit):
         '''
-        Function to read RCBH family parameters
+        Function to read 60 A family parameters
 
         :param event_info: Series of parameters
         :param new_event: DataEventCircuit object to update
         :return: new_event
         '''
         circuit_name = event_info["Circuit Name"]
         dict_params_GeneralParameters = {
@@ -398,15 +459,15 @@
         for param in dict_params_QuenchEvents:
             if param in event_info:
                 rsetattr(new_event.QuenchEvents[circuit_name], dict_params_QuenchEvents[param], event_info[param])
 
         return_list = list(dict_params_Powering.keys()) + list(dict_params_QuenchEvents.keys()) + list(dict_params_GeneralParameters.keys())
         return return_list
 
-    def __read_RCS(self, event_info: pd.Series, new_event: DataEventCircuit):
+    def __read_600A_with_EE(self, event_info: pd.Series, new_event: DataEventCircuit):
         '''
         Function to read RCS family parameters
 
         :param event_info: Series of parameters
         :param new_event: DataEventCircuit object to update
         :return: new_event
         '''
@@ -604,17 +665,17 @@
                 for subkey in key:
                     return_list.append(subkey)
             else:
                 return_list.append(key)
 
         return return_list
 
-    def __read_RCBC(self, event_info: pd.Series, new_event: DataEventCircuit):
+    def __read_80_120A(self, event_info: pd.Series, new_event: DataEventCircuit):
         '''
-        Function to read RCBCH family parameters
+        Function to read RCBC, RCBY family parameters
 
         :param event_info: Series of parameters
         :param new_event: DataEventCircuit object to update
         :return: new_event
         '''
         circuit_name = event_info["Circuit Name"]
         dict_params_GeneralParameters = {
@@ -816,88 +877,50 @@
             else:
                 return_list.append(key)
 
         return return_list
 
     def __write_event(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         circuit_type = event.GeneralParameters.circuit_type
-        if circuit_type in ['RCBH', 'RCBV']:
-            event_dict = self.__write_RCB(event, t_after_PC_off=t_after_PC_off)
-        elif circuit_type in ["RD1", "RD2", "RD3", "RD4"]:
-            event_dict = self.__write_IPD(event, t_after_PC_off=t_after_PC_off)
+        circuit_name = event.GeneralParameters.name
+        if circuit_type in ['RCBH', 'RCBV', "RQT12", "RQT13", "RSS", "RQTL7", "RQTL8", "RQTL10", "RQTL11", "RQSX3", "RCBYV", "RCBYH", "RCBCH", "RCBCV", "RD1", "RD2", "RD3", "RD4"]:
+            event_dict = self.__write_common_circuit_family(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQ":
             event_dict = self.__write_RQ(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type in ["RQ4", "RQ5", "RQ7", "RQ8", "RQ9", "RQ10"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 6):
+            event_dict = self.__write_IPQ(event, t_after_PC_off=t_after_PC_off)
         elif circuit_type == "RQX":
             event_dict = self.__write_RQX(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type in ["RCS", "ROD", "ROF", "RSD", "RSF", "RQTL9", "RQTD", "RQTF"] or (circuit_name.startswith("RQ6.") and len(circuit_name) == 8):
+            event_dict = self.__write_600A_with_EE(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type == "RB":
+            event_dict = self.__write_RB(event, t_after_PC_off=t_after_PC_off)
+        elif circuit_type == "RCBX":
+            event_dict = self.__write_RCBX(event, t_after_PC_off=t_after_PC_off)
         return event_dict
 
-    def __write_RCB(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+    def __write_common_circuit_family(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RCB.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
         Returns:
             dict: A dictionary containing the RCB information.
 
         """
         circuit_name = event.GeneralParameters.name
-
         event_dict = dict()
         t_start = 0  # hard-coded
         I_start = 0.0  # hard-coded
         dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
         dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
         current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
-        if dI_dt == 0:
-            I_end = current_at_discharge
-            dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
-            time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
-            t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
-            t_PC_off = t_start + time_to_reach_I + t_plateau
-            #event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
-
-        elif dI_dt < 0:
-            I_end_1 = 1.2*current_at_discharge
-            I_end_2 = current_at_discharge
-            t_plateau = 10  # hard-coded
-            t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
-            event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
-            event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
-
-        else:
-            I_end = str(current_at_discharge) + " + 100.0"
-            I_target = current_at_discharge + 100.0
-            t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
-            t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
-            event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target - 100.0
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
-
-        dict_time_schedule = {
-            '0.0': '0.5',
-            f'{t_PC_off - 1.000}': '0.100',
-            f'{t_PC_off - 0.100}': '0.010',
-            f'{t_PC_off - 0.010}': '0.001',
-            f'{t_PC_off - 0.001}': '0.0001',
-            f'{t_PC_off + 0.020}': '0.001',
-            f'{t_PC_off + 1.000}': '0.010',
-            f'{t_PC_off + 3.000}': '0.500'
-        }
-        event_dict['GlobalParameters.global_parameters.I_start'] = I_start
-        event_dict['GlobalParameters.global_parameters.t_start'] = t_start
-        event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-        event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
-        event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
-        event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+        t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
 
         # TODO
         # if dI/dt is 0:
         # read dI/dt and dI/st2 from the STEAM model
         # set the plateau length
         # set the I_end_1
@@ -928,95 +951,29 @@
         #     if rgetattr(event.PoweredCircuits[circuit_name], old_name) and not math.isnan(rgetattr(event.PoweredCircuits[circuit_name], old_name)):
         #         event_dict[new_name] = rgetattr(event.PoweredCircuits[circuit_name], old_name)
         #     if not new_name in event_dict:
         #         event_dict[new_name] = ''
 
         return event_dict
 
-    def __write_IPD(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
-        """
-        Extract the information for an event of circuit type IPD.
-
-        Parameters:
-            event (DataEventCircuit): The data event object to read the data.
-
-        Returns:
-            dict: A dictionary containing the IPD information.
-
-        """
-        circuit_name = event.GeneralParameters.name
-
-        event_dict = dict()
-        t_start = 0  # hard-coded
-        I_start = 0.0  # hard-coded
-        dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
-        dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
-        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
-        if dI_dt == 0:
-            I_end = current_at_discharge
-            dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
-            time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
-            t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
-            t_PC_off = t_start + time_to_reach_I + t_plateau
-            #event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
-
-        elif dI_dt < 0:
-            I_end_1 = 1.2*current_at_discharge
-            I_end_2 = current_at_discharge
-            t_plateau = 10  # hard-coded
-            t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
-            event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
-            event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
-
-        else:
-            I_end = str(current_at_discharge) + " + 100.0"
-            I_target = current_at_discharge + 100.0
-            t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
-            t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
-            event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
-            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target - 100.0
-            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
-
-        dict_time_schedule = {
-            '0.0': '0.5',
-            f'{t_PC_off - 1.000}': '0.100',
-            f'{t_PC_off - 0.100}': '0.010',
-            f'{t_PC_off - 0.010}': '0.001',
-            f'{t_PC_off - 0.001}': '0.0001',
-            f'{t_PC_off + 0.020}': '0.001',
-            f'{t_PC_off + 1.000}': '0.010',
-            f'{t_PC_off + 3.000}': '0.500'
-        }
-        event_dict['GlobalParameters.global_parameters.I_start'] = I_start
-        event_dict['GlobalParameters.global_parameters.t_start'] = t_start
-        event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
-        event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
-        event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
-        event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
-        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
-
-        return event_dict
-
     def __write_RQ(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RQ.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
         Returns:
             list[dict]: A list of dictionaries containing the RQ information.
 
         """
         circuit_name = event.GeneralParameters.name
         list= []
+        t_EE_list = []
+        t_PC_off_list = []
         for i in range(2):
             event_dict = dict()
             t_start = 0  # hard-coded
             I_start = 0.0  # hard-coded
             dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
             dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
 
@@ -1027,55 +984,86 @@
                 time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
                 t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
                 t_PC_off = t_start + time_to_reach_I + t_plateau
                 #event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
                 event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
                 event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
 
-            elif dI_dt < 0:
+            elif np.sign(dI_dt) != np.sign(current_at_discharge):
                 I_end_1 = 1.2*current_at_discharge
                 I_end_2 = current_at_discharge
                 t_plateau = 10  # hard-coded
-                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
                 event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
                 event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
                 event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
                 event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
 
             else:
                 I_end = str(current_at_discharge) + " + 100.0"
                 I_target = current_at_discharge + 100.0
                 t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
                 t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
                 event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
-                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target - 100.0
+                event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target
                 event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
 
+            t_PC_off_list.append(t_PC_off)
             dict_time_schedule = {
                 '0.0': '0.5',
                 f'{t_PC_off - 1.000}': '0.100',
                 f'{t_PC_off - 0.100}': '0.010',
                 f'{t_PC_off - 0.010}': '0.001',
                 f'{t_PC_off - 0.001}': '0.0001',
                 f'{t_PC_off + 0.020}': '0.001',
                 f'{t_PC_off + 1.000}': '0.010',
                 f'{t_PC_off + 3.000}': '0.500'
             }
             event_dict['GlobalParameters.global_parameters.I_start'] = I_start
             event_dict['GlobalParameters.global_parameters.t_start'] = t_start
             event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
             event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
+            event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + 0.096
             event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
             event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
-            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
+            event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(t_PC_off + 0.096)
 
             list.append(event_dict)
 
         return list
 
+    def __write_RCBX(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type RCBX.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RQ information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        t_PC_off_list = []
+        for i in range(2):
+            event_dict = dict()
+            t_start = 0  # hard-coded
+            I_start = 0.0  # hard-coded
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+            t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
+            t_PC_off_list.append(t_PC_off)
+            event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
+            list.append(event_dict)
+
+        return list
+
     def __write_RQX(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
         """
         Extract the information for an event of circuit type RQX.
 
         Parameters:
             event (DataEventCircuit): The data event object to read the data.
 
@@ -1102,19 +1090,19 @@
             if dI_dt == 0:
                 I_end = current_at_discharge
                 dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[ramp_rate_list[i]])
                 time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
                 t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
                 t_PC_off = t_start + time_to_reach_I + t_plateau
 
-            elif dI_dt < 0:
+            elif np.sign(dI_dt) != np.sign(current_at_discharge):
                 I_end_1 = 1.2*current_at_discharge
                 I_end_2 = current_at_discharge
                 t_plateau = 10  # hard-coded
-                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, -dI_dt2], [t_plateau, t_plateau], I_end_2)
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
 
             else:
                 I_end = str(current_at_discharge) + " + 100.0"
                 I_target = current_at_discharge + 100.0
                 t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
                 t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
 
@@ -1142,40 +1130,250 @@
             else:
                 t_start = 0
             I_start = 0.0  # hard-coded
             if dI_dt == 0:
                 event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = current_at_discharge
                 event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
                 t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
-            elif dI_dt < 0:
+            elif np.sign(dI_dt) != np.sign(current_at_discharge):
+                I_end_1 = 1.2*current_at_discharge
+                I_end_2 = current_at_discharge
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_end_1
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = I_end_2
+                event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = -dI_dt  # setting dI_dt
+                event_dict[f'GlobalParameters.global_parameters.dI_dt2_PC{i+1}'] = dI_dt2  # setting dI_dt2
+                t_plateau = 10  # hard-coded
+            else:
+                I_target = current_at_discharge + 100.0
+                event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = dI_dt  #setting dI_dt
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_target
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
+                t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+
+            event_dict[f'GlobalParameters.global_parameters.t_PC_off_PC{i+1}'] = t_PC_off
+            event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+            event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+            event_dict[f'GlobalParameters.global_parameters.I_start_PC{i+1}'] = I_start
+            event_dict[f'GlobalParameters.global_parameters.t_start_PC{i+1}'] = t_start
+            event_dict[f'GlobalParameters.global_parameters.t_plateau_PC{i + 1}'] = t_plateau
+            list.append(event_dict)
+
+        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+        return list
+
+    def __write_IPQ(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type IPQ.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the IPQ information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        t_PC_off_list = []
+        acceleration_list = ["dI_dt2_PC1", "dI_dt2_PC2"]
+        ramp_rate_list = ["dI_dt_PC1", "dI_dt_PC2"]
+
+        #loop to calculate list of t_PC_off
+        for i in range(2):
+            #event_dict = dict()
+            t_start = 0  # hard-coded
+            I_start = 0.0  # hard-coded
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[acceleration_list[i]])  # read dI/dt2 from the STEAM model
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+
+            if dI_dt == 0:
+                I_end = current_at_discharge
+                dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[ramp_rate_list[i]])
+                time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
+                t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
+                t_PC_off = t_start + time_to_reach_I + t_plateau
+
+            elif np.sign(dI_dt) != np.sign(current_at_discharge):
+                I_end_1 = 1.2*current_at_discharge
+                I_end_2 = current_at_discharge
+                t_plateau = 10  # hard-coded
+                t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_end_2], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
+
+            else:
+                I_end = str(current_at_discharge) + " + 100.0"
+                I_target = current_at_discharge + 100.0
+                t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+                t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
+
+            t_PC_off_list.append(t_PC_off)
+
+        t_PC_off = max(t_PC_off_list)
+        dict_time_schedule = {
+            '0.0': '0.5',
+            f'{t_PC_off - 1.000}': '0.100',
+            f'{t_PC_off - 0.100}': '0.010',
+            f'{t_PC_off - 0.010}': '0.001',
+            f'{t_PC_off - 0.001}': '0.0001',
+            f'{t_PC_off + 0.020}': '0.001',
+            f'{t_PC_off + 1.000}': '0.010',
+            f'{t_PC_off + 3.000}': '0.500'
+        }
+        #loop to write events
+        for i in range(2):
+            event_dict = dict()
+            dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge[i]
+            dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')[acceleration_list[i]])
+            current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge[i]
+            if t_PC_off_list[i] < t_PC_off:
+                t_start = t_PC_off - t_PC_off_list[i]
+            else:
+                t_start = 0
+            I_start = 0.0  # hard-coded
+            if dI_dt == 0:
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = current_at_discharge
+                event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
+                t_plateau = event.PoweredCircuits[circuit_name].plateau_duration[i]
+            elif np.sign(dI_dt) != np.sign(current_at_discharge):
                 I_end_1 = 1.2*current_at_discharge
                 I_end_2 = current_at_discharge
                 event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_end_1
                 event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = I_end_2
                 event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = -dI_dt  # setting dI_dt
                 event_dict[f'GlobalParameters.global_parameters.dI_dt2_PC{i+1}'] = dI_dt2  # setting dI_dt2
                 t_plateau = 10  # hard-coded
             else:
                 I_target = current_at_discharge + 100.0
                 event_dict[f'GlobalParameters.global_parameters.dI_dt_PC{i+1}'] = dI_dt  #setting dI_dt
-                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_target - 100.0
+                event_dict[f'GlobalParameters.global_parameters.I_end_1_PC{i+1}'] = I_target
                 event_dict[f'GlobalParameters.global_parameters.I_end_2_PC{i+1}'] = 0.0
                 t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
 
             event_dict[f'GlobalParameters.global_parameters.t_PC_off_PC{i+1}'] = t_PC_off
             event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
             event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
             event_dict[f'GlobalParameters.global_parameters.I_start_PC{i+1}'] = I_start
             event_dict[f'GlobalParameters.global_parameters.t_start_PC{i+1}'] = t_start
             event_dict[f'GlobalParameters.global_parameters.t_plateau_PC{i + 1}'] = t_plateau
             list.append(event_dict)
 
         event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
         return list
 
+    def __write_600A_with_EE(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type 600A with EE.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RQ information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        t_EE_list = []
+        t_PC_off_list = []
+        event_dict = dict()
+        t_start = 0  # hard-coded
+        I_start = 0.0  # hard-coded
+        dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+        dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
+        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
+        t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
+        t_PC_off_list.append(t_PC_off)
+        event_dict['GlobalParameters.global_parameters.t_EE'] = t_PC_off + 0.008
+        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off_list
+        event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = t_EE_list.append(t_PC_off + 0.008)
+
+        list.append(event_dict)
+
+        return list
+
+    def __write_RB(self, event: DataEventCircuit, t_after_PC_off: float = 10.0):
+        """
+        Extract the information for an event of circuit type RB.
+
+        Parameters:
+            event (DataEventCircuit): The data event object to read the data.
+
+        Returns:
+            list[dict]: A list of dictionaries containing the RQ information.
+
+        """
+        circuit_name = event.GeneralParameters.name
+        list= []
+        event_dict = dict()
+        t_start = 0  # hard-coded
+        I_start = 0.0  # hard-coded
+        dI_dt2 = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt2'])  # read dI/dt2 from the STEAM model
+        dI_dt = event.PoweredCircuits[circuit_name].dI_dt_at_discharge
+        current_at_discharge = event.PoweredCircuits[circuit_name].current_at_discharge
+        t_PC_off = self.__handle_ramp_rate_cases(event, circuit_name, t_after_PC_off, t_start, I_start, dI_dt, dI_dt2, current_at_discharge, event_dict)
+        event_dict['GlobalParameters.global_parameters.t_EE_1'] = t_PC_off + 0.005 # value to be confirmed for RB
+        event_dict['GlobalParameters.global_parameters.t_EE_2'] = t_PC_off + 0.005
+        event.PoweredCircuits[circuit_name].delta_t_FGC_PIC = t_PC_off
+        event.EnergyExtractionSystem[circuit_name].delta_t_EE_PIC = [t_PC_off + 0.005]*2
+
+        list.append(event_dict)
+
+        return list
+
+    def __handle_ramp_rate_cases(self, event: DataEventCircuit, circuit_name: str, t_after_PC_off: float, t_start: float, I_start: float, dI_dt: float, dI_dt2: float, current_at_discharge: float, event_dict: dict ):
+        if dI_dt == 0:
+            I_end = current_at_discharge
+            dI_dt = float(rgetattr(self.ref_model.circuit_data, 'GlobalParameters.global_parameters')['dI_dt'])
+            time_to_reach_I = self.__time_to_reach_I(I=I_end, dI_dt=dI_dt, dI_dt2=dI_dt2, I_start=I_start)
+            t_plateau = event.PoweredCircuits[circuit_name].plateau_duration
+            t_PC_off = t_start + time_to_reach_I + t_plateau
+            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end
+            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+
+        elif np.sign(dI_dt) != np.sign(current_at_discharge):
+            I_end_1 = 1.2*current_at_discharge
+            I_end_2 = current_at_discharge
+            I_target = current_at_discharge + np.sign(current_at_discharge) * 100.0
+            t_plateau = 10  # hard-coded
+            t_PC_off = calculate_t_PC_off(t_start, I_start, [I_end_1, I_target], [-dI_dt, dI_dt], [dI_dt2, dI_dt2], [t_plateau, t_plateau], I_end_2)
+            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_end_1
+            event_dict['GlobalParameters.global_parameters.I_end_2'] = I_end_2
+            event_dict['GlobalParameters.global_parameters.dI_dt'] = -dI_dt  # setting dI_dt
+            event_dict['GlobalParameters.global_parameters.dI_dt2'] = dI_dt2  # setting dI_dt2
+
+        else:
+            I_end = str(current_at_discharge) + " + 100.0"
+            I_target = current_at_discharge + 100.0
+            t_plateau = t_start + 2 * dI_dt / dI_dt2 + (I_target - I_start - dI_dt ** 2 / dI_dt2) / dI_dt
+            t_PC_off = calculate_t_PC_off(t_start, I_start,  I_target, [dI_dt], [dI_dt2], [t_plateau], I_target - 100)
+            event_dict['GlobalParameters.global_parameters.dI_dt'] = dI_dt  #setting dI_dt
+            event_dict['GlobalParameters.global_parameters.I_end_1'] = I_target
+            event_dict['GlobalParameters.global_parameters.I_end_2'] = 0.0
+
+        dict_time_schedule = {
+            '0.0': '0.5',
+            f'{t_PC_off - 1.000}': '0.100',
+            f'{t_PC_off - 0.100}': '0.010',
+            f'{t_PC_off - 0.010}': '0.001',
+            f'{t_PC_off - 0.001}': '0.0001',
+            f'{t_PC_off + 0.020}': '0.001',
+            f'{t_PC_off + 1.000}': '0.010',
+            f'{t_PC_off + 3.000}': '0.500'
+        }
+
+        event_dict['GlobalParameters.global_parameters.I_start'] = I_start
+        event_dict['GlobalParameters.global_parameters.t_start'] = t_start
+        event_dict['GlobalParameters.global_parameters.t_plateau'] = t_plateau
+        event_dict['GlobalParameters.global_parameters.t_PC_off'] = t_PC_off
+        event_dict['Analysis.simulation_time.time_end'] = t_PC_off + t_after_PC_off
+        event_dict['Analysis.simulation_time.time_schedule'] = dict_time_schedule
+
+        return t_PC_off
+
     @staticmethod
     def __time_to_reach_I(I: float, dI_dt: float, dI_dt2: float, I_start: float):
         '''
         Calculate the time to reach a current assuming a parabolic, linear, and parabolic profile
         :return: time [s]
         '''
         t_parabolic = dI_dt / dI_dt2
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.5.0/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2023.5.0/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,31 @@
+# this file defines all the possible column names for parameters of a parsim conductor step.
+# If a new input table uses different names/spelling, just add them here and the code does the rest.
 MainColumnNames:
   magnet_name:
     - Magnet
     - Magnet Name
     - magnet
     - magnet name
   coil_name:
     - Coil
     - Coil Name
     - coil
     - coil name
 ConductorSample:
+  Ra:
+    - Ra [Ohm]
+    - Ra
+  Rc:
+    - Rc [Ohm]
+    - Rc
+  f_rho_eff:
+    - f rho eff [-]
+    - f rho eff
+    - f rho
   strand_geometry.diameter:
     - Ds
     - Ds [m]
     - Ds [mm]
     - strand_diameter
     - Strand diameter [m]
     - Strand diameter [mm]
@@ -68,34 +80,28 @@
     - RRR
     - Estimated coil RRR
   Cu_noCu:
     - Ave Cu/noCu
     - Copper to non-Copper ratio
     - Cu/noCu
     - Cu_noCu
+  height:
+    - Height [m]
+    - Height [mm]
+    - Height
 Coil:
   coil_resistance_room_T:
     - RT coil resistance [Ohm]
   Cu_noCu_resistance_meas:
     - Cu/nocu from RT meas
-  total_conductor_length:
-    - tot coil length [m]
   T_ref_coil_resistance:
     - RT coil resistance temperature [degC]
   weight_factors:
     - weight factor
     - Weight factor
   T_ref_RRR_low:
     - T ref RRR low
   T_ref_RRR_high:
     - T ref RRR high
-
-
-
-
-
-# 'Number of strands': 'number_of_strands', 'number_of_strands': 'number_of_strands',
-# 'Height [m]': 'height', 'Height [mm]': 'height', 'height': 'height',
-# 'F rho eff': 'f_rho_eff', 'f_rho_eff': 'f_rho_eff',
-# 'Ra [Ohm]': 'Ra',
-# 'Rc [Ohm]': 'Rc'
+  B_resistance_meas:
+    - mag field resistance meas
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.5.0/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.5.0/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.5.0/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/plotters/PlotterSIGMA.py` & `steam-sdk-2023.5.0/steam_sdk/plotters/PlotterMap2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,79 @@
+import os
+
 import matplotlib.lines as lines
 import matplotlib.patches as patches
 import numpy as np
 import pandas as pd
 from matplotlib import pyplot as plt
 from matplotlib.colors import LogNorm
 import matplotlib.cm as cm
 #from steam_sdk.plotters.PlotterRoxie import plotEdges
 from steam_sdk.utils.misc import displayWaitAndClose
 
+def export_B_field_txt_to_map2d_SIGMA(path_map2d_roxie, path_result_txt_Bx, path_result_txt_By, path_new_file):
+    """
+    Copy content of reference map2d file and overwrites Bx and By values which are replaced values from
+    comsol output txt file and writes to a new map2d file.
+    :param path_map2d: Path to reference map2d from which all values apart from Bx and By is copied from
+    :param path_result: Comsol output txt file with evaluated B-field
+    :param path_new_file: Path to new map2d file where new B-field is stored
+    :return:
+    """
+    df_reference = pd.read_csv(path_map2d_roxie, delim_whitespace=True)
+    with open(path_result_txt_Bx) as file:  # opens a text file
+        lines = [line.strip().split() for line in file if not "%" in line]  # loops over each line
+
+    df_txt_Bx = pd.DataFrame(lines, columns=["x", "y", "Bx"])
+
+    df_txt_Bx = df_txt_Bx.apply(pd.to_numeric)
+
+    with open(path_result_txt_By) as file:  # opens a text file
+        lines = [line.strip().split() for line in file if not "%" in line]  # loops over each line
+
+    df_txt_By = pd.DataFrame(lines, columns=["x", "y", "By"])
+    df_txt_By = df_txt_By.apply(pd.to_numeric)
+
+    # Verify all evaluate field at same coordinates!
+
+    x_tol, y_tol = 1e-10, 1e-10
+    x_ref, y_ref = df_reference['X-POS/MM'] / 1000, df_reference['Y-POS/MM'] / 1000
+
+    if ((x_ref - df_txt_Bx['x']).abs().max() < x_tol) and \
+            ((x_ref - df_txt_By['x']).abs().max() < x_tol) and \
+            ((y_ref - df_txt_Bx['y']).abs().max() < y_tol) and \
+            ((y_ref - df_txt_By['y']).abs().max() < y_tol):
+        print("All dataframes have the same x and y coordinates.")
+    else:
+        raise ValueError("Error: Not all dataframes have the same x and y coordinates. Can't compare map2ds!")
+
+    # Create new map2d
+    with open(path_new_file, 'w') as file:
+        file.write("  BL.   COND.    NO.    X-POS/MM     Y-POS/MM    BX/T       BY/T"
+                   "      AREA/MM**2 CURRENT FILL FAC.\n\n")
+        content = []
+        for index, row in df_reference.iterrows():
+            bl, cond, no, x, y, Bx, By, area, curr, fill, fac = row
+            bl = int(bl)
+            cond = int(cond)
+            no = int(no)
+            x = f"{x:.4f}"
+            y = f"{y:.4f}"
+            Bx = df_txt_Bx["Bx"].iloc[index]
+            Bx = f"{Bx:.4f}"
+            By = df_txt_By["By"].iloc[index]
+            By = f"{By:.4f}"
+            area = f"{area:.4f}"
+            curr = f"{curr:.2f}"
+            fill = f"{fill:.4f}"
+            content.append(
+                "{0:>6}{1:>6}{2:>7}{3:>13}{4:>13}{5:>11}{6:>11}{7:>11}{8:>9}{9:>8}\n".format(bl, cond, no, x, y, Bx,
+                                                                                             By,
+                                                                                             area, curr, fill))
+        file.writelines(content)
 
 def plot_multiple_areas(ax, areas, color=None):
     """
     Functions takes in a list of area objects and plot them on axis ax.
     :param ax: Axis to create plots.
     :param areas: list of SIGMA area objects.
     :param color: Color of the object
@@ -291,51 +353,56 @@
     df["abs_err_x"] = abs(df["Bx1"] - df["Bx2"])
     df["abs_err_y"] = abs(df["By1"] - df["By2"])
     df["Bmod1"] = np.sqrt(df["Bx1"] ** 2 + df["By1"] ** 2)
     df["Bmod2"] = np.sqrt(df["Bx2"] ** 2 + df["By2"] ** 2)
     df["Bmod_error"] = df["Bmod1"] - df["Bmod2"]
     return df
 
-def generate_report_from_map2d(plot, map2d_file_path1, map2d_name1, map2d_file_path2, map2d_name2, type):
+def generate_report_from_map2d(working_dir_path, map2d_file_path1, map2d_name1, map2d_file_path2, map2d_name2, type, save=False):
     """
     Generate plots for comparing two map2d files. Method generates the following plots:
     Bmod fields, Bmod error, relative error Bx/By, Bx/By field, Bx/By error, absolut difference Bx/By
     :param map2d_file_path1: Path to map2d file nr 1
     :param map2d_name1: String name of map2d nr 1 (e.g SIGMA/ROXIE)
     :param map2d_file_path2: Path to map2d file nr 2
     :param map2d_name2: String name of map2d nr 1 (e.g SIGMA/ROXIE)
-    :return: 
+    :return:
     """
     df=get_df_map2d(map2d_file_path1, map2d_file_path2)
-    if plot:
-        fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
-        fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
-        fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
-        fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
-        fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
-        plot_Bmod(df, map2d_name1, map2d_name2, fig1, ax1, type)
-        plot_B_mod_error(df,map2d_name1, map2d_name2, fig2, ax2, type)
-        plot_Bx_By(df, map2d_name1, map2d_name2, fig3, ax3, type)
-        try:
-            plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig4, ax4, type)
-        except:
-            print("Couldn't generate relative error plots.")
-        plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig5, ax5, type)
-        print("----Bmod error description----- ")
-        print(df["Bmod_error"].describe())
-        print(df["Bmod_error"].nlargest(10))
-
-        print("----Rel error x description----- ")
-        print(df["rel_err_x"].describe())
-        print(df["rel_err_x"].nlargest(10))
-        print("----Rel error y description----- ")
-        print(df["rel_err_y"].describe())
-        print(df["rel_err_y"].nlargest(10))
-        displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=10)
-        plt.close('all')
+    fig1, ax1 = plt.subplots(2, 2, figsize=(12, 12))
+    fig2, ax2 = plt.subplots(1, 2, figsize=(12, 12))
+    fig3, ax3 = plt.subplots(3, 2, figsize=(12, 12))
+    fig4, ax4 = plt.subplots(2, 2, figsize=(12, 12))
+    fig5, ax5 = plt.subplots(2, 2, figsize=(12, 12))
+    plot_Bmod(df, map2d_name1, map2d_name2, fig1, ax1, type)
+    plot_B_mod_error(df,map2d_name1, map2d_name2, fig2, ax2, type)
+    plot_Bx_By(df, map2d_name1, map2d_name2, fig3, ax3, type)
+    try:
+        plot_relative_error_x_y(df, map2d_name1, map2d_name2, fig4, ax4, type)
+    except:
+        print("Couldn't generate relative error plots.")
+    plot_difference_Bx_By(df, map2d_name1, map2d_name2, fig5, ax5, type)
+    print("----Bmod error description----- ")
+    print(df["Bmod_error"].describe())
+    print(df["Bmod_error"].nlargest(10))
+
+    print("----Rel error x description----- ")
+    print(df["rel_err_x"].describe())
+    print(df["rel_err_x"].nlargest(10))
+    print("----Rel error y description----- ")
+    print(df["rel_err_y"].describe())
+    print(df["rel_err_y"].nlargest(10))
+    if save:
+        fig1.savefig(os.path.join(working_dir_path, "plot_Bmod.png"))
+        fig2.savefig(os.path.join(working_dir_path,"plot_B_mod_error.png"))
+        fig3.savefig(os.path.join(working_dir_path,"plot_Bx_By.png"))
+        fig4.savefig(os.path.join(working_dir_path,"plot_relative_error_x_y.png"))
+        fig5.savefig(os.path.join(working_dir_path,"plot_difference_Bx_By.png"))
+
+    displayWaitAndClose(waitTimeBeforeMessage=.1, waitTimeAfterMessage=10)
 
 def plot_roxie_coil(roxie_data):
     xPos = []
     yPos = []
     xBarePos = []
     yBarePos = []
     iPos = []
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.5.0/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.5.0/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.5.0/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.5.0/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.5.0/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.5.0/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/misc.py` & `steam-sdk-2023.5.0/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.5.0/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.5.0/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.5.0/steam_sdk/utils/utils_PC.py`

 * *Files 11% similar despite different names*

```diff
@@ -99,29 +99,30 @@
     current = Time_Current[1]
     return np.round(time[np.argmin(abs(current - I_final))], 4)
 
 
 
 def calculate_t_PC_off_one(t_start: float, I_start: float, I_end: float, dI_dt: float, dI_dt_2: float, t_plateau: float, I_off: float):
     delta_t_parabolic = abs(dI_dt / dI_dt_2)
-    delta_I_parabolic = 0.5 * dI_dt_2 * delta_t_parabolic ** 2
-    delta_I_linear = I_end - I_start - 2 * delta_I_parabolic
+    delta_I_parabolic = 0.5 * abs(dI_dt_2) * delta_t_parabolic ** 2
+    delta_I_linear = abs(I_end - I_start) - 2 * delta_I_parabolic
     delta_t_linear = abs(delta_I_linear / dI_dt)
+    delta_Ioff_Istart = abs(I_off - I_start)
+    I_start, I_off, dI_dt = abs(I_start), abs(I_off), abs(dI_dt)
+
     if I_off < 2 * delta_I_parabolic:
-        I_off = 0
-        raise Exception('I_target < 2 * I_parabolic')
-    elif delta_I_parabolic < 0: # case to be discussed before removal
-        delta_t_linear = (I_end - I_start - delta_I_parabolic)/dI_dt
-        t_PC_off = t_start + delta_t_parabolic + delta_t_linear
-    elif I_off < I_start + delta_I_parabolic:
-        t_PC_off = t_start + np.sqrt( (I_off - I_start) / 0.5 / dI_dt_2)
-    elif I_off < I_start + delta_I_parabolic + delta_I_linear:
-        t_PC_off = t_start + delta_t_parabolic + (I_off - I_start - delta_I_parabolic) / dI_dt
-    elif I_off < I_start + delta_I_parabolic + delta_I_linear + delta_I_parabolic:
-        t_PC_off = t_start + delta_t_parabolic + delta_t_linear + np.sqrt((I_off - I_start - delta_I_parabolic - delta_I_linear) / 0.5 / dI_dt_2)
+        #I_off = 0
+        print("Warning: I_off is less than 2 times delta_I_parabolic.")
+        t_PC_off = 9999  # a very high value hard coded
+    elif delta_Ioff_Istart < delta_I_parabolic:
+        t_PC_off = t_start + np.sqrt( delta_Ioff_Istart / 0.5 / dI_dt_2)
+    elif delta_Ioff_Istart < delta_I_parabolic + delta_I_linear:
+        t_PC_off = t_start + delta_t_parabolic + (delta_Ioff_Istart - delta_I_parabolic) / dI_dt
+    elif delta_Ioff_Istart < delta_I_parabolic + delta_I_linear + delta_I_parabolic:
+        t_PC_off = t_start + delta_t_parabolic + delta_t_linear + np.sqrt((delta_Ioff_Istart - delta_I_parabolic - delta_I_linear) / 0.5 / dI_dt_2)
     else:
         t_PC_off = t_start + 2 * delta_t_parabolic + delta_t_linear + t_plateau
     return t_PC_off
 
 
 def calculate_t_PC_off(t_start: float, I_start: float, I_end: List[float], dI_dt: List[float], dI_dt_2: List[float], t_plateau: List[float], I_off: float):
     if not isinstance(I_end, list):
@@ -137,14 +138,17 @@
     I_start_k = I_start
     # Iterate over the different defined ramps
     for k, (I_end_k, dI_dt_k, dI_dt_2_k, t_plateau_k) in enumerate(zip(I_end, dI_dt, dI_dt_2, t_plateau)):
         print(k, I_end_k, dI_dt_k, dI_dt_2_k, t_plateau_k)
         if k + 1 < len(I_end):
             t_PC_off_k = calculate_t_PC_off_one(t_start=t_PC_off_k, I_start=I_start_k, I_end=I_end_k, dI_dt=dI_dt_k, dI_dt_2=dI_dt_2_k, t_plateau=t_plateau_k, I_off=I_end_k)
             I_start_k = I_end_k
+            if t_PC_off_k == 9999:
+                I_start_k = 0
+                continue
         else:
             # At the last ramp, check the time at which I_off is reached
             t_PC_off = calculate_t_PC_off_one(t_start=t_PC_off_k, I_start=I_start_k, I_end=I_end_k, dI_dt=dI_dt_k, dI_dt_2=dI_dt_2_k, t_plateau=t_plateau_k, I_off=I_off)
     return t_PC_off
```

### Comparing `steam-sdk-2023.4.3/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.5.0/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.5.0/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.5.0/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/wrappers/java/SING/jars/steam-sing.jar` & `steam-sdk-2023.5.0/steam_sdk/wrappers/java/SING/jars/steam-sing.jar`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.5.0/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.4.3/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.5.0/steam_sdk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.4.3
+Version: 2023.5.0
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,CERN,API,SDK
+Keywords: API,SDK,CERN,STEAM
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.4.3/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.5.0/steam_sdk.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,15 @@
 steam_sdk/data/DataModelConductor.py
 steam_sdk/data/DataModelMagnet.py
 steam_sdk/data/DataParsimConductor.py
 steam_sdk/data/DataParsims.py
 steam_sdk/data/DataProteCCT.py
 steam_sdk/data/DataPyBBQ.py
 steam_sdk/data/DataRoxieParser.py
+steam_sdk/data/DataSIGMA.py
 steam_sdk/data/DataSettings.py
 steam_sdk/data/DataSignal.py
 steam_sdk/data/DictionaryLEDET.py
 steam_sdk/data/DictionaryProteCCT.py
 steam_sdk/data/DictionaryPyBBQ.py
 steam_sdk/data/Readme.md
 steam_sdk/data/TemplateLEDET.py
@@ -111,14 +112,15 @@
 steam_sdk/parsers/ParserMap2d.py
 steam_sdk/parsers/ParserMat.py
 steam_sdk/parsers/ParserPSPICE.py
 steam_sdk/parsers/ParserPdf.py
 steam_sdk/parsers/ParserProteCCT.py
 steam_sdk/parsers/ParserProtePyBBQ.py
 steam_sdk/parsers/ParserRoxie.py
+steam_sdk/parsers/ParserSIGMA.py
 steam_sdk/parsers/ParserTdms.py
 steam_sdk/parsers/ParserXYCE.py
 steam_sdk/parsers/ParserYAML.py
 steam_sdk/parsers/Readme.md
 steam_sdk/parsers/__init__.py
 steam_sdk/parsers/dict_to_in.py
 steam_sdk/parsers/templates/template_Dakota.in
@@ -126,31 +128,33 @@
 steam_sdk/parsims/ParsimDakota.py
 steam_sdk/parsims/ParsimEventCircuit.py
 steam_sdk/parsims/ParsimEventMagnet.py
 steam_sdk/parsims/ParsimSweep.py
 steam_sdk/parsims/Readme.md
 steam_sdk/parsims/__init__.py
 steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+steam_sdk/parsims/translation_dicts/event_column_names.yaml
+steam_sdk/plotters/PlotterAnalysis.py
+steam_sdk/plotters/PlotterMap2d.py
 steam_sdk/plotters/PlotterModel.py
 steam_sdk/plotters/PlotterParametric.py
 steam_sdk/plotters/PlotterRoxie.py
-steam_sdk/plotters/PlotterSIGMA.py
 steam_sdk/plotters/Readme.md
 steam_sdk/plotters/__init__.py
 steam_sdk/postprocs/PostprocsMetrics.py
 steam_sdk/postprocs/__init__.py
 steam_sdk/utils/MTF_reading_functions.py
 steam_sdk/utils/ModifyModelData.py
 steam_sdk/utils/ModifyModelDataMagnet.py
 steam_sdk/utils/ModifyModelDataconductor.py
 steam_sdk/utils/NumpyEncoder.py
 steam_sdk/utils/__init__.py
-steam_sdk/utils/builder_SIGMA_helpers.py
 steam_sdk/utils/clean_NaN_from_signal.py
 steam_sdk/utils/compare_two_parameters.py
+steam_sdk/utils/create_coordinate_file_SIGMA.py
 steam_sdk/utils/get_attribute_type.py
 steam_sdk/utils/isNaN.py
 steam_sdk/utils/make_folder_if_not_existing.py
 steam_sdk/utils/misc.py
 steam_sdk/utils/parse_str_to_list.py
 steam_sdk/utils/rgetattr.py
 steam_sdk/utils/rhasattr.py
```

### Comparing `steam-sdk-2023.4.3/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.5.0/steam_sdk.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -82,8 +82,8 @@
 tqdm==4.64.1
 traitlets==5.4.0
 typing_extensions==4.3.0
 urllib3==1.26.12
 watchdog==2.1.9
 wcwidth==0.2.5
 zipp==3.8.1
-steam-pysigma==2023.4.15
+steam-pysigma==2023.5.6
```

