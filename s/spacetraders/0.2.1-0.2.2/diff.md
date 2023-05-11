# Comparing `tmp/spacetraders-0.2.1.tar.gz` & `tmp/spacetraders-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.2.1.tar", max compression
+gzip compressed data, was "spacetraders-0.2.2.tar", max compression
```

## Comparing `spacetraders-0.2.1.tar` & `spacetraders-0.2.2.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.2.1/README.md
--rw-r--r--   0        0        0      522 2023-05-11 13:42:27.786961 spacetraders-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-11 13:36:56.146961 spacetraders-0.2.1/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-11 13:36:55.656961 spacetraders-0.2.1/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     3818 2023-05-11 13:36:56.196961 spacetraders-0.2.1/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4290 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5132 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4308 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4303 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     5015 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.666961 spacetraders-0.2.1/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     9211 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4361 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4985 2023-05-11 13:36:56.236961 spacetraders-0.2.1/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.716961 spacetraders-0.2.1/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     5255 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4513 2023-05-11 13:36:56.226961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4566 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4610 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     6213 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     5356 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5511 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4236 2023-05-11 13:36:56.266961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4338 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4970 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     6390 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4295 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4973 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5263 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     6907 2023-05-11 13:36:56.296961 spacetraders-0.2.1/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     5331 2023-05-11 13:36:56.296961 spacetraders-0.2.1/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5125 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5344 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4554 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4302 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5082 2023-05-11 13:36:56.336961 spacetraders-0.2.1/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5570 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5395 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     6303 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4838 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5624 2023-05-11 13:36:56.386961 spacetraders-0.2.1/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4812 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4398 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5944 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4984 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4799 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4213 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1170 2023-05-11 13:36:56.336961 spacetraders-0.2.1/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1200 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1351 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1376 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1563 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     1774 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1603 2023-05-11 13:36:56.386961 spacetraders-0.2.1/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1231 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1474 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1629 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1152 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1370 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1326 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1217 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1344 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1229 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1362 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1299 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1175 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1176 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1219 2023-05-11 13:36:56.446961 spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1193 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1128 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1239 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1182 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1433 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1162 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1141 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1358 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1312 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     2091 2023-05-11 13:36:55.916961 spacetraders-0.2.1/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1176 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1202 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1076 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1183 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1070 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1177 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1077 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1064 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1062 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1087 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1063 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1111 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1076 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1064 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1195 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1171 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1167 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1068 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1133 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1086 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1470 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1059 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1134 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1336 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2208 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/market.py
--rw-r--r--   0        0        0     1771 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2047 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1097 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1067 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1345 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1132 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1270 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1115 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1385 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1102 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1224 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1348 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1146 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1298 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1310 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1133 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1509 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     2269 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1035 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1032 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1040 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1038 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1383 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2141 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1369 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1086 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3041 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1385 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1401 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2114 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-11 13:36:55.816961 spacetraders-0.2.1/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1751 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2146 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1455 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1278 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1784 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1763 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-11 13:36:55.906961 spacetraders-0.2.1/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-11 13:36:55.906961 spacetraders-0.2.1/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     1988 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1829 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1388 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1802 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1137 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1217 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     1948 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1178 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1178 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1384 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1360 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-11 13:36:55.886961 spacetraders-0.2.1/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-11 13:36:55.816961 spacetraders-0.2.1/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     1838 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2371 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1088 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1636 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2166 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1100 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1626 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/system.py
--rw-r--r--   0        0        0     1003 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1243 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1190 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-11 13:36:55.886961 spacetraders-0.2.1/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1253 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1122 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1059 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1134 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1337 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2127 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1007 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1069 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1318 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-11 13:36:55.916961 spacetraders-0.2.1/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1035 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/types.py
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 spacetraders-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.2.2/README.md
+-rw-r--r--   0        0        0      522 2023-05-11 19:07:36.186983 spacetraders-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-11 19:02:43.376983 spacetraders-0.2.2/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 19:02:42.886983 spacetraders-0.2.2/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.936983 spacetraders-0.2.2/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     3818 2023-05-11 19:02:43.436983 spacetraders-0.2.2/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.936983 spacetraders-0.2.2/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4290 2023-05-11 19:02:43.446983 spacetraders-0.2.2/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5161 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4308 2023-05-11 19:02:43.446983 spacetraders-0.2.2/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4303 2023-05-11 19:02:43.476983 spacetraders-0.2.2/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     5015 2023-05-11 19:02:43.566983 spacetraders-0.2.2/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.896983 spacetraders-0.2.2/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     9240 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.936983 spacetraders-0.2.2/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4361 2023-05-11 19:02:43.446983 spacetraders-0.2.2/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4985 2023-05-11 19:02:43.466983 spacetraders-0.2.2/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.946983 spacetraders-0.2.2/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5255 2023-05-11 19:02:43.466983 spacetraders-0.2.2/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4513 2023-05-11 19:02:43.466983 spacetraders-0.2.2/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4566 2023-05-11 19:02:43.466983 spacetraders-0.2.2/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4610 2023-05-11 19:02:43.446983 spacetraders-0.2.2/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6213 2023-05-11 19:02:43.446983 spacetraders-0.2.2/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5356 2023-05-11 19:02:43.496983 spacetraders-0.2.2/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5540 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4236 2023-05-11 19:02:43.516983 spacetraders-0.2.2/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4338 2023-05-11 19:02:43.526983 spacetraders-0.2.2/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4970 2023-05-11 19:02:43.546983 spacetraders-0.2.2/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     6390 2023-05-11 19:02:43.536983 spacetraders-0.2.2/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4295 2023-05-11 19:02:43.526983 spacetraders-0.2.2/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     5002 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5292 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     6936 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5331 2023-05-11 19:02:43.546983 spacetraders-0.2.2/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5154 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5373 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4583 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4302 2023-05-11 19:02:43.566983 spacetraders-0.2.2/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5111 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5599 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5424 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     6332 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-11 19:02:42.936983 spacetraders-0.2.2/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4838 2023-05-11 19:02:43.676982 spacetraders-0.2.2/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5624 2023-05-11 19:02:43.636983 spacetraders-0.2.2/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4812 2023-05-11 19:02:43.616983 spacetraders-0.2.2/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4398 2023-05-11 19:02:43.606983 spacetraders-0.2.2/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5944 2023-05-11 19:02:43.666983 spacetraders-0.2.2/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4984 2023-05-11 19:02:43.686983 spacetraders-0.2.2/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4799 2023-05-11 19:02:43.696983 spacetraders-0.2.2/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4213 2023-05-11 19:02:43.716983 spacetraders-0.2.2/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-11 19:02:43.576983 spacetraders-0.2.2/spacetraders/errors.py
+-rw-r--r--   0        0        0    13081 2023-05-11 19:02:43.746983 spacetraders-0.2.2/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1216 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1246 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1397 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1422 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1609 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     1820 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1649 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1277 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1520 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-11 19:02:43.056983 spacetraders-0.2.2/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1675 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1198 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1416 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1251 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1372 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1263 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1390 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1275 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1408 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1204 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1345 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1221 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1222 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1265 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1239 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1174 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1285 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1228 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1479 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1208 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1187 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1404 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1358 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     2091 2023-05-11 19:02:43.146983 spacetraders-0.2.2/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1222 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1248 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1122 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1229 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1116 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1223 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1123 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1110 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1108 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1133 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1109 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1209 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1209 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1157 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1122 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     1110 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1241 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1217 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1213 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1114 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1179 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1132 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1516 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1105 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1180 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1382 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2254 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1817 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-11 19:02:43.066983 spacetraders-0.2.2/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2093 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-11 19:02:43.076983 spacetraders-0.2.2/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1143 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1113 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1204 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1391 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1251 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1178 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1316 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1161 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1299 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1431 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1148 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1270 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1204 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1394 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1192 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1344 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1356 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-11 19:02:43.126983 spacetraders-0.2.2/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1179 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1555 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     2315 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1081 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1078 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1086 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1084 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1429 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2187 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1251 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1415 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1132 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3087 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1431 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1447 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2160 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-11 19:02:43.036983 spacetraders-0.2.2/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1797 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-11 19:02:43.126983 spacetraders-0.2.2/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2192 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-11 19:02:43.046983 spacetraders-0.2.2/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1501 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1324 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1830 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-11 19:02:43.076983 spacetraders-0.2.2/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1809 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-11 19:02:43.136983 spacetraders-0.2.2/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-11 19:02:43.136983 spacetraders-0.2.2/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2034 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-11 19:02:43.046983 spacetraders-0.2.2/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1875 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1434 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-11 19:02:43.076983 spacetraders-0.2.2/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1848 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-11 19:02:43.056983 spacetraders-0.2.2/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1183 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-11 19:02:43.126983 spacetraders-0.2.2/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1263 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     1994 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1224 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1224 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1430 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1406 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-11 19:02:43.116983 spacetraders-0.2.2/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-11 19:02:43.036983 spacetraders-0.2.2/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     1884 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2417 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1134 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1682 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2212 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1146 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-11 19:02:43.056983 spacetraders-0.2.2/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1672 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1049 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-11 19:02:43.056983 spacetraders-0.2.2/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1289 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1236 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-11 19:02:43.116983 spacetraders-0.2.2/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1299 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1168 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1241 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1105 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1180 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1383 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2173 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1053 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1115 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1364 2023-05-11 19:07:21.436983 spacetraders-0.2.2/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-11 19:02:43.146983 spacetraders-0.2.2/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-11 19:02:43.056983 spacetraders-0.2.2/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1035 2023-05-11 19:02:44.006983 spacetraders-0.2.2/spacetraders/types.py
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 spacetraders-0.2.2/PKG-INFO
```

### Comparing `spacetraders-0.2.1/README.md` & `spacetraders-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/pyproject.toml` & `spacetraders-0.2.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.2.1"
+version = "0.2.2"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.2.1/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.2.2/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.2.2/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.2.2/spacetraders/api/contracts/deliver_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/contracts/{contractId}/deliver".format(
         _client.base_url, contractId=contract_id
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -78,15 +78,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DeliverContractResponse200]
     """
 
-    json_body = DeliverContractJsonBody(**json_body)
+    json_body = DeliverContractJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
         json_body=json_body,
     )
 
@@ -145,15 +145,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DeliverContractResponse200]
     """
 
-    json_body = DeliverContractJsonBody(**json_body)
+    json_body = DeliverContractJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.2.2/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.2.2/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.2.2/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/default/register.py` & `spacetraders-0.2.2/spacetraders/api/default/register.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     json_body: RegisterJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/register".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -95,15 +95,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RegisterResponse201]
     """
 
-    json_body = RegisterJsonBody(**json_body)
+    json_body = RegisterJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
@@ -200,15 +200,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RegisterResponse201]
     """
 
-    json_body = RegisterJsonBody(**json_body)
+    json_body = RegisterJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         _client=_client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
```

### Comparing `spacetraders-0.2.1/spacetraders/api/factions/get_faction.py` & `spacetraders-0.2.2/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/factions/get_factions.py` & `spacetraders-0.2.2/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.2.2/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.2.2/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.2.2/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.2.2/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.2.2/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.2.2/spacetraders/api/fleet/extract_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/extract".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -79,15 +79,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ExtractResourcesResponse201]
     """
 
-    json_body = ExtractResourcesJsonBody(**json_body)
+    json_body = ExtractResourcesJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -148,15 +148,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ExtractResourcesResponse201]
     """
 
-    json_body = ExtractResourcesJsonBody(**json_body)
+    json_body = ExtractResourcesJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.2.2/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.2.2/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.2.2/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.2.2/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/jettison.py` & `spacetraders-0.2.2/spacetraders/api/fleet/jettison.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/jettison".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -78,15 +78,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JettisonResponse200]
     """
 
-    json_body = JettisonJsonBody(**json_body)
+    json_body = JettisonJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -145,15 +145,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JettisonResponse200]
     """
 
-    json_body = JettisonJsonBody(**json_body)
+    json_body = JettisonJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/jump_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/jump".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -79,15 +79,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JumpShipResponse200]
     """
 
-    json_body = JumpShipJsonBody(**json_body)
+    json_body = JumpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -148,15 +148,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JumpShipResponse200]
     """
 
-    json_body = JumpShipJsonBody(**json_body)
+    json_body = JumpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/navigate_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/navigate".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -85,15 +85,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NavigateShipResponse200]
     """
 
-    json_body = NavigateShipJsonBody(**json_body)
+    json_body = NavigateShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -166,15 +166,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NavigateShipResponse200]
     """
 
-    json_body = NavigateShipJsonBody(**json_body)
+    json_body = NavigateShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.2.2/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/nav".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -78,15 +78,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PatchShipNavResponse200]
     """
 
-    json_body = PatchShipNavJsonBody(**json_body)
+    json_body = PatchShipNavJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -145,15 +145,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PatchShipNavResponse200]
     """
 
-    json_body = PatchShipNavJsonBody(**json_body)
+    json_body = PatchShipNavJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.2.2/spacetraders/api/fleet/purchase_cargo.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     url = "{}/my/ships/{shipSymbol}/purchase".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -82,15 +82,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseCargoPurchaseCargo201Response]
     """
 
-    json_body = PurchaseCargoPurchaseCargoRequest(**json_body)
+    json_body = PurchaseCargoPurchaseCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -149,15 +149,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseCargoPurchaseCargo201Response]
     """
 
-    json_body = PurchaseCargoPurchaseCargoRequest(**json_body)
+    json_body = PurchaseCargoPurchaseCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/purchase_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     json_body: PurchaseShipJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships".format(_client.base_url)
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -73,15 +73,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseShipResponse201]
     """
 
-    json_body = PurchaseShipJsonBody(**json_body)
+    json_body = PurchaseShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
@@ -134,15 +134,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseShipResponse201]
     """
 
-    json_body = PurchaseShipJsonBody(**json_body)
+    json_body = PurchaseShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         _client=_client,
         json_body=json_body,
     )
 
     async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.2.2/spacetraders/api/fleet/sell_cargo.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/sell".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -78,15 +78,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SellCargoSellCargo201Response]
     """
 
-    json_body = SellCargoSellCargoRequest(**json_body)
+    json_body = SellCargoSellCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -145,15 +145,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SellCargoSellCargo201Response]
     """
 
-    json_body = SellCargoSellCargoRequest(**json_body)
+    json_body = SellCargoSellCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.2.2/spacetraders/api/fleet/ship_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     url = "{}/my/ships/{shipSymbol}/refine".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -81,15 +81,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ShipRefineShipRefine200Response]
     """
 
-    json_body = ShipRefineJsonBody(**json_body)
+    json_body = ShipRefineJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -150,15 +150,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ShipRefineShipRefine200Response]
     """
 
-    json_body = ShipRefineJsonBody(**json_body)
+    json_body = ShipRefineJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.2.2/spacetraders/api/fleet/transfer_cargo.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     url = "{}/my/ships/{shipSymbol}/transfer".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -82,15 +82,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[TransferCargoTransferCargo200Response]
     """
 
-    json_body = TransferCargoTransferCargoRequest(**json_body)
+    json_body = TransferCargoTransferCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -149,15 +149,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[TransferCargoTransferCargo200Response]
     """
 
-    json_body = TransferCargoTransferCargoRequest(**json_body)
+    json_body = TransferCargoTransferCargoRequest.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.2.2/spacetraders/api/fleet/warp_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     url = "{}/my/ships/{shipSymbol}/warp".format(
         _client.base_url, shipSymbol=ship_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.dict()
+    json_json_body = json_body.dict(by_alias=True)
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
         "timeout": _client.get_timeout(),
@@ -82,15 +82,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[WarpShipResponse200]
     """
 
-    json_body = WarpShipJsonBody(**json_body)
+    json_body = WarpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
 
@@ -157,15 +157,15 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[WarpShipResponse200]
     """
 
-    json_body = WarpShipJsonBody(**json_body)
+    json_body = WarpShipJsonBody.parse_obj(json_body)
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
         _client=_client,
         json_body=json_body,
     )
```

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_market.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_system.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_systems.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_systems.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.2.2/spacetraders/api/systems/get_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/client.py` & `spacetraders-0.2.2/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/__init__.py` & `spacetraders-0.2.2/spacetraders/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.2.2/spacetraders/models/accept_contract_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "AcceptContractResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,30 +15,31 @@
 import attr
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
 from ..models.contract import Contract
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="AcceptContractResponse200Data")
+T = TypeVar("T", bound="FulfillContractResponse200Data")
 
 
-class AcceptContractResponse200Data(BaseModel):
+class FulfillContractResponse200Data(BaseModel):
     """
     Attributes:
         agent (Agent):
         contract (Contract):
     """
 
     agent: "Agent" = Field(alias="agent")
     contract: "Contract" = Field(alias="contract")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/agent.py` & `spacetraders-0.2.2/spacetraders/models/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     symbol: str = Field(alias="symbol")
     headquarters: str = Field(alias="headquarters")
     credits_: int = Field(alias="credits")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/chart.py` & `spacetraders-0.2.2/spacetraders/models/chart.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     waypoint_symbol: Union[Unset, str] = UNSET
     submitted_by: Union[Unset, str] = UNSET
     submitted_on: Union[Unset, datetime.datetime] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/connected_system.py` & `spacetraders-0.2.2/spacetraders/models/connected_system.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     y: int = Field(alias="y")
     distance: int = Field(alias="distance")
     faction_symbol: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/contract.py` & `spacetraders-0.2.2/spacetraders/models/contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     expiration: datetime.datetime = Field(alias="expiration")
     accepted: bool = False
     fulfilled: bool = False
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.2.2/spacetraders/models/contract_deliver_good.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     destination_symbol: str = Field(alias="destinationSymbol")
     units_required: int = Field(alias="unitsRequired")
     units_fulfilled: int = Field(alias="unitsFulfilled")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/contract_payment.py` & `spacetraders-0.2.2/spacetraders/models/contract_payment.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     on_accepted: int = Field(alias="onAccepted")
     on_fulfilled: int = Field(alias="onFulfilled")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/contract_terms.py` & `spacetraders-0.2.2/spacetraders/models/contract_terms.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     deadline: datetime.datetime = Field(alias="deadline")
     payment: "ContractPayment" = Field(alias="payment")
     deliver: Union[Unset, List["ContractDeliverGood"]] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/cooldown.py` & `spacetraders-0.2.2/spacetraders/models/cooldown.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     total_seconds: int = Field(alias="totalSeconds")
     remaining_seconds: int = Field(alias="remainingSeconds")
     expiration: datetime.datetime = Field(alias="expiration")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.2.2/spacetraders/models/create_chart_response_201.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "CreateChartResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/purchase_ship_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,40 +5,39 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.chart import Chart
-from ..models.waypoint import Waypoint
+from ..models.ship_type import ShipType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateChartResponse201Data")
+T = TypeVar("T", bound="PurchaseShipJsonBody")
 
 
-class CreateChartResponse201Data(BaseModel):
+class PurchaseShipJsonBody(BaseModel):
     """
     Attributes:
-        chart (Chart): The chart of a system or waypoint, which makes the location visible to other agents.
-        waypoint (Waypoint): A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
+        ship_type (ShipType):
+        waypoint_symbol (str): The symbol of the waypoint you want to purchase the ship at.
     """
 
-    chart: "Chart" = Field(alias="chart")
-    waypoint: "Waypoint" = Field(alias="waypoint")
+    ship_type: ShipType = Field(alias="shipType")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files 9% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "CreateShipShipScanResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,33 +12,34 @@
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..models.cooldown import Cooldown
-from ..models.scanned_ship import ScannedShip
+from ..models.scanned_waypoint import ScannedWaypoint
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateShipShipScanResponse201Data")
+T = TypeVar("T", bound="CreateShipWaypointScanResponse201Data")
 
 
-class CreateShipShipScanResponse201Data(BaseModel):
+class CreateShipWaypointScanResponse201Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        ships (List['ScannedShip']):
+        waypoints (List['ScannedWaypoint']):
     """
 
     cooldown: "Cooldown" = Field(alias="cooldown")
-    ships: List["ScannedShip"] = Field(alias="ships")
+    waypoints: List["ScannedWaypoint"] = Field(alias="waypoints")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "CreateShipSystemScanResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     systems: List["ScannedSystem"] = Field(alias="systems")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "CreateShipWaypointScanResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/create_chart_response_201_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,34 +11,35 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.cooldown import Cooldown
-from ..models.scanned_waypoint import ScannedWaypoint
+from ..models.chart import Chart
+from ..models.waypoint import Waypoint
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="CreateShipWaypointScanResponse201Data")
+T = TypeVar("T", bound="CreateChartResponse201Data")
 
 
-class CreateShipWaypointScanResponse201Data(BaseModel):
+class CreateChartResponse201Data(BaseModel):
     """
     Attributes:
-        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        waypoints (List['ScannedWaypoint']):
+        chart (Chart): The chart of a system or waypoint, which makes the location visible to other agents.
+        waypoint (Waypoint): A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
     """
 
-    cooldown: "Cooldown" = Field(alias="cooldown")
-    waypoints: List["ScannedWaypoint"] = Field(alias="waypoints")
+    chart: "Chart" = Field(alias="chart")
+    waypoint: "Waypoint" = Field(alias="waypoint")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.2.2/spacetraders/models/create_survey_response_201.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "CreateSurveyResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/create_survey_response_201_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     cooldown: "Cooldown" = Field(alias="cooldown")
     surveys: List["Survey"] = Field(alias="surveys")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.2.2/spacetraders/models/deliver_contract_json_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ship_symbol: str = Field(alias="shipSymbol")
     trade_symbol: str = Field(alias="tradeSymbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.2.2/spacetraders/models/deliver_contract_response_200.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "DeliverContractResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     contract: "Contract" = Field(alias="contract")
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.2.2/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "DockShipDockShip200ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.2.2/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,36 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
+from ..models.ship_fuel import ShipFuel
 from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DockShipDockShip200ResponseData")
+T = TypeVar("T", bound="NavigateShipResponse200Data")
 
 
-class DockShipDockShip200ResponseData(BaseModel):
+class NavigateShipResponse200Data(BaseModel):
     """
     Attributes:
+        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
+            or action.
         nav (ShipNav): The navigation information of the ship.
     """
 
+    fuel: "ShipFuel" = Field(alias="fuel")
     nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.2.2/spacetraders/models/extract_resources_json_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     survey: Union[Unset, "Survey"] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.2.2/spacetraders/models/extract_resources_response_201.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "ExtractResourcesResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/extract_resources_response_201_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     cooldown: "Cooldown" = Field(alias="cooldown")
     extraction: "Extraction" = Field(alias="extraction")
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/extraction.py` & `spacetraders-0.2.2/spacetraders/models/extraction.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 
     ship_symbol: str = Field(alias="shipSymbol")
     yield_: "ExtractionYield" = Field(alias="yield")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/extraction_yield.py` & `spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,30 +12,31 @@
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExtractionYield")
+T = TypeVar("T", bound="SellCargoSellCargoRequest")
 
 
-class ExtractionYield(BaseModel):
+class SellCargoSellCargoRequest(BaseModel):
     """
     Attributes:
         symbol (str):
-        units (int): The number of units extracted that were placed into the ship's cargo hold.
+        units (int):
     """
 
     symbol: str = Field(alias="symbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/faction.py` & `spacetraders-0.2.2/spacetraders/models/faction.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     description: str = Field(alias="description")
     headquarters: str = Field(alias="headquarters")
     traits: List["FactionTrait"] = Field(alias="traits")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/faction_trait.py` & `spacetraders-0.2.2/spacetraders/models/get_faction_response_200.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,40 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.faction_trait_symbol import FactionTraitSymbol
+from ..models.faction import Faction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FactionTrait")
+T = TypeVar("T", bound="GetFactionResponse200")
 
 
-class FactionTrait(BaseModel):
+class GetFactionResponse200(BaseModel):
     """
     Attributes:
-        symbol (FactionTraitSymbol): The unique identifier of the trait.
-        name (str): The name of the trait.
-        description (str): A description of the trait.
+        data (Faction):
     """
 
-    symbol: FactionTraitSymbol = Field(alias="symbol")
-    name: str = Field(alias="name")
-    description: str = Field(alias="description")
+    data: "Faction" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.2.2/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.2.2/spacetraders/models/fulfill_contract_response_200.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "FulfillContractResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/accept_contract_response_200_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,30 +15,31 @@
 import attr
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
 from ..models.contract import Contract
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="FulfillContractResponse200Data")
+T = TypeVar("T", bound="AcceptContractResponse200Data")
 
 
-class FulfillContractResponse200Data(BaseModel):
+class AcceptContractResponse200Data(BaseModel):
     """
     Attributes:
         agent (Agent):
         contract (Contract):
     """
 
     agent: "Agent" = Field(alias="agent")
     contract: "Contract" = Field(alias="contract")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_contract_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "Contract" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_contracts_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     data: List["Contract"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.2.2/spacetraders/models/system_faction.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,36 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.faction import Faction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetFactionResponse200")
+T = TypeVar("T", bound="SystemFaction")
 
 
-class GetFactionResponse200(BaseModel):
+class SystemFaction(BaseModel):
     """
     Attributes:
-        data (Faction):
+        symbol (str):
     """
 
-    data: "Faction" = Field(alias="data")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_factions_response_200.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     data: List["Faction"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_jump_gate_response_200.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "JumpGate" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_market_response_200.py` & `spacetraders-0.2.2/spacetraders/models/waypoint_faction.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,37 +5,36 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.market import Market
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetMarketResponse200")
+T = TypeVar("T", bound="WaypointFaction")
 
 
-class GetMarketResponse200(BaseModel):
+class WaypointFaction(BaseModel):
     """
     Attributes:
-        data (Market):
+        symbol (str):
     """
 
-    data: "Market" = Field(alias="data")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_my_agent_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "Agent" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.2.2/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_cargo import ShipCargo
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetMyShipCargoResponse200")
+T = TypeVar("T", bound="PatchShipNavResponse200")
 
 
-class GetMyShipCargoResponse200(BaseModel):
+class PatchShipNavResponse200(BaseModel):
     """
     Attributes:
-        data (ShipCargo):
+        data (ShipNav): The navigation information of the ship.
     """
 
-    data: "ShipCargo" = Field(alias="data")
+    data: "ShipNav" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_shipyard_response_200.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship import Ship
+from ..models.shipyard import Shipyard
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetMyShipResponse200")
+T = TypeVar("T", bound="GetShipyardResponse200")
 
 
-class GetMyShipResponse200(BaseModel):
+class GetShipyardResponse200(BaseModel):
     """
     Attributes:
-        data (Ship): A ship
+        data (Shipyard):
     """
 
-    data: "Ship" = Field(alias="data")
+    data: "Shipyard" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.2.2/spacetraders/models/navigate_ship_json_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,40 +5,36 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.meta import Meta
-from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetMyShipsResponse200")
+T = TypeVar("T", bound="NavigateShipJsonBody")
 
 
-class GetMyShipsResponse200(BaseModel):
+class NavigateShipJsonBody(BaseModel):
     """
     Attributes:
-        data (List['Ship']):
-        meta (Meta):
+        waypoint_symbol (str): The target destination.
     """
 
-    data: List["Ship"] = Field(alias="data")
-    meta: "Meta" = Field(alias="meta")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "Cooldown" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_ship_nav_response_200.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "ShipNav" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,37 +5,40 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.shipyard import Shipyard
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetShipyardResponse200")
+T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
 
 
-class GetShipyardResponse200(BaseModel):
+class TransferCargoTransferCargoRequest(BaseModel):
     """
     Attributes:
-        data (Shipyard):
+        trade_symbol (str):
+        units (int):
+        ship_symbol (str):
     """
 
-    data: "Shipyard" = Field(alias="data")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
+    ship_symbol: str = Field(alias="shipSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_system_response_200.py` & `spacetraders-0.2.2/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,31 +11,34 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.system import System
+from ..models.orbit_ship_orbit_ship_200_response_data import (
+    OrbitShipOrbitShip200ResponseData,
+)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="GetSystemResponse200")
+T = TypeVar("T", bound="OrbitShipOrbitShip200Response")
 
 
-class GetSystemResponse200(BaseModel):
+class OrbitShipOrbitShip200Response(BaseModel):
     """
     Attributes:
-        data (System):
+        data (OrbitShipOrbitShip200ResponseData):
     """
 
-    data: "System" = Field(alias="data")
+    data: "OrbitShipOrbitShip200ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     data: List["Waypoint"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_systems_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
     data: List["System"] = Field(alias="data")
     meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_waypoint_response_200.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "Waypoint" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jettison_json_body.py` & `spacetraders-0.2.2/spacetraders/models/jettison_json_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
     symbol: str = Field(alias="symbol")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jettison_response_200.py` & `spacetraders-0.2.2/spacetraders/models/jettison_response_200.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "JettisonResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/jettison_response_200_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jump_gate.py` & `spacetraders-0.2.2/spacetraders/models/jump_gate.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     jump_range: float = Field(alias="jumpRange")
     connected_systems: List["ConnectedSystem"] = Field(alias="connectedSystems")
     faction_symbol: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.2.2/spacetraders/models/jump_ship_json_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,15 @@
     """
 
     system_symbol: str = Field(alias="systemSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.2.2/spacetraders/models/jump_ship_response_200.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "JumpShipResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,41 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    Union,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.cooldown import Cooldown
 from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JumpShipResponse200Data")
+T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
 
 
-class JumpShipResponse200Data(BaseModel):
+class OrbitShipOrbitShip200ResponseData(BaseModel):
     """
     Attributes:
-        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
-        nav (Union[Unset, ShipNav]): The navigation information of the ship.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    cooldown: "Cooldown" = Field(alias="cooldown")
-    nav: Union[Unset, "ShipNav"] = UNSET
+    nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/market.py` & `spacetraders-0.2.2/spacetraders/models/market.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     exchange: List["TradeGood"] = Field(alias="exchange")
     transactions: Union[Unset, List["MarketTransaction"]] = UNSET
     trade_goods: Union[Unset, List["MarketTradeGood"]] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/market_trade_good.py` & `spacetraders-0.2.2/spacetraders/models/market_trade_good.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     supply: MarketTradeGoodSupply = Field(alias="supply")
     purchase_price: int = Field(alias="purchasePrice")
     sell_price: int = Field(alias="sellPrice")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/market_transaction.py` & `spacetraders-0.2.2/spacetraders/models/market_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     price_per_unit: int = Field(alias="pricePerUnit")
     total_price: int = Field(alias="totalPrice")
     timestamp: datetime.datetime = Field(alias="timestamp")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/meta.py` & `spacetraders-0.2.2/spacetraders/models/register_response_201_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,39 +5,49 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.contract import Contract
+from ..models.faction import Faction
+from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Meta")
+T = TypeVar("T", bound="RegisterResponse201Data")
 
 
-class Meta(BaseModel):
+class RegisterResponse201Data(BaseModel):
     """
     Attributes:
-        total (int):
-        page (int):
-        limit (int):
+        agent (Agent):
+        contract (Contract):
+        faction (Faction):
+        ship (Ship): A ship
+        token (str): A Bearer token for accessing secured API endpoints.
     """
 
-    total: int = Field(alias="total")
-    page: int = Field(alias="page")
-    limit: int = Field(alias="limit")
+    agent: "Agent" = Field(alias="agent")
+    contract: "Contract" = Field(alias="contract")
+    faction: "Faction" = Field(alias="faction")
+    ship: "Ship" = Field(alias="ship")
+    token: str = Field(alias="token")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.2.2/spacetraders/models/warp_ship_json_body.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,28 +12,29 @@
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="NavigateShipJsonBody")
+T = TypeVar("T", bound="WarpShipJsonBody")
 
 
-class NavigateShipJsonBody(BaseModel):
+class WarpShipJsonBody(BaseModel):
     """
     Attributes:
         waypoint_symbol (str): The target destination.
     """
 
     waypoint_symbol: str = Field(alias="waypointSymbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.2.2/spacetraders/models/refuel_ship_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.navigate_ship_response_200_data import NavigateShipResponse200Data
+from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="NavigateShipResponse200")
+T = TypeVar("T", bound="RefuelShipResponse200")
 
 
-class NavigateShipResponse200(BaseModel):
+class RefuelShipResponse200(BaseModel):
     """
     Attributes:
-        data (NavigateShipResponse200Data):
+        data (RefuelShipResponse200Data):
     """
 
-    data: "NavigateShipResponse200Data" = Field(alias="data")
+    data: "RefuelShipResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/warp_ship_response_200_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,31 +15,32 @@
 import attr
 from pydantic import BaseModel, Field
 
 from ..models.ship_fuel import ShipFuel
 from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="NavigateShipResponse200Data")
+T = TypeVar("T", bound="WarpShipResponse200Data")
 
 
-class NavigateShipResponse200Data(BaseModel):
+class WarpShipResponse200Data(BaseModel):
     """
     Attributes:
         fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
             or action.
         nav (ShipNav): The navigation information of the ship.
     """
 
     fuel: "ShipFuel" = Field(alias="fuel")
     nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,39 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.orbit_ship_orbit_ship_200_response_data import (
-    OrbitShipOrbitShip200ResponseData,
-)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OrbitShipOrbitShip200Response")
+T = TypeVar("T", bound="PurchaseCargoPurchaseCargoRequest")
 
 
-class OrbitShipOrbitShip200Response(BaseModel):
+class PurchaseCargoPurchaseCargoRequest(BaseModel):
     """
     Attributes:
-        data (OrbitShipOrbitShip200ResponseData):
+        symbol (str):
+        units (int):
     """
 
-    data: "OrbitShipOrbitShip200ResponseData" = Field(alias="data")
+    symbol: str = Field(alias="symbol")
+    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.2.2/spacetraders/models/register_json_body.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,37 +5,39 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_nav import ShipNav
+from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
+T = TypeVar("T", bound="RegisterJsonBody")
 
 
-class OrbitShipOrbitShip200ResponseData(BaseModel):
+class RegisterJsonBody(BaseModel):
     """
     Attributes:
-        nav (ShipNav): The navigation information of the ship.
+        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
+        symbol (str): How other agents will see your ships and information. Example: BADGER.
     """
 
-    nav: "ShipNav" = Field(alias="nav")
+    faction: RegisterJsonBodyFaction = Field(alias="faction")
+    symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.2.2/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     """
 
     flight_mode: Union[Unset, ShipNavFlightMode] = ShipNavFlightMode.CRUISE
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.2.2/spacetraders/models/get_my_ship_response_200.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_nav import ShipNav
+from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PatchShipNavResponse200")
+T = TypeVar("T", bound="GetMyShipResponse200")
 
 
-class PatchShipNavResponse200(BaseModel):
+class GetMyShipResponse200(BaseModel):
     """
     Attributes:
-        data (ShipNav): The navigation information of the ship.
+        data (Ship): A ship
     """
 
-    data: "ShipNav" = Field(alias="data")
+    data: "Ship" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "PurchaseCargoPurchaseCargo201ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
 from ..models.market_transaction import MarketTransaction
 from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PurchaseCargoPurchaseCargo201ResponseData")
+T = TypeVar("T", bound="SellCargoSellCargo201ResponseData")
 
 
-class PurchaseCargoPurchaseCargo201ResponseData(BaseModel):
+class SellCargoSellCargo201ResponseData(BaseModel):
     """
     Attributes:
         agent (Agent):
         cargo (ShipCargo):
         transaction (MarketTransaction):
     """
 
     agent: "Agent" = Field(alias="agent")
     cargo: "ShipCargo" = Field(alias="cargo")
     transaction: "MarketTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.2.2/spacetraders/models/scanned_ship_frame.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PurchaseCargoPurchaseCargoRequest")
+T = TypeVar("T", bound="ScannedShipFrame")
 
 
-class PurchaseCargoPurchaseCargoRequest(BaseModel):
-    """
+class ScannedShipFrame(BaseModel):
+    """The frame of the ship.
+
     Attributes:
         symbol (str):
-        units (int):
     """
 
     symbol: str = Field(alias="symbol")
-    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.2.2/spacetraders/models/shipyard_ship_types_item.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,38 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    Union,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..models.ship_type import ShipType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PurchaseShipJsonBody")
+T = TypeVar("T", bound="ShipyardShipTypesItem")
 
 
-class PurchaseShipJsonBody(BaseModel):
+class ShipyardShipTypesItem(BaseModel):
     """
     Attributes:
-        ship_type (ShipType):
-        waypoint_symbol (str): The symbol of the waypoint you want to purchase the ship at.
+        type (Union[Unset, ShipType]):
     """
 
-    ship_type: ShipType = Field(alias="shipType")
-    waypoint_symbol: str = Field(alias="waypointSymbol")
+    type: Union[Unset, ShipType] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.2.2/spacetraders/models/purchase_ship_response_201.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "PurchaseShipResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     agent: "Agent" = Field(alias="agent")
     ship: "Ship" = Field(alias="ship")
     transaction: "ShipyardTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.2.2/spacetraders/models/warp_ship_response_200.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,31 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
+from ..models.warp_ship_response_200_data import WarpShipResponse200Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RefuelShipResponse200")
+T = TypeVar("T", bound="WarpShipResponse200")
 
 
-class RefuelShipResponse200(BaseModel):
+class WarpShipResponse200(BaseModel):
     """
     Attributes:
-        data (RefuelShipResponse200Data):
+        data (WarpShipResponse200Data):
     """
 
-    data: "RefuelShipResponse200Data" = Field(alias="data")
+    data: "WarpShipResponse200Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
     agent: "Agent" = Field(alias="agent")
     fuel: "ShipFuel" = Field(alias="fuel")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/register_json_body.py` & `spacetraders-0.2.2/spacetraders/models/extraction_yield.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,33 +10,33 @@
     Type,
     TypeVar,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegisterJsonBody")
+T = TypeVar("T", bound="ExtractionYield")
 
 
-class RegisterJsonBody(BaseModel):
+class ExtractionYield(BaseModel):
     """
     Attributes:
-        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
-        symbol (str): How other agents will see your ships and information. Example: BADGER.
+        symbol (str):
+        units (int): The number of units extracted that were placed into the ship's cargo hold.
     """
 
-    faction: RegisterJsonBodyFaction = Field(alias="faction")
     symbol: str = Field(alias="symbol")
+    units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/register_response_201.py` & `spacetraders-0.2.2/spacetraders/models/register_response_201.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     data: "RegisterResponse201Data" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/register_response_201_data.py` & `spacetraders-0.2.2/spacetraders/models/get_my_ships_response_200.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,42 +11,35 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.agent import Agent
-from ..models.contract import Contract
-from ..models.faction import Faction
+from ..models.meta import Meta
 from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegisterResponse201Data")
+T = TypeVar("T", bound="GetMyShipsResponse200")
 
 
-class RegisterResponse201Data(BaseModel):
+class GetMyShipsResponse200(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
-        faction (Faction):
-        ship (Ship): A ship
-        token (str): A Bearer token for accessing secured API endpoints.
+        data (List['Ship']):
+        meta (Meta):
     """
 
-    agent: "Agent" = Field(alias="agent")
-    contract: "Contract" = Field(alias="contract")
-    faction: "Faction" = Field(alias="faction")
-    ship: "Ship" = Field(alias="ship")
-    token: str = Field(alias="token")
+    data: List["Ship"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_ship.py` & `spacetraders-0.2.2/spacetraders/models/scanned_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,15 @@
     frame: Union[Unset, "ScannedShipFrame"] = UNSET
     reactor: Union[Unset, "ScannedShipReactor"] = UNSET
     mounts: Union[Unset, List["ScannedShipMountsItem"]] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.2.2/spacetraders/models/scanned_ship_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.2.2/spacetraders/models/ship_fuel_consumed.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,45 @@
+import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import attr
+from dateutil.parser import isoparse
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedShipFrame")
+T = TypeVar("T", bound="ShipFuelConsumed")
 
 
-class ScannedShipFrame(BaseModel):
-    """The frame of the ship.
-
+class ShipFuelConsumed(BaseModel):
+    """
     Attributes:
-        symbol (str):
+        amount (int): The amount of fuel consumed by the most recent transit or action.
+        timestamp (datetime.datetime): The time at which the fuel was consumed.
     """
 
-    symbol: str = Field(alias="symbol")
+    amount: int = Field(alias="amount")
+    timestamp: datetime.datetime = Field(alias="timestamp")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.2.2/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.2.2/spacetraders/models/scanned_ship_reactor.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_system.py` & `spacetraders-0.2.2/spacetraders/models/system_waypoint.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,41 +10,38 @@
     Type,
     TypeVar,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.system_type import SystemType
+from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedSystem")
+T = TypeVar("T", bound="SystemWaypoint")
 
 
-class ScannedSystem(BaseModel):
+class SystemWaypoint(BaseModel):
     """
     Attributes:
         symbol (str):
-        sector_symbol (str):
-        type (SystemType): The type of waypoint.
+        type (WaypointType): The type of waypoint.
         x (int):
         y (int):
-        distance (int):
     """
 
     symbol: str = Field(alias="symbol")
-    sector_symbol: str = Field(alias="sectorSymbol")
-    type: SystemType = Field(alias="type")
+    type: WaypointType = Field(alias="type")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
-    distance: int = Field(alias="distance")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.2.2/spacetraders/models/waypoint.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from ..models.chart import Chart
 from ..models.waypoint_faction import WaypointFaction
 from ..models.waypoint_orbital import WaypointOrbital
 from ..models.waypoint_trait import WaypointTrait
 from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedWaypoint")
+T = TypeVar("T", bound="Waypoint")
 
 
-class ScannedWaypoint(BaseModel):
+class Waypoint(BaseModel):
     """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
 
     Attributes:
         symbol (str):
         type (WaypointType): The type of waypoint.
         system_symbol (str):
         x (int):
@@ -51,14 +51,15 @@
     traits: List["WaypointTrait"] = Field(alias="traits")
     faction: Union[Unset, "WaypointFaction"] = UNSET
     chart: Union[Unset, "Chart"] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.2.2/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "SellCargoSellCargo201ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.2.2/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,32 +16,33 @@
 from pydantic import BaseModel, Field
 
 from ..models.agent import Agent
 from ..models.market_transaction import MarketTransaction
 from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SellCargoSellCargo201ResponseData")
+T = TypeVar("T", bound="PurchaseCargoPurchaseCargo201ResponseData")
 
 
-class SellCargoSellCargo201ResponseData(BaseModel):
+class PurchaseCargoPurchaseCargo201ResponseData(BaseModel):
     """
     Attributes:
         agent (Agent):
         cargo (ShipCargo):
         transaction (MarketTransaction):
     """
 
     agent: "Agent" = Field(alias="agent")
     cargo: "ShipCargo" = Field(alias="cargo")
     transaction: "MarketTransaction" = Field(alias="transaction")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.2.2/spacetraders/models/get_market_response_200.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
+from ..models.market import Market
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SellCargoSellCargoRequest")
+T = TypeVar("T", bound="GetMarketResponse200")
 
 
-class SellCargoSellCargoRequest(BaseModel):
+class GetMarketResponse200(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int):
+        data (Market):
     """
 
-    symbol: str = Field(alias="symbol")
-    units: int = Field(alias="units")
+    data: "Market" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship.py` & `spacetraders-0.2.2/spacetraders/models/ship.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     mounts: List["ShipMount"] = Field(alias="mounts")
     cargo: "ShipCargo" = Field(alias="cargo")
     fuel: "ShipFuel" = Field(alias="fuel")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_cargo.py` & `spacetraders-0.2.2/spacetraders/models/ship_cargo.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     capacity: int = Field(alias="capacity")
     units: int = Field(alias="units")
     inventory: List["ShipCargoItem"] = Field(alias="inventory")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.2.2/spacetraders/models/ship_cargo_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     name: str = Field(alias="name")
     description: str = Field(alias="description")
     units: int = Field(alias="units")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_crew.py` & `spacetraders-0.2.2/spacetraders/models/ship_crew.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     morale: int = Field(alias="morale")
     wages: int = Field(alias="wages")
     rotation: ShipCrewRotation = ShipCrewRotation.STRICT
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_engine.py` & `spacetraders-0.2.2/spacetraders/models/ship_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     speed: float = Field(alias="speed")
     requirements: "ShipRequirements" = Field(alias="requirements")
     condition: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_frame.py` & `spacetraders-0.2.2/spacetraders/models/ship_frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     fuel_capacity: int = Field(alias="fuelCapacity")
     requirements: "ShipRequirements" = Field(alias="requirements")
     condition: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.2.2/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_fuel.py` & `spacetraders-0.2.2/spacetraders/models/ship_fuel.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     current: int = Field(alias="current")
     capacity: int = Field(alias="capacity")
     consumed: Union[Unset, "ShipFuelConsumed"] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.2.2/spacetraders/models/meta.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
 )
 
 import attr
-from dateutil.parser import isoparse
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipFuelConsumed")
+T = TypeVar("T", bound="Meta")
 
 
-class ShipFuelConsumed(BaseModel):
+class Meta(BaseModel):
     """
     Attributes:
-        amount (int): The amount of fuel consumed by the most recent transit or action.
-        timestamp (datetime.datetime): The time at which the fuel was consumed.
+        total (int):
+        page (int):
+        limit (int):
     """
 
-    amount: int = Field(alias="amount")
-    timestamp: datetime.datetime = Field(alias="timestamp")
+    total: int = Field(alias="total")
+    page: int = Field(alias="page")
+    limit: int = Field(alias="limit")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_module.py` & `spacetraders-0.2.2/spacetraders/models/ship_mount.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,44 +12,45 @@
     Union,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_module_symbol import ShipModuleSymbol
+from ..models.ship_mount_deposits_item import ShipMountDepositsItem
+from ..models.ship_mount_symbol import ShipMountSymbol
 from ..models.ship_requirements import ShipRequirements
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipModule")
+T = TypeVar("T", bound="ShipMount")
 
 
-class ShipModule(BaseModel):
-    """A module can be installed in a ship and provides a set of capabilities such as storage space or quarters for crew.
-    Module installations are permanent.
-
-        Attributes:
-            symbol (ShipModuleSymbol):
-            name (str):
-            requirements (ShipRequirements): The requirements for installation on a ship
-            capacity (Union[Unset, int]):
-            range_ (Union[Unset, int]):
-            description (Union[Unset, str]):
+class ShipMount(BaseModel):
+    """A mount is installed on the exterier of a ship.
+
+    Attributes:
+        symbol (ShipMountSymbol):
+        name (str):
+        requirements (ShipRequirements): The requirements for installation on a ship
+        description (Union[Unset, str]):
+        strength (Union[Unset, int]):
+        deposits (Union[Unset, List[ShipMountDepositsItem]]):
     """
 
-    symbol: ShipModuleSymbol = Field(alias="symbol")
+    symbol: ShipMountSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     requirements: "ShipRequirements" = Field(alias="requirements")
-    capacity: Union[Unset, int] = UNSET
-    range_: Union[Unset, int] = UNSET
     description: Union[Unset, str] = UNSET
+    strength: Union[Unset, int] = UNSET
+    deposits: Union[Unset, List[ShipMountDepositsItem]] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.2.2/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_mount.py` & `spacetraders-0.2.2/spacetraders/models/ship_registration.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,50 +6,42 @@
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
     Union,
-    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_mount_deposits_item import ShipMountDepositsItem
-from ..models.ship_mount_symbol import ShipMountSymbol
-from ..models.ship_requirements import ShipRequirements
+from ..models.ship_role import ShipRole
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipMount")
+T = TypeVar("T", bound="ShipRegistration")
 
 
-class ShipMount(BaseModel):
-    """A mount is installed on the exterier of a ship.
+class ShipRegistration(BaseModel):
+    """The public registration information of the ship
 
     Attributes:
-        symbol (ShipMountSymbol):
-        name (str):
-        requirements (ShipRequirements): The requirements for installation on a ship
-        description (Union[Unset, str]):
-        strength (Union[Unset, int]):
-        deposits (Union[Unset, List[ShipMountDepositsItem]]):
+        name (str): The agent's registered name of the ship
+        role (ShipRole): The registered role of the ship
+        faction_symbol (Union[Unset, str]): The symbol of the faction the ship is registered with
     """
 
-    symbol: ShipMountSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
-    requirements: "ShipRequirements" = Field(alias="requirements")
-    description: Union[Unset, str] = UNSET
-    strength: Union[Unset, int] = UNSET
-    deposits: Union[Unset, List[ShipMountDepositsItem]] = UNSET
+    role: ShipRole = Field(alias="role")
+    faction_symbol: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.2.2/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.2.2/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_nav.py` & `spacetraders-0.2.2/spacetraders/models/ship_nav.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     route: "ShipNavRoute" = Field(alias="route")
     status: ShipNavStatus = Field(alias="status")
     flight_mode: ShipNavFlightMode = ShipNavFlightMode.CRUISE
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_nav_route.py` & `spacetraders-0.2.2/spacetraders/models/ship_nav_route.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     departure: "ShipNavRouteWaypoint" = Field(alias="departure")
     departure_time: datetime.datetime = Field(alias="departureTime")
     arrival: datetime.datetime = Field(alias="arrival")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.2.2/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     system_symbol: str = Field(alias="systemSymbol")
     x: int = Field(alias="x")
     y: int = Field(alias="y")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_reactor.py` & `spacetraders-0.2.2/spacetraders/models/ship_reactor.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     power_output: int = Field(alias="powerOutput")
     requirements: "ShipRequirements" = Field(alias="requirements")
     condition: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.2.2/spacetraders/models/ship_refine_json_body.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     produce: ShipRefineJsonBodyProduce = Field(alias="produce")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "ShipRefineShipRefine200ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.2.2/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,15 @@
     consumed: List["ShipRefineShipRefine200ResponseDataConsumedItem"] = Field(
         alias="consumed"
     )
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.2.2/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,38 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    Union,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataConsumedItem")
+T = TypeVar("T", bound="GetMyShipCargoResponse200")
 
 
-class ShipRefineShipRefine200ResponseDataConsumedItem(BaseModel):
+class GetMyShipCargoResponse200(BaseModel):
     """
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        data (ShipCargo):
     """
 
-    trade_symbol: Union[Unset, str] = UNSET
-    units: Union[Unset, int] = UNSET
+    data: "ShipCargo" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.2.2/spacetraders/models/get_system_response_200.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,38 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    Union,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
+from ..models.system import System
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataProducedItem")
+T = TypeVar("T", bound="GetSystemResponse200")
 
 
-class ShipRefineShipRefine200ResponseDataProducedItem(BaseModel):
+class GetSystemResponse200(BaseModel):
     """
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        data (System):
     """
 
-    trade_symbol: Union[Unset, str] = UNSET
-    units: Union[Unset, int] = UNSET
+    data: "System" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_registration.py` & `spacetraders-0.2.2/spacetraders/models/ship_requirements.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,36 +11,36 @@
     TypeVar,
     Union,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_role import ShipRole
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRegistration")
+T = TypeVar("T", bound="ShipRequirements")
 
 
-class ShipRegistration(BaseModel):
-    """The public registration information of the ship
+class ShipRequirements(BaseModel):
+    """The requirements for installation on a ship
 
     Attributes:
-        name (str): The agent's registered name of the ship
-        role (ShipRole): The registered role of the ship
-        faction_symbol (Union[Unset, str]): The symbol of the faction the ship is registered with
+        power (Union[Unset, int]): The amount of power required from the reactor.
+        crew (Union[Unset, int]): The number of crew required for operation.
+        slots (Union[Unset, int]): The number of module slots required for installation.
     """
 
-    name: str = Field(alias="name")
-    role: ShipRole = Field(alias="role")
-    faction_symbol: Union[Unset, str] = UNSET
+    power: Union[Unset, int] = UNSET
+    crew: Union[Unset, int] = UNSET
+    slots: Union[Unset, int] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/ship_type.py` & `spacetraders-0.2.2/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/shipyard.py` & `spacetraders-0.2.2/spacetraders/models/shipyard.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     ship_types: List["ShipyardShipTypesItem"] = Field(alias="shipTypes")
     transactions: Union[Unset, List["ShipyardTransaction"]] = UNSET
     ships: Union[Unset, List["ShipyardShip"]] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/shipyard_ship.py` & `spacetraders-0.2.2/spacetraders/models/shipyard_ship.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     modules: List["ShipModule"] = Field(alias="modules")
     mounts: List["ShipMount"] = Field(alias="mounts")
     type: Union[Unset, ShipType] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.2.2/spacetraders/models/trade_good.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,37 +5,41 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    Union,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_type import ShipType
+from ..models.trade_symbol import TradeSymbol
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipyardShipTypesItem")
+T = TypeVar("T", bound="TradeGood")
 
 
-class ShipyardShipTypesItem(BaseModel):
+class TradeGood(BaseModel):
     """
     Attributes:
-        type (Union[Unset, ShipType]):
+        symbol (TradeSymbol):
+        name (str):
+        description (str):
     """
 
-    type: Union[Unset, ShipType] = UNSET
+    symbol: TradeSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.2.2/spacetraders/models/shipyard_transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     price: int = Field(alias="price")
     agent_symbol: str = Field(alias="agentSymbol")
     timestamp: datetime.datetime = Field(alias="timestamp")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/survey.py` & `spacetraders-0.2.2/spacetraders/models/survey.py`

 * *Files 9% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     deposits: List["SurveyDeposit"] = Field(alias="deposits")
     expiration: datetime.datetime = Field(alias="expiration")
     size: SurveySize = Field(alias="size")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/survey_deposit.py` & `spacetraders-0.2.2/spacetraders/models/survey_deposit.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/system.py` & `spacetraders-0.2.2/spacetraders/models/system.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     y: int = Field(alias="y")
     waypoints: List["SystemWaypoint"] = Field(alias="waypoints")
     factions: List["SystemFaction"] = Field(alias="factions")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/system_faction.py` & `spacetraders-0.2.2/spacetraders/models/waypoint_orbital.py`

 * *Files 26% similar despite different names*

```diff
@@ -12,28 +12,30 @@
 )
 
 import attr
 from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SystemFaction")
+T = TypeVar("T", bound="WaypointOrbital")
 
 
-class SystemFaction(BaseModel):
-    """
+class WaypointOrbital(BaseModel):
+    """An orbital is another waypoint that orbits a parent waypoint.
+
     Attributes:
         symbol (str):
     """
 
     symbol: str = Field(alias="symbol")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/system_waypoint.py` & `spacetraders-0.2.2/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,42 +5,41 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.waypoint_type import WaypointType
+from ..models.cooldown import Cooldown
+from ..models.scanned_ship import ScannedShip
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SystemWaypoint")
+T = TypeVar("T", bound="CreateShipShipScanResponse201Data")
 
 
-class SystemWaypoint(BaseModel):
+class CreateShipShipScanResponse201Data(BaseModel):
     """
     Attributes:
-        symbol (str):
-        type (WaypointType): The type of waypoint.
-        x (int):
-        y (int):
+        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
+        ships (List['ScannedShip']):
     """
 
-    symbol: str = Field(alias="symbol")
-    type: WaypointType = Field(alias="type")
-    x: int = Field(alias="x")
-    y: int = Field(alias="y")
+    cooldown: "Cooldown" = Field(alias="cooldown")
+    ships: List["ScannedShip"] = Field(alias="ships")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/trade_good.py` & `spacetraders-0.2.2/spacetraders/models/scanned_system.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,35 +10,42 @@
     Type,
     TypeVar,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.trade_symbol import TradeSymbol
+from ..models.system_type import SystemType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="TradeGood")
+T = TypeVar("T", bound="ScannedSystem")
 
 
-class TradeGood(BaseModel):
+class ScannedSystem(BaseModel):
     """
     Attributes:
-        symbol (TradeSymbol):
-        name (str):
-        description (str):
+        symbol (str):
+        sector_symbol (str):
+        type (SystemType): The type of waypoint.
+        x (int):
+        y (int):
+        distance (int):
     """
 
-    symbol: TradeSymbol = Field(alias="symbol")
-    name: str = Field(alias="name")
-    description: str = Field(alias="description")
+    symbol: str = Field(alias="symbol")
+    sector_symbol: str = Field(alias="sectorSymbol")
+    type: SystemType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    distance: int = Field(alias="distance")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/trade_symbol.py` & `spacetraders-0.2.2/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     """
 
     data: "TransferCargoTransferCargo200ResponseData" = Field(alias="data")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.2.2/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files 14% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     """
 
     cargo: "ShipCargo" = Field(alias="cargo")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.2.2/spacetraders/models/ship_module.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,37 +5,52 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    Union,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.warp_ship_response_200_data import WarpShipResponse200Data
+from ..models.ship_module_symbol import ShipModuleSymbol
+from ..models.ship_requirements import ShipRequirements
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WarpShipResponse200")
+T = TypeVar("T", bound="ShipModule")
 
 
-class WarpShipResponse200(BaseModel):
-    """
-    Attributes:
-        data (WarpShipResponse200Data):
+class ShipModule(BaseModel):
+    """A module can be installed in a ship and provides a set of capabilities such as storage space or quarters for crew.
+    Module installations are permanent.
+
+        Attributes:
+            symbol (ShipModuleSymbol):
+            name (str):
+            requirements (ShipRequirements): The requirements for installation on a ship
+            capacity (Union[Unset, int]):
+            range_ (Union[Unset, int]):
+            description (Union[Unset, str]):
     """
 
-    data: "WarpShipResponse200Data" = Field(alias="data")
+    symbol: ShipModuleSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    requirements: "ShipRequirements" = Field(alias="requirements")
+    capacity: Union[Unset, int] = UNSET
+    range_: Union[Unset, int] = UNSET
+    description: Union[Unset, str] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.2.2/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,35 +11,32 @@
     TypeVar,
     cast,
 )
 
 import attr
 from pydantic import BaseModel, Field
 
-from ..models.ship_fuel import ShipFuel
 from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WarpShipResponse200Data")
+T = TypeVar("T", bound="DockShipDockShip200ResponseData")
 
 
-class WarpShipResponse200Data(BaseModel):
+class DockShipDockShip200ResponseData(BaseModel):
     """
     Attributes:
-        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
-            or action.
         nav (ShipNav): The navigation information of the ship.
     """
 
-    fuel: "ShipFuel" = Field(alias="fuel")
     nav: "ShipNav" = Field(alias="nav")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/waypoint.py` & `spacetraders-0.2.2/spacetraders/models/scanned_waypoint.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 from ..models.chart import Chart
 from ..models.waypoint_faction import WaypointFaction
 from ..models.waypoint_orbital import WaypointOrbital
 from ..models.waypoint_trait import WaypointTrait
 from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Waypoint")
+T = TypeVar("T", bound="ScannedWaypoint")
 
 
-class Waypoint(BaseModel):
+class ScannedWaypoint(BaseModel):
     """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
 
     Attributes:
         symbol (str):
         type (WaypointType): The type of waypoint.
         system_symbol (str):
         x (int):
@@ -51,14 +51,15 @@
     traits: List["WaypointTrait"] = Field(alias="traits")
     faction: Union[Unset, "WaypointFaction"] = UNSET
     chart: Union[Unset, "Chart"] = UNSET
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/waypoint_trait.py` & `spacetraders-0.2.2/spacetraders/models/waypoint_trait.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     symbol: WaypointTraitSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
+        allow_population_by_field_name = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.2.1/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.2.2/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/spacetraders/types.py` & `spacetraders-0.2.2/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.1/PKG-INFO` & `spacetraders-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.2.1
+Version: 0.2.2
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

