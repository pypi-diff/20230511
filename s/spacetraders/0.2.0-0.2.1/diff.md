# Comparing `tmp/spacetraders-0.2.0.tar.gz` & `tmp/spacetraders-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.2.0.tar", max compression
+gzip compressed data, was "spacetraders-0.2.1.tar", max compression
```

## Comparing `spacetraders-0.2.0.tar` & `spacetraders-0.2.1.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.2.0/README.md
--rw-r--r--   0        0        0      522 2023-05-11 13:12:39.996959 spacetraders-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-11 03:53:44.246922 spacetraders-0.2.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-11 03:53:43.766922 spacetraders-0.2.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     3870 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4346 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5189 2023-05-11 03:53:44.356922 spacetraders-0.2.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4365 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4356 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     5069 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.776922 spacetraders-0.2.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     9261 2023-05-11 03:53:44.356922 spacetraders-0.2.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4413 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     5038 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     5308 2023-05-11 03:53:44.336922 spacetraders-0.2.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4573 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4628 2023-05-11 03:53:44.336922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4674 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     6267 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     5414 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5569 2023-05-11 03:53:44.456922 spacetraders-0.2.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4287 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4394 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     5022 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     6447 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4347 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     5023 2023-05-11 03:53:44.416922 spacetraders-0.2.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5313 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     6961 2023-05-11 03:53:44.416922 spacetraders-0.2.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     5391 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5179 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5412 2023-05-11 03:53:44.426922 spacetraders-0.2.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4608 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4354 2023-05-11 03:53:44.446922 spacetraders-0.2.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5142 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5632 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5463 2023-05-11 03:53:44.496922 spacetraders-0.2.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     6353 2023-05-11 03:53:44.486922 spacetraders-0.2.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-11 03:53:43.806922 spacetraders-0.2.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4891 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5675 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4865 2023-05-11 03:53:44.486922 spacetraders-0.2.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4449 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     6004 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     5036 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4852 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4213 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-11 03:53:44.446922 spacetraders-0.2.0/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1170 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1200 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1351 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1376 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1563 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     1774 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1603 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1231 2023-05-11 03:53:44.496922 spacetraders-0.2.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1474 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-11 03:53:43.936922 spacetraders-0.2.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1629 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1152 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1370 2023-05-11 03:53:44.556922 spacetraders-0.2.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1326 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1217 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1344 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1229 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1362 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1299 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1175 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1176 2023-05-11 03:53:44.556922 spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1219 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1193 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1128 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1239 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1182 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1433 2023-05-11 03:53:44.586922 spacetraders-0.2.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1162 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1141 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1358 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1312 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     2091 2023-05-11 03:53:44.016922 spacetraders-0.2.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1176 2023-05-11 03:53:44.586922 spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1202 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1076 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1183 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1070 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1177 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1077 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1064 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1062 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1087 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1063 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1111 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1076 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1064 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1195 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1171 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1167 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1068 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1133 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1086 2023-05-11 03:53:44.636922 spacetraders-0.2.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1470 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1059 2023-05-11 03:53:44.636922 spacetraders-0.2.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1134 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1336 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2208 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1771 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-11 03:53:43.936922 spacetraders-0.2.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2047 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1097 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1067 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1345 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1132 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1270 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1115 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1253 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1385 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1102 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1224 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1348 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1146 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1298 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1310 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-11 03:53:43.996922 spacetraders-0.2.0/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1133 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1509 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     2269 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1035 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1032 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1040 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1038 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1383 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2141 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1369 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1086 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3041 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1385 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1401 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2114 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-11 03:53:43.906922 spacetraders-0.2.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1751 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2146 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-11 03:53:43.916922 spacetraders-0.2.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1455 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1278 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1784 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1763 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     1988 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1829 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1388 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1802 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1137 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-11 03:53:43.996922 spacetraders-0.2.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1217 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     1948 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1178 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1178 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1384 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1360 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-11 03:53:43.986922 spacetraders-0.2.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-11 03:53:43.916922 spacetraders-0.2.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     1838 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2371 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1088 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1636 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2166 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1100 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1626 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1003 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1243 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1190 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-11 03:53:43.986922 spacetraders-0.2.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1253 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1122 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1059 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1134 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1337 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2127 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1007 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1069 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1318 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-11 03:53:44.016922 spacetraders-0.2.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1035 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/types.py
--rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 spacetraders-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.2.1/README.md
+-rw-r--r--   0        0        0      522 2023-05-11 13:42:27.786961 spacetraders-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-11 13:36:56.146961 spacetraders-0.2.1/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 13:36:55.656961 spacetraders-0.2.1/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     3818 2023-05-11 13:36:56.196961 spacetraders-0.2.1/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4290 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5132 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4308 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4303 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     5015 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.666961 spacetraders-0.2.1/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     9211 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4361 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4985 2023-05-11 13:36:56.236961 spacetraders-0.2.1/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.716961 spacetraders-0.2.1/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5255 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4513 2023-05-11 13:36:56.226961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4566 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4610 2023-05-11 13:36:56.206961 spacetraders-0.2.1/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6213 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5356 2023-05-11 13:36:56.216961 spacetraders-0.2.1/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5511 2023-05-11 13:36:56.246961 spacetraders-0.2.1/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4236 2023-05-11 13:36:56.266961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4338 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4970 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     6390 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4295 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     4973 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5263 2023-05-11 13:36:56.276961 spacetraders-0.2.1/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     6907 2023-05-11 13:36:56.296961 spacetraders-0.2.1/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5331 2023-05-11 13:36:56.296961 spacetraders-0.2.1/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5125 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5344 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4554 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4302 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5082 2023-05-11 13:36:56.336961 spacetraders-0.2.1/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5570 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5395 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     6303 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-11 13:36:55.706961 spacetraders-0.2.1/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4838 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5624 2023-05-11 13:36:56.386961 spacetraders-0.2.1/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4812 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4398 2023-05-11 13:36:56.366961 spacetraders-0.2.1/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5944 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4984 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4799 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4213 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-11 13:36:56.316961 spacetraders-0.2.1/spacetraders/errors.py
+-rw-r--r--   0        0        0    13081 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1170 2023-05-11 13:36:56.336961 spacetraders-0.2.1/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1200 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1351 2023-05-11 13:36:56.356961 spacetraders-0.2.1/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1376 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1563 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     1774 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1603 2023-05-11 13:36:56.386961 spacetraders-0.2.1/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1231 2023-05-11 13:36:56.376961 spacetraders-0.2.1/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1474 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1629 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1152 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1370 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.396961 spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1326 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1217 2023-05-11 13:36:56.406961 spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1344 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1229 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1362 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.416961 spacetraders-0.2.1/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1299 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1175 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1176 2023-05-11 13:36:56.436961 spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1219 2023-05-11 13:36:56.446961 spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1193 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1128 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1239 2023-05-11 13:36:56.426961 spacetraders-0.2.1/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1182 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1433 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1162 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1141 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1358 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1312 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     2091 2023-05-11 13:36:55.916961 spacetraders-0.2.1/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1176 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1202 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1076 2023-05-11 13:36:56.456961 spacetraders-0.2.1/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1183 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1070 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1177 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1077 2023-05-11 13:36:56.466961 spacetraders-0.2.1/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1064 2023-05-11 13:36:56.476961 spacetraders-0.2.1/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1062 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1087 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1063 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1111 2023-05-11 13:36:56.486961 spacetraders-0.2.1/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1076 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     1064 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1195 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1171 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1167 2023-05-11 13:36:56.496961 spacetraders-0.2.1/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1068 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1133 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1086 2023-05-11 13:36:56.506961 spacetraders-0.2.1/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1470 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1059 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1134 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1336 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2208 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1771 2023-05-11 13:36:56.516961 spacetraders-0.2.1/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2047 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1097 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1067 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1345 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.526961 spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1132 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1270 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1115 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1385 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1102 2023-05-11 13:36:56.536961 spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1224 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1158 2023-05-11 13:36:56.546961 spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1348 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1146 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1298 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1310 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1133 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1509 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     2269 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1035 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1032 2023-05-11 13:36:56.556961 spacetraders-0.2.1/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1040 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1038 2023-05-11 13:36:56.566961 spacetraders-0.2.1/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1383 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2141 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1205 2023-05-11 13:36:56.576961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1369 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1086 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3041 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1385 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1401 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2114 2023-05-11 13:36:56.586961 spacetraders-0.2.1/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-11 13:36:55.816961 spacetraders-0.2.1/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1751 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2146 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1455 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1278 2023-05-11 13:36:56.596961 spacetraders-0.2.1/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1784 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1763 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-11 13:36:55.906961 spacetraders-0.2.1/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-11 13:36:55.906961 spacetraders-0.2.1/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     1988 2023-05-11 13:36:56.606961 spacetraders-0.2.1/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1829 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1388 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-11 13:36:55.846961 spacetraders-0.2.1/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1802 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-11 13:36:55.826961 spacetraders-0.2.1/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1137 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-11 13:36:55.896961 spacetraders-0.2.1/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1217 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     1948 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1178 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1178 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1384 2023-05-11 13:36:56.626961 spacetraders-0.2.1/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1360 2023-05-11 13:36:56.616961 spacetraders-0.2.1/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-11 13:36:55.886961 spacetraders-0.2.1/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-11 13:36:55.816961 spacetraders-0.2.1/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     1838 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2371 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1088 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1636 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2166 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1100 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1626 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1003 2023-05-11 13:36:56.636961 spacetraders-0.2.1/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1243 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1190 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-11 13:36:55.886961 spacetraders-0.2.1/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1253 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1122 2023-05-11 13:36:56.646961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1059 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1134 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1337 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2127 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1007 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1069 2023-05-11 13:36:56.656961 spacetraders-0.2.1/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1318 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-11 13:36:55.916961 spacetraders-0.2.1/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-11 13:36:55.836961 spacetraders-0.2.1/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1035 2023-05-11 13:36:56.666961 spacetraders-0.2.1/spacetraders/types.py
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 spacetraders-0.2.1/PKG-INFO
```

### Comparing `spacetraders-0.2.0/README.md` & `spacetraders-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/pyproject.toml` & `spacetraders-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.2.0"
+version = "0.2.1"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.2.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.2.1/spacetraders/api/agents/get_my_agent.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyAgentResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyAgentResponse200.update_forward_refs()
-        GetMyAgentResponse200(**response.json())
+        response_200 = GetMyAgentResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.2.1/spacetraders/api/contracts/accept_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[AcceptContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AcceptContractResponse200.update_forward_refs()
-        AcceptContractResponse200(**response.json())
+        response_200 = AcceptContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.2.1/spacetraders/api/contracts/deliver_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[DeliverContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DeliverContractResponse200.update_forward_refs()
-        DeliverContractResponse200(**response.json())
+        response_200 = DeliverContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.2.1/spacetraders/api/contracts/fulfill_contract.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[FulfillContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = FulfillContractResponse200.update_forward_refs()
-        FulfillContractResponse200(**response.json())
+        response_200 = FulfillContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.2.1/spacetraders/api/contracts/get_contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetContractResponse200.update_forward_refs()
-        GetContractResponse200(**response.json())
+        response_200 = GetContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.2.1/spacetraders/api/contracts/get_contracts.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetContractsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetContractsResponse200.update_forward_refs()
-        GetContractsResponse200(**response.json())
+        response_200 = GetContractsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/default/register.py` & `spacetraders-0.2.1/spacetraders/api/default/register.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[RegisterResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = RegisterResponse201.update_forward_refs()
-        RegisterResponse201(**response.json())
+        response_201 = RegisterResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.2.1/spacetraders/api/factions/get_faction.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetFactionResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetFactionResponse200.update_forward_refs()
-        GetFactionResponse200(**response.json())
+        response_200 = GetFactionResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.2.1/spacetraders/api/factions/get_factions.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetFactionsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetFactionsResponse200.update_forward_refs()
-        GetFactionsResponse200(**response.json())
+        response_200 = GetFactionsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.2.1/spacetraders/api/fleet/create_chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateChartResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateChartResponse201.update_forward_refs()
-        CreateChartResponse201(**response.json())
+        response_201 = CreateChartResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipShipScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipShipScanResponse201.update_forward_refs()
-        CreateShipShipScanResponse201(**response.json())
+        response_201 = CreateShipShipScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipSystemScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipSystemScanResponse201.update_forward_refs()
-        CreateShipSystemScanResponse201(**response.json())
+        response_201 = CreateShipSystemScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.2.1/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipWaypointScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipWaypointScanResponse201.update_forward_refs()
-        CreateShipWaypointScanResponse201(**response.json())
+        response_201 = CreateShipWaypointScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.2.1/spacetraders/api/fleet/create_survey.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateSurveyResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateSurveyResponse201.update_forward_refs()
-        CreateSurveyResponse201(**response.json())
+        response_201 = CreateSurveyResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/dock_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[DockShipDockShip200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DockShipDockShip200Response.update_forward_refs()
-        DockShipDockShip200Response(**response.json())
+        response_200 = DockShipDockShip200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.2.1/spacetraders/api/fleet/extract_resources.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ExtractResourcesResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = ExtractResourcesResponse201.update_forward_refs()
-        ExtractResourcesResponse201(**response.json())
+        response_201 = ExtractResourcesResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipResponse200.update_forward_refs()
-        GetMyShipResponse200(**response.json())
+        response_200 = GetMyShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipCargoResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipCargoResponse200.update_forward_refs()
-        GetMyShipCargoResponse200(**response.json())
+        response_200 = GetMyShipCargoResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.2.1/spacetraders/api/fleet/get_my_ships.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipsResponse200.update_forward_refs()
-        GetMyShipsResponse200(**response.json())
+        response_200 = GetMyShipsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.2.1/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[Union[Any, GetShipCooldownResponse200]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipCooldownResponse200.update_forward_refs()
-        GetShipCooldownResponse200(**response.json())
+        response_200 = GetShipCooldownResponse200(**response.json())
 
         return response_200
     if response.status_code == HTTPStatus.NO_CONTENT:
         response_204 = cast(Any, None)
         return response_204
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.2.1/spacetraders/api/fleet/get_ship_nav.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetShipNavResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipNavResponse200.update_forward_refs()
-        GetShipNavResponse200(**response.json())
+        response_200 = GetShipNavResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.2.1/spacetraders/api/fleet/jettison.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[JettisonResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = JettisonResponse200.update_forward_refs()
-        JettisonResponse200(**response.json())
+        response_200 = JettisonResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/jump_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[JumpShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = JumpShipResponse200.update_forward_refs()
-        JumpShipResponse200(**response.json())
+        response_200 = JumpShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/navigate_ship.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[NavigateShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = NavigateShipResponse200.update_forward_refs()
-        NavigateShipResponse200(**response.json())
+        response_200 = NavigateShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/orbit_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[OrbitShipOrbitShip200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = OrbitShipOrbitShip200Response.update_forward_refs()
-        OrbitShipOrbitShip200Response(**response.json())
+        response_200 = OrbitShipOrbitShip200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.2.1/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PatchShipNavResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PatchShipNavResponse200.update_forward_refs()
-        PatchShipNavResponse200(**response.json())
+        response_200 = PatchShipNavResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.2.1/spacetraders/api/fleet/purchase_cargo.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PurchaseCargoPurchaseCargo201Response]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = PurchaseCargoPurchaseCargo201Response.update_forward_refs()
-        PurchaseCargoPurchaseCargo201Response(**response.json())
+        response_201 = PurchaseCargoPurchaseCargo201Response(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/purchase_ship.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PurchaseShipResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = PurchaseShipResponse201.update_forward_refs()
-        PurchaseShipResponse201(**response.json())
+        response_201 = PurchaseShipResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/refuel_ship.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[RefuelShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = RefuelShipResponse200.update_forward_refs()
-        RefuelShipResponse200(**response.json())
+        response_200 = RefuelShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.2.1/spacetraders/api/fleet/sell_cargo.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[SellCargoSellCargo201Response]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = SellCargoSellCargo201Response.update_forward_refs()
-        SellCargoSellCargo201Response(**response.json())
+        response_201 = SellCargoSellCargo201Response(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.2.1/spacetraders/api/fleet/ship_refine.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ShipRefineShipRefine200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ShipRefineShipRefine200Response.update_forward_refs()
-        ShipRefineShipRefine200Response(**response.json())
+        response_200 = ShipRefineShipRefine200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.2.1/spacetraders/api/fleet/transfer_cargo.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[TransferCargoTransferCargo200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TransferCargoTransferCargo200Response.update_forward_refs()
-        TransferCargoTransferCargo200Response(**response.json())
+        response_200 = TransferCargoTransferCargo200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.2.1/spacetraders/api/fleet/warp_ship.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,16 +36,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[WarpShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = WarpShipResponse200.update_forward_refs()
-        WarpShipResponse200(**response.json())
+        response_200 = WarpShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_jump_gate.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetJumpGateResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetJumpGateResponse200.update_forward_refs()
-        GetJumpGateResponse200(**response.json())
+        response_200 = GetJumpGateResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_market.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMarketResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMarketResponse200.update_forward_refs()
-        GetMarketResponse200(**response.json())
+        response_200 = GetMarketResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_shipyard.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetShipyardResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipyardResponse200.update_forward_refs()
-        GetShipyardResponse200(**response.json())
+        response_200 = GetShipyardResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_system.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_system.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemResponse200.update_forward_refs()
-        GetSystemResponse200(**response.json())
+        response_200 = GetSystemResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_system_waypoints.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemWaypointsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemWaypointsResponse200.update_forward_refs()
-        GetSystemWaypointsResponse200(**response.json())
+        response_200 = GetSystemWaypointsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_systems.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_systems.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,16 +38,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemsResponse200.update_forward_refs()
-        GetSystemsResponse200(**response.json())
+        response_200 = GetSystemsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.2.1/spacetraders/api/systems/get_waypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,16 +32,15 @@
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetWaypointResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetWaypointResponse200.update_forward_refs()
-        GetWaypointResponse200(**response.json())
+        response_200 = GetWaypointResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
```

### Comparing `spacetraders-0.2.0/spacetraders/client.py` & `spacetraders-0.2.1/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/__init__.py` & `spacetraders-0.2.1/spacetraders/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.2.1/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/agent.py` & `spacetraders-0.2.1/spacetraders/models/agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/chart.py` & `spacetraders-0.2.1/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/connected_system.py` & `spacetraders-0.2.1/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/contract.py` & `spacetraders-0.2.1/spacetraders/models/contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.2.1/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/contract_payment.py` & `spacetraders-0.2.1/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/contract_terms.py` & `spacetraders-0.2.1/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/cooldown.py` & `spacetraders-0.2.1/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.2.1/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.2.1/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.2.1/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.2.1/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.2.1/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.2.1/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/extraction.py` & `spacetraders-0.2.1/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.2.1/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/faction.py` & `spacetraders-0.2.1/spacetraders/models/faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/faction_trait.py` & `spacetraders-0.2.1/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.2.1/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.2.1/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.2.1/spacetraders/models/jettison_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.2.1/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jump_gate.py` & `spacetraders-0.2.1/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.2.1/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.2.1/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/market.py` & `spacetraders-0.2.1/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.2.1/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/market_transaction.py` & `spacetraders-0.2.1/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/meta.py` & `spacetraders-0.2.1/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.2.1/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.2.1/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.2.1/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.2.1/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.2.1/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.2.1/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/register_json_body.py` & `spacetraders-0.2.1/spacetraders/models/register_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/register_response_201.py` & `spacetraders-0.2.1/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.2.1/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.2.1/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.2.1/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.2.1/spacetraders/models/scanned_ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.2.1/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.2.1/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_system.py` & `spacetraders-0.2.1/spacetraders/models/scanned_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.2.1/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.2.1/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship.py` & `spacetraders-0.2.1/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.2.1/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.2.1/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_crew.py` & `spacetraders-0.2.1/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_engine.py` & `spacetraders-0.2.1/spacetraders/models/ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_frame.py` & `spacetraders-0.2.1/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.2.1/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.2.1/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.2.1/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_module.py` & `spacetraders-0.2.1/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.2.1/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_mount.py` & `spacetraders-0.2.1/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.2.1/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.2.1/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_nav.py` & `spacetraders-0.2.1/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.2.1/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.2.1/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.2.1/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.2.1/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.2.1/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_registration.py` & `spacetraders-0.2.1/spacetraders/models/ship_registration.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.2.1/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/ship_type.py` & `spacetraders-0.2.1/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/shipyard.py` & `spacetraders-0.2.1/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/shipyard_ship.py` & `spacetraders-0.2.1/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.2.1/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.2.1/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/survey.py` & `spacetraders-0.2.1/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.2.1/spacetraders/models/survey_deposit.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/system.py` & `spacetraders-0.2.1/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/system_faction.py` & `spacetraders-0.2.1/spacetraders/models/system_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.2.1/spacetraders/models/system_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/trade_good.py` & `spacetraders-0.2.1/spacetraders/models/trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.2.1/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.2.1/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.2.1/spacetraders/models/warp_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.2.1/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.2.1/spacetraders/models/warp_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/waypoint.py` & `spacetraders-0.2.1/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.2.1/spacetraders/models/waypoint_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.2.1/spacetraders/models/waypoint_orbital.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/waypoint_trait.py` & `spacetraders-0.2.1/spacetraders/models/waypoint_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.2.1/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/spacetraders/types.py` & `spacetraders-0.2.1/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.2.0/PKG-INFO` & `spacetraders-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.2.0
+Version: 0.2.1
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

