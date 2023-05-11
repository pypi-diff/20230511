# Comparing `tmp/steam-sdk-2023.5.1.tar.gz` & `tmp/steam-sdk-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\steam-sdk-2023.5.1.tar", last modified: Thu May 11 15:44:46 2023, max compression
+gzip compressed data, was "dist\steam-sdk-2023.5.2.tar", last modified: Thu May 11 20:05:11 2023, max compression
```

## Comparing `steam-sdk-2023.5.1.tar` & `steam-sdk-2023.5.2.tar`

### file list

```diff
@@ -1,211 +1,211 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.087008 steam-sdk-2023.5.1/
--rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.5.1/.gitignore
--rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.5.1/.gitlab-ci.yml
--rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1550 2023-05-11 15:44:46.086012 steam-sdk-2023.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.5.1/Readme.md
--rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.5.1/mkdocs.yaml
--rw-rw-rw-   0        0        0     1685 2023-05-11 15:44:13.000000 steam-sdk-2023.5.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 15:44:46.087008 steam-sdk-2023.5.1/setup.cfg
--rw-rw-rw-   0        0        0      797 2023-05-11 15:44:13.000000 steam-sdk-2023.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.944390 steam-sdk-2023.5.1/steam_sdk/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.949376 steam-sdk-2023.5.1/steam_sdk/analyses/
--rw-rw-rw-   0        0        0   119712 2023-05-11 15:13:46.000000 steam-sdk-2023.5.1/steam_sdk/analyses/AnalysisSTEAM.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.950374 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.952371 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.958352 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
--rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
--rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
--rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
--rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
--rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.960347 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
--rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.963339 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.965334 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
--rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.968340 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
--rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
--rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
--rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.971318 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
--rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.980295 steam-sdk-2023.5.1/steam_sdk/builders/
--rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderFiQuS.py
--rw-rw-rw-   0        0        0   162619 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderLEDET.py
--rw-rw-rw-   0        0        0    34260 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderModel.py
--rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderProteCCT.py
--rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderPyBBQ.py
--rw-rw-rw-   0        0        0    12076 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/builders/BuilderSIGMA.py
--rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/builders/Readme.md
--rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.5.1/steam_sdk/builders/SelfMutualInductanceCalculation.py
--rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.5.1/steam_sdk/builders/Solenoids.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/builders/__init__.py
--rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/builders/geometricFunctions.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.981291 steam-sdk-2023.5.1/steam_sdk/configs/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.982288 steam-sdk-2023.5.1/steam_sdk/configs/plotters/
--rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.984283 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.987275 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/__init__.py
--rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
--rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
--rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/Readme.md
--rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.988273 steam-sdk-2023.5.1/steam_sdk/configs/users/
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/configs/users/Readme.md
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.989270 steam-sdk-2023.5.1/steam_sdk/cosims/
--rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/cosims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/cosims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.011211 steam-sdk-2023.5.1/steam_sdk/data/
--rw-rw-rw-   0        0        0    10171 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataAnalysis.py
--rw-rw-rw-   0        0        0     8040 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataConductor.py
--rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.5.1/steam_sdk/data/DataDakota.py
--rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataEventCircuit.py
--rw-rw-rw-   0        0        0     4193 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataEventMagnet.py
--rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/data/DataFiQuS.py
--rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.5.1/steam_sdk/data/DataLEDET.py
--rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/DataModelCircuit.py
--rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/data/DataModelConductor.py
--rw-rw-rw-   0        0        0    35546 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataModelMagnet.py
--rw-rw-rw-   0        0        0     2636 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataParsimConductor.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/DataParsims.py
--rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/DataProteCCT.py
--rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.5.1/steam_sdk/data/DataPyBBQ.py
--rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/data/DataRoxieParser.py
--rw-rw-rw-   0        0        0     6791 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataSIGMA.py
--rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.5.1/steam_sdk/data/DataSettings.py
--rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.5.1/steam_sdk/data/DataSignal.py
--rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.5.1/steam_sdk/data/DictionaryLEDET.py
--rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/DictionaryProteCCT.py
--rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.5.1/steam_sdk/data/DictionaryPyBBQ.py
--rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/Readme.md
--rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.5.1/steam_sdk/data/TemplateLEDET.py
--rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/TemplateProteCCT.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.020187 steam-sdk-2023.5.1/steam_sdk/drivers/
--rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverAnalysis.py
--rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverDakota.py
--rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverFiQuS.py
--rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverLEDET.py
--rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverPSPICE.py
--rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverProteCCT.py
--rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverPyBBQ.py
--rw-rw-rw-   0        0        0     2832 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverSIGMA.py
--rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.5.1/steam_sdk/drivers/DriverXYCE.py
--rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.022195 steam-sdk-2023.5.1/steam_sdk/drivers/temp/
--rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/temp/postLEDET.py
--rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/temp/runLEDET.py
--rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/drivers/temp/simLEDET.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.043126 steam-sdk-2023.5.1/steam_sdk/parsers/
--rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/CSD_Reader.py
--rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserCOMSOLToTxt.py
--rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserCond2d.py
--rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserCsd.py
--rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserCsv.py
--rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserDakota.py
--rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserDatToCsv.py
--rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserExcel.py
--rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserFiQuS.py
--rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserLEDET.py
--rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserMap2d.py
--rw-rw-rw-   0        0        0    10920 2023-05-11 15:23:35.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserMat.py
--rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserPSPICE.py
--rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserPdf.py
--rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserProteCCT.py
--rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserProtePyBBQ.py
--rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserRoxie.py
--rw-rw-rw-   0        0        0     1928 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserSIGMA.py
--rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserTdms.py
--rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserXYCE.py
--rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.5.1/steam_sdk/parsers/ParserYAML.py
--rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/__init__.py
--rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsers/dict_to_in.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.044123 steam-sdk-2023.5.1/steam_sdk/parsers/templates/
--rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.5.1/steam_sdk/parsers/templates/template_Dakota.in
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.051104 steam-sdk-2023.5.1/steam_sdk/parsims/
--rw-rw-rw-   0        0        0    61593 2023-05-11 11:02:01.000000 steam-sdk-2023.5.1/steam_sdk/parsims/ParsimConductor.py
--rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsims/ParsimDakota.py
--rw-rw-rw-   0        0        0    70148 2023-05-11 15:13:46.000000 steam-sdk-2023.5.1/steam_sdk/parsims/ParsimEventCircuit.py
--rw-rw-rw-   0        0        0    47683 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/parsims/ParsimEventMagnet.py
--rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.5.1/steam_sdk/parsims/ParsimSweep.py
--rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsims/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/parsims/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.052102 steam-sdk-2023.5.1/steam_sdk/parsims/translation_dicts/
--rw-rw-rw-   0        0        0     2329 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
--rw-rw-rw-   0        0        0     2016 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.058086 steam-sdk-2023.5.1/steam_sdk/plotters/
--rw-rw-rw-   0        0        0     8053 2023-05-11 15:13:46.000000 steam-sdk-2023.5.1/steam_sdk/plotters/PlotterAnalysis.py
--rw-rw-rw-   0        0        0    20399 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/plotters/PlotterMap2d.py
--rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/plotters/PlotterModel.py
--rw-rw-rw-   0        0        0    22987 2023-05-11 15:23:13.000000 steam-sdk-2023.5.1/steam_sdk/plotters/PlotterParametric.py
--rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/plotters/PlotterRoxie.py
--rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/plotters/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/plotters/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.060080 steam-sdk-2023.5.1/steam_sdk/postprocs/
--rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/postprocs/PostprocsMetrics.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/postprocs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.076038 steam-sdk-2023.5.1/steam_sdk/utils/
--rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.5.1/steam_sdk/utils/MTF_reading_functions.py
--rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelData.py
--rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelDataMagnet.py
--rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelDataconductor.py
--rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/NumpyEncoder.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/__init__.py
--rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/clean_NaN_from_signal.py
--rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.5.1/steam_sdk/utils/compare_two_parameters.py
--rw-rw-rw-   0        0        0      590 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/utils/create_coordinate_file_SIGMA.py
--rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.5.1/steam_sdk/utils/get_attribute_type.py
--rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/isNaN.py
--rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/make_folder_if_not_existing.py
--rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/misc.py
--rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.5.1/steam_sdk/utils/parse_str_to_list.py
--rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/rgetattr.py
--rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.5.1/steam_sdk/utils/rhasattr.py
--rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/sgetattr.py
--rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/tic_toc.py
--rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/utils/unique.py
--rw-rw-rw-   0        0        0     7005 2023-05-11 10:23:04.000000 steam-sdk-2023.5.1/steam_sdk/utils/utils_PC.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.079030 steam-sdk-2023.5.1/steam_sdk/viewers/
--rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.5.1/steam_sdk/viewers/Viewer.py
--rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/viewers/ViewerMeas.py
--rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/viewers/ViewerSim.py
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/viewers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.082024 steam-sdk-2023.5.1/steam_sdk/wrappers/
--rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/Readme.md
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.083019 steam-sdk-2023.5.1/steam_sdk/wrappers/java/
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.084017 steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:46.085013 steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/jars/
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/jars/__init__.py
--rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
--rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/java/__init__.py
--rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.5.1/steam_sdk/wrappers/wrapper_yaml.py
-drwxrwxrwx   0        0        0        0 2023-05-11 15:44:45.948380 steam-sdk-2023.5.1/steam_sdk.egg-info/
--rw-rw-rw-   0        0        0     1550 2023-05-11 15:44:19.000000 steam-sdk-2023.5.1/steam_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     7480 2023-05-11 15:44:44.000000 steam-sdk-2023.5.1/steam_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 15:44:19.000000 steam-sdk-2023.5.1/steam_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1596 2023-05-11 15:44:19.000000 steam-sdk-2023.5.1/steam_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 15:44:19.000000 steam-sdk-2023.5.1/steam_sdk.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.137557 steam-sdk-2023.5.2/
+-rw-rw-rw-   0        0        0     3743 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/.gitignore
+-rw-rw-rw-   0        0        0     1963 2023-02-01 10:40:32.000000 steam-sdk-2023.5.2/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0      122 2023-02-02 14:39:18.000000 steam-sdk-2023.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1550 2023-05-11 20:05:11.134565 steam-sdk-2023.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1147 2023-04-11 10:02:40.000000 steam-sdk-2023.5.2/Readme.md
+-rw-rw-rw-   0        0        0     5370 2023-01-20 13:20:13.000000 steam-sdk-2023.5.2/mkdocs.yaml
+-rw-rw-rw-   0        0        0     1685 2023-05-11 15:44:13.000000 steam-sdk-2023.5.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-11 20:05:11.137557 steam-sdk-2023.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      797 2023-05-11 20:04:23.000000 steam-sdk-2023.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.831355 steam-sdk-2023.5.2/steam_sdk/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.846315 steam-sdk-2023.5.2/steam_sdk/analyses/
+-rw-rw-rw-   0        0        0   120112 2023-05-11 20:01:59.000000 steam-sdk-2023.5.2/steam_sdk/analyses/AnalysisSTEAM.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.847313 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.849307 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    23368 2022-10-17 13:51:31.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.856289 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0    16757 2022-10-07 10:25:49.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py
+-rw-rw-rw-   0        0        0     2800 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py
+-rw-rw-rw-   0        0        0     6828 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py
+-rw-rw-rw-   0        0        0    95412 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py
+-rw-rw-rw-   0        0        0     2652 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py
+-rw-rw-rw-   0        0        0     2341 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.858282 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/__init__.py
+-rw-rw-rw-   0        0        0    22374 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.863270 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4527 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     2921 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.865270 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/__init__.py
+-rw-rw-rw-   0        0        0    29433 2022-09-29 08:14:52.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.871248 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/__init__.py
+-rw-rw-rw-   0        0        0     5210 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py
+-rw-rw-rw-   0        0        0     4704 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py
+-rw-rw-rw-   0        0        0     4852 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.873243 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/__init__.py
+-rw-rw-rw-   0        0        0     1307 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.886208 steam-sdk-2023.5.2/steam_sdk/builders/
+-rw-rw-rw-   0        0        0    10098 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderFiQuS.py
+-rw-rw-rw-   0        0        0   162619 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderLEDET.py
+-rw-rw-rw-   0        0        0    34260 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderModel.py
+-rw-rw-rw-   0        0        0    12686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderProteCCT.py
+-rw-rw-rw-   0        0        0     6749 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderPyBBQ.py
+-rw-rw-rw-   0        0        0    12076 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/builders/BuilderSIGMA.py
+-rw-rw-rw-   0        0        0      246 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/Readme.md
+-rw-rw-rw-   0        0        0    11689 2023-01-20 13:20:13.000000 steam-sdk-2023.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py
+-rw-rw-rw-   0        0        0     7941 2022-12-02 14:32:36.000000 steam-sdk-2023.5.2/steam_sdk/builders/Solenoids.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/builders/__init__.py
+-rw-rw-rw-   0        0        0     8352 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/builders/geometricFunctions.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.887205 steam-sdk-2023.5.2/steam_sdk/configs/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.890197 steam-sdk-2023.5.2/steam_sdk/configs/plotters/
+-rw-rw-rw-   0        0        0      294 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.893190 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.896182 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/__init__.py
+-rw-rw-rw-   0        0        0     9137 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml
+-rw-rw-rw-   0        0        0    32890 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx
+-rw-rw-rw-   0        0        0      174 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/Readme.md
+-rw-rw-rw-   0        0        0     1426 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.897179 steam-sdk-2023.5.2/steam_sdk/configs/users/
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/configs/users/Readme.md
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.900172 steam-sdk-2023.5.2/steam_sdk/cosims/
+-rw-rw-rw-   0        0        0       69 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/cosims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/cosims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.937072 steam-sdk-2023.5.2/steam_sdk/data/
+-rw-rw-rw-   0        0        0    10200 2023-05-11 20:01:58.000000 steam-sdk-2023.5.2/steam_sdk/data/DataAnalysis.py
+-rw-rw-rw-   0        0        0     8040 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataConductor.py
+-rw-rw-rw-   0        0        0     3281 2022-09-28 15:13:02.000000 steam-sdk-2023.5.2/steam_sdk/data/DataDakota.py
+-rw-rw-rw-   0        0        0     2865 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataEventCircuit.py
+-rw-rw-rw-   0        0        0     4193 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataEventMagnet.py
+-rw-rw-rw-   0        0        0     8492 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataFiQuS.py
+-rw-rw-rw-   0        0        0    10767 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/DataLEDET.py
+-rw-rw-rw-   0        0        0     4314 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelCircuit.py
+-rw-rw-rw-   0        0        0     5869 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelConductor.py
+-rw-rw-rw-   0        0        0    35546 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataModelMagnet.py
+-rw-rw-rw-   0        0        0     2636 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataParsimConductor.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataParsims.py
+-rw-rw-rw-   0        0        0     1995 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DataProteCCT.py
+-rw-rw-rw-   0        0        0     2105 2022-09-28 15:19:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataPyBBQ.py
+-rw-rw-rw-   0        0        0     7899 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/data/DataRoxieParser.py
+-rw-rw-rw-   0        0        0     6791 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSIGMA.py
+-rw-rw-rw-   0        0        0     1650 2023-03-14 14:45:17.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSettings.py
+-rw-rw-rw-   0        0        0     3204 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/data/DataSignal.py
+-rw-rw-rw-   0        0        0    22928 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryLEDET.py
+-rw-rw-rw-   0        0        0     4482 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryProteCCT.py
+-rw-rw-rw-   0        0        0     2902 2022-09-28 14:36:21.000000 steam-sdk-2023.5.2/steam_sdk/data/DictionaryPyBBQ.py
+-rw-rw-rw-   0        0        0      153 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/Readme.md
+-rw-rw-rw-   0        0        0    27540 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/data/TemplateLEDET.py
+-rw-rw-rw-   0        0        0     7903 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/TemplateProteCCT.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.947045 steam-sdk-2023.5.2/steam_sdk/drivers/
+-rw-rw-rw-   0        0        0     3151 2022-11-24 16:16:38.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverAnalysis.py
+-rw-rw-rw-   0        0        0     2711 2022-11-24 16:16:38.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverDakota.py
+-rw-rw-rw-   0        0        0     1299 2023-02-01 20:32:34.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverFiQuS.py
+-rw-rw-rw-   0        0        0     3482 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverLEDET.py
+-rw-rw-rw-   0        0        0     1924 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverPSPICE.py
+-rw-rw-rw-   0        0        0     2062 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverProteCCT.py
+-rw-rw-rw-   0        0        0     2219 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverPyBBQ.py
+-rw-rw-rw-   0        0        0     2832 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverSIGMA.py
+-rw-rw-rw-   0        0        0     1932 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/drivers/DriverXYCE.py
+-rw-rw-rw-   0        0        0      193 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.953030 steam-sdk-2023.5.2/steam_sdk/drivers/temp/
+-rw-rw-rw-   0        0        0    27295 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/postLEDET.py
+-rw-rw-rw-   0        0        0     1820 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/runLEDET.py
+-rw-rw-rw-   0        0        0     5459 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/drivers/temp/simLEDET.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.987936 steam-sdk-2023.5.2/steam_sdk/parsers/
+-rw-rw-rw-   0        0        0     4984 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/CSD_Reader.py
+-rw-rw-rw-   0        0        0      317 2023-04-13 13:06:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCOMSOLToTxt.py
+-rw-rw-rw-   0        0        0     2290 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCond2d.py
+-rw-rw-rw-   0        0        0     1077 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsd.py
+-rw-rw-rw-   0        0        0     6220 2022-10-17 13:51:31.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsv.py
+-rw-rw-rw-   0        0        0     1650 2023-01-17 13:00:56.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserDakota.py
+-rw-rw-rw-   0        0        0     1030 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserDatToCsv.py
+-rw-rw-rw-   0        0        0     8536 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserExcel.py
+-rw-rw-rw-   0        0        0     2287 2022-09-28 15:13:08.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserFiQuS.py
+-rw-rw-rw-   0        0        0    48056 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserLEDET.py
+-rw-rw-rw-   0        0        0    12436 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserMap2d.py
+-rw-rw-rw-   0        0        0    10920 2023-05-11 15:23:35.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserMat.py
+-rw-rw-rw-   0        0        0    61567 2023-04-03 16:34:32.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserPSPICE.py
+-rw-rw-rw-   0        0        0     4780 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserPdf.py
+-rw-rw-rw-   0        0        0     6838 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserProteCCT.py
+-rw-rw-rw-   0        0        0     2942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserProtePyBBQ.py
+-rw-rw-rw-   0        0        0    92213 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserRoxie.py
+-rw-rw-rw-   0        0        0     1928 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserSIGMA.py
+-rw-rw-rw-   0        0        0    11707 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserTdms.py
+-rw-rw-rw-   0        0        0    55281 2023-02-02 14:52:07.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserXYCE.py
+-rw-rw-rw-   0        0        0     4088 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/parsers/ParserYAML.py
+-rw-rw-rw-   0        0        0      113 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/__init__.py
+-rw-rw-rw-   0        0        0        2 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsers/dict_to_in.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.988935 steam-sdk-2023.5.2/steam_sdk/parsers/templates/
+-rw-rw-rw-   0        0        0      709 2022-11-16 07:50:44.000000 steam-sdk-2023.5.2/steam_sdk/parsers/templates/template_Dakota.in
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.007883 steam-sdk-2023.5.2/steam_sdk/parsims/
+-rw-rw-rw-   0        0        0    61649 2023-05-11 20:01:58.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimConductor.py
+-rw-rw-rw-   0        0        0      916 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimDakota.py
+-rw-rw-rw-   0        0        0    70148 2023-05-11 15:13:46.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventCircuit.py
+-rw-rw-rw-   0        0        0    47683 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventMagnet.py
+-rw-rw-rw-   0        0        0     1972 2023-01-23 16:45:50.000000 steam-sdk-2023.5.2/steam_sdk/parsims/ParsimSweep.py
+-rw-rw-rw-   0        0        0       72 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/parsims/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.014864 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/
+-rw-rw-rw-   0        0        0     2329 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml
+-rw-rw-rw-   0        0        0     2016 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/event_column_names.yaml
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.042789 steam-sdk-2023.5.2/steam_sdk/plotters/
+-rw-rw-rw-   0        0        0     8134 2023-05-11 20:01:59.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterAnalysis.py
+-rw-rw-rw-   0        0        0    20399 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterMap2d.py
+-rw-rw-rw-   0        0        0    39596 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterModel.py
+-rw-rw-rw-   0        0        0    22987 2023-05-11 15:23:13.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterParametric.py
+-rw-rw-rw-   0        0        0     8871 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/plotters/PlotterRoxie.py
+-rw-rw-rw-   0        0        0      130 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/plotters/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.054758 steam-sdk-2023.5.2/steam_sdk/postprocs/
+-rw-rw-rw-   0        0        0     5564 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/postprocs/PostprocsMetrics.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/postprocs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.119605 steam-sdk-2023.5.2/steam_sdk/utils/
+-rw-rw-rw-   0        0        0     2679 2023-03-14 14:37:52.000000 steam-sdk-2023.5.2/steam_sdk/utils/MTF_reading_functions.py
+-rw-rw-rw-   0        0        0    14942 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelData.py
+-rw-rw-rw-   0        0        0     4587 2023-01-17 13:00:56.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataMagnet.py
+-rw-rw-rw-   0        0        0     2745 2022-10-04 13:23:53.000000 steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataconductor.py
+-rw-rw-rw-   0        0        0      313 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/NumpyEncoder.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/clean_NaN_from_signal.py
+-rw-rw-rw-   0        0        0     3837 2023-02-06 16:31:24.000000 steam-sdk-2023.5.2/steam_sdk/utils/compare_two_parameters.py
+-rw-rw-rw-   0        0        0      590 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/create_coordinate_file_SIGMA.py
+-rw-rw-rw-   0        0        0     1279 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/get_attribute_type.py
+-rw-rw-rw-   0        0        0      167 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/isNaN.py
+-rw-rw-rw-   0        0        0      299 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/make_folder_if_not_existing.py
+-rw-rw-rw-   0        0        0     4512 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/misc.py
+-rw-rw-rw-   0        0        0     1592 2023-04-20 15:50:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/parse_str_to_list.py
+-rw-rw-rw-   0        0        0      388 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/rgetattr.py
+-rw-rw-rw-   0        0        0      460 2023-01-10 08:52:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/rhasattr.py
+-rw-rw-rw-   0        0        0      383 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/sgetattr.py
+-rw-rw-rw-   0        0        0      863 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/tic_toc.py
+-rw-rw-rw-   0        0        0      168 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/utils/unique.py
+-rw-rw-rw-   0        0        0     7005 2023-05-11 10:23:04.000000 steam-sdk-2023.5.2/steam_sdk/utils/utils_PC.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.122597 steam-sdk-2023.5.2/steam_sdk/viewers/
+-rw-rw-rw-   0        0        0    35919 2023-03-30 13:07:50.000000 steam-sdk-2023.5.2/steam_sdk/viewers/Viewer.py
+-rw-rw-rw-   0        0        0     6127 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/ViewerMeas.py
+-rw-rw-rw-   0        0        0     1667 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/ViewerSim.py
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/viewers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.125589 steam-sdk-2023.5.2/steam_sdk/wrappers/
+-rw-rw-rw-   0        0        0      154 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/Readme.md
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.126587 steam-sdk-2023.5.2/steam_sdk/wrappers/java/
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.127584 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:11.129578 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/__init__.py
+-rw-rw-rw-   0        0        0    72381 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar
+-rw-rw-rw-   0        0        0        0 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/java/__init__.py
+-rw-rw-rw-   0        0        0     1834 2022-09-27 21:41:33.000000 steam-sdk-2023.5.2/steam_sdk/wrappers/wrapper_yaml.py
+drwxrwxrwx   0        0        0        0 2023-05-11 20:05:10.842326 steam-sdk-2023.5.2/steam_sdk.egg-info/
+-rw-rw-rw-   0        0        0     1550 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     7480 2023-05-11 20:05:09.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1596 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-11 20:04:42.000000 steam-sdk-2023.5.2/steam_sdk.egg-info/top_level.txt
```

### Comparing `steam-sdk-2023.5.1/.gitignore` & `steam-sdk-2023.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/.gitlab-ci.yml` & `steam-sdk-2023.5.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/PKG-INFO` & `steam-sdk-2023.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,SDK,API,CERN
+Keywords: SDK,STEAM,API,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.1/Readme.md` & `steam-sdk-2023.5.2/Readme.md`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/mkdocs.yaml` & `steam-sdk-2023.5.2/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/requirements.txt` & `steam-sdk-2023.5.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/setup.py` & `steam-sdk-2023.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name='steam-sdk',
-    version="2023.5.1",
+    version="2023.5.2",
     author="STEAM Team",
     author_email="steam-team@cern.ch",
     description="Source code for APIs for STEAM tools.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://gitlab.cern.ch/steam/steam_sdk",
     keywords={'STEAM', 'API', 'SDK', 'CERN'},
```

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/AnalysisSTEAM.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/AnalysisSTEAM.py`

 * *Files 1% similar despite different names*

```diff
@@ -538,14 +538,20 @@
         software = step.software
         simulation_name = step.simulation_name
         simFileType = step.simFileType
         sim_numbers = step.simulation_numbers
         if simulation_name == 'from_last_parametric_list':
             sim_numbers = list(self.input_parsim_sweep_df.simulation_number.to_numpy())
             sim_names = list(self.input_parsim_sweep_df.simulation_name.to_numpy())
+        elif simulation_name == 'from_SetUpFolder_step':
+            sim_numbers = list(self.input_parsim_sweep_df.simulation_number.to_numpy())
+            for step_data in self.data_analysis.AnalysisStepDefinition.values():
+                if step_data.type == 'SetUpFolder':
+                    sim_name = step_data.simulation_name
+            sim_names = len(sim_numbers) * [sim_name]
         else:
             sim_names = [simulation_name] * len(sim_numbers)
         for sim_name, sim_number in zip(sim_names, sim_numbers):
             if verbose:
                 print('Running simulation of model {} #{} using {}.'.format(simulation_name, sim_number, software))
             # Run simulation
             self.run_sim(software, sim_name, sim_number, simFileType, verbose)
@@ -1545,14 +1551,15 @@
 
         :param step: instance of ParsimConductor step
         :param verbose: if true displays more information
         '''
         # Unpack inputs
         model_name = step.model_name
         case_model = step.case_model
+        magnet_name = step.magnet_name
         software = step.software
         groups_to_coils = step.groups_to_coils
         length_to_coil = step.length_to_coil
         if not length_to_coil: length_to_coil = {}  # optimize coillen
         simulation_number = step.simulation_number
         input_file = step.input_file
         path_output_sweeper_csv = step.path_output_sweeper_csv
@@ -1611,18 +1618,18 @@
         if case_model == 'magnet':
             # create instance of ParsimConductor
             pc = ParsimConductor(verbose=verbose, model_data=self.list_models[model_name].model_data,
                                  dict_coilName_to_conductorIndex=dict_coilname_to_conductorindex,
                                  groups_to_coils=groups_to_coils, length_to_coil=length_to_coil,
                                  path_input_dir=Path(self.list_models[step.model_name].file_model_data).parent)
             # read the conductor database
-            pc.read_from_input(path_input_file=input_file, magnet_name=self.data_analysis.GeneralParameters.model.name,
+            pc.read_from_input(path_input_file=input_file, magnet_name=magnet_name,
                                strand_critical_current_measurements=strand_critical_current_measurements)
             # write a sweeper csv file
-            pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name, # TODO simulation_name should be step variable in definition, model_name ist not step name
+            pc.write_conductor_parameter_file(path_output_file=path_output_sweeper_csv, simulation_name=model_name, # TODO simulation_name should be step variable in definition, model_name ist not step name?
                                               simulation_number=simulation_number)
 
             # create parsim sweep step with newly created sweeper csv file and run it
             parsim_sweep_step = ParametricSweep(type='ParametricSweep', input_sweep_file=path_output_sweeper_csv, # TODO rename teh class to ParametricSweepStep? ParsimConductor is no step class and ParametricSweep is
                                                 model_name=model_name, case_model=case_model, software=software, verbose=verbose)
             self.run_parsim_sweep(parsim_sweep_step, verbose=verbose, revert=False)
         else:
```

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/analysis_short_circuit_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/calculate_short_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/copy_input_files.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_common_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_magnet_specific_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_short_circuit_analysis_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/analysis_short_circuit_LEDET_1/utils/set_simulations_to_prepare_run.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/co_simulation_QH_PyBBQ_LEDET_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/calculate_quench_propagation_velocity.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_conductor_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/co_simulation_QH_PyBBQ_LEDET_MBRD_validation_1/utils/create_magnet_analysis_file.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py` & `steam-sdk-2023.5.2/steam_sdk/analyses/custom_analyses/custom_function_test_1/custom_function_test_1.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderFiQuS.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderModel.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderPyBBQ.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/BuilderSIGMA.py` & `steam-sdk-2023.5.2/steam_sdk/builders/BuilderSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/SelfMutualInductanceCalculation.py` & `steam-sdk-2023.5.2/steam_sdk/builders/SelfMutualInductanceCalculation.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/Solenoids.py` & `steam-sdk-2023.5.2/steam_sdk/builders/Solenoids.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/builders/geometricFunctions.py` & `steam-sdk-2023.5.2/steam_sdk/builders/geometricFunctions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml` & `steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/file_used_for_testing.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx` & `steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/LEDET/variableNamesDescriptions.xlsx`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/configs/tools_defaults/ToolDefaultReader.py` & `steam-sdk-2023.5.2/steam_sdk/configs/tools_defaults/ToolDefaultReader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataAnalysis.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,14 +259,15 @@
     """
         Level 2: Analysis step to write stimulus file from coil csv file
     """
     type: Literal['ParsimConductor']
     model_name: str = None
     case_model: str = None
     input_file: str = None
+    magnet_name: str = None
     software: List[str] = []
     simulation_number: int = None
     strand_critical_current_measurements: List[StrandCriticalCurrentMeasurement] = []
     groups_to_coils: Dict[str, List[int]] = {}
     length_to_coil: Dict[str, float] = {}
     path_output_sweeper_csv: str = None
```

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataConductor.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataDakota.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataEventCircuit.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataEventMagnet.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataFiQuS.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataModelCircuit.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataModelCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataModelConductor.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataModelConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataModelMagnet.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataModelMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataParsimConductor.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataParsimConductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataPyBBQ.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataRoxieParser.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataRoxieParser.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataSIGMA.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataSettings.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataSettings.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DataSignal.py` & `steam-sdk-2023.5.2/steam_sdk/data/DataSignal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DictionaryLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/data/DictionaryLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DictionaryProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/data/DictionaryProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/DictionaryPyBBQ.py` & `steam-sdk-2023.5.2/steam_sdk/data/DictionaryPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/TemplateLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/data/TemplateLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/data/TemplateProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/data/TemplateProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverAnalysis.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverAnalysis.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverDakota.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverFiQuS.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverPSPICE.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverPyBBQ.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverPyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverSIGMA.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/DriverXYCE.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/DriverXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/temp/postLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/temp/postLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/temp/runLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/temp/runLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/drivers/temp/simLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/drivers/temp/simLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/CSD_Reader.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/CSD_Reader.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserCond2d.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCond2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserCsd.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsd.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserCsv.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserDakota.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserDatToCsv.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserDatToCsv.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserExcel.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserExcel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserFiQuS.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserFiQuS.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserLEDET.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserLEDET.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserMap2d.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserMat.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserMat.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserPSPICE.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserPSPICE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserPdf.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserPdf.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserProteCCT.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserProteCCT.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserProtePyBBQ.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserProtePyBBQ.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserRoxie.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserSIGMA.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserSIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserTdms.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserTdms.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserXYCE.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserXYCE.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/ParserYAML.py` & `steam-sdk-2023.5.2/steam_sdk/parsers/ParserYAML.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsers/templates/template_Dakota.in` & `steam-sdk-2023.5.2/steam_sdk/parsers/templates/template_Dakota.in`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/ParsimConductor.py` & `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimConductor.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         :param dict_sweeper: The dictionary where the optimized half-turn length will be stored, in the format {attributeNameDataModelMagnet: newValue}
         """
         ht_len = [0.0 for _ in range(self.number_of_groups)]
 
         # looping through the coils
         for coil_name, coil in self.data_parsim_conductor.Coils.items():
             if not coil.coil_resistance_room_T:
-                warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Using default value from modelData.')
+                warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Using default value for half_turn_length from modelData.')
                 continue
             original_conductor = self.model_data.Conductors[self.dict_coilName_to_conductorIndex[coil_name]]
             # calculate the optimized coil length for every group in the conductor sample separately
             for sample in coil.conductorSamples:
                 # optimize the length for this coil with one conductor
                 L = self.__optimize_coil_length_with_resistance_meas(sample, coil_name, original_conductor, coil)
                 # for every conductorSamples add the optimized lengths together (to later make the average)
@@ -540,15 +540,15 @@
             for name, val in Jc_avg_dict.items():
                 dict_sweeper[sweeper_cond_name + 'Jc_fit.' + name] = val
 
             # optimize the fraction of copper with the resistance measurement at room temperature
             if flag_optimize_fCu:
                 # check if RT measurement is defined
                 if not coil.coil_resistance_room_T:
-                    warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database.')
+                    warnings.warn(f'No room temperature resistance measurement for coil "{coil_name}" was found in database. Not optimizing fraction of copper.')
                     continue
                 # calculate Cu_noCu for every conductor sample and use mean value
                 list_optimized_Cu_noCu = []
                 for sample in coil.conductorSamples:
                     list_optimized_Cu_noCu.append(self.__optimize_fCu_with_resistance_meas(sample, coil_name, self.model_data.Conductors[idx], coil))
                 dict_sweeper[sweeper_cond_name + 'strand.Cu_noCu_in_strand'] = np.mean(list_optimized_Cu_noCu)
```

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/ParsimDakota.py` & `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimDakota.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/ParsimEventCircuit.py` & `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventCircuit.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/ParsimEventMagnet.py` & `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimEventMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/ParsimSweep.py` & `steam-sdk-2023.5.2/steam_sdk/parsims/ParsimSweep.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml` & `steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/conductor_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/parsims/translation_dicts/event_column_names.yaml` & `steam-sdk-2023.5.2/steam_sdk/parsims/translation_dicts/event_column_names.yaml`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/plotters/PlotterAnalysis.py` & `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterAnalysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
                     if use_markers:     # user
                         marker = markers[i]
                     else:
                         marker = 'None'
                     if len(self.values) == 3:
                         label = f'{magnet_label},{value}:{leng + sim_names[sim_nr]}'
                     else:
-                        label = f'{magnet_label}:{leng + sim_names[sim_nr]}'
+                        #label = f'{magnet_label}:{leng + sim_names[sim_nr]}'
+                        label = f'{sim_nr}'
                     ax.plot(self.time_data[magnet_label][self.time_name][sim_nr], self.data[magnet_label][value][sim_nr],
                             markevery=20, marker=marker, label=label)
                     i += 1
         ax.tick_params(labelsize=self.cs['font_size'])
         ax.set_xlabel(f"Time (s)", size=self.cs['font_size'])#.set_fontproperties(font)
         if len(self.values) == 3:   # CLIQ currents plot
             value = '$I_{A}, I_{B}, I_{CLIQ}$'
@@ -112,43 +113,44 @@
         print(self.data)
 
 if __name__ == "__main__":
     base_path = r"C:\tempLEDET\LEDET"   # path to ledet folder
     model_names_list = [['robust_12T_50_mm_MQXF_cable_5_blocks_V2'], ['robust_12T_50_mm_MQXF_cable_6_blocks_V2'], ['robust_12T_56_mm_MQXF_cable_6_blocks_V2']]
     model_labels_list = [['50mm,5b'], ['50mm,6b'], ['56mm,6b']]
 
-    # model_names = ['robust_12T_50_mm_MQXF_cable_5_blocks_V2']
-    # model_labels = ['50mm,5b']
+    model_names = ['robust_12T_50_mm_MQXF_cable_5_blocks_V2']
+    model_labels = ['50mm,5b']
     # model_names = ['robust_12T_50_mm_MQXF_cable_6_blocks_V2']
     # model_labels = ['50mm,6b']
     # model_names = ['robust_12T_56_mm_MQXF_cable_6_blocks_V2']
     # model_labels = ['56mm,6b']
     # sim_nr_list_of_lists = [[13, 113], [13, 113], [13, 113]]
     # #sim_nr_list_of_lists = [[3, 103], [3, 103], [3, 103]]
     # sim_nr_list_of_lists = [[3], [3], [3]]
     # sim_nr_list_of_lists = [[3]]
     #sim_nr_list_of_lists = [[3, 13], [3, 13], [3, 13]]
     #sim_nr_list_of_lists = [[13], [13], [13]]
 
     sim_nr_list_of_lists = [[1, 2, 3, 13, 4, 14, 5, 6, 16, 7, 17]]
+    sim_nr_list_of_lists = [[303]]
     #sim_nr_list_of_lists = [[101, 102, 103, 113, 104, 114, 105, 106, 116, 107, 117]]
 
-    sim_nr_list_of_lists = [[3, 13, 4, 14, 6, 16, 7, 17]]
-    sim_nr_list_of_lists = [[103, 113, 104, 114, 106, 116, 107, 117]]
+    #sim_nr_list_of_lists = [[3, 13, 4, 14, 6, 16, 7, 17]]
+    #sim_nr_list_of_lists = [[103, 113, 104, 114, 106, 116, 107, 117]]
     #values = ['$I_{A}$', '$I_{B}$', '$I_{CLIQ}$']
 
     #values = ['$T_{max}$']
     #values = ['$T_{max adb}$']
     #values = ['$U_{max}$']
     #values = ['$U_{min}$']
     #values = ['$R_{mag}$']
-    values = ['$I_{A}$']
+    #values = ['$I_{A}$']
     values = ['$I_{CLIQ}$']
     style = 'presentation'
 
 
     pa = PlotterAnalysis(base_path)
     pa.set_plot_style(style)
     for model_names, model_labels in zip(model_names_list, model_labels_list):
         pa.read_data(model_names, model_labels, sim_nr_list_of_lists, values)
-        pa.plot_selected_vs_time(use_markers=0, save=1)
+        pa.plot_selected_vs_time(use_markers=0, save=0)
     #pa.print_data()
```

### Comparing `steam-sdk-2023.5.1/steam_sdk/plotters/PlotterMap2d.py` & `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterMap2d.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/plotters/PlotterModel.py` & `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterModel.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/plotters/PlotterParametric.py` & `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterParametric.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/plotters/PlotterRoxie.py` & `steam-sdk-2023.5.2/steam_sdk/plotters/PlotterRoxie.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/postprocs/PostprocsMetrics.py` & `steam-sdk-2023.5.2/steam_sdk/postprocs/PostprocsMetrics.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/MTF_reading_functions.py` & `steam-sdk-2023.5.2/steam_sdk/utils/MTF_reading_functions.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelData.py` & `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelData.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelDataMagnet.py` & `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataMagnet.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/ModifyModelDataconductor.py` & `steam-sdk-2023.5.2/steam_sdk/utils/ModifyModelDataconductor.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/clean_NaN_from_signal.py` & `steam-sdk-2023.5.2/steam_sdk/utils/clean_NaN_from_signal.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/compare_two_parameters.py` & `steam-sdk-2023.5.2/steam_sdk/utils/compare_two_parameters.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/create_coordinate_file_SIGMA.py` & `steam-sdk-2023.5.2/steam_sdk/utils/create_coordinate_file_SIGMA.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/get_attribute_type.py` & `steam-sdk-2023.5.2/steam_sdk/utils/get_attribute_type.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/misc.py` & `steam-sdk-2023.5.2/steam_sdk/utils/misc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/parse_str_to_list.py` & `steam-sdk-2023.5.2/steam_sdk/utils/parse_str_to_list.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/tic_toc.py` & `steam-sdk-2023.5.2/steam_sdk/utils/tic_toc.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/utils/utils_PC.py` & `steam-sdk-2023.5.2/steam_sdk/utils/utils_PC.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/viewers/Viewer.py` & `steam-sdk-2023.5.2/steam_sdk/viewers/Viewer.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/viewers/ViewerMeas.py` & `steam-sdk-2023.5.2/steam_sdk/viewers/ViewerMeas.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/viewers/ViewerSim.py` & `steam-sdk-2023.5.2/steam_sdk/viewers/ViewerSim.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/wrappers/java/SING/jars/steam-sing.jar` & `steam-sdk-2023.5.2/steam_sdk/wrappers/java/SING/jars/steam-sing.jar`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk/wrappers/wrapper_yaml.py` & `steam-sdk-2023.5.2/steam_sdk/wrappers/wrapper_yaml.py`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk.egg-info/PKG-INFO` & `steam-sdk-2023.5.2/steam_sdk.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: steam-sdk
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: Source code for APIs for STEAM tools.
 Home-page: https://gitlab.cern.ch/steam/steam_sdk
 Author: STEAM Team
 Author-email: steam-team@cern.ch
 License: UNKNOWN
-Keywords: STEAM,SDK,API,CERN
+Keywords: SDK,STEAM,API,CERN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # STEAM_SDK
```

### Comparing `steam-sdk-2023.5.1/steam_sdk.egg-info/SOURCES.txt` & `steam-sdk-2023.5.2/steam_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `steam-sdk-2023.5.1/steam_sdk.egg-info/requires.txt` & `steam-sdk-2023.5.2/steam_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

