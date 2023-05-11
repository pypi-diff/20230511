# Comparing `tmp/spacetraders-0.1.4.tar.gz` & `tmp/spacetraders-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.1.4.tar", max compression
+gzip compressed data, was "spacetraders-0.2.0.tar", max compression
```

## Comparing `spacetraders-0.1.4.tar` & `spacetraders-0.2.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.1.4/README.md
--rw-r--r--   0        0        0      501 2023-05-10 04:44:30.269683 spacetraders-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-10 04:44:08.369683 spacetraders-0.1.4/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-10 04:44:07.839682 spacetraders-0.1.4/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     3816 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4288 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5017 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4306 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4287 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     5013 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.849683 spacetraders-0.1.4/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     9110 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4359 2023-05-10 04:44:08.429683 spacetraders-0.1.4/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4983 2023-05-10 04:44:08.469683 spacetraders-0.1.4/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.879683 spacetraders-0.1.4/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     5253 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4511 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4564 2023-05-10 04:44:08.469683 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4608 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     6211 2023-05-10 04:44:08.449683 spacetraders-0.1.4/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     5354 2023-05-10 04:44:08.439683 spacetraders-0.1.4/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5394 2023-05-10 04:44:08.459683 spacetraders-0.1.4/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4234 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4336 2023-05-10 04:44:08.499683 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4968 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     6388 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4279 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4872 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5162 2023-05-10 04:44:08.509683 spacetraders-0.1.4/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     6798 2023-05-10 04:44:08.519683 spacetraders-0.1.4/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     5329 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5002 2023-05-10 04:44:08.529682 spacetraders-0.1.4/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5209 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4445 2023-05-10 04:44:08.539682 spacetraders-0.1.4/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4300 2023-05-10 04:44:08.539682 spacetraders-0.1.4/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     4963 2023-05-10 04:44:08.569682 spacetraders-0.1.4/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5465 2023-05-10 04:44:08.569682 spacetraders-0.1.4/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5260 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     6202 2023-05-10 04:44:08.599683 spacetraders-0.1.4/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-10 04:44:07.869683 spacetraders-0.1.4/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4836 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5622 2023-05-10 04:44:08.579682 spacetraders-0.1.4/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4810 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4396 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5942 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4982 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4797 2023-05-10 04:44:08.609683 spacetraders-0.1.4/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4212 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-10 04:44:08.549682 spacetraders-0.1.4/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     2021 2023-05-10 04:44:08.589682 spacetraders-0.1.4/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     2138 2023-05-10 04:44:08.629683 spacetraders-0.1.4/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     2216 2023-05-10 04:44:08.619683 spacetraders-0.1.4/spacetraders/models/agent.py
--rw-r--r--   0        0        0     2735 2023-05-10 04:44:08.639683 spacetraders-0.1.4/spacetraders/models/chart.py
--rw-r--r--   0        0        0     2817 2023-05-10 04:44:08.659683 spacetraders-0.1.4/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     3209 2023-05-10 04:44:08.669683 spacetraders-0.1.4/spacetraders/models/contract.py
--rw-r--r--   0        0        0     2675 2023-05-10 04:44:08.659683 spacetraders-0.1.4/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1922 2023-05-10 04:44:08.669683 spacetraders-0.1.4/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     3089 2023-05-10 04:44:08.679683 spacetraders-0.1.4/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-10 04:44:08.009683 spacetraders-0.1.4/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     2629 2023-05-10 04:44:08.679683 spacetraders-0.1.4/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1929 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     2299 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     2566 2023-05-10 04:44:08.699683 spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     2134 2023-05-10 04:44:08.689683 spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     2638 2023-05-10 04:44:08.689683 spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     2162 2023-05-10 04:44:08.699683 spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     2710 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     2526 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1989 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     2052 2023-05-10 04:44:08.709683 spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     2182 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     2078 2023-05-10 04:44:08.729683 spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1833 2023-05-10 04:44:08.719683 spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     2215 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     2066 2023-05-10 04:44:08.739683 spacetraders-0.1.4/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     2666 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1980 2023-05-10 04:44:08.749683 spacetraders-0.1.4/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1750 2023-05-10 04:44:08.759683 spacetraders-0.1.4/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     2746 2023-05-10 04:44:08.779682 spacetraders-0.1.4/spacetraders/models/faction.py
--rw-r--r--   0        0        0     2067 2023-05-10 04:44:08.779682 spacetraders-0.1.4/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     2091 2023-05-10 04:44:08.119683 spacetraders-0.1.4/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     2052 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     2143 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1755 2023-05-10 04:44:08.829682 spacetraders-0.1.4/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     2300 2023-05-10 04:44:08.799682 spacetraders-0.1.4/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1741 2023-05-10 04:44:08.769683 spacetraders-0.1.4/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     2286 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1761 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1727 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1726 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1788 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1719 2023-05-10 04:44:08.789682 spacetraders-0.1.4/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     2257 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1857 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1787 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1755 2023-05-10 04:44:08.799682 spacetraders-0.1.4/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1727 2023-05-10 04:44:08.809682 spacetraders-0.1.4/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     2333 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     2272 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1846 2023-05-10 04:44:08.819682 spacetraders-0.1.4/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1683 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1782 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     3023 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1632 2023-05-10 04:44:08.839682 spacetraders-0.1.4/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1887 2023-05-10 04:44:08.869683 spacetraders-0.1.4/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     2550 2023-05-10 04:44:08.869683 spacetraders-0.1.4/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     5804 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/market.py
--rw-r--r--   0        0        0     2843 2023-05-10 04:44:08.919683 spacetraders-0.1.4/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     3546 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1749 2023-05-10 04:44:08.859683 spacetraders-0.1.4/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1666 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     2249 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.909683 spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1843 2023-05-10 04:44:08.889683 spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     2200 2023-05-10 04:44:08.889683 spacetraders-0.1.4/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1797 2023-05-10 04:44:08.879683 spacetraders-0.1.4/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     2218 2023-05-10 04:44:08.899683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     2662 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1774 2023-05-10 04:44:08.909683 spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1960 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:44:08.919683 spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     2553 2023-05-10 04:44:08.939683 spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1915 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     2198 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1971 2023-05-10 04:44:08.929683 spacetraders-0.1.4/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-10 04:44:08.099683 spacetraders-0.1.4/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:44:08.949683 spacetraders-0.1.4/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     2946 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     5575 2023-05-10 04:44:09.029682 spacetraders-0.1.4/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1560 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1554 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1580 2023-05-10 04:44:08.949683 spacetraders-0.1.4/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1566 2023-05-10 04:44:08.959683 spacetraders-0.1.4/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     2390 2023-05-10 04:44:08.989683 spacetraders-0.1.4/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     5283 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     2106 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     2622 2023-05-10 04:44:08.979683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1734 2023-05-10 04:44:09.009683 spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     6470 2023-05-10 04:44:09.049682 spacetraders-0.1.4/spacetraders/models/ship.py
--rw-r--r--   0        0        0     2590 2023-05-10 04:44:08.999683 spacetraders-0.1.4/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     2228 2023-05-10 04:44:08.999683 spacetraders-0.1.4/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     3202 2023-05-10 04:44:09.019683 spacetraders-0.1.4/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-10 04:44:07.969683 spacetraders-0.1.4/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     3124 2023-05-10 04:44:09.009683 spacetraders-0.1.4/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     3873 2023-05-10 04:44:09.049682 spacetraders-0.1.4/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-10 04:44:07.989683 spacetraders-0.1.4/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     2729 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1943 2023-05-10 04:44:09.019683 spacetraders-0.1.4/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     3305 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-10 04:44:08.029682 spacetraders-0.1.4/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     3738 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-10 04:44:08.109683 spacetraders-0.1.4/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     3267 2023-05-10 04:44:09.039682 spacetraders-0.1.4/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     3062 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     2310 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-10 04:44:08.019683 spacetraders-0.1.4/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     3227 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1708 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-10 04:44:08.099683 spacetraders-0.1.4/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     2134 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     4564 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     2085 2023-05-10 04:44:09.059682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     2085 2023-05-10 04:44:09.069682 spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     2233 2023-05-10 04:44:09.079682 spacetraders-0.1.4/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     2221 2023-05-10 04:44:09.089682 spacetraders-0.1.4/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-10 04:44:08.089682 spacetraders-0.1.4/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-10 04:44:07.989683 spacetraders-0.1.4/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     4568 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     5320 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1890 2023-05-10 04:44:09.099683 spacetraders-0.1.4/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     2737 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     3608 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1610 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     3656 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/system.py
--rw-r--r--   0        0        0     1513 2023-05-10 04:44:09.109683 spacetraders-0.1.4/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1993 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1929 2023-05-10 04:44:09.129683 spacetraders-0.1.4/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-10 04:44:08.089682 spacetraders-0.1.4/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     2218 2023-05-10 04:44:09.119683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1881 2023-05-10 04:44:09.139683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     2042 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1646 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1887 2023-05-10 04:44:09.149683 spacetraders-0.1.4/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     2229 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     5245 2023-05-10 04:44:09.199683 spacetraders-0.1.4/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1523 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1585 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     2077 2023-05-10 04:44:09.169683 spacetraders-0.1.4/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-10 04:44:08.119683 spacetraders-0.1.4/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-10 04:44:07.999683 spacetraders-0.1.4/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1035 2023-05-10 04:44:09.159683 spacetraders-0.1.4/spacetraders/types.py
--rw-r--r--   0        0        0     3909 1970-01-01 00:00:00.000000 spacetraders-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.2.0/README.md
+-rw-r--r--   0        0        0      522 2023-05-11 13:12:39.996959 spacetraders-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-11 03:53:44.246922 spacetraders-0.2.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-11 03:53:43.766922 spacetraders-0.2.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     3870 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4346 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5189 2023-05-11 03:53:44.356922 spacetraders-0.2.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4365 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4356 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     5069 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.776922 spacetraders-0.2.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     9261 2023-05-11 03:53:44.356922 spacetraders-0.2.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4413 2023-05-11 03:53:44.316922 spacetraders-0.2.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     5038 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.816922 spacetraders-0.2.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     5308 2023-05-11 03:53:44.336922 spacetraders-0.2.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4573 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4628 2023-05-11 03:53:44.336922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4674 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     6267 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     5414 2023-05-11 03:53:44.326922 spacetraders-0.2.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5569 2023-05-11 03:53:44.456922 spacetraders-0.2.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4287 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4394 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     5022 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     6447 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4347 2023-05-11 03:53:44.386922 spacetraders-0.2.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     5023 2023-05-11 03:53:44.416922 spacetraders-0.2.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5313 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     6961 2023-05-11 03:53:44.416922 spacetraders-0.2.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     5391 2023-05-11 03:53:44.406922 spacetraders-0.2.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5179 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5412 2023-05-11 03:53:44.426922 spacetraders-0.2.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4608 2023-05-11 03:53:44.436922 spacetraders-0.2.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4354 2023-05-11 03:53:44.446922 spacetraders-0.2.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5142 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5632 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5463 2023-05-11 03:53:44.496922 spacetraders-0.2.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     6353 2023-05-11 03:53:44.486922 spacetraders-0.2.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-11 03:53:43.806922 spacetraders-0.2.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4891 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5675 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4865 2023-05-11 03:53:44.486922 spacetraders-0.2.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4449 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     6004 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     5036 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4852 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4213 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-11 03:53:44.446922 spacetraders-0.2.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    13081 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1170 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1200 2023-05-11 03:53:44.476922 spacetraders-0.2.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1351 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1376 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1563 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     1774 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1603 2023-05-11 03:53:44.506922 spacetraders-0.2.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1231 2023-05-11 03:53:44.496922 spacetraders-0.2.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1474 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-11 03:53:43.936922 spacetraders-0.2.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1629 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1152 2023-05-11 03:53:44.516922 spacetraders-0.2.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1370 2023-05-11 03:53:44.556922 spacetraders-0.2.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1326 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1217 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1344 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1229 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1362 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.536922 spacetraders-0.2.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1299 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1175 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1176 2023-05-11 03:53:44.556922 spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1219 2023-05-11 03:53:44.546922 spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1193 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1128 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1239 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1182 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1433 2023-05-11 03:53:44.586922 spacetraders-0.2.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1162 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1141 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1358 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1312 2023-05-11 03:53:44.576922 spacetraders-0.2.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     2091 2023-05-11 03:53:44.016922 spacetraders-0.2.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1176 2023-05-11 03:53:44.586922 spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1202 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1076 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1183 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1070 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1177 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1077 2023-05-11 03:53:44.596922 spacetraders-0.2.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1064 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1062 2023-05-11 03:53:44.606922 spacetraders-0.2.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1087 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1063 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1111 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1076 2023-05-11 03:53:44.616922 spacetraders-0.2.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     1064 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1195 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1171 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1167 2023-05-11 03:53:44.626922 spacetraders-0.2.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1068 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1133 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1086 2023-05-11 03:53:44.636922 spacetraders-0.2.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1470 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1059 2023-05-11 03:53:44.636922 spacetraders-0.2.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1134 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1336 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2208 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1771 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-11 03:53:43.936922 spacetraders-0.2.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2047 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1097 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1067 2023-05-11 03:53:44.646922 spacetraders-0.2.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1345 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.656922 spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1132 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1270 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1115 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1253 2023-05-11 03:53:44.666922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1385 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1102 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1224 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1158 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1348 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1146 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1298 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1310 2023-05-11 03:53:44.676922 spacetraders-0.2.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-11 03:53:43.996922 spacetraders-0.2.0/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1133 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1509 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     2269 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1035 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1032 2023-05-11 03:53:44.686922 spacetraders-0.2.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1040 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1038 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1383 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2141 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1205 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1369 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1086 2023-05-11 03:53:44.696922 spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3041 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1385 2023-05-11 03:53:44.706922 spacetraders-0.2.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1401 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2114 2023-05-11 03:53:44.716922 spacetraders-0.2.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-11 03:53:43.906922 spacetraders-0.2.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1751 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2146 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-11 03:53:43.916922 spacetraders-0.2.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1455 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1278 2023-05-11 03:53:44.726922 spacetraders-0.2.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1784 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1763 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-11 03:53:44.006922 spacetraders-0.2.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     1988 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1829 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1388 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-11 03:53:43.946922 spacetraders-0.2.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1802 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1137 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-11 03:53:43.996922 spacetraders-0.2.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1217 2023-05-11 03:53:44.736922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     1948 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1178 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1178 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1384 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1360 2023-05-11 03:53:44.746922 spacetraders-0.2.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-11 03:53:43.986922 spacetraders-0.2.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-11 03:53:43.916922 spacetraders-0.2.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     1838 2023-05-11 03:53:44.756922 spacetraders-0.2.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2371 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1088 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1636 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2166 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1100 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1626 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1003 2023-05-11 03:53:44.766922 spacetraders-0.2.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1243 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1190 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-11 03:53:43.986922 spacetraders-0.2.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1253 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1122 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1059 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1134 2023-05-11 03:53:44.776922 spacetraders-0.2.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1337 2023-05-11 03:53:44.786922 spacetraders-0.2.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2127 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1007 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1069 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1318 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-11 03:53:44.016922 spacetraders-0.2.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-11 03:53:43.926922 spacetraders-0.2.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1035 2023-05-11 03:53:44.796922 spacetraders-0.2.0/spacetraders/types.py
+-rw-r--r--   0        0        0     3951 1970-01-01 00:00:00.000000 spacetraders-0.2.0/PKG-INFO
```

### Comparing `spacetraders-0.1.4/README.md` & `spacetraders-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.2.0/spacetraders/api/agents/get_my_agent.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,36 +7,37 @@
 from ...client import AuthenticatedClient, Client
 from ...models.get_my_agent_response_200 import GetMyAgentResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/agent".format(client.base_url)
+    url = "{}/my/agent".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyAgentResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyAgentResponse200.from_dict(response.json())
+        response_200 = GetMyAgentResponse200.update_forward_refs()
+        GetMyAgentResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -50,90 +51,90 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyAgentResponse200]:
     """My Agent Details
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyAgentResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyAgentResponse200]:
     """My Agent Details
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetMyAgentResponse200
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyAgentResponse200]:
     """My Agent Details
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyAgentResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyAgentResponse200]:
     """My Agent Details
 
      Fetch your agent's details.
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -141,10 +142,10 @@
 
     Returns:
         GetMyAgentResponse200
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.2.0/spacetraders/api/contracts/accept_contract.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.accept_contract_response_200 import AcceptContractResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/contracts/{contractId}/accept".format(
-        client.base_url, contractId=contract_id
+        _client.base_url, contractId=contract_id
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[AcceptContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AcceptContractResponse200.from_dict(response.json())
+        response_200 = AcceptContractResponse200.update_forward_refs()
+        AcceptContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[AcceptContractResponse200]:
     """Accept Contract
 
      Accept a contract.
 
     Args:
         contract_id (str):
@@ -73,29 +74,29 @@
 
     Returns:
         Response[AcceptContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[AcceptContractResponse200]:
     """Accept Contract
 
      Accept a contract.
 
     Args:
         contract_id (str):
@@ -106,22 +107,22 @@
 
     Returns:
         AcceptContractResponse200
     """
 
     return sync_detailed(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[AcceptContractResponse200]:
     """Accept Contract
 
      Accept a contract.
 
     Args:
         contract_id (str):
@@ -132,27 +133,27 @@
 
     Returns:
         Response[AcceptContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[AcceptContractResponse200]:
     """Accept Contract
 
      Accept a contract.
 
     Args:
         contract_id (str):
@@ -164,10 +165,10 @@
     Returns:
         AcceptContractResponse200
     """
 
     return (
         await asyncio_detailed(
             contract_id=contract_id,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.2.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.deliver_contract_response_200 import DeliverContractResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: DeliverContractJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/contracts/{contractId}/deliver".format(
-        client.base_url, contractId=contract_id
+        _client.base_url, contractId=contract_id
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[DeliverContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DeliverContractResponse200.from_dict(response.json())
+        response_200 = DeliverContractResponse200.update_forward_refs()
+        DeliverContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
-    json_body: DeliverContractJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: DeliverContractJsonBody,
 ) -> Response[DeliverContractResponse200]:
     """Deliver Contract
 
      Deliver cargo on a given contract.
 
     Args:
         contract_id (str):
@@ -78,33 +79,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DeliverContractResponse200]
     """
 
+    json_body = DeliverContractJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
-    json_body: DeliverContractJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: DeliverContractJsonBody,
 ) -> Optional[DeliverContractResponse200]:
     """Deliver Contract
 
      Deliver cargo on a given contract.
 
     Args:
         contract_id (str):
@@ -116,24 +119,24 @@
 
     Returns:
         DeliverContractResponse200
     """
 
     return sync_detailed(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
-    json_body: DeliverContractJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: DeliverContractJsonBody,
 ) -> Response[DeliverContractResponse200]:
     """Deliver Contract
 
      Deliver cargo on a given contract.
 
     Args:
         contract_id (str):
@@ -143,31 +146,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[DeliverContractResponse200]
     """
 
+    json_body = DeliverContractJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
-    json_body: DeliverContractJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: DeliverContractJsonBody,
 ) -> Optional[DeliverContractResponse200]:
     """Deliver Contract
 
      Deliver cargo on a given contract.
 
     Args:
         contract_id (str):
@@ -180,11 +185,11 @@
     Returns:
         DeliverContractResponse200
     """
 
     return (
         await asyncio_detailed(
             contract_id=contract_id,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.2.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.fulfill_contract_response_200 import FulfillContractResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/contracts/{contractId}/fulfill".format(
-        client.base_url, contractId=contract_id
+        _client.base_url, contractId=contract_id
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[FulfillContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = FulfillContractResponse200.from_dict(response.json())
+        response_200 = FulfillContractResponse200.update_forward_refs()
+        FulfillContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[FulfillContractResponse200]:
     """Fulfill Contract
 
      Fulfill a contract
 
     Args:
         contract_id (str):
@@ -73,29 +74,29 @@
 
     Returns:
         Response[FulfillContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[FulfillContractResponse200]:
     """Fulfill Contract
 
      Fulfill a contract
 
     Args:
         contract_id (str):
@@ -106,22 +107,22 @@
 
     Returns:
         FulfillContractResponse200
     """
 
     return sync_detailed(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[FulfillContractResponse200]:
     """Fulfill Contract
 
      Fulfill a contract
 
     Args:
         contract_id (str):
@@ -132,27 +133,27 @@
 
     Returns:
         Response[FulfillContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[FulfillContractResponse200]:
     """Fulfill Contract
 
      Fulfill a contract
 
     Args:
         contract_id (str):
@@ -164,10 +165,10 @@
     Returns:
         FulfillContractResponse200
     """
 
     return (
         await asyncio_detailed(
             contract_id=contract_id,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.2.0/spacetraders/api/contracts/get_contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 from ...models.get_contract_response_200 import GetContractResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/contracts/{contractId}".format(client.base_url, contractId=contract_id)
+    url = "{}/my/contracts/{contractId}".format(
+        _client.base_url, contractId=contract_id
+    )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetContractResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetContractResponse200.from_dict(response.json())
+        response_200 = GetContractResponse200.update_forward_refs()
+        GetContractResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -52,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetContractResponse200]:
     """Get Contract
 
      Get the details of a contract by ID.
 
     Args:
         contract_id (str):
@@ -71,29 +74,29 @@
 
     Returns:
         Response[GetContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetContractResponse200]:
     """Get Contract
 
      Get the details of a contract by ID.
 
     Args:
         contract_id (str):
@@ -104,22 +107,22 @@
 
     Returns:
         GetContractResponse200
     """
 
     return sync_detailed(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetContractResponse200]:
     """Get Contract
 
      Get the details of a contract by ID.
 
     Args:
         contract_id (str):
@@ -130,27 +133,27 @@
 
     Returns:
         Response[GetContractResponse200]
     """
 
     kwargs = _get_kwargs(
         contract_id=contract_id,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     contract_id: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetContractResponse200]:
     """Get Contract
 
      Get the details of a contract by ID.
 
     Args:
         contract_id (str):
@@ -162,10 +165,10 @@
     Returns:
         GetContractResponse200
     """
 
     return (
         await asyncio_detailed(
             contract_id=contract_id,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.2.0/spacetraders/api/contracts/get_contracts.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,46 +7,47 @@
 from ...client import AuthenticatedClient, Client
 from ...models.get_contracts_response_200 import GetContractsResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/my/contracts".format(client.base_url)
+    url = "{}/my/contracts".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
     params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetContractsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetContractsResponse200.from_dict(response.json())
+        response_200 = GetContractsResponse200.update_forward_refs()
+        GetContractsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -60,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetContractsResponse200]:
     """List Contracts
 
      List all of your contracts.
 
@@ -81,30 +82,30 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetContractsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetContractsResponse200]:
     """List Contracts
 
      List all of your contracts.
 
@@ -117,23 +118,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetContractsResponse200
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetContractsResponse200]:
     """List Contracts
 
      List all of your contracts.
 
@@ -146,28 +147,28 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetContractsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetContractsResponse200]:
     """List Contracts
 
      List all of your contracts.
 
@@ -181,12 +182,12 @@
 
     Returns:
         GetContractsResponse200
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             page=page,
             limit=limit,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/default/register.py` & `spacetraders-0.2.0/spacetraders/api/default/register.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 from ...models.register_json_body import RegisterJsonBody
 from ...models.register_response_201 import RegisterResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
-    client: Client,
+    _client: Client,
     json_body: RegisterJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/register".format(client.base_url)
+    url = "{}/register".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[RegisterResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = RegisterResponse201.from_dict(response.json())
+        response_201 = RegisterResponse201.update_forward_refs()
+        RegisterResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -55,16 +56,16 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Client,
-    json_body: RegisterJsonBody,
+    _client: Client,
+    **json_body: RegisterJsonBody,
 ) -> Response[RegisterResponse201]:
     """Register New Agent
 
      Creates a new agent and ties it to a temporary Account.
 
     The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
     the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
@@ -95,31 +96,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RegisterResponse201]
     """
 
+    json_body = RegisterJsonBody(**json_body)
+
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: Client,
-    json_body: RegisterJsonBody,
+    _client: Client,
+    **json_body: RegisterJsonBody,
 ) -> Optional[RegisterResponse201]:
     """Register New Agent
 
      Creates a new agent and ties it to a temporary Account.
 
     The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
     the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
@@ -151,23 +154,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         RegisterResponse201
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Client,
-    json_body: RegisterJsonBody,
+    _client: Client,
+    **json_body: RegisterJsonBody,
 ) -> Response[RegisterResponse201]:
     """Register New Agent
 
      Creates a new agent and ties it to a temporary Account.
 
     The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
     the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
@@ -198,29 +201,31 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[RegisterResponse201]
     """
 
+    json_body = RegisterJsonBody(**json_body)
+
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: Client,
-    json_body: RegisterJsonBody,
+    _client: Client,
+    **json_body: RegisterJsonBody,
 ) -> Optional[RegisterResponse201]:
     """Register New Agent
 
      Creates a new agent and ties it to a temporary Account.
 
     The agent symbol is a 3-14 character string that will represent your agent. This symbol will prefix
     the symbol of every ship you own. Agent symbols will be cast to all uppercase characters.
@@ -253,11 +258,11 @@
 
     Returns:
         RegisterResponse201
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/factions/get_faction.py` & `spacetraders-0.2.0/spacetraders/api/factions/get_faction.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.get_faction_response_200 import GetFactionResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     faction_symbol: str = "CGR",
     *,
-    client: Client,
+    _client: Client,
 ) -> Dict[str, Any]:
     url = "{}/factions/{factionSymbol}".format(
-        client.base_url, factionSymbol=faction_symbol
+        _client.base_url, factionSymbol=faction_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetFactionResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetFactionResponse200.from_dict(response.json())
+        response_200 = GetFactionResponse200.update_forward_refs()
+        GetFactionResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     faction_symbol: str = "CGR",
     *,
-    client: Client,
+    _client: Client,
 ) -> Response[GetFactionResponse200]:
     """Get Faction
 
      View the details of a faction.
 
     Args:
         faction_symbol (str):  Default: 'CGR'.
@@ -73,29 +74,29 @@
 
     Returns:
         Response[GetFactionResponse200]
     """
 
     kwargs = _get_kwargs(
         faction_symbol=faction_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     faction_symbol: str = "CGR",
     *,
-    client: Client,
+    _client: Client,
 ) -> Optional[GetFactionResponse200]:
     """Get Faction
 
      View the details of a faction.
 
     Args:
         faction_symbol (str):  Default: 'CGR'.
@@ -106,22 +107,22 @@
 
     Returns:
         GetFactionResponse200
     """
 
     return sync_detailed(
         faction_symbol=faction_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     faction_symbol: str = "CGR",
     *,
-    client: Client,
+    _client: Client,
 ) -> Response[GetFactionResponse200]:
     """Get Faction
 
      View the details of a faction.
 
     Args:
         faction_symbol (str):  Default: 'CGR'.
@@ -132,27 +133,27 @@
 
     Returns:
         Response[GetFactionResponse200]
     """
 
     kwargs = _get_kwargs(
         faction_symbol=faction_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     faction_symbol: str = "CGR",
     *,
-    client: Client,
+    _client: Client,
 ) -> Optional[GetFactionResponse200]:
     """Get Faction
 
      View the details of a faction.
 
     Args:
         faction_symbol (str):  Default: 'CGR'.
@@ -164,10 +165,10 @@
     Returns:
         GetFactionResponse200
     """
 
     return (
         await asyncio_detailed(
             faction_symbol=faction_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/factions/get_factions.py` & `spacetraders-0.2.0/spacetraders/api/factions/get_factions.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,46 +7,47 @@
 from ...client import AuthenticatedClient, Client
 from ...models.get_factions_response_200 import GetFactionsResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: Client,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/factions".format(client.base_url)
+    url = "{}/factions".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
     params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetFactionsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetFactionsResponse200.from_dict(response.json())
+        response_200 = GetFactionsResponse200.update_forward_refs()
+        GetFactionsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -60,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: Client,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetFactionsResponse200]:
     """List Factions
 
      List all discovered factions in the game.
 
@@ -81,30 +82,30 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetFactionsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: Client,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetFactionsResponse200]:
     """List Factions
 
      List all discovered factions in the game.
 
@@ -117,23 +118,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetFactionsResponse200
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: Client,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetFactionsResponse200]:
     """List Factions
 
      List all discovered factions in the game.
 
@@ -146,28 +147,28 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetFactionsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: Client,
+    _client: Client,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetFactionsResponse200]:
     """List Factions
 
      List all discovered factions in the game.
 
@@ -181,12 +182,12 @@
 
     Returns:
         GetFactionsResponse200
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             page=page,
             limit=limit,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.2.0/spacetraders/api/fleet/create_chart.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.create_chart_response_201 import CreateChartResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/chart".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateChartResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateChartResponse201.from_dict(response.json())
+        response_201 = CreateChartResponse201.update_forward_refs()
+        CreateChartResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateChartResponse201]:
     """Create Chart
 
      Command a ship to chart the current waypoint.
 
     Waypoints in the universe are uncharted by default. These locations will not show up in the API
     until they have been charted by a ship.
@@ -78,29 +79,29 @@
 
     Returns:
         Response[CreateChartResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateChartResponse201]:
     """Create Chart
 
      Command a ship to chart the current waypoint.
 
     Waypoints in the universe are uncharted by default. These locations will not show up in the API
     until they have been charted by a ship.
@@ -116,22 +117,22 @@
 
     Returns:
         CreateChartResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateChartResponse201]:
     """Create Chart
 
      Command a ship to chart the current waypoint.
 
     Waypoints in the universe are uncharted by default. These locations will not show up in the API
     until they have been charted by a ship.
@@ -147,27 +148,27 @@
 
     Returns:
         Response[CreateChartResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateChartResponse201]:
     """Create Chart
 
      Command a ship to chart the current waypoint.
 
     Waypoints in the universe are uncharted by default. These locations will not show up in the API
     until they have been charted by a ship.
@@ -184,10 +185,10 @@
     Returns:
         CreateChartResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.create_ship_ship_scan_response_201 import CreateShipShipScanResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/scan/ships".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipShipScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipShipScanResponse201.from_dict(response.json())
+        response_201 = CreateShipShipScanResponse201.update_forward_refs()
+        CreateShipShipScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipShipScanResponse201]:
     """Scan Ships
 
      Activate your ship's sensor arrays to scan for ship information.
 
     Args:
         ship_symbol (str):
@@ -73,29 +74,29 @@
 
     Returns:
         Response[CreateShipShipScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipShipScanResponse201]:
     """Scan Ships
 
      Activate your ship's sensor arrays to scan for ship information.
 
     Args:
         ship_symbol (str):
@@ -106,22 +107,22 @@
 
     Returns:
         CreateShipShipScanResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipShipScanResponse201]:
     """Scan Ships
 
      Activate your ship's sensor arrays to scan for ship information.
 
     Args:
         ship_symbol (str):
@@ -132,27 +133,27 @@
 
     Returns:
         Response[CreateShipShipScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipShipScanResponse201]:
     """Scan Ships
 
      Activate your ship's sensor arrays to scan for ship information.
 
     Args:
         ship_symbol (str):
@@ -164,10 +165,10 @@
     Returns:
         CreateShipShipScanResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 )
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/scan/systems".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipSystemScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipSystemScanResponse201.from_dict(response.json())
+        response_201 = CreateShipSystemScanResponse201.update_forward_refs()
+        CreateShipSystemScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -56,15 +57,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipSystemScanResponse201]:
     """Scan Systems
 
      Activate your ship's sensor arrays to scan for system information.
 
     Args:
         ship_symbol (str):
@@ -75,29 +76,29 @@
 
     Returns:
         Response[CreateShipSystemScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipSystemScanResponse201]:
     """Scan Systems
 
      Activate your ship's sensor arrays to scan for system information.
 
     Args:
         ship_symbol (str):
@@ -108,22 +109,22 @@
 
     Returns:
         CreateShipSystemScanResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipSystemScanResponse201]:
     """Scan Systems
 
      Activate your ship's sensor arrays to scan for system information.
 
     Args:
         ship_symbol (str):
@@ -134,27 +135,27 @@
 
     Returns:
         Response[CreateShipSystemScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipSystemScanResponse201]:
     """Scan Systems
 
      Activate your ship's sensor arrays to scan for system information.
 
     Args:
         ship_symbol (str):
@@ -166,10 +167,10 @@
     Returns:
         CreateShipSystemScanResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.2.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,38 +10,39 @@
 )
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/scan/waypoints".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateShipWaypointScanResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateShipWaypointScanResponse201.from_dict(response.json())
+        response_201 = CreateShipWaypointScanResponse201.update_forward_refs()
+        CreateShipWaypointScanResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -56,15 +57,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipWaypointScanResponse201]:
     """Scan Waypoints
 
      Activate your ship's sensor arrays to scan for waypoint information.
 
     Args:
         ship_symbol (str):
@@ -75,29 +76,29 @@
 
     Returns:
         Response[CreateShipWaypointScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipWaypointScanResponse201]:
     """Scan Waypoints
 
      Activate your ship's sensor arrays to scan for waypoint information.
 
     Args:
         ship_symbol (str):
@@ -108,22 +109,22 @@
 
     Returns:
         CreateShipWaypointScanResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateShipWaypointScanResponse201]:
     """Scan Waypoints
 
      Activate your ship's sensor arrays to scan for waypoint information.
 
     Args:
         ship_symbol (str):
@@ -134,27 +135,27 @@
 
     Returns:
         Response[CreateShipWaypointScanResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateShipWaypointScanResponse201]:
     """Scan Waypoints
 
      Activate your ship's sensor arrays to scan for waypoint information.
 
     Args:
         ship_symbol (str):
@@ -166,10 +167,10 @@
     Returns:
         CreateShipWaypointScanResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.2.0/spacetraders/api/fleet/create_survey.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.create_survey_response_201 import CreateSurveyResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/survey".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[CreateSurveyResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = CreateSurveyResponse201.from_dict(response.json())
+        response_201 = CreateSurveyResponse201.update_forward_refs()
+        CreateSurveyResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateSurveyResponse201]:
     """Create Survey
 
      If you want to target specific yields for an extraction, you can survey a waypoint, such as an
     asteroid field, and send the survey in the body of the extract request. Each survey may have
     multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
     extracting that resource.
@@ -79,29 +80,29 @@
 
     Returns:
         Response[CreateSurveyResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateSurveyResponse201]:
     """Create Survey
 
      If you want to target specific yields for an extraction, you can survey a waypoint, such as an
     asteroid field, and send the survey in the body of the extract request. Each survey may have
     multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
     extracting that resource.
@@ -118,22 +119,22 @@
 
     Returns:
         CreateSurveyResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[CreateSurveyResponse201]:
     """Create Survey
 
      If you want to target specific yields for an extraction, you can survey a waypoint, such as an
     asteroid field, and send the survey in the body of the extract request. Each survey may have
     multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
     extracting that resource.
@@ -150,27 +151,27 @@
 
     Returns:
         Response[CreateSurveyResponse201]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[CreateSurveyResponse201]:
     """Create Survey
 
      If you want to target specific yields for an extraction, you can survey a waypoint, such as an
     asteroid field, and send the survey in the body of the extract request. Each survey may have
     multiple deposits, and if a symbol shows up more than once, that indicates a higher chance of
     extracting that resource.
@@ -188,10 +189,10 @@
     Returns:
         CreateSurveyResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/dock_ship.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.dock_ship_dock_ship_200_response import DockShipDockShip200Response
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/dock".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[DockShipDockShip200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DockShipDockShip200Response.from_dict(response.json())
+        response_200 = DockShipDockShip200Response.update_forward_refs()
+        DockShipDockShip200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[DockShipDockShip200Response]:
     """Dock Ship
 
      Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
     dockable location, and your ship is capable of docking at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
@@ -76,29 +77,29 @@
 
     Returns:
         Response[DockShipDockShip200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[DockShipDockShip200Response]:
     """Dock Ship
 
      Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
     dockable location, and your ship is capable of docking at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
@@ -112,22 +113,22 @@
 
     Returns:
         DockShipDockShip200Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[DockShipDockShip200Response]:
     """Dock Ship
 
      Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
     dockable location, and your ship is capable of docking at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
@@ -141,27 +142,27 @@
 
     Returns:
         Response[DockShipDockShip200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[DockShipDockShip200Response]:
     """Dock Ship
 
      Attempt to dock your ship at it's current location. Docking will only succeed if the waypoint is a
     dockable location, and your ship is capable of docking at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already docked.
@@ -176,10 +177,10 @@
     Returns:
         DockShipDockShip200Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.2.0/spacetraders/api/fleet/extract_resources.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.extract_resources_response_201 import ExtractResourcesResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: ExtractResourcesJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/extract".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ExtractResourcesResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = ExtractResourcesResponse201.from_dict(response.json())
+        response_201 = ExtractResourcesResponse201.update_forward_refs()
+        ExtractResourcesResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ExtractResourcesJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ExtractResourcesJsonBody,
 ) -> Response[ExtractResourcesResponse201]:
     """Extract Resources
 
      Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
     specific yields.
 
     Args:
@@ -79,33 +80,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ExtractResourcesResponse201]
     """
 
+    json_body = ExtractResourcesJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ExtractResourcesJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ExtractResourcesJsonBody,
 ) -> Optional[ExtractResourcesResponse201]:
     """Extract Resources
 
      Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
     specific yields.
 
     Args:
@@ -118,24 +121,24 @@
 
     Returns:
         ExtractResourcesResponse201
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ExtractResourcesJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ExtractResourcesJsonBody,
 ) -> Response[ExtractResourcesResponse201]:
     """Extract Resources
 
      Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
     specific yields.
 
     Args:
@@ -146,31 +149,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ExtractResourcesResponse201]
     """
 
+    json_body = ExtractResourcesJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ExtractResourcesJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ExtractResourcesJsonBody,
 ) -> Optional[ExtractResourcesResponse201]:
     """Extract Resources
 
      Extract resources from the waypoint into your ship. Send an optional survey as the payload to target
     specific yields.
 
     Args:
@@ -184,11 +189,11 @@
     Returns:
         ExtractResourcesResponse201
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,36 +8,37 @@
 from ...models.get_my_ship_response_200 import GetMyShipResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}".format(client.base_url, shipSymbol=ship_symbol)
+    url = "{}/my/ships/{shipSymbol}".format(_client.base_url, shipSymbol=ship_symbol)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipResponse200.from_dict(response.json())
+        response_200 = GetMyShipResponse200.update_forward_refs()
+        GetMyShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -52,15 +53,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyShipResponse200]:
     """Get Ship
 
      Retrieve the details of your ship.
 
     Args:
         ship_symbol (str):
@@ -71,29 +72,29 @@
 
     Returns:
         Response[GetMyShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyShipResponse200]:
     """Get Ship
 
      Retrieve the details of your ship.
 
     Args:
         ship_symbol (str):
@@ -104,22 +105,22 @@
 
     Returns:
         GetMyShipResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyShipResponse200]:
     """Get Ship
 
      Retrieve the details of your ship.
 
     Args:
         ship_symbol (str):
@@ -130,27 +131,27 @@
 
     Returns:
         Response[GetMyShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyShipResponse200]:
     """Get Ship
 
      Retrieve the details of your ship.
 
     Args:
         ship_symbol (str):
@@ -162,10 +163,10 @@
     Returns:
         GetMyShipResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.get_my_ship_cargo_response_200 import GetMyShipCargoResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/cargo".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipCargoResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipCargoResponse200.from_dict(response.json())
+        response_200 = GetMyShipCargoResponse200.update_forward_refs()
+        GetMyShipCargoResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyShipCargoResponse200]:
     """Get Ship Cargo
 
      Retrieve the cargo of your ship.
 
     Args:
         ship_symbol (str):
@@ -73,29 +74,29 @@
 
     Returns:
         Response[GetMyShipCargoResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyShipCargoResponse200]:
     """Get Ship Cargo
 
      Retrieve the cargo of your ship.
 
     Args:
         ship_symbol (str):
@@ -106,22 +107,22 @@
 
     Returns:
         GetMyShipCargoResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMyShipCargoResponse200]:
     """Get Ship Cargo
 
      Retrieve the cargo of your ship.
 
     Args:
         ship_symbol (str):
@@ -132,27 +133,27 @@
 
     Returns:
         Response[GetMyShipCargoResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMyShipCargoResponse200]:
     """Get Ship Cargo
 
      Retrieve the cargo of your ship.
 
     Args:
         ship_symbol (str):
@@ -164,10 +165,10 @@
     Returns:
         GetMyShipCargoResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.2.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,46 +7,47 @@
 from ...client import AuthenticatedClient, Client
 from ...models.get_my_ships_response_200 import GetMyShipsResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships".format(client.base_url)
+    url = "{}/my/ships".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
     params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMyShipsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMyShipsResponse200.from_dict(response.json())
+        response_200 = GetMyShipsResponse200.update_forward_refs()
+        GetMyShipsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -60,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetMyShipsResponse200]:
     """List Ships
 
      Retrieve all of your ships.
 
@@ -81,30 +82,30 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyShipsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetMyShipsResponse200]:
     """List Ships
 
      Retrieve all of your ships.
 
@@ -117,23 +118,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetMyShipsResponse200
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetMyShipsResponse200]:
     """List Ships
 
      Retrieve all of your ships.
 
@@ -146,28 +147,28 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetMyShipsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetMyShipsResponse200]:
     """List Ships
 
      Retrieve all of your ships.
 
@@ -181,12 +182,12 @@
 
     Returns:
         GetMyShipsResponse200
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             page=page,
             limit=limit,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.2.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.get_ship_cooldown_response_200 import GetShipCooldownResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/cooldown".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[Union[Any, GetShipCooldownResponse200]]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipCooldownResponse200.from_dict(response.json())
+        response_200 = GetShipCooldownResponse200.update_forward_refs()
+        GetShipCooldownResponse200(**response.json())
 
         return response_200
     if response.status_code == HTTPStatus.NO_CONTENT:
         response_204 = cast(Any, None)
         return response_204
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
@@ -57,15 +58,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[Union[Any, GetShipCooldownResponse200]]:
     """Get Ship Cooldown
 
      Retrieve the details of your ship's reactor cooldown. Some actions such as activating your jump
     drive, scanning, or extracting resources taxes your reactor and results in a cooldown.
 
     Your ship cannot perform additional actions until your cooldown has expired. The duration of your
@@ -82,29 +83,29 @@
 
     Returns:
         Response[Union[Any, GetShipCooldownResponse200]]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[Union[Any, GetShipCooldownResponse200]]:
     """Get Ship Cooldown
 
      Retrieve the details of your ship's reactor cooldown. Some actions such as activating your jump
     drive, scanning, or extracting resources taxes your reactor and results in a cooldown.
 
     Your ship cannot perform additional actions until your cooldown has expired. The duration of your
@@ -121,22 +122,22 @@
 
     Returns:
         Union[Any, GetShipCooldownResponse200]
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[Union[Any, GetShipCooldownResponse200]]:
     """Get Ship Cooldown
 
      Retrieve the details of your ship's reactor cooldown. Some actions such as activating your jump
     drive, scanning, or extracting resources taxes your reactor and results in a cooldown.
 
     Your ship cannot perform additional actions until your cooldown has expired. The duration of your
@@ -153,27 +154,27 @@
 
     Returns:
         Response[Union[Any, GetShipCooldownResponse200]]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[Union[Any, GetShipCooldownResponse200]]:
     """Get Ship Cooldown
 
      Retrieve the details of your ship's reactor cooldown. Some actions such as activating your jump
     drive, scanning, or extracting resources taxes your reactor and results in a cooldown.
 
     Your ship cannot perform additional actions until your cooldown has expired. The duration of your
@@ -191,10 +192,10 @@
     Returns:
         Union[Any, GetShipCooldownResponse200]
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.2.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,36 +8,39 @@
 from ...models.get_ship_nav_response_200 import GetShipNavResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/nav".format(client.base_url, shipSymbol=ship_symbol)
+    url = "{}/my/ships/{shipSymbol}/nav".format(
+        _client.base_url, shipSymbol=ship_symbol
+    )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetShipNavResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipNavResponse200.from_dict(response.json())
+        response_200 = GetShipNavResponse200.update_forward_refs()
+        GetShipNavResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -52,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetShipNavResponse200]:
     """Get Ship Nav
 
      Get the current nav status of a ship.
 
     Args:
         ship_symbol (str):
@@ -71,29 +74,29 @@
 
     Returns:
         Response[GetShipNavResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetShipNavResponse200]:
     """Get Ship Nav
 
      Get the current nav status of a ship.
 
     Args:
         ship_symbol (str):
@@ -104,22 +107,22 @@
 
     Returns:
         GetShipNavResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetShipNavResponse200]:
     """Get Ship Nav
 
      Get the current nav status of a ship.
 
     Args:
         ship_symbol (str):
@@ -130,27 +133,27 @@
 
     Returns:
         Response[GetShipNavResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetShipNavResponse200]:
     """Get Ship Nav
 
      Get the current nav status of a ship.
 
     Args:
         ship_symbol (str):
@@ -162,10 +165,10 @@
     Returns:
         GetShipNavResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/jettison.py` & `spacetraders-0.2.0/spacetraders/api/fleet/jettison.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.jettison_response_200 import JettisonResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: JettisonJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/jettison".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[JettisonResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = JettisonResponse200.from_dict(response.json())
+        response_200 = JettisonResponse200.update_forward_refs()
+        JettisonResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JettisonJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JettisonJsonBody,
 ) -> Response[JettisonResponse200]:
     """Jettison Cargo
 
      Jettison cargo from your ship's cargo hold.
 
     Args:
         ship_symbol (str):
@@ -78,33 +79,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JettisonResponse200]
     """
 
+    json_body = JettisonJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JettisonJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JettisonJsonBody,
 ) -> Optional[JettisonResponse200]:
     """Jettison Cargo
 
      Jettison cargo from your ship's cargo hold.
 
     Args:
         ship_symbol (str):
@@ -116,24 +119,24 @@
 
     Returns:
         JettisonResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JettisonJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JettisonJsonBody,
 ) -> Response[JettisonResponse200]:
     """Jettison Cargo
 
      Jettison cargo from your ship's cargo hold.
 
     Args:
         ship_symbol (str):
@@ -143,31 +146,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JettisonResponse200]
     """
 
+    json_body = JettisonJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JettisonJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JettisonJsonBody,
 ) -> Optional[JettisonResponse200]:
     """Jettison Cargo
 
      Jettison cargo from your ship's cargo hold.
 
     Args:
         ship_symbol (str):
@@ -180,11 +185,11 @@
     Returns:
         JettisonResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/jump_ship.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.jump_ship_response_200 import JumpShipResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: JumpShipJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/jump".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[JumpShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = JumpShipResponse200.from_dict(response.json())
+        response_200 = JumpShipResponse200.update_forward_refs()
+        JumpShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JumpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
      Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
     unit of antimatter.
 
     Args:
@@ -79,33 +80,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JumpShipResponse200]
     """
 
+    json_body = JumpShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JumpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JumpShipJsonBody,
 ) -> Optional[JumpShipResponse200]:
     """Jump Ship
 
      Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
     unit of antimatter.
 
     Args:
@@ -118,24 +121,24 @@
 
     Returns:
         JumpShipResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JumpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JumpShipJsonBody,
 ) -> Response[JumpShipResponse200]:
     """Jump Ship
 
      Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
     unit of antimatter.
 
     Args:
@@ -146,31 +149,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[JumpShipResponse200]
     """
 
+    json_body = JumpShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: JumpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: JumpShipJsonBody,
 ) -> Optional[JumpShipResponse200]:
     """Jump Ship
 
      Jump your ship instantly to a target system. Unlike other forms of navigation, jumping requires a
     unit of antimatter.
 
     Args:
@@ -184,11 +189,11 @@
     Returns:
         JumpShipResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.navigate_ship_response_200 import NavigateShipResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: NavigateShipJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/navigate".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[NavigateShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = NavigateShipResponse200.from_dict(response.json())
+        response_200 = NavigateShipResponse200.update_forward_refs()
+        NavigateShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: NavigateShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: NavigateShipJsonBody,
 ) -> Response[NavigateShipResponse200]:
     """Navigate Ship
 
      Navigate to a target destination. The destination must be located within the same system as the
     ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
     out crew wages from the agent's account.
 
@@ -85,33 +86,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NavigateShipResponse200]
     """
 
+    json_body = NavigateShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: NavigateShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: NavigateShipJsonBody,
 ) -> Optional[NavigateShipResponse200]:
     """Navigate Ship
 
      Navigate to a target destination. The destination must be located within the same system as the
     ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
     out crew wages from the agent's account.
 
@@ -130,24 +133,24 @@
 
     Returns:
         NavigateShipResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: NavigateShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: NavigateShipJsonBody,
 ) -> Response[NavigateShipResponse200]:
     """Navigate Ship
 
      Navigate to a target destination. The destination must be located within the same system as the
     ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
     out crew wages from the agent's account.
 
@@ -164,31 +167,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[NavigateShipResponse200]
     """
 
+    json_body = NavigateShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: NavigateShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: NavigateShipJsonBody,
 ) -> Optional[NavigateShipResponse200]:
     """Navigate Ship
 
      Navigate to a target destination. The destination must be located within the same system as the
     ship. Navigating will consume the necessary fuel and supplies from the ship's manifest, and will pay
     out crew wages from the agent's account.
 
@@ -208,11 +213,11 @@
     Returns:
         NavigateShipResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.orbit_ship_orbit_ship_200_response import OrbitShipOrbitShip200Response
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/orbit".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[OrbitShipOrbitShip200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = OrbitShipOrbitShip200Response.from_dict(response.json())
+        response_200 = OrbitShipOrbitShip200Response.update_forward_refs()
+        OrbitShipOrbitShip200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
      Attempt to move your ship into orbit at it's current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
@@ -76,29 +77,29 @@
 
     Returns:
         Response[OrbitShipOrbitShip200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
      Attempt to move your ship into orbit at it's current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
@@ -112,22 +113,22 @@
 
     Returns:
         OrbitShipOrbitShip200Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
      Attempt to move your ship into orbit at it's current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
@@ -141,27 +142,27 @@
 
     Returns:
         Response[OrbitShipOrbitShip200Response]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[OrbitShipOrbitShip200Response]:
     """Orbit Ship
 
      Attempt to move your ship into orbit at it's current location. The request will only succeed if your
     ship is capable of moving into orbit at the time of the request.
 
     The endpoint is idempotent - successive calls will succeed even if the ship is already in orbit.
@@ -176,10 +177,10 @@
     Returns:
         OrbitShipOrbitShip200Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.2.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,40 +9,43 @@
 from ...models.patch_ship_nav_response_200 import PatchShipNavResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: PatchShipNavJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships/{shipSymbol}/nav".format(client.base_url, shipSymbol=ship_symbol)
+    url = "{}/my/ships/{shipSymbol}/nav".format(
+        _client.base_url, shipSymbol=ship_symbol
+    )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "patch",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PatchShipNavResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = PatchShipNavResponse200.from_dict(response.json())
+        response_200 = PatchShipNavResponse200.update_forward_refs()
+        PatchShipNavResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -57,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PatchShipNavJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PatchShipNavJsonBody,
 ) -> Response[PatchShipNavResponse200]:
     """Patch Ship Nav
 
      Update the nav data of a ship, such as the flight mode.
 
     Args:
         ship_symbol (str):
@@ -76,33 +79,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PatchShipNavResponse200]
     """
 
+    json_body = PatchShipNavJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PatchShipNavJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PatchShipNavJsonBody,
 ) -> Optional[PatchShipNavResponse200]:
     """Patch Ship Nav
 
      Update the nav data of a ship, such as the flight mode.
 
     Args:
         ship_symbol (str):
@@ -114,24 +119,24 @@
 
     Returns:
         PatchShipNavResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PatchShipNavJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PatchShipNavJsonBody,
 ) -> Response[PatchShipNavResponse200]:
     """Patch Ship Nav
 
      Update the nav data of a ship, such as the flight mode.
 
     Args:
         ship_symbol (str):
@@ -141,31 +146,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PatchShipNavResponse200]
     """
 
+    json_body = PatchShipNavJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PatchShipNavJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PatchShipNavJsonBody,
 ) -> Optional[PatchShipNavResponse200]:
     """Patch Ship Nav
 
      Update the nav data of a ship, such as the flight mode.
 
     Args:
         ship_symbol (str):
@@ -178,11 +185,11 @@
     Returns:
         PatchShipNavResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.2.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 )
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/purchase".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PurchaseCargoPurchaseCargo201Response]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = PurchaseCargoPurchaseCargo201Response.from_dict(response.json())
+        response_201 = PurchaseCargoPurchaseCargo201Response.update_forward_refs()
+        PurchaseCargoPurchaseCargo201Response(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -63,16 +64,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseCargoPurchaseCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Response[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
      Purchase cargo.
 
     Args:
         ship_symbol (str):
@@ -82,33 +83,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseCargoPurchaseCargo201Response]
     """
 
+    json_body = PurchaseCargoPurchaseCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseCargoPurchaseCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Optional[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
      Purchase cargo.
 
     Args:
         ship_symbol (str):
@@ -120,24 +123,24 @@
 
     Returns:
         PurchaseCargoPurchaseCargo201Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseCargoPurchaseCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Response[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
      Purchase cargo.
 
     Args:
         ship_symbol (str):
@@ -147,31 +150,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseCargoPurchaseCargo201Response]
     """
 
+    json_body = PurchaseCargoPurchaseCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseCargoPurchaseCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseCargoPurchaseCargoRequest,
 ) -> Optional[PurchaseCargoPurchaseCargo201Response]:
     """Purchase Cargo
 
      Purchase cargo.
 
     Args:
         ship_symbol (str):
@@ -184,11 +189,11 @@
     Returns:
         PurchaseCargoPurchaseCargo201Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/purchase_ship.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,40 +8,41 @@
 from ...models.purchase_ship_json_body import PurchaseShipJsonBody
 from ...models.purchase_ship_response_201 import PurchaseShipResponse201
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: PurchaseShipJsonBody,
 ) -> Dict[str, Any]:
-    url = "{}/my/ships".format(client.base_url)
+    url = "{}/my/ships".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[PurchaseShipResponse201]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = PurchaseShipResponse201.from_dict(response.json())
+        response_201 = PurchaseShipResponse201.update_forward_refs()
+        PurchaseShipResponse201(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -55,16 +56,16 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseShipJsonBody,
 ) -> Response[PurchaseShipResponse201]:
     """Purchase Ship
 
      Purchase a ship
 
     Args:
         json_body (PurchaseShipJsonBody):
@@ -73,31 +74,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseShipResponse201]
     """
 
+    json_body = PurchaseShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseShipJsonBody,
 ) -> Optional[PurchaseShipResponse201]:
     """Purchase Ship
 
      Purchase a ship
 
     Args:
         json_body (PurchaseShipJsonBody):
@@ -107,23 +110,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         PurchaseShipResponse201
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseShipJsonBody,
 ) -> Response[PurchaseShipResponse201]:
     """Purchase Ship
 
      Purchase a ship
 
     Args:
         json_body (PurchaseShipJsonBody):
@@ -132,29 +135,31 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[PurchaseShipResponse201]
     """
 
+    json_body = PurchaseShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
-    json_body: PurchaseShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: PurchaseShipJsonBody,
 ) -> Optional[PurchaseShipResponse201]:
     """Purchase Ship
 
      Purchase a ship
 
     Args:
         json_body (PurchaseShipJsonBody):
@@ -165,11 +170,11 @@
 
     Returns:
         PurchaseShipResponse201
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.refuel_ship_response_200 import RefuelShipResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/refuel".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[RefuelShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = RefuelShipResponse200.from_dict(response.json())
+        response_200 = RefuelShipResponse200.update_forward_refs()
+        RefuelShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[RefuelShipResponse200]:
     """Refuel Ship
 
      Refuel your ship from the local market.
 
     Args:
         ship_symbol (str):
@@ -73,29 +74,29 @@
 
     Returns:
         Response[RefuelShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[RefuelShipResponse200]:
     """Refuel Ship
 
      Refuel your ship from the local market.
 
     Args:
         ship_symbol (str):
@@ -106,22 +107,22 @@
 
     Returns:
         RefuelShipResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[RefuelShipResponse200]:
     """Refuel Ship
 
      Refuel your ship from the local market.
 
     Args:
         ship_symbol (str):
@@ -132,27 +133,27 @@
 
     Returns:
         Response[RefuelShipResponse200]
     """
 
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[RefuelShipResponse200]:
     """Refuel Ship
 
      Refuel your ship from the local market.
 
     Args:
         ship_symbol (str):
@@ -164,10 +165,10 @@
     Returns:
         RefuelShipResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.2.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.sell_cargo_sell_cargo_request import SellCargoSellCargoRequest
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: SellCargoSellCargoRequest,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/sell".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[SellCargoSellCargo201Response]:
     if response.status_code == HTTPStatus.CREATED:
-        response_201 = SellCargoSellCargo201Response.from_dict(response.json())
+        response_201 = SellCargoSellCargo201Response.update_forward_refs()
+        SellCargoSellCargo201Response(**response.json())
 
         return response_201
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: SellCargoSellCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: SellCargoSellCargoRequest,
 ) -> Response[SellCargoSellCargo201Response]:
     """Sell Cargo
 
      Sell cargo.
 
     Args:
         ship_symbol (str):
@@ -78,33 +79,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SellCargoSellCargo201Response]
     """
 
+    json_body = SellCargoSellCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: SellCargoSellCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: SellCargoSellCargoRequest,
 ) -> Optional[SellCargoSellCargo201Response]:
     """Sell Cargo
 
      Sell cargo.
 
     Args:
         ship_symbol (str):
@@ -116,24 +119,24 @@
 
     Returns:
         SellCargoSellCargo201Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: SellCargoSellCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: SellCargoSellCargoRequest,
 ) -> Response[SellCargoSellCargo201Response]:
     """Sell Cargo
 
      Sell cargo.
 
     Args:
         ship_symbol (str):
@@ -143,31 +146,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[SellCargoSellCargo201Response]
     """
 
+    json_body = SellCargoSellCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: SellCargoSellCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: SellCargoSellCargoRequest,
 ) -> Optional[SellCargoSellCargo201Response]:
     """Sell Cargo
 
      Sell cargo.
 
     Args:
         ship_symbol (str):
@@ -180,11 +185,11 @@
     Returns:
         SellCargoSellCargo201Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.2.0/spacetraders/api/fleet/ship_refine.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,42 +11,43 @@
 )
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: ShipRefineJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/refine".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[ShipRefineShipRefine200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = ShipRefineShipRefine200Response.from_dict(response.json())
+        response_200 = ShipRefineShipRefine200Response.update_forward_refs()
+        ShipRefineShipRefine200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -61,16 +62,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ShipRefineJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ShipRefineJsonBody,
 ) -> Response[ShipRefineShipRefine200Response]:
     """Ship Refine
 
      Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
     capable of refining at the time of the request.
 
     Args:
@@ -81,33 +82,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ShipRefineShipRefine200Response]
     """
 
+    json_body = ShipRefineJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ShipRefineJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ShipRefineJsonBody,
 ) -> Optional[ShipRefineShipRefine200Response]:
     """Ship Refine
 
      Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
     capable of refining at the time of the request.
 
     Args:
@@ -120,24 +123,24 @@
 
     Returns:
         ShipRefineShipRefine200Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ShipRefineJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ShipRefineJsonBody,
 ) -> Response[ShipRefineShipRefine200Response]:
     """Ship Refine
 
      Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
     capable of refining at the time of the request.
 
     Args:
@@ -148,31 +151,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[ShipRefineShipRefine200Response]
     """
 
+    json_body = ShipRefineJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: ShipRefineJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: ShipRefineJsonBody,
 ) -> Optional[ShipRefineShipRefine200Response]:
     """Ship Refine
 
      Attempt to refine the raw materials on your ship. The request will only succeed if your ship is
     capable of refining at the time of the request.
 
     Args:
@@ -186,11 +191,11 @@
     Returns:
         ShipRefineShipRefine200Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.2.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,42 +13,43 @@
 )
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: TransferCargoTransferCargoRequest,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/transfer".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[TransferCargoTransferCargo200Response]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = TransferCargoTransferCargo200Response.from_dict(response.json())
+        response_200 = TransferCargoTransferCargo200Response.update_forward_refs()
+        TransferCargoTransferCargo200Response(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -63,16 +64,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: TransferCargoTransferCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: TransferCargoTransferCargoRequest,
 ) -> Response[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
     Args:
         ship_symbol (str):
@@ -82,33 +83,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[TransferCargoTransferCargo200Response]
     """
 
+    json_body = TransferCargoTransferCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: TransferCargoTransferCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: TransferCargoTransferCargoRequest,
 ) -> Optional[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
     Args:
         ship_symbol (str):
@@ -120,24 +123,24 @@
 
     Returns:
         TransferCargoTransferCargo200Response
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: TransferCargoTransferCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: TransferCargoTransferCargoRequest,
 ) -> Response[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
     Args:
         ship_symbol (str):
@@ -147,31 +150,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[TransferCargoTransferCargo200Response]
     """
 
+    json_body = TransferCargoTransferCargoRequest(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: TransferCargoTransferCargoRequest,
+    _client: AuthenticatedClient,
+    **json_body: TransferCargoTransferCargoRequest,
 ) -> Optional[TransferCargoTransferCargo200Response]:
     """Transfer Cargo
 
      Transfer cargo between ships.
 
     Args:
         ship_symbol (str):
@@ -184,11 +189,11 @@
     Returns:
         TransferCargoTransferCargo200Response
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.2.0/spacetraders/api/fleet/warp_ship.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,42 +9,43 @@
 from ...models.warp_ship_response_200 import WarpShipResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     json_body: WarpShipJsonBody,
 ) -> Dict[str, Any]:
     url = "{}/my/ships/{shipSymbol}/warp".format(
-        client.base_url, shipSymbol=ship_symbol
+        _client.base_url, shipSymbol=ship_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
-    json_json_body = json_body.to_dict()
+    json_json_body = json_body.dict()
 
     return {
         "method": "post",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "json": json_json_body,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[WarpShipResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = WarpShipResponse200.from_dict(response.json())
+        response_200 = WarpShipResponse200.update_forward_refs()
+        WarpShipResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -59,16 +60,16 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: WarpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: WarpShipJsonBody,
 ) -> Response[WarpShipResponse200]:
     """Warp Ship
 
      Warp your ship to a target destination in another system. Warping will consume the necessary fuel
     and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
 
     The returned response will detail the route information including the expected time of arrival. Most
@@ -82,33 +83,35 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[WarpShipResponse200]
     """
 
+    json_body = WarpShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: WarpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: WarpShipJsonBody,
 ) -> Optional[WarpShipResponse200]:
     """Warp Ship
 
      Warp your ship to a target destination in another system. Warping will consume the necessary fuel
     and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
 
     The returned response will detail the route information including the expected time of arrival. Most
@@ -124,24 +127,24 @@
 
     Returns:
         WarpShipResponse200
     """
 
     return sync_detailed(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     ).parsed
 
 
 async def asyncio_detailed(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: WarpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: WarpShipJsonBody,
 ) -> Response[WarpShipResponse200]:
     """Warp Ship
 
      Warp your ship to a target destination in another system. Warping will consume the necessary fuel
     and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
 
     The returned response will detail the route information including the expected time of arrival. Most
@@ -155,31 +158,33 @@
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[WarpShipResponse200]
     """
 
+    json_body = WarpShipJsonBody(**json_body)
+
     kwargs = _get_kwargs(
         ship_symbol=ship_symbol,
-        client=client,
+        _client=_client,
         json_body=json_body,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     ship_symbol: str,
     *,
-    client: AuthenticatedClient,
-    json_body: WarpShipJsonBody,
+    _client: AuthenticatedClient,
+    **json_body: WarpShipJsonBody,
 ) -> Optional[WarpShipResponse200]:
     """Warp Ship
 
      Warp your ship to a target destination in another system. Warping will consume the necessary fuel
     and supplies from the ship's manifest, and will pay out crew wages from the agent's account.
 
     The returned response will detail the route information including the expected time of arrival. Most
@@ -196,11 +201,11 @@
     Returns:
         WarpShipResponse200
     """
 
     return (
         await asyncio_detailed(
             ship_symbol=ship_symbol,
-            client=client,
+            _client=_client,
             json_body=json_body,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_shipyard.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,186 +1,187 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
+from ...models.get_shipyard_response_200 import GetShipyardResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
-        client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetJumpGateResponse200]:
+) -> Optional[GetShipyardResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetJumpGateResponse200.from_dict(response.json())
+        response_200 = GetShipyardResponse200.update_forward_refs()
+        GetShipyardResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetJumpGateResponse200]:
+) -> Response[GetShipyardResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetJumpGateResponse200]:
-    """Get Jump Gate
+    _client: AuthenticatedClient,
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJumpGateResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetJumpGateResponse200]:
-    """Get Jump Gate
+    _client: AuthenticatedClient,
+) -> Optional[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetJumpGateResponse200
+        GetShipyardResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetJumpGateResponse200]:
-    """Get Jump Gate
+    _client: AuthenticatedClient,
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetJumpGateResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetJumpGateResponse200]:
-    """Get Jump Gate
+    _client: AuthenticatedClient,
+) -> Optional[GetShipyardResponse200]:
+    """Get Shipyard
 
-     Get jump gate details for a waypoint.
+     Get the shipyard for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetJumpGateResponse200
+        GetShipyardResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
             waypoint_symbol=waypoint_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_market.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_market.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,38 +9,39 @@
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/market".format(
-        client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetMarketResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetMarketResponse200.from_dict(response.json())
+        response_200 = GetMarketResponse200.update_forward_refs()
+        GetMarketResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -56,15 +57,15 @@
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
 
@@ -79,30 +80,30 @@
     Returns:
         Response[GetMarketResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
 
@@ -117,23 +118,23 @@
     Returns:
         GetMarketResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
 
@@ -148,28 +149,28 @@
     Returns:
         Response[GetMarketResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetMarketResponse200]:
     """Get Market
 
      Retrieve imports, exports and exchange data from a marketplace. Imports can be sold, exports can be
     purchased, and exchange goods can be purchased or sold. Send a ship to the waypoint to access trade
     good prices and recent transactions.
 
@@ -185,10 +186,10 @@
         GetMarketResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
             waypoint_symbol=waypoint_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_waypoint.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,186 +1,187 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_shipyard_response_200 import GetShipyardResponse200
+from ...models.get_waypoint_response_200 import GetWaypointResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
-        client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetShipyardResponse200]:
+) -> Optional[GetWaypointResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipyardResponse200.from_dict(response.json())
+        response_200 = GetWaypointResponse200.update_forward_refs()
+        GetWaypointResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetShipyardResponse200]:
+) -> Response[GetWaypointResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
+    _client: AuthenticatedClient,
+) -> Response[GetWaypointResponse200]:
+    """Get Waypoint
 
-     Get the shipyard for a waypoint.
+     View the details of a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetShipyardResponse200]
+        Response[GetWaypointResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetShipyardResponse200]:
-    """Get Shipyard
+    _client: AuthenticatedClient,
+) -> Optional[GetWaypointResponse200]:
+    """Get Waypoint
 
-     Get the shipyard for a waypoint.
+     View the details of a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetShipyardResponse200
+        GetWaypointResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
+    _client: AuthenticatedClient,
+) -> Response[GetWaypointResponse200]:
+    """Get Waypoint
 
-     Get the shipyard for a waypoint.
+     View the details of a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetShipyardResponse200]
+        Response[GetWaypointResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetShipyardResponse200]:
-    """Get Shipyard
+    _client: AuthenticatedClient,
+) -> Optional[GetWaypointResponse200]:
+    """Get Waypoint
 
-     Get the shipyard for a waypoint.
+     View the details of a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetShipyardResponse200
+        GetWaypointResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
             waypoint_symbol=waypoint_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_system.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,38 +8,39 @@
 from ...models.get_system_response_200 import GetSystemResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     system_symbol: str = "X1-OE",
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}".format(
-        client.base_url, systemSymbol=system_symbol
+        _client.base_url, systemSymbol=system_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemResponse200.from_dict(response.json())
+        response_200 = GetSystemResponse200.update_forward_refs()
+        GetSystemResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -54,15 +55,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str = "X1-OE",
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
         system_symbol (str):  Default: 'X1-OE'.
@@ -73,29 +74,29 @@
 
     Returns:
         Response[GetSystemResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str = "X1-OE",
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
         system_symbol (str):  Default: 'X1-OE'.
@@ -106,22 +107,22 @@
 
     Returns:
         GetSystemResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str = "X1-OE",
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Response[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
         system_symbol (str):  Default: 'X1-OE'.
@@ -132,27 +133,27 @@
 
     Returns:
         Response[GetSystemResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str = "X1-OE",
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Optional[GetSystemResponse200]:
     """Get System
 
      Get the details of a system.
 
     Args:
         system_symbol (str):  Default: 'X1-OE'.
@@ -164,10 +165,10 @@
     Returns:
         GetSystemResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,48 +8,49 @@
 from ...models.get_system_waypoints_response_200 import GetSystemWaypointsResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     system_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
     url = "{}/systems/{systemSymbol}/waypoints".format(
-        client.base_url, systemSymbol=system_symbol
+        _client.base_url, systemSymbol=system_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
     params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemWaypointsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemWaypointsResponse200.from_dict(response.json())
+        response_200 = GetSystemWaypointsResponse200.update_forward_refs()
+        GetSystemWaypointsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -64,15 +65,15 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemWaypointsResponse200]:
     """List Waypoints
 
      Fetch all of the waypoints for a given system. System must be charted or a ship must be present to
     return waypoint details.
@@ -88,31 +89,31 @@
 
     Returns:
         Response[GetSystemWaypointsResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetSystemWaypointsResponse200]:
     """List Waypoints
 
      Fetch all of the waypoints for a given system. System must be charted or a ship must be present to
     return waypoint details.
@@ -128,24 +129,24 @@
 
     Returns:
         GetSystemWaypointsResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemWaypointsResponse200]:
     """List Waypoints
 
      Fetch all of the waypoints for a given system. System must be charted or a ship must be present to
     return waypoint details.
@@ -161,29 +162,29 @@
 
     Returns:
         Response[GetSystemWaypointsResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetSystemWaypointsResponse200]:
     """List Waypoints
 
      Fetch all of the waypoints for a given system. System must be charted or a ship must be present to
     return waypoint details.
@@ -200,12 +201,12 @@
     Returns:
         GetSystemWaypointsResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
-            client=client,
+            _client=_client,
             page=page,
             limit=limit,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_systems.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_systems.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,46 +7,47 @@
 from ...client import AuthenticatedClient, Client
 from ...models.get_systems_response_200 import GetSystemsResponse200
 from ...types import UNSET, Response, Unset
 
 
 def _get_kwargs(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Dict[str, Any]:
-    url = "{}/systems".format(client.base_url)
+    url = "{}/systems".format(_client.base_url)
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     params: Dict[str, Any] = {}
     params["page"] = page
 
     params["limit"] = limit
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
         "params": params,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
 ) -> Optional[GetSystemsResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetSystemsResponse200.from_dict(response.json())
+        response_200 = GetSystemsResponse200.update_forward_refs()
+        GetSystemsResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
@@ -60,15 +61,15 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
 
@@ -81,30 +82,30 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetSystemsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
 
@@ -117,23 +118,23 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         GetSystemsResponse200
     """
 
     return sync_detailed(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     ).parsed
 
 
 async def asyncio_detailed(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Response[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
 
@@ -146,28 +147,28 @@
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[GetSystemsResponse200]
     """
 
     kwargs = _get_kwargs(
-        client=client,
+        _client=_client,
         page=page,
         limit=limit,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
     page: Union[Unset, None, int] = UNSET,
     limit: Union[Unset, None, int] = UNSET,
 ) -> Optional[GetSystemsResponse200]:
     """List Systems
 
      Return a list of all systems.
 
@@ -181,12 +182,12 @@
 
     Returns:
         GetSystemsResponse200
     """
 
     return (
         await asyncio_detailed(
-            client=client,
+            _client=_client,
             page=page,
             limit=limit,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.2.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,186 +1,187 @@
 from http import HTTPStatus
 from typing import Any, Dict, List, Optional, Union, cast
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_waypoint_response_200 import GetWaypointResponse200
+from ...models.get_jump_gate_response_200 import GetJumpGateResponse200
 from ...types import UNSET, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
+    _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
-        client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/jump-gate".format(
+        _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
-    headers: Dict[str, str] = client.get_headers()
-    cookies: Dict[str, Any] = client.get_cookies()
+    headers: Dict[str, str] = _client.get_headers()
+    cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
         "method": "get",
         "url": url,
         "headers": headers,
         "cookies": cookies,
-        "timeout": client.get_timeout(),
-        "follow_redirects": client.follow_redirects,
+        "timeout": _client.get_timeout(),
+        "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetWaypointResponse200]:
+) -> Optional[GetJumpGateResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetWaypointResponse200.from_dict(response.json())
+        response_200 = GetJumpGateResponse200.update_forward_refs()
+        GetJumpGateResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetWaypointResponse200]:
+) -> Response[GetJumpGateResponse200]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetWaypointResponse200]:
-    """Get Waypoint
+    _client: AuthenticatedClient,
+) -> Response[GetJumpGateResponse200]:
+    """Get Jump Gate
 
-     View the details of a waypoint.
+     Get jump gate details for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetWaypointResponse200]
+        Response[GetJumpGateResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
     response = httpx.request(
-        verify=client.verify_ssl,
+        verify=_client.verify_ssl,
         **kwargs,
     )
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 def sync(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetWaypointResponse200]:
-    """Get Waypoint
+    _client: AuthenticatedClient,
+) -> Optional[GetJumpGateResponse200]:
+    """Get Jump Gate
 
-     View the details of a waypoint.
+     Get jump gate details for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetWaypointResponse200
+        GetJumpGateResponse200
     """
 
     return sync_detailed(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     ).parsed
 
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Response[GetWaypointResponse200]:
-    """Get Waypoint
+    _client: AuthenticatedClient,
+) -> Response[GetJumpGateResponse200]:
+    """Get Jump Gate
 
-     View the details of a waypoint.
+     Get jump gate details for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetWaypointResponse200]
+        Response[GetJumpGateResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
-        client=client,
+        _client=_client,
     )
 
-    async with httpx.AsyncClient(verify=client.verify_ssl) as _client:
-        response = await _client.request(**kwargs)
+    async with httpx.AsyncClient(verify=_client.verify_ssl) as c:
+        response = await c.request(**kwargs)
 
-    return _build_response(client=client, response=response)
+    return _build_response(client=_client, response=response)
 
 
 async def asyncio(
     system_symbol: str,
     waypoint_symbol: str,
     *,
-    client: AuthenticatedClient,
-) -> Optional[GetWaypointResponse200]:
-    """Get Waypoint
+    _client: AuthenticatedClient,
+) -> Optional[GetJumpGateResponse200]:
+    """Get Jump Gate
 
-     View the details of a waypoint.
+     Get jump gate details for a waypoint.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetWaypointResponse200
+        GetJumpGateResponse200
     """
 
     return (
         await asyncio_detailed(
             system_symbol=system_symbol,
             waypoint_symbol=waypoint_symbol,
-            client=client,
+            _client=_client,
         )
     ).parsed
```

### Comparing `spacetraders-0.1.4/spacetraders/client.py` & `spacetraders-0.2.0/spacetraders/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             imp = import_module(f".{attr}", self._module.__package__)
         else:
             imp = getattr(self._module, attr)
 
         if not hasattr(imp, self._exec_mode):
             return APIStub(client=self._client, mod=imp, exec=self._exec_mode)
 
-        return partial(getattr(imp, self._exec_mode), client=self._client)
+        return partial(getattr(imp, self._exec_mode), _client=self._client)
 
 
 @attr.s(auto_attribs=True)
 class Client:
     """A class for keeping track of data related to the API
 
     Attributes:
```

### Comparing `spacetraders-0.1.4/spacetraders/models/__init__.py` & `spacetraders-0.2.0/spacetraders/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.2.0/spacetraders/models/contract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     List,
     Optional,
@@ -9,66 +10,47 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
+from ..models.contract_terms import ContractTerms
+from ..models.contract_type import ContractType
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.accept_contract_response_200_data import AcceptContractResponse200Data
+T = TypeVar("T", bound="Contract")
 
 
-T = TypeVar("T", bound="AcceptContractResponse200")
-
-
-@attr.s(auto_attribs=True)
-class AcceptContractResponse200:
+class Contract(BaseModel):
     """
     Attributes:
-        data (AcceptContractResponse200Data):
+        id (str):
+        faction_symbol (str): The symbol of the faction that this contract is for.
+        type (ContractType):
+        terms (ContractTerms):
+        accepted (bool): Whether the contract has been accepted by the agent
+        fulfilled (bool): Whether the contract has been fulfilled
+        expiration (datetime.datetime): The time at which the contract expires
     """
 
-    data: "AcceptContractResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.accept_contract_response_200_data import (
-            AcceptContractResponse200Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.accept_contract_response_200_data import (
-            AcceptContractResponse200Data,
-        )
-
-        d = src_dict.copy()
-        data = AcceptContractResponse200Data.from_dict(d.pop("data"))
-
-        accept_contract_response_200 = cls(
-            data=data,
-        )
+    id: str = Field(alias="id")
+    faction_symbol: str = Field(alias="factionSymbol")
+    type: ContractType = Field(alias="type")
+    terms: "ContractTerms" = Field(alias="terms")
+    expiration: datetime.datetime = Field(alias="expiration")
+    accepted: bool = False
+    fulfilled: bool = False
+    additional_properties: Dict[str, Any] = {}
 
-        accept_contract_response_200.additional_properties = d
-        return accept_contract_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/contract_terms.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,49 @@
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
+    Union,
     cast,
 )
 
 import attr
+from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
+from ..models.contract_deliver_good import ContractDeliverGood
+from ..models.contract_payment import ContractPayment
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.agent import Agent
-    from ..models.contract import Contract
+T = TypeVar("T", bound="ContractTerms")
 
 
-T = TypeVar("T", bound="AcceptContractResponse200Data")
-
-
-@attr.s(auto_attribs=True)
-class AcceptContractResponse200Data:
+class ContractTerms(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
+        deadline (datetime.datetime): The deadline for the contract.
+        payment (ContractPayment):
+        deliver (Union[Unset, List['ContractDeliverGood']]):
     """
 
-    agent: "Agent"
-    contract: "Contract"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.agent import Agent
-        from ..models.contract import Contract
-
-        agent = self.agent.to_dict()
-
-        contract = self.contract.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "agent": agent,
-                "contract": contract,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.agent import Agent
-        from ..models.contract import Contract
-
-        d = src_dict.copy()
-        agent = Agent.from_dict(d.pop("agent"))
-
-        contract = Contract.from_dict(d.pop("contract"))
-
-        accept_contract_response_200_data = cls(
-            agent=agent,
-            contract=contract,
-        )
+    deadline: datetime.datetime = Field(alias="deadline")
+    payment: "ContractPayment" = Field(alias="payment")
+    deliver: Union[Unset, List["ContractDeliverGood"]] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        accept_contract_response_200_data.additional_properties = d
-        return accept_contract_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/agent.py` & `spacetraders-0.2.0/spacetraders/models/agent.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,76 +8,39 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="Agent")
 
 
-@attr.s(auto_attribs=True)
-class Agent:
+class Agent(BaseModel):
     """
     Attributes:
         account_id (str):
         symbol (str):
         headquarters (str): The headquarters of the agent.
         credits_ (int): The number of credits the agent has available. Credits can be negative if funds have been
             overdrawn.
     """
 
-    account_id: str
-    symbol: str
-    headquarters: str
-    credits_: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        account_id = self.account_id
-        symbol = self.symbol
-        headquarters = self.headquarters
-        credits_ = self.credits_
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "accountId": account_id,
-                "symbol": symbol,
-                "headquarters": headquarters,
-                "credits": credits_,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        account_id = d.pop("accountId")
-
-        symbol = d.pop("symbol")
-
-        headquarters = d.pop("headquarters")
-
-        credits_ = d.pop("credits")
-
-        agent = cls(
-            account_id=account_id,
-            symbol=symbol,
-            headquarters=headquarters,
-            credits_=credits_,
-        )
+    account_id: str = Field(alias="accountId")
+    symbol: str = Field(alias="symbol")
+    headquarters: str = Field(alias="headquarters")
+    credits_: int = Field(alias="credits")
+    additional_properties: Dict[str, Any] = {}
 
-        agent.additional_properties = d
-        return agent
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/connected_system.py` & `spacetraders-0.2.0/spacetraders/models/system.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,103 +5,51 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.system_faction import SystemFaction
 from ..models.system_type import SystemType
+from ..models.system_waypoint import SystemWaypoint
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ConnectedSystem")
+T = TypeVar("T", bound="System")
 
 
-@attr.s(auto_attribs=True)
-class ConnectedSystem:
+class System(BaseModel):
     """
     Attributes:
         symbol (str):
         sector_symbol (str):
         type (SystemType): The type of waypoint.
         x (int):
         y (int):
-        distance (int):
-        faction_symbol (Union[Unset, str]): The symbol of the faction that owns the connected jump gate in the system.
+        waypoints (List['SystemWaypoint']):
+        factions (List['SystemFaction']):
     """
 
-    symbol: str
-    sector_symbol: str
-    type: SystemType
-    x: int
-    y: int
-    distance: int
-    faction_symbol: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        sector_symbol = self.sector_symbol
-        type = self.type.value
-
-        x = self.x
-        y = self.y
-        distance = self.distance
-        faction_symbol = self.faction_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "sectorSymbol": sector_symbol,
-                "type": type,
-                "x": x,
-                "y": y,
-                "distance": distance,
-            }
-        )
-        if faction_symbol is not UNSET:
-            field_dict["factionSymbol"] = faction_symbol
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        sector_symbol = d.pop("sectorSymbol")
-
-        type = SystemType(d.pop("type"))
-
-        x = d.pop("x")
-
-        y = d.pop("y")
-
-        distance = d.pop("distance")
-
-        faction_symbol = d.pop("factionSymbol", UNSET)
-
-        connected_system = cls(
-            symbol=symbol,
-            sector_symbol=sector_symbol,
-            type=type,
-            x=x,
-            y=y,
-            distance=distance,
-            faction_symbol=faction_symbol,
-        )
+    symbol: str = Field(alias="symbol")
+    sector_symbol: str = Field(alias="sectorSymbol")
+    type: SystemType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    waypoints: List["SystemWaypoint"] = Field(alias="waypoints")
+    factions: List["SystemFaction"] = Field(alias="factions")
+    additional_properties: Dict[str, Any] = {}
 
-        connected_system.additional_properties = d
-        return connected_system
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/contract_payment.py` & `spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,64 +5,37 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ContractPayment")
+T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
 
 
-@attr.s(auto_attribs=True)
-class ContractPayment:
+class OrbitShipOrbitShip200ResponseData(BaseModel):
     """
     Attributes:
-        on_accepted (int): The amount of credits received up front for accepting the contract.
-        on_fulfilled (int): The amount of credits received when the contract is fulfilled.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    on_accepted: int
-    on_fulfilled: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        on_accepted = self.on_accepted
-        on_fulfilled = self.on_fulfilled
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "onAccepted": on_accepted,
-                "onFulfilled": on_fulfilled,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        on_accepted = d.pop("onAccepted")
-
-        on_fulfilled = d.pop("onFulfilled")
-
-        contract_payment = cls(
-            on_accepted=on_accepted,
-            on_fulfilled=on_fulfilled,
-        )
+    nav: "ShipNav" = Field(alias="nav")
+    additional_properties: Dict[str, Any] = {}
 
-        contract_payment.additional_properties = d
-        return contract_payment
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.navigate_ship_response_200_data import NavigateShipResponse200Data
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.create_chart_response_201_data import CreateChartResponse201Data
+T = TypeVar("T", bound="NavigateShipResponse200")
 
 
-T = TypeVar("T", bound="CreateChartResponse201")
-
-
-@attr.s(auto_attribs=True)
-class CreateChartResponse201:
+class NavigateShipResponse200(BaseModel):
     """
     Attributes:
-        data (CreateChartResponse201Data):
+        data (NavigateShipResponse200Data):
     """
 
-    data: "CreateChartResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_chart_response_201_data import CreateChartResponse201Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_chart_response_201_data import CreateChartResponse201Data
-
-        d = src_dict.copy()
-        data = CreateChartResponse201Data.from_dict(d.pop("data"))
-
-        create_chart_response_201 = cls(
-            data=data,
-        )
+    data: "NavigateShipResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        create_chart_response_201.additional_properties = d
-        return create_chart_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.2.0/spacetraders/models/scanned_waypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,77 +5,60 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.chart import Chart
+from ..models.waypoint_faction import WaypointFaction
+from ..models.waypoint_orbital import WaypointOrbital
+from ..models.waypoint_trait import WaypointTrait
+from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.chart import Chart
-    from ..models.waypoint import Waypoint
+T = TypeVar("T", bound="ScannedWaypoint")
 
 
-T = TypeVar("T", bound="CreateChartResponse201Data")
+class ScannedWaypoint(BaseModel):
+    """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
 
-
-@attr.s(auto_attribs=True)
-class CreateChartResponse201Data:
-    """
     Attributes:
-        chart (Chart): The chart of a system or waypoint, which makes the location visible to other agents.
-        waypoint (Waypoint): A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
+        symbol (str):
+        type (WaypointType): The type of waypoint.
+        system_symbol (str):
+        x (int):
+        y (int):
+        orbitals (List['WaypointOrbital']):
+        traits (List['WaypointTrait']): The traits of the waypoint.
+        faction (Union[Unset, WaypointFaction]):
+        chart (Union[Unset, Chart]): The chart of a system or waypoint, which makes the location visible to other
+            agents.
     """
 
-    chart: "Chart"
-    waypoint: "Waypoint"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.chart import Chart
-        from ..models.waypoint import Waypoint
-
-        chart = self.chart.to_dict()
-
-        waypoint = self.waypoint.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "chart": chart,
-                "waypoint": waypoint,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.chart import Chart
-        from ..models.waypoint import Waypoint
-
-        d = src_dict.copy()
-        chart = Chart.from_dict(d.pop("chart"))
-
-        waypoint = Waypoint.from_dict(d.pop("waypoint"))
-
-        create_chart_response_201_data = cls(
-            chart=chart,
-            waypoint=waypoint,
-        )
+    symbol: str = Field(alias="symbol")
+    type: WaypointType = Field(alias="type")
+    system_symbol: str = Field(alias="systemSymbol")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    orbitals: List["WaypointOrbital"] = Field(alias="orbitals")
+    traits: List["WaypointTrait"] = Field(alias="traits")
+    faction: Union[Unset, "WaypointFaction"] = UNSET
+    chart: Union[Unset, "Chart"] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        create_chart_response_201_data.additional_properties = d
-        return create_chart_response_201_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.2.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,68 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.create_ship_ship_scan_response_201_data import (
+    CreateShipShipScanResponse201Data,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.create_ship_ship_scan_response_201_data import (
-        CreateShipShipScanResponse201Data,
-    )
-
-
 T = TypeVar("T", bound="CreateShipShipScanResponse201")
 
 
-@attr.s(auto_attribs=True)
-class CreateShipShipScanResponse201:
+class CreateShipShipScanResponse201(BaseModel):
     """
     Attributes:
         data (CreateShipShipScanResponse201Data):
     """
 
-    data: "CreateShipShipScanResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_ship_ship_scan_response_201_data import (
-            CreateShipShipScanResponse201Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_ship_ship_scan_response_201_data import (
-            CreateShipShipScanResponse201Data,
-        )
-
-        d = src_dict.copy()
-        data = CreateShipShipScanResponse201Data.from_dict(d.pop("data"))
-
-        create_ship_ship_scan_response_201 = cls(
-            data=data,
-        )
+    data: "CreateShipShipScanResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        create_ship_ship_scan_response_201.additional_properties = d
-        return create_ship_ship_scan_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,68 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.create_ship_waypoint_scan_response_201_data import (
+    CreateShipWaypointScanResponse201Data,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.create_ship_system_scan_response_201_data import (
-        CreateShipSystemScanResponse201Data,
-    )
-
+T = TypeVar("T", bound="CreateShipWaypointScanResponse201")
 
-T = TypeVar("T", bound="CreateShipSystemScanResponse201")
 
-
-@attr.s(auto_attribs=True)
-class CreateShipSystemScanResponse201:
+class CreateShipWaypointScanResponse201(BaseModel):
     """
     Attributes:
-        data (CreateShipSystemScanResponse201Data):
+        data (CreateShipWaypointScanResponse201Data):
     """
 
-    data: "CreateShipSystemScanResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_ship_system_scan_response_201_data import (
-            CreateShipSystemScanResponse201Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_ship_system_scan_response_201_data import (
-            CreateShipSystemScanResponse201Data,
-        )
-
-        d = src_dict.copy()
-        data = CreateShipSystemScanResponse201Data.from_dict(d.pop("data"))
-
-        create_ship_system_scan_response_201 = cls(
-            data=data,
-        )
+    data: "CreateShipWaypointScanResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        create_ship_system_scan_response_201.additional_properties = d
-        return create_ship_system_scan_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,68 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.dock_ship_dock_ship_200_response_data import (
+    DockShipDockShip200ResponseData,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.create_ship_waypoint_scan_response_201_data import (
-        CreateShipWaypointScanResponse201Data,
-    )
-
+T = TypeVar("T", bound="DockShipDockShip200Response")
 
-T = TypeVar("T", bound="CreateShipWaypointScanResponse201")
 
-
-@attr.s(auto_attribs=True)
-class CreateShipWaypointScanResponse201:
+class DockShipDockShip200Response(BaseModel):
     """
     Attributes:
-        data (CreateShipWaypointScanResponse201Data):
+        data (DockShipDockShip200ResponseData):
     """
 
-    data: "CreateShipWaypointScanResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_ship_waypoint_scan_response_201_data import (
-            CreateShipWaypointScanResponse201Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_ship_waypoint_scan_response_201_data import (
-            CreateShipWaypointScanResponse201Data,
-        )
-
-        d = src_dict.copy()
-        data = CreateShipWaypointScanResponse201Data.from_dict(d.pop("data"))
-
-        create_ship_waypoint_scan_response_201 = cls(
-            data=data,
-        )
+    data: "DockShipDockShip200ResponseData" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        create_ship_waypoint_scan_response_201.additional_properties = d
-        return create_ship_waypoint_scan_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,62 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.create_ship_system_scan_response_201_data import (
+    CreateShipSystemScanResponse201Data,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.create_survey_response_201_data import CreateSurveyResponse201Data
-
-
-T = TypeVar("T", bound="CreateSurveyResponse201")
+T = TypeVar("T", bound="CreateShipSystemScanResponse201")
 
 
-@attr.s(auto_attribs=True)
-class CreateSurveyResponse201:
+class CreateShipSystemScanResponse201(BaseModel):
     """
     Attributes:
-        data (CreateSurveyResponse201Data):
+        data (CreateShipSystemScanResponse201Data):
     """
 
-    data: "CreateSurveyResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_survey_response_201_data import CreateSurveyResponse201Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_survey_response_201_data import CreateSurveyResponse201Data
-
-        d = src_dict.copy()
-        data = CreateSurveyResponse201Data.from_dict(d.pop("data"))
-
-        create_survey_response_201 = cls(
-            data=data,
-        )
+    data: "CreateShipSystemScanResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        create_survey_response_201.additional_properties = d
-        return create_survey_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.2.0/spacetraders/models/register_response_201_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,71 +5,48 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.contract import Contract
+from ..models.faction import Faction
+from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="DeliverContractJsonBody")
+T = TypeVar("T", bound="RegisterResponse201Data")
 
 
-@attr.s(auto_attribs=True)
-class DeliverContractJsonBody:
+class RegisterResponse201Data(BaseModel):
     """
     Attributes:
-        ship_symbol (str):
-        trade_symbol (str):
-        units (int):
+        agent (Agent):
+        contract (Contract):
+        faction (Faction):
+        ship (Ship): A ship
+        token (str): A Bearer token for accessing secured API endpoints.
     """
 
-    ship_symbol: str
-    trade_symbol: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        ship_symbol = self.ship_symbol
-        trade_symbol = self.trade_symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "shipSymbol": ship_symbol,
-                "tradeSymbol": trade_symbol,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        ship_symbol = d.pop("shipSymbol")
-
-        trade_symbol = d.pop("tradeSymbol")
-
-        units = d.pop("units")
-
-        deliver_contract_json_body = cls(
-            ship_symbol=ship_symbol,
-            trade_symbol=trade_symbol,
-            units=units,
-        )
+    agent: "Agent" = Field(alias="agent")
+    contract: "Contract" = Field(alias="contract")
+    faction: "Faction" = Field(alias="faction")
+    ship: "Ship" = Field(alias="ship")
+    token: str = Field(alias="token")
+    additional_properties: Dict[str, Any] = {}
 
-        deliver_contract_json_body.additional_properties = d
-        return deliver_contract_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.2.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,68 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.fulfill_contract_response_200_data import FulfillContractResponse200Data
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.deliver_contract_response_200_data import (
-        DeliverContractResponse200Data,
-    )
+T = TypeVar("T", bound="FulfillContractResponse200")
 
 
-T = TypeVar("T", bound="DeliverContractResponse200")
-
-
-@attr.s(auto_attribs=True)
-class DeliverContractResponse200:
+class FulfillContractResponse200(BaseModel):
     """
     Attributes:
-        data (DeliverContractResponse200Data):
+        data (FulfillContractResponse200Data):
     """
 
-    data: "DeliverContractResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.deliver_contract_response_200_data import (
-            DeliverContractResponse200Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.deliver_contract_response_200_data import (
-            DeliverContractResponse200Data,
-        )
-
-        d = src_dict.copy()
-        data = DeliverContractResponse200Data.from_dict(d.pop("data"))
-
-        deliver_contract_response_200 = cls(
-            data=data,
-        )
+    data: "FulfillContractResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        deliver_contract_response_200.additional_properties = d
-        return deliver_contract_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,73 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.contract import Contract
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.contract import Contract
-    from ..models.ship_cargo import ShipCargo
-
-
 T = TypeVar("T", bound="DeliverContractResponse200Data")
 
 
-@attr.s(auto_attribs=True)
-class DeliverContractResponse200Data:
+class DeliverContractResponse200Data(BaseModel):
     """
     Attributes:
         contract (Contract):
         cargo (ShipCargo):
     """
 
-    contract: "Contract"
-    cargo: "ShipCargo"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.contract import Contract
-        from ..models.ship_cargo import ShipCargo
-
-        contract = self.contract.to_dict()
-
-        cargo = self.cargo.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "contract": contract,
-                "cargo": cargo,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.contract import Contract
-        from ..models.ship_cargo import ShipCargo
-
-        d = src_dict.copy()
-        contract = Contract.from_dict(d.pop("contract"))
-
-        cargo = ShipCargo.from_dict(d.pop("cargo"))
-
-        deliver_contract_response_200_data = cls(
-            contract=contract,
-            cargo=cargo,
-        )
+    contract: "Contract" = Field(alias="contract")
+    cargo: "ShipCargo" = Field(alias="cargo")
+    additional_properties: Dict[str, Any] = {}
 
-        deliver_contract_response_200_data.additional_properties = d
-        return deliver_contract_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,68 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_refine_ship_refine_200_response_data import (
+    ShipRefineShipRefine200ResponseData,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.dock_ship_dock_ship_200_response_data import (
-        DockShipDockShip200ResponseData,
-    )
-
+T = TypeVar("T", bound="ShipRefineShipRefine200Response")
 
-T = TypeVar("T", bound="DockShipDockShip200Response")
 
-
-@attr.s(auto_attribs=True)
-class DockShipDockShip200Response:
+class ShipRefineShipRefine200Response(BaseModel):
     """
     Attributes:
-        data (DockShipDockShip200ResponseData):
+        data (ShipRefineShipRefine200ResponseData):
     """
 
-    data: "DockShipDockShip200ResponseData"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.dock_ship_dock_ship_200_response_data import (
-            DockShipDockShip200ResponseData,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.dock_ship_dock_ship_200_response_data import (
-            DockShipDockShip200ResponseData,
-        )
-
-        d = src_dict.copy()
-        data = DockShipDockShip200ResponseData.from_dict(d.pop("data"))
-
-        dock_ship_dock_ship_200_response = cls(
-            data=data,
-        )
+    data: "ShipRefineShipRefine200ResponseData" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        dock_ship_dock_ship_200_response.additional_properties = d
-        return dock_ship_dock_ship_200_response
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.2.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav import ShipNav
-
-
 T = TypeVar("T", bound="DockShipDockShip200ResponseData")
 
 
-@attr.s(auto_attribs=True)
-class DockShipDockShip200ResponseData:
+class DockShipDockShip200ResponseData(BaseModel):
     """
     Attributes:
         nav (ShipNav): The navigation information of the ship.
     """
 
-    nav: "ShipNav"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav import ShipNav
-
-        nav = self.nav.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "nav": nav,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        nav = ShipNav.from_dict(d.pop("nav"))
-
-        dock_ship_dock_ship_200_response_data = cls(
-            nav=nav,
-        )
+    nav: "ShipNav" = Field(alias="nav")
+    additional_properties: Dict[str, Any] = {}
 
-        dock_ship_dock_ship_200_response_data.additional_properties = d
-        return dock_ship_dock_ship_200_response_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.2.0/spacetraders/models/extract_resources_json_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,68 +10,34 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.survey import Survey
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.survey import Survey
-
-
 T = TypeVar("T", bound="ExtractResourcesJsonBody")
 
 
-@attr.s(auto_attribs=True)
-class ExtractResourcesJsonBody:
+class ExtractResourcesJsonBody(BaseModel):
     """
     Attributes:
         survey (Union[Unset, Survey]): A resource survey of a waypoint, detailing a specific extraction location and the
             types of resources that can be found there.
     """
 
     survey: Union[Unset, "Survey"] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.survey import Survey
-
-        survey: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.survey, Unset):
-            survey = self.survey.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if survey is not UNSET:
-            field_dict["survey"] = survey
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.survey import Survey
-
-        d = src_dict.copy()
-        _survey = d.pop("survey", UNSET)
-        survey: Union[Unset, Survey]
-        if isinstance(_survey, Unset):
-            survey = UNSET
-        else:
-            survey = Survey.from_dict(_survey)
-
-        extract_resources_json_body = cls(
-            survey=survey,
-        )
+    additional_properties: Dict[str, Any] = {}
 
-        extract_resources_json_body.additional_properties = d
-        return extract_resources_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.2.0/spacetraders/models/jump_gate.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,72 +5,43 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.connected_system import ConnectedSystem
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.extract_resources_response_201_data import (
-        ExtractResourcesResponse201Data,
-    )
+T = TypeVar("T", bound="JumpGate")
 
 
-T = TypeVar("T", bound="ExtractResourcesResponse201")
-
-
-@attr.s(auto_attribs=True)
-class ExtractResourcesResponse201:
+class JumpGate(BaseModel):
     """
     Attributes:
-        data (ExtractResourcesResponse201Data):
+        jump_range (float): The maximum jump range of the gate.
+        connected_systems (List['ConnectedSystem']): The systems within range of the gate that have a corresponding
+            gate.
+        faction_symbol (Union[Unset, str]): The symbol of the faction that owns the gate.
     """
 
-    data: "ExtractResourcesResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.extract_resources_response_201_data import (
-            ExtractResourcesResponse201Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.extract_resources_response_201_data import (
-            ExtractResourcesResponse201Data,
-        )
-
-        d = src_dict.copy()
-        data = ExtractResourcesResponse201Data.from_dict(d.pop("data"))
-
-        extract_resources_response_201 = cls(
-            data=data,
-        )
+    jump_range: float = Field(alias="jumpRange")
+    connected_systems: List["ConnectedSystem"] = Field(alias="connectedSystems")
+    faction_symbol: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        extract_resources_response_201.additional_properties = d
-        return extract_resources_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/extraction.py` & `spacetraders-0.2.0/spacetraders/models/extraction.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,69 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.extraction_yield import ExtractionYield
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.extraction_yield import ExtractionYield
-
-
 T = TypeVar("T", bound="Extraction")
 
 
-@attr.s(auto_attribs=True)
-class Extraction:
+class Extraction(BaseModel):
     """
     Attributes:
         ship_symbol (str):
         yield_ (ExtractionYield):
     """
 
-    ship_symbol: str
-    yield_: "ExtractionYield"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.extraction_yield import ExtractionYield
-
-        ship_symbol = self.ship_symbol
-        yield_ = self.yield_.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "shipSymbol": ship_symbol,
-                "yield": yield_,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.extraction_yield import ExtractionYield
-
-        d = src_dict.copy()
-        ship_symbol = d.pop("shipSymbol")
-
-        yield_ = ExtractionYield.from_dict(d.pop("yield"))
-
-        extraction = cls(
-            ship_symbol=ship_symbol,
-            yield_=yield_,
-        )
+    ship_symbol: str = Field(alias="shipSymbol")
+    yield_: "ExtractionYield" = Field(alias="yield")
+    additional_properties: Dict[str, Any] = {}
 
-        extraction.additional_properties = d
-        return extraction
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/extraction_yield.py` & `spacetraders-0.2.0/spacetraders/models/get_contracts_response_200.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,64 +5,40 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.contract import Contract
+from ..models.meta import Meta
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ExtractionYield")
+T = TypeVar("T", bound="GetContractsResponse200")
 
 
-@attr.s(auto_attribs=True)
-class ExtractionYield:
+class GetContractsResponse200(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int): The number of units extracted that were placed into the ship's cargo hold.
+        data (List['Contract']):
+        meta (Meta):
     """
 
-    symbol: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        units = d.pop("units")
-
-        extraction_yield = cls(
-            symbol=symbol,
-            units=units,
-        )
+    data: List["Contract"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
+    additional_properties: Dict[str, Any] = {}
 
-        extraction_yield.additional_properties = d
-        return extraction_yield
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/faction_trait.py` & `spacetraders-0.2.0/spacetraders/models/faction_trait.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,70 +8,37 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.faction_trait_symbol import FactionTraitSymbol
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="FactionTrait")
 
 
-@attr.s(auto_attribs=True)
-class FactionTrait:
+class FactionTrait(BaseModel):
     """
     Attributes:
         symbol (FactionTraitSymbol): The unique identifier of the trait.
         name (str): The name of the trait.
         description (str): A description of the trait.
     """
 
-    symbol: FactionTraitSymbol
-    name: str
-    description: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol.value
-
-        name = self.name
-        description = self.description
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "name": name,
-                "description": description,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = FactionTraitSymbol(d.pop("symbol"))
-
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        faction_trait = cls(
-            symbol=symbol,
-            name=name,
-            description=description,
-        )
+    symbol: FactionTraitSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    additional_properties: Dict[str, Any] = {}
 
-        faction_trait.additional_properties = d
-        return faction_trait
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.2.0/spacetraders/models/faction_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,68 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.meta import Meta
+from ..models.waypoint import Waypoint
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.fulfill_contract_response_200_data import (
-        FulfillContractResponse200Data,
-    )
+T = TypeVar("T", bound="GetSystemWaypointsResponse200")
 
 
-T = TypeVar("T", bound="FulfillContractResponse200")
-
-
-@attr.s(auto_attribs=True)
-class FulfillContractResponse200:
+class GetSystemWaypointsResponse200(BaseModel):
     """
     Attributes:
-        data (FulfillContractResponse200Data):
+        data (List['Waypoint']):
+        meta (Meta):
     """
 
-    data: "FulfillContractResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.fulfill_contract_response_200_data import (
-            FulfillContractResponse200Data,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.fulfill_contract_response_200_data import (
-            FulfillContractResponse200Data,
-        )
-
-        d = src_dict.copy()
-        data = FulfillContractResponse200Data.from_dict(d.pop("data"))
-
-        fulfill_contract_response_200 = cls(
-            data=data,
-        )
+    data: List["Waypoint"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
+    additional_properties: Dict[str, Any] = {}
 
-        fulfill_contract_response_200.additional_properties = d
-        return fulfill_contract_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/accept_contract_response_200.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,73 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.accept_contract_response_200_data import AcceptContractResponse200Data
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.agent import Agent
-    from ..models.contract import Contract
+T = TypeVar("T", bound="AcceptContractResponse200")
 
 
-T = TypeVar("T", bound="FulfillContractResponse200Data")
-
-
-@attr.s(auto_attribs=True)
-class FulfillContractResponse200Data:
+class AcceptContractResponse200(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        contract (Contract):
+        data (AcceptContractResponse200Data):
     """
 
-    agent: "Agent"
-    contract: "Contract"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.agent import Agent
-        from ..models.contract import Contract
-
-        agent = self.agent.to_dict()
-
-        contract = self.contract.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "agent": agent,
-                "contract": contract,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.agent import Agent
-        from ..models.contract import Contract
-
-        d = src_dict.copy()
-        agent = Agent.from_dict(d.pop("agent"))
-
-        contract = Contract.from_dict(d.pop("contract"))
-
-        fulfill_contract_response_200_data = cls(
-            agent=agent,
-            contract=contract,
-        )
+    data: "AcceptContractResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        fulfill_contract_response_200_data.additional_properties = d
-        return fulfill_contract_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.2.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.contract import Contract
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.contract import Contract
+T = TypeVar("T", bound="AcceptContractResponse200Data")
 
 
-T = TypeVar("T", bound="GetContractResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetContractResponse200:
+class AcceptContractResponse200Data(BaseModel):
     """
     Attributes:
-        data (Contract):
+        agent (Agent):
+        contract (Contract):
     """
 
-    data: "Contract"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.contract import Contract
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.contract import Contract
-
-        d = src_dict.copy()
-        data = Contract.from_dict(d.pop("data"))
-
-        get_contract_response_200 = cls(
-            data=data,
-        )
+    agent: "Agent" = Field(alias="agent")
+    contract: "Contract" = Field(alias="contract")
+    additional_properties: Dict[str, Any] = {}
 
-        get_contract_response_200.additional_properties = d
-        return get_contract_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_factions_response_200.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,82 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.faction import Faction
+from ..models.meta import Meta
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.contract import Contract
-    from ..models.meta import Meta
+T = TypeVar("T", bound="GetFactionsResponse200")
 
 
-T = TypeVar("T", bound="GetContractsResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetContractsResponse200:
+class GetFactionsResponse200(BaseModel):
     """
     Attributes:
-        data (List['Contract']):
+        data (List['Faction']):
         meta (Meta):
     """
 
-    data: List["Contract"]
-    meta: "Meta"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.contract import Contract
-        from ..models.meta import Meta
-
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        meta = self.meta.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-                "meta": meta,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.contract import Contract
-        from ..models.meta import Meta
-
-        d = src_dict.copy()
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = Contract.from_dict(data_item_data)
-
-            data.append(data_item)
-
-        meta = Meta.from_dict(d.pop("meta"))
-
-        get_contracts_response_200 = cls(
-            data=data,
-            meta=meta,
-        )
+    data: List["Faction"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
+    additional_properties: Dict[str, Any] = {}
 
-        get_contracts_response_200.additional_properties = d
-        return get_contracts_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.meta import Meta
+from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.faction import Faction
+T = TypeVar("T", bound="GetMyShipsResponse200")
 
 
-T = TypeVar("T", bound="GetFactionResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetFactionResponse200:
+class GetMyShipsResponse200(BaseModel):
     """
     Attributes:
-        data (Faction):
+        data (List['Ship']):
+        meta (Meta):
     """
 
-    data: "Faction"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.faction import Faction
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.faction import Faction
-
-        d = src_dict.copy()
-        data = Faction.from_dict(d.pop("data"))
-
-        get_faction_response_200 = cls(
-            data=data,
-        )
+    data: List["Ship"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
+    additional_properties: Dict[str, Any] = {}
 
-        get_faction_response_200.additional_properties = d
-        return get_faction_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.2.0/spacetraders/models/register_json_body.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,86 +5,38 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.faction import Faction
-    from ..models.meta import Meta
+T = TypeVar("T", bound="RegisterJsonBody")
 
 
-T = TypeVar("T", bound="GetFactionsResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetFactionsResponse200:
+class RegisterJsonBody(BaseModel):
     """
     Attributes:
-        data (List['Faction']):
-        meta (Meta):
+        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
+        symbol (str): How other agents will see your ships and information. Example: BADGER.
     """
 
-    data: List["Faction"]
-    meta: "Meta"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.faction import Faction
-        from ..models.meta import Meta
-
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        meta = self.meta.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-                "meta": meta,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.faction import Faction
-        from ..models.meta import Meta
-
-        d = src_dict.copy()
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = Faction.from_dict(data_item_data)
-
-            data.append(data_item)
-
-        meta = Meta.from_dict(d.pop("meta"))
-
-        get_factions_response_200 = cls(
-            data=data,
-            meta=meta,
-        )
+    faction: RegisterJsonBodyFaction = Field(alias="faction")
+    symbol: str = Field(alias="symbol")
+    additional_properties: Dict[str, Any] = {}
 
-        get_factions_response_200.additional_properties = d
-        return get_factions_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.2.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.chart import Chart
+from ..models.waypoint import Waypoint
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.jump_gate import JumpGate
+T = TypeVar("T", bound="CreateChartResponse201Data")
 
 
-T = TypeVar("T", bound="GetJumpGateResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetJumpGateResponse200:
+class CreateChartResponse201Data(BaseModel):
     """
     Attributes:
-        data (JumpGate):
+        chart (Chart): The chart of a system or waypoint, which makes the location visible to other agents.
+        waypoint (Waypoint): A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
     """
 
-    data: "JumpGate"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.jump_gate import JumpGate
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.jump_gate import JumpGate
-
-        d = src_dict.copy()
-        data = JumpGate.from_dict(d.pop("data"))
-
-        get_jump_gate_response_200 = cls(
-            data=data,
-        )
+    chart: "Chart" = Field(alias="chart")
+    waypoint: "Waypoint" = Field(alias="waypoint")
+    additional_properties: Dict[str, Any] = {}
 
-        get_jump_gate_response_200.additional_properties = d
-        return get_jump_gate_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_market_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_systems_response_200.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.meta import Meta
+from ..models.system import System
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.market import Market
+T = TypeVar("T", bound="GetSystemsResponse200")
 
 
-T = TypeVar("T", bound="GetMarketResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetMarketResponse200:
+class GetSystemsResponse200(BaseModel):
     """
     Attributes:
-        data (Market):
+        data (List['System']):
+        meta (Meta):
     """
 
-    data: "Market"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.market import Market
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.market import Market
-
-        d = src_dict.copy()
-        data = Market.from_dict(d.pop("data"))
-
-        get_market_response_200 = cls(
-            data=data,
-        )
+    data: List["System"] = Field(alias="data")
+    meta: "Meta" = Field(alias="meta")
+    additional_properties: Dict[str, Any] = {}
 
-        get_market_response_200.additional_properties = d
-        return get_market_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.2.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.cooldown import Cooldown
+from ..models.survey import Survey
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.agent import Agent
+T = TypeVar("T", bound="CreateSurveyResponse201Data")
 
 
-T = TypeVar("T", bound="GetMyAgentResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetMyAgentResponse200:
+class CreateSurveyResponse201Data(BaseModel):
     """
     Attributes:
-        data (Agent):
+        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
+        surveys (List['Survey']):
     """
 
-    data: "Agent"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.agent import Agent
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.agent import Agent
-
-        d = src_dict.copy()
-        data = Agent.from_dict(d.pop("data"))
-
-        get_my_agent_response_200 = cls(
-            data=data,
-        )
+    cooldown: "Cooldown" = Field(alias="cooldown")
+    surveys: List["Survey"] = Field(alias="surveys")
+    additional_properties: Dict[str, Any] = {}
 
-        get_my_agent_response_200.additional_properties = d
-        return get_my_agent_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_cargo import ShipCargo
+T = TypeVar("T", bound="TransferCargoTransferCargo200ResponseData")
 
 
-T = TypeVar("T", bound="GetMyShipCargoResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetMyShipCargoResponse200:
+class TransferCargoTransferCargo200ResponseData(BaseModel):
     """
     Attributes:
-        data (ShipCargo):
+        cargo (ShipCargo):
     """
 
-    data: "ShipCargo"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_cargo import ShipCargo
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_cargo import ShipCargo
-
-        d = src_dict.copy()
-        data = ShipCargo.from_dict(d.pop("data"))
-
-        get_my_ship_cargo_response_200 = cls(
-            data=data,
-        )
+    cargo: "ShipCargo" = Field(alias="cargo")
+    additional_properties: Dict[str, Any] = {}
 
-        get_my_ship_cargo_response_200.additional_properties = d
-        return get_my_ship_cargo_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.2.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship import Ship
+T = TypeVar("T", bound="PatchShipNavResponse200")
 
 
-T = TypeVar("T", bound="GetMyShipResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetMyShipResponse200:
+class PatchShipNavResponse200(BaseModel):
     """
     Attributes:
-        data (Ship): A ship
+        data (ShipNav): The navigation information of the ship.
     """
 
-    data: "Ship"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship import Ship
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship import Ship
-
-        d = src_dict.copy()
-        data = Ship.from_dict(d.pop("data"))
-
-        get_my_ship_response_200 = cls(
-            data=data,
-        )
+    data: "ShipNav" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        get_my_ship_response_200.additional_properties = d
-        return get_my_ship_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.2.0/spacetraders/models/shipyard_transaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     List,
     Optional,
@@ -9,82 +10,41 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.meta import Meta
-    from ..models.ship import Ship
+T = TypeVar("T", bound="ShipyardTransaction")
 
 
-T = TypeVar("T", bound="GetMyShipsResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetMyShipsResponse200:
+class ShipyardTransaction(BaseModel):
     """
     Attributes:
-        data (List['Ship']):
-        meta (Meta):
+        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
+        ship_symbol (str): The symbol of the ship that was purchased.
+        price (int): The price of the transaction.
+        agent_symbol (str): The symbol of the agent that made the transaction.
+        timestamp (datetime.datetime): The timestamp of the transaction.
     """
 
-    data: List["Ship"]
-    meta: "Meta"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.meta import Meta
-        from ..models.ship import Ship
-
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        meta = self.meta.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-                "meta": meta,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.meta import Meta
-        from ..models.ship import Ship
-
-        d = src_dict.copy()
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = Ship.from_dict(data_item_data)
-
-            data.append(data_item)
-
-        meta = Meta.from_dict(d.pop("meta"))
-
-        get_my_ships_response_200 = cls(
-            data=data,
-            meta=meta,
-        )
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    ship_symbol: str = Field(alias="shipSymbol")
+    price: int = Field(alias="price")
+    agent_symbol: str = Field(alias="agentSymbol")
+    timestamp: datetime.datetime = Field(alias="timestamp")
+    additional_properties: Dict[str, Any] = {}
 
-        get_my_ships_response_200.additional_properties = d
-        return get_my_ships_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.cooldown import Cooldown
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cooldown import Cooldown
-
-
 T = TypeVar("T", bound="GetShipCooldownResponse200")
 
 
-@attr.s(auto_attribs=True)
-class GetShipCooldownResponse200:
+class GetShipCooldownResponse200(BaseModel):
     """
     Attributes:
         data (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
     """
 
-    data: "Cooldown"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.cooldown import Cooldown
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cooldown import Cooldown
-
-        d = src_dict.copy()
-        data = Cooldown.from_dict(d.pop("data"))
-
-        get_ship_cooldown_response_200 = cls(
-            data=data,
-        )
+    data: "Cooldown" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        get_ship_cooldown_response_200.additional_properties = d
-        return get_ship_cooldown_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav import ShipNav
-
-
 T = TypeVar("T", bound="GetShipNavResponse200")
 
 
-@attr.s(auto_attribs=True)
-class GetShipNavResponse200:
+class GetShipNavResponse200(BaseModel):
     """
     Attributes:
         data (ShipNav): The navigation information of the ship.
     """
 
-    data: "ShipNav"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav import ShipNav
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        data = ShipNav.from_dict(d.pop("data"))
-
-        get_ship_nav_response_200 = cls(
-            data=data,
-        )
+    data: "ShipNav" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        get_ship_nav_response_200.additional_properties = d
-        return get_ship_nav_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.2.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,62 +9,37 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_fuel import ShipFuel
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.shipyard import Shipyard
+T = TypeVar("T", bound="NavigateShipResponse200Data")
 
 
-T = TypeVar("T", bound="GetShipyardResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetShipyardResponse200:
+class NavigateShipResponse200Data(BaseModel):
     """
     Attributes:
-        data (Shipyard):
+        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
+            or action.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    data: "Shipyard"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.shipyard import Shipyard
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.shipyard import Shipyard
-
-        d = src_dict.copy()
-        data = Shipyard.from_dict(d.pop("data"))
-
-        get_shipyard_response_200 = cls(
-            data=data,
-        )
+    fuel: "ShipFuel" = Field(alias="fuel")
+    nav: "ShipNav" = Field(alias="nav")
+    additional_properties: Dict[str, Any] = {}
 
-        get_shipyard_response_200.additional_properties = d
-        return get_shipyard_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_system_response_200.py` & `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,66 +5,38 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
+    Union,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.system import System
+T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataConsumedItem")
 
 
-T = TypeVar("T", bound="GetSystemResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetSystemResponse200:
+class ShipRefineShipRefine200ResponseDataConsumedItem(BaseModel):
     """
     Attributes:
-        data (System):
+        trade_symbol (Union[Unset, str]):
+        units (Union[Unset, int]):
     """
 
-    data: "System"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.system import System
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.system import System
-
-        d = src_dict.copy()
-        data = System.from_dict(d.pop("data"))
-
-        get_system_response_200 = cls(
-            data=data,
-        )
+    trade_symbol: Union[Unset, str] = UNSET
+    units: Union[Unset, int] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        get_system_response_200.additional_properties = d
-        return get_system_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.2.0/spacetraders/models/connected_system.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,86 +5,49 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    cast,
+    Union,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.system_type import SystemType
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.meta import Meta
-    from ..models.waypoint import Waypoint
+T = TypeVar("T", bound="ConnectedSystem")
 
 
-T = TypeVar("T", bound="GetSystemWaypointsResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetSystemWaypointsResponse200:
+class ConnectedSystem(BaseModel):
     """
     Attributes:
-        data (List['Waypoint']):
-        meta (Meta):
+        symbol (str):
+        sector_symbol (str):
+        type (SystemType): The type of waypoint.
+        x (int):
+        y (int):
+        distance (int):
+        faction_symbol (Union[Unset, str]): The symbol of the faction that owns the connected jump gate in the system.
     """
 
-    data: List["Waypoint"]
-    meta: "Meta"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.meta import Meta
-        from ..models.waypoint import Waypoint
-
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        meta = self.meta.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-                "meta": meta,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.meta import Meta
-        from ..models.waypoint import Waypoint
-
-        d = src_dict.copy()
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = Waypoint.from_dict(data_item_data)
-
-            data.append(data_item)
-
-        meta = Meta.from_dict(d.pop("meta"))
-
-        get_system_waypoints_response_200 = cls(
-            data=data,
-            meta=meta,
-        )
+    symbol: str = Field(alias="symbol")
+    sector_symbol: str = Field(alias="sectorSymbol")
+    type: SystemType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    distance: int = Field(alias="distance")
+    faction_symbol: Union[Unset, str] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        get_system_waypoints_response_200.additional_properties = d
-        return get_system_waypoints_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.2.0/spacetraders/models/market_transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
     List,
     Optional,
@@ -9,82 +10,48 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
+from ..models.market_transaction_type import MarketTransactionType
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.meta import Meta
-    from ..models.system import System
+T = TypeVar("T", bound="MarketTransaction")
 
 
-T = TypeVar("T", bound="GetSystemsResponse200")
-
-
-@attr.s(auto_attribs=True)
-class GetSystemsResponse200:
+class MarketTransaction(BaseModel):
     """
     Attributes:
-        data (List['System']):
-        meta (Meta):
+        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
+        ship_symbol (str): The symbol of the ship that made the transaction.
+        trade_symbol (str): The symbol of the trade good.
+        type (MarketTransactionType): The type of transaction.
+        units (int): The number of units of the transaction.
+        price_per_unit (int): The price per unit of the transaction.
+        total_price (int): The total price of the transaction.
+        timestamp (datetime.datetime): The timestamp of the transaction.
     """
 
-    data: List["System"]
-    meta: "Meta"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.meta import Meta
-        from ..models.system import System
-
-        data = []
-        for data_item_data in self.data:
-            data_item = data_item_data.to_dict()
-
-            data.append(data_item)
-
-        meta = self.meta.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-                "meta": meta,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.meta import Meta
-        from ..models.system import System
-
-        d = src_dict.copy()
-        data = []
-        _data = d.pop("data")
-        for data_item_data in _data:
-            data_item = System.from_dict(data_item_data)
-
-            data.append(data_item)
-
-        meta = Meta.from_dict(d.pop("meta"))
-
-        get_systems_response_200 = cls(
-            data=data,
-            meta=meta,
-        )
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    ship_symbol: str = Field(alias="shipSymbol")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    type: MarketTransactionType = Field(alias="type")
+    units: int = Field(alias="units")
+    price_per_unit: int = Field(alias="pricePerUnit")
+    total_price: int = Field(alias="totalPrice")
+    timestamp: datetime.datetime = Field(alias="timestamp")
+    additional_properties: Dict[str, Any] = {}
 
-        get_systems_response_200.additional_properties = d
-        return get_systems_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.waypoint import Waypoint
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.waypoint import Waypoint
-
-
 T = TypeVar("T", bound="GetWaypointResponse200")
 
 
-@attr.s(auto_attribs=True)
-class GetWaypointResponse200:
+class GetWaypointResponse200(BaseModel):
     """
     Attributes:
         data (Waypoint): A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
     """
 
-    data: "Waypoint"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.waypoint import Waypoint
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.waypoint import Waypoint
-
-        d = src_dict.copy()
-        data = Waypoint.from_dict(d.pop("data"))
-
-        get_waypoint_response_200 = cls(
-            data=data,
-        )
+    data: "Waypoint" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        get_waypoint_response_200.additional_properties = d
-        return get_waypoint_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jettison_json_body.py` & `spacetraders-0.2.0/spacetraders/models/extraction_yield.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,61 +8,34 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JettisonJsonBody")
+T = TypeVar("T", bound="ExtractionYield")
 
 
-@attr.s(auto_attribs=True)
-class JettisonJsonBody:
+class ExtractionYield(BaseModel):
     """
     Attributes:
         symbol (str):
-        units (int):
+        units (int): The number of units extracted that were placed into the ship's cargo hold.
     """
 
-    symbol: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        units = d.pop("units")
-
-        jettison_json_body = cls(
-            symbol=symbol,
-            units=units,
-        )
+    symbol: str = Field(alias="symbol")
+    units: int = Field(alias="units")
+    additional_properties: Dict[str, Any] = {}
 
-        jettison_json_body.additional_properties = d
-        return jettison_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jettison_response_200.py` & `spacetraders-0.2.0/spacetraders/models/jettison_response_200.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.jettison_response_200_data import JettisonResponse200Data
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.jettison_response_200_data import JettisonResponse200Data
-
-
 T = TypeVar("T", bound="JettisonResponse200")
 
 
-@attr.s(auto_attribs=True)
-class JettisonResponse200:
+class JettisonResponse200(BaseModel):
     """
     Attributes:
         data (JettisonResponse200Data):
     """
 
-    data: "JettisonResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.jettison_response_200_data import JettisonResponse200Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.jettison_response_200_data import JettisonResponse200Data
-
-        d = src_dict.copy()
-        data = JettisonResponse200Data.from_dict(d.pop("data"))
-
-        jettison_response_200 = cls(
-            data=data,
-        )
+    data: "JettisonResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        jettison_response_200.additional_properties = d
-        return jettison_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/waypoint_trait.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,66 +5,40 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.waypoint_trait_symbol import WaypointTraitSymbol
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_cargo import ShipCargo
+T = TypeVar("T", bound="WaypointTrait")
 
 
-T = TypeVar("T", bound="JettisonResponse200Data")
-
-
-@attr.s(auto_attribs=True)
-class JettisonResponse200Data:
+class WaypointTrait(BaseModel):
     """
     Attributes:
-        cargo (ShipCargo):
+        symbol (WaypointTraitSymbol): The unique identifier of the trait.
+        name (str): The name of the trait.
+        description (str): A description of the trait.
     """
 
-    cargo: "ShipCargo"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_cargo import ShipCargo
-
-        cargo = self.cargo.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cargo": cargo,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_cargo import ShipCargo
-
-        d = src_dict.copy()
-        cargo = ShipCargo.from_dict(d.pop("cargo"))
-
-        jettison_response_200_data = cls(
-            cargo=cargo,
-        )
+    symbol: WaypointTraitSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    additional_properties: Dict[str, Any] = {}
 
-        jettison_response_200_data.additional_properties = d
-        return jettison_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.2.0/spacetraders/models/ship_engine.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,57 +5,51 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    Union,
+    cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_engine_symbol import ShipEngineSymbol
+from ..models.ship_requirements import ShipRequirements
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="JumpShipJsonBody")
+T = TypeVar("T", bound="ShipEngine")
 
 
-@attr.s(auto_attribs=True)
-class JumpShipJsonBody:
-    """
+class ShipEngine(BaseModel):
+    """The engine determines how quickly a ship travels between waypoints.
+
     Attributes:
-        system_symbol (str): The system symbol to jump to.
+        symbol (ShipEngineSymbol):
+        name (str):
+        description (str):
+        speed (float):
+        requirements (ShipRequirements): The requirements for installation on a ship
+        condition (Union[Unset, int]): Condition is a range of 0 to 100 where 0 is completely worn out and 100 is brand
+            new.
     """
 
-    system_symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        system_symbol = self.system_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "systemSymbol": system_symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        system_symbol = d.pop("systemSymbol")
-
-        jump_ship_json_body = cls(
-            system_symbol=system_symbol,
-        )
+    symbol: ShipEngineSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    speed: float = Field(alias="speed")
+    requirements: "ShipRequirements" = Field(alias="requirements")
+    condition: Union[Unset, int] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        jump_ship_json_body.additional_properties = d
-        return jump_ship_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.2.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,62 +9,37 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_fuel import ShipFuel
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.jump_ship_response_200_data import JumpShipResponse200Data
+T = TypeVar("T", bound="WarpShipResponse200Data")
 
 
-T = TypeVar("T", bound="JumpShipResponse200")
-
-
-@attr.s(auto_attribs=True)
-class JumpShipResponse200:
+class WarpShipResponse200Data(BaseModel):
     """
     Attributes:
-        data (JumpShipResponse200Data):
+        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
+            or action.
+        nav (ShipNav): The navigation information of the ship.
     """
 
-    data: "JumpShipResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.jump_ship_response_200_data import JumpShipResponse200Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.jump_ship_response_200_data import JumpShipResponse200Data
-
-        d = src_dict.copy()
-        data = JumpShipResponse200Data.from_dict(d.pop("data"))
-
-        jump_ship_response_200 = cls(
-            data=data,
-        )
+    fuel: "ShipFuel" = Field(alias="fuel")
+    nav: "ShipNav" = Field(alias="nav")
+    additional_properties: Dict[str, Any] = {}
 
-        jump_ship_response_200.additional_properties = d
-        return jump_ship_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,81 +10,36 @@
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.cooldown import Cooldown
+from ..models.ship_nav import ShipNav
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.cooldown import Cooldown
-    from ..models.ship_nav import ShipNav
-
-
 T = TypeVar("T", bound="JumpShipResponse200Data")
 
 
-@attr.s(auto_attribs=True)
-class JumpShipResponse200Data:
+class JumpShipResponse200Data(BaseModel):
     """
     Attributes:
         cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
         nav (Union[Unset, ShipNav]): The navigation information of the ship.
     """
 
-    cooldown: "Cooldown"
+    cooldown: "Cooldown" = Field(alias="cooldown")
     nav: Union[Unset, "ShipNav"] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.cooldown import Cooldown
-        from ..models.ship_nav import ShipNav
-
-        cooldown = self.cooldown.to_dict()
-
-        nav: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.nav, Unset):
-            nav = self.nav.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "cooldown": cooldown,
-            }
-        )
-        if nav is not UNSET:
-            field_dict["nav"] = nav
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.cooldown import Cooldown
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        cooldown = Cooldown.from_dict(d.pop("cooldown"))
-
-        _nav = d.pop("nav", UNSET)
-        nav: Union[Unset, ShipNav]
-        if isinstance(_nav, Unset):
-            nav = UNSET
-        else:
-            nav = ShipNav.from_dict(_nav)
-
-        jump_ship_response_200_data = cls(
-            cooldown=cooldown,
-            nav=nav,
-        )
+    additional_properties: Dict[str, Any] = {}
 
-        jump_ship_response_200_data.additional_properties = d
-        return jump_ship_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/market_trade_good.py` & `spacetraders-0.2.0/spacetraders/models/market_trade_good.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,85 +8,42 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.market_trade_good_supply import MarketTradeGoodSupply
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="MarketTradeGood")
 
 
-@attr.s(auto_attribs=True)
-class MarketTradeGood:
+class MarketTradeGood(BaseModel):
     """
     Attributes:
         symbol (str): The symbol of the trade good.
         trade_volume (int): The typical volume flowing through the market for this type of good. The larger the trade
             volume, the more stable prices will be.
         supply (MarketTradeGoodSupply): A rough estimate of the total supply of this good in the marketplace.
         purchase_price (int): The price at which this good can be purchased from the market.
         sell_price (int): The price at which this good can be sold to the market.
     """
 
-    symbol: str
-    trade_volume: int
-    supply: MarketTradeGoodSupply
-    purchase_price: int
-    sell_price: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        trade_volume = self.trade_volume
-        supply = self.supply.value
-
-        purchase_price = self.purchase_price
-        sell_price = self.sell_price
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "tradeVolume": trade_volume,
-                "supply": supply,
-                "purchasePrice": purchase_price,
-                "sellPrice": sell_price,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        trade_volume = d.pop("tradeVolume")
-
-        supply = MarketTradeGoodSupply(d.pop("supply"))
-
-        purchase_price = d.pop("purchasePrice")
-
-        sell_price = d.pop("sellPrice")
-
-        market_trade_good = cls(
-            symbol=symbol,
-            trade_volume=trade_volume,
-            supply=supply,
-            purchase_price=purchase_price,
-            sell_price=sell_price,
-        )
+    symbol: str = Field(alias="symbol")
+    trade_volume: int = Field(alias="tradeVolume")
+    supply: MarketTradeGoodSupply = Field(alias="supply")
+    purchase_price: int = Field(alias="purchasePrice")
+    sell_price: int = Field(alias="sellPrice")
+    additional_properties: Dict[str, Any] = {}
 
-        market_trade_good.additional_properties = d
-        return market_trade_good
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/market_transaction.py` & `spacetraders-0.2.0/spacetraders/models/waypoint.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,115 +1,64 @@
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
+    Union,
     cast,
 )
 
 import attr
-from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
-from ..models.market_transaction_type import MarketTransactionType
+from ..models.chart import Chart
+from ..models.waypoint_faction import WaypointFaction
+from ..models.waypoint_orbital import WaypointOrbital
+from ..models.waypoint_trait import WaypointTrait
+from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="MarketTransaction")
+T = TypeVar("T", bound="Waypoint")
 
 
-@attr.s(auto_attribs=True)
-class MarketTransaction:
-    """
+class Waypoint(BaseModel):
+    """A waypoint is a location that ships can travel to such as a Planet, Moon or Space Station.
+
     Attributes:
-        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
-        ship_symbol (str): The symbol of the ship that made the transaction.
-        trade_symbol (str): The symbol of the trade good.
-        type (MarketTransactionType): The type of transaction.
-        units (int): The number of units of the transaction.
-        price_per_unit (int): The price per unit of the transaction.
-        total_price (int): The total price of the transaction.
-        timestamp (datetime.datetime): The timestamp of the transaction.
+        symbol (str):
+        type (WaypointType): The type of waypoint.
+        system_symbol (str):
+        x (int):
+        y (int):
+        orbitals (List['WaypointOrbital']):
+        traits (List['WaypointTrait']): The traits of the waypoint.
+        faction (Union[Unset, WaypointFaction]):
+        chart (Union[Unset, Chart]): The chart of a system or waypoint, which makes the location visible to other
+            agents.
     """
 
-    waypoint_symbol: str
-    ship_symbol: str
-    trade_symbol: str
-    type: MarketTransactionType
-    units: int
-    price_per_unit: int
-    total_price: int
-    timestamp: datetime.datetime
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        waypoint_symbol = self.waypoint_symbol
-        ship_symbol = self.ship_symbol
-        trade_symbol = self.trade_symbol
-        type = self.type.value
-
-        units = self.units
-        price_per_unit = self.price_per_unit
-        total_price = self.total_price
-        timestamp = self.timestamp.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "waypointSymbol": waypoint_symbol,
-                "shipSymbol": ship_symbol,
-                "tradeSymbol": trade_symbol,
-                "type": type,
-                "units": units,
-                "pricePerUnit": price_per_unit,
-                "totalPrice": total_price,
-                "timestamp": timestamp,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        waypoint_symbol = d.pop("waypointSymbol")
-
-        ship_symbol = d.pop("shipSymbol")
-
-        trade_symbol = d.pop("tradeSymbol")
-
-        type = MarketTransactionType(d.pop("type"))
-
-        units = d.pop("units")
-
-        price_per_unit = d.pop("pricePerUnit")
-
-        total_price = d.pop("totalPrice")
-
-        timestamp = isoparse(d.pop("timestamp"))
-
-        market_transaction = cls(
-            waypoint_symbol=waypoint_symbol,
-            ship_symbol=ship_symbol,
-            trade_symbol=trade_symbol,
-            type=type,
-            units=units,
-            price_per_unit=price_per_unit,
-            total_price=total_price,
-            timestamp=timestamp,
-        )
+    symbol: str = Field(alias="symbol")
+    type: WaypointType = Field(alias="type")
+    system_symbol: str = Field(alias="systemSymbol")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    orbitals: List["WaypointOrbital"] = Field(alias="orbitals")
+    traits: List["WaypointTrait"] = Field(alias="traits")
+    faction: Union[Unset, "WaypointFaction"] = UNSET
+    chart: Union[Unset, "Chart"] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        market_transaction.additional_properties = d
-        return market_transaction
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/meta.py` & `spacetraders-0.2.0/spacetraders/models/create_survey_response_201.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,71 +5,37 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.create_survey_response_201_data import CreateSurveyResponse201Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="Meta")
+T = TypeVar("T", bound="CreateSurveyResponse201")
 
 
-@attr.s(auto_attribs=True)
-class Meta:
+class CreateSurveyResponse201(BaseModel):
     """
     Attributes:
-        total (int):
-        page (int):
-        limit (int):
+        data (CreateSurveyResponse201Data):
     """
 
-    total: int
-    page: int
-    limit: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        total = self.total
-        page = self.page
-        limit = self.limit
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "total": total,
-                "page": page,
-                "limit": limit,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        total = d.pop("total")
-
-        page = d.pop("page")
-
-        limit = d.pop("limit")
-
-        meta = cls(
-            total=total,
-            page=page,
-            limit=limit,
-        )
+    data: "CreateSurveyResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        meta.additional_properties = d
-        return meta
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.2.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,54 +8,35 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_type import ShipType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="NavigateShipJsonBody")
+T = TypeVar("T", bound="PurchaseShipJsonBody")
 
 
-@attr.s(auto_attribs=True)
-class NavigateShipJsonBody:
+class PurchaseShipJsonBody(BaseModel):
     """
     Attributes:
-        waypoint_symbol (str): The target destination.
+        ship_type (ShipType):
+        waypoint_symbol (str): The symbol of the waypoint you want to purchase the ship at.
     """
 
-    waypoint_symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    ship_type: ShipType = Field(alias="shipType")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        waypoint_symbol = self.waypoint_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "waypointSymbol": waypoint_symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        waypoint_symbol = d.pop("waypointSymbol")
-
-        navigate_ship_json_body = cls(
-            waypoint_symbol=waypoint_symbol,
-        )
-
-        navigate_ship_json_body.additional_properties = d
-        return navigate_ship_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.2.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,62 +9,50 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.cooldown import Cooldown
+from ..models.ship_cargo import ShipCargo
+from ..models.ship_refine_ship_refine_200_response_data_consumed_item import (
+    ShipRefineShipRefine200ResponseDataConsumedItem,
+)
+from ..models.ship_refine_ship_refine_200_response_data_produced_item import (
+    ShipRefineShipRefine200ResponseDataProducedItem,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.navigate_ship_response_200_data import NavigateShipResponse200Data
-
+T = TypeVar("T", bound="ShipRefineShipRefine200ResponseData")
 
-T = TypeVar("T", bound="NavigateShipResponse200")
 
-
-@attr.s(auto_attribs=True)
-class NavigateShipResponse200:
+class ShipRefineShipRefine200ResponseData(BaseModel):
     """
     Attributes:
-        data (NavigateShipResponse200Data):
+        cargo (ShipCargo):
+        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
+        produced (List['ShipRefineShipRefine200ResponseDataProducedItem']):
+        consumed (List['ShipRefineShipRefine200ResponseDataConsumedItem']):
     """
 
-    data: "NavigateShipResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.navigate_ship_response_200_data import NavigateShipResponse200Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.navigate_ship_response_200_data import NavigateShipResponse200Data
-
-        d = src_dict.copy()
-        data = NavigateShipResponse200Data.from_dict(d.pop("data"))
-
-        navigate_ship_response_200 = cls(
-            data=data,
-        )
+    cargo: "ShipCargo" = Field(alias="cargo")
+    cooldown: "Cooldown" = Field(alias="cooldown")
+    produced: List["ShipRefineShipRefine200ResponseDataProducedItem"] = Field(
+        alias="produced"
+    )
+    consumed: List["ShipRefineShipRefine200ResponseDataConsumedItem"] = Field(
+        alias="consumed"
+    )
+    additional_properties: Dict[str, Any] = {}
 
-        navigate_ship_response_200.additional_properties = d
-        return navigate_ship_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/contract_payment.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,78 +5,37 @@
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
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_fuel import ShipFuel
-    from ..models.ship_nav import ShipNav
+T = TypeVar("T", bound="ContractPayment")
 
 
-T = TypeVar("T", bound="NavigateShipResponse200Data")
-
-
-@attr.s(auto_attribs=True)
-class NavigateShipResponse200Data:
+class ContractPayment(BaseModel):
     """
     Attributes:
-        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
-            or action.
-        nav (ShipNav): The navigation information of the ship.
+        on_accepted (int): The amount of credits received up front for accepting the contract.
+        on_fulfilled (int): The amount of credits received when the contract is fulfilled.
     """
 
-    fuel: "ShipFuel"
-    nav: "ShipNav"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_fuel import ShipFuel
-        from ..models.ship_nav import ShipNav
-
-        fuel = self.fuel.to_dict()
-
-        nav = self.nav.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "fuel": fuel,
-                "nav": nav,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_fuel import ShipFuel
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        fuel = ShipFuel.from_dict(d.pop("fuel"))
-
-        nav = ShipNav.from_dict(d.pop("nav"))
-
-        navigate_ship_response_200_data = cls(
-            fuel=fuel,
-            nav=nav,
-        )
+    on_accepted: int = Field(alias="onAccepted")
+    on_fulfilled: int = Field(alias="onFulfilled")
+    additional_properties: Dict[str, Any] = {}
 
-        navigate_ship_response_200_data.additional_properties = d
-        return navigate_ship_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.2.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,68 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.orbit_ship_orbit_ship_200_response_data import (
+    OrbitShipOrbitShip200ResponseData,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.orbit_ship_orbit_ship_200_response_data import (
-        OrbitShipOrbitShip200ResponseData,
-    )
-
-
 T = TypeVar("T", bound="OrbitShipOrbitShip200Response")
 
 
-@attr.s(auto_attribs=True)
-class OrbitShipOrbitShip200Response:
+class OrbitShipOrbitShip200Response(BaseModel):
     """
     Attributes:
         data (OrbitShipOrbitShip200ResponseData):
     """
 
-    data: "OrbitShipOrbitShip200ResponseData"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.orbit_ship_orbit_ship_200_response_data import (
-            OrbitShipOrbitShip200ResponseData,
-        )
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.orbit_ship_orbit_ship_200_response_data import (
-            OrbitShipOrbitShip200ResponseData,
-        )
-
-        d = src_dict.copy()
-        data = OrbitShipOrbitShip200ResponseData.from_dict(d.pop("data"))
-
-        orbit_ship_orbit_ship_200_response = cls(
-            data=data,
-        )
+    data: "OrbitShipOrbitShip200ResponseData" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        orbit_ship_orbit_ship_200_response.additional_properties = d
-        return orbit_ship_orbit_ship_200_response
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,62 +9,37 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.ship_fuel import ShipFuel
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav import ShipNav
+T = TypeVar("T", bound="RefuelShipResponse200Data")
 
 
-T = TypeVar("T", bound="OrbitShipOrbitShip200ResponseData")
-
-
-@attr.s(auto_attribs=True)
-class OrbitShipOrbitShip200ResponseData:
+class RefuelShipResponse200Data(BaseModel):
     """
     Attributes:
-        nav (ShipNav): The navigation information of the ship.
+        agent (Agent):
+        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
+            or action.
     """
 
-    nav: "ShipNav"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav import ShipNav
-
-        nav = self.nav.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "nav": nav,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        nav = ShipNav.from_dict(d.pop("nav"))
-
-        orbit_ship_orbit_ship_200_response_data = cls(
-            nav=nav,
-        )
+    agent: "Agent" = Field(alias="agent")
+    fuel: "ShipFuel" = Field(alias="fuel")
+    additional_properties: Dict[str, Any] = {}
 
-        orbit_ship_orbit_ship_200_response_data.additional_properties = d
-        return orbit_ship_orbit_ship_200_response_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.2.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,61 +9,34 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.ship_nav_flight_mode import ShipNavFlightMode
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="PatchShipNavJsonBody")
 
 
-@attr.s(auto_attribs=True)
-class PatchShipNavJsonBody:
+class PatchShipNavJsonBody(BaseModel):
     """
     Attributes:
         flight_mode (Union[Unset, ShipNavFlightMode]): The ship's set speed when traveling between waypoints or systems.
             Default: ShipNavFlightMode.CRUISE.
     """
 
     flight_mode: Union[Unset, ShipNavFlightMode] = ShipNavFlightMode.CRUISE
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        flight_mode: Union[Unset, str] = UNSET
-        if not isinstance(self.flight_mode, Unset):
-            flight_mode = self.flight_mode.value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if flight_mode is not UNSET:
-            field_dict["flightMode"] = flight_mode
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _flight_mode = d.pop("flightMode", UNSET)
-        flight_mode: Union[Unset, ShipNavFlightMode]
-        if isinstance(_flight_mode, Unset):
-            flight_mode = UNSET
-        else:
-            flight_mode = ShipNavFlightMode(_flight_mode)
-
-        patch_ship_nav_json_body = cls(
-            flight_mode=flight_mode,
-        )
-
-        patch_ship_nav_json_body.additional_properties = d
-        return patch_ship_nav_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.2.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,62 +9,36 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.cooldown import Cooldown
+from ..models.scanned_waypoint import ScannedWaypoint
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav import ShipNav
+T = TypeVar("T", bound="CreateShipWaypointScanResponse201Data")
 
 
-T = TypeVar("T", bound="PatchShipNavResponse200")
-
-
-@attr.s(auto_attribs=True)
-class PatchShipNavResponse200:
+class CreateShipWaypointScanResponse201Data(BaseModel):
     """
     Attributes:
-        data (ShipNav): The navigation information of the ship.
+        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
+        waypoints (List['ScannedWaypoint']):
     """
 
-    data: "ShipNav"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav import ShipNav
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav import ShipNav
-
-        d = src_dict.copy()
-        data = ShipNav.from_dict(d.pop("data"))
-
-        patch_ship_nav_response_200 = cls(
-            data=data,
-        )
+    cooldown: "Cooldown" = Field(alias="cooldown")
+    waypoints: List["ScannedWaypoint"] = Field(alias="waypoints")
+    additional_properties: Dict[str, Any] = {}
 
-        patch_ship_nav_response_200.additional_properties = d
-        return patch_ship_nav_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.2.0/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,61 +8,42 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="PurchaseCargoPurchaseCargoRequest")
+T = TypeVar("T", bound="ShipNavRouteWaypoint")
 
 
-@attr.s(auto_attribs=True)
-class PurchaseCargoPurchaseCargoRequest:
-    """
+class ShipNavRouteWaypoint(BaseModel):
+    """The destination or departure of a ships nav route.
+
     Attributes:
         symbol (str):
-        units (int):
+        type (WaypointType): The type of waypoint.
+        system_symbol (str):
+        x (int):
+        y (int):
     """
 
-    symbol: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        units = d.pop("units")
-
-        purchase_cargo_purchase_cargo_request = cls(
-            symbol=symbol,
-            units=units,
-        )
+    symbol: str = Field(alias="symbol")
+    type: WaypointType = Field(alias="type")
+    system_symbol: str = Field(alias="systemSymbol")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    additional_properties: Dict[str, Any] = {}
 
-        purchase_cargo_purchase_cargo_request.additional_properties = d
-        return purchase_cargo_purchase_cargo_request
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,62 +9,35 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.purchase_cargo_purchase_cargo_201_response_data import (
+    PurchaseCargoPurchaseCargo201ResponseData,
+)
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.purchase_ship_response_201_data import PurchaseShipResponse201Data
-
-
-T = TypeVar("T", bound="PurchaseShipResponse201")
+T = TypeVar("T", bound="PurchaseCargoPurchaseCargo201Response")
 
 
-@attr.s(auto_attribs=True)
-class PurchaseShipResponse201:
+class PurchaseCargoPurchaseCargo201Response(BaseModel):
     """
     Attributes:
-        data (PurchaseShipResponse201Data):
+        data (PurchaseCargoPurchaseCargo201ResponseData):
     """
 
-    data: "PurchaseShipResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.purchase_ship_response_201_data import PurchaseShipResponse201Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.purchase_ship_response_201_data import PurchaseShipResponse201Data
-
-        d = src_dict.copy()
-        data = PurchaseShipResponse201Data.from_dict(d.pop("data"))
-
-        purchase_ship_response_201 = cls(
-            data=data,
-        )
+    data: "PurchaseCargoPurchaseCargo201ResponseData" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        purchase_ship_response_201.additional_properties = d
-        return purchase_ship_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,84 +9,39 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.market_transaction import MarketTransaction
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.agent import Agent
-    from ..models.ship import Ship
-    from ..models.shipyard_transaction import ShipyardTransaction
+T = TypeVar("T", bound="SellCargoSellCargo201ResponseData")
 
 
-T = TypeVar("T", bound="PurchaseShipResponse201Data")
-
-
-@attr.s(auto_attribs=True)
-class PurchaseShipResponse201Data:
+class SellCargoSellCargo201ResponseData(BaseModel):
     """
     Attributes:
         agent (Agent):
-        ship (Ship): A ship
-        transaction (ShipyardTransaction):
+        cargo (ShipCargo):
+        transaction (MarketTransaction):
     """
 
-    agent: "Agent"
-    ship: "Ship"
-    transaction: "ShipyardTransaction"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.agent import Agent
-        from ..models.ship import Ship
-        from ..models.shipyard_transaction import ShipyardTransaction
-
-        agent = self.agent.to_dict()
-
-        ship = self.ship.to_dict()
-
-        transaction = self.transaction.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "agent": agent,
-                "ship": ship,
-                "transaction": transaction,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.agent import Agent
-        from ..models.ship import Ship
-        from ..models.shipyard_transaction import ShipyardTransaction
-
-        d = src_dict.copy()
-        agent = Agent.from_dict(d.pop("agent"))
-
-        ship = Ship.from_dict(d.pop("ship"))
-
-        transaction = ShipyardTransaction.from_dict(d.pop("transaction"))
-
-        purchase_ship_response_201_data = cls(
-            agent=agent,
-            ship=ship,
-            transaction=transaction,
-        )
+    agent: "Agent" = Field(alias="agent")
+    cargo: "ShipCargo" = Field(alias="cargo")
+    transaction: "MarketTransaction" = Field(alias="transaction")
+    additional_properties: Dict[str, Any] = {}
 
-        purchase_ship_response_201_data.additional_properties = d
-        return purchase_ship_response_201_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.2.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
+T = TypeVar("T", bound="GetMyShipCargoResponse200")
 
 
-T = TypeVar("T", bound="RefuelShipResponse200")
-
-
-@attr.s(auto_attribs=True)
-class RefuelShipResponse200:
+class GetMyShipCargoResponse200(BaseModel):
     """
     Attributes:
-        data (RefuelShipResponse200Data):
+        data (ShipCargo):
     """
 
-    data: "RefuelShipResponse200Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
-
-        d = src_dict.copy()
-        data = RefuelShipResponse200Data.from_dict(d.pop("data"))
-
-        refuel_ship_response_200 = cls(
-            data=data,
-        )
+    data: "ShipCargo" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        refuel_ship_response_200.additional_properties = d
-        return refuel_ship_response_200
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.2.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,74 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.refuel_ship_response_200_data import RefuelShipResponse200Data
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.agent import Agent
-    from ..models.ship_fuel import ShipFuel
+T = TypeVar("T", bound="RefuelShipResponse200")
 
 
-T = TypeVar("T", bound="RefuelShipResponse200Data")
-
-
-@attr.s(auto_attribs=True)
-class RefuelShipResponse200Data:
+class RefuelShipResponse200(BaseModel):
     """
     Attributes:
-        agent (Agent):
-        fuel (ShipFuel): Details of the ship's fuel tanks including how much fuel was consumed during the last transit
-            or action.
+        data (RefuelShipResponse200Data):
     """
 
-    agent: "Agent"
-    fuel: "ShipFuel"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.agent import Agent
-        from ..models.ship_fuel import ShipFuel
-
-        agent = self.agent.to_dict()
-
-        fuel = self.fuel.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "agent": agent,
-                "fuel": fuel,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.agent import Agent
-        from ..models.ship_fuel import ShipFuel
-
-        d = src_dict.copy()
-        agent = Agent.from_dict(d.pop("agent"))
-
-        fuel = ShipFuel.from_dict(d.pop("fuel"))
-
-        refuel_ship_response_200_data = cls(
-            agent=agent,
-            fuel=fuel,
-        )
+    data: "RefuelShipResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        refuel_ship_response_200_data.additional_properties = d
-        return refuel_ship_response_200_data
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/register_json_body.py` & `spacetraders-0.2.0/spacetraders/models/contract_deliver_good.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,63 +8,39 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
-from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="RegisterJsonBody")
+T = TypeVar("T", bound="ContractDeliverGood")
 
 
-@attr.s(auto_attribs=True)
-class RegisterJsonBody:
-    """
+class ContractDeliverGood(BaseModel):
+    """The details of a delivery contract. Includes the type of good, units needed, and the destination.
+
     Attributes:
-        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
-        symbol (str): How other agents will see your ships and information. Example: BADGER.
+        trade_symbol (str): The symbol of the trade good to deliver.
+        destination_symbol (str): The destination where goods need to be delivered.
+        units_required (int): The number of units that need to be delivered on this contract.
+        units_fulfilled (int): The number of units fulfilled on this contract.
     """
 
-    faction: RegisterJsonBodyFaction
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        faction = self.faction.value
-
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "faction": faction,
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        faction = RegisterJsonBodyFaction(d.pop("faction"))
-
-        symbol = d.pop("symbol")
-
-        register_json_body = cls(
-            faction=faction,
-            symbol=symbol,
-        )
+    trade_symbol: str = Field(alias="tradeSymbol")
+    destination_symbol: str = Field(alias="destinationSymbol")
+    units_required: int = Field(alias="unitsRequired")
+    units_fulfilled: int = Field(alias="unitsFulfilled")
+    additional_properties: Dict[str, Any] = {}
 
-        register_json_body.additional_properties = d
-        return register_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/register_response_201.py` & `spacetraders-0.2.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,62 +9,33 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship import Ship
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.register_response_201_data import RegisterResponse201Data
+T = TypeVar("T", bound="GetMyShipResponse200")
 
 
-T = TypeVar("T", bound="RegisterResponse201")
-
-
-@attr.s(auto_attribs=True)
-class RegisterResponse201:
+class GetMyShipResponse200(BaseModel):
     """
     Attributes:
-        data (RegisterResponse201Data):
+        data (Ship): A ship
     """
 
-    data: "RegisterResponse201Data"
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.register_response_201_data import RegisterResponse201Data
-
-        data = self.data.to_dict()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "data": data,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.register_response_201_data import RegisterResponse201Data
-
-        d = src_dict.copy()
-        data = RegisterResponse201Data.from_dict(d.pop("data"))
-
-        register_response_201 = cls(
-            data=data,
-        )
+    data: "Ship" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        register_response_201.additional_properties = d
-        return register_response_201
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.2.0/spacetraders/models/system_waypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,55 +8,39 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.waypoint_type import WaypointType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedShipEngine")
+T = TypeVar("T", bound="SystemWaypoint")
 
 
-@attr.s(auto_attribs=True)
-class ScannedShipEngine:
-    """The engine of the ship.
-
+class SystemWaypoint(BaseModel):
+    """
     Attributes:
         symbol (str):
+        type (WaypointType): The type of waypoint.
+        x (int):
+        y (int):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        scanned_ship_engine = cls(
-            symbol=symbol,
-        )
+    symbol: str = Field(alias="symbol")
+    type: WaypointType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    additional_properties: Dict[str, Any] = {}
 
-        scanned_ship_engine.additional_properties = d
-        return scanned_ship_engine
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.2.0/spacetraders/models/scanned_system.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,55 +8,43 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.system_type import SystemType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedShipFrame")
+T = TypeVar("T", bound="ScannedSystem")
 
 
-@attr.s(auto_attribs=True)
-class ScannedShipFrame:
-    """The frame of the ship.
-
+class ScannedSystem(BaseModel):
+    """
     Attributes:
         symbol (str):
+        sector_symbol (str):
+        type (SystemType): The type of waypoint.
+        x (int):
+        y (int):
+        distance (int):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        scanned_ship_frame = cls(
-            symbol=symbol,
-        )
+    symbol: str = Field(alias="symbol")
+    sector_symbol: str = Field(alias="sectorSymbol")
+    type: SystemType = Field(alias="type")
+    x: int = Field(alias="x")
+    y: int = Field(alias="y")
+    distance: int = Field(alias="distance")
+    additional_properties: Dict[str, Any] = {}
 
-        scanned_ship_frame.additional_properties = d
-        return scanned_ship_frame
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.2.0/spacetraders/models/trade_good.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,55 +8,37 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.trade_symbol import TradeSymbol
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedShipMountsItem")
+T = TypeVar("T", bound="TradeGood")
 
 
-@attr.s(auto_attribs=True)
-class ScannedShipMountsItem:
-    """A mount on the ship.
-
+class TradeGood(BaseModel):
+    """
     Attributes:
-        symbol (str):
+        symbol (TradeSymbol):
+        name (str):
+        description (str):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        scanned_ship_mounts_item = cls(
-            symbol=symbol,
-        )
+    symbol: TradeSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    additional_properties: Dict[str, Any] = {}
 
-        scanned_ship_mounts_item.additional_properties = d
-        return scanned_ship_mounts_item
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.2.0/spacetraders/models/ship_cargo_item.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,55 +8,39 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ScannedShipReactor")
+T = TypeVar("T", bound="ShipCargoItem")
 
 
-@attr.s(auto_attribs=True)
-class ScannedShipReactor:
-    """The reactor of the ship.
+class ShipCargoItem(BaseModel):
+    """The type of cargo item and the number of units.
 
     Attributes:
-        symbol (str):
+        symbol (str): The unique identifier of the cargo item type.
+        name (str): The name of the cargo item type.
+        description (str): The description of the cargo item type.
+        units (int): The number of units of the cargo item.
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    symbol: str = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    units: int = Field(alias="units")
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        scanned_ship_reactor = cls(
-            symbol=symbol,
-        )
-
-        scanned_ship_reactor.additional_properties = d
-        return scanned_ship_reactor
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.2.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,64 +5,43 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.agent import Agent
+from ..models.market_transaction import MarketTransaction
+from ..models.ship_cargo import ShipCargo
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SellCargoSellCargoRequest")
+T = TypeVar("T", bound="PurchaseCargoPurchaseCargo201ResponseData")
 
 
-@attr.s(auto_attribs=True)
-class SellCargoSellCargoRequest:
+class PurchaseCargoPurchaseCargo201ResponseData(BaseModel):
     """
     Attributes:
-        symbol (str):
-        units (int):
+        agent (Agent):
+        cargo (ShipCargo):
+        transaction (MarketTransaction):
     """
 
-    symbol: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        units = d.pop("units")
-
-        sell_cargo_sell_cargo_request = cls(
-            symbol=symbol,
-            units=units,
-        )
+    agent: "Agent" = Field(alias="agent")
+    cargo: "ShipCargo" = Field(alias="cargo")
+    transaction: "MarketTransaction" = Field(alias="transaction")
+    additional_properties: Dict[str, Any] = {}
 
-        sell_cargo_sell_cargo_request.additional_properties = d
-        return sell_cargo_sell_cargo_request
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.2.0/spacetraders/models/ship_fuel.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,79 +5,43 @@
     Dict,
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
+    Union,
+    cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.ship_fuel_consumed import ShipFuelConsumed
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipCargoItem")
+T = TypeVar("T", bound="ShipFuel")
 
 
-@attr.s(auto_attribs=True)
-class ShipCargoItem:
-    """The type of cargo item and the number of units.
+class ShipFuel(BaseModel):
+    """Details of the ship's fuel tanks including how much fuel was consumed during the last transit or action.
 
     Attributes:
-        symbol (str): The unique identifier of the cargo item type.
-        name (str): The name of the cargo item type.
-        description (str): The description of the cargo item type.
-        units (int): The number of units of the cargo item.
+        current (int): The current amount of fuel in the ship's tanks.
+        capacity (int): The maximum amount of fuel the ship's tanks can hold.
+        consumed (Union[Unset, ShipFuelConsumed]):
     """
 
-    symbol: str
-    name: str
-    description: str
-    units: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        name = self.name
-        description = self.description
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "name": name,
-                "description": description,
-                "units": units,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        units = d.pop("units")
-
-        ship_cargo_item = cls(
-            symbol=symbol,
-            name=name,
-            description=description,
-            units=units,
-        )
+    current: int = Field(alias="current")
+    capacity: int = Field(alias="capacity")
+    consumed: Union[Unset, "ShipFuelConsumed"] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        ship_cargo_item.additional_properties = d
-        return ship_cargo_item
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.2.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.2.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,61 +11,34 @@
     Type,
     TypeVar,
     cast,
 )
 
 import attr
 from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ShipFuelConsumed")
 
 
-@attr.s(auto_attribs=True)
-class ShipFuelConsumed:
+class ShipFuelConsumed(BaseModel):
     """
     Attributes:
         amount (int): The amount of fuel consumed by the most recent transit or action.
         timestamp (datetime.datetime): The time at which the fuel was consumed.
     """
 
-    amount: int
-    timestamp: datetime.datetime
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        amount = self.amount
-        timestamp = self.timestamp.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "amount": amount,
-                "timestamp": timestamp,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        amount = d.pop("amount")
-
-        timestamp = isoparse(d.pop("timestamp"))
-
-        ship_fuel_consumed = cls(
-            amount=amount,
-            timestamp=timestamp,
-        )
+    amount: int = Field(alias="amount")
+    timestamp: datetime.datetime = Field(alias="timestamp")
+    additional_properties: Dict[str, Any] = {}
 
-        ship_fuel_consumed.additional_properties = d
-        return ship_fuel_consumed
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.2.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.2.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.2.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_nav.py` & `spacetraders-0.2.0/spacetraders/models/ship_nav.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,97 +9,46 @@
     Tuple,
     Type,
     TypeVar,
     cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.ship_nav_flight_mode import ShipNavFlightMode
+from ..models.ship_nav_route import ShipNavRoute
 from ..models.ship_nav_status import ShipNavStatus
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav_route import ShipNavRoute
-
-
 T = TypeVar("T", bound="ShipNav")
 
 
-@attr.s(auto_attribs=True)
-class ShipNav:
+class ShipNav(BaseModel):
     """The navigation information of the ship.
 
     Attributes:
         system_symbol (str): The system symbol of the ship's current location.
         waypoint_symbol (str): The waypoint symbol of the ship's current location, or if the ship is in-transit, the
             waypoint symbol of the ship's destination.
         route (ShipNavRoute): The routing information for the ship's most recent transit or current location.
         status (ShipNavStatus): The current status of the ship
         flight_mode (ShipNavFlightMode): The ship's set speed when traveling between waypoints or systems. Default:
             ShipNavFlightMode.CRUISE.
     """
 
-    system_symbol: str
-    waypoint_symbol: str
-    route: "ShipNavRoute"
-    status: ShipNavStatus
+    system_symbol: str = Field(alias="systemSymbol")
+    waypoint_symbol: str = Field(alias="waypointSymbol")
+    route: "ShipNavRoute" = Field(alias="route")
+    status: ShipNavStatus = Field(alias="status")
     flight_mode: ShipNavFlightMode = ShipNavFlightMode.CRUISE
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav_route import ShipNavRoute
-
-        system_symbol = self.system_symbol
-        waypoint_symbol = self.waypoint_symbol
-        route = self.route.to_dict()
-
-        status = self.status.value
-
-        flight_mode = self.flight_mode.value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "systemSymbol": system_symbol,
-                "waypointSymbol": waypoint_symbol,
-                "route": route,
-                "status": status,
-                "flightMode": flight_mode,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav_route import ShipNavRoute
-
-        d = src_dict.copy()
-        system_symbol = d.pop("systemSymbol")
-
-        waypoint_symbol = d.pop("waypointSymbol")
-
-        route = ShipNavRoute.from_dict(d.pop("route"))
-
-        status = ShipNavStatus(d.pop("status"))
-
-        flight_mode = ShipNavFlightMode(d.pop("flightMode"))
-
-        ship_nav = cls(
-            system_symbol=system_symbol,
-            waypoint_symbol=waypoint_symbol,
-            route=route,
-            status=status,
-            flight_mode=flight_mode,
-        )
+    additional_properties: Dict[str, Any] = {}
 
-        ship_nav.additional_properties = d
-        return ship_nav
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_nav_route.py` & `spacetraders-0.2.0/spacetraders/models/ship_nav_route.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,88 +11,41 @@
     Type,
     TypeVar,
     cast,
 )
 
 import attr
 from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
+from ..models.ship_nav_route_waypoint import ShipNavRouteWaypoint
 from ..types import UNSET, Unset
 
-if TYPE_CHECKING:
-    from ..models.ship_nav_route_waypoint import ShipNavRouteWaypoint
-
-
 T = TypeVar("T", bound="ShipNavRoute")
 
 
-@attr.s(auto_attribs=True)
-class ShipNavRoute:
+class ShipNavRoute(BaseModel):
     """The routing information for the ship's most recent transit or current location.
 
     Attributes:
         destination (ShipNavRouteWaypoint): The destination or departure of a ships nav route.
         departure (ShipNavRouteWaypoint): The destination or departure of a ships nav route.
         departure_time (datetime.datetime): The date time of the ship's departure.
         arrival (datetime.datetime): The date time of the ship's arrival. If the ship is in-transit, this is the
             expected time of arrival.
     """
 
-    destination: "ShipNavRouteWaypoint"
-    departure: "ShipNavRouteWaypoint"
-    departure_time: datetime.datetime
-    arrival: datetime.datetime
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        from ..models.ship_nav_route_waypoint import ShipNavRouteWaypoint
-
-        destination = self.destination.to_dict()
-
-        departure = self.departure.to_dict()
-
-        departure_time = self.departure_time.isoformat()
-
-        arrival = self.arrival.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "destination": destination,
-                "departure": departure,
-                "departureTime": departure_time,
-                "arrival": arrival,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.ship_nav_route_waypoint import ShipNavRouteWaypoint
-
-        d = src_dict.copy()
-        destination = ShipNavRouteWaypoint.from_dict(d.pop("destination"))
-
-        departure = ShipNavRouteWaypoint.from_dict(d.pop("departure"))
-
-        departure_time = isoparse(d.pop("departureTime"))
-
-        arrival = isoparse(d.pop("arrival"))
-
-        ship_nav_route = cls(
-            destination=destination,
-            departure=departure,
-            departure_time=departure_time,
-            arrival=arrival,
-        )
+    destination: "ShipNavRouteWaypoint" = Field(alias="destination")
+    departure: "ShipNavRouteWaypoint" = Field(alias="departure")
+    departure_time: datetime.datetime = Field(alias="departureTime")
+    arrival: datetime.datetime = Field(alias="arrival")
+    additional_properties: Dict[str, Any] = {}
 
-        ship_nav_route.additional_properties = d
-        return ship_nav_route
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.2.0/spacetraders/models/ship_refine_json_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,55 +8,33 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.ship_refine_json_body_produce import ShipRefineJsonBodyProduce
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ShipRefineJsonBody")
 
 
-@attr.s(auto_attribs=True)
-class ShipRefineJsonBody:
+class ShipRefineJsonBody(BaseModel):
     """
     Attributes:
         produce (ShipRefineJsonBodyProduce):
     """
 
-    produce: ShipRefineJsonBodyProduce
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    produce: ShipRefineJsonBodyProduce = Field(alias="produce")
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        produce = self.produce.value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "produce": produce,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        produce = ShipRefineJsonBodyProduce(d.pop("produce"))
-
-        ship_refine_json_body = cls(
-            produce=produce,
-        )
-
-        ship_refine_json_body.additional_properties = d
-        return ship_refine_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.2.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,66 +5,39 @@
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
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataConsumedItem")
+T = TypeVar("T", bound="DeliverContractJsonBody")
 
 
-@attr.s(auto_attribs=True)
-class ShipRefineShipRefine200ResponseDataConsumedItem:
+class DeliverContractJsonBody(BaseModel):
     """
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        ship_symbol (str):
+        trade_symbol (str):
+        units (int):
     """
 
-    trade_symbol: Union[Unset, str] = UNSET
-    units: Union[Unset, int] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        trade_symbol = self.trade_symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if trade_symbol is not UNSET:
-            field_dict["tradeSymbol"] = trade_symbol
-        if units is not UNSET:
-            field_dict["units"] = units
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        trade_symbol = d.pop("tradeSymbol", UNSET)
-
-        units = d.pop("units", UNSET)
-
-        ship_refine_ship_refine_200_response_data_consumed_item = cls(
-            trade_symbol=trade_symbol,
-            units=units,
-        )
-
-        ship_refine_ship_refine_200_response_data_consumed_item.additional_properties = (
-            d
-        )
-        return ship_refine_ship_refine_200_response_data_consumed_item
+    ship_symbol: str = Field(alias="shipSymbol")
+    trade_symbol: str = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
+    additional_properties: Dict[str, Any] = {}
+
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.2.0/spacetraders/models/shipyard.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,65 +6,45 @@
     List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
+from ..models.shipyard_ship import ShipyardShip
+from ..models.shipyard_ship_types_item import ShipyardShipTypesItem
+from ..models.shipyard_transaction import ShipyardTransaction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRefineShipRefine200ResponseDataProducedItem")
+T = TypeVar("T", bound="Shipyard")
 
 
-@attr.s(auto_attribs=True)
-class ShipRefineShipRefine200ResponseDataProducedItem:
+class Shipyard(BaseModel):
     """
     Attributes:
-        trade_symbol (Union[Unset, str]):
-        units (Union[Unset, int]):
+        symbol (str): The symbol of the shipyard. The symbol is the same as the waypoint where the shipyard is located.
+        ship_types (List['ShipyardShipTypesItem']): The list of ship types available for purchase at this shipyard.
+        transactions (Union[Unset, List['ShipyardTransaction']]): The list of recent transactions at this shipyard.
+        ships (Union[Unset, List['ShipyardShip']]): The ships that are currently available for purchase at the shipyard.
     """
 
-    trade_symbol: Union[Unset, str] = UNSET
-    units: Union[Unset, int] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        trade_symbol = self.trade_symbol
-        units = self.units
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if trade_symbol is not UNSET:
-            field_dict["tradeSymbol"] = trade_symbol
-        if units is not UNSET:
-            field_dict["units"] = units
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        trade_symbol = d.pop("tradeSymbol", UNSET)
-
-        units = d.pop("units", UNSET)
-
-        ship_refine_ship_refine_200_response_data_produced_item = cls(
-            trade_symbol=trade_symbol,
-            units=units,
-        )
-
-        ship_refine_ship_refine_200_response_data_produced_item.additional_properties = (
-            d
-        )
-        return ship_refine_ship_refine_200_response_data_produced_item
+    symbol: str = Field(alias="symbol")
+    ship_types: List["ShipyardShipTypesItem"] = Field(alias="shipTypes")
+    transactions: Union[Unset, List["ShipyardTransaction"]] = UNSET
+    ships: Union[Unset, List["ShipyardShip"]] = UNSET
+    additional_properties: Dict[str, Any] = {}
+
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_registration.py` & `spacetraders-0.2.0/spacetraders/models/ship_registration.py`

 * *Files 23% similar despite different names*

```diff
@@ -9,72 +9,38 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..models.ship_role import ShipRole
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ShipRegistration")
 
 
-@attr.s(auto_attribs=True)
-class ShipRegistration:
+class ShipRegistration(BaseModel):
     """The public registration information of the ship
 
     Attributes:
         name (str): The agent's registered name of the ship
         role (ShipRole): The registered role of the ship
         faction_symbol (Union[Unset, str]): The symbol of the faction the ship is registered with
     """
 
-    name: str
-    role: ShipRole
+    name: str = Field(alias="name")
+    role: ShipRole = Field(alias="role")
     faction_symbol: Union[Unset, str] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        name = self.name
-        role = self.role.value
-
-        faction_symbol = self.faction_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "name": name,
-                "role": role,
-            }
-        )
-        if faction_symbol is not UNSET:
-            field_dict["factionSymbol"] = faction_symbol
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        name = d.pop("name")
-
-        role = ShipRole(d.pop("role"))
-
-        faction_symbol = d.pop("factionSymbol", UNSET)
-
-        ship_registration = cls(
-            name=name,
-            role=role,
-            faction_symbol=faction_symbol,
-        )
-
-        ship_registration.additional_properties = d
-        return ship_registration
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_requirements.py` & `spacetraders-0.2.0/spacetraders/models/ship_requirements.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,69 +9,37 @@
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
 T = TypeVar("T", bound="ShipRequirements")
 
 
-@attr.s(auto_attribs=True)
-class ShipRequirements:
+class ShipRequirements(BaseModel):
     """The requirements for installation on a ship
 
     Attributes:
         power (Union[Unset, int]): The amount of power required from the reactor.
         crew (Union[Unset, int]): The number of crew required for operation.
         slots (Union[Unset, int]): The number of module slots required for installation.
     """
 
     power: Union[Unset, int] = UNSET
     crew: Union[Unset, int] = UNSET
     slots: Union[Unset, int] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        power = self.power
-        crew = self.crew
-        slots = self.slots
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if power is not UNSET:
-            field_dict["power"] = power
-        if crew is not UNSET:
-            field_dict["crew"] = crew
-        if slots is not UNSET:
-            field_dict["slots"] = slots
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        power = d.pop("power", UNSET)
-
-        crew = d.pop("crew", UNSET)
-
-        slots = d.pop("slots", UNSET)
-
-        ship_requirements = cls(
-            power=power,
-            crew=crew,
-            slots=slots,
-        )
-
-        ship_requirements.additional_properties = d
-        return ship_requirements
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/ship_type.py` & `spacetraders-0.2.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.2.0/spacetraders/models/chart.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,68 +1,48 @@
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
     Union,
+    cast,
 )
 
 import attr
+from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
-from ..models.ship_type import ShipType
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipyardShipTypesItem")
+T = TypeVar("T", bound="Chart")
 
 
-@attr.s(auto_attribs=True)
-class ShipyardShipTypesItem:
-    """
+class Chart(BaseModel):
+    """The chart of a system or waypoint, which makes the location visible to other agents.
+
     Attributes:
-        type (Union[Unset, ShipType]):
+        waypoint_symbol (Union[Unset, str]):
+        submitted_by (Union[Unset, str]):
+        submitted_on (Union[Unset, datetime.datetime]):
     """
 
-    type: Union[Unset, ShipType] = UNSET
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        type: Union[Unset, str] = UNSET
-        if not isinstance(self.type, Unset):
-            type = self.type.value
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update({})
-        if type is not UNSET:
-            field_dict["type"] = type
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        _type = d.pop("type", UNSET)
-        type: Union[Unset, ShipType]
-        if isinstance(_type, Unset):
-            type = UNSET
-        else:
-            type = ShipType(_type)
-
-        shipyard_ship_types_item = cls(
-            type=type,
-        )
+    waypoint_symbol: Union[Unset, str] = UNSET
+    submitted_by: Union[Unset, str] = UNSET
+    submitted_on: Union[Unset, datetime.datetime] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        shipyard_ship_types_item.additional_properties = d
-        return shipyard_ship_types_item
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.2.0/spacetraders/models/market.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,56 @@
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
+    Union,
     cast,
 )
 
 import attr
-from dateutil.parser import isoparse
+from pydantic import BaseModel, Field
 
+from ..models.market_trade_good import MarketTradeGood
+from ..models.market_transaction import MarketTransaction
+from ..models.trade_good import TradeGood
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipyardTransaction")
+T = TypeVar("T", bound="Market")
 
 
-@attr.s(auto_attribs=True)
-class ShipyardTransaction:
+class Market(BaseModel):
     """
     Attributes:
-        waypoint_symbol (str): The symbol of the waypoint where the transaction took place.
-        ship_symbol (str): The symbol of the ship that was purchased.
-        price (int): The price of the transaction.
-        agent_symbol (str): The symbol of the agent that made the transaction.
-        timestamp (datetime.datetime): The timestamp of the transaction.
+        symbol (str): The symbol of the market. The symbol is the same as the waypoint where the market is located.
+        exports (List['TradeGood']): The list of goods that are exported from this market.
+        imports (List['TradeGood']): The list of goods that are sought as imports in this market.
+        exchange (List['TradeGood']): The list of goods that are bought and sold between agents at this market.
+        transactions (Union[Unset, List['MarketTransaction']]): The list of recent transactions at this market. Visible
+            only when a ship is present at the market.
+        trade_goods (Union[Unset, List['MarketTradeGood']]): The list of goods that are traded at this market. Visible
+            only when a ship is present at the market.
     """
 
-    waypoint_symbol: str
-    ship_symbol: str
-    price: int
-    agent_symbol: str
-    timestamp: datetime.datetime
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        waypoint_symbol = self.waypoint_symbol
-        ship_symbol = self.ship_symbol
-        price = self.price
-        agent_symbol = self.agent_symbol
-        timestamp = self.timestamp.isoformat()
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "waypointSymbol": waypoint_symbol,
-                "shipSymbol": ship_symbol,
-                "price": price,
-                "agentSymbol": agent_symbol,
-                "timestamp": timestamp,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        waypoint_symbol = d.pop("waypointSymbol")
-
-        ship_symbol = d.pop("shipSymbol")
-
-        price = d.pop("price")
-
-        agent_symbol = d.pop("agentSymbol")
-
-        timestamp = isoparse(d.pop("timestamp"))
-
-        shipyard_transaction = cls(
-            waypoint_symbol=waypoint_symbol,
-            ship_symbol=ship_symbol,
-            price=price,
-            agent_symbol=agent_symbol,
-            timestamp=timestamp,
-        )
+    symbol: str = Field(alias="symbol")
+    exports: List["TradeGood"] = Field(alias="exports")
+    imports: List["TradeGood"] = Field(alias="imports")
+    exchange: List["TradeGood"] = Field(alias="exchange")
+    transactions: Union[Unset, List["MarketTransaction"]] = UNSET
+    trade_goods: Union[Unset, List["MarketTradeGood"]] = UNSET
+    additional_properties: Dict[str, Any] = {}
 
-        shipyard_transaction.additional_properties = d
-        return shipyard_transaction
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/survey_deposit.py` & `spacetraders-0.2.0/spacetraders/models/jump_ship_response_200.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,58 +5,37 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.jump_ship_response_200_data import JumpShipResponse200Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SurveyDeposit")
+T = TypeVar("T", bound="JumpShipResponse200")
 
 
-@attr.s(auto_attribs=True)
-class SurveyDeposit:
-    """A surveyed deposit of a mineral or resource available for extraction.
-
+class JumpShipResponse200(BaseModel):
+    """
     Attributes:
-        symbol (str): The symbol of the deposit.
+        data (JumpShipResponse200Data):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        survey_deposit = cls(
-            symbol=symbol,
-        )
+    data: "JumpShipResponse200Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        survey_deposit.additional_properties = d
-        return survey_deposit
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/system_faction.py` & `spacetraders-0.2.0/spacetraders/models/create_chart_response_201.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,57 +5,37 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.create_chart_response_201_data import CreateChartResponse201Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SystemFaction")
+T = TypeVar("T", bound="CreateChartResponse201")
 
 
-@attr.s(auto_attribs=True)
-class SystemFaction:
+class CreateChartResponse201(BaseModel):
     """
     Attributes:
-        symbol (str):
+        data (CreateChartResponse201Data):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    data: "CreateChartResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        system_faction = cls(
-            symbol=symbol,
-        )
-
-        system_faction.additional_properties = d
-        return system_faction
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/system_waypoint.py` & `spacetraders-0.2.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files 23% similar despite different names*

```diff
@@ -5,80 +5,40 @@
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
+from pydantic import BaseModel, Field
 
-from ..models.waypoint_type import WaypointType
+from ..models.cooldown import Cooldown
+from ..models.scanned_system import ScannedSystem
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="SystemWaypoint")
+T = TypeVar("T", bound="CreateShipSystemScanResponse201Data")
 
 
-@attr.s(auto_attribs=True)
-class SystemWaypoint:
+class CreateShipSystemScanResponse201Data(BaseModel):
     """
     Attributes:
-        symbol (str):
-        type (WaypointType): The type of waypoint.
-        x (int):
-        y (int):
+        cooldown (Cooldown): A cooldown is a period of time in which a ship cannot perform certain actions.
+        systems (List['ScannedSystem']):
     """
 
-    symbol: str
-    type: WaypointType
-    x: int
-    y: int
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-        type = self.type.value
-
-        x = self.x
-        y = self.y
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "type": type,
-                "x": x,
-                "y": y,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        type = WaypointType(d.pop("type"))
-
-        x = d.pop("x")
-
-        y = d.pop("y")
-
-        system_waypoint = cls(
-            symbol=symbol,
-            type=type,
-            x=x,
-            y=y,
-        )
+    cooldown: "Cooldown" = Field(alias="cooldown")
+    systems: List["ScannedSystem"] = Field(alias="systems")
+    additional_properties: Dict[str, Any] = {}
 
-        system_waypoint.additional_properties = d
-        return system_waypoint
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/trade_good.py` & `spacetraders-0.2.0/spacetraders/models/survey_deposit.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,70 +8,33 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
-from ..models.trade_symbol import TradeSymbol
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="TradeGood")
+T = TypeVar("T", bound="SurveyDeposit")
 
 
-@attr.s(auto_attribs=True)
-class TradeGood:
-    """
+class SurveyDeposit(BaseModel):
+    """A surveyed deposit of a mineral or resource available for extraction.
+
     Attributes:
-        symbol (TradeSymbol):
-        name (str):
-        description (str):
+        symbol (str): The symbol of the deposit.
     """
 
-    symbol: TradeSymbol
-    name: str
-    description: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol.value
-
-        name = self.name
-        description = self.description
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "name": name,
-                "description": description,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = TradeSymbol(d.pop("symbol"))
-
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        trade_good = cls(
-            symbol=symbol,
-            name=name,
-            description=description,
-        )
+    symbol: str = Field(alias="symbol")
+    additional_properties: Dict[str, Any] = {}
 
-        trade_good.additional_properties = d
-        return trade_good
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/trade_symbol.py` & `spacetraders-0.2.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.2.0/spacetraders/models/register_response_201.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,71 +5,37 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.register_response_201_data import RegisterResponse201Data
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
+T = TypeVar("T", bound="RegisterResponse201")
 
 
-@attr.s(auto_attribs=True)
-class TransferCargoTransferCargoRequest:
+class RegisterResponse201(BaseModel):
     """
     Attributes:
-        trade_symbol (str):
-        units (int):
-        ship_symbol (str):
+        data (RegisterResponse201Data):
     """
 
-    trade_symbol: str
-    units: int
-    ship_symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        trade_symbol = self.trade_symbol
-        units = self.units
-        ship_symbol = self.ship_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "tradeSymbol": trade_symbol,
-                "units": units,
-                "shipSymbol": ship_symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        trade_symbol = d.pop("tradeSymbol")
-
-        units = d.pop("units")
-
-        ship_symbol = d.pop("shipSymbol")
-
-        transfer_cargo_transfer_cargo_request = cls(
-            trade_symbol=trade_symbol,
-            units=units,
-            ship_symbol=ship_symbol,
-        )
+    data: "RegisterResponse201Data" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        transfer_cargo_transfer_cargo_request.additional_properties = d
-        return transfer_cargo_transfer_cargo_request
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.2.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,57 +5,39 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.sell_cargo_sell_cargo_201_response_data import (
+    SellCargoSellCargo201ResponseData,
+)
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WarpShipJsonBody")
+T = TypeVar("T", bound="SellCargoSellCargo201Response")
 
 
-@attr.s(auto_attribs=True)
-class WarpShipJsonBody:
+class SellCargoSellCargo201Response(BaseModel):
     """
     Attributes:
-        waypoint_symbol (str): The target destination.
+        data (SellCargoSellCargo201ResponseData):
     """
 
-    waypoint_symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        waypoint_symbol = self.waypoint_symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "waypointSymbol": waypoint_symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        waypoint_symbol = d.pop("waypointSymbol")
-
-        warp_ship_json_body = cls(
-            waypoint_symbol=waypoint_symbol,
-        )
+    data: "SellCargoSellCargo201ResponseData" = Field(alias="data")
+    additional_properties: Dict[str, Any] = {}
 
-        warp_ship_json_body.additional_properties = d
-        return warp_ship_json_body
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/waypoint_faction.py` & `spacetraders-0.2.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,54 +8,36 @@
     TextIO,
     Tuple,
     Type,
     TypeVar,
 )
 
 import attr
+from pydantic import BaseModel, Field
 
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WaypointFaction")
+T = TypeVar("T", bound="TransferCargoTransferCargoRequest")
 
 
-@attr.s(auto_attribs=True)
-class WaypointFaction:
+class TransferCargoTransferCargoRequest(BaseModel):
     """
     Attributes:
-        symbol (str):
+        trade_symbol (str):
+        units (int):
+        ship_symbol (str):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
+    trade_symbol: str = Field(alias="tradeSymbol")
+    units: int = Field(alias="units")
+    ship_symbol: str = Field(alias="shipSymbol")
+    additional_properties: Dict[str, Any] = {}
 
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        waypoint_faction = cls(
-            symbol=symbol,
-        )
-
-        waypoint_faction.additional_properties = d
-        return waypoint_faction
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.2.0/spacetraders/models/faction.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,58 +5,45 @@
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
+from pydantic import BaseModel, Field
 
+from ..models.faction_trait import FactionTrait
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WaypointOrbital")
+T = TypeVar("T", bound="Faction")
 
 
-@attr.s(auto_attribs=True)
-class WaypointOrbital:
-    """An orbital is another waypoint that orbits a parent waypoint.
-
+class Faction(BaseModel):
+    """
     Attributes:
         symbol (str):
+        name (str):
+        description (str):
+        headquarters (str):
+        traits (List['FactionTrait']):
     """
 
-    symbol: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = d.pop("symbol")
-
-        waypoint_orbital = cls(
-            symbol=symbol,
-        )
+    symbol: str = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
+    headquarters: str = Field(alias="headquarters")
+    traits: List["FactionTrait"] = Field(alias="traits")
+    additional_properties: Dict[str, Any] = {}
 
-        waypoint_orbital.additional_properties = d
-        return waypoint_orbital
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/waypoint_trait.py` & `spacetraders-0.2.0/spacetraders/models/cooldown.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,49 @@
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
+from pydantic import BaseModel, Field
 
-from ..models.waypoint_trait_symbol import WaypointTraitSymbol
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="WaypointTrait")
+T = TypeVar("T", bound="Cooldown")
 
 
-@attr.s(auto_attribs=True)
-class WaypointTrait:
-    """
+class Cooldown(BaseModel):
+    """A cooldown is a period of time in which a ship cannot perform certain actions.
+
     Attributes:
-        symbol (WaypointTraitSymbol): The unique identifier of the trait.
-        name (str): The name of the trait.
-        description (str): A description of the trait.
+        ship_symbol (str): The symbol of the ship that is on cooldown
+        total_seconds (int): The total duration of the cooldown in seconds
+        remaining_seconds (int): The remaining duration of the cooldown in seconds
+        expiration (datetime.datetime): The date and time when the cooldown expires in ISO 8601 format
     """
 
-    symbol: WaypointTraitSymbol
-    name: str
-    description: str
-    additional_properties: Dict[str, Any] = attr.ib(init=False, factory=dict)
-
-    def to_dict(self) -> Dict[str, Any]:
-        symbol = self.symbol.value
-
-        name = self.name
-        description = self.description
-
-        field_dict: Dict[str, Any] = {}
-        field_dict.update(self.additional_properties)
-        field_dict.update(
-            {
-                "symbol": symbol,
-                "name": name,
-                "description": description,
-            }
-        )
-
-        return field_dict
-
-    @classmethod
-    def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        d = src_dict.copy()
-        symbol = WaypointTraitSymbol(d.pop("symbol"))
-
-        name = d.pop("name")
-
-        description = d.pop("description")
-
-        waypoint_trait = cls(
-            symbol=symbol,
-            name=name,
-            description=description,
-        )
+    ship_symbol: str = Field(alias="shipSymbol")
+    total_seconds: int = Field(alias="totalSeconds")
+    remaining_seconds: int = Field(alias="remainingSeconds")
+    expiration: datetime.datetime = Field(alias="expiration")
+    additional_properties: Dict[str, Any] = {}
 
-        waypoint_trait.additional_properties = d
-        return waypoint_trait
+    class Config:
+        arbitrary_types_allowed = True
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
     def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
```

### Comparing `spacetraders-0.1.4/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.2.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/spacetraders/types.py` & `spacetraders-0.2.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.1.4/PKG-INFO` & `spacetraders-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.1.4
+Version: 0.2.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Description-Content-Type: text/markdown
 
 # spacetraders python client
 A client library for accessing SpaceTraders API
 
 ## Usage
 First, create a client:
```

