# Comparing `tmp/gridworks_atn-0.2.4.tar.gz` & `tmp/gridworks_atn-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridworks_atn-0.2.4.tar", max compression
+gzip compressed data, was "gridworks_atn-0.3.2.tar", max compression
```

## Comparing `gridworks_atn-0.2.4.tar` & `gridworks_atn-0.3.2.tar`

### file list

```diff
@@ -1,110 +1,89 @@
--rw-r--r--   0        0        0     1065 2023-04-29 18:36:00.003173 gridworks_atn-0.2.4/LICENSE
--rw-r--r--   0        0        0     3002 2023-04-29 18:36:00.003173 gridworks_atn-0.2.4/README.md
--rw-r--r--   0        0        0     2150 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      336 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/__init__.py
--rw-r--r--   0        0        0      226 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/__main__.py
--rw-r--r--   0        0        0     7480 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/api_types.py
--rw-r--r--   0        0        0    21829 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/atn_actor_base.py
--rw-r--r--   0        0        0     4840 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/atn_utils.py
--rw-r--r--   0        0        0     4871 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/config.py
--rw-r--r--   0        0        0     6148 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/.DS_Store
--rw-r--r--   0        0        0      202 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/__init__.py
--rw-r--r--   0        0        0    23507 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/base_g_node.py
--rw-r--r--   0        0        0      583 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_edge.py
--rw-r--r--   0        0        0     7812 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_graph.py
--rw-r--r--   0        0        0     1559 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/d_node.py
--rw-r--r--   0        0        0     5366 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/g_node.py
--rw-r--r--   0        0        0     6791 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/g_node_instance.py
--rw-r--r--   0        0        0      734 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/gps_point.py
--rw-r--r--   0        0        0     2482 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/market_type.py
--rw-r--r--   0        0        0     1494 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/data_classes/supervisor_container.py
--rw-r--r--   0        0        0    14466 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/demo_methods.py
--rw-r--r--   0        0        0      276 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/__init__.py
--rw-r--r--   0        0        0     1792 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_discoverer.py
--rw-r--r--   0        0        0    11883 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_ta_owner.py
--rw-r--r--   0        0        0    10994 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_validator.py
--rw-r--r--   0        0        0     1171 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dev_utils/make_plants.py
--rw-r--r--   0        0        0    11409 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract.py
--rw-r--r--   0        0        0    12463 2023-04-29 18:36:00.015173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/application.json
--rw-r--r--   0        0        0     5229 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/approval.teal
--rw-r--r--   0        0        0       40 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/clear.teal
--rw-r--r--   0        0        0     3937 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/contract.json
--rw-r--r--   0        0        0     2116 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/__init__.py
--rw-r--r--   0        0        0      673 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/algo_cert_type.py
--rw-r--r--   0        0        0      638 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/atn_spaceheat_strategy_name.py
--rw-r--r--   0        0        0      990 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/core_g_node_role.py
--rw-r--r--   0        0        0      700 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/distribution_tariff.py
--rw-r--r--   0        0        0      598 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/emitter_pump_feedback_model.py
--rw-r--r--   0        0        0      614 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/energy_supply_type.py
--rw-r--r--   0        0        0     2246 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/g_node_role.py
--rw-r--r--   0        0        0      992 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/g_node_status.py
--rw-r--r--   0        0        0      933 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/gni_status.py
--rw-r--r--   0        0        0      563 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_price_unit.py
--rw-r--r--   0        0        0      590 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_quantity_unit.py
--rw-r--r--   0        0        0     1394 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/market_type_name.py
--rw-r--r--   0        0        0     1326 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/message_category.py
--rw-r--r--   0        0        0     1189 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/message_category_symbol.py
--rw-r--r--   0        0        0      928 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/mixing_valve_feedback_model.py
--rw-r--r--   0        0        0      626 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/recognized_currency_unit.py
--rw-r--r--   0        0        0      570 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/recognized_temperature_unit.py
--rw-r--r--   0        0        0     1331 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/strategy_name.py
--rw-r--r--   0        0        0     1081 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/supervisor_container_status.py
--rw-r--r--   0        0        0     1918 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/enums/telemetry_name.py
--rw-r--r--   0        0        0      795 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/enums/universe_type.py
--rw-r--r--   0        0        0     6718 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/freedom_hack.py
--rw-r--r--   0        0        0        0 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/py.typed
--rw-r--r--   0        0        0     7945 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.json
--rw-r--r--   0        0        0    12518 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.py
--rw-r--r--   0        0        0    26857 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/scada_actor.py
--rw-r--r--   0        0        0      834 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/scada_codec.py
--rw-r--r--   0        0        0     4870 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/simple_atn_actor.py
--rw-r--r--   0        0        0     3169 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/ta_daemon_rest_api.py
--rw-r--r--   0        0        0      460 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/ta_validator_rest_api.py
--rw-r--r--   0        0        0    47761 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/two_channel_actor_base.py
--rw-r--r--   0        0        0    13293 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/__init__.py
--rw-r--r--   0        0        0     7780 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/accepted_bid.py
--rw-r--r--   0        0        0    20134 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_bid.py
--rw-r--r--   0        0        0    34181 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_params_heatpumpwithbooststore.py
--rw-r--r--   0        0        0     7953 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    20209 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/base_g_node_gt.py
--rw-r--r--   0        0        0     8221 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/basegnode_scada_create.py
--rw-r--r--   0        0        0    11106 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_distp_sync.py
--rw-r--r--   0        0        0    11354 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_eprt_sync.py
--rw-r--r--   0        0        0    11280 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_heat_profile.py
--rw-r--r--   0        0        0    21761 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/csv_weather_forecast_sync.py
--rw-r--r--   0        0        0     1067 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/data_channel.py
--rw-r--r--   0        0        0     9785 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/discoverycert_algo_create.py
--rw-r--r--   0        0        0     7659 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    38712 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/flo_params_heatpumpwithbooststore.py
--rw-r--r--   0        0        0    24513 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/g_node_gt.py
--rw-r--r--   0        0        0    15767 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/g_node_instance_gt.py
--rw-r--r--   0        0        0     8106 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/gt_dispatch_boolean.py
--rw-r--r--   0        0        0     6718 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/gw_cert_id.py
--rw-r--r--   0        0        0     3501 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_a.py
--rw-r--r--   0        0        0     4539 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_algo_audit.py
--rw-r--r--   0        0        0     8767 2023-04-29 18:36:12.755277 gridworks_atn-0.2.4/src/gwatn/types/heartbeat_b.py
--rw-r--r--   0        0        0     5919 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_create.py
--rw-r--r--   0        0        0     7420 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_optin.py
--rw-r--r--   0        0        0     8742 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_transfer.py
--rw-r--r--   0        0        0     7959 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/join_dispatch_contract.py
--rw-r--r--   0        0        0    12341 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/latest_price.py
--rw-r--r--   0        0        0     4928 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/market_slot.py
--rw-r--r--   0        0        0    17073 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/market_type_gt.py
--rw-r--r--   0        0        0     5294 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_algo_optin.py
--rw-r--r--   0        0        0     5196 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_send.py
--rw-r--r--   0        0        0     5024 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/old_tadeed_algo_return.py
--rw-r--r--   0        0        0     8361 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/price_quantity.py
--rw-r--r--   0        0        0     2392 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/price_quantity_unitless.py
--rw-r--r--   0        0        0     5580 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/ready.py
--rw-r--r--   0        0        0     4904 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/scada_cert_transfer.py
--rw-r--r--   0        0        0     6545 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sim_scada_driver_report.py
--rw-r--r--   0        0        0     8097 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sim_timestep.py
--rw-r--r--   0        0        0     3120 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/sla_enter.py
--rw-r--r--   0        0        0     7390 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/snapshot_heatpumpwithbooststore.py
--rw-r--r--   0        0        0     6080 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/super_starter.py
--rw-r--r--   0        0        0    12065 2023-04-29 18:36:00.019173 gridworks_atn-0.2.4/src/gwatn/types/supervisor_container_gt.py
--rw-r--r--   0        0        0     4001 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tadeed_specs_hack.py
--rw-r--r--   0        0        0     8981 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_create.py
--rw-r--r--   0        0        0    10763 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_transfer.py
--rw-r--r--   0        0        0     5142 2023-04-29 18:36:00.023173 gridworks_atn-0.2.4/src/gwatn/types/terminalasset_certify_hack.py
--rw-r--r--   0        0        0     4053 1970-01-01 00:00:00.000000 gridworks_atn-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-11 15:49:23.166622 gridworks_atn-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3002 2023-05-11 15:49:23.166622 gridworks_atn-0.3.2/README.md
+-rw-r--r--   0        0        0     2193 2023-05-11 15:49:44.203060 gridworks_atn-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      537 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/__init__.py
+-rw-r--r--   0        0        0      226 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/__main__.py
+-rw-r--r--   0        0        0    13411 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/api_types.py
+-rw-r--r--   0        0        0    21728 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/atn_actor_base.py
+-rw-r--r--   0        0        0     1655 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/atn_utils.py
+-rw-r--r--   0        0        0    19478 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/atn.py
+-rw-r--r--   0        0        0       98 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/dev_atn_params_data.csv
+-rw-r--r--   0        0        0      867 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/edge.py
+-rw-r--r--   0        0        0     7536 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/flo.py
+-rw-r--r--   0        0        0    18484 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/flo_output.py
+-rw-r--r--   0        0        0     2014 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/make_dev_input_data.py
+-rw-r--r--   0        0        0      841 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/node.py
+-rw-r--r--   0        0        0     6963 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/simple_scada_sim.py
+-rw-r--r--   0        0        0     2472 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/brick_storage_heater/strategy_utils.py
+-rw-r--r--   0        0        0     4871 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/config.py
+-rw-r--r--   0        0        0     6148 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/data_classes/.DS_Store
+-rw-r--r--   0        0        0      601 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/data_classes/__init__.py
+-rw-r--r--   0        0        0      583 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/data_classes/d_edge.py
+-rw-r--r--   0        0        0     7812 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/data_classes/d_graph.py
+-rw-r--r--   0        0        0     1559 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/data_classes/d_node.py
+-rw-r--r--   0        0        0    14466 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/demo_methods.py
+-rw-r--r--   0        0        0      276 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dev_utils/__init__.py
+-rw-r--r--   0        0        0     1792 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_discoverer.py
+-rw-r--r--   0        0        0    11883 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_ta_owner.py
+-rw-r--r--   0        0        0    10994 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_validator.py
+-rw-r--r--   0        0        0     1171 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dev_utils/make_plants.py
+-rw-r--r--   0        0        0    11409 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dispatch_contract.py
+-rw-r--r--   0        0        0    12463 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/application.json
+-rw-r--r--   0        0        0     5229 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/approval.teal
+-rw-r--r--   0        0        0       40 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/clear.teal
+-rw-r--r--   0        0        0     3937 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/contract.json
+-rw-r--r--   0        0        0     1961 2023-05-11 15:49:23.178623 gridworks_atn-0.3.2/src/gwatn/enums/__init__.py
+-rw-r--r--   0        0        0      700 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/enums/distribution_tariff.py
+-rw-r--r--   0        0        0      614 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/enums/energy_supply_type.py
+-rw-r--r--   0        0        0      570 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/enums/recognized_temperature_unit.py
+-rw-r--r--   0        0        0      122 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/errors.py
+-rw-r--r--   0        0        0        0 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/py.typed
+-rw-r--r--   0        0        0     7945 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/python_ta_daemon.json
+-rw-r--r--   0        0        0    12518 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/python_ta_daemon.py
+-rw-r--r--   0        0        0      834 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/scada_codec.py
+-rw-r--r--   0        0        0     4870 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/simple_atn_actor.py
+-rw-r--r--   0        0        0    26139 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/simple_scada_sim_actor_base.py
+-rw-r--r--   0        0        0     3169 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/ta_daemon_rest_api.py
+-rw-r--r--   0        0        0      460 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/ta_validator_rest_api.py
+-rw-r--r--   0        0        0    47761 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/two_channel_actor_base.py
+-rw-r--r--   0        0        0    13145 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/__init__.py
+-rw-r--r--   0        0        0     7868 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/accepted_bid.py
+-rw-r--r--   0        0        0    20222 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/atn_bid.py
+-rw-r--r--   0        0        0     4288 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/atn_params.py
+-rw-r--r--   0        0        0    22335 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/atn_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8144 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/atn_params_report.py
+-rw-r--r--   0        0        0     8321 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/basegnode_scada_create.py
+-rw-r--r--   0        0        0    11106 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/csv_distp_sync.py
+-rw-r--r--   0        0        0    11354 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/csv_eprt_sync.py
+-rw-r--r--   0        0        0    21761 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/csv_weather_forecast_sync.py
+-rw-r--r--   0        0        0     1067 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/data_channel.py
+-rw-r--r--   0        0        0     9885 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/discoverycert_algo_create.py
+-rw-r--r--   0        0        0     8092 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/dispatch_contract_confirmed.py
+-rw-r--r--   0        0        0     7648 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/flo_params.py
+-rw-r--r--   0        0        0    22826 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/flo_params_brickstorageheater.py
+-rw-r--r--   0        0        0     8827 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/flo_params_report.py
+-rw-r--r--   0        0        0     8206 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/gt_dispatch_boolean.py
+-rw-r--r--   0        0        0     9155 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/heartbeat_b.py
+-rw-r--r--   0        0        0     6154 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_create.py
+-rw-r--r--   0        0        0     7610 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     8932 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_transfer.py
+-rw-r--r--   0        0        0     7959 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/join_dispatch_contract.py
+-rw-r--r--   0        0        0    12429 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/latest_price.py
+-rw-r--r--   0        0        0     5028 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/market_slot.py
+-rw-r--r--   0        0        0    17161 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/market_type_gt.py
+-rw-r--r--   0        0        0     5294 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/new_tadeed_algo_optin.py
+-rw-r--r--   0        0        0     5196 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/new_tadeed_send.py
+-rw-r--r--   0        0        0     5024 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/old_tadeed_algo_return.py
+-rw-r--r--   0        0        0     8461 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/price_quantity.py
+-rw-r--r--   0        0        0     2492 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/price_quantity_unitless.py
+-rw-r--r--   0        0        0     5004 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/scada_cert_transfer.py
+-rw-r--r--   0        0        0     3682 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/simplesim_driver_data.py
+-rw-r--r--   0        0        0     4166 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/simplesim_driver_data_bsh.py
+-rw-r--r--   0        0        0     6534 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/simplesim_driver_report.py
+-rw-r--r--   0        0        0     6774 2023-05-11 15:49:23.182623 gridworks_atn-0.3.2/src/gwatn/types/simplesim_snapshot_brickstorageheater.py
+-rw-r--r--   0        0        0     3220 2023-05-11 15:49:23.186623 gridworks_atn-0.3.2/src/gwatn/types/sla_enter.py
+-rw-r--r--   0        0        0     4101 2023-05-11 15:49:23.186623 gridworks_atn-0.3.2/src/gwatn/types/tadeed_specs_hack.py
+-rw-r--r--   0        0        0     5734 2023-05-11 15:49:23.186623 gridworks_atn-0.3.2/src/gwatn/types/tavalidatorcert_algo_create.py
+-rw-r--r--   0        0        0     6371 2023-05-11 15:49:23.186623 gridworks_atn-0.3.2/src/gwatn/types/tavalidatorcert_algo_transfer.py
+-rw-r--r--   0        0        0     5242 2023-05-11 15:49:23.186623 gridworks_atn-0.3.2/src/gwatn/types/terminalasset_certify_hack.py
+-rw-r--r--   0        0        0     3949 1970-01-01 00:00:00.000000 gridworks_atn-0.3.2/PKG-INFO
```

### Comparing `gridworks_atn-0.2.4/LICENSE` & `gridworks_atn-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/README.md` & `gridworks_atn-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/pyproject.toml` & `gridworks_atn-0.3.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridworks-atn"
-version = "0.2.4"
+version = "0.3.2"
 description = "Gridworks Atn Spaceheat"
 authors = ["Jessica Millar <jmillar@gridworks-consulting.com>"]
 license = "None"
 readme = "README.md"
 homepage = "https://github.com/thegridelectric/gridworks-atn"
 repository = "https://github.com/thegridelectric/gridworks-atn"
 documentation = "https://gridworks-atn.readthedocs.io"
@@ -16,20 +16,20 @@
 ]
 
 [tool.poetry.urls]
 Changelog = "https://github.com/thegridelectric/gridworks-atn/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
-gridworks = "^0.2.1"
-gridworks-protocol = "^0.4.5"
-gridworks-proactor = "^0.1.8"
+gridworks = "^0.2.4"
+gridworks-protocol = "^0.5.2" # Note gridworks-protocol includes gridworks; these must stay in sync
+# gridworks-proactor = "^0.1.8"
 paho-mqtt = "^1.6.1"
 
-types-requests = "^2.28.11.2"
+
 numpy = "^1.23.4"
 
 
 
 [tool.poetry.dev-dependencies]
 Pygments = ">=2.10.0"
 black = ">=21.10b0"
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/api_types.py` & `gridworks_atn-0.3.2/src/gwatn/python_ta_daemon.json`

 * *Files 27% similar despite different names*

```diff
@@ -1,468 +1,497 @@
-00000000: 2222 2220 4c69 7374 206f 6620 616c 6c20  """ List of all 
-00000010: 7468 6520 7479 7065 7320 7573 6564 2222  the types used""
-00000020: 220a 6672 6f6d 2074 7970 696e 6720 696d  ".from typing im
-00000030: 706f 7274 2044 6963 740a 6672 6f6d 2074  port Dict.from t
-00000040: 7970 696e 6720 696d 706f 7274 204c 6973  yping import Lis
-00000050: 740a 6672 6f6d 2074 7970 696e 6720 696d  t.from typing im
-00000060: 706f 7274 206e 6f5f 7479 7065 5f63 6865  port no_type_che
-00000070: 636b 0a0a 6672 6f6d 2067 7761 746e 2e74  ck..from gwatn.t
-00000080: 7970 6573 2069 6d70 6f72 7420 4163 6365  ypes import Acce
-00000090: 7074 6564 4269 645f 4d61 6b65 720a 6672  ptedBid_Maker.fr
-000000a0: 6f6d 2067 7761 746e 2e74 7970 6573 2069  om gwatn.types i
-000000b0: 6d70 6f72 7420 4174 6e42 6964 5f4d 616b  mport AtnBid_Mak
-000000c0: 6572 0a66 726f 6d20 6777 6174 6e2e 7479  er.from gwatn.ty
-000000d0: 7065 7320 696d 706f 7274 2041 746e 5061  pes import AtnPa
-000000e0: 7261 6d73 4865 6174 7075 6d70 7769 7468  ramsHeatpumpwith
-000000f0: 626f 6f73 7473 746f 7265 5f4d 616b 6572  booststore_Maker
-00000100: 0a66 726f 6d20 6777 6174 6e2e 7479 7065  .from gwatn.type
-00000110: 7320 696d 706f 7274 2041 746e 5061 7261  s import AtnPara
-00000120: 6d73 5265 706f 7274 4865 6174 7075 6d70  msReportHeatpump
-00000130: 7769 7468 626f 6f73 7473 746f 7265 5f4d  withbooststore_M
-00000140: 616b 6572 0a66 726f 6d20 6777 6174 6e2e  aker.from gwatn.
-00000150: 7479 7065 7320 696d 706f 7274 2042 6173  types import Bas
-00000160: 6547 4e6f 6465 4774 5f4d 616b 6572 0a66  eGNodeGt_Maker.f
-00000170: 726f 6d20 6777 6174 6e2e 7479 7065 7320  rom gwatn.types 
-00000180: 696d 706f 7274 2042 6173 6567 6e6f 6465  import Basegnode
-00000190: 5363 6164 6143 7265 6174 655f 4d61 6b65  ScadaCreate_Make
-000001a0: 720a 6672 6f6d 2067 7761 746e 2e74 7970  r.from gwatn.typ
-000001b0: 6573 2069 6d70 6f72 7420 4469 7363 6f76  es import Discov
-000001c0: 6572 7963 6572 7441 6c67 6f43 7265 6174  erycertAlgoCreat
-000001d0: 655f 4d61 6b65 720a 6672 6f6d 2067 7761  e_Maker.from gwa
-000001e0: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-000001f0: 4469 7370 6174 6368 436f 6e74 7261 6374  DispatchContract
-00000200: 436f 6e66 6972 6d65 6448 6561 7470 756d  ConfirmedHeatpum
-00000210: 7077 6974 6862 6f6f 7374 7374 6f72 655f  pwithbooststore_
-00000220: 4d61 6b65 720a 6672 6f6d 2067 7761 746e  Maker.from gwatn
-00000230: 2e74 7970 6573 2069 6d70 6f72 7420 466c  .types import Fl
-00000240: 6f50 6172 616d 7348 6561 7470 756d 7077  oParamsHeatpumpw
-00000250: 6974 6862 6f6f 7374 7374 6f72 655f 4d61  ithbooststore_Ma
-00000260: 6b65 720a 6672 6f6d 2067 7761 746e 2e74  ker.from gwatn.t
-00000270: 7970 6573 2069 6d70 6f72 7420 474e 6f64  ypes import GNod
-00000280: 6547 745f 4d61 6b65 720a 6672 6f6d 2067  eGt_Maker.from g
-00000290: 7761 746e 2e74 7970 6573 2069 6d70 6f72  watn.types impor
-000002a0: 7420 474e 6f64 6549 6e73 7461 6e63 6547  t GNodeInstanceG
-000002b0: 745f 4d61 6b65 720a 6672 6f6d 2067 7761  t_Maker.from gwa
-000002c0: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-000002d0: 4774 4469 7370 6174 6368 426f 6f6c 6561  GtDispatchBoolea
-000002e0: 6e5f 4d61 6b65 720a 6672 6f6d 2067 7761  n_Maker.from gwa
-000002f0: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-00000300: 4777 4365 7274 4964 5f4d 616b 6572 0a66  GwCertId_Maker.f
-00000310: 726f 6d20 6777 6174 6e2e 7479 7065 7320  rom gwatn.types 
-00000320: 696d 706f 7274 2048 6561 7274 6265 6174  import Heartbeat
-00000330: 415f 4d61 6b65 720a 6672 6f6d 2067 7761  A_Maker.from gwa
-00000340: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-00000350: 4865 6172 7462 6561 7441 6c67 6f41 7564  HeartbeatAlgoAud
-00000360: 6974 5f4d 616b 6572 0a66 726f 6d20 6777  it_Maker.from gw
-00000370: 6174 6e2e 7479 7065 7320 696d 706f 7274  atn.types import
-00000380: 2048 6561 7274 6265 6174 425f 4d61 6b65   HeartbeatB_Make
-00000390: 720a 6672 6f6d 2067 7761 746e 2e74 7970  r.from gwatn.typ
-000003a0: 6573 2069 6d70 6f72 7420 496e 6974 6961  es import Initia
-000003b0: 6c54 6164 6565 6441 6c67 6f43 7265 6174  lTadeedAlgoCreat
-000003c0: 655f 4d61 6b65 720a 6672 6f6d 2067 7761  e_Maker.from gwa
-000003d0: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-000003e0: 496e 6974 6961 6c54 6164 6565 6441 6c67  InitialTadeedAlg
-000003f0: 6f4f 7074 696e 5f4d 616b 6572 0a66 726f  oOptin_Maker.fro
-00000400: 6d20 6777 6174 6e2e 7479 7065 7320 696d  m gwatn.types im
-00000410: 706f 7274 2049 6e69 7469 616c 5461 6465  port InitialTade
-00000420: 6564 416c 676f 5472 616e 7366 6572 5f4d  edAlgoTransfer_M
-00000430: 616b 6572 0a66 726f 6d20 6777 6174 6e2e  aker.from gwatn.
-00000440: 7479 7065 7320 696d 706f 7274 204a 6f69  types import Joi
-00000450: 6e44 6973 7061 7463 6843 6f6e 7472 6163  nDispatchContrac
-00000460: 745f 4d61 6b65 720a 6672 6f6d 2067 7761  t_Maker.from gwa
-00000470: 746e 2e74 7970 6573 2069 6d70 6f72 7420  tn.types import 
-00000480: 4c61 7465 7374 5072 6963 655f 4d61 6b65  LatestPrice_Make
-00000490: 720a 6672 6f6d 2067 7761 746e 2e74 7970  r.from gwatn.typ
-000004a0: 6573 2069 6d70 6f72 7420 4d61 726b 6574  es import Market
-000004b0: 536c 6f74 5f4d 616b 6572 0a66 726f 6d20  Slot_Maker.from 
-000004c0: 6777 6174 6e2e 7479 7065 7320 696d 706f  gwatn.types impo
-000004d0: 7274 204d 6172 6b65 7454 7970 6547 745f  rt MarketTypeGt_
-000004e0: 4d61 6b65 720a 6672 6f6d 2067 7761 746e  Maker.from gwatn
-000004f0: 2e74 7970 6573 2069 6d70 6f72 7420 4e65  .types import Ne
-00000500: 7754 6164 6565 6441 6c67 6f4f 7074 696e  wTadeedAlgoOptin
-00000510: 5f4d 616b 6572 0a66 726f 6d20 6777 6174  _Maker.from gwat
-00000520: 6e2e 7479 7065 7320 696d 706f 7274 204e  n.types import N
-00000530: 6577 5461 6465 6564 5365 6e64 5f4d 616b  ewTadeedSend_Mak
-00000540: 6572 0a66 726f 6d20 6777 6174 6e2e 7479  er.from gwatn.ty
-00000550: 7065 7320 696d 706f 7274 204f 6c64 5461  pes import OldTa
-00000560: 6465 6564 416c 676f 5265 7475 726e 5f4d  deedAlgoReturn_M
-00000570: 616b 6572 0a66 726f 6d20 6777 6174 6e2e  aker.from gwatn.
-00000580: 7479 7065 7320 696d 706f 7274 2050 7269  types import Pri
-00000590: 6365 5175 616e 7469 7479 5f4d 616b 6572  ceQuantity_Maker
-000005a0: 0a66 726f 6d20 6777 6174 6e2e 7479 7065  .from gwatn.type
-000005b0: 7320 696d 706f 7274 2050 7269 6365 5175  s import PriceQu
-000005c0: 616e 7469 7479 556e 6974 6c65 7373 5f4d  antityUnitless_M
-000005d0: 616b 6572 0a66 726f 6d20 6777 6174 6e2e  aker.from gwatn.
-000005e0: 7479 7065 7320 696d 706f 7274 2052 6561  types import Rea
-000005f0: 6479 5f4d 616b 6572 0a66 726f 6d20 6777  dy_Maker.from gw
-00000600: 6174 6e2e 7479 7065 7320 696d 706f 7274  atn.types import
-00000610: 2053 6361 6461 4365 7274 5472 616e 7366   ScadaCertTransf
-00000620: 6572 5f4d 616b 6572 0a66 726f 6d20 6777  er_Maker.from gw
-00000630: 6174 6e2e 7479 7065 7320 696d 706f 7274  atn.types import
-00000640: 2053 696d 5363 6164 6144 7269 7665 7252   SimScadaDriverR
-00000650: 6570 6f72 745f 4d61 6b65 720a 6672 6f6d  eport_Maker.from
-00000660: 2067 7761 746e 2e74 7970 6573 2069 6d70   gwatn.types imp
-00000670: 6f72 7420 5369 6d54 696d 6573 7465 705f  ort SimTimestep_
-00000680: 4d61 6b65 720a 6672 6f6d 2067 7761 746e  Maker.from gwatn
-00000690: 2e74 7970 6573 2069 6d70 6f72 7420 536c  .types import Sl
-000006a0: 6145 6e74 6572 5f4d 616b 6572 0a66 726f  aEnter_Maker.fro
-000006b0: 6d20 6777 6174 6e2e 7479 7065 7320 696d  m gwatn.types im
-000006c0: 706f 7274 2053 6e61 7073 686f 7448 6561  port SnapshotHea
-000006d0: 7470 756d 7077 6974 6862 6f6f 7374 7374  tpumpwithboostst
-000006e0: 6f72 655f 4d61 6b65 720a 6672 6f6d 2067  ore_Maker.from g
-000006f0: 7761 746e 2e74 7970 6573 2069 6d70 6f72  watn.types impor
-00000700: 7420 5375 7065 7253 7461 7274 6572 5f4d  t SuperStarter_M
-00000710: 616b 6572 0a66 726f 6d20 6777 6174 6e2e  aker.from gwatn.
-00000720: 7479 7065 7320 696d 706f 7274 2053 7570  types import Sup
-00000730: 6572 7669 736f 7243 6f6e 7461 696e 6572  ervisorContainer
-00000740: 4774 5f4d 616b 6572 0a66 726f 6d20 6777  Gt_Maker.from gw
-00000750: 6174 6e2e 7479 7065 7320 696d 706f 7274  atn.types import
-00000760: 2054 6164 6565 6453 7065 6373 4861 636b   TadeedSpecsHack
-00000770: 5f4d 616b 6572 0a66 726f 6d20 6777 6174  _Maker.from gwat
-00000780: 6e2e 7479 7065 7320 696d 706f 7274 2054  n.types import T
-00000790: 6176 616c 6964 6174 6f72 6365 7274 416c  avalidatorcertAl
-000007a0: 676f 4372 6561 7465 5f4d 616b 6572 0a66  goCreate_Maker.f
-000007b0: 726f 6d20 6777 6174 6e2e 7479 7065 7320  rom gwatn.types 
-000007c0: 696d 706f 7274 2054 6176 616c 6964 6174  import Tavalidat
-000007d0: 6f72 6365 7274 416c 676f 5472 616e 7366  orcertAlgoTransf
-000007e0: 6572 5f4d 616b 6572 0a66 726f 6d20 6777  er_Maker.from gw
-000007f0: 6174 6e2e 7479 7065 7320 696d 706f 7274  atn.types import
-00000800: 2054 6572 6d69 6e61 6c61 7373 6574 4365   TerminalassetCe
-00000810: 7274 6966 7948 6163 6b5f 4d61 6b65 720a  rtifyHack_Maker.
-00000820: 0a0a 5479 7065 4d61 6b65 7242 794e 616d  ..TypeMakerByNam
-00000830: 653a 2044 6963 745b 7374 722c 2048 6561  e: Dict[str, Hea
-00000840: 7274 6265 6174 415f 4d61 6b65 725d 203d  rtbeatA_Maker] =
-00000850: 207b 7d0a 0a0a 406e 6f5f 7479 7065 5f63   {}...@no_type_c
-00000860: 6865 636b 0a64 6566 2074 7970 655f 6d61  heck.def type_ma
-00000870: 6b65 7273 2829 202d 3e20 4c69 7374 5b48  kers() -> List[H
-00000880: 6561 7274 6265 6174 415f 4d61 6b65 725d  eartbeatA_Maker]
-00000890: 3a0a 2020 2020 7265 7475 726e 205b 0a20  :.    return [. 
-000008a0: 2020 2020 2020 2041 6363 6570 7465 6442         AcceptedB
-000008b0: 6964 5f4d 616b 6572 2c0a 2020 2020 2020  id_Maker,.      
-000008c0: 2020 4174 6e42 6964 5f4d 616b 6572 2c0a    AtnBid_Maker,.
-000008d0: 2020 2020 2020 2020 4174 6e50 6172 616d          AtnParam
-000008e0: 7348 6561 7470 756d 7077 6974 6862 6f6f  sHeatpumpwithboo
-000008f0: 7374 7374 6f72 655f 4d61 6b65 722c 0a20  ststore_Maker,. 
-00000900: 2020 2020 2020 2041 746e 5061 7261 6d73         AtnParams
-00000910: 5265 706f 7274 4865 6174 7075 6d70 7769  ReportHeatpumpwi
-00000920: 7468 626f 6f73 7473 746f 7265 5f4d 616b  thbooststore_Mak
-00000930: 6572 2c0a 2020 2020 2020 2020 4261 7365  er,.        Base
-00000940: 474e 6f64 6547 745f 4d61 6b65 722c 0a20  GNodeGt_Maker,. 
-00000950: 2020 2020 2020 2042 6173 6567 6e6f 6465         Basegnode
-00000960: 5363 6164 6143 7265 6174 655f 4d61 6b65  ScadaCreate_Make
-00000970: 722c 0a20 2020 2020 2020 2044 6973 636f  r,.        Disco
-00000980: 7665 7279 6365 7274 416c 676f 4372 6561  verycertAlgoCrea
-00000990: 7465 5f4d 616b 6572 2c0a 2020 2020 2020  te_Maker,.      
-000009a0: 2020 4469 7370 6174 6368 436f 6e74 7261    DispatchContra
-000009b0: 6374 436f 6e66 6972 6d65 6448 6561 7470  ctConfirmedHeatp
-000009c0: 756d 7077 6974 6862 6f6f 7374 7374 6f72  umpwithbooststor
-000009d0: 655f 4d61 6b65 722c 0a20 2020 2020 2020  e_Maker,.       
-000009e0: 2046 6c6f 5061 7261 6d73 4865 6174 7075   FloParamsHeatpu
-000009f0: 6d70 7769 7468 626f 6f73 7473 746f 7265  mpwithbooststore
-00000a00: 5f4d 616b 6572 2c0a 2020 2020 2020 2020  _Maker,.        
-00000a10: 474e 6f64 6547 745f 4d61 6b65 722c 0a20  GNodeGt_Maker,. 
-00000a20: 2020 2020 2020 2047 4e6f 6465 496e 7374         GNodeInst
-00000a30: 616e 6365 4774 5f4d 616b 6572 2c0a 2020  anceGt_Maker,.  
-00000a40: 2020 2020 2020 4774 4469 7370 6174 6368        GtDispatch
-00000a50: 426f 6f6c 6561 6e5f 4d61 6b65 722c 0a20  Boolean_Maker,. 
-00000a60: 2020 2020 2020 2047 7743 6572 7449 645f         GwCertId_
-00000a70: 4d61 6b65 722c 0a20 2020 2020 2020 2048  Maker,.        H
-00000a80: 6561 7274 6265 6174 415f 4d61 6b65 722c  eartbeatA_Maker,
-00000a90: 0a20 2020 2020 2020 2048 6561 7274 6265  .        Heartbe
-00000aa0: 6174 416c 676f 4175 6469 745f 4d61 6b65  atAlgoAudit_Make
-00000ab0: 722c 0a20 2020 2020 2020 2048 6561 7274  r,.        Heart
-00000ac0: 6265 6174 425f 4d61 6b65 722c 0a20 2020  beatB_Maker,.   
-00000ad0: 2020 2020 2049 6e69 7469 616c 5461 6465       InitialTade
-00000ae0: 6564 416c 676f 4372 6561 7465 5f4d 616b  edAlgoCreate_Mak
-00000af0: 6572 2c0a 2020 2020 2020 2020 496e 6974  er,.        Init
-00000b00: 6961 6c54 6164 6565 6441 6c67 6f4f 7074  ialTadeedAlgoOpt
-00000b10: 696e 5f4d 616b 6572 2c0a 2020 2020 2020  in_Maker,.      
-00000b20: 2020 496e 6974 6961 6c54 6164 6565 6441    InitialTadeedA
-00000b30: 6c67 6f54 7261 6e73 6665 725f 4d61 6b65  lgoTransfer_Make
-00000b40: 722c 0a20 2020 2020 2020 204a 6f69 6e44  r,.        JoinD
-00000b50: 6973 7061 7463 6843 6f6e 7472 6163 745f  ispatchContract_
-00000b60: 4d61 6b65 722c 0a20 2020 2020 2020 204c  Maker,.        L
-00000b70: 6174 6573 7450 7269 6365 5f4d 616b 6572  atestPrice_Maker
-00000b80: 2c0a 2020 2020 2020 2020 4d61 726b 6574  ,.        Market
-00000b90: 536c 6f74 5f4d 616b 6572 2c0a 2020 2020  Slot_Maker,.    
-00000ba0: 2020 2020 4d61 726b 6574 5479 7065 4774      MarketTypeGt
-00000bb0: 5f4d 616b 6572 2c0a 2020 2020 2020 2020  _Maker,.        
-00000bc0: 4e65 7754 6164 6565 6441 6c67 6f4f 7074  NewTadeedAlgoOpt
-00000bd0: 696e 5f4d 616b 6572 2c0a 2020 2020 2020  in_Maker,.      
-00000be0: 2020 4e65 7754 6164 6565 6453 656e 645f    NewTadeedSend_
-00000bf0: 4d61 6b65 722c 0a20 2020 2020 2020 204f  Maker,.        O
-00000c00: 6c64 5461 6465 6564 416c 676f 5265 7475  ldTadeedAlgoRetu
-00000c10: 726e 5f4d 616b 6572 2c0a 2020 2020 2020  rn_Maker,.      
-00000c20: 2020 5072 6963 6551 7561 6e74 6974 795f    PriceQuantity_
-00000c30: 4d61 6b65 722c 0a20 2020 2020 2020 2050  Maker,.        P
-00000c40: 7269 6365 5175 616e 7469 7479 556e 6974  riceQuantityUnit
-00000c50: 6c65 7373 5f4d 616b 6572 2c0a 2020 2020  less_Maker,.    
-00000c60: 2020 2020 5265 6164 795f 4d61 6b65 722c      Ready_Maker,
-00000c70: 0a20 2020 2020 2020 2053 6361 6461 4365  .        ScadaCe
-00000c80: 7274 5472 616e 7366 6572 5f4d 616b 6572  rtTransfer_Maker
-00000c90: 2c0a 2020 2020 2020 2020 5369 6d53 6361  ,.        SimSca
-00000ca0: 6461 4472 6976 6572 5265 706f 7274 5f4d  daDriverReport_M
-00000cb0: 616b 6572 2c0a 2020 2020 2020 2020 5369  aker,.        Si
-00000cc0: 6d54 696d 6573 7465 705f 4d61 6b65 722c  mTimestep_Maker,
-00000cd0: 0a20 2020 2020 2020 2053 6c61 456e 7465  .        SlaEnte
-00000ce0: 725f 4d61 6b65 722c 0a20 2020 2020 2020  r_Maker,.       
-00000cf0: 2053 6e61 7073 686f 7448 6561 7470 756d   SnapshotHeatpum
-00000d00: 7077 6974 6862 6f6f 7374 7374 6f72 655f  pwithbooststore_
-00000d10: 4d61 6b65 722c 0a20 2020 2020 2020 2053  Maker,.        S
-00000d20: 7570 6572 5374 6172 7465 725f 4d61 6b65  uperStarter_Make
-00000d30: 722c 0a20 2020 2020 2020 2053 7570 6572  r,.        Super
-00000d40: 7669 736f 7243 6f6e 7461 696e 6572 4774  visorContainerGt
-00000d50: 5f4d 616b 6572 2c0a 2020 2020 2020 2020  _Maker,.        
-00000d60: 5461 6465 6564 5370 6563 7348 6163 6b5f  TadeedSpecsHack_
-00000d70: 4d61 6b65 722c 0a20 2020 2020 2020 2054  Maker,.        T
-00000d80: 6176 616c 6964 6174 6f72 6365 7274 416c  avalidatorcertAl
-00000d90: 676f 4372 6561 7465 5f4d 616b 6572 2c0a  goCreate_Maker,.
-00000da0: 2020 2020 2020 2020 5461 7661 6c69 6461          Tavalida
-00000db0: 746f 7263 6572 7441 6c67 6f54 7261 6e73  torcertAlgoTrans
-00000dc0: 6665 725f 4d61 6b65 722c 0a20 2020 2020  fer_Maker,.     
-00000dd0: 2020 2054 6572 6d69 6e61 6c61 7373 6574     Terminalasset
-00000de0: 4365 7274 6966 7948 6163 6b5f 4d61 6b65  CertifyHack_Make
-00000df0: 722c 0a20 2020 205d 0a0a 0a66 6f72 206d  r,.    ]...for m
-00000e00: 616b 6572 2069 6e20 7479 7065 5f6d 616b  aker in type_mak
-00000e10: 6572 7328 293a 0a20 2020 2054 7970 654d  ers():.    TypeM
-00000e20: 616b 6572 4279 4e61 6d65 5b6d 616b 6572  akerByName[maker
-00000e30: 2e74 7970 655f 6e61 6d65 5d20 3d20 6d61  .type_name] = ma
-00000e40: 6b65 720a 0a0a 6465 6620 7665 7273 696f  ker...def versio
-00000e50: 6e5f 6279 5f74 7970 655f 6e61 6d65 2829  n_by_type_name()
-00000e60: 202d 3e20 4469 6374 5b73 7472 2c20 7374   -> Dict[str, st
-00000e70: 725d 3a0a 2020 2020 2222 220a 2020 2020  r]:.    """.    
-00000e80: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00000e90: 2044 6963 745b 7374 722c 2073 7472 5d3a   Dict[str, str]:
-00000ea0: 204b 6579 7320 6172 6520 5479 7065 4e61   Keys are TypeNa
-00000eb0: 6d65 732c 2076 616c 7565 7320 6172 6520  mes, values are 
-00000ec0: 7665 7273 696f 6e73 0a20 2020 2022 2222  versions.    """
-00000ed0: 0a0a 2020 2020 763a 2044 6963 745b 7374  ..    v: Dict[st
-00000ee0: 722c 2073 7472 5d20 3d20 7b0a 2020 2020  r, str] = {.    
-00000ef0: 2020 2020 2261 6363 6570 7465 642e 6269      "accepted.bi
-00000f00: 6422 3a20 2230 3030 222c 0a20 2020 2020  d": "000",.     
-00000f10: 2020 2022 6174 6e2e 6269 6422 3a20 2230     "atn.bid": "0
-00000f20: 3031 222c 0a20 2020 2020 2020 2022 6174  01",.        "at
-00000f30: 6e2e 7061 7261 6d73 2e68 6561 7470 756d  n.params.heatpum
-00000f40: 7077 6974 6862 6f6f 7374 7374 6f72 6522  pwithbooststore"
-00000f50: 3a20 2230 3030 222c 0a20 2020 2020 2020  : "000",.       
-00000f60: 2022 6174 6e2e 7061 7261 6d73 2e72 6570   "atn.params.rep
-00000f70: 6f72 742e 6865 6174 7075 6d70 7769 7468  ort.heatpumpwith
-00000f80: 626f 6f73 7473 746f 7265 223a 2022 3030  booststore": "00
-00000f90: 3022 2c0a 2020 2020 2020 2020 2262 6173  0",.        "bas
-00000fa0: 652e 672e 6e6f 6465 2e67 7422 3a20 2230  e.g.node.gt": "0
-00000fb0: 3032 222c 0a20 2020 2020 2020 2022 6261  02",.        "ba
-00000fc0: 7365 676e 6f64 652e 7363 6164 612e 6372  segnode.scada.cr
-00000fd0: 6561 7465 223a 2022 3030 3022 2c0a 2020  eate": "000",.  
-00000fe0: 2020 2020 2020 2264 6973 636f 7665 7279        "discovery
-00000ff0: 6365 7274 2e61 6c67 6f2e 6372 6561 7465  cert.algo.create
-00001000: 223a 2022 3030 3022 2c0a 2020 2020 2020  ": "000",.      
-00001010: 2020 2264 6973 7061 7463 682e 636f 6e74    "dispatch.cont
-00001020: 7261 6374 2e63 6f6e 6669 726d 6564 2e68  ract.confirmed.h
-00001030: 6561 7470 756d 7077 6974 6862 6f6f 7374  eatpumpwithboost
-00001040: 7374 6f72 6522 3a20 2230 3030 222c 0a20  store": "000",. 
-00001050: 2020 2020 2020 2022 666c 6f2e 7061 7261         "flo.para
-00001060: 6d73 2e68 6561 7470 756d 7077 6974 6862  ms.heatpumpwithb
-00001070: 6f6f 7374 7374 6f72 6522 3a20 2230 3030  ooststore": "000
-00001080: 222c 0a20 2020 2020 2020 2022 672e 6e6f  ",.        "g.no
-00001090: 6465 2e67 7422 3a20 2230 3032 222c 0a20  de.gt": "002",. 
-000010a0: 2020 2020 2020 2022 672e 6e6f 6465 2e69         "g.node.i
-000010b0: 6e73 7461 6e63 652e 6774 223a 2022 3030  nstance.gt": "00
-000010c0: 3022 2c0a 2020 2020 2020 2020 2267 742e  0",.        "gt.
-000010d0: 6469 7370 6174 6368 2e62 6f6f 6c65 616e  dispatch.boolean
-000010e0: 223a 2022 3131 3022 2c0a 2020 2020 2020  ": "110",.      
-000010f0: 2020 2267 772e 6365 7274 2e69 6422 3a20    "gw.cert.id": 
-00001100: 2230 3030 222c 0a20 2020 2020 2020 2022  "000",.        "
-00001110: 6865 6172 7462 6561 742e 6122 3a20 2231  heartbeat.a": "1
-00001120: 3030 222c 0a20 2020 2020 2020 2022 6865  00",.        "he
-00001130: 6172 7462 6561 742e 616c 676f 2e61 7564  artbeat.algo.aud
-00001140: 6974 223a 2022 3030 3022 2c0a 2020 2020  it": "000",.    
-00001150: 2020 2020 2268 6561 7274 6265 6174 2e62      "heartbeat.b
-00001160: 223a 2022 3030 3122 2c0a 2020 2020 2020  ": "001",.      
-00001170: 2020 2269 6e69 7469 616c 2e74 6164 6565    "initial.tadee
-00001180: 642e 616c 676f 2e63 7265 6174 6522 3a20  d.algo.create": 
-00001190: 2230 3030 222c 0a20 2020 2020 2020 2022  "000",.        "
-000011a0: 696e 6974 6961 6c2e 7461 6465 6564 2e61  initial.tadeed.a
-000011b0: 6c67 6f2e 6f70 7469 6e22 3a20 2230 3032  lgo.optin": "002
-000011c0: 222c 0a20 2020 2020 2020 2022 696e 6974  ",.        "init
-000011d0: 6961 6c2e 7461 6465 6564 2e61 6c67 6f2e  ial.tadeed.algo.
-000011e0: 7472 616e 7366 6572 223a 2022 3030 3022  transfer": "000"
-000011f0: 2c0a 2020 2020 2020 2020 226a 6f69 6e2e  ,.        "join.
-00001200: 6469 7370 6174 6368 2e63 6f6e 7472 6163  dispatch.contrac
-00001210: 7422 3a20 2230 3030 222c 0a20 2020 2020  t": "000",.     
-00001220: 2020 2022 6c61 7465 7374 2e70 7269 6365     "latest.price
-00001230: 223a 2022 3030 3022 2c0a 2020 2020 2020  ": "000",.      
-00001240: 2020 226d 6172 6b65 742e 736c 6f74 223a    "market.slot":
-00001250: 2022 3030 3022 2c0a 2020 2020 2020 2020   "000",.        
-00001260: 226d 6172 6b65 742e 7479 7065 2e67 7422  "market.type.gt"
-00001270: 3a20 2230 3030 222c 0a20 2020 2020 2020  : "000",.       
-00001280: 2022 6e65 772e 7461 6465 6564 2e61 6c67   "new.tadeed.alg
-00001290: 6f2e 6f70 7469 6e22 3a20 2230 3030 222c  o.optin": "000",
-000012a0: 0a20 2020 2020 2020 2022 6e65 772e 7461  .        "new.ta
-000012b0: 6465 6564 2e73 656e 6422 3a20 2230 3030  deed.send": "000
-000012c0: 222c 0a20 2020 2020 2020 2022 6f6c 642e  ",.        "old.
-000012d0: 7461 6465 6564 2e61 6c67 6f2e 7265 7475  tadeed.algo.retu
-000012e0: 726e 223a 2022 3030 3022 2c0a 2020 2020  rn": "000",.    
-000012f0: 2020 2020 2270 7269 6365 2e71 7561 6e74      "price.quant
-00001300: 6974 7922 3a20 2230 3030 222c 0a20 2020  ity": "000",.   
-00001310: 2020 2020 2022 7072 6963 652e 7175 616e       "price.quan
-00001320: 7469 7479 2e75 6e69 746c 6573 7322 3a20  tity.unitless": 
-00001330: 2230 3030 222c 0a20 2020 2020 2020 2022  "000",.        "
-00001340: 7265 6164 7922 3a20 2230 3031 222c 0a20  ready": "001",. 
-00001350: 2020 2020 2020 2022 7363 6164 612e 6365         "scada.ce
-00001360: 7274 2e74 7261 6e73 6665 7222 3a20 2230  rt.transfer": "0
-00001370: 3030 222c 0a20 2020 2020 2020 2022 7369  00",.        "si
-00001380: 6d2e 7363 6164 612e 6472 6976 6572 2e72  m.scada.driver.r
-00001390: 6570 6f72 7422 3a20 2230 3030 222c 0a20  eport": "000",. 
-000013a0: 2020 2020 2020 2022 7369 6d2e 7469 6d65         "sim.time
-000013b0: 7374 6570 223a 2022 3030 3022 2c0a 2020  step": "000",.  
-000013c0: 2020 2020 2020 2273 6c61 2e65 6e74 6572        "sla.enter
-000013d0: 223a 2022 3030 3022 2c0a 2020 2020 2020  ": "000",.      
-000013e0: 2020 2273 6e61 7073 686f 742e 6865 6174    "snapshot.heat
-000013f0: 7075 6d70 7769 7468 626f 6f73 7473 746f  pumpwithbooststo
-00001400: 7265 223a 2022 3030 3022 2c0a 2020 2020  re": "000",.    
-00001410: 2020 2020 2273 7570 6572 2e73 7461 7274      "super.start
-00001420: 6572 223a 2022 3030 3022 2c0a 2020 2020  er": "000",.    
-00001430: 2020 2020 2273 7570 6572 7669 736f 722e      "supervisor.
-00001440: 636f 6e74 6169 6e65 722e 6774 223a 2022  container.gt": "
-00001450: 3030 3022 2c0a 2020 2020 2020 2020 2274  000",.        "t
-00001460: 6164 6565 642e 7370 6563 732e 6861 636b  adeed.specs.hack
-00001470: 223a 2022 3030 3022 2c0a 2020 2020 2020  ": "000",.      
-00001480: 2020 2274 6176 616c 6964 6174 6f72 6365    "tavalidatorce
-00001490: 7274 2e61 6c67 6f2e 6372 6561 7465 223a  rt.algo.create":
-000014a0: 2022 3030 3022 2c0a 2020 2020 2020 2020   "000",.        
-000014b0: 2274 6176 616c 6964 6174 6f72 6365 7274  "tavalidatorcert
-000014c0: 2e61 6c67 6f2e 7472 616e 7366 6572 223a  .algo.transfer":
-000014d0: 2022 3030 3022 2c0a 2020 2020 2020 2020   "000",.        
-000014e0: 2274 6572 6d69 6e61 6c61 7373 6574 2e63  "terminalasset.c
-000014f0: 6572 7469 6679 2e68 6163 6b22 3a20 2230  ertify.hack": "0
-00001500: 3030 222c 0a20 2020 207d 0a0a 2020 2020  00",.    }..    
-00001510: 7265 7475 726e 2076 0a0a 0a64 6566 2073  return v...def s
-00001520: 7461 7475 735f 6279 5f76 6572 7369 6f6e  tatus_by_version
-00001530: 6564 5f74 7970 655f 6e61 6d65 2829 202d  ed_type_name() -
-00001540: 3e20 4469 6374 5b73 7472 2c20 7374 725d  > Dict[str, str]
-00001550: 3a0a 2020 2020 2222 220a 2020 2020 5265  :.    """.    Re
-00001560: 7475 726e 733a 0a20 2020 2020 2020 2044  turns:.        D
-00001570: 6963 745b 7374 722c 2073 7472 5d3a 204b  ict[str, str]: K
-00001580: 6579 7320 6172 6520 7665 7273 696f 6e65  eys are versione
-00001590: 6420 5479 7065 4e61 6d65 732c 2076 616c  d TypeNames, val
-000015a0: 7565 7320 6172 6520 7479 7065 2073 7461  ues are type sta
-000015b0: 7475 730a 2020 2020 2222 220a 0a20 2020  tus.    """..   
-000015c0: 2076 3a20 4469 6374 5b73 7472 2c20 7374   v: Dict[str, st
-000015d0: 725d 203d 207b 0a20 2020 2020 2020 2022  r] = {.        "
-000015e0: 6163 6365 7074 6564 2e62 6964 2e30 3030  accepted.bid.000
-000015f0: 223a 2022 5065 6e64 696e 6722 2c0a 2020  ": "Pending",.  
-00001600: 2020 2020 2020 2261 746e 2e62 6964 2e30        "atn.bid.0
-00001610: 3031 223a 2022 5065 6e64 696e 6722 2c0a  01": "Pending",.
-00001620: 2020 2020 2020 2020 2261 746e 2e70 6172          "atn.par
-00001630: 616d 732e 6865 6174 7075 6d70 7769 7468  ams.heatpumpwith
-00001640: 626f 6f73 7473 746f 7265 2e30 3030 223a  booststore.000":
-00001650: 2022 4163 7469 7665 222c 0a20 2020 2020   "Active",.     
-00001660: 2020 2022 6174 6e2e 7061 7261 6d73 2e72     "atn.params.r
-00001670: 6570 6f72 742e 6865 6174 7075 6d70 7769  eport.heatpumpwi
-00001680: 7468 626f 6f73 7473 746f 7265 2e30 3030  thbooststore.000
-00001690: 223a 2022 5065 6e64 696e 6722 2c0a 2020  ": "Pending",.  
-000016a0: 2020 2020 2020 2262 6173 652e 672e 6e6f        "base.g.no
-000016b0: 6465 2e67 742e 3030 3222 3a20 2250 656e  de.gt.002": "Pen
-000016c0: 6469 6e67 222c 0a20 2020 2020 2020 2022  ding",.        "
-000016d0: 6261 7365 676e 6f64 652e 7363 6164 612e  basegnode.scada.
-000016e0: 6372 6561 7465 2e30 3030 223a 2022 5065  create.000": "Pe
-000016f0: 6e64 696e 6722 2c0a 2020 2020 2020 2020  nding",.        
-00001700: 2264 6973 636f 7665 7279 6365 7274 2e61  "discoverycert.a
-00001710: 6c67 6f2e 6372 6561 7465 2e30 3030 223a  lgo.create.000":
-00001720: 2022 5065 6e64 696e 6722 2c0a 2020 2020   "Pending",.    
-00001730: 2020 2020 2264 6973 7061 7463 682e 636f      "dispatch.co
-00001740: 6e74 7261 6374 2e63 6f6e 6669 726d 6564  ntract.confirmed
-00001750: 2e68 6561 7470 756d 7077 6974 6862 6f6f  .heatpumpwithboo
-00001760: 7374 7374 6f72 652e 3030 3022 3a20 2250  ststore.000": "P
-00001770: 656e 6469 6e67 222c 0a20 2020 2020 2020  ending",.       
-00001780: 2022 666c 6f2e 7061 7261 6d73 2e68 6561   "flo.params.hea
-00001790: 7470 756d 7077 6974 6862 6f6f 7374 7374  tpumpwithboostst
-000017a0: 6f72 652e 3030 3022 3a20 2241 6374 6976  ore.000": "Activ
-000017b0: 6522 2c0a 2020 2020 2020 2020 2267 2e6e  e",.        "g.n
-000017c0: 6f64 652e 6774 2e30 3032 223a 2022 5065  ode.gt.002": "Pe
-000017d0: 6e64 696e 6722 2c0a 2020 2020 2020 2020  nding",.        
-000017e0: 2267 2e6e 6f64 652e 696e 7374 616e 6365  "g.node.instance
-000017f0: 2e67 742e 3030 3022 3a20 2250 656e 6469  .gt.000": "Pendi
-00001800: 6e67 222c 0a20 2020 2020 2020 2022 6774  ng",.        "gt
-00001810: 2e64 6973 7061 7463 682e 626f 6f6c 6561  .dispatch.boolea
-00001820: 6e2e 3131 3022 3a20 2250 656e 6469 6e67  n.110": "Pending
-00001830: 222c 0a20 2020 2020 2020 2022 6777 2e63  ",.        "gw.c
-00001840: 6572 742e 6964 2e30 3030 223a 2022 4163  ert.id.000": "Ac
-00001850: 7469 7665 222c 0a20 2020 2020 2020 2022  tive",.        "
-00001860: 6865 6172 7462 6561 742e 612e 3130 3022  heartbeat.a.100"
-00001870: 3a20 2250 656e 6469 6e67 222c 0a20 2020  : "Pending",.   
-00001880: 2020 2020 2022 6865 6172 7462 6561 742e       "heartbeat.
-00001890: 616c 676f 2e61 7564 6974 2e30 3030 223a  algo.audit.000":
-000018a0: 2022 5065 6e64 696e 6722 2c0a 2020 2020   "Pending",.    
-000018b0: 2020 2020 2268 6561 7274 6265 6174 2e62      "heartbeat.b
-000018c0: 2e30 3031 223a 2022 5065 6e64 696e 6722  .001": "Pending"
-000018d0: 2c0a 2020 2020 2020 2020 2269 6e69 7469  ,.        "initi
-000018e0: 616c 2e74 6164 6565 642e 616c 676f 2e63  al.tadeed.algo.c
-000018f0: 7265 6174 652e 3030 3022 3a20 2241 6374  reate.000": "Act
-00001900: 6976 6522 2c0a 2020 2020 2020 2020 2269  ive",.        "i
-00001910: 6e69 7469 616c 2e74 6164 6565 642e 616c  nitial.tadeed.al
-00001920: 676f 2e6f 7074 696e 2e30 3032 223a 2022  go.optin.002": "
-00001930: 4163 7469 7665 222c 0a20 2020 2020 2020  Active",.       
-00001940: 2022 696e 6974 6961 6c2e 7461 6465 6564   "initial.tadeed
-00001950: 2e61 6c67 6f2e 7472 616e 7366 6572 2e30  .algo.transfer.0
-00001960: 3030 223a 2022 4163 7469 7665 222c 0a20  00": "Active",. 
-00001970: 2020 2020 2020 2022 6a6f 696e 2e64 6973         "join.dis
-00001980: 7061 7463 682e 636f 6e74 7261 6374 2e30  patch.contract.0
-00001990: 3030 223a 2022 4163 7469 7665 222c 0a20  00": "Active",. 
-000019a0: 2020 2020 2020 2022 6c61 7465 7374 2e70         "latest.p
-000019b0: 7269 6365 2e30 3030 223a 2022 5065 6e64  rice.000": "Pend
-000019c0: 696e 6722 2c0a 2020 2020 2020 2020 226d  ing",.        "m
-000019d0: 6172 6b65 742e 736c 6f74 2e30 3030 223a  arket.slot.000":
-000019e0: 2022 5065 6e64 696e 6722 2c0a 2020 2020   "Pending",.    
-000019f0: 2020 2020 226d 6172 6b65 742e 7479 7065      "market.type
-00001a00: 2e67 742e 3030 3022 3a20 2250 656e 6469  .gt.000": "Pendi
-00001a10: 6e67 222c 0a20 2020 2020 2020 2022 6e65  ng",.        "ne
-00001a20: 772e 7461 6465 6564 2e61 6c67 6f2e 6f70  w.tadeed.algo.op
-00001a30: 7469 6e2e 3030 3022 3a20 2241 6374 6976  tin.000": "Activ
-00001a40: 6522 2c0a 2020 2020 2020 2020 226e 6577  e",.        "new
-00001a50: 2e74 6164 6565 642e 7365 6e64 2e30 3030  .tadeed.send.000
-00001a60: 223a 2022 4163 7469 7665 222c 0a20 2020  ": "Active",.   
-00001a70: 2020 2020 2022 6f6c 642e 7461 6465 6564       "old.tadeed
-00001a80: 2e61 6c67 6f2e 7265 7475 726e 2e30 3030  .algo.return.000
-00001a90: 223a 2022 4163 7469 7665 222c 0a20 2020  ": "Active",.   
-00001aa0: 2020 2020 2022 7072 6963 652e 7175 616e       "price.quan
-00001ab0: 7469 7479 2e30 3030 223a 2022 5065 6e64  tity.000": "Pend
-00001ac0: 696e 6722 2c0a 2020 2020 2020 2020 2270  ing",.        "p
-00001ad0: 7269 6365 2e71 7561 6e74 6974 792e 756e  rice.quantity.un
-00001ae0: 6974 6c65 7373 2e30 3030 223a 2022 5065  itless.000": "Pe
-00001af0: 6e64 696e 6722 2c0a 2020 2020 2020 2020  nding",.        
-00001b00: 2272 6561 6479 2e30 3031 223a 2022 5065  "ready.001": "Pe
-00001b10: 6e64 696e 6722 2c0a 2020 2020 2020 2020  nding",.        
-00001b20: 2273 6361 6461 2e63 6572 742e 7472 616e  "scada.cert.tran
-00001b30: 7366 6572 2e30 3030 223a 2022 5065 6e64  sfer.000": "Pend
-00001b40: 696e 6722 2c0a 2020 2020 2020 2020 2273  ing",.        "s
-00001b50: 696d 2e73 6361 6461 2e64 7269 7665 722e  im.scada.driver.
-00001b60: 7265 706f 7274 2e30 3030 223a 2022 5065  report.000": "Pe
-00001b70: 6e64 696e 6722 2c0a 2020 2020 2020 2020  nding",.        
-00001b80: 2273 696d 2e74 696d 6573 7465 702e 3030  "sim.timestep.00
-00001b90: 3022 3a20 2250 656e 6469 6e67 222c 0a20  0": "Pending",. 
-00001ba0: 2020 2020 2020 2022 736c 612e 656e 7465         "sla.ente
-00001bb0: 722e 3030 3022 3a20 2250 656e 6469 6e67  r.000": "Pending
-00001bc0: 222c 0a20 2020 2020 2020 2022 736e 6170  ",.        "snap
-00001bd0: 7368 6f74 2e68 6561 7470 756d 7077 6974  shot.heatpumpwit
-00001be0: 6862 6f6f 7374 7374 6f72 652e 3030 3022  hbooststore.000"
-00001bf0: 3a20 2250 656e 6469 6e67 222c 0a20 2020  : "Pending",.   
-00001c00: 2020 2020 2022 7375 7065 722e 7374 6172       "super.star
-00001c10: 7465 722e 3030 3022 3a20 2250 656e 6469  ter.000": "Pendi
-00001c20: 6e67 222c 0a20 2020 2020 2020 2022 7375  ng",.        "su
-00001c30: 7065 7276 6973 6f72 2e63 6f6e 7461 696e  pervisor.contain
-00001c40: 6572 2e67 742e 3030 3022 3a20 2250 656e  er.gt.000": "Pen
-00001c50: 6469 6e67 222c 0a20 2020 2020 2020 2022  ding",.        "
-00001c60: 7461 6465 6564 2e73 7065 6373 2e68 6163  tadeed.specs.hac
-00001c70: 6b2e 3030 3022 3a20 2250 656e 6469 6e67  k.000": "Pending
-00001c80: 222c 0a20 2020 2020 2020 2022 7461 7661  ",.        "tava
-00001c90: 6c69 6461 746f 7263 6572 742e 616c 676f  lidatorcert.algo
-00001ca0: 2e63 7265 6174 652e 3030 3022 3a20 2241  .create.000": "A
-00001cb0: 6374 6976 6522 2c0a 2020 2020 2020 2020  ctive",.        
-00001cc0: 2274 6176 616c 6964 6174 6f72 6365 7274  "tavalidatorcert
-00001cd0: 2e61 6c67 6f2e 7472 616e 7366 6572 2e30  .algo.transfer.0
-00001ce0: 3030 223a 2022 4163 7469 7665 222c 0a20  00": "Active",. 
-00001cf0: 2020 2020 2020 2022 7465 726d 696e 616c         "terminal
-00001d00: 6173 7365 742e 6365 7274 6966 792e 6861  asset.certify.ha
-00001d10: 636b 2e30 3030 223a 2022 5065 6e64 696e  ck.000": "Pendin
-00001d20: 6722 2c0a 2020 2020 7d0a 0a20 2020 2072  g",.    }..    r
-00001d30: 6574 7572 6e20 760a                      eturn v.
+00000000: 7b0a 2020 226e 616d 6522 3a20 2254 6144  {.  "name": "TaD
+00000010: 6165 6d6f 6e50 7974 686f 6e22 2c0a 2020  aemonPython",.  
+00000020: 2274 7970 6573 223a 205b 0a20 2020 207b  "types": [.    {
+00000030: 0a20 2020 2020 2022 6e61 6d65 223a 2022  .      "name": "
+00000040: 7369 676e 616e 6473 7562 6d69 742e 6d74  signandsubmit.mt
+00000050: 782e 616c 676f 2e30 3030 222c 0a20 2020  x.algo.000",.   
+00000060: 2020 2022 6174 7472 6962 7574 6573 223a     "attributes":
+00000070: 205b 0a20 2020 2020 2020 207b 0a20 2020   [.        {.   
+00000080: 2020 2020 2020 2022 7479 7065 223a 2022         "type": "
+00000090: 7374 7269 6e67 222c 0a20 2020 2020 2020  string",.       
+000000a0: 2020 2022 6e61 6d65 223a 2022 5479 7065     "name": "Type
+000000b0: 4e61 6d65 222c 0a20 2020 2020 2020 2020  Name",.         
+000000c0: 2022 6465 7363 223a 2022 5468 6520 5479   "desc": "The Ty
+000000d0: 7065 4e61 6d65 206f 6620 7468 6973 2074  peName of this t
+000000e0: 7970 652e 220a 2020 2020 2020 2020 7d2c  ype.".        },
+000000f0: 0a20 2020 2020 2020 207b 0a20 2020 2020  .        {.     
+00000100: 2020 2020 2022 7479 7065 223a 2022 7374       "type": "st
+00000110: 7269 6e67 222c 0a20 2020 2020 2020 2020  ring",.         
+00000120: 2022 6e61 6d65 223a 2022 5369 676e 6572   "name": "Signer
+00000130: 4164 6472 6573 7322 2c0a 2020 2020 2020  Address",.      
+00000140: 2020 2020 2264 6573 6322 3a20 2254 6865      "desc": "The
+00000150: 2070 7562 6c69 6320 6164 6472 6573 7320   public address 
+00000160: 666f 7220 7468 6520 6465 7369 7265 6420  for the desired 
+00000170: 6669 6e61 6c20 7369 676e 6572 2e22 0a20  final signer.". 
+00000180: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+00000190: 2020 7b0a 2020 2020 2020 2020 2020 2274    {.          "t
+000001a0: 7970 6522 3a20 2269 6e74 222c 0a20 2020  ype": "int",.   
+000001b0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000001c0: 5468 7265 7368 6f6c 6422 2c0a 2020 2020  Threshold",.    
+000001d0: 2020 2020 2020 2264 6573 6322 3a20 2254        "desc": "T
+000001e0: 6865 2074 6872 6573 686f 6c64 2066 6f72  he threshold for
+000001f0: 2074 6865 204d 756c 7469 7369 672e 220a   the Multisig.".
+00000200: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000210: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000220: 7479 7065 223a 2022 6c69 7374 5b73 7472  type": "list[str
+00000230: 696e 675d 222c 0a20 2020 2020 2020 2020  ing]",.         
+00000240: 2022 6e61 6d65 223a 2022 4164 6472 6573   "name": "Addres
+00000250: 7365 7322 2c0a 2020 2020 2020 2020 2020  ses",.          
+00000260: 2264 6573 6322 3a20 2254 6865 206f 7264  "desc": "The ord
+00000270: 6572 6564 206c 6973 7420 6f66 2061 6464  ered list of add
+00000280: 7265 7373 6573 2066 6f72 2074 6865 204d  resses for the M
+00000290: 756c 7469 7369 672e 220a 2020 2020 2020  ultisig.".      
+000002a0: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+000002b0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000002c0: 2022 7374 7269 6e67 222c 0a20 2020 2020   "string",.     
+000002d0: 2020 2020 2022 6e61 6d65 223a 2022 4d74       "name": "Mt
+000002e0: 7822 2c0a 2020 2020 2020 2020 2020 2264  x",.          "d
+000002f0: 6573 6322 3a20 2254 6865 2065 6e63 6f64  esc": "The encod
+00000300: 6564 2c20 7061 7274 6961 6c6c 7920 7369  ed, partially si
+00000310: 676e 6564 204d 756c 7469 7369 6754 7261  gned MultisigTra
+00000320: 6e73 6163 7469 6f6e 2e22 0a20 2020 2020  nsaction.".     
+00000330: 2020 207d 0a20 2020 2020 205d 2c0a 2020     }.      ],.  
+00000340: 2020 2020 2261 7869 6f6d 7322 3a20 5b0a      "axioms": [.
+00000350: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000360: 2020 2020 226e 616d 6522 3a20 2243 6f72      "name": "Cor
+00000370: 7265 6374 2054 7970 654e 616d 6522 2c0a  rect TypeName",.
+00000380: 2020 2020 2020 2020 2020 226e 756d 6265            "numbe
+00000390: 7222 3a20 312c 0a20 2020 2020 2020 2020  r": 1,.         
+000003a0: 2022 6465 7363 223a 2022 5479 7065 4e61   "desc": "TypeNa
+000003b0: 6d65 206d 7573 7420 6265 2073 6967 6e61  me must be signa
+000003c0: 6e64 7375 626d 6974 2e6d 7478 2e61 6c67  ndsubmit.mtx.alg
+000003d0: 6f2e 3030 3022 0a20 2020 2020 2020 207d  o.000".        }
+000003e0: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+000003f0: 2020 2020 2020 226e 616d 6522 3a20 2242        "name": "B
+00000400: 6173 6963 2074 7970 696e 6722 2c0a 2020  asic typing",.  
+00000410: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
+00000420: 3a20 322c 0a20 2020 2020 2020 2020 2022  : 2,.          "
+00000430: 6465 7363 223a 2022 5369 676e 6572 4164  desc": "SignerAd
+00000440: 6472 6573 7320 6973 2073 7472 696e 672c  dress is string,
+00000450: 204d 7478 2069 7320 6120 7374 7269 6e67   Mtx is a string
+00000460: 2c20 4164 6472 6573 7365 7320 6973 2061  , Addresses is a
+00000470: 206c 6973 7420 6f66 2073 7472 696e 6773   list of strings
+00000480: 2c20 5468 7265 7368 6f6c 6420 6973 2061  , Threshold is a
+00000490: 6e20 696e 742e 220a 2020 2020 2020 2020  n int.".        
+000004a0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+000004b0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+000004c0: 4261 7369 6320 666f 726d 6174 7469 6e67  Basic formatting
+000004d0: 222c 0a20 2020 2020 2020 2020 2022 6e75  ",.          "nu
+000004e0: 6d62 6572 223a 2033 2c0a 2020 2020 2020  mber": 3,.      
+000004f0: 2020 2020 2264 6573 6322 3a20 2253 6967      "desc": "Sig
+00000500: 6e65 7241 6464 7265 7373 2068 6173 2041  nerAddress has A
+00000510: 6c67 6f41 6464 7265 7373 5374 7269 6e67  lgoAddressString
+00000520: 2066 6f72 6d61 742c 204d 7478 2068 6173   format, Mtx has
+00000530: 2041 6c67 6f4d 7367 5061 636b 456e 636f   AlgoMsgPackEnco
+00000540: 6465 6420 666f 726d 6174 2c20 656c 7473  ded format, elts
+00000550: 206f 6620 4164 6472 6573 7365 7320 6861   of Addresses ha
+00000560: 7665 2041 6c67 6f41 6464 7265 7373 5374  ve AlgoAddressSt
+00000570: 7269 6e67 2066 6f72 6d61 742e 220a 2020  ring format.".  
+00000580: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
+00000590: 207b 0a20 2020 2020 2020 2020 2022 6e61   {.          "na
+000005a0: 6d65 223a 2022 4d74 7820 6973 204d 756c  me": "Mtx is Mul
+000005b0: 7469 7369 6754 7261 6e73 6163 7469 6f6e  tisigTransaction
+000005c0: 222c 0a20 2020 2020 2020 2020 2022 6e75  ",.          "nu
+000005d0: 6d62 6572 223a 2034 2c0a 2020 2020 2020  mber": 4,.      
+000005e0: 2020 2020 2264 6573 6322 3a20 224f 6e63      "desc": "Onc
+000005f0: 6520 6465 636f 6465 642c 204d 7478 2069  e decoded, Mtx i
+00000600: 7320 6120 4d75 6c74 6973 6967 5472 616e  s a MultisigTran
+00000610: 7361 6374 696f 6e22 0a20 2020 2020 2020  saction".       
+00000620: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00000630: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00000640: 2249 6e74 6572 6e61 6c20 636f 6e73 6973  "Internal consis
+00000650: 7465 6e63 7922 2c0a 2020 2020 2020 2020  tency",.        
+00000660: 2020 226e 756d 6265 7222 3a20 352c 0a20    "number": 5,. 
+00000670: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+00000680: 2022 5369 676e 6572 4164 6472 6573 7320   "SignerAddress 
+00000690: 6973 206f 6e65 206f 6620 7468 6520 4164  is one of the Ad
+000006a0: 6472 6573 7365 732e 5c6e 5468 7265 7368  dresses.\nThresh
+000006b0: 6f6c 6420 6973 2074 6865 2074 6872 6573  old is the thres
+000006c0: 686f 6c64 2066 6f72 2074 6865 204d 756c  hold for the Mul
+000006d0: 7469 7369 6754 7261 6e73 6163 7469 6f6e  tisigTransaction
+000006e0: 2e5c 6e41 6464 7265 7373 6573 2061 7265  .\nAddresses are
+000006f0: 2074 6865 206c 6973 7420 6f66 2061 6464   the list of add
+00000700: 7265 7373 6573 2066 6f72 2074 6865 204d  resses for the M
+00000710: 756c 7469 7369 6754 7261 6e73 6163 7469  ultisigTransacti
+00000720: 6f6e 2028 6f72 6465 7220 6d61 7474 6572  on (order matter
+00000730: 7329 2e22 0a20 2020 2020 2020 207d 2c0a  s).".        },.
+00000740: 2020 2020 2020 2020 7b0a 2020 2020 2020          {.      
+00000750: 2020 2020 226e 616d 6522 3a20 224d 7478      "name": "Mtx
+00000760: 2074 6872 6573 686f 6c64 2067 6574 7320   threshold gets 
+00000770: 6d65 7422 2c0a 2020 2020 2020 2020 2020  met",.          
+00000780: 226e 756d 6265 7222 3a20 362c 0a20 2020  "number": 6,.   
+00000790: 2020 2020 2020 2022 6465 7363 223a 2022         "desc": "
+000007a0: 4f6e 6365 2074 6865 2053 6967 6e65 7241  Once the SignerA
+000007b0: 6464 7265 7373 2073 6967 6e73 2c20 7468  ddress signs, th
+000007c0: 6520 4d74 7820 6d65 6574 7320 6974 7320  e Mtx meets its 
+000007d0: 7468 7265 7368 6f6c 6420 6f66 2073 6967  threshold of sig
+000007e0: 6e61 7475 7265 732e 220a 2020 2020 2020  natures.".      
+000007f0: 2020 7d0a 2020 2020 2020 5d2c 0a20 2020    }.      ],.   
+00000800: 2020 2022 6465 7363 223a 2022 4d65 616e     "desc": "Mean
+00000810: 7420 666f 7220 6f6e 6520 6163 636f 756e  t for one accoun
+00000820: 7420 6f66 2061 204d 756c 7469 7369 6741  t of a MultisigA
+00000830: 6363 6f75 6e74 2074 6f20 7365 6e64 2074  ccount to send t
+00000840: 6f20 616e 6f74 6865 7220 6163 636f 756e  o another accoun
+00000850: 7420 696e 2074 6861 7420 4d75 6c74 6973  t in that Multis
+00000860: 6967 4163 636f 756e 7420 666f 7220 636f  igAccount for co
+00000870: 2d73 6967 6e69 6e67 2e22 0a20 2020 207d  -signing.".    }
+00000880: 2c0a 2020 2020 7b0a 2020 2020 2020 226e  ,.    {.      "n
+00000890: 616d 6522 3a20 226f 7074 696e 2e74 6164  ame": "optin.tad
+000008a0: 6565 642e 616c 676f 2e30 3031 222c 0a20  eed.algo.001",. 
+000008b0: 2020 2020 2022 6174 7472 6962 7574 6573       "attributes
+000008c0: 223a 205b 0a20 2020 2020 2020 207b 0a20  ": [.        {. 
+000008d0: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+000008e0: 2022 7374 7269 6e67 222c 0a20 2020 2020   "string",.     
+000008f0: 2020 2020 2022 6e61 6d65 223a 2022 5479       "name": "Ty
+00000900: 7065 4e61 6d65 222c 0a20 2020 2020 2020  peName",.       
+00000910: 2020 2022 6465 7363 223a 2022 5468 6520     "desc": "The 
+00000920: 7479 7065 5f6e 616d 6520 6f66 2074 6869  type_name of thi
+00000930: 7320 7479 7065 2e22 0a20 2020 2020 2020  s type.".       
+00000940: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00000950: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00000960: 2273 7472 696e 6722 2c0a 2020 2020 2020  "string",.      
+00000970: 2020 2020 226e 616d 6522 3a20 2254 6144      "name": "TaD
+00000980: 6165 6d6f 6e41 6464 7222 2c0a 2020 2020  aemonAddr",.    
+00000990: 2020 2020 2020 2264 6573 6322 3a20 2254        "desc": "T
+000009a0: 6865 2070 7562 6c69 6320 6164 6472 6573  he public addres
+000009b0: 7320 6f66 2074 6865 2054 6144 6165 6d6f  s of the TaDaemo
+000009c0: 6e27 7320 616c 676f 2061 6363 6f75 6e74  n's algo account
+000009d0: 2e22 0a20 2020 2020 2020 207d 2c0a 2020  .".        },.  
+000009e0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000009f0: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00000a00: 6722 2c0a 2020 2020 2020 2020 2020 226e  g",.          "n
+00000a10: 616d 6522 3a20 2254 614f 776e 6572 4164  ame": "TaOwnerAd
+00000a20: 6472 222c 0a20 2020 2020 2020 2020 2022  dr",.          "
+00000a30: 6465 7363 223a 2022 5468 6520 7075 626c  desc": "The publ
+00000a40: 6963 2061 6464 7265 7373 206f 6620 7468  ic address of th
+00000a50: 6520 5461 4f77 6e65 7220 6163 636f 756e  e TaOwner accoun
+00000a60: 742e 220a 2020 2020 2020 2020 7d2c 0a20  t.".        },. 
+00000a70: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+00000a80: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+00000a90: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
+00000aa0: 6e61 6d65 223a 2022 5661 6c69 6461 746f  name": "Validato
+00000ab0: 7241 6464 7222 2c0a 2020 2020 2020 2020  rAddr",.        
+00000ac0: 2020 2264 6573 6322 3a20 2254 6865 2070    "desc": "The p
+00000ad0: 7562 6c69 6320 6164 6472 6573 7320 6f66  ublic address of
+00000ae0: 2061 6363 6f75 6e74 2066 6f72 2074 6865   account for the
+00000af0: 2056 616c 6964 6174 6f72 2066 6f72 2074   Validator for t
+00000b00: 6869 7320 5461 4465 6564 2e22 0a20 2020  his TaDeed.".   
+00000b10: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000b20: 7b0a 2020 2020 2020 2020 2020 2274 7970  {.          "typ
+00000b30: 6522 3a20 2273 7472 696e 6722 2c0a 2020  e": "string",.  
+00000b40: 2020 2020 2020 2020 226e 616d 6522 3a20          "name": 
+00000b50: 224e 6577 4465 6564 4f70 7449 6e4d 7478  "NewDeedOptInMtx
+00000b60: 222c 0a20 2020 2020 2020 2020 2022 6465  ",.          "de
+00000b70: 7363 223a 2022 4f70 7449 6e20 4d75 6c74  sc": "OptIn Mult
+00000b80: 6973 6967 5472 616e 7361 6374 696f 6e20  isigTransaction 
+00000b90: 666f 7220 7468 6520 6e65 7720 5461 4465  for the new TaDe
+00000ba0: 6564 204e 4654 2e22 0a20 2020 2020 2020  ed NFT.".       
+00000bb0: 207d 0a20 2020 2020 205d 2c0a 2020 2020   }.      ],.    
+00000bc0: 2020 2261 7869 6f6d 7322 3a20 5b0a 2020    "axioms": [.  
+00000bd0: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000be0: 2020 226e 616d 6522 3a20 2243 6f72 7265    "name": "Corre
+00000bf0: 6374 2054 7970 654e 616d 6522 2c0a 2020  ct TypeName",.  
+00000c00: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
+00000c10: 3a20 312c 0a20 2020 2020 2020 2020 2022  : 1,.          "
+00000c20: 6465 7363 223a 2022 5479 7065 4e61 6d65  desc": "TypeName
+00000c30: 206d 7573 7420 6265 206f 7074 696e 2e74   must be optin.t
+00000c40: 6164 6565 642e 616c 676f 2e30 3031 220a  adeed.algo.001".
+00000c50: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000c60: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000c70: 6e61 6d65 223a 2022 4261 7369 6320 7479  name": "Basic ty
+00000c80: 7069 6e67 222c 0a20 2020 2020 2020 2020  ping",.         
+00000c90: 2022 6e75 6d62 6572 223a 2032 2c0a 2020   "number": 2,.  
+00000ca0: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
+00000cb0: 2254 6144 6165 6d6f 6e41 6464 7220 6973  "TaDaemonAddr is
+00000cc0: 2061 2073 7472 696e 672c 2054 614f 776e   a string, TaOwn
+00000cd0: 6572 4164 6472 2069 7320 6120 7374 7269  erAddr is a stri
+00000ce0: 6e67 2c20 5661 6c69 6461 746f 7241 6464  ng, ValidatorAdd
+00000cf0: 7220 6973 2061 2073 7472 696e 672c 204e  r is a string, N
+00000d00: 6577 4465 6564 4f70 7449 6e4d 7478 2069  ewDeedOptInMtx i
+00000d10: 7320 6120 7374 7269 6e67 2e22 0a20 2020  s a string.".   
+00000d20: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000d30: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+00000d40: 6522 3a20 2242 6173 6963 2066 6f72 6d61  e": "Basic forma
+00000d50: 7474 696e 6722 2c0a 2020 2020 2020 2020  tting",.        
+00000d60: 2020 226e 756d 6265 7222 3a20 332c 0a20    "number": 3,. 
+00000d70: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+00000d80: 2022 5461 4461 656d 6f6e 4164 6472 2068   "TaDaemonAddr h
+00000d90: 6173 2041 6c67 6f41 6464 7265 7373 5374  as AlgoAddressSt
+00000da0: 7269 6e67 2066 6f72 6d61 742c 2054 614f  ring format, TaO
+00000db0: 776e 6572 4164 6472 2068 6173 2041 6c67  wnerAddr has Alg
+00000dc0: 6f41 6464 7265 7373 5374 7269 6e67 2066  oAddressString f
+00000dd0: 6f72 6d61 742c 2056 616c 6964 6174 6f72  ormat, Validator
+00000de0: 4164 6472 2068 6173 2041 6c67 6f41 6464  Addr has AlgoAdd
+00000df0: 7265 7373 5374 7269 6e67 2066 6f72 6d61  ressString forma
+00000e00: 742c 204e 6577 4465 6564 4f70 7449 6e4d  t, NewDeedOptInM
+00000e10: 7478 2068 6173 2041 6c67 6f4d 7367 5061  tx has AlgoMsgPa
+00000e20: 636b 456e 636f 6465 6420 666f 726d 6174  ckEncoded format
+00000e30: 2e22 0a20 2020 2020 2020 207d 2c0a 2020  .".        },.  
+00000e40: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00000e50: 2020 226e 616d 6522 3a20 224e 6577 4465    "name": "NewDe
+00000e60: 6564 4f70 7449 6e4d 7478 206d 7573 7420  edOptInMtx must 
+00000e70: 6265 204d 756c 7469 7369 6754 7261 6e73  be MultisigTrans
+00000e80: 6163 7469 6f6e 222c 0a20 2020 2020 2020  action",.       
+00000e90: 2020 2022 6e75 6d62 6572 223a 2034 2c0a     "number": 4,.
+00000ea0: 2020 2020 2020 2020 2020 2264 6573 6322            "desc"
+00000eb0: 3a20 224f 6e63 6520 6465 636f 6465 642c  : "Once decoded,
+00000ec0: 204e 6577 4465 6564 4f70 7449 6e4d 7478   NewDeedOptInMtx
+00000ed0: 206d 7573 7420 6265 2061 204d 756c 7469   must be a Multi
+00000ee0: 7369 6754 7261 6e73 6163 7469 6f6e 220a  sigTransaction".
+00000ef0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00000f00: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00000f10: 6e61 6d65 223a 2022 4e65 7744 6565 644f  name": "NewDeedO
+00000f20: 7074 696e 4d74 7820 7478 6e20 7479 7065  ptinMtx txn type
+00000f30: 2063 6865 636b 222c 0a20 2020 2020 2020   check",.       
+00000f40: 2020 2022 6e75 6d62 6572 223a 2035 2c0a     "number": 5,.
+00000f50: 2020 2020 2020 2020 2020 2264 6573 6322            "desc"
+00000f60: 3a20 224e 6577 4465 6564 4f70 7469 6e4d  : "NewDeedOptinM
+00000f70: 7478 2074 7261 6e73 6163 7469 6f6e 206d  tx transaction m
+00000f80: 7573 7420 6265 2061 6e20 4f70 7449 6e20  ust be an OptIn 
+00000f90: 5472 616e 7361 6374 696f 6e22 0a20 2020  Transaction".   
+00000fa0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00000fb0: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+00000fc0: 6522 3a20 2254 786e 2063 6f6e 7369 7374  e": "Txn consist
+00000fd0: 656e 6379 2063 6865 636b 222c 0a20 2020  ency check",.   
+00000fe0: 2020 2020 2020 2022 6e75 6d62 6572 223a         "number":
+00000ff0: 2036 2c0a 2020 2020 2020 2020 2020 2264   6,.          "d
+00001000: 6573 6322 3a20 2254 786e 2073 656e 6465  esc": "Txn sende
+00001010: 7220 6973 2054 614d 756c 7469 2c20 4f70  r is TaMulti, Op
+00001020: 7449 6e20 6173 7365 7420 6973 2061 206e  tIn asset is a n
+00001030: 6577 2054 6144 6565 6420 6372 6561 7465  ew TaDeed create
+00001040: 6420 616e 6420 6f77 6e65 6420 6279 2047  d and owned by G
+00001050: 6e66 4164 6d69 6e41 6363 6f75 6e74 220a  nfAdminAccount".
+00001060: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001070: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00001080: 6e61 6d65 223a 2022 4f6c 6420 5461 4465  name": "Old TaDe
+00001090: 6564 2063 6865 636b 222c 0a20 2020 2020  ed check",.     
+000010a0: 2020 2020 2022 6e75 6d62 6572 223a 2037       "number": 7
+000010b0: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+000010c0: 6322 3a20 2254 614d 756c 7469 2032 2d73  c": "TaMulti 2-s
+000010d0: 6967 205b 476e 6641 646d 696e 4163 636f  ig [GnfAdminAcco
+000010e0: 756e 742c 2054 6144 6165 6d6f 6e41 6464  unt, TaDaemonAdd
+000010f0: 722c 5c6e 5461 4f77 6e65 7241 6464 725d  r,\nTaOwnerAddr]
+00001100: 206f 776e 7320 6578 6163 746c 7920 3120   owns exactly 1 
+00001110: 5461 4465 6564 2e20 5468 6520 6372 6561  TaDeed. The crea
+00001120: 746f 7220 6f66 2074 6865 206f 6c64 2054  tor of the old T
+00001130: 6144 6565 6420 6973 2065 6974 6865 7220  aDeed is either 
+00001140: 7468 6520 476e 6641 646d 696e 4163 636f  the GnfAdminAcco
+00001150: 756e 7420 6f72 2074 6865 2056 616c 6964  unt or the Valid
+00001160: 6174 6f72 4d75 6c74 6920 322d 7369 6720  atorMulti 2-sig 
+00001170: 5b47 6e66 4164 6d69 6e41 6363 6f75 6e74  [GnfAdminAccount
+00001180: 2c20 5661 6c69 6461 746f 7241 6464 725d  , ValidatorAddr]
+00001190: 2e20 5468 6520 6173 7365 7420 696e 6465  . The asset inde
+000011a0: 7820 6f66 2074 6865 206f 6c64 2054 6144  x of the old TaD
+000011b0: 6565 6420 6973 5c6e 6c65 7373 2074 6861  eed is\nless tha
+000011c0: 6e20 7468 6520 6173 7365 7420 696e 6465  n the asset inde
+000011d0: 7820 6f66 2074 6865 206e 6577 2054 6144  x of the new TaD
+000011e0: 6565 642e 2046 696e 616c 6c79 2c20 6966  eed. Finally, if
+000011f0: 2074 6865 2063 7265 6174 6f72 206f 6620   the creator of 
+00001200: 7468 6520 6f6c 6420 5461 4465 6564 2069  the old TaDeed i
+00001210: 7320 7468 655c 6e47 6e66 4164 6d69 6e41  s the\nGnfAdminA
+00001220: 6363 6f75 6e74 2c20 7468 656e 2074 6865  ccount, then the
+00001230: 2054 614d 756c 7469 2069 7320 6f70 7465   TaMulti is opte
+00001240: 6420 696e 746f 2028 6275 7420 646f 6573  d into (but does
+00001250: 206e 6f74 206f 776e 2920 6578 6163 746c   not own) exactl
+00001260: 7920 6f6e 6520 5461 4465 6564 2063 7265  y one TaDeed cre
+00001270: 6174 6564 2062 7920 7468 655c 6e56 616c  ated by the\nVal
+00001280: 6964 6174 6f72 4d75 6c74 6920 6163 636f  idatorMulti acco
+00001290: 756e 7420 616e 6420 6f77 6e65 6420 6279  unt and owned by
+000012a0: 2074 6865 2047 6e66 4164 6d69 6e41 6363   the GnfAdminAcc
+000012b0: 6f75 6e74 2e22 0a20 2020 2020 2020 207d  ount.".        }
+000012c0: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+000012d0: 2020 2020 2020 226e 616d 6522 3a20 2243        "name": "C
+000012e0: 6f72 7265 6374 6c79 2073 6967 6e65 6422  orrectly signed"
+000012f0: 2c0a 2020 2020 2020 2020 2020 226e 756d  ,.          "num
+00001300: 6265 7222 3a20 382c 0a20 2020 2020 2020  ber": 8,.       
+00001310: 2020 2022 6465 7363 223a 2022 4e65 7744     "desc": "NewD
+00001320: 6565 644f 7074 496e 4d74 7820 6d75 7374  eedOptInMtx must
+00001330: 2062 6520 7369 676e 6564 2062 7920 476e   be signed by Gn
+00001340: 6620 4164 6d69 6e2c 2061 6e64 2074 6865  f Admin, and the
+00001350: 2073 6967 6e61 7475 7265 206d 7573 7420   signature must 
+00001360: 6d61 7463 6820 7468 6520 7478 6e2e 220a  match the txn.".
+00001370: 2020 2020 2020 2020 7d0a 2020 2020 2020          }.      
+00001380: 5d2c 0a20 2020 2020 2022 6465 7363 223a  ],.      "desc":
+00001390: 2022 4d65 7373 6167 6520 6672 6f6d 2047   "Message from G
+000013a0: 4e6f 6465 4661 6374 6f72 7920 746f 2050  NodeFactory to P
+000013b0: 7974 686f 6e54 6144 6165 6d6f 6e20 666f  ythonTaDaemon fo
+000013c0: 7220 5461 4d75 6c74 6920 6163 6374 2028  r TaMulti acct (
+000013d0: 322d 7369 6720 5b47 6e66 4164 6d69 6e2c  2-sig [GnfAdmin,
+000013e0: 2054 6144 6165 6d6f 6e2c 2054 614f 776e   TaDaemon, TaOwn
+000013f0: 6572 5d29 206f 7074 696e 6720 696e 746f  er]) opting into
+00001400: 206e 6577 2054 6144 6565 642e 220a 2020   new TaDeed.".  
+00001410: 2020 7d2c 0a20 2020 207b 0a20 2020 2020    },.    {.     
+00001420: 2022 6e61 6d65 223a 2022 6578 6368 616e   "name": "exchan
+00001430: 6765 2e74 6164 6565 642e 616c 676f 2e30  ge.tadeed.algo.0
+00001440: 3130 222c 0a20 2020 2020 2022 6174 7472  10",.      "attr
+00001450: 6962 7574 6573 223a 205b 0a20 2020 2020  ibutes": [.     
+00001460: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00001470: 7479 7065 223a 2022 7374 7269 6e67 222c  type": "string",
+00001480: 0a20 2020 2020 2020 2020 2022 6e61 6d65  .          "name
+00001490: 223a 2022 5479 7065 4e61 6d65 222c 0a20  ": "TypeName",. 
+000014a0: 2020 2020 2020 2020 2022 6465 7363 223a           "desc":
+000014b0: 2022 5468 6520 7479 7065 5f6e 616d 6520   "The type_name 
+000014c0: 6f66 2074 6869 7320 7479 7065 2e22 0a20  of this type.". 
+000014d0: 2020 2020 2020 207d 2c0a 2020 2020 2020         },.      
+000014e0: 2020 7b0a 2020 2020 2020 2020 2020 2274    {.          "t
+000014f0: 7970 6522 3a20 2273 7472 696e 6722 2c0a  ype": "string",.
+00001500: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00001510: 3a20 2254 6144 6165 6d6f 6e41 6464 7222  : "TaDaemonAddr"
+00001520: 2c0a 2020 2020 2020 2020 2020 2264 6573  ,.          "des
+00001530: 6322 3a20 2254 6865 2070 7562 6c69 6320  c": "The public 
+00001540: 6164 6472 6573 7320 6f66 2074 6865 2054  address of the T
+00001550: 6144 6165 6d6f 6e27 7320 616c 676f 2061  aDaemon's algo a
+00001560: 6363 6f75 6e74 2e22 0a20 2020 2020 2020  ccount.".       
+00001570: 207d 2c0a 2020 2020 2020 2020 7b0a 2020   },.        {.  
+00001580: 2020 2020 2020 2020 2274 7970 6522 3a20          "type": 
+00001590: 2273 7472 696e 6722 2c0a 2020 2020 2020  "string",.      
+000015a0: 2020 2020 226e 616d 6522 3a20 2254 614f      "name": "TaO
+000015b0: 776e 6572 4164 6472 222c 0a20 2020 2020  wnerAddr",.     
+000015c0: 2020 2020 2022 6465 7363 223a 2022 5468       "desc": "Th
+000015d0: 6520 7075 626c 6963 2061 6464 7265 7373  e public address
+000015e0: 206f 6620 7468 6520 5461 4f77 6e65 7220   of the TaOwner 
+000015f0: 6163 636f 756e 742e 220a 2020 2020 2020  account.".      
+00001600: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00001610: 2020 2020 2020 2020 2022 7479 7065 223a           "type":
+00001620: 2022 7374 7269 6e67 222c 0a20 2020 2020   "string",.     
+00001630: 2020 2020 2022 6e61 6d65 223a 2022 5661       "name": "Va
+00001640: 6c69 6461 746f 7241 6464 7222 2c0a 2020  lidatorAddr",.  
+00001650: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
+00001660: 2254 6865 2070 7562 6c69 6320 6164 6472  "The public addr
+00001670: 6573 7320 6f66 2061 6363 6f75 6e74 2066  ess of account f
+00001680: 6f72 2074 6865 6520 5661 6c69 6461 746f  or thee Validato
+00001690: 7220 666f 7220 7468 6973 2054 6144 6565  r for this TaDee
+000016a0: 642e 220a 2020 2020 2020 2020 7d2c 0a20  d.".        },. 
+000016b0: 2020 2020 2020 207b 0a20 2020 2020 2020         {.       
+000016c0: 2020 2022 7479 7065 223a 2022 7374 7269     "type": "stri
+000016d0: 6e67 222c 0a20 2020 2020 2020 2020 2022  ng",.          "
+000016e0: 6e61 6d65 223a 2022 4e65 7754 6144 6565  name": "NewTaDee
+000016f0: 6449 6478 222c 0a20 2020 2020 2020 2020  dIdx",.         
+00001700: 2022 6465 7363 223a 2022 5468 6520 6173   "desc": "The as
+00001710: 7365 7420 696e 6465 7820 666f 7220 7468  set index for th
+00001720: 6520 6e65 7720 5461 4465 6564 204e 4654  e new TaDeed NFT
+00001730: 2e22 0a20 2020 2020 2020 207d 2c0a 2020  .".        },.  
+00001740: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+00001750: 2020 2274 7970 6522 3a20 2273 7472 696e    "type": "strin
+00001760: 6722 2c0a 2020 2020 2020 2020 2020 226e  g",.          "n
+00001770: 616d 6522 3a20 224f 6c64 4465 6564 5472  ame": "OldDeedTr
+00001780: 616e 7366 6572 4d74 7822 2c0a 2020 2020  ansferMtx",.    
+00001790: 2020 2020 2020 2264 6573 6322 3a20 2254        "desc": "T
+000017a0: 6865 2065 6e63 6f64 6564 204d 756c 7469  he encoded Multi
+000017b0: 7369 6754 7261 6e73 6163 7469 6f6e 2074  sigTransaction t
+000017c0: 6861 7420 6361 6e20 7472 616e 7366 6572  hat can transfer
+000017d0: 2074 6865 206f 6c64 2054 6144 6565 6420   the old TaDeed 
+000017e0: 6672 6f6d 2074 6865 2054 614d 756c 7469  from the TaMulti
+000017f0: 2062 6163 6b20 746f 2074 6865 2047 6e66   back to the Gnf
+00001800: 2e22 0a20 2020 2020 2020 207d 0a20 2020  .".        }.   
+00001810: 2020 205d 2c0a 2020 2020 2020 2261 7869     ],.      "axi
+00001820: 6f6d 7322 3a20 5b0a 2020 2020 2020 2020  oms": [.        
+00001830: 7b0a 2020 2020 2020 2020 2020 226e 616d  {.          "nam
+00001840: 6522 3a20 2270 6179 6c6f 6164 2069 6e20  e": "payload in 
+00001850: 6170 6922 2c0a 2020 2020 2020 2020 2020  api",.          
+00001860: 226e 756d 6265 7222 3a20 312c 0a20 2020  "number": 1,.   
+00001870: 2020 2020 2020 2022 6465 7363 223a 2022         "desc": "
+00001880: 4d65 7373 6167 6554 7970 6520 6d75 7374  MessageType must
+00001890: 2062 6520 6f6e 6520 6f66 2074 6865 2054   be one of the T
+000018a0: 7970 654e 616d 6573 2069 6e20 7468 6973  ypeNames in this
+000018b0: 2041 5049 2022 0a20 2020 2020 2020 207d   API ".        }
+000018c0: 2c0a 2020 2020 2020 2020 7b0a 2020 2020  ,.        {.    
+000018d0: 2020 2020 2020 226e 616d 6522 3a20 2242        "name": "B
+000018e0: 6173 6963 2074 7970 696e 6722 2c0a 2020  asic typing",.  
+000018f0: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
+00001900: 3a20 322c 0a20 2020 2020 2020 2020 2022  : 2,.          "
+00001910: 6465 7363 223a 2022 5461 4461 656d 6f6e  desc": "TaDaemon
+00001920: 4164 6472 2069 7320 6120 7374 7269 6e67  Addr is a string
+00001930: 2c20 5461 4f77 6e65 7241 6464 7220 6973  , TaOwnerAddr is
+00001940: 2061 2073 7472 696e 672c 2056 616c 6964   a string, Valid
+00001950: 6174 6f72 4164 6472 2069 7320 6120 7374  atorAddr is a st
+00001960: 7269 6e67 2c20 4e65 7744 6565 644f 7074  ring, NewDeedOpt
+00001970: 496e 4d74 7820 6973 2061 2073 7472 696e  InMtx is a strin
+00001980: 6722 0a20 2020 2020 2020 207d 2c0a 2020  g".        },.  
+00001990: 2020 2020 2020 7b0a 2020 2020 2020 2020        {.        
+000019a0: 2020 226e 616d 6522 3a20 2242 6173 6963    "name": "Basic
+000019b0: 2066 6f72 6d61 7474 696e 6722 2c0a 2020   formatting",.  
+000019c0: 2020 2020 2020 2020 226e 756d 6265 7222          "number"
+000019d0: 3a20 332c 0a20 2020 2020 2020 2020 2022  : 3,.          "
+000019e0: 6465 7363 223a 2022 5461 4461 656d 6f6e  desc": "TaDaemon
+000019f0: 4164 6472 2068 6173 2041 6c67 6f41 6464  Addr has AlgoAdd
+00001a00: 7265 7373 5374 7269 6e67 2066 6f72 6d61  ressString forma
+00001a10: 742c 2054 614f 776e 6572 4164 6472 2068  t, TaOwnerAddr h
+00001a20: 6173 2041 6c67 6f41 6464 7265 7373 5374  as AlgoAddressSt
+00001a30: 7269 6e67 2066 6f72 6d61 742c 2056 616c  ring format, Val
+00001a40: 6964 6174 6f72 4164 6472 2068 6173 2041  idatorAddr has A
+00001a50: 6c67 6f41 6464 7265 7373 5374 7269 6e67  lgoAddressString
+00001a60: 2066 6f72 6d61 742c 204e 6577 4465 6564   format, NewDeed
+00001a70: 4f70 7449 6e4d 7478 2068 6173 2041 6c67  OptInMtx has Alg
+00001a80: 6f4d 7367 5061 636b 456e 636f 6465 6420  oMsgPackEncoded 
+00001a90: 666f 726d 6174 220a 2020 2020 2020 2020  format".        
+00001aa0: 7d2c 0a20 2020 2020 2020 207b 0a20 2020  },.        {.   
+00001ab0: 2020 2020 2020 2022 6e61 6d65 223a 2022         "name": "
+00001ac0: 4f6c 6444 6565 6454 7261 6e73 6665 724d  OldDeedTransferM
+00001ad0: 7478 206d 7573 7420 6265 204d 756c 7469  tx must be Multi
+00001ae0: 7369 6754 7261 6e73 6163 7469 6f6e 222c  sigTransaction",
+00001af0: 0a20 2020 2020 2020 2020 2022 6e75 6d62  .          "numb
+00001b00: 6572 223a 2034 2c0a 2020 2020 2020 2020  er": 4,.        
+00001b10: 2020 2264 6573 6322 3a20 224f 6e63 6520    "desc": "Once 
+00001b20: 6465 636f 6465 642c 204f 6c64 4465 6564  decoded, OldDeed
+00001b30: 5472 616e 7366 6572 4d74 7820 6d75 7374  TransferMtx must
+00001b40: 2062 6520 6120 4d75 6c74 6973 6967 5472   be a MultisigTr
+00001b50: 616e 7361 6374 696f 6e22 0a20 2020 2020  ansaction".     
+00001b60: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001b70: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00001b80: 3a20 224f 6c64 4465 6564 5472 616e 7366  : "OldDeedTransf
+00001b90: 6572 4d74 7820 7478 6e20 7479 7065 2063  erMtx txn type c
+00001ba0: 6865 636b 222c 0a20 2020 2020 2020 2020  heck",.         
+00001bb0: 2022 6e75 6d62 6572 223a 2035 2c0a 2020   "number": 5,.  
+00001bc0: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
+00001bd0: 224f 6c64 4465 6564 4f70 7469 6e4d 7478  "OldDeedOptinMtx
+00001be0: 2074 7261 6e73 6163 7469 6f6e 206d 7573   transaction mus
+00001bf0: 7420 6265 2061 6e20 4173 7365 7454 7261  t be an AssetTra
+00001c00: 6e73 6665 7254 786e 220a 2020 2020 2020  nsferTxn".      
+00001c10: 2020 7d2c 0a20 2020 2020 2020 207b 0a20    },.        {. 
+00001c20: 2020 2020 2020 2020 2022 6e61 6d65 223a           "name":
+00001c30: 2022 5478 6e20 636f 6e73 6973 7465 6e63   "Txn consistenc
+00001c40: 7920 6368 6563 6b22 2c0a 2020 2020 2020  y check",.      
+00001c50: 2020 2020 226e 756d 6265 7222 3a20 362c      "number": 6,
+00001c60: 0a20 2020 2020 2020 2020 2022 6465 7363  .          "desc
+00001c70: 223a 2022 546f 7461 6c20 6d75 7374 2062  ": "Total must b
+00001c80: 6520 312c 2073 656e 6465 7220 6d75 7374  e 1, sender must
+00001c90: 2062 6520 5461 4d75 6c74 692c 2072 6563   be TaMulti, rec
+00001ca0: 6569 7665 7220 6d75 7374 2062 6520 476e  eiver must be Gn
+00001cb0: 6641 646d 696e 2c20 6173 7365 7420 6d75  fAdmin, asset mu
+00001cc0: 7374 2062 6520 6120 5461 4465 6564 220a  st be a TaDeed".
+00001cd0: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
+00001ce0: 2020 207b 0a20 2020 2020 2020 2020 2022     {.          "
+00001cf0: 6e61 6d65 223a 2022 5461 4465 6564 206f  name": "TaDeed o
+00001d00: 7264 6572 222c 0a20 2020 2020 2020 2020  rder",.         
+00001d10: 2022 6e75 6d62 6572 223a 2037 2c0a 2020   "number": 7,.  
+00001d20: 2020 2020 2020 2020 2264 6573 6322 3a20          "desc": 
+00001d30: 2254 6865 2061 7373 6574 2069 6e64 6578  "The asset index
+00001d40: 206f 6620 7468 6520 6e65 7720 5461 4465   of the new TaDe
+00001d50: 6564 206d 7573 7420 6265 2067 7265 6174  ed must be great
+00001d60: 6572 2074 6861 6e20 7468 6520 6173 7365  er than the asse
+00001d70: 7420 696e 6465 7820 6f66 2074 6865 206f  t index of the o
+00001d80: 6c64 2054 6144 6565 6422 0a20 2020 2020  ld TaDeed".     
+00001d90: 2020 207d 2c0a 2020 2020 2020 2020 7b0a     },.        {.
+00001da0: 2020 2020 2020 2020 2020 226e 616d 6522            "name"
+00001db0: 3a20 2243 6f72 7265 6374 6c79 2073 6967  : "Correctly sig
+00001dc0: 6e65 6422 2c0a 2020 2020 2020 2020 2020  ned",.          
+00001dd0: 226e 756d 6265 7222 3a20 382c 0a20 2020  "number": 8,.   
+00001de0: 2020 2020 2020 2022 6465 7363 223a 2022         "desc": "
+00001df0: 4f6c 6444 6565 6454 7261 6e73 6665 724d  OldDeedTransferM
+00001e00: 7478 206d 7573 7420 6265 2073 6967 6e65  tx must be signe
+00001e10: 6420 6279 2047 6e66 4164 6d69 6e2c 2061  d by GnfAdmin, a
+00001e20: 6e64 2074 6865 2073 6967 6e61 7475 7265  nd the signature
+00001e30: 206d 7573 7420 6d61 7463 6820 7468 6520   must match the 
+00001e40: 7478 6e22 0a20 2020 2020 2020 207d 0a20  txn".        }. 
+00001e50: 2020 2020 205d 2c0a 2020 2020 2020 2264       ],.      "d
+00001e60: 6573 6322 3a20 224d 6573 7361 6765 2066  esc": "Message f
+00001e70: 6f72 2065 7863 6861 6e67 696e 6720 7468  or exchanging th
+00001e80: 6520 6f6c 6420 5461 4465 6564 2069 6e20  e old TaDeed in 
+00001e90: 7468 6520 5461 4d75 6c74 6920 6163 6374  the TaMulti acct
+00001ea0: 2028 322d 7369 6720 5b47 6e66 4164 6d69   (2-sig [GnfAdmi
+00001eb0: 6e2c 2054 6144 6165 6d6f 6e2c 2054 614f  n, TaDaemon, TaO
+00001ec0: 776e 6572 5d29 2061 6363 6f75 6e74 2077  wner]) account w
+00001ed0: 6974 6820 7468 6520 6e65 7720 5461 4465  ith the new TaDe
+00001ee0: 6564 2069 6e20 7468 6520 476e 6641 646d  ed in the GnfAdm
+00001ef0: 696e 2061 6363 6f75 6e74 2e22 0a20 2020  in account.".   
+00001f00: 207d 0a20 205d 0a7d 0a                    }.  ].}.
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/atn_actor_base.py` & `gridworks_atn-0.3.2/src/gwatn/atn_actor_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,18 +28,16 @@
 
 from gwatn.config import AtnSettings
 from gwatn.dispatch_contract import DispatchContract
 from gwatn.enums import AlgoCertType
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
 from gwatn.two_channel_actor_base import TwoChannelActorBase
-from gwatn.types import AtnParamsHeatpumpwithbooststore as AtnParams
-from gwatn.types import (
-    DispatchContractConfirmedHeatpumpwithbooststore_Maker as DispatchContractConfirmed_Maker,
-)
+from gwatn.types import AtnParams
+from gwatn.types import DispatchContractConfirmed_Maker
 from gwatn.types import GtShStatus
 from gwatn.types import GwCertId
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/config.py` & `gridworks_atn-0.3.2/src/gwatn/config.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/data_classes/.DS_Store` & `gridworks_atn-0.3.2/src/gwatn/data_classes/.DS_Store`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/data_classes/d_edge.py` & `gridworks_atn-0.3.2/src/gwatn/data_classes/d_edge.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/data_classes/d_graph.py` & `gridworks_atn-0.3.2/src/gwatn/data_classes/d_graph.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/data_classes/d_node.py` & `gridworks_atn-0.3.2/src/gwatn/data_classes/d_node.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/demo_methods.py` & `gridworks_atn-0.3.2/src/gwatn/demo_methods.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_discoverer.py` & `gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_discoverer.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_ta_owner.py` & `gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_ta_owner.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dev_utils/dev_validator.py` & `gridworks_atn-0.3.2/src/gwatn/dev_utils/dev_validator.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dev_utils/make_plants.py` & `gridworks_atn-0.3.2/src/gwatn/dev_utils/make_plants.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dispatch_contract.py` & `gridworks_atn-0.3.2/src/gwatn/dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/application.json` & `gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/application.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/approval.teal` & `gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/approval.teal`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/dispatch_contract_artifacts/contract.json` & `gridworks_atn-0.3.2/src/gwatn/dispatch_contract_artifacts/contract.json`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/enums/algo_cert_type.py` & `gridworks_atn-0.3.2/src/gwatn/enums/distribution_tariff.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class AlgoCertType(StrEnum):
+class DistributionTariff(StrEnum):
     """
-    Used to distinguish ASA vs SmartSignature certificates
+    Name of distribution tariff of local network company/utility
 
     Choices and descriptions:
 
-      * ASA: Certificate based on Algorand Standard Asset
-      * SmartSig: Certificate based on Algorand Smart Signature
+      * Unknown:
+      * VersantStorageHeatTariff:
+      * VersantATariff:
     """
 
-    ASA = auto()
-    SmartSig = auto()
+    Unknown = auto()
+    VersantStorageHeatTariff = auto()
+    VersantATariff = auto()
 
     @classmethod
-    def default(cls) -> "AlgoCertType":
+    def default(cls) -> "DistributionTariff":
         """
-        Returns default value ASA
+        Returns default value Unknown
         """
-        return cls.ASA
+        return cls.Unknown
 
     @classmethod
     def values(cls) -> List[str]:
         """
         Returns enum choices
         """
         return [elt.value for elt in cls]
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/enums/atn_spaceheat_strategy_name.py` & `gridworks_atn-0.3.2/src/gwatn/enums/energy_supply_type.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class AtnSpaceheatStrategyName(StrEnum):
+class EnergySupplyType(StrEnum):
     """
 
 
     Choices and descriptions:
 
-      * NoActor:
-      * SupervisorA:
-      * HeatPumpWithBoostStore:
+      * Unknown:
+      * StandardOffer:
+      * RealtimeLocalLmp:
     """
 
-    NoActor = auto()
-    SupervisorA = auto()
-    HeatPumpWithBoostStore = auto()
+    Unknown = auto()
+    StandardOffer = auto()
+    RealtimeLocalLmp = auto()
 
     @classmethod
-    def default(cls) -> "AtnSpaceheatStrategyName":
+    def default(cls) -> "EnergySupplyType":
         """
-        Returns default value NoActor
+        Returns default value Unknown
         """
-        return cls.NoActor
+        return cls.Unknown
 
     @classmethod
     def values(cls) -> List[str]:
         """
         Returns enum choices
         """
         return [elt.value for elt in cls]
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/enums/recognized_currency_unit.py` & `gridworks_atn-0.3.2/src/gwatn/enums/recognized_temperature_unit.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from enum import auto
 from typing import List
 
 from fastapi_utils.enums import StrEnum
 
 
-class RecognizedCurrencyUnit(StrEnum):
+class RecognizedTemperatureUnit(StrEnum):
     """
-    Unit of currency
+    Unit of temperature
 
     Choices and descriptions:
 
-      * Unknown:
-      * USD: US Dollar
-      * GBP: Pounds sterling
+      * C: Celcius
+      * F: Fahrenheit
     """
 
-    UNKNOWN = auto()
-    USD = auto()
-    GBP = auto()
+    C = auto()
+    F = auto()
 
     @classmethod
-    def default(cls) -> "RecognizedCurrencyUnit":
+    def default(cls) -> "RecognizedTemperatureUnit":
         """
-        Returns default value UNKNOWN
+        Returns default value C
         """
-        return cls.UNKNOWN
+        return cls.C
 
     @classmethod
     def values(cls) -> List[str]:
         """
         Returns enum choices
         """
         return [elt.value for elt in cls]
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/freedom_hack.py` & `gridworks_atn-0.3.2/src/gwatn/simple_atn_actor.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 import logging
 import time
-from typing import Optional
 
 import dotenv
 import rich
 from gwproto.messages import PeerActiveEvent
 from gwproto.messages import Ping as GridworksPing
-from gwproto.messages import SnapshotSpaceheatEvent
-from pydantic import BaseModel
 
 import gwatn.config as config
 from gwatn.atn_actor_base import AtnActorBase
 from gwatn.enums import TelemetryName
 from gwatn.types import GtDispatchBoolean_Maker
 from gwatn.types import GtShCliAtnCmd_Maker
 from gwatn.types import GtShStatus
@@ -24,30 +21,26 @@
 LOG_FORMAT = (
     "%(levelname) -10s %(sasctime)s %(name) -30s %(funcName) "
     "-35s %(lineno) -5d: %(message)s"
 )
 LOGGER = logging.getLogger(__name__)
 
 
-class FreedomHackAtn(AtnActorBase):
+class SimpleAtnActor(AtnActorBase):
     """Simple implementation of an AtnActor, for testing purposes"""
 
     def __init__(
         self,
         settings: config.AtnSettings = config.AtnSettings(
             _env_file=dotenv.find_dotenv()
         ),
     ):
         super().__init__(settings=settings)
         self._power_watts: int = 0
         LOGGER.info("Simple Atn Initialized")
-        self.latest_gpm: Optional[float] = None
-        self.latest_gallons: Optional[float] = None
-        self.latest_pump_read_time_s: Optional[int] = None
-        self.hp_allowed: bool = True
 
     def latest_price_from_market_maker(self, payload: LatestPrice) -> None:
         pass
 
     def new_timestep(self, payload: SimTimestep) -> None:
         """Set to work with a timestep per minute"""
 
@@ -106,50 +99,15 @@
     def _process_peer_active_event_from_scada(self, payload: PeerActiveEvent) -> None:
         """Atn has received gridworks.event.comm.peer.active message from its SCADA"""
         LOGGER.debug(f"_process_peer_active_event_from_scada: {payload}")
 
     def _process_gt_sh_status_from_scada(self, payload: GtShStatus) -> None:
         """Atn has received gt.sh.status message from its SCADA"""
         self.latest_status = payload
-        gallon_list = list(
-            filter(
-                lambda x: x.ShNodeAlias == "a.distsourcewater.pump.flowmeter",
-                payload.SimpleTelemetryList,
-            )
-        )[0]
-        prev_read_s = self.latest_pump_read_time_s
-        self.latest_pump_read_time_s = gallon_list.ReadTimeUnixMsList[-1] / 1000
-        prev_gallons = self.latest_gallons
-        self.latest_gallons = gallon_list.ValueList[-1] / 100
-        if prev_gallons is None:
-            return
-        delta_gallons = self.latest_gallons - prev_gallons
-        delta_minutes = (self.latest_pump_read_time_s - prev_read_s) / 60
-        exp_minute_weight = 0.5
-        self.latest_gpm = delta_gallons / delta_minutes
-
-        LOGGER.info(f"{round(self.latest_gpm, 2)} GPM")
-        LOGGER.info(
-            f"delta_minutes {round(delta_minutes,1)}, prev gallons: {prev_gallons}, latest gallons: {self.latest_gallons}"
-        )
-
-        if self.hp_allowed:
-            if self.latest_gpm < 2:
-                self.hp_allowed = False
-                self.turn_off("a.heatpump.relay")
-                LOGGER.info(
-                    f"gpm {round(self.latest_gpm,2)} below 2, turning off heat pump relay"
-                )
-        else:
-            if self.latest_gpm > 2.5:
-                self.hp_allowed = True
-                self.turn_on("a.heatpump.relay")
-                LOGGER.info(
-                    f"gpm {round(self.latest_gpm,2)} above 2.5, turning on heat pump relay"
-                )
+        LOGGER.debug(f"_process_gt_sh_status_from_scada: {payload}")
 
     def _process_power_watts_from_scada(self, payload: PowerWatts) -> None:
         """Atn has received power.watts message from its SCADA"""
         rich.print(f"Agg Power {payload.Watts} W")
         self._power_watts = payload.Watts
 
     def _process_snapshot_spaceheat_from_scada(
@@ -168,10 +126,8 @@
                 extra = f"{fahrenheit:5.2f} F"
             else:
                 extra = (
                     f"{payload.Snapshot.ValueList[i]} "
                     f"{payload.Snapshot.TelemetryNameList[i].value}"
                 )
             s += f"  {payload.Snapshot.AboutNodeAliasList[i]}: {extra}\n"
-        if self.latest_gpm:
-            s += f" a.distsourcewater.pump.flowmeter: {round(self.latest_gpm, 2)} GPM"
-        LOGGER.warning(s)
+        LOGGER.info(s)
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/python_ta_daemon.py` & `gridworks_atn-0.3.2/src/gwatn/python_ta_daemon.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/scada_actor.py` & `gridworks_atn-0.3.2/src/gwatn/simple_scada_sim_actor_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import random
 import time
 from typing import Optional
 from typing import no_type_check
 
 import dotenv
 import gridworks.algo_utils as algo_utils
-import gridworks.conversion_factors as cf
 import pendulum
 import requests
 from algosdk.atomic_transaction_composer import TransactionWithSigner
 from algosdk.future.transaction import *
 from algosdk.v2client.algod import AlgodClient
 from beaker.client import ApplicationClient
 from gridworks.actor_base import ActorBase
@@ -23,103 +22,91 @@
 
 import gwatn.api_types as api_types
 import gwatn.config as config
 from gwatn import DispatchContract
 from gwatn.enums import AlgoCertType
 from gwatn.enums import MessageCategorySymbol
 from gwatn.enums import UniverseType
-from gwatn.types import AtnParamsHeatpumpwithbooststore as AtnParams
-from gwatn.types import (
-    DispatchContractConfirmedHeatpumpwithbooststore as DispatchContractConfirmed,
-)
-from gwatn.types import (
-    DispatchContractConfirmedHeatpumpwithbooststore_Maker as DispatchContractConfirmed_Maker,
-)
+from gwatn.types import AtnParamsBrickstorageheater as AtnParams
+from gwatn.types import DispatchContractConfirmed
+from gwatn.types import DispatchContractConfirmed_Maker
 from gwatn.types import GtDispatchBoolean
 from gwatn.types import GtDispatchBoolean_Maker
 from gwatn.types import GwCertId
 from gwatn.types import GwCertId_Maker
 from gwatn.types import HeartbeatA
 from gwatn.types import HeartbeatA_Maker
 from gwatn.types import HeartbeatB
 from gwatn.types import HeartbeatB_Maker
 from gwatn.types import JoinDispatchContract_Maker
 from gwatn.types import ScadaCertTransfer_Maker
-from gwatn.types import SimScadaDriverReport
-from gwatn.types import SimScadaDriverReport_Maker
+from gwatn.types import SimplesimDriverReport
+from gwatn.types import SimplesimDriverReport_Maker
 from gwatn.types import SimTimestep
 from gwatn.types import SimTimestep_Maker
-from gwatn.types import SnapshotHeatpumpwithbooststore
+from gwatn.types import SnapshotBrickstorageheater as Snapshot
 
 
 DISPATCH_CONTRACT_REPORTING_ALGOS = 5
 
 LOG_FORMAT = (
     "%(levelname) -10s %(sasctime)s %(name) -30s %(funcName) "
     "-35s %(lineno) -5d: %(message)s"
 )
 LOGGER = logging.getLogger(__name__)
 
 LOGGER.setLevel(logging.INFO)
 
 
 def get_max_store_kwh_th(params: AtnParams) -> float:
-    return (
-        cf.KWH_TH_PER_GALLON_PER_DEG_F
-        * params.StoreSizeGallons
-        * (params.MaxStoreTempF - params.ZeroPotentialEnergyWaterTempF)
-    )
+    room_temp_c = (params.RoomTempF - 32) * 5 / 9
+    return params.C * (params.MaxBrickTempC - room_temp_c)
 
 
 class AtnHbStatus(BaseModel):
     LastHeartbeatReceivedMs: int
     AtnLastHex: Optional[str] = None
     ScadaLastHex: str = "0"
 
 
-class ScadaActor(ActorBase):
+class SimpleScadaSimActorBase(ActorBase):
     def __init__(
         self,
         settings: config.ScadaSettings = config.ScadaSettings(
             _env_file=dotenv.find_dotenv()
         ),
     ):
         super().__init__(settings=settings)
-        self.api_type_maker_by_name = (
-            api_types.TypeMakerByName
-        )  # overwrites base class to include types used in this repo
+
         self.settings = settings
         self.atn_gni_id = settings.atn_gni_id
         self.acct: BasicAccount = BasicAccount(settings.sk.get_secret_value())
         self.client: AlgodClient = AlgodClient(
             settings.algo_api_secrets.algod_token.get_secret_value(),
             settings.public.algod_address,
         )
-
+        self.atn_params_type_name: str = "atn.params.brickstorageheater"
         self.sp = self.client.suggested_params()
         self.cert_id: Optional[GwCertId] = None
         self.talking_with: bool = False
         self.atn_hb_status = AtnHbStatus(
             LastHeartbeatReceivedMs=int(1000 * time.time())
         )
         # The dc_client (DispatchContract client) builds on top of the Algorand beaker ApplicationClient
         self.dc_client: Optional[ApplicationClient] = None
         self.dc_app_id: Optional[int] = None
         self.algo_init_check()
         self.universe_type = as_enum(
             self.settings.universe_type_value, UniverseType, UniverseType.default()
         )
         self._time: float = self.get_initial_time_s()
-
-        self.boost_power_kw: float = 0
-        self.heatpump_power_kw: float = 0
-        self.cop: float = 0
-        self.store_kwh: int = 0
-        self.max_store_kwh: int = 0
-        self.atn_params: Optional[AtnParams] = None
+        self.api_type_maker_by_name = (
+            api_types.TypeMakerByName
+        )  # overwrites base class to include types used in this repo
+        self.atn_params_type_name: str = "atn.params"  # overwrite in the subclass
 
     @property
     def atn_alias(self):
         """Removes `scada` from the end of the SCADA's GNodeAlias"""
         return self.alias[:-6]
 
     @property
@@ -199,19 +186,19 @@
                 LOGGER.info(
                     f"Ignoring HeartbeatB from GNode with role {from_role}; expects AtomicTNode"
                 )
             try:
                 self.heartbeat_from_atn(ping=payload)
             except:
                 LOGGER.exception("Error in heartbeat_from_atn")
-        elif payload.TypeName == SimScadaDriverReport_Maker.type_name:
+        elif payload.TypeName == SimplesimDriverReport_Maker.type_name:
             try:
-                self.sim_scada_driver_report_received(payload)
+                self.simplesim_driver_report_received(payload)
             except:
-                LOGGER.exception("Error in sim_scada_driver_report_received")
+                LOGGER.exception("Error in simplesim_driver_report_received")
         elif payload.TypeName == SimTimestep_Maker.type_name:
             if from_role != GNodeRole.TimeCoordinator:
                 LOGGER.info(
                     f"Ignoring SimTimestep from GNode with role {from_role}; expects TimeCoordinator"
                 )
             try:
                 self.timestep_from_timecoordinator(payload)
@@ -519,54 +506,56 @@
             )
         if self.in_dispatch_contract():
             LOGGER.warning(
                 f"Ignoring DispatchContractConfirmed - already in dispatch contract {self.dc_app_id}"
             )
             return
 
+        if payload.AtnParamsTypeName != self.atn_params_type_name:
+            LOGGER.info(
+                f"Unexpected AtnParamsTypeName {payload.AtnParamsTypeName}. Expects {self.atn_params_type_name}"
+            )
+            return
+        self.atn_params = payload.Params
         app_state = self.dc_client.get_application_state()
         if "ta_trading_rights_idx" not in app_state.keys():
             LOGGER.warning(f"Atn bootstrap is not finished. Ignoring")
             return
 
         self.atn_gni_id = payload.FromGNodeInstanceId
-        self.atn_params = payload.AtnParams
+
         with open(".env", "a") as file:
             file.write(f'SCADA_ATN_GNI_ID="{payload.FromGNodeInstanceId}"\n')
         self.dc_client.opt_in()
         LOGGER.info(f"Dispatch Contract {self.dc_app_id} is live")
 
     #########################################################
     # Make the below into abstractmethods if pulling out base class
     #########################################################
 
-    def sim_scada_driver_report_received(self, payload: SimScadaDriverReport) -> None:
+    def simplesim_driver_report_received(self, payload: SimplesimDriverReport) -> None:
         """This gets received right before the top of the hour, from our
         best simulation of the TerminalAsset (which is happening in the
-        AtomicTNode)."""
-        if payload.FromGNodeInstanceId != self.atn_gni_id:
+        AtomicTNode).
+
+        Should be overwritten by the derived class, according to the
+        DriverDataTypeName. Should then send snapshot."""
+        if payload.FromGNodeInstanecId != self.atn_gni_id:
             LOGGER.info(f"Igoring {payload} - incorrect GNodeInstanceId")
-        self.boost_power_kw = payload.BoostPowerKwTimes1000 / 1000
-        self.heatpump_power_kw = payload.HeatpumpPowerKwTimes1000 / 1000
-        self.cop = payload.CopTimes10 / 10
-        self.store_kwh = payload.StoreKwh
-        self.max_store_kwh = payload.MaxStoreKwh
-        self.send_snapshot()
 
     def send_snapshot(self):
         """Send a snapshot of current core sensed values to AtomicTNode.
         This is done every hour, and also on sensed power change."""
         if self.atn_params is None:
             return
-        report_payload = SnapshotHeatpumpwithbooststore(
+        report_payload = Snapshot(
             FromGNodeAlias=self.alias,
             FromGNodeInstanceId=self.g_node_instance_id,
-            BoostPowerKwTimes1000=int(1000 * self.boost_power_kw),
-            HeatpumpPowerKwTimes1000=int(1000 * self.heatpump_power_kw),
-            CopTimes10=int(10 * self.cop),
+            PowerWatts=self.power_watts,
+            StoreKwh=self.store_kwh,
             MaxStoreKwh=get_max_store_kwh_th(self.atn_params),
             AboutTerminalAssetAlias=self.ta_alias,
         )
         self.send_message(
             payload=report_payload,
             to_role=GNodeRole.AtomicTNode,
             to_g_node_alias=self.atn_alias,
@@ -576,41 +565,33 @@
         """
         Dispatch received from AtomicTNode
 
           - Checks that the GNodeAlias and GNodeInstanceId belong to its
         AtomicTNode and that we have a dispatch contract
           - Sets talking_with to true
           - Follows instructions (turns on or turns off). Will turn on or
-          off boost unless AboutNodeName is "a.heatpump"
+          off boost unless AboutNodeName is "a.element"
 
         For hourly sim:
           - Updatespower
           - Send status to AtomicTNode
         """
         if self.atn_params is None or self.in_dispatch_contract() is False:
             LOGGER.info("Igoring dispatch command, DispatchContract is not started")
         if payload.FromGNodeInstanceId != self.atn_gni_id:
             LOGGER.info(f"Igoring {payload}, not my Atn's GNodeInstanceId")
         self.talking_with = True
-        if payload.AboutNodeName == "a.heatpump":
+        if payload.AboutNodeName == "a.elements":
             # Making the grossly simplifying assumption that the heat pump turns on immediately
             if payload.RelayState == 1:
-                new_heatpump_power_kw = self.atn_params.RatedHeatpumpElectricityKw
-            else:
-                new_heatpump_power_kw = 0
-            if self.heatpump_power_kw != new_heatpump_power_kw:
-                self.heatpump_power_kw = new_heatpump_power_kw
-                self.send_snapshot()
-        else:
-            if payload.RelayState == 1:
-                new_boost_power_kw = self.atn_params.StoreMaxPowerKw
+                new_power_watts = self.atn_params.RatedMaxPowerKw * 1000
             else:
-                new_boost_power_kw = 0
-            if self.boost_power_kw != new_boost_power_kw:
-                self.boost_power_kw = new_boost_power_kw
+                new_power_watts = 0
+            if self.power_watts != new_power_watts:
+                self.power_watts = new_power_watts
                 self.send_snapshot()
 
     def new_timestep(self, payload: SimTimestep) -> None:
         # LOGGER.info("New timestep")
         if not self.in_dispatch_contract():
             self.initialize_dispatch_contract()
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/scada_codec.py` & `gridworks_atn-0.3.2/src/gwatn/scada_codec.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/ta_daemon_rest_api.py` & `gridworks_atn-0.3.2/src/gwatn/ta_daemon_rest_api.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/two_channel_actor_base.py` & `gridworks_atn-0.3.2/src/gwatn/two_channel_actor_base.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/__init__.py` & `gridworks_atn-0.3.2/src/gwatn/types/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,30 @@
 """ List of all the types """
 
+# From gridworks
+from gridworks.types import BaseGNodeGt
+from gridworks.types import BaseGNodeGt_Maker
+from gridworks.types import GNodeGt
+from gridworks.types import GNodeGt_Maker
+from gridworks.types import GNodeInstanceGt
+from gridworks.types import GNodeInstanceGt_Maker
+from gridworks.types import GwCertId
+from gridworks.types import GwCertId_Maker
+from gridworks.types import HeartbeatA
+from gridworks.types import HeartbeatA_Maker
+from gridworks.types import Ready
+from gridworks.types import Ready_Maker
+from gridworks.types import SimTimestep
+from gridworks.types import SimTimestep_Maker
+from gridworks.types import SuperStarter
+from gridworks.types import SuperStarter_Maker
+from gridworks.types import SupervisorContainerGt
+from gridworks.types import SupervisorContainerGt_Maker
+
+# From gwproto
 from gwproto.types import ComponentAttributeClassGt
 from gwproto.types import ComponentAttributeClassGt_Maker
 from gwproto.types import ComponentGt
 from gwproto.types import ComponentGt_Maker
 from gwproto.types import DataChannel
 from gwproto.types import DataChannel_Maker
 from gwproto.types import EgaugeIo
@@ -65,63 +86,37 @@
 from gwproto.types.electric_meter_component_gt import ElectricMeterComponentGt
 from gwproto.types.electric_meter_component_gt import ElectricMeterComponentGt_Maker
 from gwproto.types.multipurpose_sensor_component_gt import MultipurposeSensorComponentGt
 from gwproto.types.multipurpose_sensor_component_gt import (
     MultipurposeSensorComponentGt_Maker,
 )
 
-# Not in gwproto
+# From gwatn
 from gwatn.types.accepted_bid import AcceptedBid
 from gwatn.types.accepted_bid import AcceptedBid_Maker
 from gwatn.types.atn_bid import AtnBid
 from gwatn.types.atn_bid import AtnBid_Maker
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore,
-)
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore_Maker,
-)
-from gwatn.types.atn_params_report_heatpumpwithbooststore import (
-    AtnParamsReportHeatpumpwithbooststore,
-)
-from gwatn.types.atn_params_report_heatpumpwithbooststore import (
-    AtnParamsReportHeatpumpwithbooststore_Maker,
-)
-from gwatn.types.base_g_node_gt import BaseGNodeGt
-from gwatn.types.base_g_node_gt import BaseGNodeGt_Maker
+from gwatn.types.atn_params import AtnParams
+from gwatn.types.atn_params import AtnParams_Maker
+from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater
+from gwatn.types.atn_params_brickstorageheater import AtnParamsBrickstorageheater_Maker
+from gwatn.types.atn_params_report import AtnParamsReport
+from gwatn.types.atn_params_report import AtnParamsReport_Maker
 from gwatn.types.basegnode_scada_create import BasegnodeScadaCreate
 from gwatn.types.basegnode_scada_create import BasegnodeScadaCreate_Maker
 from gwatn.types.discoverycert_algo_create import DiscoverycertAlgoCreate
 from gwatn.types.discoverycert_algo_create import DiscoverycertAlgoCreate_Maker
-from gwatn.types.dispatch_contract_confirmed_heatpumpwithbooststore import (
-    DispatchContractConfirmedHeatpumpwithbooststore,
-)
-from gwatn.types.dispatch_contract_confirmed_heatpumpwithbooststore import (
-    DispatchContractConfirmedHeatpumpwithbooststore_Maker,
-)
-from gwatn.types.flo_params_heatpumpwithbooststore import (
-    FloParamsHeatpumpwithbooststore,
-)
-from gwatn.types.flo_params_heatpumpwithbooststore import (
-    FloParamsHeatpumpwithbooststore_Maker,
-)
-from gwatn.types.g_node_gt import GNodeGt
-from gwatn.types.g_node_gt import GNodeGt_Maker
-from gwatn.types.g_node_instance_gt import GNodeInstanceGt
-from gwatn.types.g_node_instance_gt import GNodeInstanceGt_Maker
-from gwatn.types.gt_dispatch_boolean import GtDispatchBoolean
-from gwatn.types.gt_dispatch_boolean import GtDispatchBoolean_Maker
-from gwatn.types.gw_cert_id import GwCertId
-from gwatn.types.gw_cert_id import GwCertId_Maker
-from gwatn.types.heartbeat_a import HeartbeatA
-from gwatn.types.heartbeat_a import HeartbeatA_Maker
-from gwatn.types.heartbeat_algo_audit import HeartbeatAlgoAudit
-from gwatn.types.heartbeat_algo_audit import HeartbeatAlgoAudit_Maker
-from gwatn.types.heartbeat_b import HeartbeatB
-from gwatn.types.heartbeat_b import HeartbeatB_Maker
+from gwatn.types.dispatch_contract_confirmed import DispatchContractConfirmed
+from gwatn.types.dispatch_contract_confirmed import DispatchContractConfirmed_Maker
+from gwatn.types.flo_params import FloParams
+from gwatn.types.flo_params import FloParams_Maker
+from gwatn.types.flo_params_brickstorageheater import FloParamsBrickstorageheater
+from gwatn.types.flo_params_brickstorageheater import FloParamsBrickstorageheater_Maker
+from gwatn.types.flo_params_report import FloParamsReport
+from gwatn.types.flo_params_report import FloParamsReport_Maker
 from gwatn.types.initial_tadeed_algo_create import InitialTadeedAlgoCreate
 from gwatn.types.initial_tadeed_algo_create import InitialTadeedAlgoCreate_Maker
 from gwatn.types.initial_tadeed_algo_optin import InitialTadeedAlgoOptin
 from gwatn.types.initial_tadeed_algo_optin import InitialTadeedAlgoOptin_Maker
 from gwatn.types.initial_tadeed_algo_transfer import InitialTadeedAlgoTransfer
 from gwatn.types.initial_tadeed_algo_transfer import InitialTadeedAlgoTransfer_Maker
 from gwatn.types.join_dispatch_contract import JoinDispatchContract
@@ -138,32 +133,30 @@
 from gwatn.types.new_tadeed_send import NewTadeedSend_Maker
 from gwatn.types.old_tadeed_algo_return import OldTadeedAlgoReturn
 from gwatn.types.old_tadeed_algo_return import OldTadeedAlgoReturn_Maker
 from gwatn.types.price_quantity import PriceQuantity
 from gwatn.types.price_quantity import PriceQuantity_Maker
 from gwatn.types.price_quantity_unitless import PriceQuantityUnitless
 from gwatn.types.price_quantity_unitless import PriceQuantityUnitless_Maker
-from gwatn.types.ready import Ready
-from gwatn.types.ready import Ready_Maker
 from gwatn.types.scada_cert_transfer import ScadaCertTransfer
 from gwatn.types.scada_cert_transfer import ScadaCertTransfer_Maker
-from gwatn.types.sim_scada_driver_report import SimScadaDriverReport
-from gwatn.types.sim_scada_driver_report import SimScadaDriverReport_Maker
-from gwatn.types.sim_timestep import SimTimestep
-from gwatn.types.sim_timestep import SimTimestep_Maker
+from gwatn.types.simplesim_driver_data import SimplesimDriverData
+from gwatn.types.simplesim_driver_data import SimplesimDriverData_Maker
+from gwatn.types.simplesim_driver_data_bsh import SimplesimDriverDataBsh
+from gwatn.types.simplesim_driver_data_bsh import SimplesimDriverDataBsh_Maker
+from gwatn.types.simplesim_driver_report import SimplesimDriverReport
+from gwatn.types.simplesim_driver_report import SimplesimDriverReport_Maker
+from gwatn.types.simplesim_snapshot_brickstorageheater import (
+    SimplesimSnapshotBrickstorageheater,
+)
+from gwatn.types.simplesim_snapshot_brickstorageheater import (
+    SimplesimSnapshotBrickstorageheater_Maker,
+)
 from gwatn.types.sla_enter import SlaEnter
 from gwatn.types.sla_enter import SlaEnter_Maker
-from gwatn.types.snapshot_heatpumpwithbooststore import SnapshotHeatpumpwithbooststore
-from gwatn.types.snapshot_heatpumpwithbooststore import (
-    SnapshotHeatpumpwithbooststore_Maker,
-)
-from gwatn.types.super_starter import SuperStarter
-from gwatn.types.super_starter import SuperStarter_Maker
-from gwatn.types.supervisor_container_gt import SupervisorContainerGt
-from gwatn.types.supervisor_container_gt import SupervisorContainerGt_Maker
 from gwatn.types.tadeed_specs_hack import TadeedSpecsHack
 from gwatn.types.tadeed_specs_hack import TadeedSpecsHack_Maker
 from gwatn.types.tavalidatorcert_algo_create import TavalidatorcertAlgoCreate
 from gwatn.types.tavalidatorcert_algo_create import TavalidatorcertAlgoCreate_Maker
 from gwatn.types.tavalidatorcert_algo_transfer import TavalidatorcertAlgoTransfer
 from gwatn.types.tavalidatorcert_algo_transfer import TavalidatorcertAlgoTransfer_Maker
 from gwatn.types.terminalasset_certify_hack import TerminalassetCertifyHack
@@ -171,50 +164,54 @@
 
 
 __all__ = [
     "AcceptedBid",
     "AcceptedBid_Maker",
     "AtnBid",
     "AtnBid_Maker",
-    "AtnParamsHeatpumpwithbooststore",
-    "AtnParamsHeatpumpwithbooststore_Maker",
-    "AtnParamsReportHeatpumpwithbooststore",
-    "AtnParamsReportHeatpumpwithbooststore_Maker",
+    "AtnParams",
+    "AtnParams_Maker",
+    "AtnParamsBrickstorageheater",
+    "AtnParamsBrickstorageheater_Maker",
+    "AtnParamsReport",
+    "AtnParamsReport_Maker",
     "BaseGNodeGt",
     "BaseGNodeGt_Maker",
     "BasegnodeScadaCreate",
     "BasegnodeScadaCreate_Maker",
     "ComponentAttributeClassGt",
     "ComponentAttributeClassGt_Maker",
     "ComponentGt",
     "ComponentGt_Maker",
     "DataChannel",
     "DataChannel_Maker",
     "DiscoverycertAlgoCreate",
     "DiscoverycertAlgoCreate_Maker",
-    "DispatchContractConfirmedHeatpumpwithbooststore",
-    "DispatchContractConfirmedHeatpumpwithbooststore_Maker",
+    "DispatchContractConfirmed",
+    "DispatchContractConfirmed_Maker",
     "EgaugeIo",
     "EgaugeIo_Maker",
     "EgaugeRegisterConfig",
     "EgaugeRegisterConfig_Maker",
     "ElectricMeterCacGt",
     "ElectricMeterCacGt_Maker",
     "ElectricMeterComponentGt",
     "ElectricMeterComponentGt_Maker",
-    "FloParamsHeatpumpwithbooststore",
-    "FloParamsHeatpumpwithbooststore_Maker",
+    "FloParams",
+    "FloParams_Maker",
+    "FloParamsBrickstorageheater",
+    "FloParamsBrickstorageheater_Maker",
+    "FloParamsReport",
+    "FloParamsReport_Maker",
     "GNodeGt",
     "GNodeGt_Maker",
     "GNodeInstanceGt",
     "GNodeInstanceGt_Maker",
     "GtDispatchBoolean",
     "GtDispatchBoolean_Maker",
-    "GtDispatchBoolean",
-    "GtDispatchBoolean_Maker",
     "GtDispatchBooleanLocal",
     "GtDispatchBooleanLocal_Maker",
     "GtDriverBooleanactuatorCmd",
     "GtDriverBooleanactuatorCmd_Maker",
     "GtShBooleanactuatorCmdStatus",
     "GtShBooleanactuatorCmdStatus_Maker",
     "GtShCliAtnCmd",
@@ -229,18 +226,14 @@
     "GtShTelemetryFromMultipurposeSensor_Maker",
     "GtTelemetry",
     "GtTelemetry_Maker",
     "GwCertId",
     "GwCertId_Maker",
     "HeartbeatA",
     "HeartbeatA_Maker",
-    "HeartbeatAlgoAudit",
-    "HeartbeatAlgoAudit_Maker",
-    "HeartbeatB",
-    "HeartbeatB_Maker",
     "HeartbeatB",
     "HeartbeatB_Maker",
     "InitialTadeedAlgoCreate",
     "InitialTadeedAlgoCreate_Maker",
     "InitialTadeedAlgoOptin",
     "InitialTadeedAlgoOptin_Maker",
     "InitialTadeedAlgoTransfer",
@@ -281,26 +274,30 @@
     "RelayComponentGt_Maker",
     "ResistiveHeaterCacGt",
     "ResistiveHeaterCacGt_Maker",
     "ResistiveHeaterComponentGt",
     "ResistiveHeaterComponentGt_Maker",
     "ScadaCertTransfer",
     "ScadaCertTransfer_Maker",
-    "SimScadaDriverReport",
-    "SimScadaDriverReport_Maker",
     "SimTimestep",
     "SimTimestep_Maker",
     "SimpleTempSensorCacGt",
     "SimpleTempSensorCacGt_Maker",
     "SimpleTempSensorComponentGt",
     "SimpleTempSensorComponentGt_Maker",
+    "SimplesimDriverData",
+    "SimplesimDriverData_Maker",
+    "SimplesimDriverDataBsh",
+    "SimplesimDriverDataBsh_Maker",
+    "SimplesimDriverReport",
+    "SimplesimDriverReport_Maker",
+    "SimplesimSnapshotBrickstorageheater",
+    "SimplesimSnapshotBrickstorageheater_Maker",
     "SlaEnter",
     "SlaEnter_Maker",
-    "SnapshotHeatpumpwithbooststore",
-    "SnapshotHeatpumpwithbooststore_Maker",
     "SnapshotSpaceheat",
     "SnapshotSpaceheat_Maker",
     "SpaceheatNodeGt",
     "SpaceheatNodeGt_Maker",
     "SuperStarter",
     "SuperStarter_Maker",
     "SupervisorContainerGt",
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/accepted_bid.py` & `gridworks_atn-0.3.2/src/gwatn/types/accepted_bid.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,15 +63,15 @@
       MarketSlot for that MarketType (i.e. divisible by 3600
       for hourly markets)
       - The middle words have LeftRightDot format (GNodeAlias
       of the MarketMaker)
     Example: rt60gate5.d1.isone.ver.keene.1673539200
 
     """
-    from gwatn.data_classes.market_type import MarketType
+    from gwatn.data_classes import MarketType
 
     try:
         x = v.split(".")
     except AttributeError:
         raise ValueError(f"{v} failed to split on '.'")
     slot_start = x[-1]
     if len(slot_start) != 10:
@@ -155,14 +155,17 @@
             pq_pairs.append(elt.as_dict())
         d["PqPairs"] = pq_pairs
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class AcceptedBid_Maker:
     type_name = "accepted.bid"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/atn_bid.py` & `gridworks_atn-0.3.2/src/gwatn/types/atn_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -288,15 +288,15 @@
       MarketSlot for that MarketType (i.e. divisible by 3600
       for hourly markets)
       - The middle words have LeftRightDot format (GNodeAlias
       of the MarketMaker)
     Example: rt60gate5.d1.isone.ver.keene.1673539200
 
     """
-    from gwatn.data_classes.market_type import MarketType
+    from gwatn.data_classes import MarketType
 
     try:
         x = v.split(".")
     except AttributeError:
         raise ValueError(f"{v} failed to split on '.'")
     slot_start = x[-1]
     if len(slot_start) != 10:
@@ -483,14 +483,17 @@
             QuantityUnit
         )
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class AtnBid_Maker:
     type_name = "atn.bid"
     version = "001"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/atn_params_report_heatpumpwithbooststore.py` & `gridworks_atn-0.3.2/src/gwatn/types/atn_params_report.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,21 @@
-"""Type atn.params.report.heatpumpwithbooststore, version 000"""
+"""Type atn.params.report, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 from typing import Optional
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore,
-)
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore_Maker,
-)
+from gwatn.types.atn_params import AtnParams
+from gwatn.types.atn_params import AtnParams_Maker
 
 
 def check_is_reasonable_unix_time_s(v: int) -> None:
     """
     ReasonableUnixTimeS format: time in unix seconds between Jan 1 2000 and Jan 1 3000
 
     Raises:
@@ -85,39 +81,40 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-class AtnParamsReportHeatpumpwithbooststore(BaseModel):
+class AtnParamsReport(BaseModel):
     """AtomicTNode reporting its AtnParams.
 
     Parameters like the size of the thermal store.
     """
 
     GNodeAlias: str = Field(
         title="GNodeAlias",
     )
     GNodeInstanceId: str = Field(
         title="GNodeInstanceId",
     )
+    AtnParamsTypeName: str = Field(
+        title="AtnParamsTypeName",
+    )
     TimeUnixS: int = Field(
         title="TimeUnixS",
     )
     IrlTimeUnixS: Optional[int] = Field(
         title="IrlTimeUnixS",
         default=None,
     )
-    AtnParams: AtnParamsHeatpumpwithbooststore = Field(
-        title="AtnParams",
+    Params: AtnParams = Field(
+        title="Params",
     )
-    TypeName: Literal[
-        "atn.params.report.heatpumpwithbooststore"
-    ] = "atn.params.report.heatpumpwithbooststore"
+    TypeName: Literal["atn.params.report"] = "atn.params.report"
     Version: str = "000"
 
     @validator("GNodeAlias")
     def _check_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
@@ -130,14 +127,24 @@
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
                 f"GNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
+    @validator("AtnParamsTypeName")
+    def _check_atn_params_type_name(cls, v: str) -> str:
+        try:
+            check_is_left_right_dot(v)
+        except ValueError as e:
+            raise ValueError(
+                f"AtnParamsTypeName failed LeftRightDot format validation: {e}"
+            )
+        return v
+
     @validator("TimeUnixS")
     def _check_time_unix_s(cls, v: int) -> int:
         try:
             check_is_reasonable_unix_time_s(v)
         except ValueError as e:
             raise ValueError(
                 f"TimeUnixS failed ReasonableUnixTimeS format validation: {e}"
@@ -156,88 +163,92 @@
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         if d["IrlTimeUnixS"] is None:
             del d["IrlTimeUnixS"]
-        d["AtnParams"] = self.AtnParams.as_dict()
+        d["Params"] = self.Params.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class AtnParamsReportHeatpumpwithbooststore_Maker:
-    type_name = "atn.params.report.heatpumpwithbooststore"
+class AtnParamsReport_Maker:
+    type_name = "atn.params.report"
     version = "000"
 
     def __init__(
         self,
         g_node_alias: str,
         g_node_instance_id: str,
+        atn_params_type_name: str,
         time_unix_s: int,
         irl_time_unix_s: Optional[int],
-        atn_params: AtnParamsHeatpumpwithbooststore,
+        params: AtnParams,
     ):
-        self.tuple = AtnParamsReportHeatpumpwithbooststore(
+        self.tuple = AtnParamsReport(
             GNodeAlias=g_node_alias,
             GNodeInstanceId=g_node_instance_id,
+            AtnParamsTypeName=atn_params_type_name,
             TimeUnixS=time_unix_s,
             IrlTimeUnixS=irl_time_unix_s,
-            AtnParams=atn_params,
+            Params=params,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: AtnParamsReportHeatpumpwithbooststore) -> str:
+    def tuple_to_type(cls, tuple: AtnParamsReport) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> AtnParamsReportHeatpumpwithbooststore:
+    def type_to_tuple(cls, t: str) -> AtnParamsReport:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> AtnParamsReportHeatpumpwithbooststore:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> AtnParamsReport:
         d2 = dict(d)
         if "GNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing GNodeAlias")
         if "GNodeInstanceId" not in d2.keys():
             raise SchemaError(f"dict {d2} missing GNodeInstanceId")
+        if "AtnParamsTypeName" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing AtnParamsTypeName")
         if "TimeUnixS" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TimeUnixS")
         if "IrlTimeUnixS" not in d2.keys():
             d2["IrlTimeUnixS"] = None
-        if "AtnParams" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing AtnParams")
-        if not isinstance(d2["AtnParams"], dict):
-            raise SchemaError(
-                f"d['AtnParams'] {d2['AtnParams']} must be a AtnParamsHeatpumpwithbooststore!"
-            )
-        atn_params = AtnParamsHeatpumpwithbooststore_Maker.dict_to_tuple(
-            d2["AtnParams"]
-        )
-        d2["AtnParams"] = atn_params
+        if "Params" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing Params")
+        if not isinstance(d2["Params"], dict):
+            raise SchemaError(f"d['Params'] {d2['Params']} must be a AtnParams!")
+        params = AtnParams_Maker.dict_to_tuple(d2["Params"])
+        d2["Params"] = params
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return AtnParamsReportHeatpumpwithbooststore(
+        return AtnParamsReport(
             GNodeAlias=d2["GNodeAlias"],
             GNodeInstanceId=d2["GNodeInstanceId"],
+            AtnParamsTypeName=d2["AtnParamsTypeName"],
             TimeUnixS=d2["TimeUnixS"],
             IrlTimeUnixS=d2["IrlTimeUnixS"],
-            AtnParams=d2["AtnParams"],
+            Params=d2["Params"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/base_g_node_gt.py` & `gridworks_atn-0.3.2/src/gwatn/types/flo_params_brickstorageheater.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Type base.g.node.gt, version 002"""
+"""Type flo.params.brickstorageheater, version 000"""
 import json
 from enum import auto
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Literal
 from typing import Optional
@@ -10,162 +10,149 @@
 from fastapi_utils.enums import StrEnum
 from gridworks.errors import SchemaError
 from gridworks.message import as_enum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwatn.data_classes.base_g_node import BaseGNode
-from gwatn.enums import CoreGNodeRole
-from gwatn.enums import GNodeStatus
+from gwatn.enums import RecognizedCurrencyUnit
+from gwatn.enums import RecognizedTemperatureUnit
 
 
-class CoreGNodeRole000SchemaEnum:
-    enum_name: str = "core.g.node.role.000"
+class RecognizedCurrencyUnit000SchemaEnum:
+    enum_name: str = "recognized.currency.unit.000"
     symbols: List[str] = [
         "00000000",
-        "0f8872f7",
-        "d9823442",
-        "86f21dd2",
-        "9521af06",
-        "4502e355",
-        "d67e564e",
-        "7a8e4046",
+        "e57c5143",
+        "f7b38fc5",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
 
 
-class CoreGNodeRole000(StrEnum):
-    Other = auto()
-    TerminalAsset = auto()
-    AtomicTNode = auto()
-    MarketMaker = auto()
-    AtomicMeteringNode = auto()
-    ConductorTopologyNode = auto()
-    InterconnectionComponent = auto()
-    Scada = auto()
+class RecognizedCurrencyUnit000(StrEnum):
+    UNKNOWN = auto()
+    USD = auto()
+    GBP = auto()
 
     @classmethod
-    def default(cls) -> "CoreGNodeRole000":
-        return cls.Other
+    def default(cls) -> "RecognizedCurrencyUnit000":
+        return cls.UNKNOWN
 
     @classmethod
     def values(cls) -> List[str]:
         return [elt.value for elt in cls]
 
 
-class CoreGNodeRoleMap:
+class RecognizedCurrencyUnitMap:
     @classmethod
-    def type_to_local(cls, symbol: str) -> CoreGNodeRole:
-        if not CoreGNodeRole000SchemaEnum.is_symbol(symbol):
-            raise SchemaError(f"{symbol} must belong to CoreGNodeRole000 symbols")
+    def type_to_local(cls, symbol: str) -> RecognizedCurrencyUnit:
+        if not RecognizedCurrencyUnit000SchemaEnum.is_symbol(symbol):
+            raise SchemaError(
+                f"{symbol} must belong to RecognizedCurrencyUnit000 symbols"
+            )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
-        return as_enum(versioned_enum, CoreGNodeRole, CoreGNodeRole.default())
+        return as_enum(
+            versioned_enum, RecognizedCurrencyUnit, RecognizedCurrencyUnit.default()
+        )
 
     @classmethod
-    def local_to_type(cls, core_g_node_role: CoreGNodeRole) -> str:
-        if not isinstance(core_g_node_role, CoreGNodeRole):
-            raise SchemaError(f"{core_g_node_role} must be of type {CoreGNodeRole}")
+    def local_to_type(cls, recognized_currency_unit: RecognizedCurrencyUnit) -> str:
+        if not isinstance(recognized_currency_unit, RecognizedCurrencyUnit):
+            raise SchemaError(
+                f"{recognized_currency_unit} must be of type {RecognizedCurrencyUnit}"
+            )
         versioned_enum = as_enum(
-            core_g_node_role, CoreGNodeRole000, CoreGNodeRole000.default()
+            recognized_currency_unit,
+            RecognizedCurrencyUnit000,
+            RecognizedCurrencyUnit000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
-    type_to_versioned_enum_dict: Dict[str, CoreGNodeRole000] = {
-        "00000000": CoreGNodeRole000.Other,
-        "0f8872f7": CoreGNodeRole000.TerminalAsset,
-        "d9823442": CoreGNodeRole000.AtomicTNode,
-        "86f21dd2": CoreGNodeRole000.MarketMaker,
-        "9521af06": CoreGNodeRole000.AtomicMeteringNode,
-        "4502e355": CoreGNodeRole000.ConductorTopologyNode,
-        "d67e564e": CoreGNodeRole000.InterconnectionComponent,
-        "7a8e4046": CoreGNodeRole000.Scada,
+    type_to_versioned_enum_dict: Dict[str, RecognizedCurrencyUnit000] = {
+        "00000000": RecognizedCurrencyUnit000.UNKNOWN,
+        "e57c5143": RecognizedCurrencyUnit000.USD,
+        "f7b38fc5": RecognizedCurrencyUnit000.GBP,
     }
 
-    versioned_enum_to_type_dict: Dict[CoreGNodeRole000, str] = {
-        CoreGNodeRole000.Other: "00000000",
-        CoreGNodeRole000.TerminalAsset: "0f8872f7",
-        CoreGNodeRole000.AtomicTNode: "d9823442",
-        CoreGNodeRole000.MarketMaker: "86f21dd2",
-        CoreGNodeRole000.AtomicMeteringNode: "9521af06",
-        CoreGNodeRole000.ConductorTopologyNode: "4502e355",
-        CoreGNodeRole000.InterconnectionComponent: "d67e564e",
-        CoreGNodeRole000.Scada: "7a8e4046",
+    versioned_enum_to_type_dict: Dict[RecognizedCurrencyUnit000, str] = {
+        RecognizedCurrencyUnit000.UNKNOWN: "00000000",
+        RecognizedCurrencyUnit000.USD: "e57c5143",
+        RecognizedCurrencyUnit000.GBP: "f7b38fc5",
     }
 
 
-class GNodeStatus100SchemaEnum:
-    enum_name: str = "g.node.status.100"
+class RecognizedTemperatureUnit000SchemaEnum:
+    enum_name: str = "recognized.temperature.unit.000"
     symbols: List[str] = [
         "00000000",
-        "153d3475",
-        "a2cfc2f7",
-        "839b38db",
-        "f5831e1d",
+        "6f16ee63",
     ]
 
     @classmethod
     def is_symbol(cls, candidate: str) -> bool:
         if candidate in cls.symbols:
             return True
         return False
 
 
-class GNodeStatus100(StrEnum):
-    Unknown = auto()
-    Pending = auto()
-    Active = auto()
-    PermanentlyDeactivated = auto()
-    Suspended = auto()
+class RecognizedTemperatureUnit000(StrEnum):
+    C = auto()
+    F = auto()
 
     @classmethod
-    def default(cls) -> "GNodeStatus100":
-        return cls.Unknown
+    def default(cls) -> "RecognizedTemperatureUnit000":
+        return cls.C
 
     @classmethod
     def values(cls) -> List[str]:
         return [elt.value for elt in cls]
 
 
-class GNodeStatusMap:
+class RecognizedTemperatureUnitMap:
     @classmethod
-    def type_to_local(cls, symbol: str) -> GNodeStatus:
-        if not GNodeStatus100SchemaEnum.is_symbol(symbol):
-            raise SchemaError(f"{symbol} must belong to GNodeStatus100 symbols")
+    def type_to_local(cls, symbol: str) -> RecognizedTemperatureUnit:
+        if not RecognizedTemperatureUnit000SchemaEnum.is_symbol(symbol):
+            raise SchemaError(
+                f"{symbol} must belong to RecognizedTemperatureUnit000 symbols"
+            )
         versioned_enum = cls.type_to_versioned_enum_dict[symbol]
-        return as_enum(versioned_enum, GNodeStatus, GNodeStatus.default())
+        return as_enum(
+            versioned_enum,
+            RecognizedTemperatureUnit,
+            RecognizedTemperatureUnit.default(),
+        )
 
     @classmethod
-    def local_to_type(cls, g_node_status: GNodeStatus) -> str:
-        if not isinstance(g_node_status, GNodeStatus):
-            raise SchemaError(f"{g_node_status} must be of type {GNodeStatus}")
+    def local_to_type(
+        cls, recognized_temperature_unit: RecognizedTemperatureUnit
+    ) -> str:
+        if not isinstance(recognized_temperature_unit, RecognizedTemperatureUnit):
+            raise SchemaError(
+                f"{recognized_temperature_unit} must be of type {RecognizedTemperatureUnit}"
+            )
         versioned_enum = as_enum(
-            g_node_status, GNodeStatus100, GNodeStatus100.default()
+            recognized_temperature_unit,
+            RecognizedTemperatureUnit000,
+            RecognizedTemperatureUnit000.default(),
         )
         return cls.versioned_enum_to_type_dict[versioned_enum]
 
-    type_to_versioned_enum_dict: Dict[str, GNodeStatus100] = {
-        "00000000": GNodeStatus100.Unknown,
-        "153d3475": GNodeStatus100.Pending,
-        "a2cfc2f7": GNodeStatus100.Active,
-        "839b38db": GNodeStatus100.PermanentlyDeactivated,
-        "f5831e1d": GNodeStatus100.Suspended,
+    type_to_versioned_enum_dict: Dict[str, RecognizedTemperatureUnit000] = {
+        "00000000": RecognizedTemperatureUnit000.C,
+        "6f16ee63": RecognizedTemperatureUnit000.F,
     }
 
-    versioned_enum_to_type_dict: Dict[GNodeStatus100, str] = {
-        GNodeStatus100.Unknown: "00000000",
-        GNodeStatus100.Pending: "153d3475",
-        GNodeStatus100.Active: "a2cfc2f7",
-        GNodeStatus100.PermanentlyDeactivated: "839b38db",
-        GNodeStatus100.Suspended: "f5831e1d",
+    versioned_enum_to_type_dict: Dict[RecognizedTemperatureUnit000, str] = {
+        RecognizedTemperatureUnit000.C: "00000000",
+        RecognizedTemperatureUnit000.F: "6f16ee63",
     }
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
@@ -217,398 +204,464 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-def check_is_algo_address_string_format(v: str) -> None:
-    """
-    AlgoAddressStringFormat format: The public key of a private/public Ed25519
-    key pair, transformed into an  Algorand address, by adding a 4-byte checksum
-    to the end of the public key and then encoding in base32.
-
-    Raises:
-        ValueError: if not AlgoAddressStringFormat format
-    """
-    import algosdk
-
-    at = algosdk.abi.AddressType()
-    try:
-        result = at.decode(at.encode(v))
-    except Exception as e:
-        raise ValueError(f"Not AlgoAddressStringFormat: {e}")
-
-
-class BaseGNodeGt(BaseModel):
+class FloParamsBrickstorageheater(BaseModel):
     """.
 
-    BaseGNode. Authority is GNodeFactory.
+    FloParams for the BrickStorageHeater AtomicTNode strategy.
+    [More info](https://gridworks-atn.readthedocs.io/en/latest/brick-storage-heater.html).
     """
 
-    GNodeId: str = Field(
-        title="GNodeId",
-    )
-    Alias: str = Field(
-        title="Alias",
-    )
-    Status: GNodeStatus = Field(
-        title="Status",
-    )
-    Role: CoreGNodeRole = Field(
-        title="Role",
-    )
-    GNodeRegistryAddr: str = Field(
-        title="GNodeRegistryAddr",
-    )
-    PrevAlias: Optional[str] = Field(
-        title="PrevAlias",
-        default=None,
-    )
-    GpsPointId: Optional[str] = Field(
-        title="GpsPointId",
-        default=None,
-    )
-    OwnershipDeedId: Optional[int] = Field(
-        title="OwnershipDeedId",
-        default=None,
+    MaxBrickTempC: int = Field(
+        title="MaxBrickTempC",
+        default=190,
+    )
+    RatedMaxPowerKw: float = Field(
+        title="RatedMaxPowerKw",
+        default=13.5,
+    )
+    ROff: float = Field(
+        title="ROff",
+        default=0.08,
+    )
+    ROn: float = Field(
+        title="ROn",
+        default=0.15,
+    )
+    RoomTempF: int = Field(
+        title="RoomTempF",
+        default=70,
+    )
+    CurrencyUnit: RecognizedCurrencyUnit = Field(
+        title="CurrencyUnit",
+        default=RecognizedCurrencyUnit.USD,
+    )
+    TempUnit: RecognizedTemperatureUnit = Field(
+        title="TempUnit",
+        default=RecognizedTemperatureUnit.F,
+    )
+    TimezoneString: str = Field(
+        title="TimezoneString",
+        default="US/Eastern",
+    )
+    HomeCity: str = Field(
+        title="HomeCity",
+        default="MILLINOCKET_ME",
+    )
+    IsRegulating: bool = Field(
+        title="IsRegulating",
+        default=False,
+    )
+    StorageSteps: int = Field(
+        title="StorageSteps",
+        default=100,
+    )
+    SliceDurationMinutes: List[int] = Field(
+        title="SliceDurationMinutes",
+        default=[60],
+    )
+    PowerRequiredByHouseFromSystemAvgKwList: List[float] = Field(
+        title="PowerRequiredByHouseFromSystemAvgKwList",
+        default=[3.42],
+    )
+    C: Optional[float] = Field(
+        title="C",
+        default=200,
+    )
+    RealtimeElectricityPrice: List[float] = Field(
+        title="RealtimeElectricityPrice",
+        default=[10.35],
+    )
+    OutsideTempF: List[float] = Field(
+        title="OutsideTempF",
+        default=[-5.1],
+    )
+    DistributionPrice: List[float] = Field(
+        title="DistributionPrice",
+        default=[40.0],
+    )
+    RtElecPriceUid: str = Field(
+        title="RtElecPriceUid",
+    )
+    RegulationPrice: List[float] = Field(
+        title="RegulationPrice",
+        default=[25.3],
     )
-    OwnershipDeedValidatorAddr: Optional[str] = Field(
-        title="OwnershipDeedValidatorAddr",
-        default=None,
-    )
-    OwnerAddr: Optional[str] = Field(
-        title="OwnerAddr",
-        default=None,
-    )
-    DaemonAddr: Optional[str] = Field(
-        title="DaemonAddr",
-        default=None,
+    WeatherUid: str = Field(
+        title="WeatherUid",
     )
-    TradingRightsId: Optional[int] = Field(
-        title="TradingRightsId",
+    DistPriceUid: Optional[str] = Field(
+        title="DistPriceUid",
         default=None,
     )
-    ScadaAlgoAddr: Optional[str] = Field(
-        title="ScadaAlgoAddr",
+    RegPriceUid: Optional[str] = Field(
+        title="RegPriceUid",
         default=None,
     )
-    ScadaCertId: Optional[int] = Field(
-        title="ScadaCertId",
-        default=None,
-    )
-    TypeName: Literal["base.g.node.gt"] = "base.g.node.gt"
-    Version: str = "002"
+    StartYearUtc: int = Field(
+        title="StartYearUtc",
+        default=2020,
+    )
+    StartMonthUtc: int = Field(
+        title="StartMonthUtc",
+        default=1,
+    )
+    StartDayUtc: int = Field(
+        title="StartDayUtc",
+        default=1,
+    )
+    StartHourUtc: int = Field(
+        title="StartHourUtc",
+        default=0,
+    )
+    StartMinuteUtc: int = Field(
+        title="StartMinuteUtc",
+        default=0,
+    )
+    StartingStoreIdx: int = Field(
+        title="StartingStoreIdx",
+        default=50,
+    )
+    AmbientPowerInKw: float = Field(
+        title="AmbientPowerInKw",
+        default=1.25,
+    )
+    HouseWorstCaseTempF: int = Field(
+        title="HouseWorstCaseTempF",
+        default=-7,
+    )
+    GNodeAlias: str = Field(
+        title="GNodeAlias",
+    )
+    FloParamsUid: str = Field(
+        title="FloParamsUid",
+    )
+    TypeName: Literal["flo.params.brickstorageheater"] = "flo.params.brickstorageheater"
+    Version: str = "000"
+
+    @validator("CurrencyUnit")
+    def _check_currency_unit(cls, v: RecognizedCurrencyUnit) -> RecognizedCurrencyUnit:
+        return as_enum(v, RecognizedCurrencyUnit, RecognizedCurrencyUnit.UNKNOWN)
+
+    @validator("TempUnit")
+    def _check_temp_unit(
+        cls, v: RecognizedTemperatureUnit
+    ) -> RecognizedTemperatureUnit:
+        return as_enum(v, RecognizedTemperatureUnit, RecognizedTemperatureUnit.C)
 
-    @validator("GNodeId")
-    def _check_g_node_id(cls, v: str) -> str:
+    @validator("RtElecPriceUid")
+    def _check_rt_elec_price_uid(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"GNodeId failed UuidCanonicalTextual format validation: {e}"
-            )
-        return v
-
-    @validator("Alias")
-    def _check_alias(cls, v: str) -> str:
-        try:
-            check_is_left_right_dot(v)
-        except ValueError as e:
-            raise ValueError(f"Alias failed LeftRightDot format validation: {e}")
-        return v
-
-    @validator("Status")
-    def _check_status(cls, v: GNodeStatus) -> GNodeStatus:
-        return as_enum(v, GNodeStatus, GNodeStatus.Unknown)
-
-    @validator("Role")
-    def _check_role(cls, v: CoreGNodeRole) -> CoreGNodeRole:
-        return as_enum(v, CoreGNodeRole, CoreGNodeRole.Other)
-
-    @validator("GNodeRegistryAddr")
-    def _check_g_node_registry_addr(cls, v: str) -> str:
-        try:
-            check_is_algo_address_string_format(v)
-        except ValueError as e:
-            raise ValueError(
-                f"GNodeRegistryAddr failed AlgoAddressStringFormat format validation: {e}"
+                f"RtElecPriceUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("PrevAlias")
-    def _check_prev_alias(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
-        try:
-            check_is_left_right_dot(v)
-        except ValueError as e:
-            raise ValueError(f"PrevAlias failed LeftRightDot format validation: {e}")
-        return v
-
-    @validator("GpsPointId")
-    def _check_gps_point_id(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
+    @validator("WeatherUid")
+    def _check_weather_uid(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"GpsPointId failed UuidCanonicalTextual format validation: {e}"
+                f"WeatherUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("OwnershipDeedValidatorAddr")
-    def _check_ownership_deed_validator_addr(cls, v: Optional[str]) -> Optional[str]:
+    @validator("DistPriceUid")
+    def _check_dist_price_uid(cls, v: Optional[str]) -> Optional[str]:
         if v is None:
             return v
         try:
-            check_is_algo_address_string_format(v)
+            check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"OwnershipDeedValidatorAddr failed AlgoAddressStringFormat format validation: {e}"
+                f"DistPriceUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("OwnerAddr")
-    def _check_owner_addr(cls, v: Optional[str]) -> Optional[str]:
+    @validator("RegPriceUid")
+    def _check_reg_price_uid(cls, v: Optional[str]) -> Optional[str]:
         if v is None:
             return v
         try:
-            check_is_algo_address_string_format(v)
+            check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"OwnerAddr failed AlgoAddressStringFormat format validation: {e}"
+                f"RegPriceUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("DaemonAddr")
-    def _check_daemon_addr(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
+    @validator("GNodeAlias")
+    def _check_g_node_alias(cls, v: str) -> str:
         try:
-            check_is_algo_address_string_format(v)
+            check_is_left_right_dot(v)
         except ValueError as e:
-            raise ValueError(
-                f"DaemonAddr failed AlgoAddressStringFormat format validation: {e}"
-            )
+            raise ValueError(f"GNodeAlias failed LeftRightDot format validation: {e}")
         return v
 
-    @validator("ScadaAlgoAddr")
-    def _check_scada_algo_addr(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
+    @validator("FloParamsUid")
+    def _check_flo_params_uid(cls, v: str) -> str:
         try:
-            check_is_algo_address_string_format(v)
+            check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"ScadaAlgoAddr failed AlgoAddressStringFormat format validation: {e}"
+                f"FloParamsUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
-        del d["Status"]
-        Status = as_enum(self.Status, GNodeStatus, GNodeStatus.default())
-        d["StatusGtEnumSymbol"] = GNodeStatusMap.local_to_type(Status)
-        del d["Role"]
-        Role = as_enum(self.Role, CoreGNodeRole, CoreGNodeRole.default())
-        d["RoleGtEnumSymbol"] = CoreGNodeRoleMap.local_to_type(Role)
-        if d["PrevAlias"] is None:
-            del d["PrevAlias"]
-        if d["GpsPointId"] is None:
-            del d["GpsPointId"]
-        if d["OwnershipDeedId"] is None:
-            del d["OwnershipDeedId"]
-        if d["OwnershipDeedValidatorAddr"] is None:
-            del d["OwnershipDeedValidatorAddr"]
-        if d["OwnerAddr"] is None:
-            del d["OwnerAddr"]
-        if d["DaemonAddr"] is None:
-            del d["DaemonAddr"]
-        if d["TradingRightsId"] is None:
-            del d["TradingRightsId"]
-        if d["ScadaAlgoAddr"] is None:
-            del d["ScadaAlgoAddr"]
-        if d["ScadaCertId"] is None:
-            del d["ScadaCertId"]
+        del d["CurrencyUnit"]
+        CurrencyUnit = as_enum(
+            self.CurrencyUnit, RecognizedCurrencyUnit, RecognizedCurrencyUnit.default()
+        )
+        d["CurrencyUnitGtEnumSymbol"] = RecognizedCurrencyUnitMap.local_to_type(
+            CurrencyUnit
+        )
+        del d["TempUnit"]
+        TempUnit = as_enum(
+            self.TempUnit,
+            RecognizedTemperatureUnit,
+            RecognizedTemperatureUnit.default(),
+        )
+        d["TempUnitGtEnumSymbol"] = RecognizedTemperatureUnitMap.local_to_type(TempUnit)
+        if d["C"] is None:
+            del d["C"]
+        if d["DistPriceUid"] is None:
+            del d["DistPriceUid"]
+        if d["RegPriceUid"] is None:
+            del d["RegPriceUid"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
-class BaseGNodeGt_Maker:
-    type_name = "base.g.node.gt"
-    version = "002"
+
+class FloParamsBrickstorageheater_Maker:
+    type_name = "flo.params.brickstorageheater"
+    version = "000"
 
     def __init__(
         self,
-        g_node_id: str,
-        alias: str,
-        status: GNodeStatus,
-        role: CoreGNodeRole,
-        g_node_registry_addr: str,
-        prev_alias: Optional[str],
-        gps_point_id: Optional[str],
-        ownership_deed_id: Optional[int],
-        ownership_deed_validator_addr: Optional[str],
-        owner_addr: Optional[str],
-        daemon_addr: Optional[str],
-        trading_rights_id: Optional[int],
-        scada_algo_addr: Optional[str],
-        scada_cert_id: Optional[int],
+        max_brick_temp_c: int,
+        rated_max_power_kw: float,
+        r_off: float,
+        r_on: float,
+        room_temp_f: int,
+        currency_unit: RecognizedCurrencyUnit,
+        temp_unit: RecognizedTemperatureUnit,
+        timezone_string: str,
+        home_city: str,
+        is_regulating: bool,
+        storage_steps: int,
+        slice_duration_minutes: List[int],
+        power_required_by_house_from_system_avg_kw_list: List[float],
+        c: Optional[float],
+        realtime_electricity_price: List[float],
+        outside_temp_f: List[float],
+        distribution_price: List[float],
+        rt_elec_price_uid: str,
+        regulation_price: List[float],
+        weather_uid: str,
+        dist_price_uid: Optional[str],
+        reg_price_uid: Optional[str],
+        start_year_utc: int,
+        start_month_utc: int,
+        start_day_utc: int,
+        start_hour_utc: int,
+        start_minute_utc: int,
+        starting_store_idx: int,
+        ambient_power_in_kw: float,
+        house_worst_case_temp_f: int,
+        g_node_alias: str,
+        flo_params_uid: str,
     ):
-        self.tuple = BaseGNodeGt(
-            GNodeId=g_node_id,
-            Alias=alias,
-            Status=status,
-            Role=role,
-            GNodeRegistryAddr=g_node_registry_addr,
-            PrevAlias=prev_alias,
-            GpsPointId=gps_point_id,
-            OwnershipDeedId=ownership_deed_id,
-            OwnershipDeedValidatorAddr=ownership_deed_validator_addr,
-            OwnerAddr=owner_addr,
-            DaemonAddr=daemon_addr,
-            TradingRightsId=trading_rights_id,
-            ScadaAlgoAddr=scada_algo_addr,
-            ScadaCertId=scada_cert_id,
+        self.tuple = FloParamsBrickstorageheater(
+            MaxBrickTempC=max_brick_temp_c,
+            RatedMaxPowerKw=rated_max_power_kw,
+            ROff=r_off,
+            ROn=r_on,
+            RoomTempF=room_temp_f,
+            CurrencyUnit=currency_unit,
+            TempUnit=temp_unit,
+            TimezoneString=timezone_string,
+            HomeCity=home_city,
+            IsRegulating=is_regulating,
+            StorageSteps=storage_steps,
+            SliceDurationMinutes=slice_duration_minutes,
+            PowerRequiredByHouseFromSystemAvgKwList=power_required_by_house_from_system_avg_kw_list,
+            C=c,
+            RealtimeElectricityPrice=realtime_electricity_price,
+            OutsideTempF=outside_temp_f,
+            DistributionPrice=distribution_price,
+            RtElecPriceUid=rt_elec_price_uid,
+            RegulationPrice=regulation_price,
+            WeatherUid=weather_uid,
+            DistPriceUid=dist_price_uid,
+            RegPriceUid=reg_price_uid,
+            StartYearUtc=start_year_utc,
+            StartMonthUtc=start_month_utc,
+            StartDayUtc=start_day_utc,
+            StartHourUtc=start_hour_utc,
+            StartMinuteUtc=start_minute_utc,
+            StartingStoreIdx=starting_store_idx,
+            AmbientPowerInKw=ambient_power_in_kw,
+            HouseWorstCaseTempF=house_worst_case_temp_f,
+            GNodeAlias=g_node_alias,
+            FloParamsUid=flo_params_uid,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: BaseGNodeGt) -> str:
+    def tuple_to_type(cls, tuple: FloParamsBrickstorageheater) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> BaseGNodeGt:
+    def type_to_tuple(cls, t: str) -> FloParamsBrickstorageheater:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> BaseGNodeGt:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> FloParamsBrickstorageheater:
         d2 = dict(d)
-        if "GNodeId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing GNodeId")
-        if "Alias" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing Alias")
-        if "StatusGtEnumSymbol" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StatusGtEnumSymbol")
-        if d2["StatusGtEnumSymbol"] in GNodeStatus100SchemaEnum.symbols:
-            d2["Status"] = GNodeStatusMap.type_to_local(d2["StatusGtEnumSymbol"])
+        if "MaxBrickTempC" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing MaxBrickTempC")
+        if "RatedMaxPowerKw" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing RatedMaxPowerKw")
+        if "ROff" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing ROff")
+        if "ROn" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing ROn")
+        if "RoomTempF" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing RoomTempF")
+        if "CurrencyUnitGtEnumSymbol" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing CurrencyUnitGtEnumSymbol")
+        if (
+            d2["CurrencyUnitGtEnumSymbol"]
+            in RecognizedCurrencyUnit000SchemaEnum.symbols
+        ):
+            d2["CurrencyUnit"] = RecognizedCurrencyUnitMap.type_to_local(
+                d2["CurrencyUnitGtEnumSymbol"]
+            )
         else:
-            d2["Status"] = GNodeStatus.default()
-        if "RoleGtEnumSymbol" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing RoleGtEnumSymbol")
-        if d2["RoleGtEnumSymbol"] in CoreGNodeRole000SchemaEnum.symbols:
-            d2["Role"] = CoreGNodeRoleMap.type_to_local(d2["RoleGtEnumSymbol"])
+            d2["CurrencyUnit"] = RecognizedCurrencyUnit.default()
+        if "TempUnitGtEnumSymbol" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TempUnitGtEnumSymbol")
+        if d2["TempUnitGtEnumSymbol"] in RecognizedTemperatureUnit000SchemaEnum.symbols:
+            d2["TempUnit"] = RecognizedTemperatureUnitMap.type_to_local(
+                d2["TempUnitGtEnumSymbol"]
+            )
         else:
-            d2["Role"] = CoreGNodeRole.default()
-        if "GNodeRegistryAddr" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing GNodeRegistryAddr")
-        if "PrevAlias" not in d2.keys():
-            d2["PrevAlias"] = None
-        if "GpsPointId" not in d2.keys():
-            d2["GpsPointId"] = None
-        if "OwnershipDeedId" not in d2.keys():
-            d2["OwnershipDeedId"] = None
-        if "OwnershipDeedValidatorAddr" not in d2.keys():
-            d2["OwnershipDeedValidatorAddr"] = None
-        if "OwnerAddr" not in d2.keys():
-            d2["OwnerAddr"] = None
-        if "DaemonAddr" not in d2.keys():
-            d2["DaemonAddr"] = None
-        if "TradingRightsId" not in d2.keys():
-            d2["TradingRightsId"] = None
-        if "ScadaAlgoAddr" not in d2.keys():
-            d2["ScadaAlgoAddr"] = None
-        if "ScadaCertId" not in d2.keys():
-            d2["ScadaCertId"] = None
+            d2["TempUnit"] = RecognizedTemperatureUnit.default()
+        if "TimezoneString" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TimezoneString")
+        if "HomeCity" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing HomeCity")
+        if "IsRegulating" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing IsRegulating")
+        if "StorageSteps" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StorageSteps")
+        if "SliceDurationMinutes" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing SliceDurationMinutes")
+        if "PowerRequiredByHouseFromSystemAvgKwList" not in d2.keys():
+            raise SchemaError(
+                f"dict {d2} missing PowerRequiredByHouseFromSystemAvgKwList"
+            )
+        if "C" not in d2.keys():
+            d2["C"] = None
+        if "RealtimeElectricityPrice" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing RealtimeElectricityPrice")
+        if "OutsideTempF" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing OutsideTempF")
+        if "DistributionPrice" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing DistributionPrice")
+        if "RtElecPriceUid" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing RtElecPriceUid")
+        if "RegulationPrice" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing RegulationPrice")
+        if "WeatherUid" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing WeatherUid")
+        if "DistPriceUid" not in d2.keys():
+            d2["DistPriceUid"] = None
+        if "RegPriceUid" not in d2.keys():
+            d2["RegPriceUid"] = None
+        if "StartYearUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartYearUtc")
+        if "StartMonthUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartMonthUtc")
+        if "StartDayUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartDayUtc")
+        if "StartHourUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartHourUtc")
+        if "StartMinuteUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartMinuteUtc")
+        if "StartingStoreIdx" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartingStoreIdx")
+        if "AmbientPowerInKw" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing AmbientPowerInKw")
+        if "HouseWorstCaseTempF" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing HouseWorstCaseTempF")
+        if "GNodeAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing GNodeAlias")
+        if "FloParamsUid" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FloParamsUid")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return BaseGNodeGt(
-            GNodeId=d2["GNodeId"],
-            Alias=d2["Alias"],
-            Status=d2["Status"],
-            Role=d2["Role"],
-            GNodeRegistryAddr=d2["GNodeRegistryAddr"],
-            PrevAlias=d2["PrevAlias"],
-            GpsPointId=d2["GpsPointId"],
-            OwnershipDeedId=d2["OwnershipDeedId"],
-            OwnershipDeedValidatorAddr=d2["OwnershipDeedValidatorAddr"],
-            OwnerAddr=d2["OwnerAddr"],
-            DaemonAddr=d2["DaemonAddr"],
-            TradingRightsId=d2["TradingRightsId"],
-            ScadaAlgoAddr=d2["ScadaAlgoAddr"],
-            ScadaCertId=d2["ScadaCertId"],
+        return FloParamsBrickstorageheater(
+            MaxBrickTempC=d2["MaxBrickTempC"],
+            RatedMaxPowerKw=d2["RatedMaxPowerKw"],
+            ROff=d2["ROff"],
+            ROn=d2["ROn"],
+            RoomTempF=d2["RoomTempF"],
+            CurrencyUnit=d2["CurrencyUnit"],
+            TempUnit=d2["TempUnit"],
+            TimezoneString=d2["TimezoneString"],
+            HomeCity=d2["HomeCity"],
+            IsRegulating=d2["IsRegulating"],
+            StorageSteps=d2["StorageSteps"],
+            SliceDurationMinutes=d2["SliceDurationMinutes"],
+            PowerRequiredByHouseFromSystemAvgKwList=d2[
+                "PowerRequiredByHouseFromSystemAvgKwList"
+            ],
+            C=d2["C"],
+            RealtimeElectricityPrice=d2["RealtimeElectricityPrice"],
+            OutsideTempF=d2["OutsideTempF"],
+            DistributionPrice=d2["DistributionPrice"],
+            RtElecPriceUid=d2["RtElecPriceUid"],
+            RegulationPrice=d2["RegulationPrice"],
+            WeatherUid=d2["WeatherUid"],
+            DistPriceUid=d2["DistPriceUid"],
+            RegPriceUid=d2["RegPriceUid"],
+            StartYearUtc=d2["StartYearUtc"],
+            StartMonthUtc=d2["StartMonthUtc"],
+            StartDayUtc=d2["StartDayUtc"],
+            StartHourUtc=d2["StartHourUtc"],
+            StartMinuteUtc=d2["StartMinuteUtc"],
+            StartingStoreIdx=d2["StartingStoreIdx"],
+            AmbientPowerInKw=d2["AmbientPowerInKw"],
+            HouseWorstCaseTempF=d2["HouseWorstCaseTempF"],
+            GNodeAlias=d2["GNodeAlias"],
+            FloParamsUid=d2["FloParamsUid"],
             TypeName=d2["TypeName"],
-            Version="002",
+            Version="000",
         )
-
-    @classmethod
-    def tuple_to_dc(cls, t: BaseGNodeGt) -> BaseGNode:
-        if t.GNodeId in BaseGNode.by_id.keys():
-            dc = BaseGNode.by_id[t.GNodeId]
-        else:
-            dc = BaseGNode(
-                g_node_id=t.GNodeId,
-                alias=t.Alias,
-                status=t.Status,
-                role=t.Role,
-                g_node_registry_addr=t.GNodeRegistryAddr,
-                prev_alias=t.PrevAlias,
-                gps_point_id=t.GpsPointId,
-                ownership_deed_id=t.OwnershipDeedId,
-                ownership_deed_validator_addr=t.OwnershipDeedValidatorAddr,
-                owner_addr=t.OwnerAddr,
-                daemon_addr=t.DaemonAddr,
-                trading_rights_id=t.TradingRightsId,
-                scada_algo_addr=t.ScadaAlgoAddr,
-                scada_cert_id=t.ScadaCertId,
-            )
-
-        return dc
-
-    @classmethod
-    def dc_to_tuple(cls, dc: BaseGNode) -> BaseGNodeGt:
-        t = BaseGNodeGt_Maker(
-            g_node_id=dc.g_node_id,
-            alias=dc.alias,
-            status=dc.status,
-            role=dc.role,
-            g_node_registry_addr=dc.g_node_registry_addr,
-            prev_alias=dc.prev_alias,
-            gps_point_id=dc.gps_point_id,
-            ownership_deed_id=dc.ownership_deed_id,
-            ownership_deed_validator_addr=dc.ownership_deed_validator_addr,
-            owner_addr=dc.owner_addr,
-            daemon_addr=dc.daemon_addr,
-            trading_rights_id=dc.trading_rights_id,
-            scada_algo_addr=dc.scada_algo_addr,
-            scada_cert_id=dc.scada_cert_id,
-        ).tuple
-        return t
-
-    @classmethod
-    def type_to_dc(cls, t: str) -> BaseGNode:
-        return cls.tuple_to_dc(cls.type_to_tuple(t))
-
-    @classmethod
-    def dc_to_type(cls, dc: BaseGNode) -> str:
-        return cls.dc_to_tuple(dc).as_type()
-
-    @classmethod
-    def dict_to_dc(cls, d: dict[Any, str]) -> BaseGNode:
-        return cls.tuple_to_dc(cls.dict_to_tuple(d))
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/basegnode_scada_create.py` & `gridworks_atn-0.3.2/src/gwatn/types/basegnode_scada_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,14 +169,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class BasegnodeScadaCreate_Maker:
     type_name = "basegnode.scada.create"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/csv_distp_sync.py` & `gridworks_atn-0.3.2/src/gwatn/types/csv_distp_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/csv_eprt_sync.py` & `gridworks_atn-0.3.2/src/gwatn/types/csv_eprt_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/csv_weather_forecast_sync.py` & `gridworks_atn-0.3.2/src/gwatn/types/csv_weather_forecast_sync.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/data_channel.py` & `gridworks_atn-0.3.2/src/gwatn/types/data_channel.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/discoverycert_algo_create.py` & `gridworks_atn-0.3.2/src/gwatn/types/discoverycert_algo_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,17 @@
         if d["MicroLon"] is None:
             del d["MicroLon"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class DiscoverycertAlgoCreate_Maker:
     type_name = "discoverycert.algo.create"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/dispatch_contract_confirmed_heatpumpwithbooststore.py` & `gridworks_atn-0.3.2/src/gwatn/types/dispatch_contract_confirmed.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-"""Type dispatch.contract.confirmed.heatpumpwithbooststore, version 000"""
+"""Type dispatch.contract.confirmed, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
+from pydantic import root_validator
 from pydantic import validator
 
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore,
-)
-from gwatn.types.atn_params_heatpumpwithbooststore import (
-    AtnParamsHeatpumpwithbooststore_Maker,
-)
+from gwatn.types.atn_params import AtnParams
+from gwatn.types.atn_params import AtnParams_Maker
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
 
@@ -85,15 +82,15 @@
 
     try:
         algosdk.encoding.future_msgpack_decode(v)
     except Exception as e:
         raise ValueError(f"Not AlgoMsgPackEncoded format: {e}")
 
 
-class DispatchContractConfirmedHeatpumpwithbooststore(BaseModel):
+class DispatchContractConfirmed(BaseModel):
     """Message sent from AtomicTNode back to SCADA via Rabbit .
 
     Paired with join.dispatch.contract. Sent from AtomicTNode back to SCADA
     once the AtomicTNode has successfully finished bootstrapping the Dispatch
     Contract and opted in. Once it has done this, the Dispatch Contract is ready
      to collect audit information about heartbeats, dispatch, energy and power.
 
@@ -102,23 +99,24 @@
 
     FromGNodeAlias: str = Field(
         title="FromGNodeAlias",
     )
     FromGNodeInstanceId: str = Field(
         title="FromGNodeInstanceId",
     )
+    AtnParamsTypeName: str = Field(
+        title="AtnParamsTypeName",
+    )
     SignedProof: str = Field(
         title="SignedProof",
     )
-    AtnParams: AtnParamsHeatpumpwithbooststore = Field(
-        title="AtnParams",
+    Params: AtnParams = Field(
+        title="Params",
     )
-    TypeName: Literal[
-        "dispatch.contract.confirmed.heatpumpwithbooststore"
-    ] = "dispatch.contract.confirmed.heatpumpwithbooststore"
+    TypeName: Literal["dispatch.contract.confirmed"] = "dispatch.contract.confirmed"
     Version: str = "000"
 
     @validator("FromGNodeAlias")
     def _check_from_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
@@ -133,99 +131,118 @@
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
                 f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
+    @validator("AtnParamsTypeName")
+    def _check_atn_params_type_name(cls, v: str) -> str:
+        try:
+            check_is_left_right_dot(v)
+        except ValueError as e:
+            raise ValueError(
+                f"AtnParamsTypeName failed LeftRightDot format validation: {e}"
+            )
+        return v
+
     @validator("SignedProof")
     def _check_signed_proof(cls, v: str) -> str:
         try:
             check_is_algo_msg_pack_encoded(v)
         except ValueError as e:
             raise ValueError(
                 f"SignedProof failed AlgoMsgPackEncoded format validation: {e}"
             )
         return v
 
+    @root_validator
+    def check_axiom_1(cls, v: dict) -> dict:
+        """
+        Axiom 1: AtnParamsTypeName matches AtnParams.
+        AtnParams must have
+        """
+        # TODO: Implement check for axiom 1"
+        return v
+
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
-        d["AtnParams"] = self.AtnParams.as_dict()
+        d["Params"] = self.Params.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
 
-class DispatchContractConfirmedHeatpumpwithbooststore_Maker:
-    type_name = "dispatch.contract.confirmed.heatpumpwithbooststore"
+
+class DispatchContractConfirmed_Maker:
+    type_name = "dispatch.contract.confirmed"
     version = "000"
 
     def __init__(
         self,
         from_g_node_alias: str,
         from_g_node_instance_id: str,
+        atn_params_type_name: str,
         signed_proof: str,
-        atn_params: AtnParamsHeatpumpwithbooststore,
+        params: AtnParams,
     ):
-        self.tuple = DispatchContractConfirmedHeatpumpwithbooststore(
+        self.tuple = DispatchContractConfirmed(
             FromGNodeAlias=from_g_node_alias,
             FromGNodeInstanceId=from_g_node_instance_id,
+            AtnParamsTypeName=atn_params_type_name,
             SignedProof=signed_proof,
-            AtnParams=atn_params,
+            Params=params,
             #
         )
 
     @classmethod
-    def tuple_to_type(
-        cls, tuple: DispatchContractConfirmedHeatpumpwithbooststore
-    ) -> str:
+    def tuple_to_type(cls, tuple: DispatchContractConfirmed) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> DispatchContractConfirmedHeatpumpwithbooststore:
+    def type_to_tuple(cls, t: str) -> DispatchContractConfirmed:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(
-        cls, d: dict[str, Any]
-    ) -> DispatchContractConfirmedHeatpumpwithbooststore:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> DispatchContractConfirmed:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
+        if "AtnParamsTypeName" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing AtnParamsTypeName")
         if "SignedProof" not in d2.keys():
             raise SchemaError(f"dict {d2} missing SignedProof")
-        if "AtnParams" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing AtnParams")
-        if not isinstance(d2["AtnParams"], dict):
-            raise SchemaError(
-                f"d['AtnParams'] {d2['AtnParams']} must be a AtnParamsHeatpumpwithbooststore!"
-            )
-        atn_params = AtnParamsHeatpumpwithbooststore_Maker.dict_to_tuple(
-            d2["AtnParams"]
-        )
-        d2["AtnParams"] = atn_params
+        if "Params" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing Params")
+        if not isinstance(d2["Params"], dict):
+            raise SchemaError(f"d['Params'] {d2['Params']} must be a AtnParams!")
+        params = AtnParams_Maker.dict_to_tuple(d2["Params"])
+        d2["Params"] = params
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return DispatchContractConfirmedHeatpumpwithbooststore(
+        return DispatchContractConfirmed(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
+            AtnParamsTypeName=d2["AtnParamsTypeName"],
             SignedProof=d2["SignedProof"],
-            AtnParams=d2["AtnParams"],
+            Params=d2["Params"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/gt_dispatch_boolean.py` & `gridworks_atn-0.3.2/src/gwatn/types/gt_dispatch_boolean.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,14 +161,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class GtDispatchBoolean_Maker:
     type_name = "gt.dispatch.boolean"
     version = "110"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_a.py` & `gridworks_atn-0.3.2/src/gwatn/types/simplesim_driver_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,118 +1,123 @@
-"""Type heartbeat.a, version 100"""
+"""Type simplesim.driver.data, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
+from pydantic import Extra
 from pydantic import Field
 from pydantic import validator
 
 
-def check_is_hex_char(v: str) -> None:
+def check_is_left_right_dot(v: str) -> None:
     """
-    HexChar format: single-char string in '0123456789abcdefABCDEF'
+    LeftRightDot format: Lowercase alphanumeric words separated by periods,
+    most significant word (on the left) starting with an alphabet character.
 
     Raises:
-        ValueError: if not HexChar format
+        ValueError: if not LeftRightDot format
     """
-    if not isinstance(v, str):
-        raise ValueError(f"{v} must be a hex char, but not even a string")
-    if len(v) > 1:
-        raise ValueError(f"{v} must be a hex char, but not of len 1")
-    if v not in "0123456789abcdefABCDEF":
-        raise ValueError(f"{v} must be one of '0123456789abcdefABCDEF'")
+    from typing import List
 
+    try:
+        x: List[str] = v.split(".")
+    except:
+        raise ValueError(f"Failed to seperate {v} into words with split'.'")
+    first_word = x[0]
+    first_char = first_word[0]
+    if not first_char.isalpha():
+        raise ValueError(f"Most significant word of {v} must start with alphabet char.")
+    for word in x:
+        if not word.isalnum():
+            raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
+    if not v.islower():
+        raise ValueError(f"All characters of {v} must be lowercase.")
 
-class HeartbeatA(BaseModel):
-    """Used to check that an actor can both send and receive messages.
 
-    Payload for direct messages sent back and forth between actors,
-    for example a Supervisor and one of its subordinates.
+class SimplesimDriverData(BaseModel):
+    """Generic driver report for a simple Scada Simulation"""
 
-    [More info](https://gridworks.readthedocs.io/en/latest/g-node-instance.html).
-    """
-
-    MyHex: str = Field(
-        title="Hex character getting sent",
-        default="0",
+    FromGNodeAlias: str = Field(
+        title="FromGNodeAlias",
     )
-    YourLastHex: str = Field(
-        title="Last hex character received from heartbeat partner",
-        default="0",
+    TypeName: str = Field(
+        title="TypeName",
+        default="simplesim.driver.data",
     )
-    TypeName: Literal["heartbeat.a"] = "heartbeat.a"
-    Version: str = "100"
+    Version: str = "000"
 
-    @validator("MyHex")
-    def _check_my_hex(cls, v: str) -> str:
-        try:
-            check_is_hex_char(v)
-        except ValueError as e:
-            raise ValueError(f"MyHex failed HexChar format validation: {e}")
+    class Config:
+        extra = Extra.allow
+
+    @validator("TypeName")
+    def _check_type_name(cls, v: str) -> str:
+        if not v.startswith("simplesim.driver.data"):
+            raise ValueError(f"TypeName {v} must start with 'simplesim.driver.data'")
         return v
 
-    @validator("YourLastHex")
-    def _check_your_last_hex(cls, v: str) -> str:
+    @validator("FromGNodeAlias")
+    def _check_from_g_node_alias(cls, v: str) -> str:
         try:
-            check_is_hex_char(v)
+            check_is_left_right_dot(v)
         except ValueError as e:
-            raise ValueError(f"YourLastHex failed HexChar format validation: {e}")
+            raise ValueError(
+                f"FromGNodeAlias failed LeftRightDot format validation: {e}"
+            )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
+
+class SimplesimDriverData_Maker:
+    type_name = "simplesim.driver.data"
+    version = "000"
 
-class HeartbeatA_Maker:
-    type_name = "heartbeat.a"
-    version = "100"
-
-    def __init__(self, my_hex: str, your_last_hex: str):
-        self.tuple = HeartbeatA(
-            MyHex=my_hex,
-            YourLastHex=your_last_hex,
+    def __init__(self, from_g_node_alias: str):
+        self.tuple = SimplesimDriverData(
+            FromGNodeAlias=from_g_node_alias,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: HeartbeatA) -> str:
+    def tuple_to_type(cls, tuple: SimplesimDriverData) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> HeartbeatA:
+    def type_to_tuple(cls, t: str) -> SimplesimDriverData:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> HeartbeatA:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> SimplesimDriverData:
         d2 = dict(d)
-        if "MyHex" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing MyHex")
-        if "YourLastHex" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing YourLastHex")
+        if "FromGNodeAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return HeartbeatA(
-            MyHex=d2["MyHex"],
-            YourLastHex=d2["YourLastHex"],
+        return SimplesimDriverData(
+            FromGNodeAlias=d2["FromGNodeAlias"],
             TypeName=d2["TypeName"],
-            Version="100",
+            Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_algo_audit.py` & `gridworks_atn-0.3.2/src/gwatn/types/old_tadeed_algo_return.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,35 @@
-"""Type heartbeat.algo.audit, version 000"""
+"""Type old.tadeed.algo.return, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwatn.types.heartbeat_b import HeartbeatB
-from gwatn.types.heartbeat_b import HeartbeatB_Maker
 
-
-def check_is_left_right_dot(v: str) -> None:
+def check_is_algo_address_string_format(v: str) -> None:
     """
-    LeftRightDot format: Lowercase alphanumeric words separated by periods,
-    most significant word (on the left) starting with an alphabet character.
+    AlgoAddressStringFormat format: The public key of a private/public Ed25519
+    key pair, transformed into an  Algorand address, by adding a 4-byte checksum
+    to the end of the public key and then encoding in base32.
 
     Raises:
-        ValueError: if not LeftRightDot format
+        ValueError: if not AlgoAddressStringFormat format
     """
-    from typing import List
+    import algosdk
 
+    at = algosdk.abi.AddressType()
     try:
-        x: List[str] = v.split(".")
-    except:
-        raise ValueError(f"Failed to seperate {v} into words with split'.'")
-    first_word = x[0]
-    first_char = first_word[0]
-    if not first_char.isalpha():
-        raise ValueError(f"Most significant word of {v} must start with alphabet char.")
-    for word in x:
-        if not word.isalnum():
-            raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
-    if not v.islower():
-        raise ValueError(f"All characters of {v} must be lowercase.")
+        result = at.decode(at.encode(v))
+    except Exception as e:
+        raise ValueError(f"Not AlgoAddressStringFormat: {e}")
 
 
 def check_is_algo_msg_pack_encoded(v: str) -> None:
     """
     AlgoMSgPackEncoded format: the format of an  transaction sent to
     the Algorand blockchain.
 
@@ -50,94 +40,124 @@
 
     try:
         algosdk.encoding.future_msgpack_decode(v)
     except Exception as e:
         raise ValueError(f"Not AlgoMsgPackEncoded format: {e}")
 
 
-class HeartbeatAlgoAudit(BaseModel):
-    """.
-
-    Algo payload with report of last HeartbeatB sent to partner via Rabbit, to be sent to
-    DispatchContract on Algo blockchain
-    """
+class OldTadeedAlgoReturn(BaseModel):
+    """ """
 
-    SignedProof: str = Field(
-        title="Tiny signed payment to DispatchContract to prove identity",
-        description="Can be a minimal payment, as long as it comes from the AtomicTNode or SCADA.",
+    OldTaDeedIdx: int = Field(
+        title="OldTaDeedIdx",
     )
-    Heartbeat: HeartbeatB = Field(
-        title="Heartbeat sender last sent to its partner",
+    TaDaemonAddr: str = Field(
+        title="TaDaemonAddr",
     )
-    TypeName: Literal["heartbeat.algo.audit"] = "heartbeat.algo.audit"
+    ValidatorAddr: str = Field(
+        title="ValidatorAddr",
+    )
+    SignedNewDeedTransferTxn: str = Field(
+        title="SignedNewDeedTransferTxn",
+    )
+    TypeName: Literal["old.tadeed.algo.return"] = "old.tadeed.algo.return"
     Version: str = "000"
 
-    @validator("SignedProof")
-    def _check_signed_proof(cls, v: str) -> str:
+    @validator("TaDaemonAddr")
+    def _check_ta_daemon_addr(cls, v: str) -> str:
+        try:
+            check_is_algo_address_string_format(v)
+        except ValueError as e:
+            raise ValueError(
+                f"TaDaemonAddr failed AlgoAddressStringFormat format validation: {e}"
+            )
+        return v
+
+    @validator("ValidatorAddr")
+    def _check_validator_addr(cls, v: str) -> str:
+        try:
+            check_is_algo_address_string_format(v)
+        except ValueError as e:
+            raise ValueError(
+                f"ValidatorAddr failed AlgoAddressStringFormat format validation: {e}"
+            )
+        return v
+
+    @validator("SignedNewDeedTransferTxn")
+    def _check_signed_new_deed_transfer_txn(cls, v: str) -> str:
         try:
             check_is_algo_msg_pack_encoded(v)
         except ValueError as e:
             raise ValueError(
-                f"SignedProof failed AlgoMsgPackEncoded format validation: {e}"
+                f"SignedNewDeedTransferTxn failed AlgoMsgPackEncoded format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
-        d["Heartbeat"] = self.Heartbeat.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
 
-class HeartbeatAlgoAudit_Maker:
-    type_name = "heartbeat.algo.audit"
+class OldTadeedAlgoReturn_Maker:
+    type_name = "old.tadeed.algo.return"
     version = "000"
 
-    def __init__(self, signed_proof: str, heartbeat: HeartbeatB):
-        self.tuple = HeartbeatAlgoAudit(
-            SignedProof=signed_proof,
-            Heartbeat=heartbeat,
+    def __init__(
+        self,
+        old_ta_deed_idx: int,
+        ta_daemon_addr: str,
+        validator_addr: str,
+        signed_new_deed_transfer_txn: str,
+    ):
+        self.tuple = OldTadeedAlgoReturn(
+            OldTaDeedIdx=old_ta_deed_idx,
+            TaDaemonAddr=ta_daemon_addr,
+            ValidatorAddr=validator_addr,
+            SignedNewDeedTransferTxn=signed_new_deed_transfer_txn,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: HeartbeatAlgoAudit) -> str:
+    def tuple_to_type(cls, tuple: OldTadeedAlgoReturn) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> HeartbeatAlgoAudit:
+    def type_to_tuple(cls, t: str) -> OldTadeedAlgoReturn:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> HeartbeatAlgoAudit:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> OldTadeedAlgoReturn:
         d2 = dict(d)
-        if "SignedProof" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing SignedProof")
-        if "Heartbeat" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing Heartbeat")
-        if not isinstance(d2["Heartbeat"], dict):
-            raise SchemaError(f"d['Heartbeat'] {d2['Heartbeat']} must be a HeartbeatB!")
-        heartbeat = HeartbeatB_Maker.dict_to_tuple(d2["Heartbeat"])
-        d2["Heartbeat"] = heartbeat
+        if "OldTaDeedIdx" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing OldTaDeedIdx")
+        if "TaDaemonAddr" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TaDaemonAddr")
+        if "ValidatorAddr" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing ValidatorAddr")
+        if "SignedNewDeedTransferTxn" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing SignedNewDeedTransferTxn")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return HeartbeatAlgoAudit(
-            SignedProof=d2["SignedProof"],
-            Heartbeat=d2["Heartbeat"],
+        return OldTadeedAlgoReturn(
+            OldTaDeedIdx=d2["OldTaDeedIdx"],
+            TaDaemonAddr=d2["TaDaemonAddr"],
+            ValidatorAddr=d2["ValidatorAddr"],
+            SignedNewDeedTransferTxn=d2["SignedNewDeedTransferTxn"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/heartbeat_b.py` & `gridworks_atn-0.3.2/src/gwatn/types/heartbeat_b.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """Type heartbeat.b, version 001"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
-from typing import Optional
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 
@@ -109,24 +108,27 @@
     FromGNodeInstanceId: str = Field(
         title="My GNodeInstanceId",
     )
     MyHex: str = Field(
         title="Hex character getting sent",
         default="0",
     )
-    YourLastHex: Optional[str] = Field(
-        title="Last hex character received from heartbeat partner. If the heartbeat initiator wants to start the sequence over, it does not include this.",
-        default=None,
+    YourLastHex: str = Field(
+        title="Last hex character received from heartbeat partner.",
     )
     LastReceivedTimeUnixMs: int = Field(
         title="Time YourLastHex was received on my clock",
     )
     SendTimeUnixMs: int = Field(
         title="Time this message is made and sent on my clock",
     )
+    StartingOver: bool = Field(
+        title="True if the heartbeat initiator wants to start the volley over",
+        description="(typically the AtomicTNode in an AtomicTNode / SCADA pair) wants to start the heartbeating volley over. The result is that its partner will not expect the initiator to know its last Hex.",
+    )
     TypeName: Literal["heartbeat.b"] = "heartbeat.b"
     Version: str = "001"
 
     @validator("FromGNodeAlias")
     def _check_from_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
@@ -151,17 +153,15 @@
         try:
             check_is_hex_char(v)
         except ValueError as e:
             raise ValueError(f"MyHex failed HexChar format validation: {e}")
         return v
 
     @validator("YourLastHex")
-    def _check_your_last_hex(cls, v: Optional[str]) -> Optional[str]:
-        if v is None:
-            return v
+    def _check_your_last_hex(cls, v: str) -> str:
         try:
             check_is_hex_char(v)
         except ValueError as e:
             raise ValueError(f"YourLastHex failed HexChar format validation: {e}")
         return v
 
     @validator("LastReceivedTimeUnixMs")
@@ -182,42 +182,45 @@
             raise ValueError(
                 f"SendTimeUnixMs failed ReasonableUnixTimeMs format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
-        if d["YourLastHex"] is None:
-            del d["YourLastHex"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class HeartbeatB_Maker:
     type_name = "heartbeat.b"
     version = "001"
 
     def __init__(
         self,
         from_g_node_alias: str,
         from_g_node_instance_id: str,
         my_hex: str,
-        your_last_hex: Optional[str],
+        your_last_hex: str,
         last_received_time_unix_ms: int,
         send_time_unix_ms: int,
+        starting_over: bool,
     ):
         self.tuple = HeartbeatB(
             FromGNodeAlias=from_g_node_alias,
             FromGNodeInstanceId=from_g_node_instance_id,
             MyHex=my_hex,
             YourLastHex=your_last_hex,
             LastReceivedTimeUnixMs=last_received_time_unix_ms,
             SendTimeUnixMs=send_time_unix_ms,
+            StartingOver=starting_over,
             #
         )
 
     @classmethod
     def tuple_to_type(cls, tuple: HeartbeatB) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
@@ -243,25 +246,28 @@
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
         if "MyHex" not in d2.keys():
             raise SchemaError(f"dict {d2} missing MyHex")
         if "YourLastHex" not in d2.keys():
-            d2["YourLastHex"] = None
+            raise SchemaError(f"dict {d2} missing YourLastHex")
         if "LastReceivedTimeUnixMs" not in d2.keys():
             raise SchemaError(f"dict {d2} missing LastReceivedTimeUnixMs")
         if "SendTimeUnixMs" not in d2.keys():
             raise SchemaError(f"dict {d2} missing SendTimeUnixMs")
+        if "StartingOver" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartingOver")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
         return HeartbeatB(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
             MyHex=d2["MyHex"],
             YourLastHex=d2["YourLastHex"],
             LastReceivedTimeUnixMs=d2["LastReceivedTimeUnixMs"],
             SendTimeUnixMs=d2["SendTimeUnixMs"],
+            StartingOver=d2["StartingOver"],
             TypeName=d2["TypeName"],
             Version="001",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_create.py` & `gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_create.py`

 * *Files 6% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     def check_axiom_1(cls, v: dict) -> dict:
         """
         Axiom 1: Is correct Multisig.
         Decoded HalfSignedDeedCreationMtx must have type MultisigTransaction from the
         2-sig MultiAccount  [GnfAdminAddr, ValidatorAddr].
         [More info](https://gridworks.readthedocs.io/en/latest/g-node-factory.html#gnfadminaddr)
         """
+        # TODO: Implement check for axiom 1"
         return v
 
     @root_validator
     def check_axiom_2(cls, v: dict) -> dict:
         """
         Axiom 2: Creates Initial ASA TaDeed.
         The transaction must create an Algorand Standard Asset
@@ -104,31 +105,36 @@
            - Manager is GnfAdminAddr
            - AssetName has the following characteristics:
                  - length <=  32 characters
                  - LeftRightDot format
                  - final word is '.ta'
         [More info](https://gridworks.readthedocs.io/en/latest/ta-deed.html#asa-tadeed-specs)
         """
+        # TODO: Implement check for axiom 2"
         return v
 
     @root_validator
     def check_axiom_3(cls, v: dict) -> dict:
         """
         Axiom 3: Mtx signed by TaValidator.
 
         """
+        # TODO: Implement check for axiom 3"
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class InitialTadeedAlgoCreate_Maker:
     type_name = "initial.tadeed.algo.create"
     version = "000"
 
     def __init__(self, validator_addr: str, half_signed_deed_creation_mtx: str):
         self.tuple = InitialTadeedAlgoCreate(
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_optin.py` & `gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_optin.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,32 +135,37 @@
 
     @root_validator(pre=True)
     def check_axiom_1(cls, v: dict) -> dict:
         """
         Axiom 1: Is correct Multisig.
         Decoded SignedInitialDaemonFundingTxn must be a SignedTransaction signed by TaOwnerAddr.
         """
+        # TODO: Implement check for axiom 1"
         return v
 
     @root_validator
     def check_axiom_2(cls, v: dict) -> dict:
         """
         Axiom 2: TaDeed consistency.
         There is an ASA TaDeed created by and owned by the 2-sig MultiAccount [GnfAdminAddr, ValidatorAddr],
         where the TaDeed's AssetName is equal to the payload's TerminalAssetAlias.
         """
+        # TODO: Implement check for axiom 2"
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class InitialTadeedAlgoOptin_Maker:
     type_name = "initial.tadeed.algo.optin"
     version = "002"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/initial_tadeed_algo_transfer.py` & `gridworks_atn-0.3.2/src/gwatn/types/initial_tadeed_algo_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,31 +139,36 @@
     def check_axiom_1(cls, v: dict) -> dict:
         """
         Axiom 1: Is correct Multisig.
         Decoded FirstDeedTransferMtx must have type MultisigTransaction from the
         2-sig MultiAccount  [GnfAdminAddr, ValidatorAddr].
         [More info](https://gridworks.readthedocs.io/en/latest/g-node-factory.html#gnfadminaddr)
         """
+        # TODO: Implement check for axiom 1"
         return v
 
     @root_validator
     def check_axiom_2(cls, v: dict) -> dict:
         """
         Axiom 2: TaDaemon funded by TaOwner.
         The TaDaemonAddr was created with funding from the TaOwnerAddr, and has sufficient funding according to the GNodeFactory.
         """
+        # TODO: Implement check for axiom 2"
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class InitialTadeedAlgoTransfer_Maker:
     type_name = "initial.tadeed.algo.transfer"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/join_dispatch_contract.py` & `gridworks_atn-0.3.2/src/gwatn/types/join_dispatch_contract.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/latest_price.py` & `gridworks_atn-0.3.2/src/gwatn/types/latest_price.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
       MarketSlot for that MarketType (i.e. divisible by 3600
       for hourly markets)
       - The middle words have LeftRightDot format (GNodeAlias
       of the MarketMaker)
     Example: rt60gate5.d1.isone.ver.keene.1673539200
 
     """
-    from gwatn.data_classes.market_type import MarketType
+    from gwatn.data_classes import MarketType
 
     try:
         x = v.split(".")
     except AttributeError:
         raise ValueError(f"{v} failed to split on '.'")
     slot_start = x[-1]
     if len(slot_start) != 10:
@@ -289,14 +289,17 @@
         if d["MessageId"] is None:
             del d["MessageId"]
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class LatestPrice_Maker:
     type_name = "latest.price"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/market_slot.py` & `gridworks_atn-0.3.2/src/gwatn/types/market_slot.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,14 +94,17 @@
         d = self.dict()
         d["Type"] = self.Type.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class MarketSlot_Maker:
     type_name = "market.slot"
     version = "000"
 
     def __init__(self, type: MarketTypeGt, market_maker_alias: str, start_unix_s: int):
         self.tuple = MarketSlot(
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/market_type_gt.py` & `gridworks_atn-0.3.2/src/gwatn/types/market_type_gt.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fastapi_utils.enums import StrEnum
 from gridworks.errors import SchemaError
 from gridworks.message import as_enum
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
-from gwatn.data_classes.market_type import MarketType
+from gwatn.data_classes import MarketType
 from gwatn.enums import MarketPriceUnit
 from gwatn.enums import MarketQuantityUnit
 from gwatn.enums import MarketTypeName
 from gwatn.enums import RecognizedCurrencyUnit
 
 
 class MarketPriceUnit000SchemaEnum:
@@ -346,14 +346,17 @@
             CurrencyUnit
         )
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class MarketTypeGt_Maker:
     type_name = "market.type.gt"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_algo_optin.py` & `gridworks_atn-0.3.2/src/gwatn/types/new_tadeed_algo_optin.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/new_tadeed_send.py` & `gridworks_atn-0.3.2/src/gwatn/types/new_tadeed_send.py`

 * *Files identical despite different names*

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/old_tadeed_algo_return.py` & `gridworks_atn-0.3.2/src/gwatn/types/terminalasset_certify_hack.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,163 +1,165 @@
-"""Type old.tadeed.algo.return, version 000"""
+"""Type terminalasset.certify.hack, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 
-def check_is_algo_address_string_format(v: str) -> None:
+def check_is_left_right_dot(v: str) -> None:
     """
-    AlgoAddressStringFormat format: The public key of a private/public Ed25519
-    key pair, transformed into an  Algorand address, by adding a 4-byte checksum
-    to the end of the public key and then encoding in base32.
+    LeftRightDot format: Lowercase alphanumeric words separated by periods,
+    most significant word (on the left) starting with an alphabet character.
 
     Raises:
-        ValueError: if not AlgoAddressStringFormat format
+        ValueError: if not LeftRightDot format
     """
-    import algosdk
+    from typing import List
 
-    at = algosdk.abi.AddressType()
     try:
-        result = at.decode(at.encode(v))
-    except Exception as e:
-        raise ValueError(f"Not AlgoAddressStringFormat: {e}")
+        x: List[str] = v.split(".")
+    except:
+        raise ValueError(f"Failed to seperate {v} into words with split'.'")
+    first_word = x[0]
+    first_char = first_word[0]
+    if not first_char.isalpha():
+        raise ValueError(f"Most significant word of {v} must start with alphabet char.")
+    for word in x:
+        if not word.isalnum():
+            raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
+    if not v.islower():
+        raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-def check_is_algo_msg_pack_encoded(v: str) -> None:
+def check_is_algo_address_string_format(v: str) -> None:
     """
-    AlgoMSgPackEncoded format: the format of an  transaction sent to
-    the Algorand blockchain.
+    AlgoAddressStringFormat format: The public key of a private/public Ed25519
+    key pair, transformed into an  Algorand address, by adding a 4-byte checksum
+    to the end of the public key and then encoding in base32.
 
     Raises:
-        ValueError: if not AlgoMSgPackEncoded  format
+        ValueError: if not AlgoAddressStringFormat format
     """
     import algosdk
 
+    at = algosdk.abi.AddressType()
     try:
-        algosdk.encoding.future_msgpack_decode(v)
+        result = at.decode(at.encode(v))
     except Exception as e:
-        raise ValueError(f"Not AlgoMsgPackEncoded format: {e}")
+        raise ValueError(f"Not AlgoAddressStringFormat: {e}")
 
 
-class OldTadeedAlgoReturn(BaseModel):
+class TerminalassetCertifyHack(BaseModel):
     """ """
 
-    OldTaDeedIdx: int = Field(
-        title="OldTaDeedIdx",
+    TerminalAssetAlias: str = Field(
+        title="TerminalAssetAlias",
     )
-    TaDaemonAddr: str = Field(
-        title="TaDaemonAddr",
+    TaDaemonApiPort: str = Field(
+        title="TaDaemonApiPort",
     )
-    ValidatorAddr: str = Field(
-        title="ValidatorAddr",
+    TaDaemonApiFqdn: str = Field(
+        title="TaDaemonApiFqdn",
     )
-    SignedNewDeedTransferTxn: str = Field(
-        title="SignedNewDeedTransferTxn",
+    TaDaemonAddr: str = Field(
+        title="TaDaemonAddr",
     )
-    TypeName: Literal["old.tadeed.algo.return"] = "old.tadeed.algo.return"
+    TypeName: Literal["terminalasset.certify.hack"] = "terminalasset.certify.hack"
     Version: str = "000"
 
-    @validator("TaDaemonAddr")
-    def _check_ta_daemon_addr(cls, v: str) -> str:
+    @validator("TerminalAssetAlias")
+    def _check_terminal_asset_alias(cls, v: str) -> str:
         try:
-            check_is_algo_address_string_format(v)
+            check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
-                f"TaDaemonAddr failed AlgoAddressStringFormat format validation: {e}"
+                f"TerminalAssetAlias failed LeftRightDot format validation: {e}"
             )
         return v
 
-    @validator("ValidatorAddr")
-    def _check_validator_addr(cls, v: str) -> str:
+    @validator("TaDaemonAddr")
+    def _check_ta_daemon_addr(cls, v: str) -> str:
         try:
             check_is_algo_address_string_format(v)
         except ValueError as e:
             raise ValueError(
-                f"ValidatorAddr failed AlgoAddressStringFormat format validation: {e}"
-            )
-        return v
-
-    @validator("SignedNewDeedTransferTxn")
-    def _check_signed_new_deed_transfer_txn(cls, v: str) -> str:
-        try:
-            check_is_algo_msg_pack_encoded(v)
-        except ValueError as e:
-            raise ValueError(
-                f"SignedNewDeedTransferTxn failed AlgoMsgPackEncoded format validation: {e}"
+                f"TaDaemonAddr failed AlgoAddressStringFormat format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class OldTadeedAlgoReturn_Maker:
-    type_name = "old.tadeed.algo.return"
+class TerminalassetCertifyHack_Maker:
+    type_name = "terminalasset.certify.hack"
     version = "000"
 
     def __init__(
         self,
-        old_ta_deed_idx: int,
+        terminal_asset_alias: str,
+        ta_daemon_api_port: str,
+        ta_daemon_api_fqdn: str,
         ta_daemon_addr: str,
-        validator_addr: str,
-        signed_new_deed_transfer_txn: str,
     ):
-        self.tuple = OldTadeedAlgoReturn(
-            OldTaDeedIdx=old_ta_deed_idx,
+        self.tuple = TerminalassetCertifyHack(
+            TerminalAssetAlias=terminal_asset_alias,
+            TaDaemonApiPort=ta_daemon_api_port,
+            TaDaemonApiFqdn=ta_daemon_api_fqdn,
             TaDaemonAddr=ta_daemon_addr,
-            ValidatorAddr=validator_addr,
-            SignedNewDeedTransferTxn=signed_new_deed_transfer_txn,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: OldTadeedAlgoReturn) -> str:
+    def tuple_to_type(cls, tuple: TerminalassetCertifyHack) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> OldTadeedAlgoReturn:
+    def type_to_tuple(cls, t: str) -> TerminalassetCertifyHack:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> OldTadeedAlgoReturn:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> TerminalassetCertifyHack:
         d2 = dict(d)
-        if "OldTaDeedIdx" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing OldTaDeedIdx")
+        if "TerminalAssetAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TerminalAssetAlias")
+        if "TaDaemonApiPort" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TaDaemonApiPort")
+        if "TaDaemonApiFqdn" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TaDaemonApiFqdn")
         if "TaDaemonAddr" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TaDaemonAddr")
-        if "ValidatorAddr" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing ValidatorAddr")
-        if "SignedNewDeedTransferTxn" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing SignedNewDeedTransferTxn")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return OldTadeedAlgoReturn(
-            OldTaDeedIdx=d2["OldTaDeedIdx"],
+        return TerminalassetCertifyHack(
+            TerminalAssetAlias=d2["TerminalAssetAlias"],
+            TaDaemonApiPort=d2["TaDaemonApiPort"],
+            TaDaemonApiFqdn=d2["TaDaemonApiFqdn"],
             TaDaemonAddr=d2["TaDaemonAddr"],
-            ValidatorAddr=d2["ValidatorAddr"],
-            SignedNewDeedTransferTxn=d2["SignedNewDeedTransferTxn"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/price_quantity.py` & `gridworks_atn-0.3.2/src/gwatn/types/price_quantity.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,14 +167,17 @@
             QuantityUnit
         )
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class PriceQuantity_Maker:
     type_name = "price.quantity"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/price_quantity_unitless.py` & `gridworks_atn-0.3.2/src/gwatn/types/price_quantity_unitless.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class PriceQuantityUnitless_Maker:
     type_name = "price.quantity.unitless"
     version = "000"
 
     def __init__(self, price_times1000: int, quantity_times1000: int):
         self.tuple = PriceQuantityUnitless(
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/ready.py` & `gridworks_atn-0.3.2/src/gwatn/types/simplesim_driver_report.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-"""Type ready, version 001"""
+"""Type simplesim.driver.report, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
+from gwatn.types.simplesim_driver_data import SimplesimDriverData
+from gwatn.types.simplesim_driver_data import SimplesimDriverData_Maker
+
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
 
     Raises:
@@ -62,110 +65,134 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-class Ready(BaseModel):
-    """Used in simulations by TimeCoordinator GNodes.
-
-    Only intended for simulations that do not have sub-second TimeSteps.
-    TimeCoordinators based on ```gridworks-timecoordinator``` have a notion of actors
-    whose `Ready` must be received before issuing the next TimeStep.
-    [More info](https://gridworks.readthedocs.io/en/latest/time-coordinator.html).
-    """
+class SimplesimDriverReport(BaseModel):
+    """ """
 
     FromGNodeAlias: str = Field(
-        title="The GNodeAlias of the sender",
+        title="FromGNodeAlias",
+    )
+    FromGNodeInstanecId: str = Field(
+        title="FromGNodeInstanecId",
     )
-    FromGNodeInstanceId: str = Field(
-        title="The GNodeInstanceId of the sender",
+    DriverDataTypeName: str = Field(
+        title="DriverDataTypeName",
     )
-    TimeUnixS: int = Field(
-        title="Latest simulated time for sender",
-        description="The time in unix seconds of the latest TimeStep received from the TimeCoordinator by the actor that sent the payload.",
+    DriverData: SimplesimDriverData = Field(
+        title="DriverData",
     )
-    TypeName: Literal["ready"] = "ready"
-    Version: str = "001"
+    TypeName: Literal["simplesim.driver.report"] = "simplesim.driver.report"
+    Version: str = "000"
 
     @validator("FromGNodeAlias")
     def _check_from_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
                 f"FromGNodeAlias failed LeftRightDot format validation: {e}"
             )
         return v
 
-    @validator("FromGNodeInstanceId")
-    def _check_from_g_node_instance_id(cls, v: str) -> str:
+    @validator("FromGNodeInstanecId")
+    def _check_from_g_node_instanec_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
+                f"FromGNodeInstanecId failed UuidCanonicalTextual format validation: {e}"
+            )
+        return v
+
+    @validator("DriverDataTypeName")
+    def _check_driver_data_type_name(cls, v: str) -> str:
+        try:
+            check_is_left_right_dot(v)
+        except ValueError as e:
+            raise ValueError(
+                f"DriverDataTypeName failed LeftRightDot format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
+        d["DriverData"] = self.DriverData.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class Ready_Maker:
-    type_name = "ready"
-    version = "001"
+class SimplesimDriverReport_Maker:
+    type_name = "simplesim.driver.report"
+    version = "000"
 
     def __init__(
-        self, from_g_node_alias: str, from_g_node_instance_id: str, time_unix_s: int
+        self,
+        from_g_node_alias: str,
+        from_g_node_instanec_id: str,
+        driver_data_type_name: str,
+        driver_data: SimplesimDriverData,
     ):
-        self.tuple = Ready(
+        self.tuple = SimplesimDriverReport(
             FromGNodeAlias=from_g_node_alias,
-            FromGNodeInstanceId=from_g_node_instance_id,
-            TimeUnixS=time_unix_s,
+            FromGNodeInstanecId=from_g_node_instanec_id,
+            DriverDataTypeName=driver_data_type_name,
+            DriverData=driver_data,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: Ready) -> str:
+    def tuple_to_type(cls, tuple: SimplesimDriverReport) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> Ready:
+    def type_to_tuple(cls, t: str) -> SimplesimDriverReport:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> Ready:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> SimplesimDriverReport:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
-        if "FromGNodeInstanceId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
-        if "TimeUnixS" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing TimeUnixS")
+        if "FromGNodeInstanecId" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FromGNodeInstanecId")
+        if "DriverDataTypeName" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing DriverDataTypeName")
+        if "DriverData" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing DriverData")
+        if not isinstance(d2["DriverData"], dict):
+            raise SchemaError(
+                f"d['DriverData'] {d2['DriverData']} must be a SimplesimDriverData!"
+            )
+        driver_data = SimplesimDriverData_Maker.dict_to_tuple(d2["DriverData"])
+        d2["DriverData"] = driver_data
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return Ready(
+        return SimplesimDriverReport(
             FromGNodeAlias=d2["FromGNodeAlias"],
-            FromGNodeInstanceId=d2["FromGNodeInstanceId"],
-            TimeUnixS=d2["TimeUnixS"],
+            FromGNodeInstanecId=d2["FromGNodeInstanecId"],
+            DriverDataTypeName=d2["DriverDataTypeName"],
+            DriverData=d2["DriverData"],
             TypeName=d2["TypeName"],
-            Version="001",
+            Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/scada_cert_transfer.py` & `gridworks_atn-0.3.2/src/gwatn/types/scada_cert_transfer.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class ScadaCertTransfer_Maker:
     type_name = "scada.cert.transfer"
     version = "000"
 
     def __init__(self, ta_alias: str, signed_proof: str):
         self.tuple = ScadaCertTransfer(
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/sim_scada_driver_report.py` & `gridworks_atn-0.3.2/src/gwatn/types/flo_params.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-"""Type sim.scada.driver.report, version 000"""
+"""Type flo.params, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
+from pydantic import Extra
 from pydantic import Field
 from pydantic import validator
 
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
@@ -62,138 +63,178 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-class SimScadaDriverReport(BaseModel):
-    """ """
+class FloParams(BaseModel):
+    """Base class for Forward Looking Optimizer params.
 
-    FromGNodeAlias: str = Field(
-        title="FromGNodeAlias",
-    )
-    FromGNodeInstanceId: str = Field(
-        title="FromGNodeInstanceId",
-    )
-    BoostPowerKwTimes1000: int = Field(
-        title="BoostPowerKwTimes1000",
-    )
-    HeatpumpPowerKwTimes1000: int = Field(
-        title="HeatpumpPowerKwTimes1000",
-    )
-    StoreKwh: int = Field(
-        title="StoreKwh",
+    Derived classes are expected to have TypeNames enforced as literals that start with flo.params. E.g. flo.params.brickstorageheater.   This container is used for sending messages that include flo.params (i.e, flo.params.report
+    [More info](https://gridworks-atn.readthedocs.io/en/latest/flo.html#flo-params).
+    """
+
+    GNodeAlias: str = Field(
+        title="GNodeAlias",
     )
-    CopTimes10: int = Field(
-        title="CopTimes10",
+    FloParamsUid: str = Field(
+        title="FloParamsUid",
     )
-    MaxStoreKwh: int = Field(
-        title="MaxStoreKwh",
+    HomeCity: str = Field(
+        title="HomeCity",
+        default="MILLINOCKET_ME",
+    )
+    TimezoneString: str = Field(
+        title="TimezoneString",
+        default="US/Eastern",
+    )
+    StartYearUtc: int = Field(
+        title="StartYearUtc",
+        default=2020,
+    )
+    StartMonthUtc: int = Field(
+        title="StartMonthUtc",
+        default=1,
+    )
+    StartDayUtc: int = Field(
+        title="StartDayUtc",
+        default=1,
+    )
+    StartHourUtc: int = Field(
+        title="StartHourUtc",
+        default=0,
+    )
+    StartMinuteUtc: int = Field(
+        title="StartMinuteUtc",
+        default=0,
+    )
+    TypeName: str = Field(
+        title="TypeName",
+        default="flo.params",
     )
-    TypeName: Literal["sim.scada.driver.report"] = "sim.scada.driver.report"
     Version: str = "000"
 
-    @validator("FromGNodeAlias")
-    def _check_from_g_node_alias(cls, v: str) -> str:
+    class Config:
+        extra = Extra.allow
+
+    @validator("TypeName")
+    def _check_type_name(cls, v: str) -> str:
+        if not v.startswith("flo.params"):
+            raise ValueError(f"TypeName {v} must start with 'flo.params'")
+        return v
+
+    @validator("GNodeAlias")
+    def _check_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
-            raise ValueError(
-                f"FromGNodeAlias failed LeftRightDot format validation: {e}"
-            )
+            raise ValueError(f"GNodeAlias failed LeftRightDot format validation: {e}")
         return v
 
-    @validator("FromGNodeInstanceId")
-    def _check_from_g_node_instance_id(cls, v: str) -> str:
+    @validator("FloParamsUid")
+    def _check_flo_params_uid(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
+                f"FloParamsUid failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class SimScadaDriverReport_Maker:
-    type_name = "sim.scada.driver.report"
+class FloParams_Maker:
+    type_name = "flo.params"
     version = "000"
 
     def __init__(
         self,
-        from_g_node_alias: str,
-        from_g_node_instance_id: str,
-        boost_power_kw_times1000: int,
-        heatpump_power_kw_times1000: int,
-        store_kwh: int,
-        cop_times10: int,
-        max_store_kwh: int,
+        g_node_alias: str,
+        flo_params_uid: str,
+        home_city: str,
+        timezone_string: str,
+        start_year_utc: int,
+        start_month_utc: int,
+        start_day_utc: int,
+        start_hour_utc: int,
+        start_minute_utc: int,
     ):
-        self.tuple = SimScadaDriverReport(
-            FromGNodeAlias=from_g_node_alias,
-            FromGNodeInstanceId=from_g_node_instance_id,
-            BoostPowerKwTimes1000=boost_power_kw_times1000,
-            HeatpumpPowerKwTimes1000=heatpump_power_kw_times1000,
-            StoreKwh=store_kwh,
-            CopTimes10=cop_times10,
-            MaxStoreKwh=max_store_kwh,
+        self.tuple = FloParams(
+            GNodeAlias=g_node_alias,
+            FloParamsUid=flo_params_uid,
+            HomeCity=home_city,
+            TimezoneString=timezone_string,
+            StartYearUtc=start_year_utc,
+            StartMonthUtc=start_month_utc,
+            StartDayUtc=start_day_utc,
+            StartHourUtc=start_hour_utc,
+            StartMinuteUtc=start_minute_utc,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: SimScadaDriverReport) -> str:
+    def tuple_to_type(cls, tuple: FloParams) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> SimScadaDriverReport:
+    def type_to_tuple(cls, t: str) -> FloParams:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> SimScadaDriverReport:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> FloParams:
         d2 = dict(d)
-        if "FromGNodeAlias" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
-        if "FromGNodeInstanceId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
-        if "BoostPowerKwTimes1000" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing BoostPowerKwTimes1000")
-        if "HeatpumpPowerKwTimes1000" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing HeatpumpPowerKwTimes1000")
-        if "StoreKwh" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StoreKwh")
-        if "CopTimes10" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing CopTimes10")
-        if "MaxStoreKwh" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing MaxStoreKwh")
+        if "GNodeAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing GNodeAlias")
+        if "FloParamsUid" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FloParamsUid")
+        if "HomeCity" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing HomeCity")
+        if "TimezoneString" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing TimezoneString")
+        if "StartYearUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartYearUtc")
+        if "StartMonthUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartMonthUtc")
+        if "StartDayUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartDayUtc")
+        if "StartHourUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartHourUtc")
+        if "StartMinuteUtc" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StartMinuteUtc")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return SimScadaDriverReport(
-            FromGNodeAlias=d2["FromGNodeAlias"],
-            FromGNodeInstanceId=d2["FromGNodeInstanceId"],
-            BoostPowerKwTimes1000=d2["BoostPowerKwTimes1000"],
-            HeatpumpPowerKwTimes1000=d2["HeatpumpPowerKwTimes1000"],
-            StoreKwh=d2["StoreKwh"],
-            CopTimes10=d2["CopTimes10"],
-            MaxStoreKwh=d2["MaxStoreKwh"],
+        return FloParams(
+            GNodeAlias=d2["GNodeAlias"],
+            FloParamsUid=d2["FloParamsUid"],
+            HomeCity=d2["HomeCity"],
+            TimezoneString=d2["TimezoneString"],
+            StartYearUtc=d2["StartYearUtc"],
+            StartMonthUtc=d2["StartMonthUtc"],
+            StartDayUtc=d2["StartDayUtc"],
+            StartHourUtc=d2["StartHourUtc"],
+            StartMinuteUtc=d2["StartMinuteUtc"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/sim_timestep.py` & `gridworks_atn-0.3.2/src/gwatn/types/simplesim_snapshot_brickstorageheater.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,19 @@
-"""Type sim.timestep, version 000"""
+"""Type simplesim.snapshot.brickstorageheater, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
 
-def check_is_reasonable_unix_time_s(v: int) -> None:
-    """
-    ReasonableUnixTimeS format: time in unix seconds between Jan 1 2000 and Jan 1 3000
-
-    Raises:
-        ValueError: if not ReasonableUnixTimeS format
-    """
-    import pendulum
-
-    if pendulum.parse("2000-01-01T00:00:00Z").int_timestamp > v:  # type: ignore[attr-defined]
-        raise ValueError(f"{v} must be after Jan 1 2000")
-    if pendulum.parse("3000-01-01T00:00:00Z").int_timestamp < v:  # type: ignore[attr-defined]
-        raise ValueError(f"{v} must be before Jan 1 3000")
-
-
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
 
     Raises:
         ValueError: if not UuidCanonicalTextual format
@@ -77,52 +62,38 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-def check_is_reasonable_unix_time_ms(v: str) -> None:
-    """
-    ReasonableUnixTimeMs format: time in unix milliseconds between Jan 1 2000 and Jan 1 3000
-
-    Raises:
-        ValueError: if not ReasonableUnixTimeMs format
-    """
-    import pendulum
-
-    if pendulum.parse("2000-01-01T00:00:00Z").int_timestamp * 1000 > v:  # type: ignore[attr-defined]
-        raise ValueError(f"{v} must be after Jan 1 2000")
-    if pendulum.parse("3000-01-01T00:00:00Z").int_timestamp * 1000 < v:  # type: ignore[attr-defined]
-        raise ValueError(f"{v} must be before Jan 1 3000")
-
-
-class SimTimestep(BaseModel):
-    """Sent by TimeCoordinators to coordinate time.
-
-    For simulated actors, time progresses discretely on receipt of these time steps.
-    """
+class SimplesimSnapshotBrickstorageheater(BaseModel):
+    """ """
 
     FromGNodeAlias: str = Field(
-        title="The GNodeAlias of the sender",
-        description="The sender should always be a GNode Actor of role TimeCoordinator.",
+        title="FromGNodeAlias",
     )
     FromGNodeInstanceId: str = Field(
-        title="The GNodeInstanceId of the sender",
+        title="FromGNodeInstanceId",
     )
-    TimeUnixS: int = Field(
-        title="Current time in unix seconds",
+    PowerWatts: int = Field(
+        title="PowerWatts",
     )
-    TimestepCreatedMs: int = Field(
-        title="The real time created, in unix milliseconds",
+    StoreKwh: int = Field(
+        title="StoreKwh",
     )
-    MessageId: str = Field(
-        title="MessageId",
+    MaxStoreKwh: int = Field(
+        title="MaxStoreKwh",
     )
-    TypeName: Literal["sim.timestep"] = "sim.timestep"
+    AboutTerminalAssetAlias: str = Field(
+        title="AboutTerminalAssetAlias",
+    )
+    TypeName: Literal[
+        "simplesim.snapshot.brickstorageheater"
+    ] = "simplesim.snapshot.brickstorageheater"
     Version: str = "000"
 
     @validator("FromGNodeAlias")
     def _check_from_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
@@ -137,111 +108,99 @@
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
                 f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("TimeUnixS")
-    def _check_time_unix_s(cls, v: int) -> int:
-        try:
-            check_is_reasonable_unix_time_s(v)
-        except ValueError as e:
-            raise ValueError(
-                f"TimeUnixS failed ReasonableUnixTimeS format validation: {e}"
-            )
-        return v
-
-    @validator("TimestepCreatedMs")
-    def _check_timestep_created_ms(cls, v: int) -> int:
-        try:
-            check_is_reasonable_unix_time_ms(v)
-        except ValueError as e:
-            raise ValueError(
-                f"TimestepCreatedMs failed ReasonableUnixTimeMs format validation: {e}"
-            )
-        return v
-
-    @validator("MessageId")
-    def _check_message_id(cls, v: str) -> str:
+    @validator("AboutTerminalAssetAlias")
+    def _check_about_terminal_asset_alias(cls, v: str) -> str:
         try:
-            check_is_uuid_canonical_textual(v)
+            check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
-                f"MessageId failed UuidCanonicalTextual format validation: {e}"
+                f"AboutTerminalAssetAlias failed LeftRightDot format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class SimTimestep_Maker:
-    type_name = "sim.timestep"
+class SimplesimSnapshotBrickstorageheater_Maker:
+    type_name = "simplesim.snapshot.brickstorageheater"
     version = "000"
 
     def __init__(
         self,
         from_g_node_alias: str,
         from_g_node_instance_id: str,
-        time_unix_s: int,
-        timestep_created_ms: int,
-        message_id: str,
+        power_watts: int,
+        store_kwh: int,
+        max_store_kwh: int,
+        about_terminal_asset_alias: str,
     ):
-        self.tuple = SimTimestep(
+        self.tuple = SimplesimSnapshotBrickstorageheater(
             FromGNodeAlias=from_g_node_alias,
             FromGNodeInstanceId=from_g_node_instance_id,
-            TimeUnixS=time_unix_s,
-            TimestepCreatedMs=timestep_created_ms,
-            MessageId=message_id,
+            PowerWatts=power_watts,
+            StoreKwh=store_kwh,
+            MaxStoreKwh=max_store_kwh,
+            AboutTerminalAssetAlias=about_terminal_asset_alias,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: SimTimestep) -> str:
+    def tuple_to_type(cls, tuple: SimplesimSnapshotBrickstorageheater) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> SimTimestep:
+    def type_to_tuple(cls, t: str) -> SimplesimSnapshotBrickstorageheater:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> SimTimestep:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> SimplesimSnapshotBrickstorageheater:
         d2 = dict(d)
         if "FromGNodeAlias" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeAlias")
         if "FromGNodeInstanceId" not in d2.keys():
             raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
-        if "TimeUnixS" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing TimeUnixS")
-        if "TimestepCreatedMs" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing TimestepCreatedMs")
-        if "MessageId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing MessageId")
+        if "PowerWatts" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing PowerWatts")
+        if "StoreKwh" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing StoreKwh")
+        if "MaxStoreKwh" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing MaxStoreKwh")
+        if "AboutTerminalAssetAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing AboutTerminalAssetAlias")
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return SimTimestep(
+        return SimplesimSnapshotBrickstorageheater(
             FromGNodeAlias=d2["FromGNodeAlias"],
             FromGNodeInstanceId=d2["FromGNodeInstanceId"],
-            TimeUnixS=d2["TimeUnixS"],
-            TimestepCreatedMs=d2["TimestepCreatedMs"],
-            MessageId=d2["MessageId"],
+            PowerWatts=d2["PowerWatts"],
+            StoreKwh=d2["StoreKwh"],
+            MaxStoreKwh=d2["MaxStoreKwh"],
+            AboutTerminalAssetAlias=d2["AboutTerminalAssetAlias"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/sla_enter.py` & `gridworks_atn-0.3.2/src/gwatn/types/sla_enter.py`

 * *Files 3% similar despite different names*

```diff
@@ -57,14 +57,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class SlaEnter_Maker:
     type_name = "sla.enter"
     version = "000"
 
     def __init__(self, terminal_asset_alias: str):
         self.tuple = SlaEnter(
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/snapshot_heatpumpwithbooststore.py` & `gridworks_atn-0.3.2/src/gwatn/types/flo_params_report.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,18 +1,37 @@
-"""Type snapshot.heatpumpwithbooststore, version 000"""
+"""Type flo.params.report, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
+from typing import Optional
 
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import validator
 
+from gwatn.types.flo_params import FloParams
+from gwatn.types.flo_params import FloParams_Maker
+
+
+def check_is_reasonable_unix_time_s(v: int) -> None:
+    """
+    ReasonableUnixTimeS format: time in unix seconds between Jan 1 2000 and Jan 1 3000
+
+    Raises:
+        ValueError: if not ReasonableUnixTimeS format
+    """
+    import pendulum
+
+    if pendulum.parse("2000-01-01T00:00:00Z").int_timestamp > v:  # type: ignore[attr-defined]
+        raise ValueError(f"{v} must be after Jan 1 2000")
+    if pendulum.parse("3000-01-01T00:00:00Z").int_timestamp < v:  # type: ignore[attr-defined]
+        raise ValueError(f"{v} must be before Jan 1 3000")
+
 
 def check_is_uuid_canonical_textual(v: str) -> None:
     """
     UuidCanonicalTextual format:  A string of hex words separated by hyphens
     of length 8-4-4-4-12.
 
     Raises:
@@ -62,158 +81,183 @@
     for word in x:
         if not word.isalnum():
             raise ValueError(f"words of {v} split by by '.' must be alphanumeric.")
     if not v.islower():
         raise ValueError(f"All characters of {v} must be lowercase.")
 
 
-class SnapshotHeatpumpwithbooststore(BaseModel):
-    """ """
+class FloParamsReport(BaseModel):
+    """Flo Params Report.
 
-    FromGNodeAlias: str = Field(
-        title="FromGNodeAlias",
-    )
-    FromGNodeInstanceId: str = Field(
-        title="FromGNodeInstanceId",
+    Type used for a message provided by an AtomicTNode or SCADA actor re the flo parameters just used to run a FLO.
+    [More info](https://gridworks-atn.readthedocs.io/en/latest/flo.html#flo-params).
+    """
+
+    GNodeAlias: str = Field(
+        title="GNodeAlias",
     )
-    BoostPowerKwTimes1000: int = Field(
-        title="BoostPowerKwTimes1000",
+    GNodeInstanceId: str = Field(
+        title="GNodeInstanceId",
     )
-    HeatpumpPowerKwTimes1000: int = Field(
-        title="HeatpumpPowerKwTimes1000",
+    FloParamsTypeName: str = Field(
+        title="FloParamsTypeName",
     )
-    StoreKwh: int = Field(
-        title="StoreKwh",
+    FloParamsTypeVersion: str = Field(
+        title="FloParamsTypeVersion",
     )
-    CopTimes10: int = Field(
-        title="CopTimes10",
+    ReportGeneratedTimeUnixS: int = Field(
+        title="ReportGeneratedTimeUnixS",
     )
-    MaxStoreKwh: int = Field(
-        title="MaxStoreKwh",
+    IrlTimeUnixS: Optional[int] = Field(
+        title="IrlTimeUnixS",
+        default=None,
     )
-    AboutTerminalAssetAlias: str = Field(
-        title="AboutTerminalAssetAlias",
+    Params: FloParams = Field(
+        title="Params",
     )
-    TypeName: Literal[
-        "snapshot.heatpumpwithbooststore"
-    ] = "snapshot.heatpumpwithbooststore"
+    TypeName: Literal["flo.params.report"] = "flo.params.report"
     Version: str = "000"
 
-    @validator("FromGNodeAlias")
-    def _check_from_g_node_alias(cls, v: str) -> str:
+    @validator("GNodeAlias")
+    def _check_g_node_alias(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
-            raise ValueError(
-                f"FromGNodeAlias failed LeftRightDot format validation: {e}"
-            )
+            raise ValueError(f"GNodeAlias failed LeftRightDot format validation: {e}")
         return v
 
-    @validator("FromGNodeInstanceId")
-    def _check_from_g_node_instance_id(cls, v: str) -> str:
+    @validator("GNodeInstanceId")
+    def _check_g_node_instance_id(cls, v: str) -> str:
         try:
             check_is_uuid_canonical_textual(v)
         except ValueError as e:
             raise ValueError(
-                f"FromGNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
+                f"GNodeInstanceId failed UuidCanonicalTextual format validation: {e}"
             )
         return v
 
-    @validator("AboutTerminalAssetAlias")
-    def _check_about_terminal_asset_alias(cls, v: str) -> str:
+    @validator("FloParamsTypeName")
+    def _check_flo_params_type_name(cls, v: str) -> str:
         try:
             check_is_left_right_dot(v)
         except ValueError as e:
             raise ValueError(
-                f"AboutTerminalAssetAlias failed LeftRightDot format validation: {e}"
+                f"FloParamsTypeName failed LeftRightDot format validation: {e}"
+            )
+        return v
+
+    @validator("ReportGeneratedTimeUnixS")
+    def _check_report_generated_time_unix_s(cls, v: int) -> int:
+        try:
+            check_is_reasonable_unix_time_s(v)
+        except ValueError as e:
+            raise ValueError(
+                f"ReportGeneratedTimeUnixS failed ReasonableUnixTimeS format validation: {e}"
+            )
+        return v
+
+    @validator("IrlTimeUnixS")
+    def _check_irl_time_unix_s(cls, v: Optional[int]) -> Optional[int]:
+        if v is None:
+            return v
+        try:
+            check_is_reasonable_unix_time_s(v)
+        except ValueError as e:
+            raise ValueError(
+                f"IrlTimeUnixS failed ReasonableUnixTimeS format validation: {e}"
             )
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
+        if d["IrlTimeUnixS"] is None:
+            del d["IrlTimeUnixS"]
+        d["Params"] = self.Params.as_dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
-class SnapshotHeatpumpwithbooststore_Maker:
-    type_name = "snapshot.heatpumpwithbooststore"
+class FloParamsReport_Maker:
+    type_name = "flo.params.report"
     version = "000"
 
     def __init__(
         self,
-        from_g_node_alias: str,
-        from_g_node_instance_id: str,
-        boost_power_kw_times1000: int,
-        heatpump_power_kw_times1000: int,
-        store_kwh: int,
-        cop_times10: int,
-        max_store_kwh: int,
-        about_terminal_asset_alias: str,
+        g_node_alias: str,
+        g_node_instance_id: str,
+        flo_params_type_name: str,
+        flo_params_type_version: str,
+        report_generated_time_unix_s: int,
+        irl_time_unix_s: Optional[int],
+        params: FloParams,
     ):
-        self.tuple = SnapshotHeatpumpwithbooststore(
-            FromGNodeAlias=from_g_node_alias,
-            FromGNodeInstanceId=from_g_node_instance_id,
-            BoostPowerKwTimes1000=boost_power_kw_times1000,
-            HeatpumpPowerKwTimes1000=heatpump_power_kw_times1000,
-            StoreKwh=store_kwh,
-            CopTimes10=cop_times10,
-            MaxStoreKwh=max_store_kwh,
-            AboutTerminalAssetAlias=about_terminal_asset_alias,
+        self.tuple = FloParamsReport(
+            GNodeAlias=g_node_alias,
+            GNodeInstanceId=g_node_instance_id,
+            FloParamsTypeName=flo_params_type_name,
+            FloParamsTypeVersion=flo_params_type_version,
+            ReportGeneratedTimeUnixS=report_generated_time_unix_s,
+            IrlTimeUnixS=irl_time_unix_s,
+            Params=params,
             #
         )
 
     @classmethod
-    def tuple_to_type(cls, tuple: SnapshotHeatpumpwithbooststore) -> str:
+    def tuple_to_type(cls, tuple: FloParamsReport) -> str:
         """
         Given a Python class object, returns the serialized JSON type object
         """
         return tuple.as_type()
 
     @classmethod
-    def type_to_tuple(cls, t: str) -> SnapshotHeatpumpwithbooststore:
+    def type_to_tuple(cls, t: str) -> FloParamsReport:
         """
         Given a serialized JSON type object, returns the Python class object
         """
         try:
             d = json.loads(t)
         except TypeError:
             raise SchemaError("Type must be string or bytes!")
         if not isinstance(d, dict):
             raise SchemaError(f"Deserializing {t} must result in dict!")
         return cls.dict_to_tuple(d)
 
     @classmethod
-    def dict_to_tuple(cls, d: dict[str, Any]) -> SnapshotHeatpumpwithbooststore:
+    def dict_to_tuple(cls, d: dict[str, Any]) -> FloParamsReport:
         d2 = dict(d)
-        if "FromGNodeAlias" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeAlias")
-        if "FromGNodeInstanceId" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing FromGNodeInstanceId")
-        if "BoostPowerKwTimes1000" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing BoostPowerKwTimes1000")
-        if "HeatpumpPowerKwTimes1000" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing HeatpumpPowerKwTimes1000")
-        if "StoreKwh" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing StoreKwh")
-        if "CopTimes10" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing CopTimes10")
-        if "MaxStoreKwh" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing MaxStoreKwh")
-        if "AboutTerminalAssetAlias" not in d2.keys():
-            raise SchemaError(f"dict {d2} missing AboutTerminalAssetAlias")
+        if "GNodeAlias" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing GNodeAlias")
+        if "GNodeInstanceId" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing GNodeInstanceId")
+        if "FloParamsTypeName" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FloParamsTypeName")
+        if "FloParamsTypeVersion" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing FloParamsTypeVersion")
+        if "ReportGeneratedTimeUnixS" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing ReportGeneratedTimeUnixS")
+        if "IrlTimeUnixS" not in d2.keys():
+            d2["IrlTimeUnixS"] = None
+        if "Params" not in d2.keys():
+            raise SchemaError(f"dict {d2} missing Params")
+        if not isinstance(d2["Params"], dict):
+            raise SchemaError(f"d['Params'] {d2['Params']} must be a FloParams!")
+        params = FloParams_Maker.dict_to_tuple(d2["Params"])
+        d2["Params"] = params
         if "TypeName" not in d2.keys():
             raise SchemaError(f"dict {d2} missing TypeName")
 
-        return SnapshotHeatpumpwithbooststore(
-            FromGNodeAlias=d2["FromGNodeAlias"],
-            FromGNodeInstanceId=d2["FromGNodeInstanceId"],
-            BoostPowerKwTimes1000=d2["BoostPowerKwTimes1000"],
-            HeatpumpPowerKwTimes1000=d2["HeatpumpPowerKwTimes1000"],
-            StoreKwh=d2["StoreKwh"],
-            CopTimes10=d2["CopTimes10"],
-            MaxStoreKwh=d2["MaxStoreKwh"],
-            AboutTerminalAssetAlias=d2["AboutTerminalAssetAlias"],
+        return FloParamsReport(
+            GNodeAlias=d2["GNodeAlias"],
+            GNodeInstanceId=d2["GNodeInstanceId"],
+            FloParamsTypeName=d2["FloParamsTypeName"],
+            FloParamsTypeVersion=d2["FloParamsTypeVersion"],
+            ReportGeneratedTimeUnixS=d2["ReportGeneratedTimeUnixS"],
+            IrlTimeUnixS=d2["IrlTimeUnixS"],
+            Params=d2["Params"],
             TypeName=d2["TypeName"],
             Version="000",
         )
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/tadeed_specs_hack.py` & `gridworks_atn-0.3.2/src/gwatn/types/tadeed_specs_hack.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,17 @@
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class TadeedSpecsHack_Maker:
     type_name = "tadeed.specs.hack"
     version = "000"
 
     def __init__(
         self,
```

### Comparing `gridworks_atn-0.2.4/src/gwatn/types/tavalidatorcert_algo_create.py` & `gridworks_atn-0.3.2/src/gwatn/types/tavalidatorcert_algo_create.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 """Type tavalidatorcert.algo.create, version 000"""
 import json
 from typing import Any
 from typing import Dict
 from typing import Literal
 
-import gridworks.algo_utils as algo_utils
-import gridworks.api_utils as api_utils
-import gridworks.gw_config as config
-from algosdk import encoding
-from algosdk.future import transaction
 from gridworks.errors import SchemaError
 from pydantic import BaseModel
 from pydantic import Field
 from pydantic import root_validator
 from pydantic import validator
 
 
@@ -69,29 +64,21 @@
 
     @validator("ValidatorAddr")
     def check_validator_addr(cls, v: str) -> str:
         """
         Axiom 5: Uniqueness.
         There must not already be a TaValidatorCert belonging to the  2-sig [GnfAdminAddr, ValidatorAddr] address.
         """
-        ValidatorAddr = v
-        gnf_admin_addr = config.Public().gnf_admin_addr
-        multi = algo_utils.MultisigAccount(
-            version=1,
-            threshold=2,
-            addresses=[gnf_admin_addr, ValidatorAddr],
-        )
         try:
             check_is_algo_address_string_format(v)
         except ValueError as e:
             raise ValueError(
                 f"ValidatorAddr failed AlgoAddressStringFormat format validation: {e}"
             )
-        if api_utils.is_validator_addr(ValidatorAddr):
-            ValueError("Axiom 5: Already has TaValidatorCert")
+        # TODO: Axiom
         return v
 
     @validator("HalfSignedCertCreationMtx")
     def check_half_signed_cert_creation_mtx(cls, v: str) -> str:
         """
         Axioms 2, 3:
 
@@ -105,94 +92,38 @@
         """
         try:
             check_is_algo_msg_pack_encoded(v)
         except ValueError as e:
             raise ValueError(
                 f"HalfSignedCertCreationMtx failed AlgoMsgPackEncoded format validation: {e}"
             )
-        mtx = encoding.future_msgpack_decode(v)
-        txn = mtx.transaction
-        gnf_admin_addr = config.Public().gnf_admin_addr
-        if not isinstance(txn, transaction.AssetConfigTxn):
-            raise ValueError(
-                "Axiom 2: The transaction must have type AssetConfigTxn"
-                f" got {type(txn)}."
-            )
-        if not txn.total == 1:
-            raise ValueError(
-                "Axiom 3: TaValidatorCert ASA Total must be 1, "
-                f" got {txn.total}."
-                " See https://gridworks.readthedocs.io/en/latest/ta-validator.html#tavalidator-certificate"
-            )
-        if not txn.decimals == 0:
-            raise ValueError(
-                "Axiom 3: TaValidatorCert ASA Decimals must be 0, "
-                f" got {txn.decimals}."
-                " See https://gridworks.readthedocs.io/en/latest/ta-validator.html#tavalidator-certificate"
-            )
-        if not txn.unit_name == "VLDTR":
-            raise ValueError(
-                "Axiom 3: TaValidatorCert ASA UnitName must be 'VLDTR', "
-                f" got {txn.decimals}."
-                " See https://gridworks.readthedocs.io/en/latest/ta-validator.html#tavalidator-certificate"
-            )
-        if not txn.manager == gnf_admin_addr:
-            raise ValueError(
-                "Axiom 3: TaValidatorCert manager must be Universe gnf_admin_addr, "
-                f" got {txn.decimals}."
-                " See https://gridworks.readthedocs.io/en/latest/ta-validator.html#tavalidator-certificate"
-            )
-        if (txn.asset_name is None) or (txn.asset_name == ""):
-            raise ValueError(
-                "Axiom 3: TaValidatorCert AssetName cannot be blank, "
-                " See https://gridworks.readthedocs.io/en/latest/ta-validator.html#tavalidator-certificate"
-            )
+        # TODO: Axiom
         return v
 
     @root_validator(pre=True)
     def check_axiom_1(cls, v: dict) -> dict:
         """
         Axiom 1: Is correct Multisig.
         Decoded HalfSignedCertCreationMtx must have type MultisigTransaction from the
         2-sig MultiAccount  [GnfAdminAddr, ValidatorAddr], signed by ValidatorAddr.
         [More info](https://gridworks.readthedocs.io/en/latest/g-node-factory.html#gnfadminaddr)
         """
-        mtx = encoding.future_msgpack_decode(v.get("HalfSignedCertCreationMtx", None))
-        ValidatorAddr = v.get("ValidatorAddr")
-        gnf_admin_addr = config.Public().gnf_admin_addr
-        multi = algo_utils.MultisigAccount(
-            version=1,
-            threshold=2,
-            addresses=[gnf_admin_addr, ValidatorAddr],
-        )
-
-        if not isinstance(mtx, transaction.MultisigTransaction):
-            raise ValueError(
-                "Axiom 1: Decoded HalfSignedCertCreationMtx must have type MultisigTransaction,"
-                f" got {type(mtx)}."
-            )
-
-        if not multi.addr == mtx.multisig.address():
-            raise ValueError(
-                "Axiom 1: Decoded HalfSignedCertCreationMtx must come from the 2-sig MultiAccount ,"
-                f" [GnfAdminAddr, ValidatorAddr], got {type(mtx)}."
-            )
-        if mtx.multisig.subsigs[1].signature is None:
-            raise ValueError(
-                "Axiom 1: Decoded HalfSignedCertCreationMtx missing TaValidator signature.}"
-            )
+        # TODO: Implement check for axiom 1"
         return v
 
     def as_dict(self) -> Dict[str, Any]:
         d = self.dict()
         return d
 
     def as_type(self) -> str:
         return json.dumps(self.as_dict())
 
+    def __hash__(self):
+        return hash((type(self),) + tuple(self.__dict__.values()))  # noqa
+
 
 class TavalidatorcertAlgoCreate_Maker:
     type_name = "tavalidatorcert.algo.create"
     version = "000"
 
     def __init__(self, validator_addr: str, half_signed_cert_creation_mtx: str):
         self.tuple = TavalidatorcertAlgoCreate(
```

### Comparing `gridworks_atn-0.2.4/PKG-INFO` & `gridworks_atn-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 Metadata-Version: 2.1
 Name: gridworks-atn
-Version: 0.2.4
+Version: 0.3.2
 Summary: Gridworks Atn Spaceheat
 Home-page: https://github.com/thegridelectric/gridworks-atn
 License: None
 Author: Jessica Millar
 Author-email: jmillar@gridworks-consulting.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gridworks (>=0.2.1,<0.3.0)
-Requires-Dist: gridworks-proactor (>=0.1.8,<0.2.0)
-Requires-Dist: gridworks-protocol (>=0.4.5,<0.5.0)
+Requires-Dist: gridworks (>=0.2.4,<0.3.0)
+Requires-Dist: gridworks-protocol (>=0.5.2,<0.6.0)
 Requires-Dist: numpy (>=1.23.4,<2.0.0)
 Requires-Dist: paho-mqtt (>=1.6.1,<2.0.0)
-Requires-Dist: types-requests (>=2.28.11.2,<3.0.0.0)
 Project-URL: Changelog, https://github.com/thegridelectric/gridworks-atn/releases
 Project-URL: Documentation, https://gridworks-atn.readthedocs.io
 Project-URL: Repository, https://github.com/thegridelectric/gridworks-atn
 Description-Content-Type: text/markdown
 
 # Gridworks Atn
```

