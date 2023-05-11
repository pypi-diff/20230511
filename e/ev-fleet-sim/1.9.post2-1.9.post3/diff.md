# Comparing `tmp/ev-fleet-sim-1.9.post2.tar.gz` & `tmp/ev-fleet-sim-1.9.post3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ev-fleet-sim-1.9.post2.tar", last modified: Thu Jan 26 10:40:06 2023, max compression
+gzip compressed data, was "ev-fleet-sim-1.9.post3.tar", last modified: Thu Jan 26 10:42:40 2023, max compression
```

## Comparing `ev-fleet-sim-1.9.post2.tar` & `ev-fleet-sim-1.9.post3.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    35120 2021-07-26 04:52:59.000000 ev-fleet-sim-1.9.post2/LICENSE
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     6118 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/PKG-INFO
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     5455 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/README.md
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      104 2021-11-02 17:25:33.000000 ev-fleet-sim-1.9.post2/pyproject.toml
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     1330 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/setup.cfg
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.772083 ev-fleet-sim-1.9.post2/src/
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    21641 2023-01-26 10:38:41.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)      203 2023-01-26 10:38:25.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/__main__.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/
--rw-r--r--   0 abrac     (1000) abrac     (1000)      110 2021-11-04 10:17:47.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/__init__.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     5153 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/animation.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      635 2021-11-04 11:39:42.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/map_calcs.py
--rw-r--r--   0 abrac     (1000) abrac     (1000)     4941 2021-11-21 15:12:35.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/mapping.py
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)      428 2021-02-21 18:28:12.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/mpl_figopen.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/
--rw-r--r--   0 abrac     (1000) abrac     (1000)     3586 2021-02-14 16:28:59.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/[deprecated]_charge_monitor_traffic.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-09-22 05:27:32.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/__init__.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    14212 2023-01-26 10:24:55.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/hull_ev_simulation.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)    11906 2023-01-21 12:14:48.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/results_splitter.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     7179 2023-01-21 07:34:39.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/sumo_ev_simulation.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__dirty/
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__dirty/__init__.py
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)     7553 2021-06-25 20:09:30.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__dirty/dirty_charging_potential.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      312 2021-10-11 10:56:35.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__dirty/instructions.md
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1605 2021-11-09 17:03:35.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/energy_usage_boxplots_aggregator.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)      428 2021-11-02 10:09:14.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/mpl_figopen
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     4265 2021-11-23 12:35:40.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/power_energy_plot_extractor.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)     1617 2020-12-06 22:16:24.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_data_analysis_new.py
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)      507 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_mk_output_dir.sh
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)      809 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_ren_output_dir.sh
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)      557 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_trash_output_dir.sh
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-09-22 08:46:52.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/__init__.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     5219 2023-01-25 16:51:22.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/analysis_functions.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     6671 2023-01-25 17:02:04.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/ev_box_plots.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)    63003 2023-01-26 09:25:39.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/ev_results_analysis.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)    25431 2023-01-19 11:48:32.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/pv_results_analysis.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    25096 2023-01-19 11:48:43.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/wind_results_analysis.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/
--rw-r--r--   0 abrac     (1000) abrac     (1000)     2785 2020-09-30 17:41:22.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/[deprecated]_charge_monitor.py
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)     1198 2020-12-04 20:55:33.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/[deprecated]_duarouter.sh
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-03-17 20:46:47.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3065 2023-01-21 07:35:22.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/fcd_conversion.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    29876 2023-01-21 15:04:56.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/routing.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     6926 2023-01-20 05:39:04.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/1Hz_GPS_Tracking_Data.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1252 2021-11-04 11:58:43.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Convert.r
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3846 2021-10-19 12:26:42.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Split.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     4436 2021-07-09 19:19:48.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Kampala_UTX.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3632 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Stellenbosch.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     5160 2021-07-09 19:57:18.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/data_quality_analysis.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.776083 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3542 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/netconvert.sh
--rw-r--r--   0 abrac     (1000) abrac     (1000)     5053 2021-10-11 11:11:33.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/osmNetconvert_Africa.typ.xml
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)      115 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/pbf_to_osm.bat
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)      188 2022-09-23 18:04:33.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/pbf_to_osm.sh
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/__init__.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      100 2021-10-11 07:13:07.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/boundary.csv
--rw-r--r--   0 abrac     (1000) abrac     (1000)     2791 2021-02-14 16:28:59.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/custom_osm_test.template.sumocfg
--rw-r--r--   0 abrac     (1000) abrac     (1000)     1154 2021-04-12 14:39:11.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.Tesla_S70D.vtype.xml
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     1014 2022-08-18 09:35:35.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.eMBT.vtype.xml
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     1039 2022-10-25 10:12:55.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.vtype.xml
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-10-05 17:59:01.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/__init__.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      249 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/initialisation-instructions.md
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     4641 2023-01-22 15:13:53.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/scenario_initialisation.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/
--rw-r--r--   0 abrac     (1000) abrac     (1000)       96 2021-09-17 07:16:31.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/__init__.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1809 2021-10-20 09:20:12.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/save_dates_remaining.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    13457 2023-01-18 06:36:49.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/spatial_clustering.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     7600 2023-01-20 14:29:29.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/spatial_filtering.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/
--rw-r--r--   0 abrac     (1000) abrac     (1000)       93 2021-09-17 08:32:55.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/__init__.py
--rwxr-xr-x   0 abrac     (1000) abrac     (1000)      340 2021-03-15 13:34:19.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/export_to_png.sh
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3851 2023-01-18 08:27:22.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/stop_duration_box_plots.py
--rwxrwxr-x   0 abrac     (1000) abrac     (1000)    28413 2023-01-18 13:33:59.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/stop_extraction.py
--rw-rw-r--   0 abrac     (1000) abrac     (1000)    27615 2023-01-19 18:15:03.000000 ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/temporal_clustering.py
-drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:40:06.780083 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     6118 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/PKG-INFO
--rw-rw-r--   0 abrac     (1000) abrac     (1000)     4686 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/SOURCES.txt
--rw-rw-r--   0 abrac     (1000) abrac     (1000)        1 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/dependency_links.txt
--rw-rw-r--   0 abrac     (1000) abrac     (1000)       57 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/entry_points.txt
--rw-rw-r--   0 abrac     (1000) abrac     (1000)      322 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/requires.txt
--rw-rw-r--   0 abrac     (1000) abrac     (1000)       19 2023-01-26 10:40:06.000000 ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/top_level.txt
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    35120 2021-07-26 04:52:59.000000 ev-fleet-sim-1.9.post3/LICENSE
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     6118 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/PKG-INFO
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     5455 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/README.md
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      104 2021-11-02 17:25:33.000000 ev-fleet-sim-1.9.post3/pyproject.toml
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     1330 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/setup.cfg
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.425425 ev-fleet-sim-1.9.post3/src/
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.425425 ev-fleet-sim-1.9.post3/src/data_processing_ev/
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    21665 2023-01-26 10:41:50.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)      203 2023-01-26 10:38:25.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/__main__.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/
+-rw-r--r--   0 abrac     (1000) abrac     (1000)      110 2021-11-04 10:17:47.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/__init__.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     5153 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/animation.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      635 2021-11-04 11:39:42.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/map_calcs.py
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     4941 2021-11-21 15:12:35.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/mapping.py
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)      428 2021-02-21 18:28:12.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/mpl_figopen.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     3586 2021-02-14 16:28:59.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/[deprecated]_charge_monitor_traffic.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-09-22 05:27:32.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/__init__.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    14212 2023-01-26 10:24:55.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/hull_ev_simulation.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)    11906 2023-01-21 12:14:48.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/results_splitter.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     7179 2023-01-21 07:34:39.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/sumo_ev_simulation.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__dirty/
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__dirty/__init__.py
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)     7553 2021-06-25 20:09:30.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__dirty/dirty_charging_potential.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      312 2021-10-11 10:56:35.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__dirty/instructions.md
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1605 2021-11-09 17:03:35.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/energy_usage_boxplots_aggregator.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)      428 2021-11-02 10:09:14.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/mpl_figopen
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     4265 2021-11-23 12:35:40.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/power_energy_plot_extractor.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)     1617 2020-12-06 22:16:24.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_data_analysis_new.py
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)      507 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_mk_output_dir.sh
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)      809 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_ren_output_dir.sh
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)      557 2020-09-30 17:41:25.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_trash_output_dir.sh
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-09-22 08:46:52.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/__init__.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     5219 2023-01-25 16:51:22.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/analysis_functions.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     6671 2023-01-25 17:02:04.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/ev_box_plots.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)    63003 2023-01-26 09:25:39.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/ev_results_analysis.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)    25431 2023-01-19 11:48:32.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/pv_results_analysis.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    25096 2023-01-19 11:48:43.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/wind_results_analysis.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     2785 2020-09-30 17:41:22.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/[deprecated]_charge_monitor.py
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)     1198 2020-12-04 20:55:33.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/[deprecated]_duarouter.sh
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-03-17 20:46:47.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3065 2023-01-21 07:35:22.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/fcd_conversion.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    29876 2023-01-21 15:04:56.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/routing.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.429425 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     6926 2023-01-20 05:39:04.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/1Hz_GPS_Tracking_Data.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1252 2021-11-04 11:58:43.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Convert.r
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3846 2021-10-19 12:26:42.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Split.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     4436 2021-07-09 19:19:48.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Kampala_UTX.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3632 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Stellenbosch.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     5160 2021-07-09 19:57:18.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/data_quality_analysis.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3542 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/netconvert.sh
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     5053 2021-10-11 11:11:33.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/osmNetconvert_Africa.typ.xml
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)      115 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/pbf_to_osm.bat
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)      188 2022-09-23 18:04:33.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/pbf_to_osm.sh
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/__init__.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      100 2021-10-11 07:13:07.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/boundary.csv
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     2791 2021-02-14 16:28:59.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/custom_osm_test.template.sumocfg
+-rw-r--r--   0 abrac     (1000) abrac     (1000)     1154 2021-04-12 14:39:11.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.Tesla_S70D.vtype.xml
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     1014 2022-08-18 09:35:35.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.eMBT.vtype.xml
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     1039 2022-10-25 10:12:55.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.vtype.xml
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        0 2021-10-05 17:59:01.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/__init__.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      249 2022-08-18 09:08:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/initialisation-instructions.md
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     4641 2023-01-22 15:13:53.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/scenario_initialisation.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/
+-rw-r--r--   0 abrac     (1000) abrac     (1000)       96 2021-09-17 07:16:31.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/__init__.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     1809 2021-10-20 09:20:12.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/save_dates_remaining.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    13457 2023-01-18 06:36:49.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/spatial_clustering.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     7600 2023-01-20 14:29:29.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/spatial_filtering.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/
+-rw-r--r--   0 abrac     (1000) abrac     (1000)       93 2021-09-17 08:32:55.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/__init__.py
+-rwxr-xr-x   0 abrac     (1000) abrac     (1000)      340 2021-03-15 13:34:19.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/export_to_png.sh
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)     3851 2023-01-18 08:27:22.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/stop_duration_box_plots.py
+-rwxrwxr-x   0 abrac     (1000) abrac     (1000)    28413 2023-01-18 13:33:59.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/stop_extraction.py
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)    27615 2023-01-19 18:15:03.000000 ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/temporal_clustering.py
+drwxrwxr-x   0 abrac     (1000) abrac     (1000)        0 2023-01-26 10:42:40.433425 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     6118 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/PKG-INFO
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)     4686 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/SOURCES.txt
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)        1 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/dependency_links.txt
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)       57 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/entry_points.txt
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)      322 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/requires.txt
+-rw-rw-r--   0 abrac     (1000) abrac     (1000)       19 2023-01-26 10:42:40.000000 ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/top_level.txt
```

### Comparing `ev-fleet-sim-1.9.post2/LICENSE` & `ev-fleet-sim-1.9.post3/LICENSE`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/PKG-INFO` & `ev-fleet-sim-1.9.post3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ev-fleet-sim
-Version: 1.9.post2
+Version: 1.9.post3
 Summary: This software computes the electrical energy requirements of a fleet of vehicles. It also determines how much of this energy can be offset by renewable energy.
 Home-page: https://gitlab.com/eputs/ev-fleet-sim
 Author: Chris Abraham
 Author-email: chrisbrhm@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/eputs/ev-fleet-sim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ev-fleet-sim-1.9.post2/README.md` & `ev-fleet-sim-1.9.post3/README.md`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/setup.cfg` & `ev-fleet-sim-1.9.post3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ev-fleet-sim
-version = 1.9.post2
+version = 1.9.post3
 author = Chris Abraham
 author_email = chrisbrhm@gmail.com
 description = This software computes the electrical energy requirements of a fleet of vehicles. It also determines how much of this energy can be offset by renewable energy.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitlab.com/eputs/ev-fleet-sim
 project_urls =
```

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/__init__.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # TODO Maybe convert the dir structure to format in
 # https://stackoverflow.com/a/62570479/10462623 OR Create the dir structure in
 # the file system, and store it using Path.glob('**')
+# PYTHON_ARGCOMPLETE_OK
 
 DATA_FMTS = {'GPS': 0, 'GTFS': 1}
 
 EV_MODELS = {'SUMO': 0, 'Hull': 1}
 
 from .scenario_initialisation.scenario_initialisation \
     import initialise_scenario
```

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/animation.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/animation.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/map_calcs.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/map_calcs.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/data_visualisation/mapping.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/data_visualisation/mapping.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/[deprecated]_charge_monitor_traffic.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/[deprecated]_charge_monitor_traffic.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/hull_ev_simulation.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/hull_ev_simulation.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/results_splitter.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/results_splitter.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/ev_simulation/sumo_ev_simulation.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/ev_simulation/sumo_ev_simulation.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/__dirty/dirty_charging_potential.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/__dirty/dirty_charging_potential.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/energy_usage_boxplots_aggregator.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/energy_usage_boxplots_aggregator.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/helper_scripts/power_energy_plot_extractor.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/helper_scripts/power_energy_plot_extractor.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_data_analysis_new.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_data_analysis_new.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_ren_output_dir.sh` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_ren_output_dir.sh`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/[deprecated]_trash_output_dir.sh` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/[deprecated]_trash_output_dir.sh`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/analysis_functions.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/ev_box_plots.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/ev_box_plots.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/ev_results_analysis.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/ev_results_analysis.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/pv_results_analysis.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/pv_results_analysis.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/results_analysis/wind_results_analysis.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/results_analysis/wind_results_analysis.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/[deprecated]_charge_monitor.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/[deprecated]_charge_monitor.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/[deprecated]_duarouter.sh` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/[deprecated]_duarouter.sh`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/fcd_conversion.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/fcd_conversion.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/routing/routing.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/routing/routing.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/1Hz_GPS_Tracking_Data.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/1Hz_GPS_Tracking_Data.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Convert.r` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Convert.r`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Split.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/GTFS_Split.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Kampala_UTX.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Kampala_UTX.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Stellenbosch.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/Stellenbosch.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/data_quality_analysis.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Data_Pre-Processing/data_quality_analysis.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/netconvert.sh` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/netconvert.sh`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/osmNetconvert_Africa.typ.xml` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/Map_Construction/osmNetconvert_Africa.typ.xml`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/custom_osm_test.template.sumocfg` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/custom_osm_test.template.sumocfg`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.Tesla_S70D.vtype.xml` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.Tesla_S70D.vtype.xml`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.eMBT.vtype.xml` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.eMBT.vtype.xml`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.vtype.xml` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/Initialisation_Files/ev_template.vtype.xml`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/scenario_initialisation/scenario_initialisation.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/scenario_initialisation/scenario_initialisation.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/save_dates_remaining.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/save_dates_remaining.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/spatial_clustering.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/spatial_clustering.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/spatial_clustering/spatial_filtering.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/spatial_clustering/spatial_filtering.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/stop_duration_box_plots.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/stop_duration_box_plots.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/stop_extraction.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/stop_extraction.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/data_processing_ev/temporal_clustering/temporal_clustering.py` & `ev-fleet-sim-1.9.post3/src/data_processing_ev/temporal_clustering/temporal_clustering.py`

 * *Files identical despite different names*

### Comparing `ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/PKG-INFO` & `ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ev-fleet-sim
-Version: 1.9.post2
+Version: 1.9.post3
 Summary: This software computes the electrical energy requirements of a fleet of vehicles. It also determines how much of this energy can be offset by renewable energy.
 Home-page: https://gitlab.com/eputs/ev-fleet-sim
 Author: Chris Abraham
 Author-email: chrisbrhm@gmail.com
 Project-URL: Bug Tracker, https://gitlab.com/eputs/ev-fleet-sim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `ev-fleet-sim-1.9.post2/src/ev_fleet_sim.egg-info/SOURCES.txt` & `ev-fleet-sim-1.9.post3/src/ev_fleet_sim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

