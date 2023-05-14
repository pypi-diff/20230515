# Comparing `tmp/FreeTAKServer-2.0.21.tar.gz` & `tmp/FreeTAKServer-2.0.66.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTAKServer-2.0.21.tar", last modified: Sat Mar 18 20:56:55 2023, max compression
+gzip compressed data, was "FreeTAKServer-2.0.66.tar", last modified: Sun May 14 22:50:48 2023, max compression
```

## Comparing `FreeTAKServer-2.0.21.tar` & `FreeTAKServer-2.0.66.tar`

### file list

```diff
@@ -1,735 +1,1351 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.117326 FreeTAKServer-2.0.21/FreeTAKServer/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.117326 FreeTAKServer-2.0.21/FreeTAKServer/components/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.117326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/cot_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/cot_property.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/telemetry_exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/core_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/abstract_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/main_cot_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/xml_element.py
--rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/xml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/domain_action_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/domain_health_check.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/domain_metrics_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/business_rules/serialization_business_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/domain_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/external_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/manifest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/cot2525_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/dict_to_node_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/abstract_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_element.py
--rw-r--r--   0 runner    (1001) docker     (123)     5140 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serialization_orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.121326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_dest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_emergency.py
--rw-r--r--   0 runner    (1001) docker     (123)     4980 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_event.py
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_marti.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_remarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_usericon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/ContactVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/DetailVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/EmergencyVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/EventVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/LinkVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/PointVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/message_sender/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/message_sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/message_sender/main_message_sender.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/base/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/base/type_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/external_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/manifest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/type_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/caching_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/database_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/mapping_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/memory_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/type_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/type_mapping_strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/persistence/type_mappings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/type_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/type_mapping.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/base/
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/base/xml_serializer_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/external_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/manifest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/component_name.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/type_mapping.json
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/xml_serializer_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/controllers/xml_serialization_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/xml_serializer_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.125326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/base/
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/base/emergency_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_off_business_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_on_business_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/emergency_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/external_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/manifest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/dest_schema.json
--rw-r--r--   0 runner    (1001) docker     (123)    58048 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_alert.json
--rw-r--r--   0 runner    (1001) docker     (123)    28252 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_delete.json
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/type_mapping.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_general_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_off_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_on_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3509 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_sender_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/_emergency.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/model_constants/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/model_constants/EmergencyVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/model_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/emergency_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/base/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.129326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)    20364 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/ExCheckController.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/SendExcheckUpdateController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/CompleteDTG.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistColumn.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistTask.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklists.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/columnName.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/columnType.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/columnWidth.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/creatorCallsign.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/creatorUid.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/description.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/lineBreak.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/model_constants/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/model_constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/number.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/startTime.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/templateName.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklistController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheckController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistTask.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstance.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContents.py
--rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContentsData.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.113326 FreeTAKServer-2.0.21/FreeTAKServer/configuration/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/configuration/routing/
--rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/configuration/routing/action_mapping.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/controllers/services/
--rw-r--r--   0 runner    (1001) docker     (123)    71177 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/controllers/services/FTS.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/controllers/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.133326 FreeTAKServer-2.0.21/FreeTAKServer/core/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.137326 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/
--rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/RestEnumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendChatController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendDeleteVideoStreamController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendEmergencyController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendImageryVideoController.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendPresenceController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendRouteController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSPISensorController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSensorDroneController.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSimpleCoTController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendVideoStreamController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.137326 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendChecklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendCoTAbstractController.py
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendDisconnectController.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendDropPointController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendEmergencyController.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendFederatedCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendGeoChatController.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendHealthCheckController.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendInvalidCoTController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendOtherController.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendPingController.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendTakPongController.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendUserUpdateController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.137326 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/ArgumentConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/ClientReceptionHandlerConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/ClientReceptionLoggingConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/CreateLoggerController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/CreateStartupFilesController.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/DataPackageServerConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/DatabaseConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/LoggingConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)    22779 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/MainConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/OrchestratorConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/ReceiveConnectionsConstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/RestAPIVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/SQLcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/configuration_wizard.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ActiveThreadsController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ClientInformationController.py
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ClientReceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/MainSocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)     7118 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ReceiveConnections.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ReceiveConnectionsProcessController.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/SSLSocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/SendDataController.py
--rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/TCPCoTServiceController.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/TCPSocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/connection/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/base/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/base/cot_management_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/business_rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/business_rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/business_rules/cot_management_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/cot_management_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/external_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/logging.conf
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/manifest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42146 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/deletegeoobject.json
--rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/geoobject.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_general_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_geo_object_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_persistence.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_sender_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/cot_management_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/persistence/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/base/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/base/data_package_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/data_package_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.141326 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/BasicModelInstantiate.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/base/domain_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/domain_facade.py
--rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/domain/object_id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/base/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/base/fts_configuration_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/fts_configuration_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/base/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/base/fts_core_action_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/configuration/internal_action_mapping.ini
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/fts_core_facade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/health/
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/health/HealthCheckController.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/health/ServerStatusController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/health/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/ApplyFullJsonController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/JsonController.py
--rw-r--r--   0 runner    (1001) docker     (123)    14010 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/XMLCoTController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/templateToJsonSerializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/APICallController.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/APIUsersController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/ActiveEmergencysController.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/ActiveFederationsController.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/DataPackageTableController.py
--rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/DatabaseController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/EventTableController.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/FederationsController.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/TableController.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/UserTableController.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/VideoStreamTableController.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/_VideoTableController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/system_user_table_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/table_controllers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/queries/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/SqlAlchemyObjectController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.145326 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/api_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/geo_object_adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/protobuf_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/serializer_abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     9802 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/xml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.149326 FreeTAKServer-2.0.21/FreeTAKServer/core/services/
--rw-r--r--   0 runner    (1001) docker     (123)    22465 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/DataPackageServer.py
--rw-r--r--   0 runner    (1001) docker     (123)    47459 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/Orchestrator.py
--rw-r--r--   0 runner    (1001) docker     (123)    84722 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/RestAPI.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/SSLCoTServiceController.py
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/SSLDataPackageService.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/TCPDataPackageService.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.149326 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/
--rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/FederationClientService.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/Handler.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/external_data_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/federation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/federation_service_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/internal_telemetry_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/services/service_abstracts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.149326 FreeTAKServer-2.0.21/FreeTAKServer/core/telemetry/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/telemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.149326 FreeTAKServer-2.0.21/FreeTAKServer/core/util/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/util/AddDataToCoTList.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/util/certificate_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/core/util/geo_manager_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.153326 FreeTAKServer-2.0.21/FreeTAKServer/model/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ActiveThreads.py
--rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ClientInformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ClientInformationQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/Connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/DataQueue.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/DestList.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.153326 FreeTAKServer-2.0.21/FreeTAKServer/model/Enumerations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/Enumerations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/Enumerations/connectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/Enumerations/serviceTypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.157326 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Chat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Chatgrp.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Checklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ChecklistColumns.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ChecklistDetails.py
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ChecklistTasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Checklists.py
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ConnectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Contact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ContentResource.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/CreatorCallsign.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/CreatorUid.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Description.py
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Dest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Detail.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/DimensionTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Emergency.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/EntityTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    16928 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Filename.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Group.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Hash.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/IdentityTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Link_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Marti.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MimeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Mission.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MissionChange.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MissionChanges.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MissionName.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Name.py
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Point.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Precisionlocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Remarks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Serverdestination.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Size.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/StartTime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Status.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/SubmissionTime.py
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Takv.py
--rw-r--r--   0 runner    (1001) docker     (123)      801 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Track.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Usericon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_Group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_Video.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_medevac_ .py
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_uastool.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/fts_protocol_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.161326 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChatVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChatgrpVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChecklistColumnsVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChecklistDetailsVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChecklistTasksVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChecklistVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ChecklistsVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ColorVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ConnectionEntryVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ContactVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ContentResourceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/CreatorCallsignVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/CreatorUidVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/DescriptionVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/DestVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/DetailVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/EmergencyVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/EventVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/FilenameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/HashVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/KeywordsVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/LinkVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/Link_attrVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MartiVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MimeTypeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MissionChangeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MissionChangesVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MissionNameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/MissionVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/NameVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/PointVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/PrecisionlocationVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/RemarksVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ServerdestinationVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/SizeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/StartTimeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/SubmissionTimeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/SubmitterVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/SummaryVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/TakvVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/TimestampVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ToolVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/TrackVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/TypeVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/UidVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/UsericonVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/_GroupVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/_VideoVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/_uastoolVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/sensorVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/statusVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/FilterGroup.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RawCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RawConnectionInformation.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ReceiveConnectionsProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.165326 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/ChatPost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/DroneSensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Emergency.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/EmergencyDelete.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/EmergencyPost.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/GeoObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/GeoObjectPost.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/ImageryVideo.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Presence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/PresencePost.py
--rw-r--r--   0 runner    (1001) docker     (123)    65028 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/RestEnumerations.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Route.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/RoutePost.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/SPISensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/SimpleAPIMessageAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/SimpleCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Teams.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/VideoStreamDelete.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/rest_message_abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.165326 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/APICalls.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/APIUsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/ActiveEmergencys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.169326 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Archive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Chat.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/CoTTableAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Color.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/ConnectionEntry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Contact.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Dest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Detail.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Emergency.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Link.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Marti.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Point.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Precisionlocation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Remarks.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Serverdestination.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Status.py
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Takv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Track.py
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Uid.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Usericon.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/_Group.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/_Video.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/DataPackage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/Event.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/ExCheckData.py
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/ExCheckKeywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/Root.py
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/User.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/UserConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/VideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/federations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/system_user.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SSLConnection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.169326 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/CoTService.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/CoTServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/ComponentRegistration.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/ComponentRegistrationVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FTS.py
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FTSVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/Federate.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederateClients.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationClientService.py
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationClientServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationServerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationServerServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/IntegrationManagerService.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/IntegrationManagerServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RestAPIService.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RestAPIServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RoutingProxyService.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RoutingProxyServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/SSLCoTService.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/SSLCoTServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/SSLDataPackageService.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/SSLDataPackageVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/TCPDataPackageService.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/TCPDataPackageServiceVariables.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SimpleClient.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SimpleClientVariables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/Presence.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendChecklist.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendDeleteVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendDisconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendDropPoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendEmergency.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendExcheckUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendFederatedCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendGeoChat.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendHealthCheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendImageryVideo.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendInvalidCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendOther.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendPing.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendRoute.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendSPISensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendSensorDrone.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendSimpleCoT.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendTakPong.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendUserUpdate.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendVideoStream.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SpecificCoTAbstract.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/TCPConnection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/User.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/clients.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/detailObject.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/federate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/model/protobuf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobuf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/contact_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/cotevent_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/detail_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/fig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/group_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/precisionlocation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/simple_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takcontrol_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takmessage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takv_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/track_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/socketInformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/MainSocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/SSLServerSocket.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/TCPServerSocket.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/model/testobj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    90971 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/rest_api_service_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/views/base_view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/configuration/ssl_cot_service_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.173326 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/ClientReceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/ReceiveConnections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/SSLSocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/SendDataController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/send_component_data_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/raw_ssl_connection_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/ssl_client_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/ssl_cot_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    53205 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/ssl_cot_service_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/configuration/tcp_cot_service_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/ClientReceptionHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/ReceiveConnections.py
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/SendDataController.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/TCPSocketController.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/send_component_data_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/model/tcp_cot_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    51804 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/tcp_cot_service_main.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/FreeTAKServer/test_nothing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-18 20:56:55.117326 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-03-18 20:56:54.000000 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    36038 2023-03-18 20:56:55.000000 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-18 20:56:54.000000 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-03-18 20:56:54.000000 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-18 20:56:54.000000 FreeTAKServer-2.0.21/FreeTAKServer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-18 20:56:55.177326 FreeTAKServer-2.0.21/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-03-18 20:56:47.000000 FreeTAKServer-2.0.21/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/cot_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/cot_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/telemetry_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/core_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/abstract_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/main_cot_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/xml_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16109 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/xml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/domain_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/domain_health_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/domain_metrics_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/business_rules/serialization_business_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/domain_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/external_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1790 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/manifest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/cot2525_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/dict_to_node_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/abstract_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serialization_orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_dest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_emergency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6050 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_marti.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_remarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_usericon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/ContactVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/DetailVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/EmergencyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/EventVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/LinkVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/PointVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/message_sender/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/message_sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/message_sender/main_message_sender.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.859085 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/base/type_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/external_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/manifest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/type_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/caching_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/database_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/mapping_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/memory_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/type_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/type_mapping_strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/persistence/type_mappings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/type_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/base/xml_serializer_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/external_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/manifest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/component_name.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/type_mapping.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/xml_serializer_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/controllers/xml_serialization_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/xml_serializer_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.863086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/base/companion_parrot_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/base/companion_parrot_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/companion_parrot_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/business_rules/companion_parrot.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/companion_parrot_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/model_definitions/companion_parrot.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13131 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/model_definitions/companion_parrot.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/companion_parrot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/companion_parrot_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/companion_parrot_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/controllers/companion_parrot_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/companion_parrot/domain/model_constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/base/cotmanager_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/base/cotmanager_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/business_rules/cotmanager.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/cotmanager_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.867086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/model_definitions/cotmanager.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/model_definitions/cotmanager.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cot_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cot_query_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cotmanager_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cotmanager_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cotmanager_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/controllers/cotmanager_sender_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/cotmanager_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/cotmanager/domain/model_constants/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/base/emergency_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_off_business_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_on_business_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/emergency_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/external_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/manifest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/dest_schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)    58048 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_alert.json
+-rw-r--r--   0 runner    (1001) docker     (123)    28252 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_delete.json
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4009 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_off_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_on_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.871086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/_emergency.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/model_constants/EmergencyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/emergency_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/persistence/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/base/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)    20364 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/ExCheckController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/SendExcheckUpdateController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7912 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/ex_check_api_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/CompleteDTG.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistColumn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/columnName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/columnType.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/columnWidth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/creatorCallsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/creatorUid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/lineBreak.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.875086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/startTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/templateName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklistController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheckController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistTask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContentsData.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/base/federation_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1926 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/base/federation_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/business_rules/federation.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/federation_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/model_definitions/federation.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13125 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/model_definitions/federation.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9129 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_config_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/controllers/federation_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.879086 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/federation/federation_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/controllers/file_configuration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/files/controllers/file_user_account_management_api_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/base/master_parrot_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/base/master_parrot_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/business_rules/master_parrot.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/master_parrot_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/model_definitions/master_parrot.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/model_definitions/master_parrot.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/master_parrot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/master_parrot_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/master_parrot_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/controllers/master_parrot_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/master_parrot/master_parrot_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.883087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/base/mission_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/base/mission_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/business_rules/mission.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/mission_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/model_definitions/mission.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13122 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/model_definitions/mission.json
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23894 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/mission_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/mission_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/mission_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2938 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/mission_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/controllers/mission_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/mission_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.887087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.891087 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/authorization_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/cert_manager_admin_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/cert_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2599 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/ci_trap_report_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/classification_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/config_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/contact_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/contacts_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/cop_view_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/groups_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/home_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/iconset_icon_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/injection_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/ldap_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/locate_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/map_layers_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/metadata_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/plugin_data_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/plugin_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3921 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/profile_admin_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/profile_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/properties_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/qo_s_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/registration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/security_authentication_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/sequence_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/submission_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3019 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/subscription_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/token_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/uid_search_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/vbm_configuration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/version_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/controllers/video_connection_manager_v2_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.923089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18429 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/announce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6002 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_citrap_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_federatecertificates_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_iconset_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5092 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_authentication_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_caveat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_collection_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_collection_injector_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4803 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_collection_map_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_collection_plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_collection_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_connection_modify_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_entry_integer_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_entry_integer_integer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_entry_string_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_external_mission_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4450 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_federate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_federation_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_federation_outgoing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_input_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4313 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_caveat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5017 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_certificate_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_client_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_connection_info_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_cot_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_entry_string_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_federate_ca_group_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_federate_group_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_mission_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_mission_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_mission_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4937 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_profile_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_profile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_repeatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4616 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_tak_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_token_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_list_uid_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_long.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4451 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_map_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_map_string_collection_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_map_string_integer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_map_string_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_messaging_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_mission_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_mission_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_navigable_set_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_profile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_security_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_cop_hierarchy_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_injector_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_mission_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_mission_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4417 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_set_subscription_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_federate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_input_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4812 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_ldap_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5453 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_outgoing_connection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_remote_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_sorted_set_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_subscription_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_tak_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/api_response_user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9583 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7101 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/authentication_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/base_model_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/caveat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/certificate_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/certificate_signing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/certificate_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4365 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6285 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist_column.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2145 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist_columns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10836 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/checklist_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/citrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/citrap_id_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/classification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7561 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/client_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9839 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24425 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_cert_issuer_dn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_cert_public_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_cert_subject_x500_principal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_read_count.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11272 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_info_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_modify_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7739 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connection_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12995 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/contact_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/contents_missionpackage_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/coordinate_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/coordinate_sequence_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/cop_hierarchy_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/cot_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/crl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14544 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/data_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/delivery_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/dos_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/dos_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/dropfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10457 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4887 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/external_mission_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8610 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federate_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3407 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federate_ca_group_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federate_group_association.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21521 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federation_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9481 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federation_outgoing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federation_port.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/federation_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/feed_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3508 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/ferry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/file_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/file_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9120 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/flowtag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5479 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/geocache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17156 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/geometry_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/geospatial_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5751 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/group_name_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/id_attachment_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/injectionfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/injector_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7145 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/input_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/input_metric_bytes_recieveds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5486 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/input_metric_reads_received.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/latest_sa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27236 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/ldap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/ldap_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/locate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/log_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/map_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7698 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/messaging_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5452 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/microsoft_ca_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20325 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3961 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_add_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_add_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10963 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_disruption_tolerance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_feed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5999 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_role.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/mission_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/missions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/missions_name_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/model_async.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/name_entries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/name_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/name_file_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/name_submit_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/name_submit_body1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22538 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/new_user_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9627 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/outgoing_connection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9755 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/plugin_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18910 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/precision_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/priority.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6789 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/profile_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/profile_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/properties_uid_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/qos.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52451 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/rate_limit_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2637 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/read_rate_limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/remote_contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/remote_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/remote_subscription_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5036 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/repeatable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/repeatable_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/repeater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13807 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11581 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2112 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15533 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/security_config_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/server_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4978 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/simple_group_with_users_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/simple_user_group_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6583 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/streamingbroker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3922 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/submission.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/submit_result_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27003 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/subscription_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/tak_cert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7633 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/tak_server_ca_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/tak_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/thumbnail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/tmp_static_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/token_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/typefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6929 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/uid_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/uid_filename_body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/uid_inject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2120 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/uid_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/urladd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6523 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/user_generation_in_bulk_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/user_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/user_password_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/username_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/v1_tls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/vbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/vbm_configuration_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/version_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/video_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/video_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4151 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/whitelist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6694 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/models/xmpp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.927089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_cert_manager_admin_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_cert_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_ci_trap_report_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_classification_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_config_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_contact_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_contacts_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_cop_view_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_cot_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_cot_query_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10519 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_ex_check_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13763 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_federation_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_federation_config_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_file_configuration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4576 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_file_user_account_management_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_groups_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_home_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_iconset_icon_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_injection_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_ldap_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_locate_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_map_layers_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_metadata_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33621 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_mission_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_plugin_data_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_plugin_manager_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_profile_admin_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_profile_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3009 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_properties_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3096 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_qo_s_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_registration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_repeater_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_security_authentication_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_sequence_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_submission_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_subscription_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_token_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_uid_search_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_vbm_configuration_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_version_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_video_connection_manager_v2_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/test/test_xmpp_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/type_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/swagger_server/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/mission/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.927089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.927089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/base/repeater_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/base/repeater_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/business_rules/repeater.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/model_definitions/repeater.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13123 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/model_definitions/repeater.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/repeater_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/repeater_api_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2171 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/repeater_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/repeater_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/repeater_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/controllers/repeater_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/repeater/repeater_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/base/report_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/base/report_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/business_rules/report.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/model_definitions/report.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13121 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/model_definitions/report.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/report_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.931089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/report_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/report_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/report_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/controllers/report_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2191 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/report/report_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/base/track_manager_action_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/base/track_manager_domain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/business_rules/track_manager.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/model_definitions/track_manager.ini
+-rw-r--r--   0 runner    (1001) docker     (123)    13128 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/model_definitions/track_manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/track_manager_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/configuration/type_mapping.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/track_manager_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/track_manager_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/track_manager_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/controllers/track_manager_sender_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/_component_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/model_constants/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/model_constants/ComponentPropertyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/domain/model_constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/components/extended/track_manager/track_manager_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.835084 FreeTAKServer-2.0.66/FreeTAKServer/configuration/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/configuration/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5430 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/configuration/routing/action_mapping.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/controllers/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    71186 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/controllers/services/FTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/controllers/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.935089 FreeTAKServer-2.0.66/FreeTAKServer/core/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.939089 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/
+-rw-r--r--   0 runner    (1001) docker     (123)    60055 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/RestEnumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendChatController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendDeleteVideoStreamController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendEmergencyController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendImageryVideoController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendPresenceController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2664 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendRouteController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSPISensorController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSensorDroneController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSimpleCoTController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendVideoStreamController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.939089 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendChecklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3854 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendCoTAbstractController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendDisconnectController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendDropPointController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendEmergencyController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendFederatedCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendGeoChatController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendHealthCheckController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendInvalidCoTController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendOtherController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendPingController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendTakPongController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendUserUpdateController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/ArgumentConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/ClientReceptionHandlerConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/ClientReceptionLoggingConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/CreateLoggerController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/CreateStartupFilesController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      925 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/DataPackageServerConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/DatabaseConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7341 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/LoggingConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22950 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/MainConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/OrchestratorConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/ReceiveConnectionsConstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6799 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/RestAPIVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/SQLcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/configuration_wizard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ActiveThreadsController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ClientInformationController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ClientReceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/MainSocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ReceiveConnections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ReceiveConnectionsProcessController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/SSLSocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/SendDataController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5309 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/TCPCoTServiceController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/TCPSocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/connection/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/base/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/base/cot_management_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/business_rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/business_rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/business_rules/cot_management_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/cot_management_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/external_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/logging.conf
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/manifest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.943090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18098 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/base_object.json
+-rw-r--r--   0 runner    (1001) docker     (123)    42146 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/deletegeoobject.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55430 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/geoobject.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_general_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_geo_object_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_private_cot_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_persistence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_sender_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5018 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/cot_management_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/persistence/repeated_messages.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/base/data_package_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/data_package_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/BasicModelInstantiate.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/base/domain_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/domain_facade.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40459 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/domain/object_id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/base/fts_configuration_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/fts_configuration_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/base/fts_core_action_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/configuration/internal_action_mapping.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/fts_core_facade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/health/
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/health/HealthCheckController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/health/ServerStatusController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/health/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.947090 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/ApplyFullJsonController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/JsonController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14011 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/XMLCoTController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/templateToJsonSerializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.951090 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/APICallController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/APIUsersController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/ActiveEmergencysController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/ActiveFederationsController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/DataPackageTableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18952 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/DatabaseController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/EventTableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/FederationsController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/TableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/UserTableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/VideoStreamTableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/_VideoTableController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/system_user_table_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/table_controllers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.951090 FreeTAKServer-2.0.66/FreeTAKServer/core/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.951090 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/SqlAlchemyObjectController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.951090 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/api_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/geo_object_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/protobuf_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/serializer_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/xml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.951090 FreeTAKServer-2.0.66/FreeTAKServer/core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)    23713 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/DataPackageServer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47459 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/Orchestrator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84722 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/RestAPI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/SSLCoTServiceController.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/SSLDataPackageService.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/TCPDataPackageService.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.955090 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14655 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/FederationClientService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/Handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/external_data_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13559 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/federation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/federation_service_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/internal_telemetry_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/services/service_abstracts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.955090 FreeTAKServer-2.0.66/FreeTAKServer/core/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/telemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.955090 FreeTAKServer-2.0.66/FreeTAKServer/core/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/util/AddDataToCoTList.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22416 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/util/certificate_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/core/util/geo_manager_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.955090 FreeTAKServer-2.0.66/FreeTAKServer/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ActiveThreads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1297 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ClientInformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ClientInformationQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/Connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/DataQueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/DestList.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.955090 FreeTAKServer-2.0.66/FreeTAKServer/model/Enumerations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/Enumerations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/Enumerations/connectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/Enumerations/serviceTypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.963091 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Chatgrp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ChecklistColumns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ChecklistDetails.py
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ChecklistTasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Checklists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ConnectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6716 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ContentResource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/CreatorCallsign.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/CreatorUid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Description.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Dest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9886 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/DimensionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Emergency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/EntityTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16928 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Hash.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/IdentityTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Link_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Marti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MimeType.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Mission.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MissionChange.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MissionChanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MissionName.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Precisionlocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Remarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Serverdestination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Size.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/StartTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/SubmissionTime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Takv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Track.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Usericon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_medevac_ .py
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_uastool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/fts_protocol_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.971091 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChatVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChatgrpVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChecklistColumnsVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChecklistDetailsVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChecklistTasksVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChecklistVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ChecklistsVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ColorVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ConnectionEntryVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ContactVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ContentResourceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/CreatorCallsignVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/CreatorUidVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/DescriptionVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/DestVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/DetailVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/EmergencyVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/EventVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/FilenameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/HashVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/KeywordsVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/LinkVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/Link_attrVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MartiVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MimeTypeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MissionChangeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MissionChangesVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MissionNameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/MissionVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/NameVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/PointVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/PrecisionlocationVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/RemarksVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ServerdestinationVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/SizeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/StartTimeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/SubmissionTimeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/SubmitterVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/SummaryVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/TakvVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/TimestampVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ToolVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/TrackVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/TypeVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/UidVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/UsericonVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/_GroupVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/_VideoVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/_uastoolVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/sensorVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/statusVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/FilterGroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RawCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RawConnectionInformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ReceiveConnectionsProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.971091 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/ChatPost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/DroneSensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Emergency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/EmergencyDelete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/EmergencyPost.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/GeoObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/GeoObjectPost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/ImageryVideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/PresencePost.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65028 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/RestEnumerations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/RoutePost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/SPISensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/SimpleAPIMessageAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/SimpleCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/VideoStreamDelete.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/rest_message_abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.975091 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/APICalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/APIUsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/ActiveEmergencys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.975091 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/CoTTableAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Color.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/ConnectionEntry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1650 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Contact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Dest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Detail.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Emergency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Marti.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Precisionlocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Remarks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Serverdestination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Takv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Track.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Usericon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/_Group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/_Video.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/DataPackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/Event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/ExCheckData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/ExCheckKeywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/Root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/UserConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/VideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/federations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/system_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SSLConnection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.979092 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/CoTService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/CoTServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/ComponentRegistration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/ComponentRegistrationVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FTS.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FTSVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/Federate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederateClients.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationClientService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationClientServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationServerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationServerServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/IntegrationManagerService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/IntegrationManagerServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RestAPIService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RestAPIServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RoutingProxyService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RoutingProxyServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/SSLCoTService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/SSLCoTServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/SSLDataPackageService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/SSLDataPackageVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/TCPDataPackageService.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/TCPDataPackageServiceVariables.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SimpleClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SimpleClientVariables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/Presence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendChecklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendDeleteVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendDisconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendDropPoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendEmergency.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendExcheckUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendFederatedCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendGeoChat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendHealthCheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendImageryVideo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendInvalidCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendOther.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendPing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendRoute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendSPISensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendSensorDrone.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendSimpleCoT.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendTakPong.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendUserUpdate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendVideoStream.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SpecificCoTAbstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/TCPConnection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/User.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/detailObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/federate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/model/protobuf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobuf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/contact_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/cotevent_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/detail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40136 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/fig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/group_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/precisionlocation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/simple_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takcontrol_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takmessage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takv_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/track_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/socketInformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/MainSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/SSLServerSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/TCPServerSocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/model/testobj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89830 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/rest_api_service_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3616 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/views/base_view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/views/base_view_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/views/emergency_view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.983092 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/configuration/ssl_cot_service_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7812 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/ClientReceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/ReceiveConnections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/SSLSocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/SendDataController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8776 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/client_connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/client_disconnection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/send_component_data_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/raw_ssl_connection_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/ssl_client_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/ssl_cot_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35574 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/ssl_cot_service_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/configuration/tcp_cot_service_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/ClientReceptionHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7239 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/ReceiveConnections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11360 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/SendDataController.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/TCPSocketController.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/client_connection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6145 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/client_disconnection_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3312 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/send_component_data_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/model/tcp_cot_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35162 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/tcp_cot_service_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/FreeTAKServer/test_nothing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 22:50:48.855085 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-14 22:50:48.000000 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    82487 2023-05-14 22:50:48.000000 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 22:50:48.000000 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-14 22:50:48.000000 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-14 22:50:48.000000 FreeTAKServer-2.0.66/FreeTAKServer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14197 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8129 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6452 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-14 22:50:48.987092 FreeTAKServer-2.0.66/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-14 22:50:36.000000 FreeTAKServer-2.0.66/setup.py
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/domain.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/domain.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/abstract_component/telemetry_exporter.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/abstract_component/telemetry_exporter.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/abstract_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/abstract_serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/main_cot_parser.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/main_cot_parser.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/cot_parser/xml_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/cot_parser/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/base/domain_metrics_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/base/domain_metrics_controller.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """this module contains only the DomainMetricsController class"""
-from digitalpy.component.impl.default_meter_controller import MeterController
+from digitalpy.core.main.impl.default_meter_controller import MeterController
 from ..configuration.domain_constants import COMPONENT_NAME, METRICS_ADDRESS
 
 
 class DomainMetricsController(MeterController):
     """the metrics controller implementation for the domain
     component."""
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/business_rules/serialization_business_rules.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/business_rules/serialization_business_rules.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/domain_constants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/domain_constants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/external_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/external_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/dict_to_node_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/json_serializer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,55 +1,49 @@
-from digitalpy.core.main.controller import Controller
-from digitalpy.core.telemetry.tracer import Tracer
-from digitalpy.core.domain.node import Node
-
-
-class DictToNodeController(Controller):
-    def execute(self, method=None):
-        return getattr(self, method)(**self.request.get_values())
-
-    def convert_dict_to_node(
-        self,
-        dictionary: dict,
-        model_object: Node,
-        tracer: Tracer,
-        object_class_name,
-        **kwargs
-    ):
-        """fill the node object with the values from the dictionary
-
-        Args:
-            dictionary (dict): a dictionary containing key value pairs which match to the given node attributes.
-            model_object (Node): a node object instance with null attributes.
-            tracer (Tracer, optional): a tracer object used for logging which should be passed by the facade. Defaults to None.
-        """
-        with tracer.start_as_current_span("convert_dict_to_node") as span:
-            try:
-                span.add_event(
-                    "serializing " + str(dictionary) + " to node " + str(model_object)
-                )
-                self.response.set_value(
-                    "model_object",
-                    self.serialize(dictionary[object_class_name.lower()], model_object),
-                )
-                span.add_event("serialization completed successfully")
-            except Exception as ex:
-                span.record_exception(ex)
-
-    def serialize(self, dictionary, node):
-        """recursively serialize a single layer of the given dictionary
-        to a node object until a nested dictionary is found"""
-        for key, value in dictionary.items():
-            self.add_value_to_node(key, value, node)
-        return node
-
-    def add_value_to_node(self, key, value, node):
-        """add a value to a node object"""
-
-        if isinstance(value, dict):
-            self.serialize(value, getattr(node, key))
-
-        elif isinstance(value, list):
-            for l_item in value:
-                self.add_value_to_node(key, l_item, node)
+from typing import List
+
+from FreeTAKServer.core.serializers.serializer_abstract import SerializerAbstract
+from FreeTAKServer.model.FTSModel.Event import Event
+
+# TODO: clean up this whole class
+
+class JsonSerializer(SerializerAbstract):
+
+    def from_format_to_fts_object(self, object: dict, FTSObject: Event) -> Event:
+        for key, value in object.items():
+            if type(value) is dict:
+                self._handle_sub_dictionary(FTSObject, key, value)
+            else:
+                self._handle_attribute(FTSObject, key, value)
+        return FTSObject
+
+    def _handle_attribute(self, FTSObject, key, value, expected_class_name=None):
+        # retrieve setter list
+        setters = self._get_fts_object_var_setter(FTSObject, key)
+        # get correct setter
+        setter = self._get_method_in_method_list(setters, expected_class_name)
+        # call setter
+        setter(value)
+
+    def _handle_sub_dictionary(self, FTSObject, name: str, value: dict):
+        for key, value in value.items():
+            if value is dict:
+                self._handle_sub_dictionary(FTSObject, key, value)
+            else:
+                self._handle_attribute(FTSObject, key, value, name)
+
+    def _get_method_in_method_list(self, method_list: List[callable], expected_class_name: str = None) -> callable:
+        if len(method_list) == 1:
+            return method_list[0]
+
+        elif len(method_list) == 0:
+            raise AttributeError(expected_class_name + ' does not have specified attribute')
+
+        elif len(method_list) > 1 and expected_class_name is not None:
+            for method in method_list:
+                if method.__self__.__class__.__name__.lower() == expected_class_name.lower():
+                    return method
+                else:
+                    pass
+            raise AttributeError('invalid json')
+
         else:
-            setattr(node, key.strip("@"), value)
+            raise AttributeError('invalid json')
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/domain.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/domain.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/abstract_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/abstract_serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serialization_orchestrator.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serialization_orchestrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,30 +4,35 @@
 from digitalpy.core.zmanager.response import Response
 from digitalpy.core.zmanager.action_mapper import ActionMapper
 from digitalpy.core.digipy_configuration.configuration import Configuration
 
 from .xml_serializer import XmlSerializer
 from .xml_element import ExtendedElement
 from FreeTAKServer.model.FTSModel.fts_protocol_object import FTSProtocolObject
-
+from ...domain import Domain
 
 class XMLSerializationOrchestrator(Controller):
     def __init__(
         self,
         request: Request,
         response: Response,
-        action_mapper: ActionMapper,
+        sync_action_mapper: ActionMapper,
         configuration: Configuration,
     ):
         super().__init__(
             request=request,
             response=response,
-            action_mapper=action_mapper,
+            action_mapper=sync_action_mapper,
             configuration=configuration,
         )
+        self.domain_controller = Domain(request, response, sync_action_mapper, configuration)
+
+    def initialize(self, request, response):
+        super().initialize(request, response)
+        self.domain_controller.initialize(request, response)
 
     def execute(self, method=None):
         getattr(self, method)(**self.request.get_values())
         return self.response
 
     def node_to_xml(self, model_objects, **kwargs):
         self.response.set_values(kwargs)
@@ -45,19 +50,15 @@
             model_object, self._get_parent
         )
         parser = etree.XMLParser(target=target_xml_to_model_object)
         model_object = etree.XML(xml, parser)
         self.response.set_value("model_object", model_object)
 
     def _get_parent(self, node, type=""):
-        self.request.set_value("node", node)
-        self.request.set_context(type)
-        sub_response = self.execute_sub_action("GetNodeParent")
-        return sub_response.get_value("parent")
-
+        return self.domain_controller.get_parent(node)
 
 class TargetXMLToModel_object:
     def __init__(self, model_object, parent_getter):
         self.internal_parser = etree.XMLParser()
         lookup = etree.ElementDefaultClassLookup(element=ExtendedElement)
         self.internal_parser.set_element_class_lookup(lookup)
         self.model_object = model_object
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/controllers/serialization/xml_serialization/xml_serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/__init__.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_contact.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_contact.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_dest.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_dest.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_detail.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_detail.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_emergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_emergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_event.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_event.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from digitalpy.core.parsing.load_configuration import Configuration
 from .model_constants import EventVariables as vars
 import uuid
 from datetime import datetime as dt
 import datetime
 from FreeTAKServer.components.core.abstract_component.cot_node import CoTNode
 from FreeTAKServer.components.core.abstract_component.cot_property import CoTProperty
+from lxml import etree
 
-
+DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
+DEFAULT_STALE_TIME = 60
 class Event(CoTNode):
     # TODO: fix emergency methods
     # Event.py
     """Python implementation of the Class Event
     # represents a TAK event: this class is instantiated with a standard set of
     #    values.
     # Generated by Enterprise Architect
@@ -22,14 +24,17 @@
     # <?xml version="1.0" encoding="UTF-8" standalone="yes"?><event version="2.0" uid="Linux-ABC.server-ping" type="b-t-f" time="2020-02-14T20:32:31.444Z" start="2020-02-14T20:32:31.444Z" stale="2020-02-15T20:32:31.444Z" how="h-g-i-g-o">
 
     # default constructor
 
     def __init__(self, configuration: Configuration, model, oid=None):
 
         super().__init__(self.__class__.__name__, configuration, model, oid)
+        # modify the xml object to be event instead of Event
+        self.xml = etree.Element(self.__class__.__name__.lower())
+
         self.cot_attributes["version"] = None
         self.cot_attributes["uid"] = None
         self.cot_attributes["type"] = None
         self.cot_attributes["how"] = None
         self.cot_attributes["stale"] = None
         self.cot_attributes["start"] = None
         self.cot_attributes["time"] = None
@@ -57,19 +62,26 @@
         # additional information attached.
         # e.g.  -ping means that this request is a ping
 
         # flag to determine if this event is a Ping, in this case append to the UID
 
     @CoTProperty
     def start(self):
-        return self.cot_attributes.get("start", None)
-
+        start_val = self.cot_attributes.get("start", None)
+        if start_val == None:
+            timer = dt
+            now = timer.utcnow()
+            zulu = now.strftime(DATETIME_FMT)
+            self.cot_attributes["start"] = zulu
+            return zulu
+        else:
+            return start_val
     @start.setter
     def start(self, start=0):
-        DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
+        
         if start == None:
             timer = dt
             now = timer.utcnow()
             zulu = now.strftime(DATETIME_FMT)
             self.cot_attributes["start"] = zulu
         else:
             self.cot_attributes["start"] = start
@@ -100,29 +112,45 @@
 
     @version.setter
     def version(self, version):
         self.cot_attributes["version"] = version
 
     @CoTProperty
     def time(self):
-        return self.cot_attributes.get("time", None)
+        time_val = self.cot_attributes.get("time", None)
+        if time_val == None:
+            timer = dt
+            now = timer.utcnow()
+            zulu = now.strftime(DATETIME_FMT)
+            self.cot_attributes["time"] = zulu
+            return zulu
+        else:
+            return time_val
 
     @time.setter
     def time(self, time=0):
         DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
         if time == None:
             timer = dt
             now = timer.utcnow()
             zulu = now.strftime(DATETIME_FMT)
             self.time = zulu
         else:
             self.cot_attributes["time"] = time
 
     @CoTProperty
     def stale(self):
+        stale_val = self.cot_attributes.get("stale", None)
+        if stale_val == None:
+            timer = dt
+            now = timer.utcnow()
+            zulu = now.strftime(DATETIME_FMT)
+            add = datetime.timedelta(seconds=DEFAULT_STALE_TIME)
+            stale_part = dt.strptime(zulu, DATETIME_FMT) + add
+            self.cot_attributes["stale"] = stale_part.strftime(DATETIME_FMT)
         return self.cot_attributes.get("stale", None)
 
     @stale.setter
     def stale(self, stale=None, staletime=60):
         if stale == None:
             DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
             timer = dt
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_link.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_link.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_marti.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_marti.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,12 +22,12 @@
         super().__init__(self.__class__.__name__, configuration, model)
         self.cot_attributes["dest"] = []
         self.__index = 0
         # self.__firstrun = True
 
     @CoTProperty
     def dest(self):
-        return self.cot_attributes["dest"]
+        return self.get_children_ex(children_type="dest")
 
     @dest.setter
     def dest(self, dest):
-        self.cot_attributes["dest"].append(dest)
+        self.add_child(dest)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_point.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_point.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_remarks.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_remarks.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/_usericon.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/_usericon.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/ContactVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/ContactVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/EventVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/EventVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain/model_constants/LinkVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain/model_constants/LinkVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/domain/domain_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/xml_serializer_facade.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 from digitalpy.core.component_management.impl.default_facade import DefaultFacade
 from FreeTAKServer.core.configuration.MainConfig import MainConfig
-from FreeTAKServer.components.core.domain.configuration.domain_constants import (
+from FreeTAKServer.components.core.xml_serializer.configuration.xml_serializer_constants import (
     ACTION_MAPPING_PATH,
+    TYPE_MAPPINGS,
     LOGGING_CONFIGURATION_PATH,
     INTERNAL_ACTION_MAPPING_PATH,
     MANIFEST_PATH,
 )
 from . import base
 
 config = MainConfig.instance()
 
 
-class Domain(DefaultFacade):
-    """This is the facade class for the domain component, it is responsible
-    for handling all public routing and forwards all requests to the internal routing
+class XmlSerializer(DefaultFacade):
+    """Facade class for the Component component. Responsible for handling all public routing.
+    Forwards all requests to the internal router.
     """
 
     def __init__(
         self,
-        domain_action_mapper,
+        xml_serializer_action_mapper,
         request,
         response,
         configuration,
         tracing_provider_instance=None,
     ):
         super().__init__(
             # the path to the external action mapping
             action_mapping_path=ACTION_MAPPING_PATH,
             # the path to the internal action mapping
             internal_action_mapping_path=INTERNAL_ACTION_MAPPING_PATH,
+            # the type mapping in dictionary form
+            type_mapping=TYPE_MAPPINGS,
             # the path to the logger configuration
             logger_configuration=LOGGING_CONFIGURATION_PATH,
             # the package containing the base classes
             base=base,
             # the component specific action mapper (passed by constructor)
-            action_mapper=domain_action_mapper,
+            action_mapper=xml_serializer_action_mapper,
             # the request object (passed by constructor)
             request=request,
             # the response object (passed by constructor)
             response=response,
             # the configuration object (passed by constructor)
             configuration=configuration,
             # log file path
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/message_sender/main_message_sender.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/message_sender/main_message_sender.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/external_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/external_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/configuration/type_constants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/configuration/type_constants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/mapping_interface.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/mapping_interface.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/controllers/memory_mapping.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/controllers/memory_mapping.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/type/type_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/type/type_facade.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/external_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/external_action_mapping.ini`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 ; Args:
 ;   message (str): xml string to be converted to a dictionary
 
 ; Returns:
 ;   dict (Dict): dictionary representation of the xml string message
 ??XMLToDict = FreeTAKServer.components.core.xml_serializer.xml_serializer_facade.XmlSerializer.XMLToDict
 
+; converts the provided dictionary to an xml string
+; Args:
+;   xml_dict (Dict): dictionary representation of the xml string message
+;
+; Returns:
+;   message (str): dictionary in form of xml string
+??DictToXML = FreeTAKServer.components.core.xml_serializer.xml_serializer_facade.XmlSerializer.DictToXML
+
 ;this action converts the provided node to an xml string
 ;Args:
 ;   node (Node): the node to be serialized to xml
 ;returns message(str)
 ??NodeToXML = FreeTAKServer.components.core.xml_serializer.controllers.xml_serialization_controller.XMLSerializationController.convert_node_to_xml
 
 [XMLSerializer]
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/internal_action_mapping.ini`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 [actionmapping]
 ComponentName??Type = absolute.path.to.xml_serializer.controllers.xml_serializer_controller.ComponentNameController.evaluate_request
 
 ??XMLToDict = FreeTAKServer.components.core.xml_serializer.controllers.xml_serialization_controller.XMLSerializationController.convert_xml_to_dict
 
+??DictToXML = FreeTAKServer.components.core.xml_serializer.controllers.xml_serialization_controller.XMLSerializationController.convert_dict_to_xml
+
 ??BroadcastComponentName = absolute.path.to.xml_serializer.controllers.xml_serializer_sender_controller.ComponentNameSenderController.broadcast_xml_serializer
 
 ??ParseComponentName = absolute.path.to.xml_serializer.controllers.xml_serializer_controller.ComponentNameController.parse_xml_serializer
 
 ??SerializeComponentName = absolute.path.to.xml_serializer.controllers.xml_serializer_general_controller.ComponentNameGeneralController.serialize_xml_serializer
 
 ??NodeToXML = FreeTAKServer.components.core.xml_serializer.controllers.xml_serialization_controller.XMLSerializationController.convert_node_to_xml
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/logging.conf` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/logging.conf`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/component_name.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/model_definitions/component_name.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/configuration/xml_serializer_constants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/configuration/xml_serializer_constants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/controllers/xml_serialization_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/xml_serializer/controllers/xml_serialization_controller.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,22 @@
         """converts the provided xml string to a dictionary
 
         Args:
             message (str): xml string to be converted to a dictionary
         """
         self.response.set_value("dict", xmltodict.parse(message))
 
+    def convert_dict_to_xml(self, xml_dict: dict, **kwargs) -> str:
+        """converts the provided dictionary to an xml string
+
+        Args:
+            xml_dict (dict): a dictionary parsed by xmltodict
+        """
+        self.response.set_value("xml", xmltodict.unparse(xml_dict))
+    
     def convert_node_to_xml(self, node, **kwargs):
         """converts the provided node to an xml string
 
         Args:
             node (Node): the node to be serialized to xml
         """
         self.response.set_value(
@@ -47,25 +55,25 @@
             tag_name (str): the name of the root node class to be serialized
             level (int, optional): _description_. Defaults to 0.
 
         Returns:
             Union[str, Element]: the original call to this method returns a string representing the xml
                 the Element is only returned in the case of recursive calls
         """
-        xml = Element(tag_name)
+        xml = node.xml
         # handles text data within tag
         if hasattr(node, "text"):
             xml.text = node.text
 
         for attribName in node.get_properties():
             # below line is required because get_properties function returns only cot property names
             value = getattr(node, attribName)
             if hasattr(value, "__dict__"):
                 tagElement = self._serialize_node(value, attribName, level=level + 1)
-                # TODO: modify so double underscores are handled differently
+                # T2ODO: modify so double underscores are handled differently
                 try:
                     if attribName[0] == "_":
                         tagElement.tag = "_" + tagElement.tag
                         xml.append(tagElement)
                 except:
                     pass
                 else:
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/core/xml_serializer/xml_serializer_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/emergency_facade.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,42 @@
+#######################################################
+#
+# EmergencyFacade.py
+# Python implementation of the Class Emergency
+# part of Component:
+# Component Version: 1.0
+# Generated by ComponentNameFacade
+# Generated on: 2022-11-18   13:57:53.712997600
+# Author: (Future feature of EA-Bridge)
+#######################################################
+
 from digitalpy.core.component_management.impl.default_facade import DefaultFacade
 from FreeTAKServer.core.configuration.MainConfig import MainConfig
-from FreeTAKServer.components.core.xml_serializer.configuration.xml_serializer_constants import (
+from FreeTAKServer.components.extended.emergency.configuration.emergency_constants import (
     ACTION_MAPPING_PATH,
     TYPE_MAPPINGS,
     LOGGING_CONFIGURATION_PATH,
     INTERNAL_ACTION_MAPPING_PATH,
     MANIFEST_PATH,
+    CONFIGURATION_PATH_TEMPLATE,
 )
 from . import base
 
 config = MainConfig.instance()
 
 
-class XmlSerializer(DefaultFacade):
-    """Facade class for the Component component. Responsible for handling all public routing.
+class Emergency(DefaultFacade):
+    """Facade class for the Component Emergency.
+    Responsible for handling all public routing.
     Forwards all requests to the internal router.
     """
 
     def __init__(
         self,
-        xml_serializer_action_mapper,
+        emergency_action_mapper,
         request,
         response,
         configuration,
         tracing_provider_instance=None,
     ):
         super().__init__(
             # the path to the external action mapping
@@ -33,21 +46,23 @@
             # the type mapping in dictionary form
             type_mapping=TYPE_MAPPINGS,
             # the path to the logger configuration
             logger_configuration=LOGGING_CONFIGURATION_PATH,
             # the package containing the base classes
             base=base,
             # the component specific action mapper (passed by constructor)
-            action_mapper=xml_serializer_action_mapper,
+            action_mapper=emergency_action_mapper,
             # the request object (passed by constructor)
             request=request,
             # the response object (passed by constructor)
             response=response,
             # the configuration object (passed by constructor)
             configuration=configuration,
             # log file path
             log_file_path=config.LogFilePath,
             # the tracing provider used
             tracing_provider_instance=tracing_provider_instance,
+            # the template for the absolute path to the model object definitions
+            configuration_path_template=CONFIGURATION_PATH_TEMPLATE,
             # the path to the manifest file
             manifest_path=MANIFEST_PATH,
         )
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_on_business_rules.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/business_rules/emergency_on_business_rules.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/emergency_constants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/emergency_constants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/external_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/external_action_mapping.ini`

 * *Files 18% similar despite different names*

```diff
@@ -35,14 +35,26 @@
 ;  values:
 ;    uid
 ; Response values:
 ;  values:
 ;    model_object (Node): the uid of an emergency to be deleted
 ??DeleteEmergency = FreeTAKServer.components.extended.emergency.emergency_facade.Emergency.delete_emergency
 
+; this action is exposing an API endpoint and should be called accordingly
+; Request 
+;  action: GetEmergency
+;  context: EmergencyAPI
+;  values:
+;    None
+; Response values:
+;  values:
+;    APIResponse (Dict): json dictionary containing a list of critical information of all emergency's
+?EmergencyAPI?GetEmergency = FreeTAKServer.components.extended.emergency.emergency_facade.Emergency.GetEmergencyAPI
+
+
 [Emergency]
 __class = FreeTAKServer.components.extended.emergency.emergency_facade.Emergency
 
 [Request]
 __class = digitalpy.core.zmanager.impl.default_request.DefaultRequest
 
 [ActionMapper]
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/internal_action_mapping.ini`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,25 @@
 ;  values:
 ;    uid
 ; Response values:
 ;  values:
 ;    model_object (Node): the uid of an emergency to be deleted
 ??DeleteEmergency = FreeTAKServer.components.extended.emergency.controllers.emergency_persistence.EmergencyPersistence.delete_emergency
 
+; this action is exposing an API endpoint and should be called accordingly
+; Request 
+;  action: GetEmergency
+;  context: EmergencyAPI
+;  values:
+;    None
+; Response values:
+;  values:
+;   json dictionary containing a list of critical information of all emergency's
+?EmergencyAPI?GetEmergency = FreeTAKServer.components.extended.emergency.controllers.emergency_api_controller.ManageEmergency.get_emergency
+
 [Request]
 __class = digitalpy.core.zmanager.impl.default_request.DefaultRequest
 
 [ActionMapper]
 __class = digitalpy.core.zmanager.impl.default_action_mapper.DefaultActionMapper
 
 [event_manager]
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/manifest.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/manifest.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/dest_schema.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/dest_schema.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_alert.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_alert.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_delete.json` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/configuration/model_definitions/emergency_delete.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_general_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_general_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_off_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_off_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_on_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_on_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_persistence.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_persistence.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                 json.dump(self._persistence, f)
 
         # load the mapping persistence into memory
         with open(PERSISTENCE_PATH, mode="r+", encoding="utf-8") as f:
             self._persistence = json.load(f)
             self.emergencies = self._persistence["emergencies"]
 
+        super().__init__(request, response, action_mapper, configuration)
     def execute(self, method=None):
         getattr(self, method)(**self.request.get_values())
         return self.response
 
     def save_emergency(self, model_object, **kwargs) -> None:
         """this method adds a new emergency to the list of emergencies
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/controllers/emergency_sender_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/controllers/emergency_sender_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/domain/_emergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/emergency/domain/_emergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/emergency/emergency_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/core/domain/domain_facade.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,85 @@
-#######################################################
-#
-# EmergencyFacade.py
-# Python implementation of the Class Emergency
-# part of Component:
-# Component Version: 1.0
-# Generated by ComponentNameFacade
-# Generated on: 2022-11-18   13:57:53.712997600
-# Author: (Future feature of EA-Bridge)
-#######################################################
-
 from digitalpy.core.component_management.impl.default_facade import DefaultFacade
 from FreeTAKServer.core.configuration.MainConfig import MainConfig
-from FreeTAKServer.components.extended.emergency.configuration.emergency_constants import (
+from FreeTAKServer.components.core.domain.configuration.domain_constants import (
     ACTION_MAPPING_PATH,
-    TYPE_MAPPINGS,
     LOGGING_CONFIGURATION_PATH,
     INTERNAL_ACTION_MAPPING_PATH,
     MANIFEST_PATH,
-    CONFIGURATION_PATH_TEMPLATE,
 )
+
+from .controllers.dict_to_node_controller import DictToNodeController
+from .controllers.domain import Domain as DomainController
 from . import base
 
 config = MainConfig.instance()
 
 
-class Emergency(DefaultFacade):
-    """Facade class for the Component Emergency.
-    Responsible for handling all public routing.
-    Forwards all requests to the internal router.
+class Domain(DefaultFacade):
+    """This is the facade class for the domain component, it is responsible
+    for handling all public routing and forwards all requests to the internal routing
     """
 
     def __init__(
         self,
-        emergency_action_mapper,
+        sync_action_mapper,
         request,
         response,
         configuration,
         tracing_provider_instance=None,
     ):
         super().__init__(
             # the path to the external action mapping
             action_mapping_path=ACTION_MAPPING_PATH,
             # the path to the internal action mapping
             internal_action_mapping_path=INTERNAL_ACTION_MAPPING_PATH,
-            # the type mapping in dictionary form
-            type_mapping=TYPE_MAPPINGS,
             # the path to the logger configuration
             logger_configuration=LOGGING_CONFIGURATION_PATH,
             # the package containing the base classes
             base=base,
             # the component specific action mapper (passed by constructor)
-            action_mapper=emergency_action_mapper,
+            action_mapper=sync_action_mapper,
             # the request object (passed by constructor)
             request=request,
             # the response object (passed by constructor)
             response=response,
             # the configuration object (passed by constructor)
             configuration=configuration,
             # log file path
             log_file_path=config.LogFilePath,
             # the tracing provider used
             tracing_provider_instance=tracing_provider_instance,
-            # the template for the absolute path to the model object definitions
-            configuration_path_template=CONFIGURATION_PATH_TEMPLATE,
             # the path to the manifest file
             manifest_path=MANIFEST_PATH,
         )
+        self.dict_to_node_controller = DictToNodeController(request, response, sync_action_mapper, configuration)
+        self.domain_controller = DomainController(request, response, sync_action_mapper, configuration)
+
+    def initialize(self, request, response):
+        super().initialize(request, response)
+        self.dict_to_node_controller.initialize(request, response)
+        self.domain_controller.initialize(request, response)
+
+    def execute(self, method):
+        try:
+            if hasattr(self, method):
+                getattr(self, method)(**self.request.get_values())
+            else:
+                self.request.set_value("logger", self.logger)
+                self.request.set_value("config_loader", self.config_loader)
+                self.request.set_value("tracer", self.tracer)
+                response = self.execute_sub_action(self.request.get_action())
+                self.response.set_values(response.get_values())
+        except Exception as e:
+            self.logger.fatal(str(e))
+
+    @DefaultFacade.public
+    def convert_dict_to_node(self, *args, **kwargs):
+        self.dict_to_node_controller.convert_dict_to_node(*args,**kwargs)
+
+    @DefaultFacade.public
+    def create_node(self, *args, **kwargs):
+        self.domain_controller.create_node(*args, **kwargs)
+    
+    @DefaultFacade.public
+    def get_node_parent(self, *args, **kwargs):
+        self.domain_controller.get_parent(*args, **kwargs)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/ExCheckController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/ExCheckController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/controllers/SendExcheckUpdateController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/controllers/SendExcheckUpdateController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklist.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklist.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistColumn.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistColumn.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistColumns.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistColumns.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistDetails.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistDetails.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistTask.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistTask.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklistTasks.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklistTasks.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/domain/checklists.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/domain/checklists.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/Checklist.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/Checklist.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheck.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheck.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklist.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheckChecklist.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/ExCheckController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/ExCheckController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistDetails.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistDetails.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistTask.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistTask.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/checklistTasks.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/checklistTasks.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstance.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstance.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContents.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContents.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContentsData.py` & `FreeTAKServer-2.0.66/FreeTAKServer/components/extended/excheck/persistence/templateInstanceContentsData.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/configuration/routing/action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/configuration/routing/action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/controllers/services/FTS.py` & `FreeTAKServer-2.0.66/FreeTAKServer/controllers/services/FTS.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,19 +283,19 @@
             )
             self.CoTService.start()
             self.pipeList["TCPCoTServiceFTSPipe"] = self.TCPCoTService
             self.FilterGroup.add_receiver(
                 self.TCPCoTService, ServiceTypes.TCPCOTSERVICE
             )
             self.FilterGroup.add_source(self.TCPCoTService, ServiceTypes.TCPCOTSERVICE)
-            print("CoTService started")
+            logger.info("CoT Service Started")
             return 1
-        except Exception as e:
+        except Exception as ex:
             logger.error(
-                "an exception has been thrown in CoT service startup " + str(e)
+                "an exception has been thrown in CoT service startup " + str(ex)
             )
             return -1
 
     def stop_cot_service(self):
         """terminate the cot service process and associated ISC resources
 
         :return:
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/RestEnumerations.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/RestEnumerations.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendChatController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendChatController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendDeleteVideoStreamController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendDeleteVideoStreamController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendEmergencyController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendEmergencyController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendImageryVideoController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendImageryVideoController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendPresenceController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendPresenceController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendRouteController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendRouteController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSPISensorController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSPISensorController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSensorDroneController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSensorDroneController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendSimpleCoTController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendSimpleCoTController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/RestMessageControllers/SendVideoStreamController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/RestMessageControllers/SendVideoStreamController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendChecklist.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendChecklist.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendCoTAbstractController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendCoTAbstractController.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
             else:
                 pass
         except Exception as e:
             print(e)
             logger.warning(
                 'there has been an exception in the creation of a database instance of this object ' + str(e))
             raise Exception(e)
-        logger.info("serialized CoT "+str(RawCoT.xmlString)+" to type "+str(self))
+        logger.debug("serialized CoT "+str(RawCoT.xmlString)+" to type "+str(self))
         self.setObject(object)
 
     def create_model_object(self, tempObject, xmlString):
         """
         this function takes an empty model object and xml as arguments and then calls the serializer within the xmlcotcontroller
         module which returns a model object occupied with all the data from the CoT
         """
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendDisconnectController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendDisconnectController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendDropPointController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendDropPointController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendEmergencyController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendEmergencyController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendFederatedCoT.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendFederatedCoT.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendGeoChatController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendGeoChatController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendInvalidCoTController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendInvalidCoTController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendOtherController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendOtherController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendPingController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendPingController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/SpecificCoTControllers/SendUserUpdateController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/SpecificCoTControllers/SendUserUpdateController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/CreateLoggerController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/CreateLoggerController.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 from FreeTAKServer.core.configuration.LoggingConstants import LoggingConstants
+from FreeTAKServer.core.configuration.MainConfig import MainConfig
 from logging.handlers import RotatingFileHandler
 import logging
 import os
 import sys
 
+config = MainConfig.instance()
+
 loggingConstants = LoggingConstants()
 class CreateLoggerController:
     def __init__(self, loggername, logging_constants=loggingConstants):
         self.logger = logging.getLogger(loggername)
         self.logger.propagate = True
         log_format = logging.Formatter(logging_constants.LOGFORMAT)
-        self.logger.setLevel(logging.DEBUG)
-        self.logger.addHandler(self.newHandler(logging_constants.DEBUGLOG, logging.DEBUG, log_format, logging_constants))
-        self.logger.addHandler(self.newHandler(logging_constants.ERRORLOG, logging.ERROR, log_format, logging_constants))
-        self.logger.addHandler(self.newHandler(logging_constants.INFOLOG, logging.INFO, log_format, logging_constants))
+
+        if config.LogLevel.lower() == "info":
+            log_level = logging.INFO
+            self.logger.addHandler(self.newHandler(logging_constants.INFOLOG, log_level, log_format, logging_constants))
+        elif config.LogLevel.lower() == "error":
+            log_level = logging.ERROR
+            self.logger.addHandler(self.newHandler(logging_constants.ERRORLOG, log_level, log_format, logging_constants))
+        elif config.LogLevel.lower() == "debug":
+            log_level = logging.DEBUG
+            self.logger.addHandler(self.newHandler(logging_constants.DEBUGLOG, log_level, log_format, logging_constants))
+            
+
+        self.logger.setLevel(log_level)
         self.logger.addHandler(logging.StreamHandler(sys.stdout))
         """console = logging.StreamHandler(sys.stdout)
         console.setFormatter(log_format)
         console.setLevel(logging.DEBUG)
         self.logger.info('test')
         self.logger.addHandler(console)"""
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/CreateStartupFilesController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/CreateStartupFilesController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/DataPackageServerConstants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/DataPackageServerConstants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/LoggingConstants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/LoggingConstants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/MainConfig.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/MainConfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,19 @@
 currentPath = os.path.dirname(os.path.abspath(__file__))
 
 from pathlib import Path
 from uuid import uuid4
 
 # the version information of the server (recommended to leave as default)
 
-FTS_VERSION = "FreeTAKServer-2.0.21"
+FTS_VERSION = "FreeTAKServer-2.0.66"
 API_VERSION = "3.0"
 ROOTPATH = "/"
 MAINPATH = Path(__file__).parent.parent.parent
+USERPATH = rf"{ROOTPATH}usr/local/lib/"
 PERSISTENCE_PATH = r'/opt/fts'
 
 class MainConfig:
     """
     this is the main configuration file and is the only one which
     should need to be changed
     """
@@ -49,14 +50,15 @@
         "version": {"default": FTS_VERSION, "type": str, "readonly": True},
         "APIVersion": {"default": API_VERSION, "type": str, "readonly": True},
         "SecretKey": {"default": "vnkdjnfjknfl1232#", "type": str},
         "nodeID": {"default": f"FreeTAKServer-{_node_id}", "type": str},
         "OptimizeAPI": {"default": True, "type": bool},
         "DataReceptionBuffer": {"default": 1024, "type": int},
         "MaxReceptionTime": {"default": 4, "type": int},
+        "LogLevel": {"default": "info", "type": str},
         "UserPersistencePath": {
             "default": Path("/opt/user_persistence.txt"),
             "type": str,
         },
         # number of milliseconds to wait between each iteration of main loop
         # decreasing will increase CPU usage and server performance
         # increasing will decrease CPU usage and server performance
@@ -248,15 +250,16 @@
         "FTS_INTEGRATION_MANAGER_PULLER_ADDRESS": "IntegrationManagerPullerAddress",
         # port from which to publish messages by the integration manager
         "FTS_INTEGRATION_MANAGER_PUBLISHER_PORT": "IntegrationManagerPublisherPort",
         # address from which to publish messages by the integration manager
         "FTS_INTEGRATION_MANAGER_PUBLISHER_ADDRESS": "IntegrationManagerPublisherAddress",
         # radius of emergency within-which users will receive it
         "FTS_EMERGENCY_RADIUS": "EmergencyRadius",
-        "FTS_PERSISTENCE_PATH": "persistencePath"
+        "FTS_PERSISTENCE_PATH": "persistencePath",
+        "FTS_LOG_LEVEL": "LogLevel"
     }
 
     # This is a simple representation of the YAML config schema with
     # mappings to config var
     _yaml_keys = {
         "System": {
             "FTS_NODE_ID": "nodeID",
@@ -316,14 +319,15 @@
             "FTS_CLIENT_PACKAGES_PATH": "ClientPackages",
             "FTS_CORE_COMPONENTS_PATH": "CoreComponentsPath",
             "FTS_CORE_COMPONENTS_IMPORT_ROOT": "CoreComponentsImportRoot",
             "FTS_INTERNAL_COMPONENTS_PATH": "InternalComponentsPath",
             "FTS_INTERNAL_COMPONENTS_IMPORT_ROOT": "InternalComponentsImportRoot",
             "FTS_EXTERNAL_COMPONENTS_PATH": "ExternalComponentsPath",
             "FTS_EXTERNAL_COMPONENTS_IMPORT_ROOT": "ExternalComponentsImportRoot",
+            "FTS_LOG_LEVEL": "LogLevel"
         },
         "Certs": {
             "FTS_SERVER_KEYDIR": "keyDir",
             "FTS_SERVER_PEMDIR": "pemDir",
             "FTS_TESTCLIENT_PEMDIR": "testPem",
             "FTS_TESTCLIENT_KEYDIR": "testKey",
             "FTS_UNENCRYPTED_KEYDIR": "unencryptedKey",
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/OrchestratorConstants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/OrchestratorConstants.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/RestAPIVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/RestAPIVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/SQLcommands.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/SQLcommands.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/configuration/configuration_wizard.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/configuration/configuration_wizard.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ActiveThreadsController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ActiveThreadsController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ClientInformationController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ClientInformationController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ClientReceptionHandler.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ClientReceptionHandler.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/MainSocketController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/MainSocketController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ReceiveConnections.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ReceiveConnections.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
                     return -1
             except Exception as e:
                 client.close()
                 logger.warning('exception in returning data ' + str(e))
                 return -1
 
         except Exception as e:
-            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR)
+            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR + ": " + str(e))
             try:
                 client.close()
             except Exception as e:
                 pass
             finally:
                 return -1
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/ReceiveConnectionsProcessController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/ReceiveConnectionsProcessController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/SSLSocketController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/SSLSocketController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/SendDataController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/SendDataController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/connection/TCPCoTServiceController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/connection/TCPCoTServiceController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/cot_management_constants.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/cot_management_constants.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 CURRENT_COMPONENT_PATH = pathlib.Path(__file__).parent.parent.absolute()
 
 GEO_OBJECT = "geoobject"
 
 DELETE_GEO_OBJECT = "deletegeoobject"
 
+BASE_OBJECT = "base_object"
+
 CONFIGURATION_PATH_TEMPLATE = Template(
     str(
         pathlib.PurePath(
             CURRENT_COMPONENT_PATH, "configuration/model_definitions/$message_type"
         )
     )
     + f".{CONFIGURATION_FORMAT}"
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/external_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/external_action_mapping.ini`

 * *Files 9% similar despite different names*

```diff
@@ -73,14 +73,35 @@
 ;  next action: CreateNode
 ;  context: Repeater
 ;  values:
 ;    object_class_name (str): the root object class used for model instantiation. Usualy Event.
 ;    configuration (Configuration): the configuration defining the classes composing a geo-object delete
 ??DeleteGeoObject = FreeTAKServer.core.cot_management.cot_management_facade.CotManagement.delete_geo_object
 
+; this action is responsible for parsing and re-sending generic XML CoT's
+; Request 
+;  context: XMLCoT
+;  action: None
+;  values:
+;    dictionary: dictionary of CoT
+; Response:
+;  values:
+;    model_object (Node): an CoTManager node to be persisted
+?XMLCoT? = FreeTAKServer.core.cot_management.cot_management_facade.CotManagement.default_cot_processor
+
+; this action is responsible for determining the type of a given CoT
+; Request 
+;  action: GetCoTType
+;  values:
+;    cot_dict (dict): the cot in dictionary format
+; Response:
+;  values:
+;    emergencies (List[Node]): a list of node objects representing persisted CoTManager objects
+??GetCoTType = FreeTAKServer.core.cot_management.cot_management_facade.CotManagement.get_cot_type
+
 [CotManagement]
 __class = FreeTAKServer.core.cot_management.cot_management_facade.CotManagement
 
 [Request]
 __class = digitalpy.core.zmanager.impl.default_request.DefaultRequest
 
 [ActionMapper]
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/logging.conf` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/logging.conf`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/manifest.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/manifest.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/deletegeoobject.json` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/deletegeoobject.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/configuration/model_definitions/geoobject.json` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/configuration/model_definitions/geoobject.json`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_geo_object_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_geo_object_controller.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 class CotManagementGeoObjectController(Controller):
     """this class is responsible for handling geo objects
     """
     def __init__(
         self,
         request: Request,
         response: Response,
-        cot_management_action_mapper: ActionMapper,
+        sync_action_mapper: ActionMapper,
         configuration: Configuration,
     ) -> None:
-        super().__init__(request, response, cot_management_action_mapper, configuration)
+        super().__init__(request, response, sync_action_mapper, configuration)
 
     def initialize(self, request, response):
         self.request = request
         self.response = response
     
     def execute(self, method=None):
         getattr(self, method)(**self.request.get_values())
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_controller.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 class CotManagementRepeaterController(Controller):
     """this class is responsible for handling the business logic regarding the repeated messages
     """
     def __init__(
         self,
         request: Request,
         response: Response,
-        cot_management_action_mapper: ActionMapper,
+        sync_action_mapper: ActionMapper,
         configuration: Configuration,
     ) -> None:
-        super().__init__(request, response, cot_management_action_mapper, configuration)
-        self.persistency_controller = CotManagementRepeaterPersistence(request, response, cot_management_action_mapper, configuration)
-        self.geo_object_cotroller = CotManagementGeoObjectController(request, response, cot_management_action_mapper, configuration)
+        super().__init__(request, response, sync_action_mapper, configuration)
+        self.persistency_controller = CotManagementRepeaterPersistence(request, response, sync_action_mapper, configuration)
+        self.geo_object_cotroller = CotManagementGeoObjectController(request, response, sync_action_mapper, configuration)
 
     def initialize(self, request, response):
         self.geo_object_cotroller.initialize(request, response)
         self.request = request
         self.response = response
 
     def connected_user(self, **kwargs):
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_persistence.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_repeater_persistence.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/controllers/cot_management_sender_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/controllers/cot_management_sender_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/cot_management/cot_management_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/cot_management/cot_management_facade.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from digitalpy.core.component_management.impl.default_facade import DefaultFacade
 
 from FreeTAKServer.core.cot_management.controllers.cot_management_repeater_controller import CotManagementRepeaterController
 from FreeTAKServer.core.cot_management.controllers.cot_management_geo_object_controller import CotManagementGeoObjectController
+from FreeTAKServer.core.cot_management.controllers.cot_management_general_controller import COTManagementGeneralController
 from FreeTAKServer.core.cot_management.configuration.cot_management_constants import (
     ACTION_MAPPING_PATH,
     LOGGING_CONFIGURATION_PATH,
     INTERNAL_ACTION_MAPPING_PATH,
     MANIFEST_PATH,
     CONFIGURATION_PATH_TEMPLATE,
     LOG_FILE_PATH
@@ -24,31 +25,31 @@
     </li>
       	<li><b>Loose Coupling</b>: Availability of loose coupling between the
     clients and the Subsystems.</li>
       </ul>
     """
     def __init__(
         self,
-        cot_management_action_mapper,
+        sync_action_mapper,
         request,
         response,
         configuration,
         tracing_provider_instance=None,
     ):
         super().__init__(
             # the path to the external action mapping
             action_mapping_path=ACTION_MAPPING_PATH,
             # the path to the internal action mapping
             internal_action_mapping_path=INTERNAL_ACTION_MAPPING_PATH,
             # the path to the logger configuration
             logger_configuration=LOGGING_CONFIGURATION_PATH,
             # the package containing the base classes
             base=base,
-            # the component specific action mapper (passed by constructor)
-            action_mapper=cot_management_action_mapper,
+            # the general action mapper (passed by constructor)
+            action_mapper=sync_action_mapper,
             # the request object (passed by constructor)
             request=request,
             # the response object (passed by constructor)
             response=response,
             # the configuration object (passed by constructor)
             configuration=configuration,
             # log file path
@@ -56,36 +57,38 @@
             # the tracing provider used
             tracing_provider_instance=tracing_provider_instance,
             # the template for the absolute path to the model object definitions
             configuration_path_template=CONFIGURATION_PATH_TEMPLATE,
             # the path to the manifest file
             manifest_path=MANIFEST_PATH,
         )
-        self.repeater_controller = CotManagementRepeaterController(request, response, cot_management_action_mapper, configuration)
-        self.geo_object_controller = CotManagementGeoObjectController(request, response, cot_management_action_mapper, configuration)
+        self.repeater_controller = CotManagementRepeaterController(request, response, sync_action_mapper, configuration)
+        self.geo_object_controller = CotManagementGeoObjectController(request, response, sync_action_mapper, configuration)
+        self.general_controller = COTManagementGeneralController(request, response, sync_action_mapper, configuration)
+
+    
+    def initialize(self, request, response):
+        super().initialize(request, response)
+        self.repeater_controller.initialize(request, response)
+        self.geo_object_controller.initialize(request, response)
+        self.general_controller.initialize(request, response)
 
     def execute(self, method):
-        
         try:
             if hasattr(self, method):
                 getattr(self, method)(**self.request.get_values())
             else:
                 self.request.set_value("logger", self.logger)
                 self.request.set_value("config_loader", self.config_loader)
                 self.request.set_value("tracer", self.tracer)
                 response = self.execute_sub_action(self.request.get_action())
                 self.response.set_values(response.get_values())
         except Exception as e:
             self.logger.fatal(str(e))
-
-    def initialize(self, request, response):
-        super().initialize(request, response)
-        self.repeater_controller.initialize(request, response)
-        self.geo_object_controller.initialize(request, response)
-
+            
     @DefaultFacade.public
     def connection(self, *args, **kwargs):
         self.repeater_controller.connected_user(*args, **kwargs)
 
     @DefaultFacade.public
     def get_repeated_messages(self, *args, **kwargs):
         self.repeater_controller.get_repeated_messages(*args, **kwargs)
@@ -99,8 +102,12 @@
     
     @DefaultFacade.public
     def create_geo_object(self, *args, **kwargs):
         self.geo_object_controller.create_geo_object(*args, **kwargs)
 
     @DefaultFacade.public
     def delete_geo_object(self, *args, **kwargs):
-        self.geo_object_controller.delete_geo_object(*args, **kwargs)
+        self.geo_object_controller.delete_geo_object(*args, **kwargs)
+
+    @DefaultFacade.public
+    def default_cot_processor(self, *args, **kwargs):
+        self.general_controller.handle_default_cot(**kwargs)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/data_package/data_package_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/data_package/data_package_facade.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/domain/BasicModelInstantiate.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/domain/BasicModelInstantiate.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/domain/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/domain/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/domain/domain_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/domain/domain_facade.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/domain/node.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/domain/node.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/domain/object_id.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/domain/object_id.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/fts_configuration/fts_configuration_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/fts_configuration/fts_configuration_facade.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/configuration/internal_action_mapping.ini` & `FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/configuration/internal_action_mapping.ini`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/fts_core/fts_core_facade.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/fts_core/fts_core_facade.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/health/HealthCheckController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/health/HealthCheckController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/health/ServerStatusController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/health/ServerStatusController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/ApplyFullJsonController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/ApplyFullJsonController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/XMLCoTController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/XMLCoTController.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
                 self.logger.error(
                     loggingConstants.XMLCOTCONTROLLERDETERMINECOTGENERALERRORA + str(e)
                 )
         # this runs if it is infact regular data
         elif data.xmlString == b"" or data.xmlString == None:
             # this handeles a client dissconection CoT
             return ("clientDisconnected", data)
+
         else:
             # serialize the XML to an etree object
             event = etree.fromstring(data.xmlString)
             request = ObjectFactory.get_new_instance("request")
             request.set_action("XMLToDict")
             request.set_value("message", data.xmlString)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/parsers/templateToJsonSerializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/parsers/templateToJsonSerializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/ActiveEmergencysController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/ActiveEmergencysController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/DatabaseController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/DatabaseController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/EventTableController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/EventTableController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/TableController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/TableController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/VideoStreamTableController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/VideoStreamTableController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/persistence/table_controllers.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/persistence/table_controllers.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/SqlAlchemyObjectController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/SqlAlchemyObjectController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/api_adapters.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/api_adapters.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/api_adapters/geo_object_adapter.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/api_adapters/geo_object_adapter.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/protobuf_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/protobuf_serializer.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/serializer_abstract.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/serializer_abstract.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/serializers/xml_serializer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/serializers/xml_serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
                 setters = self._get_fts_object_var_setter(FTSObject, subelem.tag)
                 setter = self._get_method_in_method_list(setters, element.tag)
                 getters = self._get_fts_object_var_getter(FTSObject, subelem.tag)
                 getter = self._get_method_in_method_list(getters, element.tag)
                 fts_obj = getter()
                 setter(self.from_format_to_fts_object(etree.tostring(subelem), fts_obj))
             except AttributeError:
-                logger.info("the following tag is missing from the FTS model, missing cot "+str(etree.tostring(element)) + " missing tag name: "+str(subelem.tag))
+                logger.debug("the following tag is missing from the FTS model, missing cot "+str(etree.tostring(element)) + " missing tag name: "+str(subelem.tag))
 
     def from_fts_object_to_format(self, FTSObject: Event, root: Element = None) -> Element:
         """ serialize a FTS_object to an etree Element
         this function takes as parameters any FTSObject and will convert
         into the cooresponding etree element which can be converted into
         an xmlstring or left as a python object
         :rtype: etree._Element
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/DataPackageServer.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/DataPackageServer.py`

 * *Files 6% similar despite different names*

```diff
@@ -299,15 +299,34 @@
 
 
 @app.route('/')
 def home():
     return 'data package service is up, good job.'
 
 
-# exCheckStuff
+# exCheck functions
+"""   TODO End Points for 4.8 Support  
+    The Execution Checklist (ExCheck) allows users to monitor and update the status of a shared 
+    checklist that is hosted out on a TAK server. Each checklist is an instance of a template 
+    that defines a number of tasks to be completed. 
+   
+    @app.route('/Marti/api/excheck/<checklistUid>/stop', methods=['POST'])
+    @app.route('/Marti/api/excheck/<templateUid>/start', methods=['POST'])
+    @app.route('/Marti/api/excheck/checklist', methods=['POST'])
+    @app.route('/Marti/api/excheck/checklist/<checklistUid>', methods=['GET'])
+    @app.route('/Marti/api/excheck/checklist/<checklistUid>/mission/<missionName>', methods=['PUT', 'DELETE'])
+    @app.route('/Marti/api/excheck/checklist/<checklistUid>/status', methods=['GET', 'DELETE'])
+    @app.route('/Marti/api/excheck/checklist/<checklistUid>/task/<taskUid>', methods=['GET', 'PUT','DELETE'])
+    @app.route('/Marti/api/excheck/checklist/active', methods=['GET'])
+    @app.route('/Marti/api/excheck/template', methods=['POST'])
+    @app.route('/Marti/api/excheck/template/<templateUid>', methods=['GET', 'DELETE'])
+    @app.route('/Marti/api/excheck/template/<templateUid>/task/<taskUid>', methods=['GET', 'PUT','DELETE','POST'])
+"""
+
+
 @app.route('/Marti/api/missions/exchecktemplates/changes', methods=['GET'])
 def check_changes():
     try:
         # example return data {"version":"2","type":"MissionChange","data":[],"nodeId":"TAK-Server-a6htdf93"}
         # this endpoint should return any excheck template change since specified time
         # TODO: learn what squached represents
         request.args.get('squached')
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/Orchestrator.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/Orchestrator.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/RestAPI.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/RestAPI.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/SSLCoTServiceController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/SSLCoTServiceController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/SSLDataPackageService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/SSLDataPackageService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/TCPDataPackageService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/TCPDataPackageService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/FederationClientService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/FederationClientService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/external_data_handlers.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/external_data_handlers.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/federation.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/federation.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/federation_service_base.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/federation_service_base.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/federation/handlers.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/federation/handlers.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/internal_telemetry_service.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/internal_telemetry_service.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/services/service_abstracts.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/services/service_abstracts.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/util/AddDataToCoTList.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/util/AddDataToCoTList.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/util/certificate_generation.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/util/certificate_generation.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/core/util/geo_manager_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/core/util/geo_manager_controller.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ActiveThreads.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ActiveThreads.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ClientInformation.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ClientInformation.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/Connection.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/Connection.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Chat.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Chat.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Chatgrp.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Chatgrp.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Checklist.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Checklist.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ChecklistDetails.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ChecklistDetails.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Checklists.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Checklists.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Color.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Color.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ConnectionEntry.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ConnectionEntry.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Contact.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Contact.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/ContentResource.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/ContentResource.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/CreatorCallsign.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/CreatorCallsign.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/CreatorUid.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/CreatorUid.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Dest.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Dest.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Detail.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Detail.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/DimensionTypes.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/DimensionTypes.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Emergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Emergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/EntityTypes.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/EntityTypes.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Event.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Event.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Filename.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Filename.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Group.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Group.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/IdentityTypes.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/IdentityTypes.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Keywords.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Keywords.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Link.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Link.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Link_attr.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Link_attr.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Marti.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Marti.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MimeType.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MimeType.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Mission.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Mission.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MissionChange.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MissionChange.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/MissionName.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/MissionName.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Name.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Name.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Point.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Point.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Precisionlocation.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Precisionlocation.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Remarks.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Remarks.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Serverdestination.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Serverdestination.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Status.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Status.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/SubmissionTime.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/SubmissionTime.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Submitter.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Submitter.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Summary.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Summary.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Takv.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Takv.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Timestamp.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Timestamp.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Track.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Track.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Uid.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Uid.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/Usericon.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/Usericon.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_Group.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_Group.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_Video.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_Video.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_medevac_ .py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_medevac_ .py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/_uastool.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/_uastool.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModel/sensor.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModel/sensor.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ConnectionEntryVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ConnectionEntryVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/ContactVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/ContactVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/EventVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/EventVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/LinkVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/LinkVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/PrecisionlocationVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/PrecisionlocationVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/RemarksVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/RemarksVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/TrackVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/TrackVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FTSModelVariables/sensorVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FTSModelVariables/sensorVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/FilterGroup.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/FilterGroup.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RawCoT.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RawCoT.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/DroneSensor.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/DroneSensor.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Emergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Emergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/EmergencyPost.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/EmergencyPost.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/GeoObject.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/GeoObject.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/GeoObjectPost.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/GeoObjectPost.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/Presence.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/Presence.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/PresencePost.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/PresencePost.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/RestEnumerations.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/RestEnumerations.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/RoutePost.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/RoutePost.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/SPISensor.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/SPISensor.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/RestMessages/SimpleAPIMessageAbstract.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/RestMessages/SimpleAPIMessageAbstract.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/APICalls.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/APICalls.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/APIUsers.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/APIUsers.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/ActiveEmergencys.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/ActiveEmergencys.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Archive.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Archive.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Chat.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Chat.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Color.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Color.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/ConnectionEntry.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/ConnectionEntry.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Contact.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Contact.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Dest.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Dest.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Detail.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Detail.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Emergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Emergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Link.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Link.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Marti.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Marti.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Point.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Point.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Precisionlocation.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Precisionlocation.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Remarks.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Remarks.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Sensor.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Sensor.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Serverdestination.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Serverdestination.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Status.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Status.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Summary.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Summary.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Takv.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Takv.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Track.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Track.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Uid.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Uid.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/Usericon.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/Usericon.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/_Group.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/_Group.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/CoTTables/_Video.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/CoTTables/_Video.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/DataPackage.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/DataPackage.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/Event.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/Event.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/ExCheckData.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/ExCheckData.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/User.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/User.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/VideoStream.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/VideoStream.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/federations.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/federations.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SQLAlchemy/system_user.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SQLAlchemy/system_user.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SSLConnection.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SSLConnection.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/ComponentRegistration.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/ComponentRegistration.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/ComponentRegistrationVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/ComponentRegistrationVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FTS.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FTS.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/Federate.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/Federate.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederateClients.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederateClients.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationClientService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationClientService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/FederationServerService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/FederationServerService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/IntegrationManagerService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/IntegrationManagerService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/IntegrationManagerServiceVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/IntegrationManagerServiceVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RoutingProxyService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RoutingProxyService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/RoutingProxyServiceVariables.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/RoutingProxyServiceVariables.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/SSLDataPackageService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/SSLDataPackageService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/ServiceObjects/TCPDataPackageService.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/ServiceObjects/TCPDataPackageService.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SendEmergency.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SendEmergency.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/SpecificCoT/SpecificCoTAbstract.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/SpecificCoT/SpecificCoTAbstract.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/TCPConnection.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/TCPConnection.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/User.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/User.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/contact_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/contact_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/cotevent_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/cotevent_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/detail_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/detail_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/fig_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/fig_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/group_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/group_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/precisionlocation_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/precisionlocation_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/simple_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/simple_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/status_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/status_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takcontrol_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takcontrol_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takmessage_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takmessage_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/takv_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/takv_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/protobufModel/track_pb2.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/protobufModel/track_pb2.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/MainSocket.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/MainSocket.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/model/sockets/SSLServerSocket.py` & `FreeTAKServer-2.0.66/FreeTAKServer/model/sockets/SSLServerSocket.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/rest_api_service/rest_api_service_main.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/rest_api_service/rest_api_service_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -466,15 +466,14 @@
                 dbController.create_datapackage(uid=user_id, Name=cert_name + '.zip', Hash=file_hash,
                                                 SubmissionUser='server',
                                                 CreatorUid='server-uid', Size=fileSize, Privacy=1)
                 dbController.create_systemUser(name=systemuser["Name"], group=systemuser["Group"],
                                                 token=systemuser["Token"], password=systemuser["Password"],
                                                 uid=user_id,
                                                 certificate_package_name=cert_name + '.zip', device_type = systemuser["DeviceType"])
-                import datetime as dt
                 DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
                 timer = dt.datetime
                 now = timer.utcnow()
                 zulu = now.strftime(DATETIME_FMT)
                 add = dt.timedelta(seconds=600)
                 stale_part = dt.datetime.strptime(zulu, DATETIME_FMT) + add
                 stale = stale_part.strftime(DATETIME_FMT)
@@ -1781,14 +1780,52 @@
     socketio.emit('up', json.dumps(returnValue), broadcast=True)
     data = Updates
     for client in data:
         returnValue.append(ApplyFullJsonController().serialize_model_to_json(client))
     socketio.emit('up', json.dumps(returnValue), broadcast=True)
     return 1
 
+@app.route('/v2/<context>/<action>', methods=[restMethods.GET, restMethods.POST])
+@auth.login_required
+def api_routing(context, action):
+    """the main method for the routing based API which uses information fro
+    the route and the method to send the request to the internal router, 
+    returning the response
+
+    Args:
+        context (str): the context of the request, for use in the routing
+        action (str): the action of the request, for use in the routing
+
+    Raises:
+        ValueError: if the synchronous parameter is true and the service_idis 
+
+    Returns:
+        dict: the values of the response returned by the component
+    """
+    synchronous = request.args.get("synchronous", True) # all requests are by default synchronous
+    service_id = request.args.get("service_id")
+    values = request.get_json()
+    rest_api_service = ObjectFactory.get_instance("RestAPIService")
+    service_id_different = service_id is not None and rest_api_service.service_id != service_id
+    if synchronous == True and service_id_different:
+        raise ValueError("synchronous is true and service_id is neither None or rest api service id,\
+                            this will result in an undefined state where we are waiting for a response that will never come")
+
+    # request to get repeated messages
+    internal_request: Request = ObjectFactory.get_new_instance("request")
+    internal_request.set_action(action)
+    internal_request.set_context(context)
+    internal_request.set_sender(rest_api_service.__class__.__name__.lower())
+    internal_request.set_format("pickled")
+    internal_request.set_values(values or {})
+    rest_api_service.subject_send_request(internal_request, APPLICATION_PROTOCOL, service_id)
+    if synchronous == True:
+        response = rest_api_service.retrieve_response(internal_request.get_id())
+        return response.get_values()
+
 # TODO: move this out of the rest_api_service and into it's own file in views
 # this will require changing it from using the API Pipe to use the ZManager instead
 import json
 import datetime as dt
 import datetime
 
 from flask import request
@@ -1797,22 +1834,23 @@
 from digitalpy.core.zmanager.request import Request
 from geopy import Point, distance
 
 from FreeTAKServer.core.RestMessageControllers.SendSimpleCoTController import SendSimpleCoTController
 from FreeTAKServer.core.parsers.JsonController import JsonController
 
 from FreeTAKServer.services.rest_api_service.views.base_view import BaseView
+from FreeTAKServer.services.rest_api_service.views.emergency_view import ManageEmergency
 
 class ManageGeoObjects(BaseView):
     """this class is responsible for creating the flask views required for managing
     geo objects in FTS
     """
     decorators = [auth.login_required]
     
-    def __init__(self) -> None:
+    def __init__(self, *args, **kwargs) -> None:
         endpoints: Dict[str, callable] = {
             "GetRepeatedMessages": self.get_repeated_messages,
             "postGeoObject": self.post_geo_object,
             "DeleteRepeatedMessages": self.delete_repeated_messages,
         }
         super().__init__(endpoints)
 
@@ -1860,53 +1898,52 @@
                     end_point = d.destination(point=start_point, bearing=jsondata["bearing"])
                 else:
                     end_point = d.destination(point=start_point, bearing=360)
                 jsonobj.setlatitude(end_point.latitude)
                 jsonobj.setlongitude(end_point.longitude)
 
             simpleCoTObject = SendSimpleCoTController(jsonobj).getCoTObject()
+            # make request to create a geoobject node
+            response = self.make_request("CreateGeoObject", {"id": jsonobj.getuid()})
+            # apply the given values to the model object
+            model_object = response.get_value("model_object")
+            model_object.uid = jsonobj.getuid()
+            COTTYPE = jsonobj.getgeoObject()
+            if "-.-" in COTTYPE:
+                ID = jsonobj.getattitude()
+                COTTYPE = COTTYPE.replace('-.-', ID)
+            else:
+                pass
+            model_object.type = COTTYPE
+            model_object.how = jsonobj.gethow()
+            
+            model_object.start = None # set to default val
+            model_object.time = None  # set to default val
+            if jsonobj.gettimeout() != '' and jsonobj.gettimeout() != None:
+                DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
+                timer = dt.datetime
+                now = timer.utcnow()
+                add = datetime.timedelta(seconds=int(jsonobj.gettimeout()))
+                stale = now+add
+                model_object.stale = stale.strftime(DATETIME_FMT)
+            else:
+                model_object.stale = None # set to default val
+            #    DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
+            #    timer = dt.datetime
+            #    now = timer.utcnow()
+            #    zulu = now.strftime(DATETIME_FMT)
+            #    add = datetime.timedelta(seconds=int(jsonobj.gettimeout()))
+            #    stale_part = dt.datetime.strptime(zulu, DATETIME_FMT) + add
+            #model_object.stale = stale_part
+            model_object.point.lat = jsonobj.getlatitude()
+            model_object.point.lon = jsonobj.getlongitude()
+            model_object.detail.contact.callsign = jsonobj.getname()
 
             # if the message should be repeated then make a request to repeat it
             if jsonobj.getrepeat():
-                # make request to create a geoobject node
-                response = self.make_request("CreateGeoObject", {"id": jsonobj.getuid()})
-                
-                # apply the given values to the model object
-                model_object = response.get_value("model_object")
-                model_object.uid = jsonobj.getuid()
-                COTTYPE = jsonobj.getgeoObject()
-                if "-.-" in COTTYPE:
-                    ID = jsonobj.getattitude()
-                    COTTYPE = COTTYPE.replace('-.-', ID)
-                else:
-                    pass
-                model_object.type = COTTYPE
-                model_object.how = jsonobj.gethow()
-                
-                model_object.start = None # set to default val
-                model_object.time = None  # set to default val
-                if jsonobj.gettimeout() != '' and jsonobj.gettimeout() != None:
-                    DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
-                    timer = dt.datetime
-                    now = timer.utcnow()
-                    add = datetime.timedelta(seconds=int(jsonobj.gettimeout()))
-                    stale = now+add
-                    model_object.stale = stale.strftime(DATETIME_FMT)
-                else:
-                    model_object.stale = None # set to default val
-                #    DATETIME_FMT = "%Y-%m-%dT%H:%M:%S.%fZ"
-                #    timer = dt.datetime
-                #    now = timer.utcnow()
-                #    zulu = now.strftime(DATETIME_FMT)
-                #    add = datetime.timedelta(seconds=int(jsonobj.gettimeout()))
-                #    stale_part = dt.datetime.strptime(zulu, DATETIME_FMT) + add
-                #model_object.stale = stale_part
-                model_object.point.lat = jsonobj.getlatitude()
-                model_object.point.lon = jsonobj.getlongitude()
-                model_object.detail.contact.callsign = jsonobj.getname()
                
                 # make request to persist the model object to be re-sent
                 response = self.make_request("CreateRepeatedMessage", {"message": [model_object]})
 
             print("putting in queue")
             APIPipe.put(simpleCoTObject)
             print(simpleCoTObject.xmlString)
@@ -1945,80 +1982,15 @@
                 return 'operation failed', 500
         except Exception as e:
             return str(e), 500
 
 # TODO: move this out of the rest_api_service and into it's own file in views
 # this will require changing it from using the API Pipe to use the ZManager instead
 
-from FreeTAKServer.services.rest_api_service.views.base_view import BaseView
-from typing import Dict
-from flask import request
-
-from FreeTAKServer.core.configuration.LoggingConstants import LoggingConstants
-from FreeTAKServer.core.configuration.CreateLoggerController import CreateLoggerController
-from FreeTAKServer.core.parsers.JsonController import JsonController
-from FreeTAKServer.core.RestMessageControllers.SendEmergencyController import SendEmergencyController
-
-loggingConstants = LoggingConstants(log_name="FTS-ManageEmergencyView")
-logger = CreateLoggerController("FTS-ManageEmergencyView", logging_constants=loggingConstants).getLogger()
-
-class ManageEmergency(BaseView):
-    decorators = [auth.login_required]
-    
-    def __init__(self) -> None:
-        endpoints = {
-            "getEmergency": self.get_emergency,
-            "postEmergency": self.post_emergency,
-            "deleteEmergency": self.delete_emergency,
-        }
-        super().__init__(endpoints)
-    
-    def get_emergency(self):
-        """method to retrieve all emergency's
-        Returns:
-            str: returns a json string containing dictionary of emergency's
-
-        """
-        response = self.make_request("GetAllEmergencies") # retrieve emergencies from the emergency component
-        emergencies = response.get_value("emergencies")
-        output = {"json_list": []}
-        for emergency in emergencies:
-            try:
-                serialized_emergency = {
-                    "lat": emergency.point.lat,
-                    "lon": emergency.point.lon,
-                    "type": emergency.detail.emergency.type,
-                    "name": emergency.detail.contact.callsign,
-                    "uid": emergency.uid
-                }
-                output["json_list"].append(serialized_emergency)
-            except AttributeError as ex:
-                logger.error("emergency model object missing attribute %s", ex)
-        return output
-    
-    def post_emergency(self):
-        jsondata = request.get_json(force=True)
-        jsonobj = JsonController().serialize_emergency_post(jsondata)
-        emergency_object = SendEmergencyController(jsonobj).getCoTObject()
-        self.make_request("SaveEmergency", {"model_object": emergency_object.modelObject})
-        APIPipe.put(emergency_object)
-        return emergency_object.modelObject.getuid(), 200
-    
-    def delete_emergency(self) -> str:
-        """delete an emergency from the emergency persistence
-
-        """
-        jsondata = request.get_json(force=True)
-        jsonobj = JsonController().serialize_emergency_delete(jsondata)
-        emergency_object = SendEmergencyController(jsonobj).getCoTObject()
-        APIPipe.put(emergency_object)
-        self.make_request("DeleteEmergency", {"model_object": emergency_object.modelObject})
-        return 'success', 200
-
-app.add_url_rule('/ManageEmergency/<method>', view_func=ManageEmergency.as_view('/ManageEmergency/<method>'), methods=["POST", "GET", "DELETE"])
+ManageEmergency.decorators.append(auth.login_required)
 app.add_url_rule('/ManageGeoObject/<method>', view_func=ManageGeoObjects.as_view('/ManageGeoObject/<method>'), methods=["POST", "GET","DELETE"])
 
 APPLICATION_PROTOCOL = "xml"
 API_REQUEST_TIMEOUT = 5000
 
 class RestAPI(DigitalPyService):
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/ClientReceptionHandler.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/ClientReceptionHandler.py`

 * *Files 14% similar despite different names*

```diff
@@ -18,16 +18,16 @@
 from FreeTAKServer.core.configuration.CreateLoggerController import CreateLoggerController
 from FreeTAKServer.core.configuration.LoggingConstants import LoggingConstants
 from defusedxml import ElementTree as etree
 
 # Make a connection to the MainConfig object for all routines below
 config = MainConfig.instance()
 
-loggingConstants = LoggingConstants(log_name="FTS_ClientReceptionHandler")
-logger = CreateLoggerController("FTS_ClientReceptionHandler", logging_constants=loggingConstants).getLogger()
+loggingConstants = LoggingConstants(log_name="FTS_SSLClientReceptionHandler")
+logger = CreateLoggerController("FTS_SSLClientReceptionHandler", logging_constants=loggingConstants).getLogger()
 from FreeTAKServer.core.configuration.ClientReceptionLoggingConstants import ClientReceptionLoggingConstants
 
 loggingConstants = ClientReceptionLoggingConstants()
 BUFF_SIZE = DATA_RECEPTION_BUFFER_SIZE
 
 class ClientReceptionHandler:
     def __init__(self):
@@ -38,14 +38,15 @@
         try:
             self.clientInformationArray = clientInformationArray  # create copy of client information array so it cant be changed during iteration
             '''logger.propagate = False
             logger.info(loggingConstants.CLIENTRECEPTIONHANDLERSTART)
             logger.propagate = True'''
             output = self.monitorForData(self.dataPipe)
             if output == 1:
+                if len(self.dataPipe)>0: logger.debug("returning data array %s", str(self.dataPipe))
                 return self.dataPipe
             else:
                 return -1
             '''
             time.sleep(600)
             # temporarily remove due to being unnecessary and excessively flooding logs
             logger.info('the number of threads is ' + str(threading.active_count()) + ' monitor event process alive is ' + str(monitorEventProcess.is_alive()) +
@@ -64,47 +65,79 @@
                 sock = self.clientInformationArray[user_id][0]
                 client = user_id
                 #client = self.clientInformationArray[user_id][1]
                 try:
                     sock.settimeout(0.001)
                     try:
                         xmlstring = self.recv_until(sock).decode()
-                        if xmlstring == b'' or xmlstring == '' or xmlstring is None: 
+                        if xmlstring == b'' or xmlstring == '' or xmlstring is None:
+                            #xmlstring = self.validate_client_disconnect(queue, sock, client)
+                            #if xmlstring is None:
+                            #    continue
                             self.returnReceivedData(client, b'', queue)
-                            logger.debug("empty string sent, standard disconnect")
                             continue
                         xmlstring = "<multiEvent>" + xmlstring + "</multiEvent>"  # convert to xmlstring wrapped by multiEvent tags
                         xmlstring = re.sub(r'(?s)\<\?xml(.*)\?\>', '', xmlstring)  # replace xml definition tag with empty string as it breaks serilization
                         events = etree.fromstring(xmlstring)  # serialize to object
                         for event in events.findall('event'):
+                            event_str = etree.tostring(event)
+                            logger.debug("received: %s from %s", event_str, client)
                             self.returnReceivedData(client, etree.tostring(event), queue)  # send each instance of event to the core
-                    except socket.timeout as e:
+                    except socket.timeout as ex:
                         continue
-                    except BrokenPipeError as e:
+                    except BrokenPipeError as ex:
+                        logger.debug("disconnecting client %s due to broken pipe", client)
                         self.returnReceivedData(client, b'', queue)
                         continue
-                    except Exception as e:
+                    except ConnectionAbortedError as ex:
+                        logger.debug("disconnecting client %s due to connection aborted", client)
+                        self.returnReceivedData(client, b'', queue)
+                        continue
+                    except ConnectionResetError as ex:
+                        logger.debug("disconnecting client %s due to connection reset", client)
+                        self.returnReceivedData(client, b'', queue)
+                        continue
+                    except Exception as ex:
                         import traceback
-                        if hasattr(e, "errno") and e.errno == errno.EWOULDBLOCK:  # this prevents errno 11 from spontanieously disconnecting clients due to the socket blocking set to 0
-                            logger.debug("EWOULDBLOCK error passed " + str(e))
+                        if hasattr(ex, "errno") and ex.errno == errno.EWOULDBLOCK:  # this prevents errno 11 from spontanieously disconnecting clients due to the socket blocking set to 0
+                            logger.debug("EWOULDBLOCK error passed " + str(ex))
                             continue
                         logger.error(
-                            "Exception other than broken pipe in monitor for data function " + str(e) + ''.join(traceback.format_exception(None, e, e.__traceback__)))
+                            "Exception other than broken pipe in monitor for data function " + str(ex) + ''.join(traceback.format_exception(None, ex, ex.__traceback__)))
                         self.returnReceivedData(client, b'', queue)
                         continue
 
-                except Exception as e:
-                    logger.error(loggingConstants.CLIENTRECEPTIONHANDLERMONITORFORDATAERRORD + str(e))
+                except Exception as ex:
+                    logger.error(loggingConstants.CLIENTRECEPTIONHANDLERMONITORFORDATAERRORD + str(ex))
                     self.returnReceivedData(client, b'', queue)
                     # return -1 commented out so entire run isn't stopped because of one disconnect
             return 1
-        except Exception as e:
-            logger.error('exception in monitor for data ' + str(e))
+        except Exception as ex:
+            logger.error('exception in monitor for data ' + str(ex))
             return -1
 
+    def validate_client_disconnect(self, queue, sock, client):
+        """ensure that the client is correctly disconnected
+
+        Args:
+            queue (_type_): _description_
+            sock (_type_): _description_
+            client (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        for _ in range(10):
+            xmlstring = self.recv_until(sock).decode()
+            if xmlstring != b'' or xmlstring != '' or xmlstring is not None:
+                return xmlstring
+        logger.debug("empty string sent from %s, standard disconnect", client)
+        self.returnReceivedData(client, b'', queue)
+        return None
+
     def returnReceivedData(self, clientInformation, data, queue):
         try:
             from FreeTAKServer.model.RawCoT import RawCoT
             RawCoT = RawCoT()
             RawCoT.clientInformation = clientInformation
             RawCoT.xmlString = data.replace(b'\n', b'')  # replace all newlines with empty
             self.dataPipe.append(RawCoT)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/ReceiveConnections.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/ReceiveConnections.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,28 +64,51 @@
         client.settimeout(int(ReceiveConnectionsConstants().RECEIVECONNECTIONDATATIMEOUT))
         xmlstring = "<multiEvent>" + part.decode() + xmlstring + "</multiEvent>"  # convert to xmlstring wrapped by multiEvent tags
         xmlstring = re.sub(r'(?s)\<\?xml(.*)\?\>', '',
                            xmlstring)  # replace xml definition tag with empty string as it breaks serilization
         events = etree.fromstring(xmlstring)
         return events
 
-    def listen(self, sock):
+    def listen(self, sock: socket.socket) -> Union[sat, int]:
+        """
+        Listen for incoming client connections and process them.
+
+        This method listens for incoming client connections, receives data from the
+        client, and then instantiates a client object with the received data. If
+        any errors occur during this process, the method returns -1. Otherwise, it
+        returns the instantiated client object.
+
+        Parameters
+        ----------
+        sock : socket.socket
+            The socket to listen for incoming connections on.
+
+        Returns
+        -------
+        Union[sat, int]
+            The instantiated client object, or -1 if any errors occurred.
+        """
+
         # logger = CreateLoggerController("ReceiveConnections").getLogger()
-        # listen for client connections
+
+        # Listen for client connections
         sock.listen(ReceiveConnectionsConstants().LISTEN_COUNT)
         try:
             # establish the socket variables
             socket.setdefaulttimeout(ReceiveConnectionsConstants().SSL_SOCK_TIMEOUT)
             sock.settimeout(ReceiveConnectionsConstants().SSL_SOCK_TIMEOUT)
             # logger.debug('receive connection started')
             try:
                 client, address = sock.accept()
+            except socket.timeout:
+                logger.debug("ssl sock threw timeout error")
+                return -1
+            try:    
                 ssl_client = SSLSocketController().wrap_client_socket(client)
             except ssl.SSLError as ex:
-                print(ex)
                 self.disconnect_socket(client, ssl_client)
                 logger.warning('ssl error thrown in connection attempt ' + str(ex))
                 return -1
 
             except asyncio.TimeoutError as ex:
                 self.disconnect_socket(client, ssl_client)
                 logger.warning('timeout error thrown in connection attempt '+str(ex))
@@ -119,15 +142,15 @@
                     return -1
             except Exception as ex:
                 self.disconnect_socket(client, ssl_client)
                 logger.warning('exception in returning data ' + str(ex))
                 return -1
 
         except Exception as ex:
-            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR)
+            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR + ": " + str(ex))
             try:
                 self.disconnect_socket(client, ssl_client)
             except Exception as ex:
                 pass
             finally:
                 return -1
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/SSLSocketController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/SSLSocketController.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/SendDataController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/controllers/SendDataController.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             if (
                                 client[1].m_presence.modelObject.detail.contact.callsign
                                 == dest
                             ):
                                 sock = client[0]
                                 try:
                                     sock.send(processedCoT.xmlString)
-                                    logger.info(
+                                    logger.debug(
                                         str(processedCoT.xmlString)
                                         + " sent to client "
                                         + client_id
                                     )
                                 except Exception as e:
                                     logger.error(
                                         "error sending data with marti to client data "
@@ -164,23 +164,23 @@
                 try:
                     if hasattr(processedCoT, "xmlString"):
                         # print('sending to all ' + str(processedCoT.xmlString))
                         try:
                             sock.send(processedCoT.xmlString)
                         except TypeError:
                             sock.send(processedCoT.xmlString.encode())
-                        logger.info(
+                        logger.debug(
                             str(processedCoT.xmlString) + " sent to client " + client_id
                         )
                     else:
                         try:
                             sock.send(processedCoT.idData)
                         except TypeError:
                             sock.send(processedCoT.idData.encode())
-                        logger.info(
+                        logger.debug(
                             str(processedCoT.idData) + " sent to client " + client_id
                         )
                 except Exception as e:
                     logger.error("error in sending of data " + str(e))
                     return (-1, client[1])
             if shareDataPipe != None:
                 processedCoT.clientInformation = None
@@ -235,15 +235,15 @@
                         logger.error(
                             "error sending data with marti to client within if data is "
                             + str(processedCoT.xmlString)
                             + "error is "
                             + str(e)
                         )
                         return -1
-                logger.info("CoT sent " + str(processedCoT.modelObject.uid))
+                logger.debug("CoT sent " + str(processedCoT.modelObject.uid))
                 if shareDataPipe != None:
                     processedCoT.clientInformation = None
                     if hasattr(self, "messages_to_core_count"):
                         self.messages_to_core_count += 1
                     shareDataPipe.put(processedCoT)
                 else:
                     pass
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/controllers/send_component_data_controller.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/send_component_data_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from typing import Dict
 
-from FreeTAKServer.services.ssl_cot_service.model.ssl_cot_connection import SSLCoTConnection
-from ..configuration.ssl_cot_service_constants import MessageTypes
+from FreeTAKServer.services.tcp_cot_service.model.tcp_cot_connection import TCPCoTConnection
+from ..configuration.tcp_cot_service_constants import MessageTypes
 
 from digitalpy.core.main.controller import Controller
 
+import logging
+
 class SendComponentDataController(Controller):
-    def __init__(self, request, response, action_mapper, configuration) -> None:
-        super().__init__(request, response, action_mapper, configuration)
+    def __init__(self, logger) -> None:
+        self.logger = logger
 
     def send_message(self, connections, message, recipients, **kwargs):
         message_type = self.determine_message_type(recipients)
         if message_type == MessageTypes.SEND_TO_ALL:
             self.send_message_to_all(connections, message)
         
         elif message_type == MessageTypes.SEND_TO_SOME:
@@ -20,34 +22,50 @@
     def determine_message_type(self, recipients) -> MessageTypes:
         """determine whether the message is to be sent to all or only
         some connections based on the value of recipients
 
         Returns:
             MessageTypes: _description_
         """
-        if recipients == None or recipients == []:
+        if recipients is None or recipients == []:
             return MessageTypes.SEND_TO_ALL
         else:
             return MessageTypes.SEND_TO_SOME
     
-    def send_message_to_some(self, connections:Dict[str, SSLCoTConnection], message: bytes, recipients):
+    def send_message_to_some(self, connections:Dict[str, TCPCoTConnection], message: bytes, recipients):
         """send a given message to some connections based on value of recipients
 
         Args:
-            connections (dict[str, SSLCoTConnection]): a dictionary of connections indexed by their OIDs
+            connections (dict[str, TCPCoTConnection]): a dictionary of connections indexed by their OIDs
             message (bytes): the message to be sent to some clients
         """
         
         for oid in recipients:
             connection = connections.get(oid)
             if connection != None:
-                connection.sock.send(message)
+                self.logger.debug("sending: %s, to: %s", str(message), str(connection))
+                try:
+                    connection.sock.send(message)
+                except TimeoutError:
+                    self.logger.debug("failed to send message to %s with timeout error", str(connection.get_oid()))
+                except BrokenPipeError:
+                    self.logger.warning("failed to send message to %s with broken pipe error", str(connection.get_oid()))
+                except OSError as os_err:
+                    self.logger.warning("failed to send message to %s with os error %s", str(connection.get_oid()), str(os_err))
 
-    def send_message_to_all(self, connections:Dict[str, SSLCoTConnection], message: bytes):
+    def send_message_to_all(self, connections:Dict[str, TCPCoTConnection], message: bytes):
         """send a message to all connections
 
         Args:
-            connections (dict[str, SSLCoTConnection]): a dictionary of connections indexed by their OIDs
+            connections (dict[str, TCPCoTConnection]): a dictionary of connections indexed by their OIDs
             message (bytes): the message to be sent to some clients
         """
+        self.logger.debug("sending %s to %s", message, connections)
         for connection in connections.values():
-            connection.sock.send(message)
+            try:
+                connection.sock.send(message)
+            except TimeoutError:
+                self.logger.debug("failed to send message to %s with timeout error", str(connection.get_oid()))
+            except BrokenPipeError:
+                self.logger.warning("failed to send message to %s with broken pipe error", str(connection.get_oid()))
+            except OSError as os_err:
+                self.logger.warning("failed to send message to %s with os error %s", str(connection.get_oid()), str(os_err))
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/ssl_client_information.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/ssl_client_information.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/model/ssl_cot_connection.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/model/ssl_cot_connection.py`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/ssl_cot_service/ssl_cot_service_main.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/tcp_cot_service_main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,143 +1,203 @@
 from asyncio import Queue
 import threading
 import time
-import traceback
 from multiprocessing.pool import ThreadPool
 import os
 import multiprocessing
-import importlib
-import socket
 from opentelemetry.trace import Status, StatusCode
-from typing import List, Union, Dict
-from FreeTAKServer.services.ssl_cot_service.controllers.send_component_data_controller import SendComponentDataController
-from FreeTAKServer.services.ssl_cot_service.model.raw_ssl_connection_information import RawSSLConnectionInformation
-from FreeTAKServer.services.ssl_cot_service.model.ssl_cot_connection import SSLCoTConnection
+from typing import List, Dict
+from FreeTAKServer.services.tcp_cot_service.controllers.client_disconnection_controller import (
+    ClientDisconnectionController,
+)
+from FreeTAKServer.services.tcp_cot_service.controllers.send_component_data_controller import (
+    SendComponentDataController,
+)
+
+import traceback
 
 from digitalpy.core.service_management.digitalpy_service import DigitalPyService
 from digitalpy.core.domain.node import Node
 from digitalpy.core.main.object_factory import ObjectFactory
 from digitalpy.core.telemetry.tracer import Tracer
 from digitalpy.core.parsing.formatter import Formatter
 
 from FreeTAKServer.model.Enumerations.connectionTypes import ConnectionTypes
-from .controllers.SSLSocketController import SSLSocketController
-from FreeTAKServer.core.util.geo_manager_controller import GeoManagerController
-from FreeTAKServer.core.connection.ActiveThreadsController import ActiveThreadsController
+from .controllers.TCPSocketController import TCPSocketController
+from FreeTAKServer.core.connection.ActiveThreadsController import (
+    ActiveThreadsController,
+)
 from FreeTAKServer.core.connection.ClientInformationController import (
     ClientInformationController,
 )
 from FreeTAKServer.core.persistence.DatabaseController import (
     DatabaseController,
 )
 from .controllers.ReceiveConnections import ReceiveConnections
 from FreeTAKServer.core.connection.ReceiveConnectionsProcessController import (
     ReceiveConnectionsProcessController,
 )
 
 from .controllers.SendDataController import SendDataController
-from FreeTAKServer.core.SpecificCoTControllers.SendDisconnectController import (
-    SendDisconnectController,
-)
+
 from FreeTAKServer.core.parsers.XMLCoTController import XMLCoTController
 from FreeTAKServer.core.configuration.LoggingConstants import LoggingConstants
 
 from FreeTAKServer.model.RawCoT import RawCoT
-from FreeTAKServer.core.configuration.OrchestratorConstants import (
-    OrchestratorConstants,
-)
 from FreeTAKServer.model.FTSModel.Event import Event
 from FreeTAKServer.model.SpecificCoT.Presence import Presence
-from FreeTAKServer.model.SSLConnection import SSLConnection
 from FreeTAKServer.model.User import User
 from FreeTAKServer.model.ClientInformation import ClientInformation
 
-from .configuration.ssl_cot_service_constants import SERVICE_NAME
-from FreeTAKServer.core.configuration.CreateLoggerController import CreateLoggerController
+from .controllers.client_connection_controller import ClientConnectionController
+from .configuration.tcp_cot_service_constants import SERVICE_NAME
+from .model.tcp_cot_connection import TCPCoTConnection
+
+from FreeTAKServer.core.configuration.CreateLoggerController import (
+    CreateLoggerController,
+)
+
 loggingConstants = LoggingConstants()
-loggingConstants = LoggingConstants(log_name="FTS-SSL_CoT_Service")
+loggingConstants = LoggingConstants(log_name="TCPCoTService")
 logger = CreateLoggerController(
-    "FTS-SSL_CoT_Service", logging_constants=loggingConstants
+    "TCPCoTService", logging_constants=loggingConstants
 ).getLogger()
 
 from .controllers.ClientReceptionHandler import ClientReceptionHandler
 
 NODE_TO_XML = "NodeToXML"
 GET_MACHINE_READABLE_TYPE = "ConvertHumanReadableToMachineReadable"
-# TODO: the application protocol should be COT not SSL COT
 APPLICATION_PROTOCOL = "XML"
 # MAJOR TODO: Make explicit exception classes!!!
 
-class SSLCoTServiceMain(DigitalPyService):
-     # TODO: fix repeat attempts to add user
-    def __init__(self, service_id: str, subject_address: str, subject_port: int, subject_protocol, integration_manager_address: str, integration_manager_port: int, integration_manager_protocol: str, formatter: Formatter):
-        super().__init__(service_id, subject_address, subject_port, subject_protocol, integration_manager_address, integration_manager_port, integration_manager_protocol, formatter)
+
+class TCPCoTServiceMain(DigitalPyService):
+    """this service is responsible for handling the CoT listener for XML"""
+
+    # TODO: prevent repeat add user
+    def __init__(
+        self,
+        service_id,
+        subject_address,
+        subject_port,
+        subject_protocol,
+        integration_manager_address,
+        integration_manager_port,
+        integration_manager_protocol,
+        formatter: Formatter,
+    ):
+        super().__init__(
+            service_id,
+            subject_address,
+            subject_port,
+            subject_protocol,
+            integration_manager_address,
+            integration_manager_port,
+            integration_manager_protocol,
+            formatter
+        )
         self.logger = logger
 
         # Server info
         self.connection_received = 0
         self.sent_message_count = 0
         self.received_message_count = 0
         self.messages_to_core_count = 0
         self.messages_from_core_count = 0
         self.openSockets = 0
 
         # Contains info on clients
         self.client_information_queue = {}
         self.clientDataPipe: Queue
-        self.connections: dict[str, SSLCoTConnection] = {} # meant to eventually obsolete the client information queue
+        self.connections: Dict[
+            str, TCPCoTConnection
+        ] = {}  # meant to eventually obsolete the client information queue
 
         # instantiate controllers
         self.ActiveThreadsController = ActiveThreadsController()
         self.ClientInformationController = ClientInformationController()
         self.ReceiveConnections = ReceiveConnections()
         self.ReceiveConnectionsProcessController = ReceiveConnectionsProcessController()
         self.XMLCoTController = XMLCoTController()
         self.dbController: DatabaseController
-        self.send_component_data_controller = SendComponentDataController
-
-    @property
-    def connection_type(self):
-        return ConnectionTypes.SSL
+        self.send_component_data_controller = SendComponentDataController(self.logger)
+        self.client_connection_controller = ClientConnectionController(
+            self.logger,
+            self.client_information_queue,
+            self.connections,
+            self.openSockets
+        )
+        self.client_disconnection_controller = ClientDisconnectionController(
+            self.logger,
+            self.client_information_queue,
+            self.ActiveThreadsController,
+            self.connections,
+            self.openSockets,
+            self.connection_type,
+        )
 
-    def remove_service_user(self, clientInformation: ClientInformation):
-        """Generates the presence object from the
-        clientInformation parameter and sends it as a remove message
-        to the client data pipe
+    def start(
+        self,
+        IP,
+        CoTPort,
+        Event,
+        clientDataPipe,
+        ReceiveConnectionKillSwitch,
+        RestAPIPipe,
+        clientDataRecvPipe,
+        factory,
+        tracing_provider_instance
+    ):
+        try:
+            # configure the object factory with the passed factory instance
+            ObjectFactory.configure(factory)
 
-        Args:
-            clientInformation: Client information
+            # instantiate the tracer instance for this service
+            self.tracer: Tracer = tracing_provider_instance.create_tracer(SERVICE_NAME)
 
-        Returns: None
-        """
-        try:
-            # TODO this doesnt guarantee that put call will succeed, need to implement blocking...
-            if not self.clientDataPipe.full():
+            actionmapper = ObjectFactory.get_instance("actionMapper")
+            # subscribe to responses originating from this controller
+            actionmapper.add_topic(
+                f"/routing/response/{self.__class__.__name__.lower()}"
+            )
 
-                # Process removal of client in clientDataPipe
-                # TODO add blocking
-                self.clientDataPipe.put(
-                    [
-                        "remove",
-                        clientInformation,
-                        self.openSockets,
-                        self.connection_type,
-                    ]
-                )
-                self.logger.debug(
-                    f"Client removal has been sent through queue {str(clientInformation)}"
-                )
-            else:
-                self.logger.critical("Client data pipe is full!")
+            self.dbController = DatabaseController()
+            # self.clear_user_table()
+            os.chdir("../../../")
+            # create socket controller
+            self.TCPSocketController = TCPSocketController()
+            self.TCPSocketController.changeIP(IP)
+            self.TCPSocketController.changePort(CoTPort)
+            sock = self.TCPSocketController.createSocket()
+            pool = ThreadPool(processes=2)
+            self.pool = pool
+            self.clientDataRecvPipe = clientDataRecvPipe
+            clientData = pool.apply_async(
+                ClientReceptionHandler().startup, (self.client_information_queue,)
+            )
+            self.initialize_connections(APPLICATION_PROTOCOL)
+            receiveConnection = pool.apply_async(ReceiveConnections().listen, (sock,))
+            # instantiate domain model and save process as object
+            self.mainRunFunction(
+                clientData,
+                receiveConnection,
+                sock,
+                pool,
+                Event,
+                clientDataPipe,
+                ReceiveConnectionKillSwitch,
+                RestAPIPipe,
+            )
         except Exception as ex:
-            with self.tracer.start_as_current_span("remove_service_user") as span:
-                span.set_status(Status(StatusCode.ERROR))
-                span.record_exception(ex)
             raise ex
 
+    @property
+    def connection_type(self):
+        return ConnectionTypes.TCP
+
     def update_client_information(self, clientInformation: ClientInformation):
         """Generates a Presence object from the clientInformation parameter and
         sends it as an update message to the client data pipe.
 
         :param clientInformation: Client information
 
         Returns: None
@@ -167,54 +227,14 @@
                 self.logger.critical("client data pipe is Full !")
         except Exception as ex:
             with self.tracer.start_as_current_span("update_client_information") as span:
                 span.set_status(Status(StatusCode.ERROR))
                 span.record_exception(ex)
             raise ex
 
-    def add_service_user(self, clientInformation: ClientInformation):
-        """this method generates the presence and connection objects from the
-        clientInformation parameter and sends it to the clientDataPipe for processing
-
-        :param clientInformation: this is the information of the client to be added
-        """
-        try:
-            # TODO this doesnt guarantee that put call will succeed, need to implement blocking...
-            if not self.clientDataPipe.full():
-                presence_object = Presence()
-                presence_object.setModelObject(clientInformation.modelObject)
-
-                # TODO why is this not xmlString?
-                presence_object.setXmlString(clientInformation.idData)
-                # is this duplicate of modelobject ?
-                presence_object.setClientInformation(clientInformation.modelObject)
-
-                connection_object = SSLConnection()
-                # TODO: add certificate name derived from socket
-                connection_object.certificate_name = None
-                connection_object.sock = None
-                connection_object.user_id = clientInformation.modelObject.uid
-
-                # Updating clientDataPipe
-                # TODO add blocking...
-                self.clientDataPipe.put(
-                    ["add", presence_object, self.openSockets, connection_object]
-                )
-                self.logger.debug(
-                    "client addition has been sent through queue "
-                    + str(clientInformation)
-                )
-            else:
-                self.logger.critical("client data pipe is Full !")
-        except Exception as ex:
-            with self.tracer.start_as_current_span("add_service_user") as span:
-                span.set_status(Status(StatusCode.ERROR))
-                span.record_exception(ex)
-            raise ex
-
     def get_client_information(self):
         """this method gets client information from the client information pipe and returns it as a dict merged
         with the current client information list and updates the self variable
 
         :return:
         """
         try:
@@ -237,409 +257,62 @@
                     ):
                         self.client_information_queue[client_id].append(
                             user_dict[client_id]
                         )
 
                     elif (
                         client_id in user_dict.keys()
-                        and len(self.client_information_queue[client_id]) == 3
+                        and len(self.client_information_queue[client_id]) == 2
                     ):
-                        self.client_information_queue[client_id][1] = user_dict[client_id]
-
-                    # if the entry isn't present in FTS core than the client will be disconnected
-                    # and deleted to maintain single source of truth
-                    elif client_id not in user_dict.keys():
-                        self.logger.debug(
-                            f"disconnection client {str(client_id)} because client was not in FTS core user_dict"
-                        )
-                        self.disconnect_socket(
-                            self.client_information_queue[client_id][0]
-                        )
-                        del self.client_information_queue[client_id]
-
-                    # TODO this case will never happen
-                    else:
-                        self.logger.error(
-                            "the data for this client is invalid " + str(client_id)
-                        )
+                        self.client_information_queue[client_id][1] = user_dict[
+                            client_id
+                        ]
             else:
                 self.logger.critical("client data pipe is Full !")
         except Exception as ex:
             with self.tracer.start_as_current_span("get_client_information") as span:
                 span.set_status(Status(StatusCode.ERROR))
                 span.record_exception(ex)
 
-    # TODO make raise an exception
-    def send_user_connection_geo_chat(self, clientInformation):
-        """function to create and send pm to newly connected user
-
-        :param clientInformation: the object containing information about the user to which the msg is sent
-        :return:
-        """
-        # TODO: refactor as it has a proper implementation of a PM to a user generated by the server
-        from FreeTAKServer.core.SpecificCoTControllers.SendGeoChatController import (
-            SendGeoChatController,
-        )
-        from FreeTAKServer.model.RawCoT import RawCoT
-        from FreeTAKServer.model.FTSModel.Dest import Dest
-        import uuid
-
-        if OrchestratorConstants().DEFAULTCONNECTIONGEOCHATOBJ != None:
-            ChatObj = RawCoT()
-            ChatObj.xmlString = f"<event><point/><detail><remarks>{OrchestratorConstants().DEFAULTCONNECTIONGEOCHATOBJ}</remarks><marti><dest/></marti></detail></event>"
-
-            classobj = SendGeoChatController(ChatObj, AddToDB=False)
-            instobj = classobj.getObject()
-            instobj.modelObject.detail._chat.chatgrp.setuid1(
-                clientInformation.modelObject.uid
-            )
-            dest = Dest()
-            dest.setcallsign(clientInformation.modelObject.detail.contact.callsign)
-            instobj.modelObject.detail.marti.setdest(dest)
-            instobj.modelObject.detail._chat.setchatroom(
-                clientInformation.modelObject.detail.contact.callsign
-            )
-            instobj.modelObject.detail._chat.setparent("RootContactGroup")
-            instobj.modelObject.detail._chat.setid(clientInformation.modelObject.uid)
-            instobj.modelObject.detail._chat.setgroupOwner("True")
-            instobj.modelObject.detail.remarks.setto(clientInformation.modelObject.uid)
-            instobj.modelObject.setuid(
-                "GeoChat."
-                + "SERVER-UID."
-                + clientInformation.modelObject.detail.contact.callsign
-                + "."
-                + str(uuid.uuid1())
-            )
-            instobj.modelObject.detail._chat.chatgrp.setid(
-                clientInformation.modelObject.uid
-            )
-            classobj.reloadXmlString()
-            # self.get_client_information()
-            self.sent_message_count += 1
-            self.send_message(None, instobj, use_share_pipe=False)
-            return 1
-        else:
-            return 1
-
-    def clientConnected(self, raw_connection_information: RawSSLConnectionInformation):
-        """Controls the client connection sequence, calling methods which perform the following:
-            1. Instantiate the client object
-            2. Share the client with core
-            3. Add the client to the database
-            4. Send the connection message
-
-        :param raw_connection_information:
-        :return:
-        """
-        try:
-            from FreeTAKServer.core.persistence.EventTableController import (
-                EventTableController,
-            )
-
-            clientPipe = None
-
-            self.logger.info(loggingConstants.CLIENTCONNECTED)
-
-            # Instantiate the client object
-            clientInformation = self.ClientInformationController.intstantiateClientInformationModelFromConnection(
-                raw_connection_information, None
-            )
-
-            # TODO remove
-            if clientInformation == -1:
-                self.logger.info(
-                    "client had invalid connection information and has been disconnected"
-                )
-                return -1
-
-            # TODO remove or handle better
-            if not self.checkOutput(clientInformation):
-                raise Exception("Error in the creation of client information")
-            self.openSockets += 1
-            # breaks ssl
-            try:
-                if hasattr(clientInformation.socket, "getpeercert"):
-                    cn = "placeholder"
-                else:
-                    cn = None
-                CoT_row = EventTableController().convert_model_to_row(clientInformation.modelObject)
-                self.dbController.create_user(
-                    uid=clientInformation.modelObject.uid,
-                    callsign=clientInformation.modelObject.detail.contact.callsign,
-                    IP=clientInformation.IP,
-                    CoT=CoT_row,
-                    CN=cn,
-                )
-            except Exception as ex:
-                with self.tracer.start_as_current_span("clientConnected") as span:
-                    span.set_status(Status(StatusCode.ERROR))
-                    span.record_exception(ex)
-
-            self.logger.debug("Adding client...")
-            self.add_service_user(clientInformation=clientInformation)
-
-            # Add client info to queue
-            self.client_information_queue[clientInformation.modelObject.uid] = [clientInformation.socket, clientInformation, raw_connection_information.unwrapped_sock]
-            
-            # instantiate an object_id with a value of the client uid
-            object_id = ObjectFactory.get_new_instance("ObjectId", dynamic_configuration={"id": clientInformation.modelObject.uid, "type": "connection"})
-            
-            # TODO the instantiation of the connection object and the connection action
-            # call should be moved out of the tcp_cot_service main and into the connection
-            # controller
-            
-            # instantiate a new SSLCoTConnection with an object_id of the client uid
-            connection = SSLCoTConnection(object_id)
-            connection.model_object = clientInformation.modelObject
-            connection.sock = clientInformation.socket
-            self.connections[str(connection.get_oid())] = connection
-
-            # Update the iam component with the new client information
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("connection")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_value("connection", connection)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-            self.logger.debug("Client saved")
-
-            # Broadcast user in geochat
-            self.send_user_connection_geo_chat(clientInformation)
-
-            # Send emergency information to newly connected client
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("SendEmergenciesToClient")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_value("user", connection)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-
-            
-            # Send repeated messages to newly connected clients
-            request = ObjectFactory.get_new_instance("request")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_action("connection")
-            request.set_context("Repeater")
-            request.set_value("connection", connection)
-            request.set_value("recipients", [str(connection.get_oid())])
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-
-            return clientInformation
-        except Exception as e:
-            self.logger.warning(loggingConstants.CLIENTCONNECTEDERROR)
-
-
-    def dataReceived(self, raw_cot: RawCoT):
-        """this will be executed in the event that the use case for the CoT isn't specified in the orchestrator
-
-        :param raw_cot: the CoT to be processed and shared
-        """
-        try:
-            # this will check if the CoT is applicable to any specific controllers
-            raw_cot = self.XMLCoTController.determineCoTType(raw_cot)
-
-            # the following calls whatever controller was specified by the above function
-            module = importlib.import_module(
-                "FreeTAKServer.core.SpecificCoTControllers." + raw_cot.CoTType
-            )
-            CoTSerializer = getattr(module, raw_cot.CoTType)
-            # TODO: improve way in which the dbController is passed to CoTSerializer
-            raw_cot.dbController = self.dbController
-            processedCoT = CoTSerializer(raw_cot).getObject()
-
-            # this statement checks if the data type is a user update and if so it will be saved to the associated client object
-            if raw_cot.CoTType == "SendUserUpdateController":
-                # find entry with this uid
-                self.update_client_information(clientInformation=processedCoT)
-            return processedCoT
-        except Exception as e:
-            self.logger.error(loggingConstants.DATARECEIVEDERROR + str(e))
-            return -1
-
-    def clientDisconnected(self, clientInformation: User):
-        """Handles the disconnection of clients
-
-        :param clientInformation:
-        :return:
-        """
-        import traceback
-
-        self.logger.debug("Disconnecting client")
-
-        # TODO add proper exception handling
-        # Get socket info from client object
-        try:
-            if isinstance(clientInformation, str):
-                clientInformation = self.client_information_queue[clientInformation][1]
-            elif isinstance(clientInformation, RawCoT):
-                clientInformation = self.client_information_queue[
-                    clientInformation.clientInformation
-                ][1]
-            sock = self.client_information_queue[clientInformation.user_id][0]
-            unwrapped_sock = self.client_information_queue[clientInformation.user_id][2]
-        except Exception as e:
-            self.logger.critical(
-                "getting sock from client information queue failed " + str(e)
-            )
-
-        try:
-            self.logger.debug(
-                "client "
-                + clientInformation.m_presence.modelObject.uid
-                + " disconnected "
-                + "\n".join(traceback.format_stack())
-            )
-        except Exception as e:
-            self.logger.critical(
-                "there was an error logging disconnection information " + str(e)
-            )
-
-        # Removes the user id from client info queue
-        try:
-            del self.client_information_queue[clientInformation.user_id]
-            # Update the iam component with the new client information
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("disconnection")
-            request.set_sender(self.__class__.__name__.lower())
-            if hasattr(clientInformation, "modelObject"):
-                uid = clientInformation.modelObject.uid
-            elif hasattr(clientInformation, "m_presence"):
-                uid = clientInformation.m_presence.modelObject.uid
-            conn_id = str(ObjectFactory.get_instance("ObjectId", {"id": uid, "type": "connection"}))
-            del self.connections[conn_id]
-            request.set_value("connection_id", conn_id)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-        except Exception as e:
-            self.logger.critical("client removal failed " + str(e))
-
-        # Remove the active thread and database connection
-        try:
-            self.ActiveThreadsController.removeClientThread(clientInformation)
-            self.dbController.remove_user(query=f'uid = "{clientInformation.user_id}"')
-        except Exception as e:
-            self.logger.critical(
-                f"There has been an error in a clients disconnection while adding information to the database {str(e)}"
-            )
-
-        try:
-            self.remove_service_user(clientInformation=clientInformation)
-            self.disconnect_socket(sock, unwrapped_sock)
-
-            self.logger.info(loggingConstants.CLIENTDISCONNECTSTART)
-
-            # TODO: remove string
-            self.send_disconnect_cot(clientInformation)
-            self.logger.info(
-                loggingConstants.CLIENTDISCONNECTEND
-                + str(clientInformation.m_presence.modelObject.uid)
-            )
-            return 1
-        except Exception as e:
-            import traceback
-            import sys, linecache
-
-            exc_type, exc_obj, tb = sys.exc_info()
-            f = tb.tb_frame
-            lineno = tb.tb_lineno
-            filename = f.f_code.co_filename
-            linecache.checkcache(filename)
-            line = linecache.getline(filename, lineno, f.f_globals)
-            self.logger.error(
-                loggingConstants.CLIENTCONNECTEDERROR
-                + " "
-                + str(e)
-                + " on line: "
-                + line
-            )
+    def component_handler(self, xml_cot):
+        """this method is responsible for handling cases where the cot sent should
+        be handled (parsed and manipulated) by a specific component it is
+        responsible for calling the routing (via the async action mapper)
+        of the CoT data
 
-    def send_disconnect_cot(self, clientInformation):
-        """send the disconnection information for a specific client to all connected clients
         Args:
-            clientInformation: client to be displayed as
-                disconnected by all connected devices
+            xml_cot (str): xml representation of CoT
         """
-        # TODO: remove string
-        tempXml = RawCoT()
-        tempXml.xmlString = '<event><detail><link uid="{0}"/></detail></event>'.format(
-            clientInformation.user_id
-        ).encode()
-        disconnect = SendDisconnectController(tempXml)
-        self.get_client_information()
-        self.sent_message_count += 1
-        self.messages_to_core_count += 1
-        self.send_message(disconnect.getObject().clientInformation, disconnect.getObject())
 
-    def disconnect_socket(self, sock: socket.socket, unwrapped_socket: socket.socket) -> None:
-        """this method is responsible for disconnecting all socket objects
-
-        :param sock: socket object to be disconnected
-        """
-        self.logger.debug("Shutting down socket")
-        try:
-            sock.shutdown(socket.SHUT_RDWR)
-        except Exception as e:
-            self.logger.error(
-                "Error shutting socket down in client disconnection "
-                + str(e)
-                + "\n".join(traceback.format_stack())
-            )
-        try:
-            sock.close()
-        except Exception as e:
-            self.logger.error(
-                "error closing socket in client disconnection "
-                + str(e)
-                + "\n".join(traceback.format_stack())
-            )
-        try:
-            unwrapped_socket.close()
-        except Exception as e:
-            self.logger.error(
-                "error closing unwrapped socket in client disconnection "
-                + str(e)
-                + "\n".join(traceback.format_stack())
-            )
-
-    def component_handler(self, cot):
-        """this method is responsible for handling cases where the cot sent should
-        be handled (parsed and manipulated) by a specific component it is
-        responsible for calling the routing (via the async action mapper)
-        of the CoT data"""
-        if not hasattr(cot, "xmlString"):
-            raise ValueError("cot missing required attribute 'xmlString'")
+        dict_cot = self.convert_xml_to_dict(xml_cot)
 
         request = ObjectFactory.get_new_instance("request")
         # must get a new instance of the async action mapper for each request
         # to prevent run conditions and to prevent responses going to the wrong
         # callers
-        actionmapper = ObjectFactory.get_instance("actionMapper")
         response = ObjectFactory.get_new_instance("response")
 
         # instantiate and define the request
         request = ObjectFactory.get_new_instance("request")
         request.set_format("pickled")
-        request.set_action(cot.data_dict["event"]["@type"])
-        request.set_context("XML")
+        human_readable_type = self.get_human_readable_type(dict_cot)
+        request.set_action(human_readable_type)
+        request.set_context("XMLCoT")
         request.set_sender(self.__class__.__name__.lower())
-        request.set_value("dictionary", cot.data_dict)
+        request.set_value("dictionary", dict_cot)
 
         # instantiate and define the response
         response = ObjectFactory.get_new_instance("response")
         response.set_format("pickled")
 
         # final request for the actual cot but listener is not returned because
         # it should be handled by the main loop which listens for all responses
         # with a request source of Orchestrator
+        self.logger.debug("sending request to subject %s", str(request.get_values()))
         self.subject_send_request(request, APPLICATION_PROTOCOL)
-        
-        # one is returned so that the message is ignored and can be processed later once the
-        # response is received by the component receiver
-        return 1
 
     def convert_to_xml(self, model_object: Node) -> str:
         """call the domain component to convert the model object to xml
         Args:
             model_object (Node): the model object to convert it's xml representation
 
         Returns:
@@ -710,69 +383,86 @@
 
                 # Check if the response model object is a list
                 if isinstance(response.get_value("message"), list):
                     for model_object in response.get_value("message"):
                         self.send_component_message(response, model_object)
                 else:
                     self.send_component_message(response, response.get_value("message"))
-            except Exception as e:
+            except Exception as ex:
                 self.logger.error(
                     f"There was an exception sending a single response:\n"
                     f"Sender: {sender}\n"
-                    f"Model object: {model_object}\n"
                     f"Context: {response.get_context()}\n"
                     f"Action: {response.get_action()}\n"
+                    f"Exception: {str(ex)}"
+                )
+                self.logger.debug(
+                    "single response exception traceback: %s", traceback.format_exc()
                 )
 
     def send_component_message(self, request, message):
-        response = ObjectFactory.get_instance("response")
-        send_component_data_controller_inst = self.send_component_data_controller(None, None, None, None)
-        send_component_data_controller_inst.initialize(request, response)
-        send_component_data_controller_inst.send_message(self.connections, message, request.get_value("recipients"))
+        self.send_component_data_controller.send_message(
+            self.connections, message, request.get_value("recipients")
+        )
 
     def send_message(self, sender, message, use_share_pipe=True):
-        if not use_share_pipe:
-            cot_share_pipe = None
-        else: 
-            cot_share_pipe = self.CoTSharePipe
         return SendDataController().sendDataInQueue(
-                    sender,
-                    message,  # pylint: disable=no-member; isinstance checks that CoTOutput is of proper type
-                    self.client_information_queue,
-                    cot_share_pipe,
-                )
+            sender,
+            message,  # pylint: disable=no-member; isinstance checks that CoTOutput is of proper type
+            self.client_information_queue,
+            self.CoTSharePipe,
+        )
+
+    def convert_xml_to_dict(self, data) -> dict:
+        """convert the xml format to a dict containing the same data via the xml_serializer
+        component.
+
+        Args:
+            data (str): an xml string containing the data from a given client
 
-    def monitor_raw_cot(self, data: RawCoT) -> object:
+        Returns:
+            dict: dictionary representation of the cot data
         """
-        This method takes as input a sent CoT and calls its associated function. This method supports three handlers defined
-        in XMLCoTController which handle connect, disconnect, and misc messages respectively.
+        request = ObjectFactory.get_new_instance("request")
+        request.set_action("XMLToDict")
+        request.set_value("message", data)
+
+        actionmapper = ObjectFactory.get_instance("syncactionMapper")
+        response = ObjectFactory.get_new_instance("response")
+        actionmapper.process_action(request, response)
+
+        # dictionary representation of the xml
+        data_dict = response.get_value("dict")
+        return data_dict
+
+    def get_human_readable_type(self, dict_cot: dict) -> str:
+        """parse the cot type and send request to the type component to
+        convert it to a human readable type
 
         Args:
-            data (RawCoT): The raw CoT data to be processed.
+            dict_cot (dict): cot message in dictionary format
 
         Returns:
-            object: The output of the handler function called on the CoT data.
+            str: the human readable
         """
-        try:
-            if isinstance(data, int):
-                return None
-            else:
-                cot = XMLCoTController(logger=self.logger).determineCoTGeneral(data, self.client_information_queue)
-                handler_name, handler_data = cot
-                handler = getattr(self, handler_name, None)
-                if handler is None:
-                    self.logger.error(f"No handler found for {handler_name}")
-                    return -1
-                output = handler(handler_data)
-                if output != 1:  # when the process is a disconnect the output is 1
-                    output.clientInformation = self.client_information_queue[data.clientInformation][1]
-                return output
-        except Exception as e:
-            self.logger.error(loggingConstants.MONITORRAWCOTERRORB + str(e))
-            return -1
+        # this convert the machine readable type to a human readable type
+        request = ObjectFactory.get_new_instance("request")
+        request.set_format("pickled")
+        request.set_action("ConvertMachineReadableToHumanReadable")
+        request.set_context("MEMORY")
+        request.set_value("machine_readable_type", dict_cot["event"]["@type"])
+        request.set_value("default", dict_cot["event"]["@type"])
+
+        # must get a new instance of the async action mapper for each request
+        # to prevent run conditions and to prevent responses going to the wrong
+        # callers
+        actionmapper = ObjectFactory.get_instance("syncactionMapper")
+        response = ObjectFactory.get_new_instance("response")
+        actionmapper.process_action(request, response)
+        return response.get_value("human_readable_type")
 
     # TODO Remove or replace
     def checkOutput(self, output):
         """this method checks whether or not the return data was valid
 
         :param output: any type which was returned by a function
         :rtype: bool indicating whether the output was valid or not
@@ -827,14 +517,16 @@
         receiveconntimeoutcount = datetime.datetime.now()
         lastprint = datetime.datetime.now()
         start_timer = time.time() - 60
 
         while event.is_set():
             self.CoTSharePipe = CoTSharePipe
             try:
+                if ssl == True:
+                    pass
                 self.clientDataPipe = clientDataPipe
                 if event.is_set():
                     try:
                         if ReceiveConnectionKillSwitch.is_set():
                             try:
                                 receiveConnection.successful()
                             except:
@@ -848,36 +540,34 @@
                             receiveConnectionOutput = receiveConnection.get(
                                 timeout=0.01
                             )
                             self.connection_received += 1
                             print(self.connection_received)
                             receiveConnection = pool.apply_async(
                                 ReceiveConnections().listen,
-                                (
-                                    sock,
-                                ),
+                                (sock,),
                             )
                             receiveconntimeoutcount = datetime.datetime.now()
                             lastprint = datetime.datetime.now()
-                            CoTOutput = self.handle_connection_data(
+                            CoTOutput = self.handle_connection(
                                 receiveConnectionOutput
                             )
 
                     except multiprocessing.TimeoutError:
 
                         if (
                             datetime.datetime.now() - receiveconntimeoutcount
                         ) > datetime.timedelta(seconds=60) and ssl == True:
                             from multiprocessing.pool import ThreadPool
 
                             try:
                                 pass
                             except Exception as e:
                                 print(str(e))
-                        elif (
+                        elif ssl == True and (
                             datetime.datetime.now() - lastprint
                         ) > datetime.timedelta(seconds=30):
                             print(
                                 "time since last reset "
                                 + str(datetime.datetime.now() - receiveconntimeoutcount)
                             )
                             lastprint = datetime.datetime.now()
@@ -903,15 +593,15 @@
                                 recent_client_data_output = (
                                     clientDataOutput,
                                     time.time(),
                                 )
                             self.received_message_count += len(
                                 clientDataOutput
                             )  # add the length of this list to the number of received messages
-                            CoTOutput = self.handle_regular_data(clientDataOutput)
+                            self.handle_regular_data(clientDataOutput)
                         else:
                             clientData = pool.apply_async(
                                 ClientReceptionHandler().startup,
                                 (self.client_information_queue,),
                             )
                             raise Exception(
                                 "client reception handler has returned data which is not of type list data is "
@@ -962,16 +652,16 @@
                     if time.time() > start_timer + 60:
                         start_timer = time.time()
                         self.logger.debug(str("mainRunFunction is running"))
                         # self.logger.debug('CoTSharePipe is full ' + str(CoTSharePipe.full()))
                         # self.logger.debug('clientDataPipe is full ' + str(clientDataPipe.full()))
                         if "recent_client_data_output" in locals():
                             self.logger.debug(
-                                "most recent client data "
-                                + str(recent_client_data_output)
+                                "most recent client data %s",
+                                str(recent_client_data_output),
                             )
                             self.logger.debug(
                                 "time since last valid data "
                                 + str(time.time() - recent_client_data_output[1])
                             )
                             self.logger.debug(
                                 "content of last valid data "
@@ -985,188 +675,129 @@
                         "the periodic debug message has thrown an error " + str(e)
                     )
             except Exception as e:
                 self.logger.info(
                     "there has been an uncaught error thrown in mainRunFunction"
                     + str(e)
                 )
-                pass
         self.stop()
 
     def handle_shared_data(self, modelData):
         """this method is responsible for receiving and forwarding data shared via IPC
 
         :param modelData:
         :return:
         """
         try:
             self.get_client_information()
             self.messages_from_core_count += 1
             if hasattr(modelData, "clientInformation"):
                 self.sent_message_count += 1
-                self.send_message(modelData.clientInformation, modelData, use_share_pipe=False)
+                self.send_message(
+                    modelData.clientInformation, modelData, use_share_pipe=False
+                )
             else:
                 self.sent_message_count += 1
                 self.send_message(None, modelData, use_share_pipe=False)
-        except Exception as e:
-            self.logger.error("data base connection error " + str(e))
-    
+        except Exception as ex:
+            self.logger.error("data base connection error " + str(ex))
+
     def handle_regular_data(self, clientDataOutput: List[RawCoT]):
         """
         Handle "regular" data being sent by clients. Regular data is data that is neither a new connection nor a disconnection.
 
         This method initiates the serialization and distribution of regular data.
 
         Args:
             clientDataOutput (List[RawCoT]): List of RawCoT objects
 
         Returns:
             None
         """
         # Iterate through each piece of client data
         try:
-            for clientDataOutputSingle in clientDataOutput:
+            for data_object in clientDataOutput:
                 try:
+                    self.logger.debug(f"begginning processing {data_object.xmlString}")
                     # Skip this iteration if the data is invalid
-                    if clientDataOutputSingle == -1:
+                    if data_object == -1:
                         continue
-
-                    # Process the raw CoT data and serialize it
-                    CoTOutput = self.monitor_raw_cot(clientDataOutputSingle)
-                    # Skip this iteration if the CoT data is invalid
-                    if CoTOutput == 1:
+                    elif data_object.xmlString == b"":
+                        self.handle_disconnection(data_object.clientInformation)
                         continue
-                    
-                    self.logger.info(f"CoT serialized {CoTOutput.modelObject.uid}")
+                    # Process the raw CoT data and serialize it
+                    self.component_handler(data_object.xmlString)
+                    self.logger.debug(f"finished processing {data_object.xmlString}")
 
-                    # Check if the CoT data is valid and can be sent
-                    if self.checkOutput(CoTOutput):
-                        # Get client information and send the message
-                        self.get_client_information()
-                        self.sent_message_count += 1
-                        self.messages_to_core_count += 1
-                        output = self.send_message(CoTOutput.clientInformation, CoTOutput)
-
-                        # Check if the message was sent successfully
-                        if self.checkOutput(output) and not isinstance(output, tuple):
-                            # Message was sent successfully
-                            pass
-                        elif isinstance(output, tuple):
-                            # There was an issue sending the message, so disconnect the client
-                            self.logger.error("Issue sending data to client, now disconnecting")
-                            self.clientDisconnected(output[1])
-                        else:
-                            # There was an issue sending the message
-                            self.logger.error(f"Send data failed with data {CoTOutput.xmlString} from client {CoTOutput.clientInformation.modelObject.detail.contact.callsign}")
-                    else:
-                        # The CoT data is invalid, raise an exception
-                        raise Exception("Error in general data processing")
-                except Exception as e:
-                    self.logger.info(f"Exception in client data processing within main run function {e} data is {CoTOutput}")
-        except Exception as e:
-            self.logger.info(f"Error iterating client data output {e}")
+                except Exception as ex:
+                    self.logger.error(
+                        f"Exception in client data processing within main run function {ex} data is {data_object.xmlString} trace is {traceback.format_exc()}"
+                    )
+                    continue
+        except Exception as ex:
+            self.logger.info(f"Error iterating client data output {ex}")
             return -1
         return 1
 
+    def handle_disconnection(self, client_information):
+        """handle a client disconnection from the service by disconnecting the socket and informing clients of the disconnection
+
+        Args:
+            client_information (_type_): _description_
+        """
+        sock = self.client_disconnection_controller.get_sock(client_information)
+        
+        self.client_disconnection_controller.delete_client_connection(client_information)
+
+        self.client_disconnection_controller.disconnect_socket(sock)
+
+        connection_id = self.client_disconnection_controller.get_connection_id(client_information)
+
+        iam_disconnect_request = self.client_disconnection_controller.create_iam_disconnect_request(connection_id)
+        self.subject_send_request(iam_disconnect_request, APPLICATION_PROTOCOL)
 
-    def handle_connection_data(self, receive_connection_output: RawCoT) -> None:
+        self.client_disconnection_controller.send_disconnect_cot(client_information)
+
+    def handle_connection(self, receive_connection_output: RawCoT) -> None:
         """this method should be called to initiate the process for receiving new connection data
         :rtype: None
         :param receive_connection_output: a RawCoT object from a newly connected client
         """
         try:
             self.logger.debug("Handling connection data")
             if receive_connection_output == -1:
                 return None
 
-            CoTOutput = self.monitor_raw_cot(receive_connection_output)
-            if CoTOutput != -1 and CoTOutput != None and CoTOutput != 1:
-                self.sent_message_count += 1
-                output = self.send_message(CoTOutput, CoTOutput)
+            client_connection, client_information = self.client_connection_controller.create_client_connection(
+                receive_connection_output, self.dbController
+            )
+            self.client_connection_controller.save_client_to_db(client_information, self.dbController)
+            
+            iam_request = self.client_connection_controller.create_iam_request(client_connection)
+            self.subject_send_request(iam_request, APPLICATION_PROTOCOL)
+            
+            repeated_messages_request = self.client_connection_controller.create_send_repeated_messages_request(client_connection)
+            self.subject_send_request(repeated_messages_request, APPLICATION_PROTOCOL)
+            
+            send_emergencies_request = self.client_connection_controller.create_send_emergencies_request(client_connection)
+            self.subject_send_request(send_emergencies_request, APPLICATION_PROTOCOL)
+
+            self.client_connection_controller.send_user_connection_geo_chat(client_information)
+
+            # self.handle_regular_data([receive_connection_output])
 
-                if self.checkOutput(output):
-                    self.logger.debug(
-                        f"Connection data from client {CoTOutput.modelObject.detail.contact.callsign} successfully processed."
-                    )
-                else:
-                    raise Exception("error in sending data")
         except Exception as e:
             self.logger.error(
                 "exception in receive connection data processing within main run function "
                 + str(e)
-                + " data is "
-                + str(CoTOutput)
             )
-            return -1
-        return 1
-
-    def start(
-        self,
-        IP,
-        CoTPort,
-        Event,
-        clientDataPipe,
-        ReceiveConnectionKillSwitch,
-        RestAPIPipe,
-        clientDataRecvPipe,
-        factory,
-        tracing_provider_instance
-    ):
-        try:
-             # configure the object factory with the passed factory instance
-            ObjectFactory.configure(factory)
-
-            # instantiate the tracer instance for this service
-            self.tracer: Tracer = tracing_provider_instance.create_tracer(
-                SERVICE_NAME
-            )
-            
-            actionmapper = ObjectFactory.get_instance("actionMapper")
-            # subscribe to responses originating from this controller
-            actionmapper.add_topic(
-                f"/routing/response/{self.__class__.__name__.lower()}"
-            )
-
-            self.dbController = DatabaseController()
-            print("ssl cot service starting")
-            os.chdir("../../")
-            # create socket controller
-            self.SSLSocketController = SSLSocketController()
-            self.SSLSocketController.changeIP(IP)
-            self.SSLSocketController.changePort(CoTPort)
-            sock = self.SSLSocketController.createSocket()
-            # threadpool is used as it allows the transfer of SSL socket unlike processes
-            pool = ThreadPool(processes=2)
-            self.clientDataRecvPipe = clientDataRecvPipe
-            self.pool = pool
-            clientData = pool.apply_async(
-                ClientReceptionHandler().startup, (self.client_information_queue,)
-            )
-            self.initialize_connections(APPLICATION_PROTOCOL)
-
-            receiveConnection = pool.apply_async(ReceiveConnections().listen, (sock,))
-            # instantiate domain model and save process as object
-            self.mainRunFunction(
-                clientData,
-                receiveConnection,
-                sock,
-                pool,
-                Event,
-                clientDataPipe,
-                ReceiveConnectionKillSwitch,
-                RestAPIPipe,
-                True,
-            )
-        except Exception as e:
-            print(e)
-            logger.error(
-                "there has been an exception thrown in"
-                " the starting of the ssl service " + str(e)
+            self.logger.debug(
+                "with traceback: %s", traceback.format_exc()
             )
-            return e
+        return 1
 
     def stop(self):
         self.clientDataPipe.close()
         self.pool.terminate()
         self.pool.close()
         self.pool.join()
 
@@ -1194,15 +825,15 @@
                 self.logger.debug(
                     f"messages shared with core in {logging_interval} seconds: {self.messages_to_core_count}"
                 )
                 self.logger.debug(
                     f"messages shared with core in {logging_interval} seconds: {self.messages_from_core_count}"
                 )
                 self.logger.debug(
-                    f"number of connected client: {str(len(self.client_information_queue.keys()))}"
+                    f"number of connected client: {str(len(self.connections.keys()))}"
                 )
                 self.sent_message_count = 0
                 self.received_message_count = 0
                 self.messages_to_core_count = 0
                 self.messages_from_core_count = 0
             except Exception as e:
                 self.logger.critical("logging service failed with exception " + str(e))
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/ClientReceptionHandler.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/ClientReceptionHandler.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,15 @@
         try:
             self.clientInformationArray = clientInformationArray  # create copy of client information array so it cant be changed during iteration
             '''logger.propagate = False
             logger.info(loggingConstants.CLIENTRECEPTIONHANDLERSTART)
             logger.propagate = True'''
             output = self.monitorForData(self.dataPipe)
             if output == 1:
+                if len(self.dataPipe)>0: logger.debug("returning data array %s", str(self.dataPipe))
                 return self.dataPipe
             else:
                 return -1
             '''
             time.sleep(600)
             # temporarily remove due to being unnecessary and excessively flooding logs
             logger.info('the number of threads is ' + str(threading.active_count()) + ' monitor event process alive is ' + str(monitorEventProcess.is_alive()) +
@@ -64,47 +65,81 @@
                 sock = self.clientInformationArray[user_id][0]
                 client = user_id
                 #client = self.clientInformationArray[user_id][1]
                 try:
                     sock.settimeout(0.001)
                     try:
                         xmlstring = self.recv_until(sock).decode()
+                        logger.debug("received raw data %s", str(xmlstring))
                         if xmlstring == b'' or xmlstring == '' or xmlstring is None: 
+                            #xmlstring = self.validate_client_disconnect(queue, sock, client)
+                            #if xmlstring is None:
+                            #    continue
                             self.returnReceivedData(client, b'', queue)
-                            logger.debug("empty string sent, standard disconnect")
                             continue
                         xmlstring = "<multiEvent>" + xmlstring + "</multiEvent>"  # convert to xmlstring wrapped by multiEvent tags
-                        xmlstring = re.sub(r'(?s)\<\?xml(.*)\?\>', '', xmlstring)  # replace xml definition tag with empty string as it breaks serilization
+                        xmlstring = re.sub(r"<\?xml.*?\?>", '', xmlstring)  # replace xml definition tag with empty string as it breaks serilization
+                        logger.debug("data after xmltag substitution: %s", xmlstring)
                         events = etree.fromstring(xmlstring)  # serialize to object
                         for event in events.findall('event'):
+                            event_str = etree.tostring(event)
+                            logger.debug("received: %s from %s", event_str, client)
                             self.returnReceivedData(client, etree.tostring(event), queue)  # send each instance of event to the core
-                    except socket.timeout as e:
+                    except socket.timeout:
                         continue
-                    except BrokenPipeError as e:
+                    except BrokenPipeError as ex:
+                        logger.debug("disconnecting client %s due to broken pipe", client)
                         self.returnReceivedData(client, b'', queue)
                         continue
-                    except Exception as e:
+                    except ConnectionAbortedError as ex:
+                        logger.debug("disconnecting client %s due to connection aborted", client)
+                        self.returnReceivedData(client, b'', queue)
+                        continue
+                    except ConnectionResetError as ex:
+                        logger.debug("disconnecting client %s due to connection reset", client)
+                        self.returnReceivedData(client, b'', queue)
+                        continue
+                    except Exception as ex:
                         import traceback
-                        if hasattr(e, "errno") and e.errno == errno.EWOULDBLOCK:  # this prevents errno 11 from spontanieously disconnecting clients due to the socket blocking set to 0
-                            logger.debug("EWOULDBLOCK error passed " + str(e))
+                        if hasattr(ex, "errno") and ex.errno == errno.EWOULDBLOCK:  # this prevents errno 11 from spontanieously disconnecting clients due to the socket blocking set to 0
+                            logger.debug("EWOULDBLOCK error passed " + str(ex))
                             continue
                         logger.error(
-                            "Exception other than broken pipe in monitor for data function " + str(e) + ''.join(traceback.format_exception(None, e, e.__traceback__)))
+                            "Exception other than broken pipe in monitor for data function " + str(ex) + ''.join(traceback.format_exception(None, ex, ex.__traceback__)))
                         self.returnReceivedData(client, b'', queue)
                         continue
 
-                except Exception as e:
-                    logger.error(loggingConstants.CLIENTRECEPTIONHANDLERMONITORFORDATAERRORD + str(e))
+                except Exception as ex:
+                    logger.error(loggingConstants.CLIENTRECEPTIONHANDLERMONITORFORDATAERRORD + str(ex))
                     self.returnReceivedData(client, b'', queue)
                     # return -1 commented out so entire run isn't stopped because of one disconnect
             return 1
-        except Exception as e:
-            logger.error('exception in monitor for data ' + str(e))
+        except Exception as ex:
+            logger.error('exception in monitor for data ' + str(ex))
             return -1
 
+    def validate_client_disconnect(self, queue, sock, client):
+        """ensure that the client is correctly disconnected
+
+        Args:
+            queue (_type_): _description_
+            sock (_type_): _description_
+            client (_type_): _description_
+
+        Returns:
+            _type_: _description_
+        """
+        for _ in range(10):
+            xmlstring = self.recv_until(sock).decode()
+            if xmlstring != b'' or xmlstring != '' or xmlstring is not None:
+                return xmlstring
+        logger.debug("empty string sent from %s, standard disconnect", client)
+        self.returnReceivedData(client, b'', queue)
+        return None
+    
     def returnReceivedData(self, clientInformation, data, queue):
         try:
             from FreeTAKServer.model.RawCoT import RawCoT
             RawCoT = RawCoT()
             RawCoT.clientInformation = clientInformation
             RawCoT.xmlString = data.replace(b'\n', b'')  # replace all newlines with empty
             self.dataPipe.append(RawCoT)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/ReceiveConnections.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/ReceiveConnections.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 # Generated by Enterprise Architect
 # Created on:      19-May-2020 6:21:05 PM
 # Original author: Natha Paquette
 # 
 #######################################################
 import asyncio
 import socket
-import logging
 import logging.handlers
 import re
 from lxml import etree
 import time
 import os
 from typing import Union
 
@@ -87,17 +86,21 @@
 
         # logger = CreateLoggerController("ReceiveConnections").getLogger()
 
         # Listen for client connections
         sock.listen(ReceiveConnectionsConstants().LISTEN_COUNT)
 
         try:
-            # Accept a client connection
-            client, address = sock.accept()
 
+            try:
+                # Accept a client connection
+                client, address = sock.accept()
+            except socket.timeout:
+                logger.debug("tcp sock threw timeout error")
+                return -1
             # Receive data from the client
             try:
                 events = self.receive_connection_data(client=client)
             except Exception as e:
                 try:
                     events = self.receive_connection_data(client=client)
                 except Exception as e:
@@ -108,40 +111,39 @@
             # TODO: move out to separate function
             if events == TEST_SUCCESS:
                 client.send(b'success')
 
             # Set the socket to non-blocking
             client.settimeout(0)
 
-            # Log that a client was accepted
-            logger.info(loggingConstants.RECEIVECONNECTIONSLISTENINFO)
-
             # Instantiate a client object with the received data
             raw_connection_information = self.instantiate_client_object(address, client, events)
-            logger.info("Client accepted")
+
+            # Log that a client was accepted
+            logger.info(loggingConstants.RECEIVECONNECTIONSLISTENINFO)
 
             # Return the client object if it is valid, or -1 if it is not
             try:
                 if sock is not None and raw_connection_information.xmlString != b'':
                     return raw_connection_information
                 else:
                     logger.warning("Final socket entry is invalid")
                     client.close()
                     return -1
-            except Exception as e:
+            except Exception as ex:
                 client.close()
-                logger.warning('Exception in returning data ' + str(e))
+                logger.warning('Exception in returning data ' + str(ex))
                 return -1
                 
-        except Exception as e:
-            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR)
+        except Exception as ex:
+            logger.warning(loggingConstants.RECEIVECONNECTIONSLISTENERROR + ": %s", str(ex))
             try:
                 client.close()
-            except Exception as e:
-                pass
+            except Exception as ex_sub:
+                logger.error("unhandled exception %s", str(ex_sub))
             finally:
                 return -1
 
 
     def instantiate_client_object(self, address, client, events):
         raw_connection_information = sat()
         raw_connection_information.ip = address[0]
@@ -157,14 +159,16 @@
             delimiter (bytes): bytestring representing the delimiter
 
         Returns:
             Union[None, bytes]: None if no data was received otherwise send received data
         """        
         message = b""
         start_receive_time = time.time()
+        received_count = 0
         client.settimeout(4)
-        while delimiter not in message and time.time() - start_receive_time <= ReceiveConnectionsConstants().RECEIVECONNECTIONDATATIMEOUT:
+        while delimiter not in message and time.time() - start_receive_time <= ReceiveConnectionsConstants().RECEIVECONNECTIONDATATIMEOUT and received_count <= ReceiveConnectionsConstants().MAX_RECEPTION_ITERATIONS:
             try:
+                received_count += 1
                 message = message + client.recv(ReceiveConnectionsConstants().CONNECTION_DATA_BUFFER)
             except:
                 return message
         return message
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/controllers/SendDataController.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/controllers/SendDataController.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                             if (
                                 client[1].m_presence.modelObject.detail.contact.callsign
                                 == dest
                             ):
                                 sock = client[0]
                                 try:
                                     sock.send(processedCoT.xmlString)
-                                    logger.info(
+                                    logger.debug(
                                         str(processedCoT.xmlString)
                                         + " sent to client "
                                         + client_id
                                     )
                                 except Exception as e:
                                     logger.error(
                                         "error sending data with marti to client data "
@@ -164,23 +164,23 @@
                 try:
                     if hasattr(processedCoT, "xmlString"):
                         # print('sending to all ' + str(processedCoT.xmlString))
                         try:
                             sock.send(processedCoT.xmlString)
                         except TypeError:
                             sock.send(processedCoT.xmlString.encode())
-                        logger.info(
+                        logger.debug(
                             str(processedCoT.xmlString) + " sent to client " + client_id
                         )
                     else:
                         try:
                             sock.send(processedCoT.idData)
                         except TypeError:
                             sock.send(processedCoT.idData.encode())
-                        logger.info(
+                        logger.debug(
                             str(processedCoT.idData) + " sent to client " + client_id
                         )
                 except Exception as e:
                     logger.error("error in sending of data " + str(e))
                     return (-1, client[1])
             if shareDataPipe != None:
                 processedCoT.clientInformation = None
@@ -235,15 +235,15 @@
                         logger.error(
                             "error sending data with marti to client within if data is "
                             + str(processedCoT.xmlString)
                             + "error is "
                             + str(e)
                         )
                         return -1
-                logger.info("CoT sent " + str(processedCoT.modelObject.uid))
+                logger.debug("CoT sent " + str(processedCoT.modelObject.uid))
                 if shareDataPipe != None:
                     processedCoT.clientInformation = None
                     if hasattr(self, "messages_to_core_count"):
                         self.messages_to_core_count += 1
                     shareDataPipe.put(processedCoT)
                 else:
                     pass
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/model/tcp_cot_connection.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/tcp_cot_service/model/tcp_cot_connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,8 +34,11 @@
         self._sock = sock_new
 
     # defined to avoid pickling the socket
     def __getstate__(self):
         state = self.__dict__
         state_cp = copy.copy(state)
         state_cp["_sock"] = None
-        return state_cp
+        return state_cp
+    
+    def __str__(self):
+        return f"{self._protocol}-{self._service_id}-{self._model_object.uid}"
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer/services/tcp_cot_service/tcp_cot_service_main.py` & `FreeTAKServer-2.0.66/FreeTAKServer/services/ssl_cot_service/ssl_cot_service_main.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,24 +5,29 @@
 from multiprocessing.pool import ThreadPool
 import os
 import multiprocessing
 import importlib
 import socket
 from opentelemetry.trace import Status, StatusCode
 from typing import List, Union, Dict
-from FreeTAKServer.services.tcp_cot_service.controllers.send_component_data_controller import SendComponentDataController
+from FreeTAKServer.services.ssl_cot_service.controllers.client_connection_controller import ClientConnectionController
+from FreeTAKServer.services.ssl_cot_service.controllers.client_disconnection_controller import ClientDisconnectionController
+from FreeTAKServer.services.ssl_cot_service.controllers.send_component_data_controller import SendComponentDataController
+from FreeTAKServer.services.ssl_cot_service.model.raw_ssl_connection_information import RawSSLConnectionInformation
+from FreeTAKServer.services.ssl_cot_service.model.ssl_cot_connection import SSLCoTConnection
 
 from digitalpy.core.service_management.digitalpy_service import DigitalPyService
 from digitalpy.core.domain.node import Node
 from digitalpy.core.main.object_factory import ObjectFactory
 from digitalpy.core.telemetry.tracer import Tracer
 from digitalpy.core.parsing.formatter import Formatter
 
 from FreeTAKServer.model.Enumerations.connectionTypes import ConnectionTypes
-from .controllers.TCPSocketController import TCPSocketController
+from .controllers.SSLSocketController import SSLSocketController
+from FreeTAKServer.core.util.geo_manager_controller import GeoManagerController
 from FreeTAKServer.core.connection.ActiveThreadsController import ActiveThreadsController
 from FreeTAKServer.core.connection.ClientInformationController import (
     ClientInformationController,
 )
 from FreeTAKServer.core.persistence.DatabaseController import (
     DatabaseController,
 )
@@ -31,110 +36,136 @@
     ReceiveConnectionsProcessController,
 )
 
 from .controllers.SendDataController import SendDataController
 from FreeTAKServer.core.SpecificCoTControllers.SendDisconnectController import (
     SendDisconnectController,
 )
-from FreeTAKServer.core.parsers.XMLCoTController import XMLCoTController
 from FreeTAKServer.core.configuration.LoggingConstants import LoggingConstants
 
 from FreeTAKServer.model.RawCoT import RawCoT
 from FreeTAKServer.core.configuration.OrchestratorConstants import (
     OrchestratorConstants,
 )
 from FreeTAKServer.model.FTSModel.Event import Event
 from FreeTAKServer.model.SpecificCoT.Presence import Presence
-from FreeTAKServer.model.TCPConnection import TCPConnection
+from FreeTAKServer.model.SSLConnection import SSLConnection
 from FreeTAKServer.model.User import User
 from FreeTAKServer.model.ClientInformation import ClientInformation
 
-from .configuration.tcp_cot_service_constants import SERVICE_NAME
-from .model.tcp_cot_connection import TCPCoTConnection
-
+from .configuration.ssl_cot_service_constants import SERVICE_NAME
 from FreeTAKServer.core.configuration.CreateLoggerController import CreateLoggerController
 loggingConstants = LoggingConstants()
-loggingConstants = LoggingConstants(log_name="FTS-TCP_CoT_Service")
+loggingConstants = LoggingConstants(log_name="SSLCoTService")
 logger = CreateLoggerController(
-    "FTS-TCP_CoT_Service", logging_constants=loggingConstants
+    "SSLCoTService", logging_constants=loggingConstants
 ).getLogger()
 
 from .controllers.ClientReceptionHandler import ClientReceptionHandler
 
 NODE_TO_XML = "NodeToXML"
 GET_MACHINE_READABLE_TYPE = "ConvertHumanReadableToMachineReadable"
 APPLICATION_PROTOCOL = "XML"
 # MAJOR TODO: Make explicit exception classes!!!
 
-
-class TCPCoTServiceMain(DigitalPyService):
-    """this service is responsible for handling the CoT listener for XML"""
-
+class SSLCoTServiceMain(DigitalPyService):
+    # TODO: fix repeat attempts to add user
     # TODO: prevent repeat add user
-    def __init__(self, service_id: str, subject_address: str, subject_port: int, subject_protocol, integration_manager_address: str, integration_manager_port: int, integration_manager_protocol: str, formatter: Formatter):
-        super().__init__(service_id, subject_address, subject_port, subject_protocol, integration_manager_address, integration_manager_port, integration_manager_protocol, formatter)
+    def __init__(
+        self,
+        service_id,
+        subject_address,
+        subject_port,
+        subject_protocol,
+        integration_manager_address,
+        integration_manager_port,
+        integration_manager_protocol,
+        formatter: Formatter,
+    ):
+        super().__init__(
+            service_id,
+            subject_address,
+            subject_port,
+            subject_protocol,
+            integration_manager_address,
+            integration_manager_port,
+            integration_manager_protocol,
+            formatter
+        )
         self.logger = logger
 
         # Server info
         self.connection_received = 0
         self.sent_message_count = 0
         self.received_message_count = 0
         self.messages_to_core_count = 0
         self.messages_from_core_count = 0
         self.openSockets = 0
 
         # Contains info on clients
         self.client_information_queue = {}
         self.clientDataPipe: Queue
-        self.connections:Dict[str, TCPCoTConnection] = {} # meant to eventually obsolete the client information queue
+        self.connections: dict[str, SSLCoTConnection] = {} # meant to eventually obsolete the client information queue
 
         # instantiate controllers
         self.ActiveThreadsController = ActiveThreadsController()
         self.ClientInformationController = ClientInformationController()
         self.ReceiveConnections = ReceiveConnections()
         self.ReceiveConnectionsProcessController = ReceiveConnectionsProcessController()
-        self.XMLCoTController = XMLCoTController()
         self.dbController: DatabaseController
-        self.send_component_data_controller = SendComponentDataController
+        self.send_component_data_controller = SendComponentDataController(self.logger)
+        self.client_connection_controller = ClientConnectionController(
+            self.logger,
+            self.client_information_queue,
+            self.connections,
+            self.openSockets
+        )
+        self.client_disconnection_controller = ClientDisconnectionController(
+            self.logger,
+            self.client_information_queue,
+            self.ActiveThreadsController,
+            self.connections,
+            self.openSockets,
+            self.connection_type,
+        )
 
     def start(
         self,
         IP,
         CoTPort,
         Event,
         clientDataPipe,
         ReceiveConnectionKillSwitch,
         RestAPIPipe,
         clientDataRecvPipe,
         factory,
         tracing_provider_instance
     ):
         try:
-            # configure the object factory with the passed factory instance
+             # configure the object factory with the passed factory instance
             ObjectFactory.configure(factory)
 
             # instantiate the tracer instance for this service
-            self.tracer: Tracer = tracing_provider_instance.create_tracer(
-                SERVICE_NAME
-            )
-            
+            self.tracer: Tracer = tracing_provider_instance.create_tracer(SERVICE_NAME)
+
             actionmapper = ObjectFactory.get_instance("actionMapper")
             # subscribe to responses originating from this controller
             actionmapper.add_topic(
                 f"/routing/response/{self.__class__.__name__.lower()}"
             )
 
             self.dbController = DatabaseController()
             # self.clear_user_table()
             os.chdir("../../../")
             # create socket controller
-            self.TCPSocketController = TCPSocketController()
-            self.TCPSocketController.changeIP(IP)
-            self.TCPSocketController.changePort(CoTPort)
-            sock = self.TCPSocketController.createSocket()
+            self.SSLSocketController = SSLSocketController()
+            self.SSLSocketController.changeIP(IP)
+            self.SSLSocketController.changePort(CoTPort)
+            sock = self.SSLSocketController.createSocket()
+            # threadpool is used as it allows the transfer of SSL socket unlike processes
             pool = ThreadPool(processes=2)
             self.pool = pool
             self.clientDataRecvPipe = clientDataRecvPipe
             clientData = pool.apply_async(
                 ClientReceptionHandler().startup, (self.client_information_queue,)
             )
             self.initialize_connections(APPLICATION_PROTOCOL)
@@ -145,56 +176,22 @@
                 receiveConnection,
                 sock,
                 pool,
                 Event,
                 clientDataPipe,
                 ReceiveConnectionKillSwitch,
                 RestAPIPipe,
+                True,
             )
         except Exception as ex:
-            return ex
-        
+            raise ex
+
     @property
     def connection_type(self):
-        return ConnectionTypes.TCP    
-
-    def remove_service_user(self, clientInformation: ClientInformation):
-        """Generates the presence object from the
-        clientInformation parameter and sends it as a remove message
-        to the client data pipe
-
-        Args:
-            clientInformation: Client information
-
-        Returns: None
-        """
-        try:
-            # TODO this doesnt guarantee that put call will succeed, need to implement blocking...
-            if not self.clientDataPipe.full():
-
-                # Process removal of client in clientDataPipe
-                # TODO add blocking
-                self.clientDataPipe.put(
-                    [
-                        "remove",
-                        clientInformation,
-                        self.openSockets,
-                        self.connection_type,
-                    ]
-                )
-                self.logger.debug(
-                    f"Client removal has been sent through queue {str(clientInformation)}"
-                )
-            else:
-                self.logger.critical("Client data pipe is full!")
-        except Exception as ex:
-            with self.tracer.start_as_current_span("remove_service_user") as span:
-                span.set_status(Status(StatusCode.ERROR))
-                span.record_exception(ex)
-            raise ex
+        return ConnectionTypes.SSL
 
     def update_client_information(self, clientInformation: ClientInformation):
         """Generates a Presence object from the clientInformation parameter and
         sends it as an update message to the client data pipe.
 
         :param clientInformation: Client information
 
@@ -225,53 +222,14 @@
                 self.logger.critical("client data pipe is Full !")
         except Exception as ex:
             with self.tracer.start_as_current_span("update_client_information") as span:
                 span.set_status(Status(StatusCode.ERROR))
                 span.record_exception(ex)
             raise ex
 
-    def add_service_user(self, clientInformation: ClientInformation):
-        """this method generates the presence and connection objects from the
-        clientInformation parameter and sends it to
-
-        :param clientInformation: this is the information of the client to be added
-        :return:
-        """
-        try:
-            # TODO this doesnt guarantee that put call will succeed, need to implement blocking...
-            if not self.clientDataPipe.full():
-                presence_object = Presence()
-                presence_object.setModelObject(clientInformation.modelObject)
-
-                # TODO why is this not xmlString?
-                presence_object.setXmlString(clientInformation.idData)
-                # Is this duplicate of modelObject?
-                presence_object.setClientInformation(clientInformation.modelObject)
-
-                connection_object = TCPConnection()
-                connection_object.sock = None
-                connection_object.user_id = clientInformation.modelObject.uid
-
-                # Updating clientDataPipe
-                # TODO add blocking...
-                self.clientDataPipe.put(
-                    ["add", presence_object, self.openSockets, connection_object]
-                )
-                self.logger.debug(
-                    "client addition has been sent through queue "
-                    + str(clientInformation)
-                )
-            else:
-                self.logger.critical("client data pipe is Full !")
-        except Exception as ex:
-            with self.tracer.start_as_current_span("add_service_user") as span:
-                span.set_status(Status(StatusCode.ERROR))
-                span.record_exception(ex)
-            raise ex
-
     def get_client_information(self):
         """this method gets client information from the client information pipe and returns it as a dict merged
         with the current client information list and updates the self variable
 
         :return:
         """
         try:
@@ -294,388 +252,62 @@
                     ):
                         self.client_information_queue[client_id].append(
                             user_dict[client_id]
                         )
 
                     elif (
                         client_id in user_dict.keys()
-                        and len(self.client_information_queue[client_id]) == 2
+                        and len(self.client_information_queue[client_id]) == 3
                     ):
-                        self.client_information_queue[client_id][1] = user_dict[client_id]
-
-                    # if the entry isn't present in FTS core than the client will be disconnected
-                    # and deleted to maintain single source of truth
-                    elif client_id not in user_dict.keys():
-                        self.logger.debug(
-                            f"disconnection client {str(client_id)} because client was not in FTS core user_dict"
-                        )
-                        self.disconnect_socket(
-                            self.client_information_queue[client_id][0]
-                        )
-                        del self.client_information_queue[client_id]
-
-                    # TODO this case will never happen
-                    else:
-                        self.logger.error(
-                            "the data for this client is invalid " + str(client_id)
-                        )
+                        self.client_information_queue[client_id][1] = user_dict[
+                            client_id
+                        ]
             else:
                 self.logger.critical("client data pipe is Full !")
         except Exception as ex:
             with self.tracer.start_as_current_span("get_client_information") as span:
                 span.set_status(Status(StatusCode.ERROR))
                 span.record_exception(ex)
 
-    # TODO make raise an exception
-    def send_user_connection_geo_chat(self, clientInformation):
-        """function to create and send pm to newly connected user
-
-        :param clientInformation: the object containing information about the user to which the msg is sent
-        :return:
-        """
-        # TODO: refactor as it has a proper implementation of a PM to a user generated by the server
-        from FreeTAKServer.core.SpecificCoTControllers.SendGeoChatController import (
-            SendGeoChatController,
-        )
-        from FreeTAKServer.model.RawCoT import RawCoT
-        from FreeTAKServer.model.FTSModel.Dest import Dest
-        import uuid
-
-        if OrchestratorConstants().DEFAULTCONNECTIONGEOCHATOBJ != None:
-            ChatObj = RawCoT()
-            ChatObj.xmlString = f"<event><point/><detail><remarks>{OrchestratorConstants().DEFAULTCONNECTIONGEOCHATOBJ}</remarks><marti><dest/></marti></detail></event>"
-
-            classobj = SendGeoChatController(ChatObj, AddToDB=False)
-            instobj = classobj.getObject()
-            instobj.modelObject.detail._chat.chatgrp.setuid1(
-                clientInformation.modelObject.uid
-            )
-            dest = Dest()
-            dest.setcallsign(clientInformation.modelObject.detail.contact.callsign)
-            instobj.modelObject.detail.marti.setdest(dest)
-            instobj.modelObject.detail._chat.setchatroom(
-                clientInformation.modelObject.detail.contact.callsign
-            )
-            instobj.modelObject.detail._chat.setparent("RootContactGroup")
-            instobj.modelObject.detail._chat.setid(clientInformation.modelObject.uid)
-            instobj.modelObject.detail._chat.setgroupOwner("True")
-            instobj.modelObject.detail.remarks.setto(clientInformation.modelObject.uid)
-            instobj.modelObject.setuid(
-                "GeoChat."
-                + "SERVER-UID."
-                + clientInformation.modelObject.detail.contact.callsign
-                + "."
-                + str(uuid.uuid1())
-            )
-            instobj.modelObject.detail._chat.chatgrp.setid(
-                clientInformation.modelObject.uid
-            )
-            classobj.reloadXmlString()
-            # self.get_client_information()
-            self.sent_message_count += 1
-            self.send_message(None, instobj, use_share_pipe=False)
-            return 1
-        else:
-            return 1
-
-    def clientConnected(self, raw_connection_information: RawCoT):
-        """Controls the client connection sequence, calling methods which perform the following:
-            1. Instantiate the client object
-            2. Share the client with core
-            3. Add the client to the database
-            4. Send the connection message
-
-        :param raw_connection_information: RawCoT object containing client connection information
-        :return: ClientInformation object for the newly connected client, or -1 if there was an error
-        """
-        try:
-            from FreeTAKServer.core.persistence.EventTableController import EventTableController
-
-            self.logger.info(loggingConstants.CLIENTCONNECTED)
-
-            # Instantiate the client object
-            clientInformation = self.ClientInformationController.intstantiateClientInformationModelFromConnection(
-                raw_connection_information, None
-            )
-            if clientInformation == -1:
-                self.logger.info("Client had invalid connection information and has been disconnected")
-                return -1
-
-            # Add client to database
-            try:
-                if hasattr(clientInformation.socket, "getpeercert"):
-                    cn = "placeholder"
-                else:
-                    cn = None
-                CoT_row = EventTableController().convert_model_to_row(clientInformation.modelObject)
-                self.dbController.create_user(
-                    uid=clientInformation.modelObject.uid,
-                    callsign=clientInformation.modelObject.detail.contact.callsign,
-                    IP=clientInformation.IP,
-                    CoT=CoT_row,
-                    CN=cn,
-                )
-            except Exception as ex:
-                with self.tracer.start_as_current_span("clientConnected") as span:
-                    span.set_status(Status(StatusCode.ERROR))
-                    span.record_exception(ex)
-
-            self.logger.debug("Adding client...")
-            self.add_service_user(clientInformation=clientInformation)
-
-            # Add client info to queue
-            self.client_information_queue[clientInformation.modelObject.uid] = [clientInformation.socket, clientInformation]
-            
-            # instantiate an object_id with a value of the client uid
-            object_id = ObjectFactory.get_new_instance("ObjectId", dynamic_configuration={"id": clientInformation.modelObject.uid, "type": "connection"})
-            
-            # TODO the instantiation of the connection object and the connection action
-            # call should be moved out of the tcp_cot_service main and into the connection
-            # controller
-
-            # instantiate a new TCPCoTConnection with an object_id of the client uid
-            connection = TCPCoTConnection(object_id)
-            connection.model_object = clientInformation.modelObject
-            connection.sock = clientInformation.socket
-            self.connections[str(connection.get_oid())] = connection
-
-            # Update the iam component with the new client information
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("connection")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_value("connection", connection)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-            self.logger.debug("Client saved")
-
-            # Broadcast user in geochat
-            self.send_user_connection_geo_chat(clientInformation)
-
-            # Send emergency information to newly connected client
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("SendEmergenciesToClient")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_value("user", connection)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-
-            
-            # Send repeated messages to newly connected clients
-            request = ObjectFactory.get_new_instance("request")
-            request.set_sender(self.__class__.__name__.lower())
-            request.set_action("connection")
-            request.set_context("Repeater")
-            request.set_value("connection", connection)
-            request.set_value("recipients", [str(connection.get_oid())])
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-
-            return clientInformation
-        except Exception as e:
-            self.logger.warning(loggingConstants.CLIENTCONNECTEDERROR)
-
-
-    def dataReceived(self, raw_cot: RawCoT):
-        """this will be executed in the event that the use case for the CoT isn't specified in the orchestrator
-
-        :param raw_cot: the CoT to be processed and shared
-        """
-        try:
-            # this will check if the CoT is applicable to any specific controllers
-            raw_cot = self.XMLCoTController.determineCoTType(raw_cot)
-
-            # the following calls whatever controller was specified by the above function
-            module = importlib.import_module(
-                "FreeTAKServer.core.SpecificCoTControllers." + raw_cot.CoTType
-            )
-            CoTSerializer = getattr(module, raw_cot.CoTType)
-            # TODO: improve way in which the dbController is passed to CoTSerializer
-            raw_cot.dbController = self.dbController
-            processedCoT = CoTSerializer(raw_cot).getObject()
-
-            # this statement checks if the data type is a user update and if so it will be saved to the associated client object
-            if raw_cot.CoTType == "SendUserUpdateController":
-                # find entry with this uid
-                self.update_client_information(clientInformation=processedCoT)
-            return processedCoT
-        except Exception as e:
-            self.logger.error(loggingConstants.DATARECEIVEDERROR + str(e))
-            return -1
-
-    def clientDisconnected(self, clientInformation: User):
-        """Handles the disconnection of clients
-
-        :param clientInformation:
-        :return:
-        """
-        import traceback
-
-        self.logger.debug("Disconnecting client")
-
-        # TODO add proper exception handling
-        # Get socket info from client object
-        try:
-            if isinstance(clientInformation, str):
-                clientInformation = self.client_information_queue[clientInformation][1]
-            elif isinstance(clientInformation, RawCoT):
-                clientInformation = self.client_information_queue[
-                    clientInformation.clientInformation
-                ][1]
-            sock = self.client_information_queue[clientInformation.user_id][0]
-        except Exception as e:
-            self.logger.critical(
-                "getting sock from client information queue failed " + str(e)
-            )
-
-        try:
-            self.logger.debug(
-                "client "
-                + clientInformation.m_presence.modelObject.uid
-                + " disconnected "
-                + "\n".join(traceback.format_stack())
-            )
-        except Exception as e:
-            self.logger.critical(
-                "there was an error logging disconnection information " + str(e)
-            )
-
-        # Removes the user id from client info queue
-        try:
-            del self.client_information_queue[clientInformation.user_id]
-            # Update the iam component with the new client information
-            request = ObjectFactory.get_new_instance("request")
-            request.set_action("disconnection")
-            request.set_sender(self.__class__.__name__.lower())
-            if hasattr(clientInformation, "modelObject"):
-                uid = clientInformation.modelObject.uid
-            elif hasattr(clientInformation, "m_presence"):
-                uid = clientInformation.m_presence.modelObject.uid
-            conn_id = str(ObjectFactory.get_instance("ObjectId", {"id": uid, "type": "connection"}))
-            del self.connections[conn_id]
-            request.set_value("connection_id", conn_id)
-            request.set_format("pickled")
-            self.subject_send_request(request, APPLICATION_PROTOCOL)
-        except Exception as e:
-            self.logger.critical("client removal failed " + str(e))
-
-        # Remove the active thread and database connection
-        try:
-            self.ActiveThreadsController.removeClientThread(clientInformation)
-            self.dbController.remove_user(query=f'uid = "{clientInformation.user_id}"')
-        except Exception as e:
-            self.logger.critical(
-                f"There has been an error in a clients disconnection while adding information to the database {str(e)}"
-            )
-
-        try:
-            self.remove_service_user(clientInformation=clientInformation)
-            self.disconnect_socket(sock)
-
-            self.logger.info(loggingConstants.CLIENTDISCONNECTSTART)
-
-            # TODO: remove string
-            self.send_disconnect_cot(clientInformation)
-            self.logger.info(
-                loggingConstants.CLIENTDISCONNECTEND
-                + str(clientInformation.m_presence.modelObject.uid)
-            )
-            return 1
-        except Exception as e:
-            import traceback
-            import sys, linecache
-
-            exc_type, exc_obj, tb = sys.exc_info()
-            f = tb.tb_frame
-            lineno = tb.tb_lineno
-            filename = f.f_code.co_filename
-            linecache.checkcache(filename)
-            line = linecache.getline(filename, lineno, f.f_globals)
-            self.logger.error(
-                loggingConstants.CLIENTCONNECTEDERROR
-                + " "
-                + str(e)
-                + " on line: "
-                + line
-            )
+    def component_handler(self, xml_cot):
+        """this method is responsible for handling cases where the cot sent should
+        be handled (parsed and manipulated) by a specific component it is
+        responsible for calling the routing (via the async action mapper)
+        of the CoT data
 
-    def send_disconnect_cot(self, clientInformation):
-        """send the disconnection information for a specific client to all connected clients
         Args:
-            clientInformation: client to be displayed as
-                disconnected by all connected devices
+            xml_cot (str): xml representation of CoT
         """
-        # TODO: remove string
-        tempXml = RawCoT()
-        tempXml.xmlString = '<event><detail><link uid="{0}"/></detail></event>'.format(
-            clientInformation.user_id
-        ).encode()
-        disconnect = SendDisconnectController(tempXml)
-        self.get_client_information()
-        self.sent_message_count += 1
-        self.messages_to_core_count += 1
-        self.send_message(disconnect.getObject().clientInformation, disconnect.getObject())
 
-    def disconnect_socket(self, sock: socket.socket) -> None:
-        """this method is responsible for disconnecting all socket objects
-
-        :param sock: socket object to be disconnected
-        """
-        self.logger.debug("Shutting down socket")
-        try:
-            sock.shutdown(socket.SHUT_RDWR)
-        except Exception as e:
-            self.logger.error(
-                "Error shutting socket down in client disconnection "
-                + str(e)
-                + "\n".join(traceback.format_stack())
-            )
-        try:
-            sock.close()
-        except Exception as e:
-            self.logger.error(
-                "error closing socket in client disconnection "
-                + str(e)
-                + "\n".join(traceback.format_stack())
-            )
-
-    def component_handler(self, cot):
-        """this method is responsible for handling cases where the cot sent should
-        be handled (parsed and manipulated) by a specific component it is
-        responsible for calling the routing (via the async action mapper)
-        of the CoT data"""
-        if not hasattr(cot, "xmlString"):
-            raise ValueError("cot missing required attribute 'xmlString'")
+        dict_cot = self.convert_xml_to_dict(xml_cot)
 
         request = ObjectFactory.get_new_instance("request")
         # must get a new instance of the async action mapper for each request
         # to prevent run conditions and to prevent responses going to the wrong
         # callers
-        actionmapper = ObjectFactory.get_instance("actionMapper")
         response = ObjectFactory.get_new_instance("response")
 
         # instantiate and define the request
         request = ObjectFactory.get_new_instance("request")
         request.set_format("pickled")
-        request.set_action(cot.data_dict["event"]["@type"])
-        request.set_context("XML")
+        human_readable_type = self.get_human_readable_type(dict_cot)
+        request.set_action(human_readable_type)
+        request.set_context("XMLCoT")
         request.set_sender(self.__class__.__name__.lower())
-        request.set_value("dictionary", cot.data_dict)
+        request.set_value("dictionary", dict_cot)
 
         # instantiate and define the response
         response = ObjectFactory.get_new_instance("response")
         response.set_format("pickled")
 
         # final request for the actual cot but listener is not returned because
         # it should be handled by the main loop which listens for all responses
         # with a request source of Orchestrator
+        self.logger.debug("sending request to subject %s", str(request.get_values()))
         self.subject_send_request(request, APPLICATION_PROTOCOL)
-        
-        # one is returned so that the message is ignored and can be processed later once the
-        # response is received by the component receiver
-        return 1
 
     def convert_to_xml(self, model_object: Node) -> str:
         """call the domain component to convert the model object to xml
         Args:
             model_object (Node): the model object to convert it's xml representation
 
         Returns:
@@ -746,65 +378,86 @@
 
                 # Check if the response model object is a list
                 if isinstance(response.get_value("message"), list):
                     for model_object in response.get_value("message"):
                         self.send_component_message(response, model_object)
                 else:
                     self.send_component_message(response, response.get_value("message"))
-            except Exception as e:
+            except Exception as ex:
                 self.logger.error(
                     f"There was an exception sending a single response:\n"
                     f"Sender: {sender}\n"
-                    f"Model object: {model_object}\n"
                     f"Context: {response.get_context()}\n"
                     f"Action: {response.get_action()}\n"
+                    f"Exception: {str(ex)}"
+                )
+                self.logger.debug(
+                    "single response exception traceback: %s", traceback.format_exc()
                 )
 
     def send_component_message(self, request, message):
-        response = ObjectFactory.get_instance("response")
-        send_component_data_controller_inst = self.send_component_data_controller(None, None, None, None)
-        send_component_data_controller_inst.initialize(request, response)
-        send_component_data_controller_inst.send_message(self.connections, message, request.get_value("recipients"))
+        self.send_component_data_controller.send_message(
+            self.connections, message, request.get_value("recipients")
+        )
 
     def send_message(self, sender, message, use_share_pipe=True):
         return SendDataController().sendDataInQueue(
-                    sender,
-                    message,  # pylint: disable=no-member; isinstance checks that CoTOutput is of proper type
-                    self.client_information_queue,
-                    self.CoTSharePipe,
-                )
+            sender,
+            message,  # pylint: disable=no-member; isinstance checks that CoTOutput is of proper type
+            self.client_information_queue,
+            self.CoTSharePipe,
+        )
+
+    def convert_xml_to_dict(self, data) -> dict:
+        """convert the xml format to a dict containing the same data via the xml_serializer
+        component.
+
+        Args:
+            data (str): an xml string containing the data from a given client
 
-    def monitor_raw_cot(self, data: RawCoT) -> object:
+        Returns:
+            dict: dictionary representation of the cot data
         """
-        This method takes as input a sent CoT and calls its associated function. This method supports three handlers defined
-        in XMLCoTController which handle connect, disconnect, and misc messages respectively.
+        request = ObjectFactory.get_new_instance("request")
+        request.set_action("XMLToDict")
+        request.set_value("message", data)
+
+        actionmapper = ObjectFactory.get_instance("syncactionMapper")
+        response = ObjectFactory.get_new_instance("response")
+        actionmapper.process_action(request, response)
+
+        # dictionary representation of the xml
+        data_dict = response.get_value("dict")
+        return data_dict
+
+    def get_human_readable_type(self, dict_cot: dict) -> str:
+        """parse the cot type and send request to the type component to
+        convert it to a human readable type
 
         Args:
-            data (RawCoT): The raw CoT data to be processed.
+            dict_cot (dict): cot message in dictionary format
 
         Returns:
-            object: The output of the handler function called on the CoT data.
+            str: the human readable
         """
-        try:
-            if isinstance(data, int):
-                return None
-            else:
-                cot = XMLCoTController(logger=self.logger).determineCoTGeneral(data, self.client_information_queue)
-                handler_name, handler_data = cot
-                handler = getattr(self, handler_name, None)
-                if handler is None:
-                    self.logger.error(f"No handler found for {handler_name}")
-                    return -1
-                output = handler(handler_data)
-                if output != 1:  # when the process is a disconnect the output is 1
-                    output.clientInformation = self.client_information_queue[data.clientInformation][1]
-                return output
-        except Exception as e:
-            self.logger.error(loggingConstants.MONITORRAWCOTERRORB + str(e))
-            return -1
+        # this convert the machine readable type to a human readable type
+        request = ObjectFactory.get_new_instance("request")
+        request.set_format("pickled")
+        request.set_action("ConvertMachineReadableToHumanReadable")
+        request.set_context("MEMORY")
+        request.set_value("machine_readable_type", dict_cot["event"]["@type"])
+        request.set_value("default", dict_cot["event"]["@type"])
+
+        # must get a new instance of the async action mapper for each request
+        # to prevent run conditions and to prevent responses going to the wrong
+        # callers
+        actionmapper = ObjectFactory.get_instance("syncactionMapper")
+        response = ObjectFactory.get_new_instance("response")
+        actionmapper.process_action(request, response)
+        return response.get_value("human_readable_type")
 
     # TODO Remove or replace
     def checkOutput(self, output):
         """this method checks whether or not the return data was valid
 
         :param output: any type which was returned by a function
         :rtype: bool indicating whether the output was valid or not
@@ -859,16 +512,14 @@
         receiveconntimeoutcount = datetime.datetime.now()
         lastprint = datetime.datetime.now()
         start_timer = time.time() - 60
 
         while event.is_set():
             self.CoTSharePipe = CoTSharePipe
             try:
-                if ssl == True:
-                    pass
                 self.clientDataPipe = clientDataPipe
                 if event.is_set():
                     try:
                         if ReceiveConnectionKillSwitch.is_set():
                             try:
                                 receiveConnection.successful()
                             except:
@@ -882,36 +533,34 @@
                             receiveConnectionOutput = receiveConnection.get(
                                 timeout=0.01
                             )
                             self.connection_received += 1
                             print(self.connection_received)
                             receiveConnection = pool.apply_async(
                                 ReceiveConnections().listen,
-                                (
-                                    sock,
-                                ),
+                                (sock,),
                             )
                             receiveconntimeoutcount = datetime.datetime.now()
                             lastprint = datetime.datetime.now()
-                            CoTOutput = self.handle_connection_data(
+                            CoTOutput = self.handle_connection(
                                 receiveConnectionOutput
                             )
 
                     except multiprocessing.TimeoutError:
 
                         if (
                             datetime.datetime.now() - receiveconntimeoutcount
                         ) > datetime.timedelta(seconds=60) and ssl == True:
                             from multiprocessing.pool import ThreadPool
 
                             try:
                                 pass
                             except Exception as e:
                                 print(str(e))
-                        elif ssl == True and (
+                        elif (
                             datetime.datetime.now() - lastprint
                         ) > datetime.timedelta(seconds=30):
                             print(
                                 "time since last reset "
                                 + str(datetime.datetime.now() - receiveconntimeoutcount)
                             )
                             lastprint = datetime.datetime.now()
@@ -937,15 +586,15 @@
                                 recent_client_data_output = (
                                     clientDataOutput,
                                     time.time(),
                                 )
                             self.received_message_count += len(
                                 clientDataOutput
                             )  # add the length of this list to the number of received messages
-                            CoTOutput = self.handle_regular_data(clientDataOutput)
+                            self.handle_regular_data(clientDataOutput)
                         else:
                             clientData = pool.apply_async(
                                 ClientReceptionHandler().startup,
                                 (self.client_information_queue,),
                             )
                             raise Exception(
                                 "client reception handler has returned data which is not of type list data is "
@@ -996,16 +645,16 @@
                     if time.time() > start_timer + 60:
                         start_timer = time.time()
                         self.logger.debug(str("mainRunFunction is running"))
                         # self.logger.debug('CoTSharePipe is full ' + str(CoTSharePipe.full()))
                         # self.logger.debug('clientDataPipe is full ' + str(clientDataPipe.full()))
                         if "recent_client_data_output" in locals():
                             self.logger.debug(
-                                "most recent client data "
-                                + str(recent_client_data_output)
+                                "most recent client data %s",
+                                str(recent_client_data_output),
                             )
                             self.logger.debug(
                                 "time since last valid data "
                                 + str(time.time() - recent_client_data_output[1])
                             )
                             self.logger.debug(
                                 "content of last valid data "
@@ -1019,122 +668,129 @@
                         "the periodic debug message has thrown an error " + str(e)
                     )
             except Exception as e:
                 self.logger.info(
                     "there has been an uncaught error thrown in mainRunFunction"
                     + str(e)
                 )
-                pass
         self.stop()
 
     def handle_shared_data(self, modelData):
         """this method is responsible for receiving and forwarding data shared via IPC
 
         :param modelData:
         :return:
         """
         try:
             self.get_client_information()
             self.messages_from_core_count += 1
             if hasattr(modelData, "clientInformation"):
                 self.sent_message_count += 1
-                self.send_message(modelData.clientInformation, modelData, use_share_pipe=False)
+                self.send_message(
+                    modelData.clientInformation, modelData, use_share_pipe=False
+                )
             else:
                 self.sent_message_count += 1
                 self.send_message(None, modelData, use_share_pipe=False)
-        except Exception as e:
-            self.logger.error("data base connection error " + str(e))
-    
+        except Exception as ex:
+            self.logger.error("data base connection error " + str(ex))
+
     def handle_regular_data(self, clientDataOutput: List[RawCoT]):
         """
         Handle "regular" data being sent by clients. Regular data is data that is neither a new connection nor a disconnection.
 
         This method initiates the serialization and distribution of regular data.
 
         Args:
             clientDataOutput (List[RawCoT]): List of RawCoT objects
 
         Returns:
             None
         """
         # Iterate through each piece of client data
         try:
-            for clientDataOutputSingle in clientDataOutput:
+            for data_object in clientDataOutput:
                 try:
                     # Skip this iteration if the data is invalid
-                    if clientDataOutputSingle == -1:
+                    if data_object == -1:
                         continue
-
-                    # Process the raw CoT data and serialize it
-                    CoTOutput = self.monitor_raw_cot(clientDataOutputSingle)
-                    self.logger.info(f"CoT serialized {CoTOutput.modelObject.uid}")
-
-                    # Skip this iteration if the CoT data is invalid
-                    if CoTOutput == 1:
+                    elif data_object.xmlString == b"":
+                        self.handle_disconnection(data_object.clientInformation)
                         continue
+                    # Process the raw CoT data and serialize it
+                    self.component_handler(data_object.xmlString)
+                    self.logger.debug(f"CoT serialized {data_object.xmlString}")
 
-                    # Check if the CoT data is valid and can be sent
-                    if self.checkOutput(CoTOutput):
-                        # Get client information and send the message
-                        self.get_client_information()
-                        self.sent_message_count += 1
-                        self.messages_to_core_count += 1
-                        output = self.send_message(CoTOutput.clientInformation, CoTOutput)
-
-                        # Check if the message was sent successfully
-                        if self.checkOutput(output) and not isinstance(output, tuple):
-                            # Message was sent successfully
-                            pass
-                        elif isinstance(output, tuple):
-                            # There was an issue sending the message, so disconnect the client
-                            self.logger.error("Issue sending data to client, now disconnecting")
-                            self.clientDisconnected(output[1])
-                        else:
-                            # There was an issue sending the message
-                            self.logger.error(f"Send data failed with data {CoTOutput.xmlString} from client {CoTOutput.clientInformation.modelObject.detail.contact.callsign}")
-                    else:
-                        # The CoT data is invalid, raise an exception
-                        raise Exception("Error in general data processing")
-                except Exception as e:
-                    self.logger.info(f"Exception in client data processing within main run function {e} data is {CoTOutput}")
-        except Exception as e:
-            self.logger.info(f"Error iterating client data output {e}")
+                except Exception as ex:
+                    self.logger.error(
+                        f"Exception in client data processing within main run function {ex} data is {data_object.xmlString} trace is {traceback.format_exc()}"
+                    )
+                    continue
+        except Exception as ex:
+            self.logger.info(f"Error iterating client data output {ex}")
             return -1
         return 1
 
+    def handle_disconnection(self, client_information):
+        """handle a client disconnection from the service by disconnecting the socket and informing clients of the disconnection
+
+        Args:
+            client_information (_type_): _description_
+        """
+        ssl_sock, unwrapped_sock = self.client_disconnection_controller.get_socks(client_information)
+        
+        self.client_disconnection_controller.delete_client_connection(client_information)
+
+        self.client_disconnection_controller.disconnect_socket(unwrapped_sock)
+
+        self.client_disconnection_controller.disconnect_socket(ssl_sock)
+
+        connection_id = self.client_disconnection_controller.get_connection_id(client_information)
+
+        iam_disconnect_request = self.client_disconnection_controller.create_iam_disconnect_request(connection_id)
+        self.subject_send_request(iam_disconnect_request, APPLICATION_PROTOCOL)
 
-    def handle_connection_data(self, receive_connection_output: RawCoT) -> None:
+        self.client_disconnection_controller.send_disconnect_cot(client_information)
+
+    def handle_connection(self, receive_connection_output: RawCoT) -> None:
         """this method should be called to initiate the process for receiving new connection data
         :rtype: None
         :param receive_connection_output: a RawCoT object from a newly connected client
         """
         try:
             self.logger.debug("Handling connection data")
             if receive_connection_output == -1:
                 return None
 
-            CoTOutput = self.monitor_raw_cot(receive_connection_output)
-            if CoTOutput != -1 and CoTOutput != None and CoTOutput != 1:
-                self.sent_message_count += 1
-                output = self.send_message(CoTOutput, CoTOutput)
+            client_connection, client_information = self.client_connection_controller.create_client_connection(
+                receive_connection_output, self.dbController
+            )
+            self.client_connection_controller.save_client_to_db(client_information, self.dbController)
+            
+            iam_request = self.client_connection_controller.create_iam_request(client_connection)
+            self.subject_send_request(iam_request, APPLICATION_PROTOCOL)
+            
+            repeated_messages_request = self.client_connection_controller.create_send_repeated_messages_request(client_connection)
+            self.subject_send_request(repeated_messages_request, APPLICATION_PROTOCOL)
+            
+            send_emergencies_request = self.client_connection_controller.create_send_emergencies_request(client_connection)
+            self.subject_send_request(send_emergencies_request, APPLICATION_PROTOCOL)
+
+            self.client_connection_controller.send_user_connection_geo_chat(client_information)
+
+            # self.handle_regular_data([receive_connection_output])
 
-                if self.checkOutput(output):
-                    self.logger.debug(
-                        f"Connection data from client {CoTOutput.modelObject.detail.contact.callsign} successfully processed."
-                    )
-                else:
-                    raise Exception("error in sending data")
         except Exception as e:
             self.logger.error(
                 "exception in receive connection data processing within main run function "
                 + str(e)
-                + " data is "
-                + str(CoTOutput)
             )
-            return -1
+            self.logger.debug(
+                "with traceback: %s", traceback.format_exc()
+            )
         return 1
 
     def stop(self):
         self.clientDataPipe.close()
         self.pool.terminate()
         self.pool.close()
         self.pool.join()
@@ -1163,15 +819,15 @@
                 self.logger.debug(
                     f"messages shared with core in {logging_interval} seconds: {self.messages_to_core_count}"
                 )
                 self.logger.debug(
                     f"messages shared with core in {logging_interval} seconds: {self.messages_from_core_count}"
                 )
                 self.logger.debug(
-                    f"number of connected client: {str(len(self.client_information_queue.keys()))}"
+                    f"number of connected client: {str(len(self.connections.keys()))}"
                 )
                 self.sent_message_count = 0
                 self.received_message_count = 0
                 self.messages_to_core_count = 0
                 self.messages_from_core_count = 0
             except Exception as e:
                 self.logger.critical("logging service failed with exception " + str(e))
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer.egg-info/PKG-INFO` & `FreeTAKServer-2.0.66/FreeTAKServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTAKServer
-Version: 2.0.21
+Version: 2.0.66
 Summary: An open source server for the TAK family of applications.
 Home-page: https://github.com/FreeTAKTeam/FreeTakServer
 Author: FreeTAKTeam
 Author-email: FreeTakTeam@gmail.com
 License: EPL-2.0
 Download-URL: https://github.com/FreeTAKTeam/FreeTakServer/releases
 Description: # FreeTAKServer [![Downloads](https://pepy.tech/badge/freetakserver)](https://pepy.tech/project/freetakserver) ![PyPI](https://img.shields.io/pypi/v/FreeTAKServer) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/FreeTAKTeam/FreeTakServer) ![Lines of code](https://img.shields.io/tokei/lines/github.com/FreeTAKTeam/FreeTakServer)
```

### Comparing `FreeTAKServer-2.0.21/FreeTAKServer.egg-info/requires.txt` & `FreeTAKServer-2.0.66/FreeTAKServer.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/LICENSE` & `FreeTAKServer-2.0.66/LICENSE`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/PKG-INFO` & `FreeTAKServer-2.0.66/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTAKServer
-Version: 2.0.21
+Version: 2.0.66
 Summary: An open source server for the TAK family of applications.
 Home-page: https://github.com/FreeTAKTeam/FreeTakServer
 Author: FreeTAKTeam
 Author-email: FreeTakTeam@gmail.com
 License: EPL-2.0
 Download-URL: https://github.com/FreeTAKTeam/FreeTakServer/releases
 Description: # FreeTAKServer [![Downloads](https://pepy.tech/badge/freetakserver)](https://pepy.tech/project/freetakserver) ![PyPI](https://img.shields.io/pypi/v/FreeTAKServer) ![GitHub release (latest by date)](https://img.shields.io/github/v/release/FreeTAKTeam/FreeTakServer) ![Lines of code](https://img.shields.io/tokei/lines/github.com/FreeTAKTeam/FreeTakServer)
```

### Comparing `FreeTAKServer-2.0.21/README.md` & `FreeTAKServer-2.0.66/README.md`

 * *Files identical despite different names*

### Comparing `FreeTAKServer-2.0.21/setup.py` & `FreeTAKServer-2.0.66/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 with open(path.join(this_directory, "README.md")) as f:
     long_description = f.read()
 setup(
     name="FreeTAKServer",
     packages=find_packages(
         include=["FreeTAKServer", "FreeTAKServer.*", "*.json", "*.ini", "*.conf"]
     ),
-    version="2.0.21",
+    version="2.0.66",
     license="EPL-2.0",
     description="An open source server for the TAK family of applications.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="FreeTAKTeam",
     author_email="FreeTakTeam@gmail.com",
     url="https://github.com/FreeTAKTeam/FreeTakServer",
```

