# Comparing `tmp/d_geolib-0.6.0.tar.gz` & `tmp/d_geolib-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "d_geolib-0.6.0.tar", max compression
+gzip compressed data, was "d_geolib-1.0.0.tar", max compression
```

## Comparing `d_geolib-0.6.0.tar` & `d_geolib-1.0.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
--rw-r--r--   0        0        0       97 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/__init__.py
--rw-r--r--   0        0        0      629 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/errors.py
--rw-r--r--   0        0        0       86 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/geometry/__init__.py
--rw-r--r--   0        0        0     1018 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/geometry/one.py
--rw-r--r--   0        0        0      510 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/__init__.py
--rw-r--r--   0        0        0    11538 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/base_model.py
--rw-r--r--   0        0        0      749 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/base_model_structure.py
--rw-r--r--   0        0        0      109 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/__init__.py
--rw-r--r--   0        0        0    12327 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_model.py
--rw-r--r--   0        0        0     1621 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_parserprovider.py
--rw-r--r--   0        0        0     3532 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_structures.py
--rw-r--r--   0        0        0    27774 2023-04-17 12:25:37.521419 d_geolib-0.6.0/geolib/models/dfoundations/internal.py
--rw-r--r--   0        0        0     3020 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dfoundations/internal_soil.py
--rw-r--r--   0        0        0    19272 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/piles.py
--rw-r--r--   0        0        0     3958 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/profiles.py
--rw-r--r--   0        0        0      603 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/serializer.py
--rw-r--r--   0        0        0     4350 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
--rw-r--r--   0        0        0     4337 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
--rw-r--r--   0        0        0    27924 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dfoundations/templates/input.foi.j2
--rw-r--r--   0        0        0      114 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dgeoflow/__init__.py
--rw-r--r--   0        0        0    16856 2023-04-20 08:35:02.111023 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_model.py
--rw-r--r--   0        0        0     4281 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
--rw-r--r--   0        0        0      333 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_validator.py
--rw-r--r--   0        0        0    31789 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dgeoflow/internal.py
--rw-r--r--   0        0        0     3517 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/serializer.py
--rw-r--r--   0        0        0      581 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dgeoflow/utils.py
--rw-r--r--   0        0        0    54613 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dseries_parser.py
--rw-r--r--   0        0        0      106 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsettlement/__init__.py
--rw-r--r--   0        0        0      301 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/drain_types.py
--rw-r--r--   0        0        0     5529 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/drains.py
--rw-r--r--   0        0        0    21412 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_model.py
--rw-r--r--   0        0        0     1520 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_parserprovider.py
--rw-r--r--   0        0        0     7149 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_structures.py
--rw-r--r--   0        0        0    34039 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/internal.py
--rw-r--r--   0        0        0     5500 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/internal_soil.py
--rw-r--r--   0        0        0     5962 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/loads.py
--rw-r--r--   0        0        0      233 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/probabilistic_calculation_types.py
--rw-r--r--   0        0        0      559 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/serializer.py
--rw-r--r--   0        0        0    18393 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/templates/input.sli.j2
--rw-r--r--   0        0        0     4965 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsettlement/templates/soil_template.j2
--rw-r--r--   0        0        0      110 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/__init__.py
--rw-r--r--   0        0        0    11248 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/calculation_options.py
--rw-r--r--   0        0        0    21608 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/constructions.py
--rw-r--r--   0        0        0    19439 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_model.py
--rw-r--r--   0        0        0     1530 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
--rw-r--r--   0        0        0     4647 2023-04-17 12:25:37.537040 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
--rw-r--r--   0        0        0     3841 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
--rw-r--r--   0        0        0    53551 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/internal.py
--rw-r--r--   0        0        0    15561 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/internal_partial_factors.py
--rw-r--r--   0        0        0     9894 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/loads.py
--rw-r--r--   0        0        0     1726 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/profiles.py
--rw-r--r--   0        0        0      561 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/serializer.py
--rw-r--r--   0        0        0     5060 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/settings.py
--rw-r--r--   0        0        0     3467 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/supports.py
--rw-r--r--   0        0        0     1702 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/surface.py
--rw-r--r--   0        0        0    35235 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dsheetpiling/templates/input.shi.j2
--rw-r--r--   0        0        0      462 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dsheetpiling/water_level.py
--rw-r--r--   0        0        0      118 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/__init__.py
--rw-r--r--   0        0        0    12238 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/analysis.py
--rw-r--r--   0        0        0    27144 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/dstability_model.py
--rw-r--r--   0        0        0     4195 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/dstability_parserprovider.py
--rw-r--r--   0        0        0     2199 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/dstability_validator.py
--rw-r--r--   0        0        0    79894 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/internal.py
--rw-r--r--   0        0        0     2528 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/loads.py
--rw-r--r--   0        0        0     3435 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/reinforcements.py
--rw-r--r--   0        0        0     3529 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/serializer.py
--rw-r--r--   0        0        0     3331 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/dstability/states.py
--rw-r--r--   0        0        0      581 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/dstability/utils.py
--rw-r--r--   0        0        0      142 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/internal.py
--rw-r--r--   0        0        0     1781 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/meta.py
--rw-r--r--   0        0        0       89 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/model_enums.py
--rw-r--r--   0        0        0     1821 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/parsers.py
--rw-r--r--   0        0        0      840 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/models/serializers.py
--rw-r--r--   0        0        0     2433 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/utils.py
--rw-r--r--   0        0        0      314 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/models/validators.py
--rw-r--r--   0        0        0       55 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/service/__init__.py
--rw-r--r--   0        0        0     5659 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/service/main.py
--rw-r--r--   0        0        0      546 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/service/README.md
--rw-r--r--   0        0        0      797 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/soils/__init__.py
--rw-r--r--   0        0        0     1720 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/layers.py
--rw-r--r--   0        0        0      592 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/library.py
--rw-r--r--   0        0        0    37210 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/soils/soil.py
--rw-r--r--   0        0        0      775 2023-04-17 12:25:37.552666 d_geolib-0.6.0/geolib/soils/soil_utils.py
--rw-r--r--   0        0        0     1574 2023-04-20 08:35:02.126648 d_geolib-0.6.0/geolib/utils.py
--rw-r--r--   0        0        0     1086 2023-04-17 12:25:37.505796 d_geolib-0.6.0/LICENSE
--rw-r--r--   0        0        0     1982 2023-04-20 08:35:02.126648 d_geolib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2955 2023-04-20 08:35:02.111023 d_geolib-0.6.0/README.rst
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 d_geolib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/__init__.py
+-rw-r--r--   0        0        0      631 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/errors.py
+-rw-r--r--   0        0        0       86 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/geometry/__init__.py
+-rw-r--r--   0        0        0     1023 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/geometry/one.py
+-rw-r--r--   0        0        0      510 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/__init__.py
+-rw-r--r--   0        0        0    11570 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/base_model.py
+-rw-r--r--   0        0        0      749 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/base_model_structure.py
+-rw-r--r--   0        0        0      109 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/__init__.py
+-rw-r--r--   0        0        0    12325 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_model.py
+-rw-r--r--   0        0        0     1619 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_parserprovider.py
+-rw-r--r--   0        0        0     3539 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_structures.py
+-rw-r--r--   0        0        0    27768 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/internal.py
+-rw-r--r--   0        0        0     3020 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/internal_soil.py
+-rw-r--r--   0        0        0    19272 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/piles.py
+-rw-r--r--   0        0        0     3958 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/profiles.py
+-rw-r--r--   0        0        0      603 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/serializer.py
+-rw-r--r--   0        0        0     4350 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv
+-rw-r--r--   0        0        0     4337 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv
+-rw-r--r--   0        0        0    27924 2023-05-15 11:19:36.395430 d_geolib-1.0.0/geolib/models/dfoundations/templates/input.foi.j2
+-rw-r--r--   0        0        0      114 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/__init__.py
+-rw-r--r--   0        0        0    16831 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/dgeoflow_model.py
+-rw-r--r--   0        0        0     4275 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py
+-rw-r--r--   0        0        0      333 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/dgeoflow_validator.py
+-rw-r--r--   0        0        0    31320 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/internal.py
+-rw-r--r--   0        0        0     3513 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/serializer.py
+-rw-r--r--   0        0        0      581 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dgeoflow/utils.py
+-rw-r--r--   0        0        0    54527 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dseries_parser.py
+-rw-r--r--   0        0        0      106 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/__init__.py
+-rw-r--r--   0        0        0      301 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/drain_types.py
+-rw-r--r--   0        0        0     5529 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/drains.py
+-rw-r--r--   0        0        0    21412 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_model.py
+-rw-r--r--   0        0        0     1518 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_parserprovider.py
+-rw-r--r--   0        0        0     7147 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_structures.py
+-rw-r--r--   0        0        0    34035 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/internal.py
+-rw-r--r--   0        0        0     5500 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/internal_soil.py
+-rw-r--r--   0        0        0     5960 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/loads.py
+-rw-r--r--   0        0        0      233 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/probabilistic_calculation_types.py
+-rw-r--r--   0        0        0      559 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/serializer.py
+-rw-r--r--   0        0        0    18393 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/templates/input.sli.j2
+-rw-r--r--   0        0        0     4965 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsettlement/templates/soil_template.j2
+-rw-r--r--   0        0        0      110 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/__init__.py
+-rw-r--r--   0        0        0    11250 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/calculation_options.py
+-rw-r--r--   0        0        0    21608 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/constructions.py
+-rw-r--r--   0        0        0    19431 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_model.py
+-rw-r--r--   0        0        0     1528 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py
+-rw-r--r--   0        0        0     4647 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_structures.py
+-rw-r--r--   0        0        0     3841 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_validator.py
+-rw-r--r--   0        0        0    53609 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/internal.py
+-rw-r--r--   0        0        0    15559 2023-05-15 11:19:36.411053 d_geolib-1.0.0/geolib/models/dsheetpiling/internal_partial_factors.py
+-rw-r--r--   0        0        0     9894 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/loads.py
+-rw-r--r--   0        0        0     1726 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/profiles.py
+-rw-r--r--   0        0        0      561 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/serializer.py
+-rw-r--r--   0        0        0     5062 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/settings.py
+-rw-r--r--   0        0        0     3465 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/supports.py
+-rw-r--r--   0        0        0     1700 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/surface.py
+-rw-r--r--   0        0        0    35235 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/templates/input.shi.j2
+-rw-r--r--   0        0        0      462 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dsheetpiling/water_level.py
+-rw-r--r--   0        0        0      118 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/__init__.py
+-rw-r--r--   0        0        0    12506 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/analysis.py
+-rw-r--r--   0        0        0    36730 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/dstability_model.py
+-rw-r--r--   0        0        0     4189 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/dstability_parserprovider.py
+-rw-r--r--   0        0        0     2865 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/dstability_validator.py
+-rw-r--r--   0        0        0    90749 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/internal.py
+-rw-r--r--   0        0        0     2528 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/loads.py
+-rw-r--r--   0        0        0     3435 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/reinforcements.py
+-rw-r--r--   0        0        0     3525 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/serializer.py
+-rw-r--r--   0        0        0     3331 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/states.py
+-rw-r--r--   0        0        0      581 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/dstability/utils.py
+-rw-r--r--   0        0        0      142 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/internal.py
+-rw-r--r--   0        0        0     1781 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/meta.py
+-rw-r--r--   0        0        0       89 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/model_enums.py
+-rw-r--r--   0        0        0     1821 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/parsers.py
+-rw-r--r--   0        0        0      840 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/serializers.py
+-rw-r--r--   0        0        0     2433 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/utils.py
+-rw-r--r--   0        0        0      314 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/models/validators.py
+-rw-r--r--   0        0        0       55 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/service/__init__.py
+-rw-r--r--   0        0        0     5849 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/service/main.py
+-rw-r--r--   0        0        0      546 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/service/README.md
+-rw-r--r--   0        0        0      797 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/soils/__init__.py
+-rw-r--r--   0        0        0     1720 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/soils/layers.py
+-rw-r--r--   0        0        0      592 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/soils/library.py
+-rw-r--r--   0        0        0    37608 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/soils/soil.py
+-rw-r--r--   0        0        0      775 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/soils/soil_utils.py
+-rw-r--r--   0        0        0     1574 2023-05-15 11:19:36.426685 d_geolib-1.0.0/geolib/utils.py
+-rw-r--r--   0        0        0     1086 2023-05-15 11:19:36.379814 d_geolib-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2018 2023-05-15 11:19:36.442311 d_geolib-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2955 2023-05-15 11:19:36.379814 d_geolib-1.0.0/README.rst
+-rw-r--r--   0        0        0     3999 1970-01-01 00:00:00.000000 d_geolib-1.0.0/PKG-INFO
```

### Comparing `d_geolib-0.6.0/geolib/errors.py` & `d_geolib-1.0.0/geolib/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Error definitions for GEOLib.
 """
 
+
 class GEOLibError(Exception):
     """Base GEOLib Exception class."""
 
 
 class CalculationError(GEOLibError):
     """CalculationError with a status_code."""
```

### Comparing `d_geolib-0.6.0/geolib/geometry/one.py` & `d_geolib-1.0.0/geolib/geometry/one.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 NODATA = -999.0  # TODO why is this implemented instead of None?
 
 
 class Point(BaseDataClass):
     """A single Point Class."""
 
     label: Optional[str] = ""
-    id: Optional[int]
+    id: Optional[int] = None
     x: float = NODATA
     y: float = NODATA
     z: float = NODATA
     tolerance: float = 1e-4
 
     def __eq__(self, other):
-
         if isinstance(other, Point):
             return (
                 isclose(self.x, other.x, abs_tol=self.tolerance)
                 and isclose(self.y, other.y, abs_tol=self.tolerance)
                 and isclose(self.z, other.z, abs_tol=self.tolerance)
             )
         else:
```

### Comparing `d_geolib-0.6.0/geolib/models/base_model.py` & `d_geolib-1.0.0/geolib/models/base_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,17 @@
                 )
                 error = self.get_error_context()
                 raise CalculationError(process.returncode, error)
 
         # Unsuccessful run
         else:
             error = self.get_error_context()
-            raise CalculationError(process.returncode, error + " Path: " + str(output_filename.absolute))
+            raise CalculationError(
+                process.returncode, error + " Path: " + str(output_filename.absolute)
+            )
 
     def execute_remote(self, endpoint: HttpUrl) -> "BaseModel":
         """Execute a Model on a remote endpoint.
 
         A new model instance is returned.
         """
         response = requests.post(
```

### Comparing `d_geolib-0.6.0/geolib/models/base_model_structure.py` & `d_geolib-1.0.0/geolib/models/base_model_structure.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_model.py` & `d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,14 @@
 
     @classmethod
     def model_type(cls):
         raise NotImplementedError("Implement in concrete classes.")
 
 
 class BearingPilesModel(ModelOptions):
-
     factor_gamma_b: Optional[confloat(ge=1, le=100)] = None
     factor_gamma_s: Optional[confloat(ge=1, le=100)] = None
     factor_gamma_fnk: Optional[confloat(ge=-100, le=100)] = None
     area: Optional[confloat(ge=0, le=100000)] = None
 
     @classmethod
     def model_type(cls):
```

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_parserprovider.py` & `d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_parserprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 
     @property
     def dserie_structure(self) -> Type[DFoundationsDumpStructure]:
         return DFoundationsDumpStructure
 
 
 class DFoundationsParserProvider(BaseParserProvider):
-
     __input_parsers = None
     __output_parsers = None
 
     @property
     def input_parsers(self) -> Tuple[DFoundationsInputParser]:
         if not self.__input_parsers:
             self.__input_parsers = (DFoundationsInputParser(),)
```

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/dfoundations_structures.py` & `d_geolib-1.0.0/geolib/models/dfoundations/dfoundations_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,23 +79,23 @@
         def split_line(text: str) -> List[str]:
             parts = re.split(" |\t", text.strip())
             return list(filter(lambda part: part != "", parts))
 
         table_text = list(DSerieParser.parse_list_group(text).values())[0]
         table_data = list(DSerieParser.parse_list_group(table_text).values())
         if len(table_data) == 0:
-            values_dict_list = table_data;
+            values_dict_list = table_data
             collection_property_name = list(cls.__fields__.items())[0][0]
             return cls(**{collection_property_name: values_dict_list})
         else:
             # Expected two groups (column_indication and data)
             keys = table_data[0].split("\n")
             values_dict_list = [
-            dict(zip(keys, values))
-            for values in map(split_line, table_data[1].split("\n"))
+                dict(zip(keys, values))
+                for values in map(split_line, table_data[1].split("\n"))
             ]
             collection_property_name = list(cls.__fields__.items())[0][0]
 
         return cls(**{collection_property_name: values_dict_list})
 
 
 class DFoundationsCPTCollectionWrapper(DSerieListGroupNextStructure):
```

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/internal.py` & `d_geolib-1.0.0/geolib/models/dfoundations/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,14 @@
     top_level: float  # [m]
     excess_pore_pressure_top: float = 0.0  # [kN/m3]
     excess_pore_pressure_bottom: float = 0.0  # [kN/m3]
     ocr_value: float = 1.0  # [-]
     reduction_core_resistance: float = 0.0  # [%]
 
 
-
 class ReductionCoreResistanceEnum(IntEnum):
     SAFE = 0
     BEGEMANN = 1
     MANUAL = 2
 
 
 class Profile(DSeriesTreeStructure):
@@ -424,15 +423,14 @@
             for cpt in self.cpt_collection:
                 if cpt.cptname == key:
                     return cpt
             raise KeyError(key)
 
 
 class CalculationOptions(DSeriesNoParseSubStructure):
-
     # Rigidity of superstructure
     is_rigid: Bool = Bool.TRUE
 
     # Transformation
     max_allowed_settlement_lim_state_str: confloat(ge=0, le=100000) = 0
     max_allowed_rel_rotation_lim_state_str: conint(ge=1, le=10000) = 100
     max_allowed_settlement_lim_state_serv: confloat(ge=0, le=100000) = 0
@@ -786,13 +784,12 @@
 
 
 class DFoundationsStructure(DSeriesStructure):
     input_data: DFoundationsInputStructure = DFoundationsInputStructure()
     dumpfile_output: Optional[DFoundationsDumpfileOutputStructure]
 
 
-
 class DFoundationsDumpStructure(DSeriesStructure):
     dumpfile: DFoundationsStructure = DFoundationsStructure()
 
 
 # endregion
```

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/internal_soil.py` & `d_geolib-1.0.0/geolib/models/dfoundations/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/piles.py` & `d_geolib-1.0.0/geolib/models/dfoundations/piles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/profiles.py` & `d_geolib-1.0.0/geolib/models/dfoundations/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/serializer.py` & `d_geolib-1.0.0/geolib/models/dfoundations/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv` & `d_geolib-1.0.0/geolib/models/dfoundations/soil_csv/bearing_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv` & `d_geolib-1.0.0/geolib/models/dfoundations/soil_csv/tension_piles_soils.csv`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dfoundations/templates/input.foi.j2` & `d_geolib-1.0.0/geolib/models/dfoundations/templates/input.foi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_model.py` & `d_geolib-1.0.0/geolib/models/dgeoflow/dgeoflow_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     DGeoFlowResult,
     DGeoFlowStructure,
     GroundwaterFlowResult,
     PersistableSoil,
     PersistableSoilLayer,
     PipeLengthResult,
     PipeTrajectory,
+    Scenario,
     SoilCollection,
     SoilLayerCollection,
 )
 from .serializer import DGeoFlowInputSerializer, DGeoFlowInputZipSerializer
 
 
 class DGeoFlowObject(BaseModel, metaclass=abc.ABCMeta):
@@ -39,14 +40,15 @@
 
     This model can read, modify and create
     .flox files
     """
 
     current_scenario: int = -1
     current_scenario_index: int = 0
+    current_stage_index: int = 0
     current_calculation_index: int = 0
     datastructure: DGeoFlowStructure = DGeoFlowStructure()
     current_id: int = -1
 
     def __init__(self, *args, **data) -> None:
         super().__init__(*args, **data)
         self.current_id = self.datastructure.get_unique_id()
@@ -134,39 +136,14 @@
         else:
             serializer = DGeoFlowInputZipSerializer(ds=self.datastructure)
         serializer.write(location)
 
         if isinstance(location, Path):
             self.filename = location
 
-    def copy_scenario(self, label: str, notes: str, set_current=True) -> int:
-        """Copy an existing scenario and add it to the model.
-
-        Args:
-            label: Label for the scenario
-            notes: Notes for the scenario
-            set_current: Whether to make the new scenario the current scenario.
-
-        Returns:
-            the id of the new scenario
-        """
-        new_id = self._get_next_id()
-        new_scenario_id, new_unique_id = self.datastructure.duplicate_scenario(
-            self.current_scenario, label, notes, new_id
-        )
-
-        if set_current:
-            self.current_scenario = new_scenario_id
-            self.current_scenario_index += 1
-        self.current_id = new_unique_id
-        return new_scenario_id
-
-    def add_point(self, point: Point, scenario=None) -> int:
-        """Add point, which should be unique in the model and return the created point id."""
-
     def add_soil(self, soil: Soil) -> int:
         """
         Add a new soil to the model. The code must be unique, the id will be generated
 
         Args:
             soil (Soil): a new soil
 
@@ -311,65 +288,104 @@
         boundary_condition_id = self._get_next_id()
         boundary_conditions.add_boundary_condition(
             boundary_condition_id, label, notes, points, head_level
         )
 
         return boundary_condition_id
 
+    @property
+    def scenarios(self) -> List[Scenario]:
+        return self.datastructure.scenarios
+
     def add_scenario(
+        self, label: str = "Scenario", notes: str = "", set_current: bool = True
+    ) -> int:
+        """Add a new scenario to the model.
+
+        Args:
+            label: Label for the scenario.
+            notes: Notes for the scenario.
+            set_current: Whether to make the new scenario the current scenario.
+
+        Returns:
+            the id of the new stage
+        """
+        new_id = self._get_next_id()
+        new_scenario_id, new_unique_id = self.datastructure.add_default_scenario(
+            label, notes, new_id
+        )
+
+        if set_current:
+            self.current_scenario = new_scenario_id
+            self.current_stage_index = 0
+            self.current_calculation_index = 0
+
+        self.current_id = new_unique_id
+        return new_scenario_id
+
+    def add_stage(
         self,
-        scenario_index: int = None,
-        boundaryconditions_id: int = None,
-        soillayers_id: int = None,
-        geometry_id: int = None,
-        meshproperties_id: int = None,
-        label: str = "",
+        scenario_index: Optional[int] = None,
+        label: str = "Stage",
         notes: str = "",
-        calculations_notes: str = "",
-        stage_notes: str = "",
-        calculations_label: str = None,
-        stage_label: str = None,
+        set_current=True,
     ) -> int:
-        """
-        Add a scenario to the model
+        """Add a new stage to the model at the given scenario index.
 
         Args:
-            scenario_index (int): scenario to add to, defaults to 0
-            boundaryconditions_id (int): id of the boundary conditions collection to add to the scenario
-            soillayers_id (int): id of the soil layers to add to the scenario
-            geometry_id (int): id of the geometry to add to the scenario
-            meshproperties_id (int): id of the mesh properties to add to the scenario
-            label (str): label of the scenario, defaults to empty string
-            notes (str): notes of the scenario, defaults to empty string
-            calculations_notes (str): notes of the calculation, defaults to empty string
-            stage_notes (str): notes of the stage, defaults to empty string
-            calculations_label (str): label of the calculation, defaults to empty string
-            stage_label (str): label of the stage, defaults to empty string
+            scenario_index: The scenario index to add the stage to, defaults to the current scenario.
+            label: Label for the stage.
+            notes: Notes for the stage.
+            set_current: Whether to make the new stage the current stage.
 
         Returns:
-            int: id of the scenario
+            the id of the new stage
         """
+        scenario_index = (
+            scenario_index if scenario_index is not None else self.current_scenario
+        )
 
-        scenarios = self.datastructure.scenarios[scenario_index]
+        new_id = self._get_next_id()
+        new_stage_index = self.datastructure.add_default_stage(
+            scenario_index, label, notes, new_id
+        )
 
-        scenarios.Label = label
-        scenarios.Notes = notes
-        scenarios.GeometryId = geometry_id
-        scenarios.SoilLayersId = soillayers_id
-        scenarios.add_calculation(
-            label=calculations_label,
-            notes=calculations_notes,
-            mesh_properties_id=meshproperties_id,
+        if set_current:
+            self.current_stage_index = new_stage_index
+        return new_stage_index
+
+    def add_calculation(
+        self,
+        scenario_index: Optional[int] = None,
+        label: str = "Calculation",
+        notes: str = "",
+        set_current: bool = True,
+    ) -> int:
+        """Add a new calculation to the model.
+
+        Args:
+            scenario_index: The scenario index to add the calculation to, defaults to the current scenario.
+            label: Label for the calculation.
+            notes: Notes for the calculation.
+            set_current: Whether to make the new calculation the current calculation.
+
+        Returns:
+            the id of the new stage
+        """
+        scenario_index = (
+            scenario_index if scenario_index is not None else self.current_scenario
         )
-        scenarios.add_stage(
-            label=stage_label,
-            notes=stage_notes,
-            boundaryconditions_collection_id=boundaryconditions_id,
+
+        new_calculation_index = self.datastructure.add_default_calculation(
+            scenario_index, label, notes
         )
-        return int(scenarios.Id)
+
+        if set_current:
+            self.current_calculation_index = new_calculation_index
+        return new_calculation_index
 
     def set_calculation_type(
         self,
         scenario_index: int = 0,
         calculation_index: int = 0,
         calculation_type: CalculationTypeEnum = CalculationTypeEnum.GROUNDWATER_FLOW,
     ) -> None:
```

### Comparing `d_geolib-0.6.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py` & `d_geolib-1.0.0/geolib/models/dgeoflow/dgeoflow_parserprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         return super().can_parse(filename) or filename.is_dir()
 
     def parse(self, filepath: DirectoryPath) -> BaseModelStructure:
         data_structure = {}
 
         # Find required .json files via type hints
         for field, fieldtype in get_filtered_type_hints(self.structure):
-
             # On List types, parse a folder
             if type(fieldtype) == _GenericAlias:  # quite hacky
                 element_type, *_ = fieldtype.__args__  # use getargs in 3.8
                 print(field, element_type, filepath)
                 data_structure[field] = self.__parse_folder(element_type, filepath / "")
 
             # Otherwise it is a single .json in the root folder
@@ -74,15 +73,14 @@
         return [".flox"]
 
     def can_parse(self, filename: FilePath) -> bool:
         return filename.suffix in self.suffix_list
 
     def parse(self, filepath: FilePath) -> BaseModelStructure:
         with ZipFile(filepath) as zip:
-
             # Fix backslashes in zipfile (until fixed in DGeoFlow)
             for file in zip.filelist:
                 new_filename = file.filename.replace("\\", "/")
                 if new_filename != file.filename:
                     file.filename = new_filename
             for key in list(zip.NameToInfo.keys()):
                 new_key = key.replace("\\", "/")
@@ -91,15 +89,14 @@
 
             path = Path(zip)
             data_structure = super().parse(path)
         return data_structure
 
 
 class DGeoFlowParserProvider(BaseParserProvider):
-
     _input_parsers = None
     _output_parsers = None
 
     @property
     def input_parsers(self) -> Tuple[DGeoFlowParser, DGeoFlowZipParser]:
         if not self._input_parsers:
             self._input_parsers = (DGeoFlowZipParser(), DGeoFlowParser())
```

### Comparing `d_geolib-0.6.0/geolib/models/dgeoflow/internal.py` & `d_geolib-1.0.0/geolib/models/dgeoflow/internal.py`

 * *Files 6% similar despite different names*

```diff
@@ -745,15 +745,14 @@
     class Config:
         arbitrary_types_allowed = True
         validate_assignment = True
 
     def get_result_substructure(
         self, calculation_type: CalculationTypeEnum
     ) -> List[DGeoFlowResult]:
-
         result_types_mapping = {
             CalculationTypeEnum.GROUNDWATER_FLOW: self.groundwater_flow_results,
             CalculationTypeEnum.PIPE_LENGTH: self.pipe_length_results,
             CalculationTypeEnum.CRITICAL_HEAD: self.critical_head_results,
         }
 
         return result_types_mapping[calculation_type]
@@ -772,123 +771,118 @@
 
             if scenario.GeometryId != values.get("geometries")[i].Id:
                 raise ValueError("GeometryIds not linked!")
             if scenario.SoilLayersId != values.get("soillayers")[i].Id:
                 raise ValueError("SoilLayersIds not linked!")
         return values
 
-    @property
-    def stage_specific_fields(self):
-        return [
-            "soillayers",
-            "geometries",
-            "boundaryconditions",
-            "meshproperties",
-            "scenarios",
-        ]
-
-    def get_scenario_specific_fields(self, stage=0) -> Tuple[str, DGeoFlowSubStructure]:
-        """Yield stage specific fields for given stage."""
-        for fieldname in self.stage_specific_fields:
-            field = getattr(self, fieldname)
-            if len(field) > stage:
-                yield fieldname, field[stage]
-
-    def renumber_fk_fields(self, instance, mapping: Dict, unique_id: int) -> int:
-        """Replace id (foreign key) fields on instance based on a mapping and unique id."""
-        fk = ForeignKeys()
-        fkfields = fk.class_fields
-
-        def get_correct_key(key, mapping):
-            if key not in mapping:
-                nonlocal unique_id
-                mapping[key] = unique_id
-                unique_id += 1
-            return mapping[key]
-
-        for fkfield in fkfields.get(instance.__class__.__name__, []):
-            value = getattr(instance, fkfield)
-            if isinstance(value, (list, set, tuple)):
-                setattr(
-                    instance,
-                    fkfield,
-                    [get_correct_key(x, mapping) for x in value],
-                )
-            if isinstance(value, (int, float, str)):
-                setattr(instance, fkfield, get_correct_key(value, mapping))
-
-        return unique_id
-
-    def duplicate_scenario(
-        self, current_scenario: int, label: str, notes: str, unique_start_id: int
-    ):
-        """Duplicates an existing scenario.
-        Copies the specific scenario fields for a scenario and renumbers all Ids,
-        taking into account foreign keys by using the same renumbering.
-        """
+    @root_validator(skip_on_failure=True, allow_reuse=True)
+    def ensure_validity_foreign_keys(cls, values):
+        def list_has_id(values, id):
+            for entry in values:
+                if entry.Id == id:
+                    return True
+            return False
 
-        old_to_new = {}
-        for fieldname, scenario_field in self.get_scenario_specific_fields(
-            current_scenario
-        ):
-            new_scenario_fields = scenario_field.copy(deep=True)
-
-            # Renumber the upper class
-            unique_start_id = self.renumber_fk_fields(
-                new_scenario_fields, old_to_new, unique_start_id
-            )
-            # Renumber all children
-            for class_instance in children(new_scenario_fields):
-                unique_start_id = self.renumber_fk_fields(
-                    class_instance, old_to_new, unique_start_id
-                )
-
-            # Update the stage with extra supplied fields
-            if fieldname == "stages":
-                new_scenario_fields.Label = label
-                new_scenario_fields.Notes = notes
+        for _, scenario in enumerate(values.get("scenarios")):
+            for _, stage in enumerate(scenario.Stages):
+                if not list_has_id(
+                    values.get("boundary_conditions"), stage.BoundaryConditionCollectionId
+                ):
+                    raise ValueError("BoundaryConditionCollectionIds not linked!")
 
-            getattr(self, fieldname).append(new_scenario_fields)
+            if not list_has_id(values.get("geometries"), scenario.GeometryId):
+                raise ValueError("GeometryIds not linked!")
+            if not list_has_id(values.get("soillayers"), scenario.SoilLayersId):
+                raise ValueError("SoilLayersIds not linked!")
 
-        return len(self.stages) - 1, unique_start_id
+        return values
 
     def add_default_scenario(
-        self, label: str, notes: str, unique_start_id=500
+        self, label: str, notes: str, unique_start_id: Optional[int] = None
     ) -> Tuple[int, int]:
         """Add a new default (empty) scenario to DGeoFlow."""
+        if unique_start_id is None:
+            unique_start_id = self.get_unique_id()
 
+        scenario_id = unique_start_id + 7
         self.soillayers += [SoilLayerCollection(Id=str(unique_start_id + 1))]
         self.mesh_properties += [MeshProperty(Id=str(unique_start_id + 2))]
-        self.geometries += [Geometry(Id=str(unique_start_id + 4))]
+        self.geometries += [Geometry(Id=str(unique_start_id + 3))]
         self.boundary_conditions += [
-            BoundaryConditionCollection(Id=str(unique_start_id + 5))
+            BoundaryConditionCollection(Id=str(unique_start_id + 4))
         ]
 
         self.scenarios += [
             Scenario(
-                Id=str(str(unique_start_id + 7)),
-                Label="Scenario 1",
-                GeometryId=str(unique_start_id + 4),
+                Id=str(scenario_id),
+                Label=label,
+                Notes=notes,
+                GeometryId=str(unique_start_id + 3),
                 SoilLayersId=str(unique_start_id + 1),
-                Calculations=[
-                    PersistableCalculation(
-                        Id=str(unique_start_id + 6), Label="Calculation 1"
-                    )
-                ],
+                Calculations=[PersistableCalculation(Label="Calculation 1")],
                 Stages=[
                     PersistableStage(
-                        Id=str(unique_start_id + 6),
                         Label="Stage 1",
-                        BoundaryConditionCollectionId=str(unique_start_id + 5),
+                        BoundaryConditionCollectionId=str(unique_start_id + 4),
                     )
                 ],
             )
         ]
 
-        return len(self.scenarios) - 1, unique_start_id + 11
+        return len(self.scenarios) - 1, scenario_id
+
+    def add_default_stage(
+        self,
+        scenario_index: int,
+        label: str,
+        notes: str,
+        unique_start_id: Optional[int] = None,
+    ) -> int:
+        """Add a new default (empty) stage to DStability."""
+        if unique_start_id is None:
+            unique_start_id = self.get_unique_id()
+
+        self.boundary_conditions += [
+            BoundaryConditionCollection(Id=str(unique_start_id + 1))
+        ]
+
+        new_stage = PersistableStage(
+            Label=label,
+            Notes=notes,
+            BoundaryConditionCollectionId=str(unique_start_id + 1),
+        )
+
+        scenario = self.scenarios[scenario_index]
+
+        if scenario.Stages is None:
+            scenario.Stages = []
+
+        scenario.Stages.append(new_stage)
+        return len(scenario.Stages) - 1
+
+    def add_default_calculation(
+        self,
+        scenario_index: int,
+        label: str,
+        notes: str,
+    ) -> int:
+        """Add a new default (empty) calculation to DStability."""
+
+        new_calculation = PersistableCalculation(
+            Label=label, Notes=notes, CalculationType=CalculationTypeEnum.GROUNDWATER_FLOW
+        )
+
+        scenario = self.scenarios[scenario_index]
+
+        if scenario.Calculations is None:
+            scenario.Calculations = []
+
+        scenario.Calculations.append(new_calculation)
+        return len(scenario.Calculations) - 1
 
     def get_unique_id(self) -> int:
         """Return unique id that can be used in DGeoFlow.
         Finds all existing ids, takes the max and does +1.
         """
 
         fk = ForeignKeys()
```

### Comparing `d_geolib-0.6.0/geolib/models/dgeoflow/serializer.py` & `d_geolib-1.0.0/geolib/models/dgeoflow/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 
 class DGeoFlowInputSerializer(DGeoFlowBaseSerializer):
     def write(self, filepath: DirectoryPath) -> DirectoryPath:
         serialized_datastructure = self.serialize()
 
         for filename, data in serialized_datastructure.items():
-
             if isinstance(data, dict):
                 folder = filepath / filename
                 folder.mkdir(parents=True, exist_ok=True)
 
                 for ffilename, fdata in data.items():
                     fn = folder / ffilename
                     with fn.open("wb") as io:
@@ -75,15 +74,14 @@
     """DStabilSerializer for zipped.stix files."""
 
     def write(self, filepath: Union[FilePath, BytesIO]) -> Union[FilePath, BytesIO]:
         with ZipFile(filepath, mode="w", compression=ZIP_DEFLATED) as zip:
             serialized_datastructure = self.serialize()
 
             for filename, data in serialized_datastructure.items():
-
                 if isinstance(data, dict):
                     folder = filename
                     for ffilename, fdata in data.items():
                         fn = folder + "/" + ffilename
                         with zip.open(fn, "w") as io:
                             io.write(fdata.encode("utf-8"))
                 else:
```

### Comparing `d_geolib-0.6.0/geolib/models/dgeoflow/utils.py` & `d_geolib-1.0.0/geolib/models/dgeoflow/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dseries_parser.py` & `d_geolib-1.0.0/geolib/models/dseries_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,14 @@
                 f"""Got more fields than defined on model {self.__class__.__name__}:
                 parser has {a.difference(b)} fields and
                 model has {b.difference(a)} fields not set.
                 """
             )
 
         for field, fieldtype in get_type_hints(self).items():
-
             # If the body is a string, we should check
             # whether we can parse it further.
             if field in kwargs and isinstance(kwargs[field], str):
                 body = kwargs[field]
 
                 # Optional, Union, etc.
                 if is_union(fieldtype):
@@ -99,18 +98,18 @@
                 else:
                     if DataClass in fieldtype.__mro__:
                         logger.debug(f"Can't parse {fieldtype} for {field} yet")
 
             # If the body is a List[string], we should check
             # whether we can parse it further.
             elif (
-                    field in kwargs
-                    and isinstance(kwargs[field], list)
-                    and len(kwargs[field]) > 0
-                    and isinstance(kwargs[field][0], str)
+                field in kwargs
+                and isinstance(kwargs[field], list)
+                and len(kwargs[field]) > 0
+                and isinstance(kwargs[field][0], str)
             ):
                 body = kwargs[field]
 
                 # We need to decompose a possible Union
                 if is_union(fieldtype):
                     fieldtype, *_ = get_args(fieldtype)
 
@@ -332,15 +331,15 @@
         def split_line(text: str) -> List[str]:
             parts = re.split("[ \t]", text.strip())
             return list(filter(lambda part: part != "", parts))
 
         table_text = list(DSerieParser.parse_list_group(text).values())[0]
         table_data = list(DSerieParser.parse_list_group(table_text).values())
         if len(table_data) == 0:
-            values_dict_list = table_data;
+            values_dict_list = table_data
             collection_property_name = list(cls.__fields__.items())[0][0]
             return cls(**{collection_property_name: values_dict_list})
         else:
             # Expected two groups (column_indication and data)
             keys = table_data[0].split("\n")
             keys = [make_key(j) for j in keys]
 
@@ -348,14 +347,15 @@
                 dict(zip(keys, values))
                 for values in map(split_line, table_data[1].split("\n"))
             ]
             collection_property_name = list(cls.__fields__.items())[0][0]
 
         return cls(**{collection_property_name: values_dict_list})
 
+
 class DSerieOldTableStructure(DSeriesStructure):
     @classmethod
     def parse_text(cls, text: str):
         """Creates a DSeriesStructure that can parse fields like
 
         [GROUP]
         [COLUMN INDICATION]
@@ -536,15 +536,15 @@
     @classmethod
     def get_properties_in_text(cls, text: str):
         required_properties_names = [
             structure_name for structure_name, _ in cls.get_structure_required_fields()
         ]
         header_lines = cls.header_lines()
         for idx, (key, value) in enumerate(
-                DSerieParser.parse_group(text, loose_properties=True)
+            DSerieParser.parse_group(text, loose_properties=True)
         ):
             if idx < header_lines:
                 continue
             if not key:
                 # Only loose properties would get through here.
                 # So a grouped property enclosed like [PROPERTY][END OF PROPERTY].
                 key, value = cls.get_property_key_value(
@@ -764,16 +764,16 @@
 
         Returns:
             DSeriesStructure: Parsed structrure.
         """
         generated_dict = {}
         no_key_group_values = []
         for group_key, group_values in groupby(
-                list(DSerieParser.parse_group(text, loose_properties=True)),
-                lambda key_value: key_value[0],
+            list(DSerieParser.parse_group(text, loose_properties=True)),
+            lambda key_value: key_value[0],
         ):
             filtered_values = [value for key, value in group_values]
             if not group_key:
                 no_key_group_values.extend(filtered_values)
                 continue
             if cls.group_value_is_list(group_key):
                 if group_key in generated_dict:
@@ -899,15 +899,15 @@
         parsed_structure, _ = cls.parse_text_lines(
             [split_line_elements(line) for line in text.split("\n") if line != ""]
         )
         return parsed_structure
 
     @classmethod
     def parse_text_lines(
-            cls, text_lines: List[List[str]]
+        cls, text_lines: List[List[str]]
     ) -> Tuple[DSeriesStructure, int]:
         """Parses a list of strings into the properties of a structure.
         Example:
             [   ["1", "Property value"],
                 ["2", "Values in Property"],
                 ["4", "2"]]
         Args:
@@ -919,15 +919,15 @@
 
         Returns:
             DSeriesStructure: Structure with parsed properties.
             int: Index of last line being read as part of current structure.
         """
 
         def get_list_values(
-                struct_idx: int, field_name: str, text_lines: list
+            struct_idx: int, field_name: str, text_lines: list
         ) -> Tuple[DSeriesStructure, int]:
             """Auxiliar method to either parse as a DSeriesStructure or as a list of
             any different object.
 
             Args:
                 struct_idx (int): Type index in the class definition.
                 field_name (str): Name of the field.
@@ -954,17 +954,17 @@
         for struct_idx, (field_name, field) in enumerate(required_fields):
             if lines_read >= len(text_lines):
                 raise ValueError(f"Expected text line property for {field_name}.")
             iteration_lines = 1
             field = unpack_if_union(field)
             # if the current property is a list, then extract the next line values.
             if (
-                    is_list(field)
-                    or issubclass(field, list)
-                    or is_structure_collection(field)
+                is_list(field)
+                or issubclass(field, list)
+                or is_structure_collection(field)
             ):
                 lines_to_parse = cls.get_next_property_text_lines(text_lines[lines_read:])
                 parsed_tuple = get_list_values(struct_idx, field_name, lines_to_parse)
                 (
                     properties[field_name],
                     iteration_lines,
                 ) = cls.get_tree_structure_read_lines(parsed_tuple)
@@ -990,15 +990,15 @@
         Returns:
             list: Filtered list of text to be parsed into a property.
         """
         return text_lines
 
     @classmethod
     def get_tree_structure_read_lines(
-            cls, parsed_tuple: Tuple[DSeriesStructure, int]
+        cls, parsed_tuple: Tuple[DSeriesStructure, int]
     ) -> Tuple[DSeriesStructure, int]:
         """Allows inherited classes to override how many lines have been actually been read
         for a given parsed structure based on the cls being instantiated.
 
         Args:
             parsed_tuple (Tuple[DSeriesStructure, int]): Tuple of parsed structure and read lines for it.
 
@@ -1052,15 +1052,15 @@
             for line in text_lines[0][0].split("\n")
             if line != ""
         ]
         return filtered_property_lines
 
     @classmethod
     def get_tree_structure_read_lines(
-            cls, parsed_tuple: Tuple[DSeriesStructure, int]
+        cls, parsed_tuple: Tuple[DSeriesStructure, int]
     ) -> Tuple[DSeriesStructure, int]:
         # Only one line is meant to be read as parsed_text_lines is mapped 1:1 lines-properties.
         return parsed_tuple[0], 1
 
 
 class DSeriesTreeStructureCollection(DSeriesStructure):
     # TODO Deprecate.
@@ -1103,15 +1103,15 @@
         Returns:
             int: Number of structures expected.
         """
         return int(get_line_property_value(lines[0][0], reversed_key=True))
 
     @classmethod
     def parse_collection_type(
-            cls, collecion_type: Type, lines: list
+        cls, collecion_type: Type, lines: list
     ) -> Tuple[DSeriesStructure, int]:
         return collecion_type.parse_text_lines(lines)
 
     @classmethod
     def parse_text_lines(cls, lines: List[str]) -> Tuple[DSeriesStructure, int]:
         # Get class types
         collection_property_name = list(cls.__fields__.items())[0][0]
@@ -1139,15 +1139,15 @@
 class DSeriesMatrixTreeStructureCollection(DSeriesTreeStructureCollection):
     # TODO Deprecate.
     # This class is overdoing logic that is later on being handled by its parent (DSeriesStructure).
     # It should therefore only be responsible for generating a dictionary of field name - string values,
     # but not object creation.
     @classmethod
     def parse_collection_type(
-            cls, collecion_type: Type, lines: list
+        cls, collecion_type: Type, lines: list
     ) -> Tuple[DSeriesStructure, int]:
         parsed_structure, _ = collecion_type.parse_text_lines(
             [[line] for line in lines[0]]
         )
         return parsed_structure, 1
 
 
@@ -1213,15 +1213,15 @@
         }
 
         """
         return dict(DSerieParser.parse_group(text_lines=text_lines, unique_keys=True))
 
     @staticmethod
     def parse_group(
-            text_lines: str, loose_properties: bool = False, unique_keys: bool = False
+        text_lines: str, loose_properties: bool = False, unique_keys: bool = False
     ) -> Iterable[Tuple[str, str]]:
         """Parses a text with headers such as [GROUP] and [END OF GROUP] and
         yields each property of the group as a Tuple[property name, value].
         Because it is an iterable it may contain repeated elements.
         Delegating responsibility on what to do with such elements to the caller.
 
         Example:
@@ -1286,17 +1286,17 @@
                 if currentkey:
                     data += line + "\n"
                 elif not currentkey and loose_properties:
                     yield (currentkey, line)
 
     @staticmethod
     def parse_list_group(
-            text: str,
-            exceptions=["vertical", "soil", "residual_settlements"],
-            skipped_keys=[],
+        text: str,
+        exceptions=["vertical", "soil", "residual_settlements"],
+        skipped_keys=[],
     ) -> Dict[str, Union[List[str], str]]:
         """Method to parse several groups in a sli/sld file that can include repeated groups.
 
         Includes an exception to always parse a group as a list.
         Can parse the following:
 
         [GROUP A]
@@ -1348,15 +1348,14 @@
                 elif currentkey == key:
                     raise ValueError(
                         f"Can't parse duplicate key at line {i} without first encountering and END OF."
                     )
 
                 # end of current group signaled with [END OF GROUP]
                 elif key == "end_of_" + currentkey:
-
                     # If key already exists, this is a repeated group -> List
                     if currentkey in parsed_dict:
                         # Append in case of a list (2+ elements)
                         if isinstance(parsed_dict[currentkey], list):
                             parsed_dict[currentkey].append(data.strip())
                         # Else create the list first (1 element)
                         else:
@@ -1494,15 +1493,15 @@
 
 
 def is_structure_collection(field: Type) -> bool:
     return inspect.isclass(field) and issubclass(field, DSeriesStructure)
 
 
 def read_property_as_list(
-        field_name: str, field: Type, text_lines: list
+    field_name: str, field: Type, text_lines: list
 ) -> Tuple[List[DSeriesStructure], int]:
     """Reads a property containing a collection of values represented as
     a list of strings.
 
     Args:
         field_name (str): Name of the field to parse.
         field (Type): Type to parse the values to.
@@ -1523,15 +1522,15 @@
     while len(list_values) < list_size:
         if lines_read >= len(text_lines):
             raise ValueError(f"Expected {list_size} values for property {field_name}.")
         iteration_lines = 1
         lines_to_parse = text_lines[lines_read:]
         if issubclass(field, DSeriesTreeStructureCollection):
             # If its an encapsuled collection, number of lines needs to be given.
-            lines_to_parse = text_lines[lines_read - 1:]
+            lines_to_parse = text_lines[lines_read - 1 :]
 
         if is_structure_collection(field):
             parsed_values, iteration_lines = field.parse_text_lines(lines_to_parse)
             list_values.append(parsed_values)
         else:
             parsed_values = text_lines[lines_read]
             list_values.extend(parsed_values)
```

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/drains.py` & `d_geolib-1.0.0/geolib/models/dsettlement/drains.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_model.py` & `d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_model.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_parserprovider.py` & `d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_parserprovider.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     @property
     def dserie_structure(self) -> Type[DSettlementOutputStructure]:
         return DSettlementOutputStructure
 
 
 class DSettlementParserProvider(BaseParserProvider):
-
     __input_parsers = None
     __output_parsers = None
 
     @property
     def input_parsers(self) -> Tuple[DSettlementInputParser]:
         if not self.__input_parsers:
             self.__input_parsers = (DSettlementInputParser(),)
```

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/dsettlement_structures.py` & `d_geolib-1.0.0/geolib/models/dsettlement/dsettlement_structures.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,14 @@
                     currentkey = key
                     if len(data) > 0:
                         args.extend(data)
                     data = []
 
                 # duplicate group before end
                 elif currentkey == key:
-
                     # If key already exists, this is a group -> List
                     if currentkey in parsed_dict:
                         parsed_dict[currentkey] = parsed_dict[currentkey] + [
                             "".join(data)
                         ]
                     elif currentkey in EXCEPTIONS:
                         parsed_dict[currentkey] = ["".join(data)]
```

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/internal.py` & `d_geolib-1.0.0/geolib/models/dsettlement/internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,14 @@
             )
             curve.id = new_curve_id
             self.curves.append(curve)
 
         return curve
 
     def create_curves(self, sorted_points: List[DSeriePoint]) -> List[Curve]:
-
         new_curves = [
             self.create_curve(sorted_points[i], sorted_points[i + 1])
             for i in range(len(sorted_points) - 1)
         ]
         return new_curves
 
     def __getitem__(self, curve_id: int) -> Curve:
@@ -267,15 +266,14 @@
 
 class Layers(DSeriesTreeStructureCollection):
     """Representation of [LAYERS] group."""
 
     layers: List[Layer] = []
 
     def add_layer(self, layer: Layer):
-
         if layer in self.layers:
             existing_layer = self.layers[self.layers.index(layer)]
             logger.warning(
                 f"It's not possible to replace existing layers: {existing_layer}"
             )
             return existing_layer
         else:
```

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/internal_soil.py` & `d_geolib-1.0.0/geolib/models/dsettlement/internal_soil.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/loads.py` & `d_geolib-1.0.0/geolib/models/dsettlement/loads.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,14 @@
     gamma: float = 0
     height: float = 0
     xl: float = 0
     xm: float = 0
     xr: float = 0
 
     def _to_internal(self, time: timedelta, p: Point) -> _OtherLoad:
-
         load_values = LoadValuesTrapeziform(
             gamma=self.gamma,
             height=self.height,
             xl=self.xl,
             xm=self.xm,
             xr=self.xr,
             Xp=p.x,
```

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/serializer.py` & `d_geolib-1.0.0/geolib/models/dsettlement/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/templates/input.sli.j2` & `d_geolib-1.0.0/geolib/models/dsettlement/templates/input.sli.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsettlement/templates/soil_template.j2` & `d_geolib-1.0.0/geolib/models/dsettlement/templates/soil_template.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/calculation_options.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/calculation_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Union
 
-from geolib.models import BaseDataClass
 from pydantic.types import confloat, conint
 
+from geolib.models import BaseDataClass
+
 from .settings import (
     CalculationType,
     DesignType,
     PartialFactorCalculationType,
     PartialFactorSetCUR,
     PartialFactorSetEC,
     PartialFactorSetEC7NADBE,
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/constructions.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/constructions.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_model.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from abc import ABCMeta, abstractmethod
 from pathlib import Path
 from subprocess import CompletedProcess, run
 from typing import Any, BinaryIO, List, Optional, Type, Union
 
+from pydantic import FilePath, PositiveFloat
+from pydantic.types import confloat, conint
+
 from geolib.geometry import Point
 from geolib.models import BaseDataClass, BaseModel, BaseModelStructure
 from geolib.models.dsheetpiling.constructions import DiaphragmWall, Pile, Sheet
 from geolib.models.meta import CONSOLE_RUN_BATCH_FLAG
 from geolib.soils import Soil
-from pydantic import FilePath, PositiveFloat
-from pydantic.types import confloat, conint
 
 from .calculation_options import CalculationOptions, CalculationOptionsPerStage
 from .dsheetpiling_parserprovider import DSheetPilingParserProvider
 from .internal import CalculationOptions as CalculationOptionsInternal
 from .internal import (
     DSheetPilingDumpStructure,
     DSheetPilingOutputStructure,
@@ -113,15 +114,14 @@
 class DiaphragmModelType(BaseModelType):
     method: Optional[LateralEarthPressureMethod] = None
     check_vertical_balance: Optional[bool] = None
     verification: Optional[bool] = None
     elastic_calculation: bool = False
     diepwand_calculation: bool = True
 
-
     @property
     def model(self) -> ModelType:
         return ModelType.SHEET_PILING
 
 
 class DSheetPilingModel(BaseModel):
     r"""DSheetPiling is a tool used to design sheetpile and diaphragm walls and
@@ -409,15 +409,15 @@
         """Adds other loads of type Moment, HorizontalLineLoad, NormalForce, SoilDisplacement or UniformLoad
 
         Args:
             load: Add a load with the types of Moment, HorizontalLineLoad, NormalForce, SoilDisplacement or UniformLoad.
             stage_id: Load is added to this stage.
 
         Note: SoilDisplacement and UniformLoad are only valid for a sheetpiling construction.
-        
+
         Raises:
             ValueError: When non-existing stage_id is passed.
             ValueError: When a verification calculation is selected but duration_type and load_type are not defined for the load.
         """
         self._check_if_stage_id_exists(stage_id)
         self.datastructure.input_data.add_load(load=load.to_internal(), stage_id=stage_id)
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_parserprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 
     @property
     def dserie_structure(self) -> Type[DSheetPilingDumpStructure]:
         return DSheetPilingDumpStructure
 
 
 class DSheetPilingParserProvider(BaseParserProvider):
-
     __input_parsers = None
     __output_parsers = None
 
     @property
     def input_parsers(self) -> Tuple[DSheetPilingInputParser]:
         if not self.__input_parsers:
             self.__input_parsers = (DSheetPilingInputParser(),)
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_structures.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_structures.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/dsheetpiling_validator.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/dsheetpiling_validator.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/internal.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/internal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import logging
 import warnings
 from abc import ABCMeta
 from enum import Enum, IntEnum
 from inspect import cleandoc
 from typing import Any, Dict, List, Optional, Set, Tuple, Union
 
+from pydantic import confloat, conint, conlist, constr
+
 import geolib.models.dsheetpiling.constructions as constructions
 from geolib.geometry import Point
 from geolib.models import BaseDataClass
 from geolib.models.dseries_parser import (
     DSerieListStructure,
     DSeriesInlineMappedProperties,
     DSeriesInlineReversedProperties,
@@ -18,15 +20,14 @@
     DSeriesStructureCollection,
     DSeriesTableStructure,
     DSeriesUnmappedNameProperties,
     DSeriesWrappedTableStructure,
     DSerieVersion,
 )
 from geolib.utils import make_newline_validator
-from pydantic import confloat, conint, conlist, constr
 
 from .calculation_options import (
     CalculationOptionsPerStage as CalculationOptionsPerStageExternal,
 )
 from .dsheetpiling_structures import (
     DSeriesPilingDumpParserStructure,
     DSeriesPilingParserStructure,
@@ -1299,28 +1300,36 @@
     factors_for_overall_stability: Optional[str]
     overall_stability_results: Optional[str]
 
     # Verify calculation according to CUR or EC7-NL with method B
     factors_for_verification: Optional[str]
 
     # Verify calculation according to CUR or EC7-NL
-    verify_step_6____5_serviceability_limit_state: Optional[BaseVerificationStructureProperties]
+    verify_step_6____5_serviceability_limit_state: Optional[
+        BaseVerificationStructureProperties
+    ]
     verify_step_6____5_multiplied_by_factor: Optional[BaseVerificationStructureProperties]
     verify_step_6____1_low_modulus_of_subgrade_reaction_and_high_passive_water_level: Optional[
-        BaseVerificationStructureProperties]
+        BaseVerificationStructureProperties
+    ]
     verify_step_6____2_high_modulus_of_subgrade_reaction_and_high_passive_water_level: Optional[
-        BaseVerificationStructureProperties]
+        BaseVerificationStructureProperties
+    ]
     verify_step_6____3_low_modulus_of_subgrade_reaction_and_low_passive_water_level: Optional[
-        BaseVerificationStructureProperties]
+        BaseVerificationStructureProperties
+    ]
     verify_step_6____4_high_modulus_of_subgrade_reaction_and_low_passive_water_level: Optional[
-        BaseVerificationStructureProperties]
+        BaseVerificationStructureProperties
+    ]
     cur_anchor_force_results: Optional[CurAnchorForceResults]
 
     # Verify calculation according to EC7-BE or EC7-General
-    verify_deformation_serviceability_limit_state: Optional[BaseVerificationStructureProperties]
+    verify_deformation_serviceability_limit_state: Optional[
+        BaseVerificationStructureProperties
+    ]
     eurocode_1_set_1: Optional[BaseVerificationStructureProperties]
     eurocode_1_set_2: Optional[BaseVerificationStructureProperties]
     eurocode_2: Optional[BaseVerificationStructureProperties]
     eurocode_3: Optional[BaseVerificationStructureProperties]
     eurocode_belgium_set_1: Optional[BaseVerificationStructureProperties]
     eurocode_belgium_set_2: Optional[BaseVerificationStructureProperties]
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/internal_partial_factors.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/internal_partial_factors.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,8 +360,7 @@
     geometrydeltaactivephreaticline: float = 0.05
     overallstabilityfactordrivingmoment: float = 1.10
     overallstabilityfactorcohesion: float = 1.50
     overallstabilityfactortgphi: float = 1.20
     overallstabilityfactorunitweight: float = 1.00
     factorrepvaluesmdpmax: float = 0.00
     verticalbalancegammamb: float = 1.25
-
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/loads.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/profiles.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/profiles.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/serializer.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/serializer.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/settings.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/settings.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum, IntEnum
 
-from geolib.models import BaseDataClass
 from pydantic import conint
 
+from geolib.models import BaseDataClass
+
 
 class LateralEarthPressureMethod(IntEnum):
     """The method for input of the lateral earth pressure ratio"""
 
     MIXED = 2
     KA_KO_KP = 0
     C_PHI_DELTA = 1
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/supports.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/supports.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,14 @@
     """Rigid support."""
 
     name: constr(min_length=1, max_length=50)
     level: float
     support_type: SupportType
 
     def to_internal(self) -> InternalSupport:
-
         rotational_stiffness, translational_stiffness = {
             SupportType.TRANSLATION.value: (0, 1),
             SupportType.ROTATION.value: (1, 0),
             SupportType.TRANSLATION_AND_ROTATION.value: (1, 1),
         }[self.support_type.value]
 
         return InternalSupport(
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/surface.py` & `d_geolib-1.0.0/geolib/models/dsheetpiling/surface.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,13 @@
                 f"X-coordinate first point should be zero, received {x_coords[0]}"
             )
         if x_coords != sorted(x_coords):
             raise ValueError("x-coordinates must be strictly increasing")
         return v
 
     def to_internal(self) -> InternalSurface:
-
         kwargs = self.dict(exclude_none=True, exclude={"points"})
         kwargs["points"] = [
             {"Nr": i, "X-coord": p.x, "Value": p.z}
             for i, p in enumerate(self.points, start=1)
         ]
         return InternalSurface(**kwargs)
```

### Comparing `d_geolib-0.6.0/geolib/models/dsheetpiling/templates/input.shi.j2` & `d_geolib-1.0.0/geolib/models/dsheetpiling/templates/input.shi.j2`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dstability/analysis.py` & `d_geolib-1.0.0/geolib/models/dstability/analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -188,15 +188,15 @@
     extrapolate_search_space: bool = True
     search_grid: DStabilitySearchGrid
     slip_plane_constraints: DStabilitySlipPlaneConstraints = (
         DStabilitySlipPlaneConstraints()
     )
     bottom_tangent_line_z: float
     number_of_tangent_lines: PositiveInt
-    space_tangent_lines: confloat(gt=0)
+    space_tangent_lines: confloat(gt=0)  # type: ignore
 
     def _to_internal_datastructure(self) -> PersistableBishopBruteForceSettings:
         return PersistableBishopBruteForceSettings(
             GridEnhancements=PersistableGridEnhancements(
                 ExtrapolateSearchSpace=self.extrapolate_search_space
             ),
             SearchGrid=self.search_grid._to_internal_datastructure(),
@@ -214,18 +214,24 @@
 
     Args:
         slipplane ([Point]): The points of the slipplane
     """
 
     _analysis_type: AnalysisType = AnalysisType.SPENCER
     slipplane: List[Point]
+    slip_plane_constraints: DStabilityGeneticSlipPlaneConstraints = (
+        DStabilityGeneticSlipPlaneConstraints()
+    )
 
     def _to_internal_datastructure(self) -> PersistableSpencerSettings:
         return PersistableSpencerSettings(
-            SlipPlane=[PersistablePoint(X=point.x, Z=point.z) for point in self.slipplane]
+            SlipPlane=[
+                PersistablePoint(X=point.x, Z=point.z) for point in self.slipplane
+            ],
+            SlipPlaneConstraints=self.slip_plane_constraints._to_internal_datastructure(),
         )
 
 
 class DStabilitySpencerGeneticAnalysisMethod(DStabilityAnalysisMethod):
     """Generates the input for the genetic spencer algorithm
 
     Args:
```

### Comparing `d_geolib-0.6.0/geolib/models/dstability/dstability_parserprovider.py` & `d_geolib-1.0.0/geolib/models/dstability/dstability_parserprovider.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
         return super().can_parse(filename) or filename.is_dir()
 
     def parse(self, filepath: DirectoryPath) -> BaseModelStructure:
         ds = {}
 
         # Find required .json files via type hints
         for field, fieldtype in get_filtered_type_hints(self.structure):
-
             # On List types, parse a folder
             if type(fieldtype) == _GenericAlias:  # quite hacky
                 element_type, *_ = fieldtype.__args__  # use getargs in 3.8
                 ds[field] = self.__parse_folder(element_type, filepath / "")
 
             # Otherwise it is a single .json in the root folder
             else:
@@ -76,15 +75,14 @@
         return [".stix"]
 
     def can_parse(self, filename: FilePath) -> bool:
         return filename.suffix in self.suffix_list
 
     def parse(self, filepath: FilePath) -> BaseModelStructure:
         with ZipFile(filepath) as zip:
-
             # Fix backslashes in zipfile (until fixed in DStability)
             for file in zip.filelist:
                 new_filename = file.filename.replace("\\", "/")
                 if new_filename != file.filename:
                     file.filename = new_filename
             for key in list(zip.NameToInfo.keys()):
                 new_key = key.replace("\\", "/")
@@ -93,15 +91,14 @@
 
             path = Path(zip)
             ds = super().parse(path)
         return ds
 
 
 class DStabilityParserProvider(BaseParserProvider):
-
     _input_parsers = None
     _output_parsers = None
 
     @property
     def input_parsers(self) -> Tuple[DStabilityParser, DStabilityZipParser]:
         if not self._input_parsers:
             self._input_parsers = (DStabilityZipParser(), DStabilityParser())
```

### Comparing `d_geolib-0.6.0/geolib/models/dstability/dstability_validator.py` & `d_geolib-1.0.0/geolib/models/dstability/dstability_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,46 +10,65 @@
     """Validator for DStability structure.
 
     Has access to self.ds from parent class.
     Will run all is_valid_ functions to check for validity."""
 
     def is_valid_stages(self) -> bool:
         """Number of stages should be the same:"""
+
+        stage_count = 0
+        for scenario in self.ds.scenarios:
+            for _ in scenario.Stages:
+                stage_count += 1
+
         lengths_set = set()
         valid = True
         for key, value in (
-            (k, v) for k, v in self.ds.dict().items() if "result" not in k
+            (k, v)
+            for k, v in self.ds.dict().items()
+            if "result" not in k
+            and "scenarios" not in k
+            and "calculationsettings" not in k
         ):  # Results not required for stage validity.
             if isinstance(value, list):
                 lengths_set.add(len(value))
-                if len(lengths_set) > 1:
+                if len(value) > stage_count:
                     logger.error(
                         f"{self.is_valid_stages.__doc__} {key} has different number of stages: {len(value)}."
                     )
                     valid = False
                     break
 
         return valid
 
     def is_valid_layer_loads(self) -> bool:
         """Each layer load must have a consolidation degree for each soil layer"""
-        for stage_id, _ in enumerate(self.ds.stages):
-            soil_layer_ids: Set[str] = {
-                layer.LayerId for layer in self.ds.soillayers[stage_id].SoilLayers
-            }
-
-            layer_load_layer_ids: Set[str] = set()
-            for layer_load in self.ds.loads[stage_id].LayerLoads:
-                layer_load_layer_ids.add(layer_load.LayerId)
-
-                consolidation_layer_id_references: Set[str] = set()
-                for consolidation in layer_load.Consolidations:
-                    consolidation_layer_id_references.add(consolidation.LayerId)
-                    if consolidation.LayerId is None:
+        for scenario_index, _ in enumerate(self.ds.scenarios):
+            for stage_index, _ in enumerate(self.ds.scenarios[scenario_index].Stages):
+                soil_layer_ids: Set[str] = {
+                    layer.LayerId
+                    for layer in self.ds._get_soil_layers(
+                        scenario_index, stage_index
+                    ).SoilLayers
+                }
+
+                if len(soil_layer_ids) == 0:
+                    return True
+
+                layer_load_layer_ids: Set[str] = set()
+                for layer_load in self.ds._get_loads(
+                    scenario_index, stage_index
+                ).LayerLoads:
+                    layer_load_layer_ids.add(layer_load.LayerId)
+
+                    consolidation_layer_id_references: Set[str] = set()
+                    for consolidation in layer_load.Consolidations:
+                        consolidation_layer_id_references.add(consolidation.LayerId)
+                        if consolidation.LayerId is None:
+                            return False
+                    if soil_layer_ids - consolidation_layer_id_references != set(
+                        [layer_load.LayerId]
+                    ):  # All other soillayer ids are included except the soillayers own id.
                         return False
-                if soil_layer_ids - consolidation_layer_id_references != set(
-                    [layer_load.LayerId]
-                ):  # All other soillayer ids are included except the soillayers own id.
+                if layer_load_layer_ids != soil_layer_ids:
                     return False
-            if layer_load_layer_ids != soil_layer_ids:
-                return False
         return True
```

### Comparing `d_geolib-0.6.0/geolib/models/dstability/internal.py` & `d_geolib-1.0.0/geolib/models/dstability/internal.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,16 +70,16 @@
     @classmethod
     def structure_group(cls):
         return cls.structure_name()
 
 
 # waternet schema
 class PersistablePoint(DStabilityBaseModelStructure):
-    X: Optional[float] = "NaN"
-    Z: Optional[float] = "NaN"
+    X: Optional[Union[float, str]] = "NaN"
+    Z: Optional[Union[float, str]] = "NaN"
 
 
 class PersistableHeadLine(DStabilityBaseModelStructure):
     Id: Optional[str]
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     Points: Optional[List[Optional[PersistablePoint]]]
@@ -103,15 +103,15 @@
 
     @classmethod
     def structure_name(cls) -> str:
         return "waternets"
 
     Id: Optional[str]
     ContentVersion: Optional[str] = "1"
-    PhreaticLineId: Optional[str]
+    PhreaticLineId: Optional[str] = None
     HeadLines: List[PersistableHeadLine] = []
     ReferenceLines: List[PersistableReferenceLine] = []
     UnitWeightWater: Optional[float] = 9.81
 
     def get_head_line(self, head_line_id: str) -> PersistableHeadLine:
         for head_line in self.HeadLines:
             if head_line.Id == head_line_id:
@@ -174,71 +174,73 @@
         reference_line.TopHeadLineId = top_head_line_id
 
         self.ReferenceLines.append(reference_line)
         return reference_line
 
 
 class PersistableDitchCharacteristics(DStabilityBaseModelStructure):
-    DitchBottomEmbankmentSide: Optional[float] = "NaN"
-    DitchBottomLandSide: Optional[float] = "NaN"
-    DitchEmbankmentSide: Optional[float] = "NaN"
-    DitchLandSide: Optional[float] = "NaN"
+    DitchBottomEmbankmentSide: Optional[Union[float, str]] = "NaN"
+    DitchBottomLandSide: Optional[Union[float, str]] = "NaN"
+    DitchEmbankmentSide: Optional[Union[float, str]] = "NaN"
+    DitchLandSide: Optional[Union[float, str]] = "NaN"
 
 
 class PersistableEmbankmentCharacteristics(DStabilityBaseModelStructure):
-    EmbankmentToeLandSide: Optional[float] = "NaN"
-    EmbankmentToeWaterSide: Optional[float] = "NaN"
-    EmbankmentTopLandSide: Optional[float] = "NaN"
-    EmbankmentTopWaterSide: Optional[float] = "NaN"
-    ShoulderBaseLandSide: Optional[float] = "NaN"
+    EmbankmentToeLandSide: Optional[Union[float, str]] = "NaN"
+    EmbankmentToeWaterSide: Optional[Union[float, str]] = "NaN"
+    EmbankmentTopLandSide: Optional[Union[float, str]] = "NaN"
+    EmbankmentTopWaterSide: Optional[Union[float, str]] = "NaN"
+    ShoulderBaseLandSide: Optional[Union[float, str]] = "NaN"
 
 
 class EmbankmentSoilScenarioEnum(str, Enum):
     CLAY_EMBANKMENT_ON_CLAY = "ClayEmbankmentOnClay"
     CLAY_EMBANKMENT_ON_SAND = "ClayEmbankmentOnSand"
     SAND_EMBANKMENT_ON_CLAY = "SandEmbankmentOnClay"
     SAND_EMBANKMENT_ON_SAND = "SandEmbankmentOnSand"
 
 
 class WaternetCreatorSettings(DStabilitySubStructure):
     """waternetcreatorsettings/waternetcreatorsettings_x.json"""
 
     AdjustForUplift: Optional[bool] = False
-    AquiferInsideAquitardLayerId: Optional[str]
-    AquiferLayerId: Optional[str]
-    AquiferLayerInsideAquitardLeakageLengthInwards: Optional[float] = "NaN"
-    AquiferLayerInsideAquitardLeakageLengthOutwards: Optional[float] = "NaN"
-    AquitardHeadLandSide: Optional[float] = "NaN"
-    AquitardHeadWaterSide: Optional[float] = "NaN"
+    AquiferInsideAquitardLayerId: Optional[str] = None
+    AquiferLayerId: Optional[str] = None
+    AquiferLayerInsideAquitardLeakageLengthInwards: Optional[Union[float, str]] = "NaN"
+    AquiferLayerInsideAquitardLeakageLengthOutwards: Optional[Union[float, str]] = "NaN"
+    AquitardHeadLandSide: Optional[Union[float, str]] = "NaN"
+    AquitardHeadWaterSide: Optional[Union[float, str]] = "NaN"
     ContentVersion: Optional[str] = "1"
     DitchCharacteristics: Optional[
         PersistableDitchCharacteristics
     ] = PersistableDitchCharacteristics()
     DrainageConstruction: Optional[PersistablePoint] = PersistablePoint()
     EmbankmentCharacteristics: Optional[
         PersistableEmbankmentCharacteristics
     ] = PersistableEmbankmentCharacteristics()
-    EmbankmentSoilScenario: EmbankmentSoilScenarioEnum = "ClayEmbankmentOnClay"
+    EmbankmentSoilScenario: EmbankmentSoilScenarioEnum = (
+        EmbankmentSoilScenarioEnum.CLAY_EMBANKMENT_ON_CLAY
+    )
     Id: Optional[str]
-    InitialLevelEmbankmentTopLandSide: Optional[float] = "NaN"
-    InitialLevelEmbankmentTopWaterSide: Optional[float] = "NaN"
-    IntrusionLength: Optional[float] = "NaN"
+    InitialLevelEmbankmentTopLandSide: Optional[Union[float, str]] = "NaN"
+    InitialLevelEmbankmentTopWaterSide: Optional[Union[float, str]] = "NaN"
+    IntrusionLength: Optional[Union[float, str]] = "NaN"
     IsAquiferLayerInsideAquitard: Optional[bool] = False
     IsDitchPresent: Optional[bool] = False
     IsDrainageConstructionPresent: Optional[bool] = False
-    MeanWaterLevel: Optional[float] = "NaN"
-    NormativeWaterLevel: Optional[float] = "NaN"
-    OffsetEmbankmentToeLandSide: Optional[float] = "NaN"
-    OffsetEmbankmentTopLandSide: Optional[float] = "NaN"
-    OffsetEmbankmentTopWaterSide: Optional[float] = "NaN"
-    OffsetShoulderBaseLandSide: Optional[float] = "NaN"
-    PleistoceneLeakageLengthInwards: Optional[float] = "NaN"
-    PleistoceneLeakageLengthOutwards: Optional[float] = "NaN"
+    MeanWaterLevel: Optional[Union[float, str]] = "NaN"
+    NormativeWaterLevel: Optional[Union[float, str]] = "NaN"
+    OffsetEmbankmentToeLandSide: Optional[Union[float, str]] = "NaN"
+    OffsetEmbankmentTopLandSide: Optional[Union[float, str]] = "NaN"
+    OffsetEmbankmentTopWaterSide: Optional[Union[float, str]] = "NaN"
+    OffsetShoulderBaseLandSide: Optional[Union[float, str]] = "NaN"
+    PleistoceneLeakageLengthInwards: Optional[Union[float, str]] = "NaN"
+    PleistoceneLeakageLengthOutwards: Optional[Union[float, str]] = "NaN"
     UseDefaultOffsets: Optional[bool] = True
-    WaterLevelHinterland: Optional[float] = "NaN"
+    WaterLevelHinterland: Optional[Union[float, str]] = "NaN"
 
     @classmethod
     def structure_group(cls) -> str:
         return "waternetcreatorsettings"
 
 
 class PersistableStochasticParameter(DStabilityBaseModelStructure):
@@ -308,16 +310,18 @@
     def add_state_point(self, state_point: PersistableStatePoint) -> None:
         self.StatePoints.append(state_point)
 
     def add_state_line(
         self,
         points: List[PersistablePoint],
         state_points: List[PersistableStateLinePoint],
-    ):
+    ) -> PersistableStateLine:
+        state_line = PersistableStateLine(Points=points, Values=state_points)
         self.StateLines.append(PersistableStateLine(Points=points, Values=state_points))
+        return state_line
 
     def get_state(
         self, state_id: int
     ) -> Union[PersistableStatePoint, PersistableStateLine]:
         for state in self.StatePoints + self.StateLines:
             if state.Id == str(state_id):
                 return state
@@ -361,32 +365,55 @@
     def structure_name(cls) -> str:
         return "stage"
 
     @classmethod
     def structure_group(cls) -> str:
         return "stages"
 
-    AnalysisType: Optional[AnalysisTypeEnum] = AnalysisType.BISHOP_BRUTE_FORCE
-    CalculationSettingsId: Optional[str]
-    ContentVersion: Optional[str] = "1"
     DecorationsId: Optional[str]
     GeometryId: Optional[str]
     Id: Optional[str]
     Label: Optional[str] = ""
     LoadsId: Optional[str]
     Notes: Optional[str] = ""
     ReinforcementsId: Optional[str]
-    ResultId: Optional[str] = None
     SoilLayersId: Optional[str]
     StateCorrelationsId: Optional[str]
     StateId: Optional[str]
     WaternetCreatorSettingsId: Optional[str]
     WaternetId: Optional[str]
 
 
+class PersistableCalculation(DStabilityBaseModelStructure):
+    Id: Optional[str]
+    Label: Optional[str] = ""
+    Notes: Optional[str] = ""
+    ResultId: Optional[str] = None
+    CalculationSettingsId: Optional[str]
+
+
+class Scenario(DStabilitySubStructure):
+    """scenarios/scenario_x.json"""
+
+    @classmethod
+    def structure_name(cls) -> str:
+        return "scenario"
+
+    @classmethod
+    def structure_group(cls) -> str:
+        return "scenarios"
+
+    Stages: Optional[List[Stage]] = []
+    Calculations: Optional[List[PersistableCalculation]] = []
+    ContentVersion: Optional[str] = "2"
+    Id: Optional[str]
+    Label: Optional[str] = ""
+    Notes: Optional[str] = ""
+
+
 class PersistableShadingType(Enum):
     DIAGONAL_A = "DiagonalA"
     DIAGONAL_B = "DiagonalB"
     DIAGONAL_C = "DiagonalC"
     DIAGONAL_D = "DiagonalD"
     DOT_A = "DotA"
     DOT_B = "DotB"
@@ -478,22 +505,24 @@
 
 class ShearStrengthModelTypePhreaticLevelInternal(Enum):
     """
     Shear Strength Model Type. These types represent the types that
     are internally defined in the json files of D-Stability.
     """
 
-    C_PHI = "CPhi"
+    MOHR_COULOMB_ADVANCED = "MohrCoulombAdvanced"
+    MOHR_COULOMB_CLASSIC = "MohrCoulombClassic"
     NONE = "None"
     SU = "Su"
     SUTABLE = "SuTable"
 
     def to_global_shear_strength_model(self):
         transform_dictionary = {
-            "CPhi": "Mohr_Coulomb",
+            "MohrCoulombAdvanced": "Mohr_Coulomb",
+            "MohrCoulombClassic": "Mohr_Coulomb",
             "None": "None",
             "Su": "SHANSEP",
             "SuTable": "SuTable",
         }
         return transform_dictionary[self.value]
 
 
@@ -518,47 +547,74 @@
         for su_table_point in self.SuTablePoints:
             su_table.append(
                 SuTablePoint(su=su_table_point.Su, stress=su_table_point.EffectiveStress)
             )
         return su_table
 
 
-class PersistableSoil(DStabilityBaseModelStructure):
-    Code: str = ""
-    Cohesion: float = 0.0
+class PersistableMohrCoulombClassicShearStrengthModel(DStabilityBaseModelStructure):
+    Cohesion: Optional[float] = 0.0
     CohesionAndFrictionAngleCorrelated: bool = False
     CohesionStochasticParameter: PersistableStochasticParameter = (
         PersistableStochasticParameter()
     )
-    Dilatancy: float = 0.0
+    FrictionAngle: Optional[float] = 0.0
+    FrictionAngleStochasticParameter: PersistableStochasticParameter = (
+        PersistableStochasticParameter()
+    )
+
+
+class PersistableMohrCoulombAdvancedShearStrengthModel(DStabilityBaseModelStructure):
+    Cohesion: Optional[float] = 0.0
+    CohesionAndFrictionAngleCorrelated: bool = False
+    CohesionStochasticParameter: PersistableStochasticParameter = (
+        PersistableStochasticParameter()
+    )
+    Dilatancy: Optional[float] = 0.0
     DilatancyStochasticParameter: PersistableStochasticParameter = (
         PersistableStochasticParameter()
     )
-    FrictionAngle: float = 0.0
+    FrictionAngle: Optional[float] = 0.0
     FrictionAngleStochasticParameter: PersistableStochasticParameter = (
         PersistableStochasticParameter()
     )
+
+
+class PersistableSuShearStrengthModel(DStabilityBaseModelStructure):
+    ShearStrengthRatio: Optional[float] = 0.0
+    ShearStrengthRatioAndShearStrengthExponentCorrelated: bool = False
+    ShearStrengthRatioStochasticParameter: PersistableStochasticParameter = (
+        PersistableStochasticParameter()
+    )
+    StrengthIncreaseExponent: Optional[float] = 1.0
+    StrengthIncreaseExponentStochasticParameter: PersistableStochasticParameter = (
+        PersistableStochasticParameter()
+    )
+
+
+class PersistableSoil(DStabilityBaseModelStructure):
+    Code: str = ""
     Id: str = ""
     IsProbabilistic: bool = False
     Name: Optional[str] = ""
     Notes: Optional[str] = ""
     ShearStrengthModelTypeAbovePhreaticLevel: ShearStrengthModelTypePhreaticLevelInternal = (
-        ShearStrengthModelTypePhreaticLevelInternal.C_PHI
+        ShearStrengthModelTypePhreaticLevelInternal.MOHR_COULOMB_ADVANCED
     )
     ShearStrengthModelTypeBelowPhreaticLevel: ShearStrengthModelTypePhreaticLevelInternal = (
         ShearStrengthModelTypePhreaticLevelInternal.SU
     )
-    ShearStrengthRatio: float = 0.0
-    ShearStrengthRatioAndShearStrengthExponentCorrelated: bool = False
-    ShearStrengthRatioStochasticParameter: PersistableStochasticParameter = (
-        PersistableStochasticParameter()
+    MohrCoulombClassicShearStrengthModel: PersistableMohrCoulombClassicShearStrengthModel = (
+        PersistableMohrCoulombClassicShearStrengthModel()
     )
-    StrengthIncreaseExponent: float = 1.0
-    StrengthIncreaseExponentStochasticParameter: PersistableStochasticParameter = (
-        PersistableStochasticParameter()
+    MohrCoulombAdvancedShearStrengthModel: PersistableMohrCoulombAdvancedShearStrengthModel = (
+        PersistableMohrCoulombAdvancedShearStrengthModel()
+    )
+    SuShearStrengthModel: PersistableSuShearStrengthModel = (
+        PersistableSuShearStrengthModel()
     )
     VolumetricWeightAbovePhreaticLevel: float = 0.0
     VolumetricWeightBelowPhreaticLevel: float = 0.0
     SuTable: PersistableSuTable = PersistableSuTable()
 
 
 class SoilCollection(DStabilitySubStructure):
@@ -566,145 +622,140 @@
 
     ContentVersion: Optional[str] = "1"
     Soils: List[PersistableSoil] = [
         PersistableSoil(
             Id="2",
             Name="Embankment new",
             Code="H_Aa_ht_new",
-            Cohesion=7.0,
-            FrictionAngle=30.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.26,
-            StrengthIncreaseExponent=0.9,
+            MohrCoulombAdvancedShearStrengthModel=PersistableMohrCoulombAdvancedShearStrengthModel(
+                Cohesion=7.0, FrictionAngle=30.0, Dilatancy=0.0
+            ),
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.26,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=19.3,
             VolumetricWeightBelowPhreaticLevel=19.3,
         ),
         PersistableSoil(
             Id="3",
             Name="Embankment old",
             Code="H_Aa_ht_old",
-            Cohesion=7.0,
-            FrictionAngle=30.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.26,
-            StrengthIncreaseExponent=0.9,
+            MohrCoulombAdvancedShearStrengthModel=PersistableMohrCoulombAdvancedShearStrengthModel(
+                Cohesion=7.0, FrictionAngle=30.0, Dilatancy=0.0
+            ),
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.26,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=18.0,
             VolumetricWeightBelowPhreaticLevel=18.0,
         ),
         PersistableSoil(
             Id="4",
             Name="Clay, shallow",
             Code="H_Rk_k_shallow",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.23,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.23,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=14.8,
             VolumetricWeightBelowPhreaticLevel=14.8,
         ),
         PersistableSoil(
             Id="5",
             Name="Clay, deep",
             Code="H_Rk_k_deep",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.23,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.23,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=15.6,
             VolumetricWeightBelowPhreaticLevel=15.6,
         ),
         PersistableSoil(
             Id="6",
             Name="Organic clay",
             Code="H_Rk_ko",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.24,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.85,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.24,
+                StrengthIncreaseExponent=0.85,
+            ),
             VolumetricWeightAbovePhreaticLevel=13.9,
             VolumetricWeightBelowPhreaticLevel=13.9,
         ),
         PersistableSoil(
             Id="7",
             Name="Peat, shallow",
             Code="H_vhv_v",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.3,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.3,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=10.1,
             VolumetricWeightBelowPhreaticLevel=10.1,
         ),
         PersistableSoil(
             Id="8",
             Name="Peat, deep",
             Code="H_vbv_v",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.27,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.27,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=11.0,
             VolumetricWeightBelowPhreaticLevel=11.0,
         ),
         PersistableSoil(
             Id="9",
             Name="Sand",
             Code="Sand",
-            Cohesion=0.0,
-            FrictionAngle=30.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.0,
-            ShearStrengthModelTypeBelowPhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.C_PHI,
-            StrengthIncreaseExponent=0.0,
+            MohrCoulombAdvancedShearStrengthModel=PersistableMohrCoulombAdvancedShearStrengthModel(
+                Cohesion=0.0, FrictionAngle=30.0, Dilatancy=0.0
+            ),
+            ShearStrengthModelTypeBelowPhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.MOHR_COULOMB_ADVANCED,
             VolumetricWeightAbovePhreaticLevel=18.0,
             VolumetricWeightBelowPhreaticLevel=20.0,
         ),
         PersistableSoil(
             Id="10",
             Name="Clay with silt",
             Code="P_Rk_k&s",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.22,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.22,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=18.0,
             VolumetricWeightBelowPhreaticLevel=18.0,
         ),
         PersistableSoil(
             Id="11",
             Name="Sand with clay",
             Code="H_Ro_z&k",
-            Cohesion=0.0,
-            FrictionAngle=0.0,
-            Dilatancy=0.0,
-            ShearStrengthRatio=0.22,
             ShearStrengthModelTypeAbovePhreaticLevel=ShearStrengthModelTypePhreaticLevelInternal.SU,
-            StrengthIncreaseExponent=0.9,
+            SuShearStrengthModel=PersistableSuShearStrengthModel(
+                ShearStrengthRatio=0.22,
+                StrengthIncreaseExponent=0.9,
+            ),
             VolumetricWeightAbovePhreaticLevel=18.0,
             VolumetricWeightBelowPhreaticLevel=18.0,
         ),
     ]
 
     @classmethod
     def structure_name(cls) -> str:
         return "soils"
 
-    def has_soilcode(self, code: str) -> bool:
+    def has_soil_code(self, code: str) -> bool:
         """
         Checks if the soilcode is available in the current soil list.
 
         Args:
             code (str): code of the soil
 
         Returns:
@@ -743,15 +794,15 @@
         # shear increase exponent taken from persistable_soil.SuTable or just from persistable_soil
         if (
             persistable_soil.ShearStrengthModelTypeAbovePhreaticLevel.value == "Su"
             or persistable_soil.ShearStrengthModelTypeBelowPhreaticLevel.value == "Su"
         ):
             # SHANSEP model is selected so the StrengthIncreaseExponentStochasticParameter from persistable_soil should be used
             return self.__to_global_stochastic_parameter(
-                persistable_soil.StrengthIncreaseExponentStochasticParameter
+                persistable_soil.SuShearStrengthModel.StrengthIncreaseExponentStochasticParameter
             )
         elif (
             persistable_soil.ShearStrengthModelTypeAbovePhreaticLevel.value == "SuTable"
             or persistable_soil.ShearStrengthModelTypeBelowPhreaticLevel.value
             == "SuTable"
         ):
             # SU table is selected so the StrengthIncreaseExponentStochasticParameter from SuTable should be used
@@ -766,34 +817,34 @@
             MohrCoulombParameters,
             SoilWeightParameters,
             UndrainedParameters,
         )
 
         mohr_coulomb_parameters = MohrCoulombParameters(
             cohesion=self.__to_global_stochastic_parameter(
-                persistable_soil.CohesionStochasticParameter
+                persistable_soil.MohrCoulombAdvancedShearStrengthModel.CohesionStochasticParameter
             ),
             friction_angle=self.__to_global_stochastic_parameter(
-                persistable_soil.FrictionAngleStochasticParameter
+                persistable_soil.MohrCoulombAdvancedShearStrengthModel.FrictionAngleStochasticParameter
             ),
             dilatancy_angle=self.__to_global_stochastic_parameter(
-                persistable_soil.DilatancyStochasticParameter
+                persistable_soil.MohrCoulombAdvancedShearStrengthModel.DilatancyStochasticParameter
             ),
-            cohesion_and_friction_angle_correlated=persistable_soil.CohesionAndFrictionAngleCorrelated,
+            cohesion_and_friction_angle_correlated=persistable_soil.MohrCoulombAdvancedShearStrengthModel.CohesionAndFrictionAngleCorrelated,
         )
 
         strength_increase_exponent = self.__determine_strength_increase_exponent(
             persistable_soil
         )
         undrained_parameters = UndrainedParameters(
             shear_strength_ratio=self.__to_global_stochastic_parameter(
-                persistable_soil.ShearStrengthRatioStochasticParameter
+                persistable_soil.SuShearStrengthModel.ShearStrengthRatioStochasticParameter
             ),
             strength_increase_exponent=strength_increase_exponent,
-            shear_strength_ratio_and_shear_strength_exponent_correlated=persistable_soil.ShearStrengthRatioAndShearStrengthExponentCorrelated,
+            shear_strength_ratio_and_shear_strength_exponent_correlated=persistable_soil.SuShearStrengthModel.ShearStrengthRatioAndShearStrengthExponentCorrelated,
             su_table=persistable_soil.SuTable.to_global_su_table(),
             probabilistic_su_table=persistable_soil.SuTable.IsSuTableProbabilistic,
             su_table_variation_coefficient=persistable_soil.SuTable.SuTableVariationCoefficient,
         )
 
         soil_weight_parameters = SoilWeightParameters()
         soil_weight_parameters.saturated_weight.mean = (
@@ -811,81 +862,61 @@
             shear_strength_model_above_phreatic_level=persistable_soil.ShearStrengthModelTypeAbovePhreaticLevel.to_global_shear_strength_model(),
             shear_strength_model_below_phreatic_level=persistable_soil.ShearStrengthModelTypeBelowPhreaticLevel.to_global_shear_strength_model(),
             mohr_coulomb_parameters=mohr_coulomb_parameters,
             soil_weight_parameters=soil_weight_parameters,
             undrained_parameters=undrained_parameters,
         )
 
-    def get_soil(self, code: str) -> Soil:
+    def get_soil(self, code: str) -> PersistableSoil:
         """
         Get soil by the given code.
 
         Args:
             code (str): code of the soil
 
         Returns:
             Soil: the soil object
         """
         for persistable_soil in self.Soils:
             if persistable_soil.Code == code:
-                return self.__internal_soil_to_global_soil(persistable_soil)
+                return persistable_soil
 
         raise ValueError(f"Soil code '{code}' not found in the SoilCollection")
 
-    def edit_soil(self, code: str, **kwargs: dict) -> PersistableSoil:
+    def get_soil_by_name(self, name: str) -> PersistableSoil:
         """
-        Update a soil.
+        Get soil by the given name.
 
         Args:
-            code (str): code of the soil.
-            kwargs (dict): dictionary with argument names and values
+            code (str): name of the soil
 
         Returns:
-            PersistableSoil: the edited soil
+            Soil: the soil object
         """
-
         for persistable_soil in self.Soils:
-            if persistable_soil.Code == code:
-                return self.edit_persistable_soil(
-                    persistable_soil=persistable_soil, kwargs=kwargs
-                )
-        raise ValueError(f"Soil code '{code}' not found in the SoilCollection")
+            if persistable_soil.Name == name:
+                return persistable_soil
+
+        raise ValueError(f"Soil name '{name}' not found in the SoilCollection")
 
-    def edit_soil_by_name(
-        self, name: Optional[str] = None, **kwargs: dict
-    ) -> PersistableSoil:
+    def get_global_soil(self, code: str) -> Soil:
         """
-        Update a soil, searching by name. This method will edit the first occurence of the name
-        if it is used multiple times.
+        Get soil by the given code.
 
         Args:
-            name (str): name of the soil.
-            kwargs (dict): dictionary with argument names and values
+            code (str): code of the soil
 
         Returns:
-            PersistableSoil: the edited soil
+            Soil: the soil object
         """
-
         for persistable_soil in self.Soils:
-            if persistable_soil.Name == name:
-                return self.edit_persistable_soil(
-                    persistable_soil=persistable_soil, kwargs=kwargs
-                )
-        raise ValueError(f"Soil name '{name}' not found in the SoilCollection")
+            if persistable_soil.Code == code:
+                return self.__internal_soil_to_global_soil(persistable_soil)
 
-    def edit_persistable_soil(self, persistable_soil: PersistableSoil, kwargs: dict):
-        for k, v in kwargs.items():
-            try:
-                setattr(persistable_soil, snake_to_camel(k), v)
-                k_stochastic = f"{snake_to_camel(k)}StochasticParameter"
-                if hasattr(persistable_soil, k_stochastic):
-                    getattr(persistable_soil, k_stochastic).Mean = v
-            except AttributeError:
-                raise ValueError(f"Unknown soil parameter {k}.")
-        return persistable_soil
+        raise ValueError(f"Soil code '{code}' not found in the SoilCollection")
 
 
 # Reinforcements
 
 
 class PersistableForbiddenLine(DStabilityBaseModelStructure):
     Label: Optional[str] = ""
@@ -1177,15 +1208,15 @@
             Points=[PersistablePoint(X=p.x, Z=p.z) for p in points],
         )
 
         self.Layers.append(layer)
         return layer
 
 
-class PersistableBerm(DStabilityBaseModelStructure):
+class PersistableElevation(DStabilityBaseModelStructure):
     AddedLayerId: Optional[str]
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     Points: Optional[List[Optional[PersistablePoint]]]
 
 
 class PersistableExcavation(DStabilityBaseModelStructure):
@@ -1193,41 +1224,41 @@
     Notes: Optional[str] = ""
     Points: Optional[List[Optional[PersistablePoint]]]
 
 
 class Decorations(DStabilitySubStructure):
     """decorations/decorations_x.json."""
 
-    Berms: Optional[List[Optional[PersistableBerm]]] = []
+    Elevations: Optional[List[Optional[PersistableElevation]]] = []
     ContentVersion: Optional[str] = "1"
     Excavations: Optional[List[Optional[PersistableExcavation]]] = []
     Id: Optional[str]
 
 
 # Calculation Settings
 
 
 class PersistableCircle(DStabilityBaseModelStructure):
     Center: Optional[PersistablePoint] = PersistablePoint()
-    Radius: Optional[float] = "NaN"
+    Radius: Optional[Union[float, str]] = "NaN"
 
 
 class PersistableBishopSettings(DStabilityBaseModelStructure):
     Circle: Optional[PersistableCircle] = PersistableCircle()
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
 
 
 class PersistableGridEnhancements(DStabilityBaseModelStructure):
     ExtrapolateSearchSpace: Optional[bool] = True
 
 
 class NullablePersistablePoint(DStabilityBaseModelStructure):
-    X: Optional[float] = "NaN"
-    Z: Optional[float] = "NaN"
+    X: Optional[Union[float, str]] = "NaN"
+    Z: Optional[Union[float, str]] = "NaN"
 
 
 class PersistableSearchGrid(DStabilityBaseModelStructure):
     BottomLeft: Optional[NullablePersistablePoint] = None
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     NumberOfPointsInX: Optional[int] = 1
@@ -1244,15 +1275,15 @@
     WidthZoneA: Optional[float] = 0.0
     WidthZoneB: Optional[float] = 0.0
     XLeftZoneA: Optional[float] = 0.0
     XLeftZoneB: Optional[float] = 0.0
 
 
 class PersistableTangentLines(DStabilityBaseModelStructure):
-    BottomTangentLineZ: Optional[float] = "NaN"
+    BottomTangentLineZ: Optional[Union[float, str]] = "NaN"
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     NumberOfTangentLines: Optional[int] = 1
     Space: Optional[float] = 0.5
 
 
 class PersistableBishopBruteForceSettings(DStabilityBaseModelStructure):
@@ -1272,48 +1303,51 @@
     MEAN = "Mean"
     PROBABILISTIC = "Probabilistic"
 
 
 CalculationType = CalculationTypeEnum
 
 
+class PersistableGeneticSlipPlaneConstraints(DStabilityBaseModelStructure):
+    IsEnabled: Optional[bool] = False
+    MinimumAngleBetweenSlices: Optional[float] = 0.0
+    MinimumThrustLinePercentageInsideSlices: Optional[float] = 0.0
+
+
 class PersistableSpencerSettings(DStabilityBaseModelStructure):
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     SlipPlane: Optional[List[Optional[PersistablePoint]]] = None
+    SlipPlaneConstraints: Optional[
+        PersistableGeneticSlipPlaneConstraints
+    ] = PersistableGeneticSlipPlaneConstraints()
 
 
 class OptionsTypeEnum(Enum):
     DEFAULT = "Default"
     THOROUGH = "Thorough"
 
 
 OptionsType = OptionsTypeEnum
 
 
-class PersistableGeneticSlipPlaneConstraints(DStabilityBaseModelStructure):
-    IsEnabled: Optional[bool] = False
-    MinimumAngleBetweenSlices: Optional[float] = 0.0
-    MinimumThrustLinePercentageInsideSlices: Optional[float] = 0.0
-
-
 class PersistableSpencerGeneticSettings(DStabilityBaseModelStructure):
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     OptionsType: Optional[OptionsTypeEnum] = OptionsType.DEFAULT
     SlipPlaneA: Optional[List[Optional[PersistablePoint]]] = None
     SlipPlaneB: Optional[List[Optional[PersistablePoint]]] = None
     SlipPlaneConstraints: Optional[
         PersistableGeneticSlipPlaneConstraints
     ] = PersistableGeneticSlipPlaneConstraints()
 
 
 class PersistableTwoCirclesOnTangentLine(DStabilityBaseModelStructure):
     FirstCircleCenter: Optional[NullablePersistablePoint] = NullablePersistablePoint()
-    FirstCircleRadius: Optional[float] = "NaN"
+    FirstCircleRadius: Optional[Union[float, str]] = "NaN"
     SecondCircleCenter: Optional[NullablePersistablePoint] = NullablePersistablePoint()
 
 
 class PersistableUpliftVanSettings(DStabilityBaseModelStructure):
     Label: Optional[str] = ""
     Notes: Optional[str] = ""
     SlipPlane: Optional[
@@ -1347,15 +1381,15 @@
     ] = PersistableSlipPlaneConstraints()
     TangentArea: Optional[PersistableTangentArea] = PersistableTangentArea()
 
 
 class CalculationSettings(DStabilitySubStructure):
     """calculationsettings/calculationsettings_x.json"""
 
-    AnalysisType: Optional[AnalysisTypeEnum]
+    AnalysisType: Optional[AnalysisTypeEnum] = AnalysisTypeEnum.BISHOP_BRUTE_FORCE
     Bishop: Optional[PersistableBishopSettings] = PersistableBishopSettings()
     BishopBruteForce: Optional[
         PersistableBishopBruteForceSettings
     ] = PersistableBishopBruteForceSettings()
     CalculationType: Optional[CalculationTypeEnum] = CalculationTypeEnum.DETERMINISTIC
     ContentVersion: Optional[str] = "1"
     Id: Optional[str] = "19"
@@ -1477,18 +1511,18 @@
     Alpha: Optional[float] = None
     Property: Optional[str] = None
     SoilId: Optional[str] = None
     UncorrelatedAlpha: Optional[float] = None
     Value: Optional[float] = None
 
 
-class PersistableStageContribution(DStabilityBaseModelStructure):
+class PersistableCalculationContribution(DStabilityBaseModelStructure):
     Alpha: Optional[float] = None
     Property: Optional[str] = None
-    StageId: Optional[str] = None
+    CalculationId: Optional[str] = None
     UncorrelatedAlpha: Optional[float] = None
     Value: Optional[float] = None
 
 
 class PersistableStateLinePointContribution(DStabilityBaseModelStructure):
     Alpha: Optional[float] = None
     Property: Optional[str] = None
@@ -1507,16 +1541,19 @@
 
 class BishopReliabilityResult(DStabilitySubStructure):
     Circle: Optional[PersistableCircle] = None
     Converged: Optional[bool] = None
     FailureProbability: Optional[float] = None
     Id: Optional[str] = None
     ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
     SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
-    StageContributions: Optional[List[Optional[PersistableStageContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
     StateLinePointContributions: Optional[
         List[Optional[PersistableStateLinePointContribution]]
     ] = None
     StatePointContributions: Optional[
         List[Optional[PersistableStatePointContribution]]
     ] = None
 
@@ -1532,14 +1569,48 @@
             )
         except (ValidationError, AttributeError):
             raise ValueError(
                 f"Slipcircle not available for {self.__class__.__name__} with id {self.Id}"
             )
 
 
+class BishopBruteForceReliabilityResult(DStabilitySubStructure):
+    Circle: Optional[PersistableCircle] = None
+    Converged: Optional[bool] = None
+    FailureProbability: Optional[float] = None
+    Id: Optional[str] = None
+    ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
+    SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
+    StateLinePointContributions: Optional[
+        List[Optional[PersistableStateLinePointContribution]]
+    ] = None
+    StatePointContributions: Optional[
+        List[Optional[PersistableStatePointContribution]]
+    ] = None
+
+    @classmethod
+    def structure_group(cls) -> str:
+        return "results/bishopbruteforcereliability/"
+
+    def get_slipcircle_output(self) -> BishopSlipCircleResult:
+        """Get condensed slipcircle data"""
+        try:
+            return BishopSlipCircleResult(
+                x=self.Circle.Center.X, z=self.Circle.Center.Z, radius=self.Circle.Radius
+            )
+        except (ValidationError, AttributeError):
+            raise ValueError(
+                f"Slipcircle not available for {self.__class__.__name__} with id {self.Id}"
+            )
+
+
 class BishopResult(DStabilitySubStructure):
     Circle: Optional[PersistableCircle] = None
     FactorOfSafety: Optional[float] = None
     Id: Optional[str] = None
     Points: Optional[List[Optional[PersistablePoint]]] = None
     Slices: Optional[List[Optional[PersistableSlice]]] = None
 
@@ -1632,17 +1703,20 @@
 
 
 class SpencerReliabilityResult(DStabilitySubStructure):
     Converged: Optional[bool] = None
     FailureProbability: Optional[float] = None
     Id: Optional[str] = None
     ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
     SlipPlane: Optional[List[Optional[PersistablePoint]]] = None
     SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
-    StageContributions: Optional[List[Optional[PersistableStageContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
     StateLinePointContributions: Optional[
         List[Optional[PersistableStateLinePointContribution]]
     ] = None
     StatePointContributions: Optional[
         List[Optional[PersistableStatePointContribution]]
     ] = None
 
@@ -1658,14 +1732,48 @@
             )
         except (ValidationError, TypeError):
             raise ValueError(
                 f"Slip plane not available for {self.__class__.__name__} with id {self.Id}"
             )
 
 
+class SpencerGeneticAlgorithmReliabilityResult(DStabilitySubStructure):
+    Converged: Optional[bool] = None
+    FailureProbability: Optional[float] = None
+    Id: Optional[str] = None
+    ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
+    SlipPlane: Optional[List[Optional[PersistablePoint]]] = None
+    SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
+    StateLinePointContributions: Optional[
+        List[Optional[PersistableStateLinePointContribution]]
+    ] = None
+    StatePointContributions: Optional[
+        List[Optional[PersistableStatePointContribution]]
+    ] = None
+
+    @classmethod
+    def structure_group(cls) -> str:
+        return "results/spencergeneticreliability/"
+
+    def get_slipplane_output(self) -> SpencerSlipPlaneResult:
+        """Get condensed slipplane data"""
+        try:
+            return SpencerSlipPlaneResult(
+                slipplane=[Point(x=p.X, z=p.Z) for p in self.SlipPlane]
+            )
+        except (ValidationError, TypeError):
+            raise ValueError(
+                f"Slip plane not available for {self.__class__.__name__} with id {self.Id}"
+            )
+
+
 class SpencerResult(DStabilitySubStructure):
     FactorOfSafety: Optional[float] = None
     Id: Optional[str] = None
     Points: Optional[List[Optional[PersistablePoint]]] = None
     Slices: Optional[List[Optional[PersistableSpencerSlice]]] = None
     SlipPlane: Optional[List[Optional[PersistablePoint]]] = None
 
@@ -1716,17 +1824,20 @@
 
 class UpliftVanReliabilityResult(DStabilitySubStructure):
     Converged: Optional[bool] = None
     FailureProbability: Optional[float] = None
     Id: Optional[str] = None
     LeftCenter: Optional[PersistablePoint] = None
     ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
     RightCenter: Optional[PersistablePoint] = None
     SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
-    StageContributions: Optional[List[Optional[PersistableStageContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
     StateLinePointContributions: Optional[
         List[Optional[PersistableStateLinePointContribution]]
     ] = None
     StatePointContributions: Optional[
         List[Optional[PersistableStatePointContribution]]
     ] = None
     TangentLine: Optional[float] = None
@@ -1747,14 +1858,54 @@
             )
         except (ValidationError, AttributeError):
             raise ValueError(
                 f"Slipcircle not available for {self.__class__.__name__} with id {self.Id}"
             )
 
 
+class UpliftVanParticleSwarmReliabilityResult(DStabilitySubStructure):
+    Converged: Optional[bool] = None
+    FailureProbability: Optional[float] = None
+    Id: Optional[str] = None
+    LeftCenter: Optional[PersistablePoint] = None
+    ReliabilityIndex: Optional[float] = None
+    DistanceToConvergence: Optional[float] = None
+    RightCenter: Optional[PersistablePoint] = None
+    SoilContributions: Optional[List[Optional[PersistableSoilContribution]]] = None
+    CalculationContributions: Optional[
+        List[Optional[PersistableCalculationContribution]]
+    ] = None
+    StateLinePointContributions: Optional[
+        List[Optional[PersistableStateLinePointContribution]]
+    ] = None
+    StatePointContributions: Optional[
+        List[Optional[PersistableStatePointContribution]]
+    ] = None
+    TangentLine: Optional[float] = None
+
+    @classmethod
+    def structure_group(cls) -> str:
+        return "results/upliftvanparticleswarmreliability/"
+
+    def get_slipcircle_output(self) -> UpliftVanSlipCircleResult:
+        """Get condensed slipcircle data"""
+        try:
+            return UpliftVanSlipCircleResult(
+                x_left=self.LeftCenter.X,
+                z_left=self.LeftCenter.Z,
+                x_right=self.RightCenter.X,
+                z_right=self.RightCenter.Z,
+                z_tangent=self.TangentLine,
+            )
+        except (ValidationError, AttributeError):
+            raise ValueError(
+                f"Slipcircle not available for {self.__class__.__name__} with id {self.Id}"
+            )
+
+
 class UpliftVanResult(DStabilitySubStructure):
     FactorOfSafety: Optional[float] = None
     Id: Optional[str] = None
     LeftCenter: Optional[PersistablePoint] = None
     Points: Optional[List[Optional[PersistablePoint]]] = None
     RightCenter: Optional[PersistablePoint] = None
     Slices: Optional[List[Optional[PersistableSlice]]] = None
@@ -1780,21 +1931,24 @@
             )
 
 
 DStabilityResult = Union[
     UpliftVanResult,
     UpliftVanParticleSwarmResult,
     UpliftVanReliabilityResult,
+    UpliftVanParticleSwarmReliabilityResult,
     SpencerGeneticAlgorithmResult,
     SpencerReliabilityResult,
+    SpencerGeneticAlgorithmReliabilityResult,
     SpencerResult,
     BishopBruteForceResult,
     BishopReliabilityResult,
+    BishopBruteForceReliabilityResult,
     BishopResult,
-    None
+    None,
 ]
 
 
 ###########################
 # INPUT AND OUTPUT COMBINED
 ###########################
 
@@ -1814,208 +1968,249 @@
     waternetcreatorsettings: List[WaternetCreatorSettings] = [
         WaternetCreatorSettings(Id="15")
     ]  # waternetcreatorsettings/waternetcreatorsettings_x.json
     states: List[State] = [State(Id="16")]  # states/states_x.json
     statecorrelations: List[StateCorrelation] = [
         StateCorrelation(Id="17")
     ]  # statecorrelations/statecorrelations_x.json
-    stages: List[Stage] = [
-        Stage(
-            CalculationSettingsId="20",
-            DecorationsId="12",
-            GeometryId="11",
+    scenarios: List[Scenario] = [
+        Scenario(
             Id="0",
-            Label="Stage 1",
-            LoadsId="18",
-            Notes="Default stage by GEOLib",
-            ReinforcementsId="19",
-            SoilLayersId="13",
-            StateId="16",
-            StateCorrelationsId="17",
-            WaternetCreatorSettingsId="15",
-            WaternetId="14",
+            Label="Scenario 1",
+            Notes="Default Scenario by GEOLib",
+            Stages=[
+                Stage(
+                    DecorationsId="12",
+                    GeometryId="11",
+                    Id="43",
+                    Label="Stage 1",
+                    LoadsId="18",
+                    Notes="Default stage by GEOLib",
+                    ReinforcementsId="19",
+                    SoilLayersId="13",
+                    StateId="16",
+                    StateCorrelationsId="17",
+                    WaternetCreatorSettingsId="15",
+                    WaternetId="14",
+                )
+            ],
+            Calculations=[
+                PersistableCalculation(
+                    CalculationSettingsId="20",
+                    Id="42",
+                    Label="Calculation 1",
+                    Notes="Default calculation by GEOLib",
+                )
+            ],
         )
-    ]  # stages/stage_x.json
-    soillayers: List[SoilLayerCollection] = [
-        SoilLayerCollection(Id="13")
-    ]  # soillayers/soillayers_x.json
-    soilcorrelation: SoilCorrelation = SoilCorrelation()  # soilcorrelations.json
-    soils: SoilCollection = SoilCollection()  # soils.json
-    soilvisualizations: SoilVisualisation = SoilVisualisation()  # soilvisualizations.json
-    reinforcements: List[Reinforcements] = [
-        Reinforcements(Id="19")
-    ]  # reinforcements/reinforcements_x.json
-    projectinfo: ProjectInfo = ProjectInfo()  # projectinfo.json
-    nailproperties: NailProperties = NailProperties()  # nailpropertiesforsoils.json
-    loads: List[Loads] = [Loads(Id="18")]  # loads/loads_x.json
-    decorations: List[Decorations] = [
-        Decorations(Id="12")
-    ]  # decorations/decorations_x.json
-    calculationsettings: List[CalculationSettings] = [
-        CalculationSettings(Id="20")
-    ]  # calculationsettings/calculationsettings_x.json
-    geometries: List[Geometry] = [Geometry(Id="11")]  # geometries/geometry_x.json
+    ]
+    soillayers: List[SoilLayerCollection] = [SoilLayerCollection(Id="13")]
+    soilcorrelation: SoilCorrelation = SoilCorrelation()
+    soils: SoilCollection = SoilCollection()
+    soilvisualizations: SoilVisualisation = SoilVisualisation()
+    reinforcements: List[Reinforcements] = [Reinforcements(Id="19")]
+    projectinfo: ProjectInfo = ProjectInfo()
+    nailproperties: NailProperties = NailProperties()
+    loads: List[Loads] = [Loads(Id="18")]
+    decorations: List[Decorations] = [Decorations(Id="12")]
+    calculationsettings: List[CalculationSettings] = [CalculationSettings(Id="20")]
+    geometries: List[Geometry] = [Geometry(Id="11")]
 
     # Output parts
     uplift_van_results: List[UpliftVanResult] = []
     uplift_van_particle_swarm_results: List[UpliftVanParticleSwarmResult] = []
     uplift_van_reliability_results: List[UpliftVanReliabilityResult] = []
+    uplift_van_particle_swarm_reliability_results: List[
+        UpliftVanParticleSwarmReliabilityResult
+    ] = []
+    spencer_results: List[SpencerResult] = []
     spencer_genetic_algorithm_results: List[SpencerGeneticAlgorithmResult] = []
     spencer_reliability_results: List[SpencerReliabilityResult] = []
-    spencer_results: List[SpencerResult] = []
+    spencer_genetic_algorithm_reliability_results: List[
+        SpencerGeneticAlgorithmReliabilityResult
+    ] = []
+    bishop_results: List[BishopResult] = []
     bishop_bruteforce_results: List[BishopBruteForceResult] = []
     bishop_reliability_results: List[BishopReliabilityResult] = []
-    bishop_results: List[BishopResult] = []
+    bishop_bruteforce_reliability_results: List[BishopBruteForceReliabilityResult] = []
 
     @root_validator(skip_on_failure=True, allow_reuse=True)
     def ensure_validity_foreign_keys(cls, values):
-        """TODO Include more fk relations, left for another issue."""
-        for i, stage in enumerate(values.get("stages")):
-            if stage.CalculationSettingsId != values.get("calculationsettings")[i].Id:
-                raise ValueError("CalculationSettingsIds not linked!")
-            if stage.DecorationsId != values.get("decorations")[i].Id:
-                raise ValueError("DecorationsIds not linked!")
-            if stage.GeometryId != values.get("geometries")[i].Id:
-                raise ValueError("GeometryIds not linked!")
-            if stage.LoadsId != values.get("loads")[i].Id:
-                raise ValueError("LoadsIds not linked!")
-            if stage.ReinforcementsId != values.get("reinforcements")[i].Id:
-                raise ValueError("ReinforcementsIds not linked!")
-            if stage.SoilLayersId != values.get("soillayers")[i].Id:
-                raise ValueError("SoilLayersIds not linked!")
-            if stage.StateId != values.get("states")[i].Id:
-                raise ValueError("StateIds not linked!")
-            if stage.StateCorrelationsId != values.get("statecorrelations")[i].Id:
-                raise ValueError("StateCorrelationsIds not linked!")
-            if (
-                stage.WaternetCreatorSettingsId
-                != values.get("waternetcreatorsettings")[i].Id
-            ):
-                raise ValueError("WaternetCreatorSettingsIds not linked!")
-            if stage.WaternetId != values.get("waternets")[i].Id:
-                raise ValueError("WaternetIds not linked!")
-        return values
-
-    @property
-    def stage_specific_fields(self):
-        return [
-            "waternets",
-            "waternetcreatorsettings",
-            "states",
-            "statecorrelations",
-            "stages",
-            "soillayers",
-            "reinforcements",
-            "loads",
-            "decorations",
-            "calculationsettings",
-            "geometries",
-        ]
-
-    def get_stage_specific_fields(
-        self, stage=0
-    ) -> Generator[Tuple[str, DStabilitySubStructure], None, None]:
-        """Yield stage specific fields for given stage."""
-        for fieldname in self.stage_specific_fields:
-            field = getattr(self, fieldname)
-            if len(field) > stage:
-                yield fieldname, field[stage]
-
-    def renumber_fk_fields(self, instance, mapping: Dict, unique_id: int) -> int:
-        """Replace id (foreign key) fields on instance based on a mapping and unique id."""
-        fk = ForeignKeys()
-        fkfields = fk.class_fields
-
-        def get_correct_key(key, mapping):
-            if key not in mapping:
-                nonlocal unique_id
-                mapping[key] = unique_id
-                unique_id += 1
-            return mapping[key]
-
-        for fkfield in fkfields.get(instance.__class__.__name__, []):
-            value = getattr(instance, fkfield)
-            if isinstance(value, (list, set, tuple)):
-                setattr(
-                    instance,
-                    fkfield,
-                    [get_correct_key(x, mapping) for x in value],
-                )
-            if isinstance(value, (int, float, str)):
-                setattr(instance, fkfield, get_correct_key(value, mapping))
-
-        return unique_id
-
-    def duplicate_stage(
-        self, current_stage: int, label: str, notes: str, unique_start_id: int
-    ):
-        """Duplicates an existing stage.
-        Copies the specific stage fields for a stage and renumbers all Ids,
-        taking into account foreign keys by using the same renumbering.
-        """
+        def list_has_id(values, id):
+            for entry in values:
+                if entry.Id == id:
+                    return True
+            return False
 
-        old_to_new = {}
-        for fieldname, stagefield in self.get_stage_specific_fields(current_stage):
-            newstagefield = stagefield.copy(deep=True)
-
-            # Renumber the upper class
-            unique_start_id = self.renumber_fk_fields(
-                newstagefield, old_to_new, unique_start_id
-            )
-            # Renumber all children
-            for classinstance in children(newstagefield):
-                unique_start_id = self.renumber_fk_fields(
-                    classinstance, old_to_new, unique_start_id
-                )
+        for _, scenario in enumerate(values.get("scenarios")):
+            for _, stage in enumerate(scenario.Stages):
+                if not list_has_id(values.get("decorations"), stage.DecorationsId):
+                    raise ValueError("DecorationsIds not linked!")
+                if not list_has_id(values.get("geometries"), stage.GeometryId):
+                    raise ValueError("GeometryIds not linked!")
+                if not list_has_id(values.get("loads"), stage.LoadsId):
+                    raise ValueError("LoadsIds not linked!")
+                if not list_has_id(values.get("reinforcements"), stage.ReinforcementsId):
+                    raise ValueError("ReinforcementsIds not linked!")
+                if not list_has_id(values.get("soillayers"), stage.SoilLayersId):
+                    raise ValueError("SoilLayersIds not linked!")
+                if not list_has_id(values.get("states"), stage.StateId):
+                    raise ValueError("StateIds not linked!")
+                if not list_has_id(
+                    values.get("statecorrelations"), stage.StateCorrelationsId
+                ):
+                    raise ValueError("StateCorrelationsIds not linked!")
+                if not list_has_id(
+                    values.get("waternetcreatorsettings"), stage.WaternetCreatorSettingsId
+                ):
+                    raise ValueError("WaternetCreatorSettingsIds not linked!")
+                if not list_has_id(values.get("waternets"), stage.WaternetId):
+                    raise ValueError("WaternetIds not linked!")
+            for _, calculation in enumerate(scenario.Calculations):
+                if not list_has_id(
+                    values.get("calculationsettings"), calculation.CalculationSettingsId
+                ):
+                    raise ValueError("CalculationSettingsIds not linked!")
 
-            # Update the stage with extra supplied fields
-            if fieldname == "stages":
-                newstagefield.Label = label
-                newstagefield.Notes = notes
+        return values
 
-            getattr(self, fieldname).append(newstagefield)
+    def add_default_scenario(
+        self, label: str, notes: str, unique_start_id: Optional[int] = None
+    ) -> Tuple[int, int]:
+        """Add a new default (empty) scenario to DStability."""
+        if unique_start_id is None:
+            unique_start_id = self.get_unique_id()
 
-        return len(self.stages) - 1, unique_start_id
+        scenario_id = unique_start_id + 13
 
-    def add_default_stage(
-        self, label: str, notes: str, unique_start_id=500
-    ) -> Tuple[int, int]:
-        """Add a new default (empty) stage to DStability."""
         self.waternets += [Waternet(Id=str(unique_start_id + 1))]
         self.waternetcreatorsettings += [
             WaternetCreatorSettings(Id=str(unique_start_id + 2))
         ]
         self.states += [State(Id=str(unique_start_id + 3))]
         self.statecorrelations += [StateCorrelation(Id=str(unique_start_id + 4))]
         self.soillayers += [SoilLayerCollection(Id=str(unique_start_id + 5))]
         self.soilcorrelation: SoilCorrelation = SoilCorrelation()
         self.reinforcements += [Reinforcements(Id=str(unique_start_id + 6))]
         self.loads += [Loads(Id=str(unique_start_id + 7))]
         self.decorations += [Decorations(Id=str(unique_start_id + 9))]
         self.calculationsettings += [CalculationSettings(Id=str(unique_start_id + 10))]
         self.geometries += [Geometry(Id=str(unique_start_id + 8))]
-        self.stages += [
-            Stage(
-                CalculationSettingsId=str(unique_start_id + 10),
-                DecorationsId=str(unique_start_id + 9),
-                GeometryId=str(unique_start_id + 8),
-                Id=str(unique_start_id),
+        self.scenarios += [
+            Scenario(
+                Id=str(scenario_id),
                 Label=label,
-                LoadsId=str(unique_start_id + 7),
                 Notes=notes,
-                ReinforcementsId=str(unique_start_id + 6),
-                SoilLayersId=str(unique_start_id + 5),
-                StateId=str(unique_start_id + 3),
-                StateCorrelationsId=str(unique_start_id + 4),
-                WaternetCreatorSettingsId=str(unique_start_id + 2),
-                WaternetId=str(unique_start_id + 1),
+                Stages=[
+                    Stage(
+                        Id=str(unique_start_id + 11),
+                        Label="Stage 1",
+                        Notes="",
+                        DecorationsId=str(unique_start_id + 9),
+                        GeometryId=str(unique_start_id + 8),
+                        LoadsId=str(unique_start_id + 7),
+                        ReinforcementsId=str(unique_start_id + 6),
+                        SoilLayersId=str(unique_start_id + 5),
+                        StateId=str(unique_start_id + 3),
+                        StateCorrelationsId=str(unique_start_id + 4),
+                        WaternetCreatorSettingsId=str(unique_start_id + 2),
+                        WaternetId=str(unique_start_id + 1),
+                    )
+                ],
+                Calculations=[
+                    PersistableCalculation(
+                        Id=str(unique_start_id + 12),
+                        Label="Calculation 1",
+                        Notes="",
+                        CalculationSettingsId=str(unique_start_id + 10),
+                    )
+                ],
             )
         ]
 
-        return len(self.stages) - 1, unique_start_id + 11
+        return len(self.scenarios) - 1, scenario_id
+
+    def add_default_stage(
+        self,
+        scenario_index: int,
+        label: str,
+        notes: str,
+        unique_start_id: Optional[int] = None,
+    ) -> Tuple[int, int]:
+        """Add a new default (empty) stage to DStability."""
+        if unique_start_id is None:
+            unique_start_id = self.get_unique_id()
+
+        stage_id = unique_start_id + 13
+
+        self.waternets += [Waternet(Id=str(unique_start_id + 1))]
+        self.waternetcreatorsettings += [
+            WaternetCreatorSettings(Id=str(unique_start_id + 2))
+        ]
+        self.states += [State(Id=str(unique_start_id + 3))]
+        self.statecorrelations += [StateCorrelation(Id=str(unique_start_id + 4))]
+        self.soillayers += [SoilLayerCollection(Id=str(unique_start_id + 5))]
+        self.soilcorrelation: SoilCorrelation = SoilCorrelation()
+        self.reinforcements += [Reinforcements(Id=str(unique_start_id + 6))]
+        self.loads += [Loads(Id=str(unique_start_id + 7))]
+        self.decorations += [Decorations(Id=str(unique_start_id + 9))]
+        self.geometries += [Geometry(Id=str(unique_start_id + 8))]
+
+        new_stage = Stage(
+            Id=str(stage_id),
+            Label=label,
+            Notes=notes,
+            DecorationsId=str(unique_start_id + 9),
+            GeometryId=str(unique_start_id + 8),
+            LoadsId=str(unique_start_id + 7),
+            ReinforcementsId=str(unique_start_id + 6),
+            SoilLayersId=str(unique_start_id + 5),
+            StateId=str(unique_start_id + 3),
+            StateCorrelationsId=str(unique_start_id + 4),
+            WaternetCreatorSettingsId=str(unique_start_id + 2),
+            WaternetId=str(unique_start_id + 1),
+        )
+
+        scenario = self.scenarios[scenario_index]
+
+        if scenario.Stages is None:
+            scenario.Stages = []
+
+        scenario.Stages.append(new_stage)
+        return len(scenario.Stages) - 1, stage_id
+
+    def add_default_calculation(
+        self,
+        scenario_index: int,
+        label: str,
+        notes: str,
+        unique_start_id: Optional[int] = None,
+    ) -> Tuple[int, int]:
+        """Add a new default (empty) calculation to DStability."""
+        if unique_start_id is None:
+            unique_start_id = self.get_unique_id()
+
+        calculation_id = unique_start_id + 13
+
+        self.calculationsettings += [CalculationSettings(Id=str(unique_start_id + 1))]
+
+        new_calculation = PersistableCalculation(
+            Id=str(calculation_id),
+            Label=label,
+            Notes=notes,
+            CalculationSettingsId=str(unique_start_id + 1),
+        )
+
+        scenario = self.scenarios[scenario_index]
+
+        if scenario.Calculations is None:
+            scenario.Calculations = []
+
+        scenario.Calculations.append(new_calculation)
+        return len(scenario.Calculations) - 1, calculation_id
 
     def get_unique_id(self) -> int:
         """Return unique id that can be used in DStability.
         Finds all existing ids, takes the max and does +1.
         """
 
         fk = ForeignKeys()
@@ -2032,89 +2227,156 @@
 
         new_id = max({int(id) for id in ids if id is not None}) + 1
         return new_id
 
     def validator(self):
         return DStabilityValidator(self)
 
-    def has_stage(self, stage_id: int) -> bool:
+    def has_stage(self, scenario_index: int, stage_index: int) -> bool:
         try:
-            self.stages[stage_id]
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Stages is None:
+                return False
+
+            scenario.Stages[stage_index]
+            return True
+        except IndexError:
+            return False
+
+    def has_calculation(self, scenario_index: int, calculation_index: int) -> bool:
+        try:
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Calculations is None:
+                return False
+
+            scenario.Calculations[calculation_index]
             return True
         except IndexError:
             return False
 
-    def has_result(self, stage_id: int) -> bool:
-        if self.has_stage(stage_id):
-            result_id = self.stages[stage_id].ResultId
+    def has_scenario(self, scenario_index: int) -> bool:
+        try:
+            self.scenarios[scenario_index]
+            return True
+        except IndexError:
+            return False
+
+    def has_result(self, scenario_index: int, calculation_index: int) -> bool:
+        if self.has_calculation(scenario_index, calculation_index):
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Calculations is None:
+                return False
+
+            result_id = scenario.Calculations[calculation_index].ResultId
             if result_id is None:
                 return False
             else:
                 return True
         return False
 
-    def has_loads(self, stage_id: int) -> bool:
-        if self.has_stage(stage_id):
-            loads_id = self.stages[stage_id].LoadsId
+    def has_loads(self, scenario_index: int, stage_index: int) -> bool:
+        if self.has_stage(scenario_index, stage_index):
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Stages is None:
+                return False
+
+            loads_id = scenario.Stages[stage_index].LoadsId
             if loads_id is None:
                 return False
             else:
                 return True
         return False
 
-    def has_soil_layers(self, stage_id: int) -> bool:
-        if self.has_stage(stage_id):
-            soil_layers_id = self.stages[stage_id].SoilLayersId
+    def has_soil_layers(self, scenario_index: int, stage_index: int) -> bool:
+        if self.has_stage(scenario_index, stage_index):
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Stages is None:
+                return False
+
+            soil_layers_id = scenario.Stages[stage_index].SoilLayersId
             if soil_layers_id is None:
                 return False
             else:
                 return True
         return False
 
-    def has_soil_layer(self, stage_id: int, soil_layer_id: int) -> bool:
-        if self.has_soil_layers(stage_id):
-            for layer in self.soillayers[stage_id].SoilLayers:
+    def has_soil_layer(
+        self, scenario_index: int, stage_index: int, soil_layer_id: int
+    ) -> bool:
+        if self.has_soil_layers(scenario_index, stage_index):
+            for layer in self.soillayers[stage_index].SoilLayers:
                 if str(soil_layer_id) == layer.LayerId:
                     return True
             return False
         return False
 
-    def has_reinforcements(self, stage_id: int) -> bool:
-        if self.has_stage(stage_id):
-            reinforcements_id = self.stages[stage_id].ReinforcementsId
+    def has_reinforcements(self, scenario_index: int, stage_index: int) -> bool:
+        if self.has_stage(scenario_index, stage_index):
+            scenario = self.scenarios[scenario_index]
+
+            if scenario.Stages is None:
+                return False
+
+            reinforcements_id = scenario.Stages[stage_index].ReinforcementsId
             if reinforcements_id is None:
                 return False
             else:
                 return True
         return False
 
+    def _get_soil_layers(self, scenario_index: int, stage_index: int):
+        soil_layers_id = self.scenarios[scenario_index].Stages[stage_index].SoilLayersId
+
+        for soil_layers in self.soillayers:
+            if soil_layers.Id == soil_layers_id:
+                return soil_layers
+
+        raise ValueError(
+            f"No soil layers found for stage {stage_index} in scenario {scenario_index}."
+        )
+
+    def _get_loads(self, scenario_index: int, stage_index: int):
+        loads_id = self.scenarios[scenario_index].Stages[stage_index].LoadsId
+
+        for loads in self.loads:
+            if loads.Id == loads_id:
+                return loads
+
+        raise ValueError(
+            f"No loads found for stage {stage_index} in scenario {scenario_index}."
+        )
+
     def get_result_substructure(
         self, analysis_type: AnalysisTypeEnum, calculation_type: CalculationTypeEnum
     ) -> List[DStabilityResult]:
-
         result_types_mapping = {
             AnalysisTypeEnum.UPLIFT_VAN: {
                 "non_probabilistic": self.uplift_van_results,
                 "probabilistic": self.uplift_van_reliability_results,
             },
             AnalysisTypeEnum.UPLIFT_VAN_PARTICLE_SWARM: {
                 "non_probabilistic": self.uplift_van_particle_swarm_results,
-                "probabilistic": self.uplift_van_reliability_results,
+                "probabilistic": self.uplift_van_particle_swarm_reliability_results,
             },
             AnalysisTypeEnum.SPENCER_GENETIC: {
                 "non_probabilistic": self.spencer_genetic_algorithm_results,
-                "probabilistic": self.spencer_reliability_results,
+                "probabilistic": self.spencer_genetic_algorithm_reliability_results,
             },
             AnalysisTypeEnum.SPENCER: {
                 "non_probabilistic": self.spencer_results,
                 "probabilistic": self.spencer_reliability_results,
             },
             AnalysisTypeEnum.BISHOP_BRUTE_FORCE: {
                 "non_probabilistic": self.bishop_bruteforce_results,
-                "probabilistic": self.bishop_reliability_results,
+                "probabilistic": self.bishop_bruteforce_reliability_results,
             },
             AnalysisTypeEnum.BISHOP: {
                 "non_probabilistic": self.bishop_results,
                 "probabilistic": self.bishop_reliability_results,
             },
         }
 
@@ -2138,37 +2400,37 @@
         ),
         "PersistableReferenceLine.Id": ("Waternet.PhreaticLineId",),
         "PersistableLayer.Id": (
             "PersistableStatePoint.LayerId",
             "PersistableSoilLayer.LayerId",
             "PersistableConsolidation.LayerId",
             "PersistableLayerLoad.LayerId",
-            "PersistableBerm.AddedLayerId",
+            "PersistableElevation.AddedLayerId",
             "WaternetCreatorSettings.AquiferInsideAquitardLayerId",
             "WaternetCreatorSettings.AquiferLayerId",
         ),
         # Soil commented out for now, isn't used in stages
         # "PersistableSoil.Id": (
         #     "PersistableSoilVisualization.SoilId",
         #     "PersistableSoilLayer.SoilId",
         #     "PersistableSoilCorrelation.CorrelatedSoilIds",
         #     "PersistableNailPropertiesForSoil.SoilId",
         #     "PersistableSoilContribution.SoilId"
         # ),
-        "CalculationSettings.Id": ("Stage.CalculationSettingsId",),
+        "CalculationSettings.Id": ("Calculation.CalculationSettingsId",),
         "Decorations.Id": ("Stage.DecorationsId",),
         "Geometry.Id": ("Stage.GeometryId",),
         "Loads.Id": ("Stage.LoadsId",),
         "Reinforcements.Id": ("Stage.ReinforcementsId",),
-        "Result.Id": ("Stage.ResultId",),
+        "Result.Id": ("Calculation.ResultId",),
         "SoilLayerCollection.Id": ("Stage.SoilLayersId",),
         "StateCorrelation.Id": ("Stage.StateCorrelationsId",),
         "State.Id": ("Stage.StateId",),
         "WaternetCreatorSettings.Id": ("Stage.WaternetCreatorSettingsId",),
-        "Stage.Id": ("PersistableStageContribution.StageId",),
+        "Calculation.Id": ("PersistableCalculationContribution.CalculationId",),
         "PersistableStateLinePoint.Id": (
             "PersistableStateCorrelation.CorrelatedStateIds",
             "PersistableStateLinePointContribution.StateLinePointId",
         ),
         "PersistableStatePoint.Id": ("PersistableStatePointContribution.StatePointId",),
     }
```

### Comparing `d_geolib-0.6.0/geolib/models/dstability/loads.py` & `d_geolib-1.0.0/geolib/models/dstability/loads.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dstability/reinforcements.py` & `d_geolib-1.0.0/geolib/models/dstability/reinforcements.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dstability/serializer.py` & `d_geolib-1.0.0/geolib/models/dstability/serializer.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
 
 
 class DStabilityInputSerializer(DStabilityBaseSerializer):
     def write(self, filepath: DirectoryPath) -> DirectoryPath:
         serialized_datastructure = self.serialize()
 
         for filename, data in serialized_datastructure.items():
-
             if isinstance(data, dict):
                 folder = filepath / filename
                 folder.mkdir(parents=True, exist_ok=True)
 
                 for ffilename, fdata in data.items():
                     fn = folder / ffilename
                     with fn.open("wb") as io:
@@ -75,15 +74,14 @@
     """DStabilSerializer for zipped.stix files."""
 
     def write(self, filepath: Union[FilePath, BytesIO]) -> Union[FilePath, BytesIO]:
         with ZipFile(filepath, mode="w", compression=ZIP_DEFLATED) as zip:
             serialized_datastructure = self.serialize()
 
             for filename, data in serialized_datastructure.items():
-
                 if isinstance(data, dict):
                     folder = filename
                     for ffilename, fdata in data.items():
                         fn = folder + "/" + ffilename
                         with zip.open(fn, "w") as io:
                             io.write(fdata.encode("utf-8"))
                 else:
```

### Comparing `d_geolib-0.6.0/geolib/models/dstability/states.py` & `d_geolib-1.0.0/geolib/models/dstability/states.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/dstability/utils.py` & `d_geolib-1.0.0/geolib/models/dstability/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/meta.py` & `d_geolib-1.0.0/geolib/models/meta.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/parsers.py` & `d_geolib-1.0.0/geolib/models/parsers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/serializers.py` & `d_geolib-1.0.0/geolib/models/serializers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/models/utils.py` & `d_geolib-1.0.0/geolib/models/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/service/main.py` & `d_geolib-1.0.0/geolib/service/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 
 @app.get("/users/me")
 def read_current_user(username: str = Depends(get_current_username)):
     return {"username": username}
 
 
-@app.get("/")
+@app.get("/", response_model=False)
 async def root():
     return {"message": "Hello World"}
 
 
 def cleanup(path: Path):
     print(f"Cleaning up {path}")
     shutil.rmtree(path)
@@ -78,78 +78,78 @@
         )
     else:
         return output
     finally:
         background_tasks.add_task(cleanup, unique_folder)
 
 
-@app.post("/calculate/dsettlementmodel")
+@app.post("/calculate/dsettlementmodel", response_model=None)
 async def calculate_dsettlementmodel(
     model: DSettlementModel,
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> DSettlementModel:
     return execute(model, background_tasks)
 
 
-@app.post("/calculate/dfoundationsmodel")
+@app.post("/calculate/dfoundationsmodel", response_model=None)
 async def calculate_dfoundationsmodel(
     model: DFoundationsModel,
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> DFoundationsModel:
     return execute(model, background_tasks)
 
 
-@app.post("/calculate/dsheetpilingmodel")
+@app.post("/calculate/dsheetpilingmodel", response_model=None)
 async def calculate_dsheetpilingmodel(
     model: DSheetPilingModel,
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> DSheetPilingModel:
     return execute(model, background_tasks)
 
 
-@app.post("/calculate/dstabilitymodel")
+@app.post("/calculate/dstabilitymodel", response_model=None)
 async def calculate_dstabilitymodel(
     model: DStabilityModel,
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> DStabilityModel:
     return execute(model, background_tasks)
 
 
-@app.post("/calculate/dsettlementmodels")
+@app.post("/calculate/dsettlementmodels", response_model=None)
 async def calculate_many_dsettlementmodels(
     models: conlist(DSettlementModel, min_items=1),
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> List[DSettlementModel]:
     return execute_many(models, background_tasks)
 
 
-@app.post("/calculate/dfoundationsmodels")
+@app.post("/calculate/dfoundationsmodels", response_model=None)
 async def calculate_many_dfoundationsmodel(
     models: conlist(DFoundationsModel, min_items=1),
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> List[DFoundationsModel]:
     return execute_many(models, background_tasks)
 
 
-@app.post("/calculate/dsheetpilingmodels")
+@app.post("/calculate/dsheetpilingmodels", response_model=None)
 async def calculate_many_dsheetpilingmodel(
     models: conlist(DSheetPilingModel, min_items=1),
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> List[DSheetPilingModel]:
     return execute_many(models, background_tasks)
 
 
-@app.post("/calculate/dstabilitymodels")
+@app.post("/calculate/dstabilitymodels", response_model=None)
 async def calculate_many_dstabilitymodel(
     models: conlist(DStabilityModel, min_items=1),
     background_tasks: BackgroundTasks,
     _: str = Depends(get_current_username),
 ) -> List[DStabilityModel]:
     return execute_many(models, background_tasks)
```

### Comparing `d_geolib-0.6.0/geolib/service/README.md` & `d_geolib-1.0.0/geolib/service/README.md`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/soils/__init__.py` & `d_geolib-1.0.0/geolib/soils/__init__.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/soils/layers.py` & `d_geolib-1.0.0/geolib/soils/layers.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/soils/library.py` & `d_geolib-1.0.0/geolib/soils/library.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/soils/soil.py` & `d_geolib-1.0.0/geolib/soils/soil.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
     def transform_shear_strength_model_type_to_internal(self):
         from geolib.models.dstability.internal import (
             ShearStrengthModelTypePhreaticLevelInternal,
         )
 
         transformation_dict = {
-            "Mohr_Coulomb": ShearStrengthModelTypePhreaticLevelInternal.C_PHI,
+            "Mohr_Coulomb": ShearStrengthModelTypePhreaticLevelInternal.MOHR_COULOMB_ADVANCED,
             "None": ShearStrengthModelTypePhreaticLevelInternal.NONE,
             "SHANSEP": ShearStrengthModelTypePhreaticLevelInternal.SU,
             "SuTable": ShearStrengthModelTypePhreaticLevelInternal.SUTABLE,
         }
         return transformation_dict[self.value]
 
 
@@ -73,15 +73,17 @@
     """
     Mohr Coulomb parameters class
     """
 
     cohesion: Optional[Union[float, StochasticParameter]] = StochasticParameter()
     dilatancy_angle: Optional[Union[float, StochasticParameter]] = StochasticParameter()
     friction_angle: Optional[Union[float, StochasticParameter]] = StochasticParameter()
-    friction_angle_interface: Optional[Union[float, StochasticParameter]] = StochasticParameter()
+    friction_angle_interface: Optional[
+        Union[float, StochasticParameter]
+    ] = StochasticParameter()
     is_delta_angle_automatically_calculated: Optional[bool] = None
     cohesion_and_friction_angle_correlated: Optional[bool] = None
 
 
 class SuTablePoint(SoilBaseModel):
     su: float = None
     stress: float = None
@@ -373,14 +375,15 @@
     LOAM = 2
     CLAY = 3
     PEAT = 4
     SANDY_LOAM = 5
     TERTCLAY = 6
     CLAYEYSAND = 7
 
+
 class Soil(SoilBaseModel):
     """Soil Material."""
 
     id: Optional[str] = None
     name: Optional[str] = None
     code: Optional[str] = None
     color: Color = Color("grey")
@@ -455,30 +458,32 @@
 
         Returns:
 
         """
         for field in self.__fields__:
             self.set_stochastic_parameters(self.__getattribute__(field))
 
-    @staticmethod
-    def __transfer_soil_dict_to_model(soil_dict, model_soil):
+    def __transfer_soil_dict_to_model(self, soil_dict, model_soil):
         """
         Transfers items from soil dictionary to model if the item is not None
         Args:
             soil_dict: soil dictionary
             model_soil: internal soil in model
 
         Returns:
 
         """
         for key, value in dict(
             soil_dict
         ).items():  # override default values with those of the soil
             if key in dict(model_soil).keys() and value is not None:
-                setattr(model_soil, key, value)
+                if type(value) is dict:
+                    self.__transfer_soil_dict_to_model(value, getattr(model_soil, key))
+                else:
+                    setattr(model_soil, key, value)
         return model_soil
 
     def __to_dstability_stochastic_parameter(
         self, stochastic_parameter: StochasticParameter
     ):
         from geolib.models.dstability.internal import (
             PersistableStochasticParameter as DStabilityStochasticParameter,
@@ -528,36 +533,40 @@
                 self.shear_strength_model_below_phreatic_level
             )
 
         kwargs = {
             "Id": self.id,
             "Name": self.name,
             "Code": self.code,
-            "Cohesion": self.mohr_coulomb_parameters.cohesion.mean,
-            "CohesionStochasticParameter": self.__to_dstability_stochastic_parameter(
-                self.mohr_coulomb_parameters.cohesion
-            ),
-            "FrictionAngle": self.mohr_coulomb_parameters.friction_angle.mean,
-            "FrictionAngleStochasticParameter": self.__to_dstability_stochastic_parameter(
-                self.mohr_coulomb_parameters.friction_angle
-            ),
-            "CohesionAndFrictionAngleCorrelated": self.mohr_coulomb_parameters.cohesion_and_friction_angle_correlated,
-            "Dilatancy": self.mohr_coulomb_parameters.dilatancy_angle.mean,
-            "DilatancyStochasticParameter": self.__to_dstability_stochastic_parameter(
-                self.mohr_coulomb_parameters.dilatancy_angle
-            ),
-            "ShearStrengthRatio": self.undrained_parameters.shear_strength_ratio.mean,
-            "ShearStrengthRatioStochasticParameter": self.__to_dstability_stochastic_parameter(
-                self.undrained_parameters.shear_strength_ratio
-            ),
-            "StrengthIncreaseExponent": self.undrained_parameters.strength_increase_exponent.mean,
-            "StrengthIncreaseExponentStochasticParameter": self.__to_dstability_stochastic_parameter(
-                self.undrained_parameters.strength_increase_exponent
-            ),
-            "ShearStrengthRatioAndShearStrengthExponentCorrelated": self.undrained_parameters.shear_strength_ratio_and_shear_strength_exponent_correlated,
+            "MohrCoulombAdvancedShearStrengthModel": {
+                "Cohesion": self.mohr_coulomb_parameters.cohesion.mean,
+                "CohesionStochasticParameter": self.__to_dstability_stochastic_parameter(
+                    self.mohr_coulomb_parameters.cohesion
+                ),
+                "FrictionAngle": self.mohr_coulomb_parameters.friction_angle.mean,
+                "FrictionAngleStochasticParameter": self.__to_dstability_stochastic_parameter(
+                    self.mohr_coulomb_parameters.friction_angle
+                ),
+                "CohesionAndFrictionAngleCorrelated": self.mohr_coulomb_parameters.cohesion_and_friction_angle_correlated,
+                "Dilatancy": self.mohr_coulomb_parameters.dilatancy_angle.mean,
+                "DilatancyStochasticParameter": self.__to_dstability_stochastic_parameter(
+                    self.mohr_coulomb_parameters.dilatancy_angle
+                ),
+            },
+            "ShansepShearStrengthModel": {
+                "ShearStrengthRatio": self.undrained_parameters.shear_strength_ratio.mean,
+                "ShearStrengthRatioStochasticParameter": self.__to_dstability_stochastic_parameter(
+                    self.undrained_parameters.shear_strength_ratio
+                ),
+                "StrengthIncreaseExponent": self.undrained_parameters.strength_increase_exponent.mean,
+                "StrengthIncreaseExponentStochasticParameter": self.__to_dstability_stochastic_parameter(
+                    self.undrained_parameters.strength_increase_exponent
+                ),
+                "ShearStrengthRatioAndShearStrengthExponentCorrelated": self.undrained_parameters.shear_strength_ratio_and_shear_strength_exponent_correlated,
+            },
             "VolumetricWeightAbovePhreaticLevel": self.soil_weight_parameters.unsaturated_weight.mean,
             "VolumetricWeightBelowPhreaticLevel": self.soil_weight_parameters.saturated_weight.mean,
             "IsProbabilistic": self.is_probabilistic,
             "ShearStrengthModelTypeAbovePhreaticLevel": shear_strength_model_above_phreatic_level,
             "ShearStrengthModelTypeBelowPhreaticLevel": shear_strength_model_below_phreatic_level,
             "SuTable": self.__to_su_table(),
         }
```

### Comparing `d_geolib-0.6.0/geolib/soils/soil_utils.py` & `d_geolib-1.0.0/geolib/soils/soil_utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/geolib/utils.py` & `d_geolib-1.0.0/geolib/utils.py`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/LICENSE` & `d_geolib-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/pyproject.toml` & `d_geolib-1.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,51 @@
 [tool.poetry]
 name = "d-geolib"
-version = "0.6.0"
+version = "1.0.0"
 description = "Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models"
 authors = ["Maarten Pronk <maarten.pronk@deltares.nl>", "Deltares"]
 license = "MIT"
 homepage = "https://deltares.github.io/GEOLib/"
 documentation = "https://deltares.github.io/GEOLib/"
 repository = "https://github.com/Deltares/GEOLib"
 readme = "README.rst"
 packages = [
     {include = "geolib"}
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
-pydantic = {version = "^1.6.1", extras = ["dotenv"]}
-zipp = "^3.11.0"
-fastapi = {version = "^0.88.0", optional = true}
-uvicorn = {version = "^0.20.0", optional = true}
-requests = "^2.28.1"
+python = ">=3.8.1,<4.0.0"
+pydantic = {version = "^1.10.7", extras = ["dotenv"]}
+zipp = "^3.15.0"
+fastapi = {version = "^0.95.1", optional = true}
+uvicorn = {version = "^0.21.1", optional = true}
+requests = "^2.29.0"
 jinja2 = "^3.1.2"
-httpx = {version = "^0.23.1", optional = true}
+httpx = {version = "^0.24.0", optional = true}
+starlette = "^0.26.1"
 
 [tool.poetry.group.dev.dependencies]
 teamcity-messages = "^1.32"
-flake8 = "^5.0.4"
-black = ">=22.8.0,<22.10.0"
-devtools = "^0.10.0"
-pytest = "^7.2.1"
+flake8 = "^6.0.0"
+black = "^23.3.0"
+devtools = "^0.11.0"
+pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
-mypy = "^0.991"
-sphinx = "^4.3.2"
+mypy = "^1.2.0"
+sphinx = "^7.0.1"
 recommonmark = "^0.7.1"
-sphinx-autodoc-typehints = "^1.17.1"
-releases = "^1.6.3"
+sphinx-autodoc-typehints = "^1.23.0"
+releases = "^2.1.0"
 sphinx-multiversion = "^0.2.4"
-isort = "^5.11.4"
-commitizen = "^2.40.0"
-tomlkit = "^0.11.6"
+isort = "^5.12.0"
+commitizen = "^3.1.0"
+tomlkit = "^0.11.8"
 
 [tool.poetry.extras]
-server = ["fastapi", "uvicorn", "httpx"]
+server = ["fastapi", "uvicorn", "httpx", "starlette"]
 
 [tool.poetry.scripts]
 geolib_server = "geolib.service.main:app"
 
 [tool.black]
 line-length = 90
 target-version = ['py37']
@@ -66,15 +67,15 @@
 force_grid_wrap=0
 use_parentheses=true
 line_length=90
 profile = "black"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.6.0"
+version = "1.0.0"
 tag_format = "v$major.$minor.$patch$prerelease"
 version_files = [
     "pyproject.toml:^version",
     "tests/test_geolib.py",
     "geolib/__init__.py:__version__",
 ]
 annotated_tag = true
```

### Comparing `d_geolib-0.6.0/README.rst` & `d_geolib-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `d_geolib-0.6.0/PKG-INFO` & `d_geolib-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 Metadata-Version: 2.1
 Name: d-geolib
-Version: 0.6.0
+Version: 1.0.0
 Summary: Python wrappers around the input and output files of the Deltares D-Serie and D-GEO Suite models
 Home-page: https://deltares.github.io/GEOLib/
 License: MIT
 Author: Maarten Pronk
 Author-email: maarten.pronk@deltares.nl
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: server
-Requires-Dist: fastapi (>=0.88.0,<0.89.0) ; extra == "server"
-Requires-Dist: httpx (>=0.23.1,<0.24.0) ; extra == "server"
+Requires-Dist: fastapi (>=0.95.1,<0.96.0) ; extra == "server"
+Requires-Dist: httpx (>=0.24.0,<0.25.0) ; extra == "server"
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
-Requires-Dist: pydantic[dotenv] (>=1.6.1,<2.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "server"
-Requires-Dist: zipp (>=3.11.0,<4.0.0)
+Requires-Dist: pydantic[dotenv] (>=1.10.7,<2.0.0)
+Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: starlette (>=0.26.1,<0.27.0) ; extra == "server"
+Requires-Dist: uvicorn (>=0.21.1,<0.22.0) ; extra == "server"
+Requires-Dist: zipp (>=3.15.0,<4.0.0)
 Project-URL: Documentation, https://deltares.github.io/GEOLib/
 Project-URL: Repository, https://github.com/Deltares/GEOLib
 Description-Content-Type: text/x-rst
 
 GEOLib
 =============================
```

