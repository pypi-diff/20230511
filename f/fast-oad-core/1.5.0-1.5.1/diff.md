# Comparing `tmp/fast_oad_core-1.5.0.tar.gz` & `tmp/fast_oad_core-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_oad_core-1.5.0.tar", max compression
+gzip compressed data, was "fast_oad_core-1.5.1.tar", max compression
```

## Comparing `fast_oad_core-1.5.0.tar` & `fast_oad_core-1.5.1.tar`

### file list

```diff
@@ -1,234 +1,234 @@
--rw-r--r--   0        0        0    32472 2023-04-27 14:57:11.135288 fast_oad_core-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0     3488 2023-04-27 14:57:11.135288 fast_oad_core-1.5.0/README.md
--rw-r--r--   0        0        0     4231 2023-04-27 14:57:32.796920 fast_oad_core-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     1186 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/__init__.py
--rw-r--r--   0        0        0      829 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/__init__.py
--rw-r--r--   0        0        0     1059 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/files.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/__init__.py
--rw-r--r--   0        0        0     2922 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/contents.py
--rw-r--r--   0        0        0     3581 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/copy.py
--rw-r--r--   0        0        0     3030 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/strings.py
--rw-r--r--   0        0        0     1858 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/_utils/testing.py
--rw-r--r--   0        0        0     3375 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/api.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/cmd/__init__.py
--rw-r--r--   0        0        0    30528 2023-04-27 14:57:11.147289 fast_oad_core-1.5.0/src/fastoad/cmd/api.py
--rw-r--r--   0        0        0    10473 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/cli.py
--rw-r--r--   0        0        0     2994 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/cli_utils.py
--rw-r--r--   0        0        0     1477 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/exceptions.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/resources/__init__.py
--rw-r--r--   0        0        0     2460 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/cmd/resources/fastoad.yml
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/configurations/__init__.py
--rw-r--r--   0        0        0     2974 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/constants.py
--rw-r--r--   0        0        0     1675 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/exceptions.py
--rw-r--r--   0        0        0     1087 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/__init__.py
--rw-r--r--   0        0        0    23361 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/analysis_and_plots.py
--rw-r--r--   0        0        0      905 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/exceptions.py
--rw-r--r--   0        0        0     4073 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/mission_viewer.py
--rw-r--r--   0        0        0    21069 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/optimization_viewer.py
--rw-r--r--   0        0        0    16093 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/gui/variable_viewer.py
--rw-r--r--   0        0        0      898 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/__init__.py
--rw-r--r--   0        0        0      882 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/__init__.py
--rw-r--r--   0        0        0    19153 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/configuration.py
--rw-r--r--   0        0        0     3154 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/exceptions.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/__init__.py
--rw-r--r--   0        0        0     4038 2023-04-27 14:57:11.151289 fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/configuration.json
--rw-r--r--   0        0        0     1558 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/formatter.py
--rw-r--r--   0        0        0     9033 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/variable_io.py
--rw-r--r--   0        0        0      976 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/__init__.py
--rw-r--r--   0        0        0     1065 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/constants.py
--rw-r--r--   0        0        0     1907 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/exceptions.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/__init__.py
--rw-r--r--   0        0        0    37628 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/legacy1.txt
--rw-r--r--   0        0        0     1476 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/resources/remove_duplicate_variables.py
--rw-r--r--   0        0        0     4869 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/translator.py
--rw-r--r--   0        0        0     8181 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_base.py
--rw-r--r--   0        0        0     1431 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_legacy.py
--rw-r--r--   0        0        0     3966 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_standard.py
--rw-r--r--   0        0        0      888 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/__init__.py
--rw-r--r--   0        0        0    10543 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/atmosphere.py
--rw-r--r--   0        0        0     1900 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/datacls.py
--rw-r--r--   0        0        0     9806 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/flight_point.py
--rw-r--r--   0        0        0     8996 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/model_base/propulsion.py
--rw-r--r--   0        0        0      949 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/__init__.py
--rw-r--r--   0        0        0      797 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/__init__.py
--rw-r--r--   0        0        0      807 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/__init__.py
--rw-r--r--   0        0        0     9057 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/base.py
--rw-r--r--   0        0        0     1705 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/exceptions.py
--rw-r--r--   0        0        0     6217 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/__init__.py
--rw-r--r--   0        0        0      988 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/exceptions.py
--rw-r--r--   0        0        0      896 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py
--rw-r--r--   0        0        0     1022 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py
--rw-r--r--   0        0        0     8930 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py
--rw-r--r--   0        0        0    23483 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py
--rw-r--r--   0        0        0    15608 2023-04-27 14:57:11.155289 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py
--rw-r--r--   0        0        0     9592 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json
--rw-r--r--   0        0        0     5090 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/schema.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/__init__.py
--rw-r--r--   0        0        0     9130 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/base.py
--rw-r--r--   0        0        0     1616 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/link_mtow.py
--rw-r--r--   0        0        0    10612 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission.py
--rw-r--r--   0        0        0     9878 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_run.py
--rw-r--r--   0        0        0    10152 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py
--rw-r--r--   0        0        0    21188 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/payload_range.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/__init__.py
--rw-r--r--   0        0        0     2229 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml
--rw-r--r--   0        0        0     5896 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml
--rw-r--r--   0        0        0     3624 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar.py
--rw-r--r--   0        0        0     4019 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar_modifier.py
--rw-r--r--   0        0        0     6561 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/routes.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/__init__.py
--rw-r--r--   0        0        0    11836 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/base.py
--rw-r--r--   0        0        0     4912 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/macro_segments.py
--rw-r--r--   0        0        0     1241 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/__init__.py
--rw-r--r--   0        0        0     7782 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/altitude_change.py
--rw-r--r--   0        0        0    10181 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/cruise.py
--rw-r--r--   0        0        0     2163 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/ground_speed_change.py
--rw-r--r--   0        0        0     1486 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/hold.py
--rw-r--r--   0        0        0     1648 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/mass_input.py
--rw-r--r--   0        0        0     2390 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/speed_change.py
--rw-r--r--   0        0        0     1887 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/start.py
--rw-r--r--   0        0        0     1135 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/__init__.py
--rw-r--r--   0        0        0     6038 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/end_of_takeoff.py
--rw-r--r--   0        0        0     3142 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/rotation.py
--rw-r--r--   0        0        0     2659 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/takeoff.py
--rw-r--r--   0        0        0     2063 2023-04-27 14:57:11.159290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/taxi.py
--rw-r--r--   0        0        0     2873 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/transition.py
--rw-r--r--   0        0        0    17916 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/time_step_base.py
--rw-r--r--   0        0        0     2245 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/performances/mission/util.py
--rw-r--r--   0        0        0     1695 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/models/variable_descriptions.txt
--rw-r--r--   0        0        0      805 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/__init__.py
--rw-r--r--   0        0        0    14623 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/_bundle_loader.py
--rw-r--r--   0        0        0    18578 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/_plugins.py
--rw-r--r--   0        0        0     1442 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/constants.py
--rw-r--r--   0        0        0     7475 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/exceptions.py
--rw-r--r--   0        0        0    19567 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/module_management/service_registry.py
--rw-r--r--   0        0        0       64 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/.gitignore
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/__init__.py
--rw-r--r--   0        0        0    14508 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/__init__.py
--rw-r--r--   0        0        0      922 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml
--rw-r--r--   0        0        0      935 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml
--rw-r--r--   0        0        0     1260 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml
--rw-r--r--   0        0        0     1227 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/__init__.py
--rw-r--r--   0        0        0    18684 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png
--rw-r--r--   0        0        0     5532 2023-04-27 14:57:11.163290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/problem_description.png
--rw-r--r--   0        0        0   134937 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/__init__.py
--rw-r--r--   0        0        0     1988 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/displacements.py
--rw-r--r--   0        0        0     1561 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py
--rw-r--r--   0        0        0     2150 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/stresses.py
--rw-r--r--   0        0        0      540 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt
--rw-r--r--   0        0        0     1670 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/weight.py
--rw-r--r--   0        0        0       37 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/.gitignore
--rw-r--r--   0        0        0    11579 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb
--rw-r--r--   0        0        0    34406 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb
--rw-r--r--   0        0        0    13485 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb
--rw-r--r--   0        0        0    55116 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb
--rw-r--r--   0        0        0    20123 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/__init__.py
--rw-r--r--   0        0        0      461 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/source_file.xml
--rw-r--r--   0        0        0     7146 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png
--rw-r--r--   0        0        0     6097 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png
--rw-r--r--   0        0        0   113972 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png
--rw-r--r--   0        0        0   125428 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/__init__.py
--rw-r--r--   0        0        0    29150 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png
--rw-r--r--   0        0        0    40682 2023-04-27 14:57:11.167290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png
--rw-r--r--   0        0        0    46219 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png
--rw-r--r--   0        0        0    18684 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png
--rw-r--r--   0        0        0    23022 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png
--rw-r--r--   0        0        0    11722 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png
--rw-r--r--   0        0        0    65293 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png
--rw-r--r--   0        0        0    32808 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/__init__.py
--rw-r--r--   0        0        0      866 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/__init__.py
--rw-r--r--   0        0        0      346 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/__init__.py
--rw-r--r--   0        0        0      485 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/mass.py
--rw-r--r--   0        0        0      982 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/__init__.py
--rw-r--r--   0        0        0      355 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/performance.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/sub_components/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/__init__.py
--rw-r--r--   0        0        0     1019 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/__init__.py
--rw-r--r--   0        0        0      687 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/__init__.py
--rw-r--r--   0        0        0      860 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py
--rw-r--r--   0        0        0     2288 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
--rw-r--r--   0        0        0     1036 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/__init__.py
--rw-r--r--   0        0        0      241 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/__init__.py
--rw-r--r--   0        0        0      806 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/__init__.py
--rw-r--r--   0        0        0      695 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/__init__.py
--rw-r--r--   0        0        0      946 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py
--rw-r--r--   0        0        0      389 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe_exercise.py
--rw-r--r--   0        0        0     1539 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py
--rw-r--r--   0        0        0     1586 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/__init__.py
--rw-r--r--   0        0        0      244 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/performance.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/__init__.py
--rw-r--r--   0        0        0     1580 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/__init__.py
--rw-r--r--   0        0        0      920 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/__init__.py
--rw-r--r--   0        0        0     1101 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/__init__.py
--rw-r--r--   0        0        0      458 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_induced_drag_coefficient.py
--rw-r--r--   0        0        0     1255 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
--rw-r--r--   0        0        0      579 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/__init__.py
--rw-r--r--   0        0        0      416 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/geometry.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/__init__.py
--rw-r--r--   0        0        0      358 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/compute_wing_area.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/__init__.py
--rw-r--r--   0        0        0      688 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/__init__.py
--rw-r--r--   0        0        0      531 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py
--rw-r--r--   0        0        0      850 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py
--rw-r--r--   0        0        0     1942 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py
--rw-r--r--   0        0        0     1918 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/__init__.py
--rw-r--r--   0        0        0      922 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/__init__.py
--rw-r--r--   0        0        0     1052 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/__init__.py
--rw-r--r--   0        0        0      578 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py
--rw-r--r--   0        0        0        0 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/__init__.py
--rw-r--r--   0        0        0     1913 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py
--rw-r--r--   0        0        0     2102 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py
--rw-r--r--   0        0        0     1057 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py
--rw-r--r--   0        0        0      825 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py
--rw-r--r--   0        0        0     1308 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/README.md
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.171290 fast_oad_core-1.5.0/src/fastoad/notebooks/__init__.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/__init__.py
--rw-r--r--   0        0        0     4032 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/_utils.py
--rw-r--r--   0        0        0     1378 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/exceptions.py
--rw-r--r--   0        0        0    12567 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/problem.py
--rw-r--r--   0        0        0      758 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/resources/__init__.py
--rw-r--r--   0        0        0    11038 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/validity_checker.py
--rw-r--r--   0        0        0      877 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/__init__.py
--rw-r--r--   0        0        0    12467 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable.py
--rw-r--r--   0        0        0    21838 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable_list.py
--rw-r--r--   0        0        0     2128 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/openmdao/whatsopt.py
--rw-r--r--   0        0        0      757 2023-04-27 14:57:11.175291 fast_oad_core-1.5.0/src/fastoad/source_data_files/__init__.py
--rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 fast_oad_core-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    32472 2023-05-11 14:35:08.366809 fast_oad_core-1.5.1/LICENSE.txt
+-rw-r--r--   0        0        0     3488 2023-05-11 14:35:08.366809 fast_oad_core-1.5.1/README.md
+-rw-r--r--   0        0        0     4231 2023-05-11 14:35:31.062960 fast_oad_core-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     1186 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/__init__.py
+-rw-r--r--   0        0        0      829 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/__init__.py
+-rw-r--r--   0        0        0     1059 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/files.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/__init__.py
+-rw-r--r--   0        0        0     2922 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/contents.py
+-rw-r--r--   0        0        0     3581 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/copy.py
+-rw-r--r--   0        0        0     3030 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/strings.py
+-rw-r--r--   0        0        0     1858 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/_utils/testing.py
+-rw-r--r--   0        0        0     3375 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/api.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/__init__.py
+-rw-r--r--   0        0        0    30528 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/api.py
+-rw-r--r--   0        0        0    10473 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/cli.py
+-rw-r--r--   0        0        0     2994 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/cli_utils.py
+-rw-r--r--   0        0        0     1477 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/exceptions.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/resources/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-11 14:35:08.382809 fast_oad_core-1.5.1/src/fastoad/cmd/resources/fastoad.yml
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/configurations/__init__.py
+-rw-r--r--   0        0        0     2974 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/constants.py
+-rw-r--r--   0        0        0     1675 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/exceptions.py
+-rw-r--r--   0        0        0     1087 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/__init__.py
+-rw-r--r--   0        0        0    23361 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/analysis_and_plots.py
+-rw-r--r--   0        0        0      905 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/exceptions.py
+-rw-r--r--   0        0        0     4073 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/mission_viewer.py
+-rw-r--r--   0        0        0    21069 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/optimization_viewer.py
+-rw-r--r--   0        0        0    16093 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/gui/variable_viewer.py
+-rw-r--r--   0        0        0      898 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/__init__.py
+-rw-r--r--   0        0        0      882 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/configuration/__init__.py
+-rw-r--r--   0        0        0    19153 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/configuration/configuration.py
+-rw-r--r--   0        0        0     3154 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/configuration/exceptions.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/configuration/resources/__init__.py
+-rw-r--r--   0        0        0     4038 2023-05-11 14:35:08.386809 fast_oad_core-1.5.1/src/fastoad/io/configuration/resources/configuration.json
+-rw-r--r--   0        0        0     1558 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/formatter.py
+-rw-r--r--   0        0        0     9033 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/variable_io.py
+-rw-r--r--   0        0        0      976 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/constants.py
+-rw-r--r--   0        0        0     1907 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/exceptions.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/resources/__init__.py
+-rw-r--r--   0        0        0    37628 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/resources/legacy1.txt
+-rw-r--r--   0        0        0     1476 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/resources/remove_duplicate_variables.py
+-rw-r--r--   0        0        0     4869 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/translator.py
+-rw-r--r--   0        0        0     8181 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_base.py
+-rw-r--r--   0        0        0     1431 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_legacy.py
+-rw-r--r--   0        0        0     3966 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_standard.py
+-rw-r--r--   0        0        0      888 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/model_base/__init__.py
+-rw-r--r--   0        0        0    10543 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/model_base/atmosphere.py
+-rw-r--r--   0        0        0     1900 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/model_base/datacls.py
+-rw-r--r--   0        0        0     9806 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/model_base/flight_point.py
+-rw-r--r--   0        0        0     8996 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/model_base/propulsion.py
+-rw-r--r--   0        0        0      949 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/__init__.py
+-rw-r--r--   0        0        0      797 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/__init__.py
+-rw-r--r--   0        0        0      807 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/__init__.py
+-rw-r--r--   0        0        0     9057 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/base.py
+-rw-r--r--   0        0        0     1705 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/exceptions.py
+-rw-r--r--   0        0        0     5971 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/__init__.py
+-rw-r--r--   0        0        0      988 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/exceptions.py
+-rw-r--r--   0        0        0      896 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py
+-rw-r--r--   0        0        0     1022 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py
+-rw-r--r--   0        0        0     8930 2023-05-11 14:35:08.390809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py
+-rw-r--r--   0        0        0    23483 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py
+-rw-r--r--   0        0        0    15608 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py
+-rw-r--r--   0        0        0     9592 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json
+-rw-r--r--   0        0        0     5090 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/schema.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/__init__.py
+-rw-r--r--   0        0        0     9130 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/base.py
+-rw-r--r--   0        0        0     1616 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/link_mtow.py
+-rw-r--r--   0        0        0    10558 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission.py
+-rw-r--r--   0        0        0     9878 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission_run.py
+-rw-r--r--   0        0        0    10152 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py
+-rw-r--r--   0        0        0    21188 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/payload_range.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/__init__.py
+-rw-r--r--   0        0        0     2229 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml
+-rw-r--r--   0        0        0     5896 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml
+-rw-r--r--   0        0        0     3624 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/polar.py
+-rw-r--r--   0        0        0     4019 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/polar_modifier.py
+-rw-r--r--   0        0        0     6561 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/routes.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/__init__.py
+-rw-r--r--   0        0        0    11836 2023-05-11 14:35:08.394809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/base.py
+-rw-r--r--   0        0        0     4912 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/macro_segments.py
+-rw-r--r--   0        0        0     1241 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/__init__.py
+-rw-r--r--   0        0        0     7782 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/altitude_change.py
+-rw-r--r--   0        0        0    10181 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/cruise.py
+-rw-r--r--   0        0        0     2163 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/ground_speed_change.py
+-rw-r--r--   0        0        0     1486 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/hold.py
+-rw-r--r--   0        0        0     1648 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/mass_input.py
+-rw-r--r--   0        0        0     2390 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/speed_change.py
+-rw-r--r--   0        0        0     1887 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/start.py
+-rw-r--r--   0        0        0     1135 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/__init__.py
+-rw-r--r--   0        0        0     6038 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/end_of_takeoff.py
+-rw-r--r--   0        0        0     3142 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/rotation.py
+-rw-r--r--   0        0        0     2659 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/takeoff.py
+-rw-r--r--   0        0        0     2063 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/taxi.py
+-rw-r--r--   0        0        0     2873 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/transition.py
+-rw-r--r--   0        0        0    17916 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/time_step_base.py
+-rw-r--r--   0        0        0     2245 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/performances/mission/util.py
+-rw-r--r--   0        0        0     1695 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/models/variable_descriptions.txt
+-rw-r--r--   0        0        0      805 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/__init__.py
+-rw-r--r--   0        0        0    14623 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/_bundle_loader.py
+-rw-r--r--   0        0        0    18578 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/_plugins.py
+-rw-r--r--   0        0        0     1442 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/constants.py
+-rw-r--r--   0        0        0     7475 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/exceptions.py
+-rw-r--r--   0        0        0    19567 2023-05-11 14:35:08.398809 fast_oad_core-1.5.1/src/fastoad/module_management/service_registry.py
+-rw-r--r--   0        0        0       64 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/.gitignore
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/__init__.py
+-rw-r--r--   0        0        0    14508 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml
+-rw-r--r--   0        0        0      935 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml
+-rw-r--r--   0        0        0     1260 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml
+-rw-r--r--   0        0        0     1227 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/__init__.py
+-rw-r--r--   0        0        0    18684 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png
+-rw-r--r--   0        0        0     5532 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/problem_description.png
+-rw-r--r--   0        0        0   134937 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/__init__.py
+-rw-r--r--   0        0        0     1988 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/displacements.py
+-rw-r--r--   0        0        0     1561 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py
+-rw-r--r--   0        0        0     2150 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/stresses.py
+-rw-r--r--   0        0        0      540 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt
+-rw-r--r--   0        0        0     1670 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/weight.py
+-rw-r--r--   0        0        0       37 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/.gitignore
+-rw-r--r--   0        0        0    11579 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb
+-rw-r--r--   0        0        0    34406 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb
+-rw-r--r--   0        0        0    13485 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb
+-rw-r--r--   0        0        0    55116 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb
+-rw-r--r--   0        0        0    20123 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/__init__.py
+-rw-r--r--   0        0        0      461 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/data/source_file.xml
+-rw-r--r--   0        0        0     7146 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png
+-rw-r--r--   0        0        0     6097 2023-05-11 14:35:08.402809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png
+-rw-r--r--   0        0        0   113972 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png
+-rw-r--r--   0        0        0   125428 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/__init__.py
+-rw-r--r--   0        0        0    29150 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png
+-rw-r--r--   0        0        0    40682 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png
+-rw-r--r--   0        0        0    46219 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png
+-rw-r--r--   0        0        0    18684 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png
+-rw-r--r--   0        0        0    23022 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png
+-rw-r--r--   0        0        0    11722 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png
+-rw-r--r--   0        0        0    65293 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png
+-rw-r--r--   0        0        0    32808 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/__init__.py
+-rw-r--r--   0        0        0      346 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/__init__.py
+-rw-r--r--   0        0        0      485 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mass/mass.py
+-rw-r--r--   0        0        0      982 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/__init__.py
+-rw-r--r--   0        0        0     1019 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.406809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/__init__.py
+-rw-r--r--   0        0        0      860 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py
+-rw-r--r--   0        0        0     2288 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
+-rw-r--r--   0        0        0     1036 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/__init__.py
+-rw-r--r--   0        0        0      241 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/__init__.py
+-rw-r--r--   0        0        0      806 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/__init__.py
+-rw-r--r--   0        0        0      695 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py
+-rw-r--r--   0        0        0      389 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe_exercise.py
+-rw-r--r--   0        0        0     1539 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py
+-rw-r--r--   0        0        0     1586 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0     1580 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/__init__.py
+-rw-r--r--   0        0        0      920 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/__init__.py
+-rw-r--r--   0        0        0     1101 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/__init__.py
+-rw-r--r--   0        0        0      458 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_induced_drag_coefficient.py
+-rw-r--r--   0        0        0     1255 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py
+-rw-r--r--   0        0        0      579 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/__init__.py
+-rw-r--r--   0        0        0      416 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/geometry.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/__init__.py
+-rw-r--r--   0        0        0      358 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/geometry/sub_components/compute_wing_area.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/__init__.py
+-rw-r--r--   0        0        0      688 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/__init__.py
+-rw-r--r--   0        0        0      531 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py
+-rw-r--r--   0        0        0      850 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py
+-rw-r--r--   0        0        0     1942 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py
+-rw-r--r--   0        0        0     1918 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/__init__.py
+-rw-r--r--   0        0        0     1052 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/__init__.py
+-rw-r--r--   0        0        0      578 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py
+-rw-r--r--   0        0        0        0 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/__init__.py
+-rw-r--r--   0        0        0     1913 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py
+-rw-r--r--   0        0        0     2102 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py
+-rw-r--r--   0        0        0     1057 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py
+-rw-r--r--   0        0        0     1029 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py
+-rw-r--r--   0        0        0      825 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py
+-rw-r--r--   0        0        0     1308 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/README.md
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/notebooks/__init__.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/openmdao/__init__.py
+-rw-r--r--   0        0        0     4032 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/openmdao/_utils.py
+-rw-r--r--   0        0        0     1378 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/openmdao/exceptions.py
+-rw-r--r--   0        0        0    12567 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/openmdao/problem.py
+-rw-r--r--   0        0        0      758 2023-05-11 14:35:08.410809 fast_oad_core-1.5.1/src/fastoad/openmdao/resources/__init__.py
+-rw-r--r--   0        0        0    11038 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/openmdao/validity_checker.py
+-rw-r--r--   0        0        0      877 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/openmdao/variables/__init__.py
+-rw-r--r--   0        0        0    12467 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/openmdao/variables/variable.py
+-rw-r--r--   0        0        0    21838 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/openmdao/variables/variable_list.py
+-rw-r--r--   0        0        0     2128 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/openmdao/whatsopt.py
+-rw-r--r--   0        0        0      757 2023-05-11 14:35:08.414809 fast_oad_core-1.5.1/src/fastoad/source_data_files/__init__.py
+-rw-r--r--   0        0        0     5910 1970-01-01 00:00:00.000000 fast_oad_core-1.5.1/PKG-INFO
```

### Comparing `fast_oad_core-1.5.0/LICENSE.txt` & `fast_oad_core-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/README.md` & `fast_oad_core-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/pyproject.toml` & `fast_oad_core-1.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "FAST-OAD-core"
-version = "1.5.0" # This version number is overwritten by GitHub packaging workflow but setting this version here will allow installation of CS25 models in development mode
+version = "1.5.1" # This version number is overwritten by GitHub packaging workflow but setting this version here will allow installation of CS25 models in development mode
 description = "FAST-OAD is a framework for performing rapid Overall Aircraft Design"
 readme = "README.md"
 authors = [
     "Christophe DAVID <christophe.david@onera.fr>",
     "Scott DELBECQ <Scott.DELBECQ@isae-supaero.fr>"
 ]
 packages = [
```

### Comparing `fast_oad_core-1.5.0/src/fastoad/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/files.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/files.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/contents.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/contents.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/resource_management/copy.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/resource_management/copy.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/strings.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/strings.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/_utils/testing.py` & `fast_oad_core-1.5.1/src/fastoad/_utils/testing.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/api.py` & `fast_oad_core-1.5.1/src/fastoad/api.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/api.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/api.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/cli.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/cli_utils.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/cli_utils.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/cmd/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/cmd/resources/fastoad.yml` & `fast_oad_core-1.5.1/src/fastoad/cmd/resources/fastoad.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/configurations/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/constants.py` & `fast_oad_core-1.5.1/src/fastoad/constants.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/analysis_and_plots.py` & `fast_oad_core-1.5.1/src/fastoad/gui/analysis_and_plots.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/gui/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/mission_viewer.py` & `fast_oad_core-1.5.1/src/fastoad/gui/mission_viewer.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/optimization_viewer.py` & `fast_oad_core-1.5.1/src/fastoad/gui/optimization_viewer.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/gui/variable_viewer.py` & `fast_oad_core-1.5.1/src/fastoad/gui/variable_viewer.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/configuration/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/io/configuration/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/configuration/configuration.py` & `fast_oad_core-1.5.1/src/fastoad/io/configuration/configuration.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/configuration/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/io/configuration/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/io/configuration/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/configuration/resources/configuration.json` & `fast_oad_core-1.5.1/src/fastoad/io/configuration/resources/configuration.json`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/formatter.py` & `fast_oad_core-1.5.1/src/fastoad/io/formatter.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/variable_io.py` & `fast_oad_core-1.5.1/src/fastoad/io/variable_io.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/constants.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/constants.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/legacy1.txt` & `fast_oad_core-1.5.1/src/fastoad/io/xml/resources/legacy1.txt`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/resources/remove_duplicate_variables.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/resources/remove_duplicate_variables.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/translator.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/translator.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_base.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_base.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_legacy.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_legacy.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/io/xml/variable_io_standard.py` & `fast_oad_core-1.5.1/src/fastoad/io/xml/variable_io_standard.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/model_base/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/model_base/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/model_base/atmosphere.py` & `fast_oad_core-1.5.1/src/fastoad/model_base/atmosphere.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/model_base/datacls.py` & `fast_oad_core-1.5.1/src/fastoad/model_base/datacls.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/model_base/flight_point.py` & `fast_oad_core-1.5.1/src/fastoad/model_base/flight_point.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/model_base/propulsion.py` & `fast_oad_core-1.5.1/src/fastoad/model_base/propulsion.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/base.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/base.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                     return route
 
         return None
 
     def compute_from(self, start: FlightPoint) -> pd.DataFrame:
         if self.target_fuel_consumption is None:
             flight_points = super().compute_from(start)
-            flight_points.name.loc[flight_points.name.isnull()] = ""
+            flight_points.loc[flight_points.name.isnull()].name = ""
             self._compute_reserve(flight_points)
             return flight_points
 
         return self._solve_cruise_distance(start)
 
     def get_reserve_fuel(self):
         """:returns: the fuel quantity for reserve, obtained after mission computation."""
@@ -105,25 +105,20 @@
         if self.reserve_ratio > 0.0:
             if self.reserve_base_route_name is None:
                 base_route_name = self.first_route.name
             else:
                 base_route_name = self.reserve_base_route_name
 
             reserve_fuel = self.reserve_ratio * self._get_consumed_mass_in_route(base_route_name)
-            reserve_points = pd.DataFrame(
-                [
-                    deepcopy(flight_points.iloc[-1]),
-                    deepcopy(flight_points.iloc[-1]),
-                ]
-            )
+            last_flight_point = flight_points.iloc[-1]
+
+            after_reserve_point = deepcopy(last_flight_point)
+            after_reserve_point.mass = last_flight_point.mass - reserve_fuel
 
-            # We are not using -= here because it would operate last_flight_point.mass can be
-            # an array. The operator would operate element-wise and would modify the original
-            # flight point, despite the deepcopy.
-            reserve_points.mass.iloc[-1] = reserve_points.mass.iloc[0] - reserve_fuel
+            reserve_points = pd.DataFrame([last_flight_point, after_reserve_point])
             reserve_points["name"] = f"{self.name}:reserve"
 
             self.part_flight_points.append(reserve_points)
 
     def _solve_cruise_distance(self, start: FlightPoint) -> pd.DataFrame:
         """
         Adjusts cruise distance through a solver to have whole route that
@@ -154,11 +149,11 @@
 
         :param cruise_distance:
         :param start:
         :return: difference between computed fuel and self.target_fuel_consumption
         """
         self.first_route.cruise_distance = cruise_distance
         flight_points = super().compute_from(start)
-        flight_points.name.loc[flight_points.name.isnull()] = ""
+        flight_points.loc[flight_points.name.isnull()].name = ""
         self._compute_reserve(flight_points)
         self._flight_points = flight_points
         return self.target_fuel_consumption - self.consumed_fuel
```

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/constants.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/input_definition.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/mission_builder.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/mission_builder/structure_builders.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/resources/mission_schema.json`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/mission_definition/schema.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/mission_definition/schema.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/base.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/base.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/link_mtow.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/link_mtow.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,21 @@
             types=bool,
             desc="If True, input weight will be deduced from block fuel.\n"
             "If False, block fuel will be deduced from input weight.\n"
             "Not used (actually forced to True) if adjust_fuel is True.",
         )
         self.options.declare(
             "compute_TOW",
-            default=None,
+            default=False,
             types=bool,
-            deprecation='Option "compute_TOW" is deprecated for mission module. '
-            'Please use "compute_input_weight" instead.',
+            deprecation=(
+                'Option "compute_TOW" is deprecated for mission module. '
+                'Please use "compute_input_weight" instead.',
+                "compute_input_weight",
+            ),
             desc="If True, TakeOff Weight will be computed from onboard fuel at takeoff and ZFW.\n"
             "If False, block fuel will be computed from ramp weight and ZFW.\n"
             "Not used (actually forced to True) if adjust_fuel is True.",
         )
         self.options.declare(
             "add_solver",
             default=False,
@@ -98,17 +101,14 @@
             desc="If True, TOW will be considered equal to MTOW and mission payload will be "
             "considered equal to design payload.",
         )
 
     def setup(self):
         super().setup()
 
-        if self.options["compute_TOW"] is not None:
-            self.options["compute_input_weight"] = self.options["compute_TOW"]
-
         mission_options = {
             key: val for key, val in self.options.items() if key in AdvancedMissionComp().options
         }
         mission_component = AdvancedMissionComp(**mission_options)
 
         self.add_subsystem("ZFW_computation", self._get_zfw_component(), promotes=["*"])
```

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_run.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission_run.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/mission_wrapper.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/payload_range.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/payload_range.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/sizing_breguet.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/openmdao/resources/sizing_mission.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/polar.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/polar_modifier.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/polar_modifier.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/routes.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/routes.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/base.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/base.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/macro_segments.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/macro_segments.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/altitude_change.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/altitude_change.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/cruise.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/cruise.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/ground_speed_change.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/ground_speed_change.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/hold.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/hold.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/mass_input.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/mass_input.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/speed_change.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/speed_change.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/start.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/start.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/end_of_takeoff.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/end_of_takeoff.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/rotation.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/rotation.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/takeoff/takeoff.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/takeoff/takeoff.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/taxi.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/taxi.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/registered/transition.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/registered/transition.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/segments/time_step_base.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/segments/time_step_base.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/performances/mission/util.py` & `fast_oad_core-1.5.1/src/fastoad/models/performances/mission/util.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/models/variable_descriptions.txt` & `fast_oad_core-1.5.1/src/fastoad/models/variable_descriptions.txt`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/_bundle_loader.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/_bundle_loader.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/_plugins.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/_plugins.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/constants.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/constants.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/module_management/service_registry.py` & `fast_oad_core-1.5.1/src/fastoad/module_management/service_registry.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/beam_problem.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/beam_problem.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/beam_problem_stress.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/problem_inputs.xml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/data/problem_inputs_stress.xml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/problem_description.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/problem_description.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/img/stress_config.gif`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/displacements.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/displacements.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/section_properties.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/stresses.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/stresses.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/variable_descriptions.txt`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/01_Quick_start/modules/weight.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/01_Quick_start/modules/weight.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/01_summary.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/02_pure_Python.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/03_scipy.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/04_OpenMDAO.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/05_FAST-OAD.ipynb`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Component.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/Lift_to_drag.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/N2_diagram_correct.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/aerodynamics.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/global_process.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/handy_analogy.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-ISAE_SUPAERO.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/logo-onera.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mass.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/mdo.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/img/module_architecture.png`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/FAST-OAD/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_induced_drag_coefficient.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_lift_to_drag_ratio.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/aerodynamics/sub_components/compute_profile_drag.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/geometry/sub_components/compute_wing_area.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_owe.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mass/sub_components/compute_wing_mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/performance/sub_components/compute_fuel_mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/OpenMDAO/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/aerodynamics.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_lift_to_drag_ratio.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/aerodynamics/sub_components/compute_profile_drag.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_owe.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mass/sub_components/compute_wing_mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_and_fuel_loop.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/mtow_loop.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/performance.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/performance/sub_components/compute_fuel_mass.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/pure_python/update_mtow/update_mtow.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/compute_fuel_scipy.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/python_for_scipy/mtow_loop_scipy.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/modules/widget.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_discipline/mda_discipline.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDA_global_group/mda_global_group.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/MDO_MTOW/mdo_mtow.yml`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/02_From_Python_to_FAST-OAD/working_folder/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/README.md` & `fast_oad_core-1.5.1/src/fastoad/notebooks/README.md`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/notebooks/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/_utils.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/_utils.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/exceptions.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/problem.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/problem.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/resources/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/validity_checker.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/validity_checker.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/variables/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/variables/variable.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/variables/variable_list.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/variables/variable_list.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/openmdao/whatsopt.py` & `fast_oad_core-1.5.1/src/fastoad/openmdao/whatsopt.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/src/fastoad/source_data_files/__init__.py` & `fast_oad_core-1.5.1/src/fastoad/source_data_files/__init__.py`

 * *Files identical despite different names*

### Comparing `fast_oad_core-1.5.0/PKG-INFO` & `fast_oad_core-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-oad-core
-Version: 1.5.0
+Version: 1.5.1
 Summary: FAST-OAD is a framework for performing rapid Overall Aircraft Design
 Home-page: https://github.com/fast-aircraft-design/FAST-OAD
 License: GPL-3.0-only
 Keywords: aircraft,design,multi-disciplinary
 Author: Christophe DAVID
 Author-email: christophe.david@onera.fr
 Requires-Python: >=3.7,<4.0
```

