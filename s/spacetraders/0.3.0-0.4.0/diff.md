# Comparing `tmp/spacetraders-0.3.0.tar.gz` & `tmp/spacetraders-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetraders-0.3.0.tar", max compression
+gzip compressed data, was "spacetraders-0.4.0.tar", max compression
```

## Comparing `spacetraders-0.3.0.tar` & `spacetraders-0.4.0.tar`

### file list

```diff
@@ -1,208 +1,208 @@
--rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.3.0/README.md
--rw-r--r--   0        0        0      664 2023-05-13 04:32:06.857117 spacetraders-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      250 2023-05-13 04:23:44.257117 spacetraders-0.3.0/spacetraders/__init__.py
--rw-r--r--   0        0        0       47 2023-05-13 04:23:43.767117 spacetraders-0.3.0/spacetraders/api/__init__.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.817117 spacetraders-0.3.0/spacetraders/api/agents/__init__.py
--rw-r--r--   0        0        0     4139 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/agents/get_my_agent.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.817117 spacetraders-0.3.0/spacetraders/api/contracts/__init__.py
--rw-r--r--   0        0        0     4425 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/contracts/accept_contract.py
--rw-r--r--   0        0        0     5022 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/contracts/deliver_contract.py
--rw-r--r--   0        0        0     4437 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/contracts/fulfill_contract.py
--rw-r--r--   0        0        0     4420 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/contracts/get_contract.py
--rw-r--r--   0        0        0     4900 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/contracts/get_contracts.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.777117 spacetraders-0.3.0/spacetraders/api/default/__init__.py
--rw-r--r--   0        0        0     6960 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/default/register.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.817117 spacetraders-0.3.0/spacetraders/api/factions/__init__.py
--rw-r--r--   0        0        0     4427 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/factions/get_faction.py
--rw-r--r--   0        0        0     4853 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/factions/get_factions.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.827117 spacetraders-0.3.0/spacetraders/api/fleet/__init__.py
--rw-r--r--   0        0        0     4900 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/create_chart.py
--rw-r--r--   0        0        0     4550 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/create_ship_ship_scan.py
--rw-r--r--   0        0        0     4587 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/create_ship_system_scan.py
--rw-r--r--   0        0        0     4615 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
--rw-r--r--   0        0        0     5382 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/create_survey.py
--rw-r--r--   0        0        0     4961 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/dock_ship.py
--rw-r--r--   0        0        0     5217 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/extract_resources.py
--rw-r--r--   0        0        0     4373 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/get_my_ship.py
--rw-r--r--   0        0        0     4447 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/get_my_ship_cargo.py
--rw-r--r--   0        0        0     4871 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/get_my_ships.py
--rw-r--r--   0        0        0     5562 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/get_ship_cooldown.py
--rw-r--r--   0        0        0     4414 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/get_ship_nav.py
--rw-r--r--   0        0        0     4905 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/jettison.py
--rw-r--r--   0        0        0     5049 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/jump_ship.py
--rw-r--r--   0        0        0     5893 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/navigate_ship.py
--rw-r--r--   0        0        0     4954 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/fleet/orbit_ship.py
--rw-r--r--   0        0        0     5001 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/patch_ship_nav.py
--rw-r--r--   0        0        0     5192 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/purchase_cargo.py
--rw-r--r--   0        0        0     4680 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/purchase_ship.py
--rw-r--r--   0        0        0     4419 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/refuel_ship.py
--rw-r--r--   0        0        0     5010 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/sell_cargo.py
--rw-r--r--   0        0        0     5244 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/ship_refine.py
--rw-r--r--   0        0        0     5215 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/transfer_cargo.py
--rw-r--r--   0        0        0     5569 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/fleet/warp_ship.py
--rw-r--r--   0        0        0        0 2023-05-13 04:23:43.807117 spacetraders-0.3.0/spacetraders/api/systems/__init__.py
--rw-r--r--   0        0        0     4735 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_jump_gate.py
--rw-r--r--   0        0        0     5121 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_market.py
--rw-r--r--   0        0        0     4721 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_shipyard.py
--rw-r--r--   0        0        0     4469 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_system.py
--rw-r--r--   0        0        0     5421 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/api/systems/get_system_waypoints.py
--rw-r--r--   0        0        0     4877 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_systems.py
--rw-r--r--   0        0        0     4710 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/api/systems/get_waypoint.py
--rw-r--r--   0        0        0     4384 2023-05-13 04:23:44.617117 spacetraders-0.3.0/spacetraders/client.py
--rw-r--r--   0        0        0      470 2023-05-13 04:23:44.557117 spacetraders-0.3.0/spacetraders/errors.py
--rw-r--r--   0        0        0    13081 2023-05-13 04:23:44.717117 spacetraders-0.3.0/spacetraders/models/__init__.py
--rw-r--r--   0        0        0     1269 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/accept_contract_response_200.py
--rw-r--r--   0        0        0     1299 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/accept_contract_response_200_data.py
--rw-r--r--   0        0        0     1460 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/agent.py
--rw-r--r--   0        0        0     1532 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/chart.py
--rw-r--r--   0        0        0     1709 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/connected_system.py
--rw-r--r--   0        0        0     1887 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/contract.py
--rw-r--r--   0        0        0     1712 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/contract_deliver_good.py
--rw-r--r--   0        0        0     1340 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/contract_payment.py
--rw-r--r--   0        0        0     1567 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/contract_terms.py
--rw-r--r--   0        0        0      201 2023-05-13 04:23:43.937117 spacetraders-0.3.0/spacetraders/models/contract_type.py
--rw-r--r--   0        0        0     1691 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/cooldown.py
--rw-r--r--   0        0        0     1251 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/create_chart_response_201.py
--rw-r--r--   0        0        0     1469 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_chart_response_201_data.py
--rw-r--r--   0        0        0     1304 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/create_ship_ship_scan_response_201.py
--rw-r--r--   0        0        0     1425 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
--rw-r--r--   0        0        0     1316 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_ship_system_scan_response_201.py
--rw-r--r--   0        0        0     1443 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_ship_system_scan_response_201_data.py
--rw-r--r--   0        0        0     1328 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
--rw-r--r--   0        0        0     1461 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
--rw-r--r--   0        0        0     1257 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/create_survey_response_201.py
--rw-r--r--   0        0        0     1398 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/create_survey_response_201_data.py
--rw-r--r--   0        0        0     1284 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/deliver_contract_json_body.py
--rw-r--r--   0        0        0     1275 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/deliver_contract_response_200.py
--rw-r--r--   0        0        0     1318 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/deliver_contract_response_200_data.py
--rw-r--r--   0        0        0     1292 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/dock_ship_dock_ship_200_response.py
--rw-r--r--   0        0        0     1227 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
--rw-r--r--   0        0        0     1368 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/extract_resources_json_body.py
--rw-r--r--   0        0        0     1281 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/extract_resources_response_201.py
--rw-r--r--   0        0        0     1532 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/extract_resources_response_201_data.py
--rw-r--r--   0        0        0     1261 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/extraction.py
--rw-r--r--   0        0        0     1250 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/extraction_yield.py
--rw-r--r--   0        0        0     1457 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/faction.py
--rw-r--r--   0        0        0     1421 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/faction_trait.py
--rw-r--r--   0        0        0     2091 2023-05-13 04:23:44.017117 spacetraders-0.3.0/spacetraders/models/faction_trait_symbol.py
--rw-r--r--   0        0        0     1275 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/fulfill_contract_response_200.py
--rw-r--r--   0        0        0     1301 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/fulfill_contract_response_200_data.py
--rw-r--r--   0        0        0     1175 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_contract_response_200.py
--rw-r--r--   0        0        0     1282 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_contracts_response_200.py
--rw-r--r--   0        0        0     1169 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_faction_response_200.py
--rw-r--r--   0        0        0     1276 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_factions_response_200.py
--rw-r--r--   0        0        0     1176 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_jump_gate_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_market_response_200.py
--rw-r--r--   0        0        0     1161 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_my_agent_response_200.py
--rw-r--r--   0        0        0     1186 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_my_ship_cargo_response_200.py
--rw-r--r--   0        0        0     1162 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_my_ship_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_my_ships_response_200.py
--rw-r--r--   0        0        0     1262 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_ship_cooldown_response_200.py
--rw-r--r--   0        0        0     1210 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_ship_nav_response_200.py
--rw-r--r--   0        0        0     1175 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_shipyard_response_200.py
--rw-r--r--   0        0        0     1163 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_system_response_200.py
--rw-r--r--   0        0        0     1294 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/get_system_waypoints_response_200.py
--rw-r--r--   0        0        0     1270 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_systems_response_200.py
--rw-r--r--   0        0        0     1266 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/get_waypoint_response_200.py
--rw-r--r--   0        0        0     1177 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/jettison_json_body.py
--rw-r--r--   0        0        0     1232 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/jettison_response_200.py
--rw-r--r--   0        0        0     1185 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/jettison_response_200_data.py
--rw-r--r--   0        0        0     1606 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/jump_gate.py
--rw-r--r--   0        0        0     1168 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/jump_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/jump_ship_response_200.py
--rw-r--r--   0        0        0     1462 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/jump_ship_response_200_data.py
--rw-r--r--   0        0        0     2398 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/market.py
--rw-r--r--   0        0        0     1880 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/market_trade_good.py
--rw-r--r--   0        0        0      224 2023-05-13 04:23:43.937117 spacetraders-0.3.0/spacetraders/models/market_trade_good_supply.py
--rw-r--r--   0        0        0     2109 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/market_transaction.py
--rw-r--r--   0        0        0      170 2023-05-13 04:23:43.947117 spacetraders-0.3.0/spacetraders/models/market_transaction_type.py
--rw-r--r--   0        0        0     1206 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/meta.py
--rw-r--r--   0        0        0     1176 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/navigate_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/navigate_ship_response_200.py
--rw-r--r--   0        0        0     1444 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/navigate_ship_response_200_data.py
--rw-r--r--   0        0        0     1304 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
--rw-r--r--   0        0        0     1231 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
--rw-r--r--   0        0        0     1420 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/patch_ship_nav_json_body.py
--rw-r--r--   0        0        0     1214 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/patch_ship_nav_response_200.py
--rw-r--r--   0        0        0     1352 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
--rw-r--r--   0        0        0     1484 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
--rw-r--r--   0        0        0     1211 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
--rw-r--r--   0        0        0     1333 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/purchase_ship_json_body.py
--rw-r--r--   0        0        0     1257 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/purchase_ship_response_201.py
--rw-r--r--   0        0        0     1447 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/purchase_ship_response_201_data.py
--rw-r--r--   0        0        0     1245 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/refuel_ship_response_200.py
--rw-r--r--   0        0        0     1397 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/refuel_ship_response_200_data.py
--rw-r--r--   0        0        0     1419 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/register_json_body.py
--rw-r--r--   0        0        0      244 2023-05-13 04:23:43.997117 spacetraders-0.3.0/spacetraders/models/register_json_body_faction.py
--rw-r--r--   0        0        0     1232 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/register_response_201.py
--rw-r--r--   0        0        0     1608 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/register_response_201_data.py
--rw-r--r--   0        0        0     2444 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/scanned_ship.py
--rw-r--r--   0        0        0     1144 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/scanned_ship_engine.py
--rw-r--r--   0        0        0     1141 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/scanned_ship_frame.py
--rw-r--r--   0        0        0     1149 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/scanned_ship_mounts_item.py
--rw-r--r--   0        0        0     1147 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/scanned_ship_reactor.py
--rw-r--r--   0        0        0     1492 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/scanned_system.py
--rw-r--r--   0        0        0     2293 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/scanned_waypoint.py
--rw-r--r--   0        0        0     1304 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
--rw-r--r--   0        0        0     1468 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
--rw-r--r--   0        0        0     1195 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_request.py
--rw-r--r--   0        0        0     3140 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship.py
--rw-r--r--   0        0        0     1484 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_cargo.py
--rw-r--r--   0        0        0     1510 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_cargo_item.py
--rw-r--r--   0        0        0     2248 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_crew.py
--rw-r--r--   0        0        0      167 2023-05-13 04:23:43.907117 spacetraders-0.3.0/spacetraders/models/ship_crew_rotation.py
--rw-r--r--   0        0        0     1883 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_engine.py
--rw-r--r--   0        0        0      319 2023-05-13 04:23:43.997117 spacetraders-0.3.0/spacetraders/models/ship_engine_symbol.py
--rw-r--r--   0        0        0     2278 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_frame.py
--rw-r--r--   0        0        0      694 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/ship_frame_symbol.py
--rw-r--r--   0        0        0     1586 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_fuel.py
--rw-r--r--   0        0        0     1340 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_fuel_consumed.py
--rw-r--r--   0        0        0     1965 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_module.py
--rw-r--r--   0        0        0     1033 2023-05-13 04:23:43.947117 spacetraders-0.3.0/spacetraders/models/ship_module_symbol.py
--rw-r--r--   0        0        0     1947 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_mount.py
--rw-r--r--   0        0        0      572 2023-05-13 04:23:44.007117 spacetraders-0.3.0/spacetraders/models/ship_mount_deposits_item.py
--rw-r--r--   0        0        0      854 2023-05-13 04:23:44.007117 spacetraders-0.3.0/spacetraders/models/ship_mount_symbol.py
--rw-r--r--   0        0        0     2114 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_nav.py
--rw-r--r--   0        0        0      206 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/ship_nav_flight_mode.py
--rw-r--r--   0        0        0     1891 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_nav_route.py
--rw-r--r--   0        0        0     1497 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_nav_route_waypoint.py
--rw-r--r--   0        0        0      196 2023-05-13 04:23:43.947117 spacetraders-0.3.0/spacetraders/models/ship_nav_status.py
--rw-r--r--   0        0        0     1934 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_reactor.py
--rw-r--r--   0        0        0      344 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/ship_reactor_symbol.py
--rw-r--r--   0        0        0     1246 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_refine_json_body.py
--rw-r--r--   0        0        0      330 2023-05-13 04:23:43.997117 spacetraders-0.3.0/spacetraders/models/ship_refine_json_body_produce.py
--rw-r--r--   0        0        0     1316 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response.py
--rw-r--r--   0        0        0     2047 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
--rw-r--r--   0        0        0     1344 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
--rw-r--r--   0        0        0     1344 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
--rw-r--r--   0        0        0     1530 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/ship_registration.py
--rw-r--r--   0        0        0     1541 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/ship_requirements.py
--rw-r--r--   0        0        0      479 2023-05-13 04:23:43.987117 spacetraders-0.3.0/spacetraders/models/ship_role.py
--rw-r--r--   0        0        0      549 2023-05-13 04:23:43.917117 spacetraders-0.3.0/spacetraders/models/ship_type.py
--rw-r--r--   0        0        0     2009 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/shipyard.py
--rw-r--r--   0        0        0     2498 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/shipyard_ship.py
--rw-r--r--   0        0        0     1225 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/shipyard_ship_types_item.py
--rw-r--r--   0        0        0     1698 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/shipyard_transaction.py
--rw-r--r--   0        0        0     2228 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/survey.py
--rw-r--r--   0        0        0     1209 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/survey_deposit.py
--rw-r--r--   0        0        0      181 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/survey_size.py
--rw-r--r--   0        0        0     1725 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/system.py
--rw-r--r--   0        0        0     1112 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/system_faction.py
--rw-r--r--   0        0        0      405 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/system_type.py
--rw-r--r--   0        0        0     1352 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/system_waypoint.py
--rw-r--r--   0        0        0     1299 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/trade_good.py
--rw-r--r--   0        0        0     4422 2023-05-13 04:23:43.987117 spacetraders-0.3.0/spacetraders/models/trade_symbol.py
--rw-r--r--   0        0        0     1352 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
--rw-r--r--   0        0        0     1221 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
--rw-r--r--   0        0        0     1304 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
--rw-r--r--   0        0        0     1168 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/warp_ship_json_body.py
--rw-r--r--   0        0        0     1233 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/warp_ship_response_200.py
--rw-r--r--   0        0        0     1436 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/warp_ship_response_200_data.py
--rw-r--r--   0        0        0     2279 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/waypoint.py
--rw-r--r--   0        0        0     1116 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/waypoint_faction.py
--rw-r--r--   0        0        0     1178 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/models/waypoint_orbital.py
--rw-r--r--   0        0        0     1427 2023-05-13 04:23:44.997117 spacetraders-0.3.0/spacetraders/models/waypoint_trait.py
--rw-r--r--   0        0        0     2200 2023-05-13 04:23:44.017117 spacetraders-0.3.0/spacetraders/models/waypoint_trait_symbol.py
--rw-r--r--   0        0        0      381 2023-05-13 04:23:43.927117 spacetraders-0.3.0/spacetraders/models/waypoint_type.py
--rw-r--r--   0        0        0     1341 2023-05-13 04:23:45.007117 spacetraders-0.3.0/spacetraders/types.py
--rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3472 2023-05-10 04:00:00.539673 spacetraders-0.4.0/README.md
+-rw-r--r--   0        0        0      664 2023-05-15 19:26:39.587370 spacetraders-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      250 2023-05-15 19:23:16.207370 spacetraders-0.4.0/spacetraders/__init__.py
+-rw-r--r--   0        0        0       47 2023-05-15 19:23:15.557370 spacetraders-0.4.0/spacetraders/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/agents/__init__.py
+-rw-r--r--   0        0        0     4139 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/agents/get_my_agent.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/contracts/__init__.py
+-rw-r--r--   0        0        0     4425 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/contracts/accept_contract.py
+-rw-r--r--   0        0        0     5022 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/contracts/deliver_contract.py
+-rw-r--r--   0        0        0     4437 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/api/contracts/fulfill_contract.py
+-rw-r--r--   0        0        0     4420 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/contracts/get_contract.py
+-rw-r--r--   0        0        0     4900 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/api/contracts/get_contracts.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.567370 spacetraders-0.4.0/spacetraders/api/default/__init__.py
+-rw-r--r--   0        0        0     6960 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/default/register.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.607370 spacetraders-0.4.0/spacetraders/api/factions/__init__.py
+-rw-r--r--   0        0        0     4427 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/factions/get_faction.py
+-rw-r--r--   0        0        0     4853 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/factions/get_factions.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.617370 spacetraders-0.4.0/spacetraders/api/fleet/__init__.py
+-rw-r--r--   0        0        0     4900 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/create_chart.py
+-rw-r--r--   0        0        0     4550 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_ship_scan.py
+-rw-r--r--   0        0        0     4587 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_system_scan.py
+-rw-r--r--   0        0        0     4615 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/create_ship_waypoint_scan.py
+-rw-r--r--   0        0        0     5382 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/create_survey.py
+-rw-r--r--   0        0        0     4961 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/dock_ship.py
+-rw-r--r--   0        0        0     5217 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/extract_resources.py
+-rw-r--r--   0        0        0     4373 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship.py
+-rw-r--r--   0        0        0     4447 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship_cargo.py
+-rw-r--r--   0        0        0     4871 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/get_my_ships.py
+-rw-r--r--   0        0        0     5562 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/get_ship_cooldown.py
+-rw-r--r--   0        0        0     4414 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/get_ship_nav.py
+-rw-r--r--   0        0        0     4905 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/jettison.py
+-rw-r--r--   0        0        0     5049 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/jump_ship.py
+-rw-r--r--   0        0        0     5893 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/navigate_ship.py
+-rw-r--r--   0        0        0     4954 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/orbit_ship.py
+-rw-r--r--   0        0        0     5001 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/patch_ship_nav.py
+-rw-r--r--   0        0        0     5192 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/purchase_cargo.py
+-rw-r--r--   0        0        0     4680 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/purchase_ship.py
+-rw-r--r--   0        0        0     4419 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/refuel_ship.py
+-rw-r--r--   0        0        0     5010 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/fleet/sell_cargo.py
+-rw-r--r--   0        0        0     5244 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/fleet/ship_refine.py
+-rw-r--r--   0        0        0     5215 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/transfer_cargo.py
+-rw-r--r--   0        0        0     5569 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/fleet/warp_ship.py
+-rw-r--r--   0        0        0        0 2023-05-15 19:23:15.597370 spacetraders-0.4.0/spacetraders/api/systems/__init__.py
+-rw-r--r--   0        0        0     4735 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_jump_gate.py
+-rw-r--r--   0        0        0     5121 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/systems/get_market.py
+-rw-r--r--   0        0        0     4951 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/systems/get_shipyard.py
+-rw-r--r--   0        0        0     4469 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_system.py
+-rw-r--r--   0        0        0     5421 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/api/systems/get_system_waypoints.py
+-rw-r--r--   0        0        0     4877 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/api/systems/get_systems.py
+-rw-r--r--   0        0        0     4710 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/api/systems/get_waypoint.py
+-rw-r--r--   0        0        0     4384 2023-05-15 19:23:16.717370 spacetraders-0.4.0/spacetraders/client.py
+-rw-r--r--   0        0        0      470 2023-05-15 19:23:16.507370 spacetraders-0.4.0/spacetraders/errors.py
+-rw-r--r--   0        0        0    13081 2023-05-15 19:23:16.897370 spacetraders-0.4.0/spacetraders/models/__init__.py
+-rw-r--r--   0        0        0     1269 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/accept_contract_response_200.py
+-rw-r--r--   0        0        0     1299 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/accept_contract_response_200_data.py
+-rw-r--r--   0        0        0     1460 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/agent.py
+-rw-r--r--   0        0        0     1532 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/chart.py
+-rw-r--r--   0        0        0     1709 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/connected_system.py
+-rw-r--r--   0        0        0     1887 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract.py
+-rw-r--r--   0        0        0     1712 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_deliver_good.py
+-rw-r--r--   0        0        0     1340 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_payment.py
+-rw-r--r--   0        0        0     1567 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/contract_terms.py
+-rw-r--r--   0        0        0      201 2023-05-15 19:23:15.757370 spacetraders-0.4.0/spacetraders/models/contract_type.py
+-rw-r--r--   0        0        0     1691 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/cooldown.py
+-rw-r--r--   0        0        0     1251 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_chart_response_201.py
+-rw-r--r--   0        0        0     1469 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_chart_response_201_data.py
+-rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201.py
+-rw-r--r--   0        0        0     1425 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201_data.py
+-rw-r--r--   0        0        0     1316 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201.py
+-rw-r--r--   0        0        0     1443 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201_data.py
+-rw-r--r--   0        0        0     1328 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201.py
+-rw-r--r--   0        0        0     1461 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py
+-rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/create_survey_response_201.py
+-rw-r--r--   0        0        0     1398 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/create_survey_response_201_data.py
+-rw-r--r--   0        0        0     1284 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/deliver_contract_json_body.py
+-rw-r--r--   0        0        0     1275 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200.py
+-rw-r--r--   0        0        0     1318 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200_data.py
+-rw-r--r--   0        0        0     1292 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response.py
+-rw-r--r--   0        0        0     1227 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py
+-rw-r--r--   0        0        0     1368 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extract_resources_json_body.py
+-rw-r--r--   0        0        0     1281 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/extract_resources_response_201.py
+-rw-r--r--   0        0        0     1532 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extract_resources_response_201_data.py
+-rw-r--r--   0        0        0     1261 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/extraction.py
+-rw-r--r--   0        0        0     1250 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/extraction_yield.py
+-rw-r--r--   0        0        0     1457 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/faction.py
+-rw-r--r--   0        0        0     1421 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/faction_trait.py
+-rw-r--r--   0        0        0     1869 2023-05-15 19:23:15.857370 spacetraders-0.4.0/spacetraders/models/faction_trait_symbol.py
+-rw-r--r--   0        0        0     1275 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200.py
+-rw-r--r--   0        0        0     1301 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200_data.py
+-rw-r--r--   0        0        0     1175 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_contract_response_200.py
+-rw-r--r--   0        0        0     1282 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_contracts_response_200.py
+-rw-r--r--   0        0        0     1169 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_faction_response_200.py
+-rw-r--r--   0        0        0     1276 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_factions_response_200.py
+-rw-r--r--   0        0        0     1176 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_jump_gate_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_market_response_200.py
+-rw-r--r--   0        0        0     1161 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_my_agent_response_200.py
+-rw-r--r--   0        0        0     1186 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_my_ship_cargo_response_200.py
+-rw-r--r--   0        0        0     1162 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_my_ship_response_200.py
+-rw-r--r--   0        0        0     1262 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_my_ships_response_200.py
+-rw-r--r--   0        0        0     1262 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_ship_cooldown_response_200.py
+-rw-r--r--   0        0        0     1210 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1175 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_shipyard_response_200.py
+-rw-r--r--   0        0        0     1163 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/get_system_response_200.py
+-rw-r--r--   0        0        0     1294 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/get_system_waypoints_response_200.py
+-rw-r--r--   0        0        0     1270 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/get_systems_response_200.py
+-rw-r--r--   0        0        0     1266 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/get_waypoint_response_200.py
+-rw-r--r--   0        0        0     1177 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jettison_json_body.py
+-rw-r--r--   0        0        0     1232 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jettison_response_200.py
+-rw-r--r--   0        0        0     1185 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/jettison_response_200_data.py
+-rw-r--r--   0        0        0     1606 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_gate.py
+-rw-r--r--   0        0        0     1168 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/jump_ship_response_200.py
+-rw-r--r--   0        0        0     1462 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/jump_ship_response_200_data.py
+-rw-r--r--   0        0        0     2398 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/market.py
+-rw-r--r--   0        0        0     1880 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/market_trade_good.py
+-rw-r--r--   0        0        0      224 2023-05-15 19:23:15.757370 spacetraders-0.4.0/spacetraders/models/market_trade_good_supply.py
+-rw-r--r--   0        0        0     2109 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/market_transaction.py
+-rw-r--r--   0        0        0      170 2023-05-15 19:23:15.767370 spacetraders-0.4.0/spacetraders/models/market_transaction_type.py
+-rw-r--r--   0        0        0     1206 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/meta.py
+-rw-r--r--   0        0        0     1176 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/navigate_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200.py
+-rw-r--r--   0        0        0     1444 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200_data.py
+-rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py
+-rw-r--r--   0        0        0     1231 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py
+-rw-r--r--   0        0        0     1420 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/patch_ship_nav_json_body.py
+-rw-r--r--   0        0        0     1214 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/patch_ship_nav_response_200.py
+-rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py
+-rw-r--r--   0        0        0     1484 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1211 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py
+-rw-r--r--   0        0        0     1333 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_ship_json_body.py
+-rw-r--r--   0        0        0     1257 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201.py
+-rw-r--r--   0        0        0     1447 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201_data.py
+-rw-r--r--   0        0        0     1245 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200.py
+-rw-r--r--   0        0        0     1397 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200_data.py
+-rw-r--r--   0        0        0     1611 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/register_json_body.py
+-rw-r--r--   0        0        0      244 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/register_json_body_faction.py
+-rw-r--r--   0        0        0     1232 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/register_response_201.py
+-rw-r--r--   0        0        0     1608 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/register_response_201_data.py
+-rw-r--r--   0        0        0     2444 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/scanned_ship.py
+-rw-r--r--   0        0        0     1144 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_ship_engine.py
+-rw-r--r--   0        0        0     1141 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_frame.py
+-rw-r--r--   0        0        0     1149 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_mounts_item.py
+-rw-r--r--   0        0        0     1147 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/scanned_ship_reactor.py
+-rw-r--r--   0        0        0     1492 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_system.py
+-rw-r--r--   0        0        0     2293 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/scanned_waypoint.py
+-rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py
+-rw-r--r--   0        0        0     1468 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py
+-rw-r--r--   0        0        0     1195 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_request.py
+-rw-r--r--   0        0        0     3140 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship.py
+-rw-r--r--   0        0        0     1484 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_cargo.py
+-rw-r--r--   0        0        0     1510 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_cargo_item.py
+-rw-r--r--   0        0        0     2248 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_crew.py
+-rw-r--r--   0        0        0      167 2023-05-15 19:23:15.727370 spacetraders-0.4.0/spacetraders/models/ship_crew_rotation.py
+-rw-r--r--   0        0        0     1883 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_engine.py
+-rw-r--r--   0        0        0      319 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_engine_symbol.py
+-rw-r--r--   0        0        0     2278 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_frame.py
+-rw-r--r--   0        0        0      694 2023-05-15 19:23:15.737370 spacetraders-0.4.0/spacetraders/models/ship_frame_symbol.py
+-rw-r--r--   0        0        0     1586 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_fuel.py
+-rw-r--r--   0        0        0     1340 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_fuel_consumed.py
+-rw-r--r--   0        0        0     1965 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_module.py
+-rw-r--r--   0        0        0     1033 2023-05-15 19:23:15.777370 spacetraders-0.4.0/spacetraders/models/ship_module_symbol.py
+-rw-r--r--   0        0        0     1947 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_mount.py
+-rw-r--r--   0        0        0      572 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_mount_deposits_item.py
+-rw-r--r--   0        0        0      854 2023-05-15 19:23:15.847370 spacetraders-0.4.0/spacetraders/models/ship_mount_symbol.py
+-rw-r--r--   0        0        0     2114 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_nav.py
+-rw-r--r--   0        0        0      206 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/ship_nav_flight_mode.py
+-rw-r--r--   0        0        0     1891 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_nav_route.py
+-rw-r--r--   0        0        0     1497 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_nav_route_waypoint.py
+-rw-r--r--   0        0        0      196 2023-05-15 19:23:15.767370 spacetraders-0.4.0/spacetraders/models/ship_nav_status.py
+-rw-r--r--   0        0        0     1934 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_reactor.py
+-rw-r--r--   0        0        0      344 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/ship_reactor_symbol.py
+-rw-r--r--   0        0        0     1246 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_refine_json_body.py
+-rw-r--r--   0        0        0      330 2023-05-15 19:23:15.837370 spacetraders-0.4.0/spacetraders/models/ship_refine_json_body_produce.py
+-rw-r--r--   0        0        0     1316 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response.py
+-rw-r--r--   0        0        0     2047 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py
+-rw-r--r--   0        0        0     1344 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py
+-rw-r--r--   0        0        0     1344 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py
+-rw-r--r--   0        0        0     1477 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/ship_registration.py
+-rw-r--r--   0        0        0     1541 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/ship_requirements.py
+-rw-r--r--   0        0        0      479 2023-05-15 19:23:15.827370 spacetraders-0.4.0/spacetraders/models/ship_role.py
+-rw-r--r--   0        0        0      549 2023-05-15 19:23:15.737370 spacetraders-0.4.0/spacetraders/models/ship_type.py
+-rw-r--r--   0        0        0     2009 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard.py
+-rw-r--r--   0        0        0     2498 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard_ship.py
+-rw-r--r--   0        0        0     1225 2023-05-15 19:23:17.137370 spacetraders-0.4.0/spacetraders/models/shipyard_ship_types_item.py
+-rw-r--r--   0        0        0     1698 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/shipyard_transaction.py
+-rw-r--r--   0        0        0     2228 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/survey.py
+-rw-r--r--   0        0        0     1209 2023-05-15 19:23:17.167370 spacetraders-0.4.0/spacetraders/models/survey_deposit.py
+-rw-r--r--   0        0        0      181 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/survey_size.py
+-rw-r--r--   0        0        0     1725 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system.py
+-rw-r--r--   0        0        0     1112 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system_faction.py
+-rw-r--r--   0        0        0      405 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/system_type.py
+-rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/system_waypoint.py
+-rw-r--r--   0        0        0     1299 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/trade_good.py
+-rw-r--r--   0        0        0     4422 2023-05-15 19:23:15.827370 spacetraders-0.4.0/spacetraders/models/trade_symbol.py
+-rw-r--r--   0        0        0     1352 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py
+-rw-r--r--   0        0        0     1221 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py
+-rw-r--r--   0        0        0     1304 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py
+-rw-r--r--   0        0        0     1168 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/warp_ship_json_body.py
+-rw-r--r--   0        0        0     1233 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/warp_ship_response_200.py
+-rw-r--r--   0        0        0     1436 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/warp_ship_response_200_data.py
+-rw-r--r--   0        0        0     2279 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/waypoint.py
+-rw-r--r--   0        0        0     1116 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/waypoint_faction.py
+-rw-r--r--   0        0        0     1178 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/models/waypoint_orbital.py
+-rw-r--r--   0        0        0     1427 2023-05-15 19:23:17.147370 spacetraders-0.4.0/spacetraders/models/waypoint_trait.py
+-rw-r--r--   0        0        0     2200 2023-05-15 19:23:15.857370 spacetraders-0.4.0/spacetraders/models/waypoint_trait_symbol.py
+-rw-r--r--   0        0        0      381 2023-05-15 19:23:15.747370 spacetraders-0.4.0/spacetraders/models/waypoint_type.py
+-rw-r--r--   0        0        0     1341 2023-05-15 19:23:17.157370 spacetraders-0.4.0/spacetraders/types.py
+-rw-r--r--   0        0        0     4031 1970-01-01 00:00:00.000000 spacetraders-0.4.0/PKG-INFO
```

### Comparing `spacetraders-0.3.0/README.md` & `spacetraders-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/pyproject.toml` & `spacetraders-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spacetraders"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python API for Space Traders"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "spacetraders"}]
 
 [tool.poetry.dependencies]
```

### Comparing `spacetraders-0.3.0/spacetraders/api/agents/get_my_agent.py` & `spacetraders-0.4.0/spacetraders/api/agents/get_my_agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/contracts/accept_contract.py` & `spacetraders-0.4.0/spacetraders/api/contracts/accept_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/contracts/deliver_contract.py` & `spacetraders-0.4.0/spacetraders/api/contracts/deliver_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/contracts/fulfill_contract.py` & `spacetraders-0.4.0/spacetraders/api/contracts/fulfill_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/contracts/get_contract.py` & `spacetraders-0.4.0/spacetraders/api/contracts/get_contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/contracts/get_contracts.py` & `spacetraders-0.4.0/spacetraders/api/contracts/get_contracts.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/default/register.py` & `spacetraders-0.4.0/spacetraders/api/default/register.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/factions/get_faction.py` & `spacetraders-0.4.0/spacetraders/api/factions/get_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/factions/get_factions.py` & `spacetraders-0.4.0/spacetraders/api/factions/get_factions.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/create_chart.py` & `spacetraders-0.4.0/spacetraders/api/fleet/create_chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/create_ship_ship_scan.py` & `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_ship_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/create_ship_system_scan.py` & `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_system_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/create_ship_waypoint_scan.py` & `spacetraders-0.4.0/spacetraders/api/fleet/create_ship_waypoint_scan.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/create_survey.py` & `spacetraders-0.4.0/spacetraders/api/fleet/create_survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/dock_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/dock_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/extract_resources.py` & `spacetraders-0.4.0/spacetraders/api/fleet/extract_resources.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/get_my_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/get_my_ship_cargo.py` & `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/get_my_ships.py` & `spacetraders-0.4.0/spacetraders/api/fleet/get_my_ships.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/get_ship_cooldown.py` & `spacetraders-0.4.0/spacetraders/api/fleet/get_ship_cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/get_ship_nav.py` & `spacetraders-0.4.0/spacetraders/api/fleet/get_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/jettison.py` & `spacetraders-0.4.0/spacetraders/api/fleet/jettison.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/jump_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/jump_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/navigate_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/navigate_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/orbit_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/orbit_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/patch_ship_nav.py` & `spacetraders-0.4.0/spacetraders/api/fleet/patch_ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/purchase_cargo.py` & `spacetraders-0.4.0/spacetraders/api/fleet/purchase_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/purchase_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/purchase_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/refuel_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/refuel_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/sell_cargo.py` & `spacetraders-0.4.0/spacetraders/api/fleet/sell_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/ship_refine.py` & `spacetraders-0.4.0/spacetraders/api/fleet/ship_refine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/transfer_cargo.py` & `spacetraders-0.4.0/spacetraders/api/fleet/transfer_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/fleet/warp_ship.py` & `spacetraders-0.4.0/spacetraders/api/fleet/warp_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_jump_gate.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_market.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_shipyard.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_waypoint.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_shipyard_response_200 import GetShipyardResponse200
+from ...models.get_waypoint_response_200 import GetWaypointResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -31,57 +31,57 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetShipyardResponse200]:
+) -> Optional[GetWaypointResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetShipyardResponse200(**response.json())
+        response_200 = GetWaypointResponse200(**response.json())
 
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
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
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
         _client=_client,
     )
@@ -120,29 +120,29 @@
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetShipyardResponse200]:
-    """Get Shipyard
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
         _client=_client,
     )
```

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_system.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_system_waypoints.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_system_waypoints.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_systems.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_systems.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/api/systems/get_waypoint.py` & `spacetraders-0.4.0/spacetraders/api/systems/get_shipyard.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 from http import HTTPStatus
 from typing import Any, Dict, Optional
 
 import httpx
 
 from ... import errors
 from ...client import AuthenticatedClient, Client
-from ...models.get_waypoint_response_200 import GetWaypointResponse200
+from ...models.get_shipyard_response_200 import GetShipyardResponse200
 from ...types import ApiError, Error, Response
 
 
 def _get_kwargs(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
 ) -> Dict[str, Any]:
-    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}".format(
+    url = "{}/systems/{systemSymbol}/waypoints/{waypointSymbol}/shipyard".format(
         _client.base_url, systemSymbol=system_symbol, waypointSymbol=waypoint_symbol
     )
 
     headers: Dict[str, str] = _client.get_headers()
     cookies: Dict[str, Any] = _client.get_cookies()
 
     return {
@@ -31,57 +31,58 @@
         "timeout": _client.get_timeout(),
         "follow_redirects": _client.follow_redirects,
     }
 
 
 def _parse_response(
     *, client: Client, response: httpx.Response
-) -> Optional[GetWaypointResponse200]:
+) -> Optional[GetShipyardResponse200]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetWaypointResponse200(**response.json())
+        response_200 = GetShipyardResponse200(**response.json())
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
 def _build_response(
     *, client: Client, response: httpx.Response
-) -> Response[GetWaypointResponse200]:
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
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetWaypointResponse200]:
-    """Get Waypoint
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     View the details of a waypoint.
+     Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
+    available for purchase and recent transactions.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetWaypointResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
@@ -120,29 +121,30 @@
 
 async def asyncio_detailed(
     system_symbol: str,
     waypoint_symbol: str,
     *,
     _client: AuthenticatedClient,
     raise_on_error: Optional[bool] = None,
-) -> Response[GetWaypointResponse200]:
-    """Get Waypoint
+) -> Response[GetShipyardResponse200]:
+    """Get Shipyard
 
-     View the details of a waypoint.
+     Get the shipyard for a waypoint. Send a ship to the waypoint to access ships that are currently
+    available for purchase and recent transactions.
 
     Args:
         system_symbol (str):
         waypoint_symbol (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetWaypointResponse200]
+        Response[GetShipyardResponse200]
     """
 
     kwargs = _get_kwargs(
         system_symbol=system_symbol,
         waypoint_symbol=waypoint_symbol,
         _client=_client,
     )
```

### Comparing `spacetraders-0.3.0/spacetraders/client.py` & `spacetraders-0.4.0/spacetraders/client.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/__init__.py` & `spacetraders-0.4.0/spacetraders/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/accept_contract_response_200.py` & `spacetraders-0.4.0/spacetraders/models/accept_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/accept_contract_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/accept_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/agent.py` & `spacetraders-0.4.0/spacetraders/models/agent.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/chart.py` & `spacetraders-0.4.0/spacetraders/models/chart.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/connected_system.py` & `spacetraders-0.4.0/spacetraders/models/connected_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/contract.py` & `spacetraders-0.4.0/spacetraders/models/contract.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/contract_deliver_good.py` & `spacetraders-0.4.0/spacetraders/models/contract_deliver_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/contract_payment.py` & `spacetraders-0.4.0/spacetraders/models/contract_payment.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/contract_terms.py` & `spacetraders-0.4.0/spacetraders/models/contract_terms.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/cooldown.py` & `spacetraders-0.4.0/spacetraders/models/cooldown.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_chart_response_201.py` & `spacetraders-0.4.0/spacetraders/models/create_chart_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_chart_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/create_chart_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_ship_scan_response_201.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_ship_scan_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_ship_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_system_scan_response_201.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_system_scan_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_system_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_waypoint_scan_response_201.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/create_ship_waypoint_scan_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_survey_response_201.py` & `spacetraders-0.4.0/spacetraders/models/create_survey_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/create_survey_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/create_survey_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/deliver_contract_json_body.py` & `spacetraders-0.4.0/spacetraders/models/deliver_contract_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/deliver_contract_response_200.py` & `spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/deliver_contract_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/deliver_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/dock_ship_dock_ship_200_response.py` & `spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py` & `spacetraders-0.4.0/spacetraders/models/dock_ship_dock_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/extract_resources_json_body.py` & `spacetraders-0.4.0/spacetraders/models/extract_resources_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/extract_resources_response_201.py` & `spacetraders-0.4.0/spacetraders/models/extract_resources_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/extract_resources_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/extract_resources_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/extraction.py` & `spacetraders-0.4.0/spacetraders/models/extraction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/extraction_yield.py` & `spacetraders-0.4.0/spacetraders/models/extraction_yield.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/faction.py` & `spacetraders-0.4.0/spacetraders/models/faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/faction_trait.py` & `spacetraders-0.4.0/spacetraders/models/faction_trait.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/faction_trait_symbol.py` & `spacetraders-0.4.0/spacetraders/models/faction_trait_symbol.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 from enum import Enum
 
 
 class FactionTraitSymbol(str, Enum):
     ADAPTABLE = "ADAPTABLE"
     AGGRESSIVE = "AGGRESSIVE"
-    ANARCHIST = "ANARCHIST"
-    AUTHORITARIAN = "AUTHORITARIAN"
     BOLD = "BOLD"
     BRUTAL = "BRUTAL"
     BUREAUCRATIC = "BUREAUCRATIC"
     CAPITALISTIC = "CAPITALISTIC"
     CLAN = "CLAN"
     COLLABORATIVE = "COLLABORATIVE"
     COMMERCIAL = "COMMERCIAL"
-    CONFLICTED = "CONFLICTED"
     COOPERATIVE = "COOPERATIVE"
     CURIOUS = "CURIOUS"
     DARING = "DARING"
-    DECENTRALIZED = "DECENTRALIZED"
     DEFENSIVE = "DEFENSIVE"
-    DEMOCRACTIC = "DEMOCRACTIC"
     DEXTEROUS = "DEXTEROUS"
     DISTRUSTFUL = "DISTRUSTFUL"
     DIVERSE = "DIVERSE"
     DOMINANT = "DOMINANT"
     DOMINION = "DOMINION"
-    DYNASTIC = "DYNASTIC"
     ENTREPRENEURIAL = "ENTREPRENEURIAL"
     ESTABLISHED = "ESTABLISHED"
     EXILES = "EXILES"
     EXPLORATORY = "EXPLORATORY"
     FLEETING = "FLEETING"
     FLEXIBLE = "FLEXIBLE"
     FORSAKEN = "FORSAKEN"
@@ -43,15 +37,14 @@
     INESCAPABLE = "INESCAPABLE"
     INNOVATIVE = "INNOVATIVE"
     INTELLIGENT = "INTELLIGENT"
     ISOLATED = "ISOLATED"
     LOCALIZED = "LOCALIZED"
     MILITARISTIC = "MILITARISTIC"
     NOTABLE = "NOTABLE"
-    OLIGARCHICAL = "OLIGARCHICAL"
     PEACEFUL = "PEACEFUL"
     PIRATES = "PIRATES"
     PROGRESSIVE = "PROGRESSIVE"
     PROUD = "PROUD"
     RAIDERS = "RAIDERS"
     REBELLIOUS = "REBELLIOUS"
     RESEARCH_FOCUSED = "RESEARCH_FOCUSED"
```

### Comparing `spacetraders-0.3.0/spacetraders/models/fulfill_contract_response_200.py` & `spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/fulfill_contract_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/fulfill_contract_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_contract_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_contract_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_contracts_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_contracts_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_faction_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_faction_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_factions_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_factions_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_jump_gate_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_jump_gate_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_market_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_market_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_my_agent_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_my_agent_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_my_ship_cargo_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_my_ship_cargo_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_my_ship_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_my_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_my_ships_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_my_ships_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_ship_cooldown_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_ship_cooldown_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_ship_nav_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_shipyard_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_shipyard_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_system_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_system_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_system_waypoints_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_system_waypoints_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_systems_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_systems_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/get_waypoint_response_200.py` & `spacetraders-0.4.0/spacetraders/models/get_waypoint_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jettison_json_body.py` & `spacetraders-0.4.0/spacetraders/models/jettison_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jettison_response_200.py` & `spacetraders-0.4.0/spacetraders/models/jettison_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jettison_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/jettison_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jump_gate.py` & `spacetraders-0.4.0/spacetraders/models/jump_gate.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jump_ship_json_body.py` & `spacetraders-0.4.0/spacetraders/models/jump_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jump_ship_response_200.py` & `spacetraders-0.4.0/spacetraders/models/jump_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/jump_ship_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/jump_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/market.py` & `spacetraders-0.4.0/spacetraders/models/market.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/market_trade_good.py` & `spacetraders-0.4.0/spacetraders/models/market_trade_good.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/market_transaction.py` & `spacetraders-0.4.0/spacetraders/models/market_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/meta.py` & `spacetraders-0.4.0/spacetraders/models/meta.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/navigate_ship_json_body.py` & `spacetraders-0.4.0/spacetraders/models/navigate_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/navigate_ship_response_200.py` & `spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/navigate_ship_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/navigate_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py` & `spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py` & `spacetraders-0.4.0/spacetraders/models/orbit_ship_orbit_ship_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/patch_ship_nav_json_body.py` & `spacetraders-0.4.0/spacetraders/models/patch_ship_nav_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/patch_ship_nav_response_200.py` & `spacetraders-0.4.0/spacetraders/models/patch_ship_nav_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py` & `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py` & `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py` & `spacetraders-0.4.0/spacetraders/models/purchase_cargo_purchase_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_ship_json_body.py` & `spacetraders-0.4.0/spacetraders/models/purchase_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_ship_response_201.py` & `spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/purchase_ship_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/purchase_ship_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/refuel_ship_response_200.py` & `spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/refuel_ship_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/refuel_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/register_json_body.py` & `spacetraders-0.4.0/spacetraders/models/trade_good.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,29 +3,31 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.register_json_body_faction import RegisterJsonBodyFaction
+from ..models.trade_symbol import TradeSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="RegisterJsonBody")
+T = TypeVar("T", bound="TradeGood")
 
 
-class RegisterJsonBody(BaseModel):
+class TradeGood(BaseModel):
     """
     Attributes:
-        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
-        symbol (str): How other agents will see your ships and information. Example: BADGER.
+        symbol (TradeSymbol):
+        name (str):
+        description (str):
     """
 
-    faction: RegisterJsonBodyFaction = Field(alias="faction")
-    symbol: str = Field(alias="symbol")
+    symbol: TradeSymbol = Field(alias="symbol")
+    name: str = Field(alias="name")
+    description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.3.0/spacetraders/models/register_response_201.py` & `spacetraders-0.4.0/spacetraders/models/register_response_201.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/register_response_201_data.py` & `spacetraders-0.4.0/spacetraders/models/register_response_201_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_ship.py` & `spacetraders-0.4.0/spacetraders/models/scanned_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_ship_engine.py` & `spacetraders-0.4.0/spacetraders/models/scanned_ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_ship_frame.py` & `spacetraders-0.4.0/spacetraders/models/scanned_ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_ship_mounts_item.py` & `spacetraders-0.4.0/spacetraders/models/scanned_ship_mounts_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_ship_reactor.py` & `spacetraders-0.4.0/spacetraders/models/scanned_ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_system.py` & `spacetraders-0.4.0/spacetraders/models/scanned_system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/scanned_waypoint.py` & `spacetraders-0.4.0/spacetraders/models/scanned_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py` & `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py` & `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_201_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/sell_cargo_sell_cargo_request.py` & `spacetraders-0.4.0/spacetraders/models/sell_cargo_sell_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship.py` & `spacetraders-0.4.0/spacetraders/models/ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_cargo.py` & `spacetraders-0.4.0/spacetraders/models/ship_cargo.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_cargo_item.py` & `spacetraders-0.4.0/spacetraders/models/ship_cargo_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_crew.py` & `spacetraders-0.4.0/spacetraders/models/ship_crew.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_engine.py` & `spacetraders-0.4.0/spacetraders/models/ship_engine.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_frame.py` & `spacetraders-0.4.0/spacetraders/models/ship_frame.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_frame_symbol.py` & `spacetraders-0.4.0/spacetraders/models/ship_frame_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_fuel.py` & `spacetraders-0.4.0/spacetraders/models/ship_fuel.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_fuel_consumed.py` & `spacetraders-0.4.0/spacetraders/models/ship_fuel_consumed.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_module.py` & `spacetraders-0.4.0/spacetraders/models/ship_module.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_module_symbol.py` & `spacetraders-0.4.0/spacetraders/models/ship_module_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_mount.py` & `spacetraders-0.4.0/spacetraders/models/ship_mount.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_mount_deposits_item.py` & `spacetraders-0.4.0/spacetraders/models/ship_mount_deposits_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_mount_symbol.py` & `spacetraders-0.4.0/spacetraders/models/ship_mount_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_nav.py` & `spacetraders-0.4.0/spacetraders/models/ship_nav.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_nav_route.py` & `spacetraders-0.4.0/spacetraders/models/ship_nav_route.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_nav_route_waypoint.py` & `spacetraders-0.4.0/spacetraders/models/ship_nav_route_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_reactor.py` & `spacetraders-0.4.0/spacetraders/models/ship_reactor.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_refine_json_body.py` & `spacetraders-0.4.0/spacetraders/models/ship_refine_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response.py` & `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py` & `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py` & `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_consumed_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py` & `spacetraders-0.4.0/spacetraders/models/ship_refine_ship_refine_200_response_data_produced_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_registration.py` & `spacetraders-0.4.0/spacetraders/models/register_json_body.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,32 +4,31 @@
     List,
     TypeVar,
     Union,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.ship_role import ShipRole
+from ..models.register_json_body_faction import RegisterJsonBodyFaction
 from ..types import UNSET, Unset
 
-T = TypeVar("T", bound="ShipRegistration")
+T = TypeVar("T", bound="RegisterJsonBody")
 
 
-class ShipRegistration(BaseModel):
-    """The public registration information of the ship
-
+class RegisterJsonBody(BaseModel):
+    """
     Attributes:
-        name (str): The agent's registered name of the ship
-        role (ShipRole): The registered role of the ship
-        faction_symbol (Union[Unset, str]): The symbol of the faction the ship is registered with
+        faction (RegisterJsonBodyFaction): The faction you choose determines your headquarters.
+        symbol (str): How other agents will see your ships and information. Example: BADGER.
+        email (Union[Unset, str]): Your email address. This is used if you reserved your call sign between resets.
     """
 
-    name: str = Field(alias="name")
-    role: ShipRole = Field(alias="role")
-    faction_symbol: Union[Unset, str] = Field(UNSET, alias="factionSymbol")
+    faction: RegisterJsonBodyFaction = Field(alias="faction")
+    symbol: str = Field(alias="symbol")
+    email: Union[Unset, str] = Field(UNSET, alias="email")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
 
     def dict(self, *args, **kwargs):
```

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_requirements.py` & `spacetraders-0.4.0/spacetraders/models/ship_requirements.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/ship_type.py` & `spacetraders-0.4.0/spacetraders/models/ship_type.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/shipyard.py` & `spacetraders-0.4.0/spacetraders/models/shipyard.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/shipyard_ship.py` & `spacetraders-0.4.0/spacetraders/models/shipyard_ship.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/shipyard_ship_types_item.py` & `spacetraders-0.4.0/spacetraders/models/shipyard_ship_types_item.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/shipyard_transaction.py` & `spacetraders-0.4.0/spacetraders/models/shipyard_transaction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/survey.py` & `spacetraders-0.4.0/spacetraders/models/survey.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/survey_deposit.py` & `spacetraders-0.4.0/spacetraders/models/survey_deposit.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/system.py` & `spacetraders-0.4.0/spacetraders/models/system.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/system_faction.py` & `spacetraders-0.4.0/spacetraders/models/system_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/system_waypoint.py` & `spacetraders-0.4.0/spacetraders/models/system_waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/trade_good.py` & `spacetraders-0.4.0/spacetraders/models/waypoint_trait.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,29 +3,29 @@
     Dict,
     List,
     TypeVar,
 )
 
 from pydantic import BaseModel, Field
 
-from ..models.trade_symbol import TradeSymbol
+from ..models.waypoint_trait_symbol import WaypointTraitSymbol
 from ..types import Unset
 
-T = TypeVar("T", bound="TradeGood")
+T = TypeVar("T", bound="WaypointTrait")
 
 
-class TradeGood(BaseModel):
+class WaypointTrait(BaseModel):
     """
     Attributes:
-        symbol (TradeSymbol):
-        name (str):
-        description (str):
+        symbol (WaypointTraitSymbol): The unique identifier of the trait.
+        name (str): The name of the trait.
+        description (str): A description of the trait.
     """
 
-    symbol: TradeSymbol = Field(alias="symbol")
+    symbol: WaypointTraitSymbol = Field(alias="symbol")
     name: str = Field(alias="name")
     description: str = Field(alias="description")
     additional_properties: Dict[str, Any] = {}
 
     class Config:
         arbitrary_types_allowed = True
         allow_population_by_field_name = True
```

### Comparing `spacetraders-0.3.0/spacetraders/models/trade_symbol.py` & `spacetraders-0.4.0/spacetraders/models/trade_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py` & `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py` & `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_200_response_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py` & `spacetraders-0.4.0/spacetraders/models/transfer_cargo_transfer_cargo_request.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/warp_ship_json_body.py` & `spacetraders-0.4.0/spacetraders/models/warp_ship_json_body.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/warp_ship_response_200.py` & `spacetraders-0.4.0/spacetraders/models/warp_ship_response_200.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/warp_ship_response_200_data.py` & `spacetraders-0.4.0/spacetraders/models/warp_ship_response_200_data.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/waypoint.py` & `spacetraders-0.4.0/spacetraders/models/waypoint.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/waypoint_faction.py` & `spacetraders-0.4.0/spacetraders/models/waypoint_faction.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/waypoint_orbital.py` & `spacetraders-0.4.0/spacetraders/models/waypoint_orbital.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/models/waypoint_trait_symbol.py` & `spacetraders-0.4.0/spacetraders/models/waypoint_trait_symbol.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/spacetraders/types.py` & `spacetraders-0.4.0/spacetraders/types.py`

 * *Files identical despite different names*

### Comparing `spacetraders-0.3.0/PKG-INFO` & `spacetraders-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetraders
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python API for Space Traders
 License: Apache-2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

