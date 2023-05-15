# Comparing `tmp/oaklib-0.5.5.tar.gz` & `tmp/oaklib-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.5.tar", max compression
+gzip compressed data, was "oaklib-0.5.6.tar", max compression
```

## Comparing `oaklib-0.5.5.tar` & `oaklib-0.5.6.tar`

### file list

```diff
@@ -1,269 +1,269 @@
--rw-r--r--   0        0        0    11357 2023-05-11 19:01:04.647427 oaklib-0.5.5/LICENSE
--rw-r--r--   0        0        0     7241 2023-05-11 19:01:04.647427 oaklib-0.5.5/README.md
--rw-r--r--   0        0        0     1883 2023-05-11 19:01:53.195605 oaklib-0.5.5/pyproject.toml
--rw-r--r--   0        0        0      271 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/__init__.py
--rw-r--r--   0        0        0   193630 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12159 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5155 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    36266 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    11740 2023-05-11 19:01:04.779427 oaklib-0.5.5/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13328 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14564 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15768 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    45533 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    17625 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-05-11 19:01:04.783427 oaklib-0.5.5/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5614 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5602 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5996 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0     4563 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2179 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1053 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30434 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16240 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2532 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1238 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35620 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/rustsim/__init__.py
--rw-r--r--   0        0        0    14065 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/rustsim/rustsim_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.787427 oaklib-0.5.5/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34382 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   106362 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    20557 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8830 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      977 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13681 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    18964 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     2638 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2087 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7906 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1524 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-05-11 19:01:04.791427 oaklib-0.5.5/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2208 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1130 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1432 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8084 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/resource.py
--rw-r--r--   0        0        0    14739 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3419 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1540 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14443 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22274 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-05-11 19:01:04.795427 oaklib-0.5.5/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8871 1970-01-01 00:00:00.000000 oaklib-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-15 15:52:40.563784 oaklib-0.5.6/LICENSE
+-rw-r--r--   0        0        0     7241 2023-05-15 15:52:40.563784 oaklib-0.5.6/README.md
+-rw-r--r--   0        0        0     1883 2023-05-15 15:53:30.576518 oaklib-0.5.6/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   193630 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5793 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    36266 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    11740 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-05-15 15:52:40.687786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    46876 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    18191 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5614 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5623 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5996 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     4563 2023-05-15 15:52:40.691786 oaklib-0.5.6/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30434 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16240 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2532 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35620 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0    14075 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34382 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   106362 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    20557 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8830 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-05-15 15:52:40.695786 oaklib-0.5.6/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      977 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13681 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    18964 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     2638 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2087 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7906 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1524 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2208 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1130 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1432 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8084 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3419 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14467 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22274 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-05-15 15:52:40.699786 oaklib-0.5.6/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-05-15 15:52:40.703786 oaklib-0.5.6/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8867 1970-01-01 00:00:00.000000 oaklib-0.5.6/PKG-INFO
```

### Comparing `oaklib-0.5.5/LICENSE` & `oaklib-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/README.md` & `oaklib-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/pyproject.toml` & `oaklib-0.5.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.5"
+version = "v0.5.6"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -16,32 +16,32 @@
 networkx = ">=2.7.1"
 sssom-schema = ">=0.11.0"
 sssom = ">=0.3.26"
 ratelimit = ">=2.2.1"
 appdirs = ">=1.4.4"
 semsql = ">=0.3.1"
 lark = ">=1.1.2"
-kgcl-schema = ">=0.3.5"
+kgcl-schema = "0.5.0"
 funowl = ">=0.1.12"
 gilda = {version = "^0.10.1", optional = true}
-kgcl-rdflib = "^0.3.0"
+kgcl-rdflib = "0.5.0"
 pystow = ">=0.5.0"
 class-resolver = ">=0.4.2"
 ontoportal-client = ">=0.0.3"
 bioregistry = ">=0.6.35"
 prefixmaps = ">=0.1.2"
 ols-client = ">=0.1.1"
 linkml-renderer = ">=0.1.2"
 airium = ">=0.2.5"
 ndex2 = "^3.5.0"
-rustsim = ">=0.1.6"
 pysolr = "^3.9.0"
 eutils = ">=0.6.0"
 requests-cache = "^1.0.1"
 click = "*"
+semsimian = ">=0.1.13"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 pandas = ">=1.5.1"
 jupyter = ">=1.0.0"
 sphinx-rtd-theme = "^1.0.0"
```

### Comparing `oaklib-0.5.5/src/oaklib/cli.py` & `oaklib-0.5.6/src/oaklib/cli.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.6/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.6/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.6/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.6/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.6/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.6/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from oaklib.datamodels.obograph import (
     RDF,
     Edge,
     Graph,
     GraphDocument,
     Meta,
     Node,
+    PropertyTypeEnum,
     PropertyValue,
 )
 from oaklib.datamodels.vocabulary import (
     HAS_BROAD_SYNONYM,
     HAS_DBXREF,
     HAS_DEFINITION_URI,
     HAS_EXACT_SYNONYM,
@@ -85,14 +86,25 @@
             self._convert_edge(e, target=target)
         return target
 
     def _convert_node(self, source: Node, target: rdflib.Graph) -> rdflib.Graph:
         uri = self._uri_ref(source.id)
         if not source.type or source.type == "CLASS":
             target.add((uri, RDF.type, OWL.Class))
+        elif source.type == "PROPERTY":
+            if source.propertyType == PropertyTypeEnum.OBJECT:
+                target.add((uri, RDF.type, OWL.ObjectProperty))
+            elif source.propertyType == PropertyTypeEnum.ANNOTATION:
+                target.add((uri, RDF.type, OWL.AnnotationProperty))
+            elif source.propertyType == PropertyTypeEnum.DATA:
+                target.add((uri, RDF.type, OWL.DatatypeProperty))
+        elif source.type == "INDIVIDUAL":
+            target.add((uri, RDF.type, OWL.NamedIndividual))
+        else:
+            raise ValueError(f"Unknown node type: {source.type}")
         if source.lbl:
             target.add((uri, RDFS.label, rdflib.Literal(source.lbl)))
         if source.meta:
             self._convert_meta(uri, source.meta, target=target)
         return target
 
     def _convert_meta(self, uri: rdflib.URIRef, source: Meta, target: rdflib.Graph) -> rdflib.Graph:
```

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/association.py` & `oaklib-0.5.6/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/cx.py` & `oaklib-0.5.6/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.6/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.6/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.6/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.6/src/oaklib/datamodels/obograph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from obograph.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-16T14:19:05
+# Generation date: 2023-05-03T08:52:36
 # Schema: obographs_datamodel
 #
 # id: https://github.com/geneontology/obographs
 # description: A data model for graph-oriented representations of ontologies. Each ontology is represented as a
 #              Graph, and multiple ontologies can be connected together in a GraphDocument. The principle elements
 #              of a Graph are Node objects and Edge objects. A Node represents an arbitrary ontology element,
 #              including but not limited to the core terms in the ontology. Edges represent simple relationships
@@ -326,28 +326,32 @@
     class_class_curie: ClassVar[str] = "rdf:Resource"
     class_name: ClassVar[str] = "Node"
     class_model_uri: ClassVar[URIRef] = OBOGRAPHS.Node
 
     id: Union[str, NodeId] = None
     lbl: Optional[str] = None
     type: Optional[str] = None
+    propertyType: Optional[Union[str, "PropertyTypeEnum"]] = None
     meta: Optional[Union[dict, "Meta"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NodeId):
             self.id = NodeId(self.id)
 
         if self.lbl is not None and not isinstance(self.lbl, str):
             self.lbl = str(self.lbl)
 
         if self.type is not None and not isinstance(self.type, str):
             self.type = str(self.type)
 
+        if self.propertyType is not None and not isinstance(self.propertyType, PropertyTypeEnum):
+            self.propertyType = PropertyTypeEnum(self.propertyType)
+
         if self.meta is not None and not isinstance(self.meta, Meta):
             self.meta = Meta(**as_dict(self.meta))
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
@@ -875,14 +879,44 @@
 
     _defn = EnumDefinition(
         name="ScopeEnum",
         description='A vocabulary of terms that can be used to "scope" a synonym',
     )
 
 
+class NodeTypeEnum(EnumDefinitionImpl):
+    """
+    The main type of a node
+    """
+
+    CLASS = PermissibleValue(text="CLASS", meaning=OWL.Class)
+    PROPERTY = PermissibleValue(text="PROPERTY", meaning=RDFS.Property)
+    INDIVIDUAL = PermissibleValue(text="INDIVIDUAL", meaning=OWL.NamedIndividual)
+
+    _defn = EnumDefinition(
+        name="NodeTypeEnum",
+        description="The main type of a node",
+    )
+
+
+class PropertyTypeEnum(EnumDefinitionImpl):
+    """
+    The node subtype for property nodes
+    """
+
+    ANNOTATION = PermissibleValue(text="ANNOTATION", meaning=OWL.AnnotationProperty)
+    OBJECT = PermissibleValue(text="OBJECT", meaning=OWL.ObjectProperty)
+    DATA = PermissibleValue(text="DATA", meaning=OWL.DatatypeProperty)
+
+    _defn = EnumDefinition(
+        name="PropertyTypeEnum",
+        description="The node subtype for property nodes",
+    )
+
+
 # Slots
 class slots:
     pass
 
 
 slots.id = Slot(
     uri=OBOGRAPHS.id,
@@ -961,14 +995,23 @@
     name="type",
     curie=OBOGRAPHS.curie("type"),
     model_uri=OBOGRAPHS.type,
     domain=None,
     range=Optional[str],
 )
 
+slots.propertyType = Slot(
+    uri=OBOGRAPHS.propertyType,
+    name="propertyType",
+    curie=OBOGRAPHS.curie("propertyType"),
+    model_uri=OBOGRAPHS.propertyType,
+    domain=None,
+    range=Optional[Union[str, "PropertyTypeEnum"]],
+)
+
 slots.meta = Slot(
     uri=OBOGRAPHS.meta,
     name="meta",
     curie=OBOGRAPHS.curie("meta"),
     model_uri=OBOGRAPHS.meta,
     domain=None,
     range=Optional[Union[dict, Meta]],
```

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/obograph.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -54,14 +54,32 @@
         meaning: oio:hasBroadSynonym
         description: The synonym represents something broader in meaning than the node.
       hasRelatedSynonym:
         meaning: oio:hasRelatedSynonym
         description: >-
           The synonym represents something closely related in meaning than the node,
           but in not exact, broad, or narrow.
+  NodeTypeEnum:
+    description: The main type of a node
+    permissible_values:
+      CLASS:
+        meaning: owl:Class
+      PROPERTY:
+        meaning: rdfs:Property
+      INDIVIDUAL:
+        meaning: owl:NamedIndividual
+  PropertyTypeEnum:
+    description: The node subtype for property nodes
+    permissible_values:
+      ANNOTATION:
+        meaning: owl:AnnotationProperty
+      OBJECT:
+        meaning: owl:ObjectProperty
+      DATA:
+        meaning: owl:DatatypeProperty
 
 types:
   XrefString:
     typeof: string
     description: >-
       A string that is a cross reference to another entity represented in another ontology, vocabulary, database, or
       website. The string SHOULD be a CURIE or a URL, but this standard relaxes this to a string to support
@@ -144,16 +162,19 @@
     range: string
     description: >-
       the human-readable label of a node
     slot_uri: rdfs:label
     comments:
       - the name "lbl" exists for legacy purposes, this should be considered identical to label in rdfs
   type:
-    # TODO: rdf:type not working - import problem?
+    # switch to enums when we move to pydantic
+    # range: NodeTypeEnum
     range: string
+  propertyType:
+     range: PropertyTypeEnum
   meta:
     aliases:
       - annotations
     range: Meta
     description: >-
       A collection of metadata about either an ontology (graph), an entity, or an axiom
   definition:
@@ -363,14 +384,15 @@
     description: >-
       A node is a class, property, or other entity in an ontology
     class_uri: rdf:Resource
     slots:
       - id
       - lbl
       - type
+      - propertyType
       - meta
 
   Edge:
     description: >-
       An edge is a simple typed relationship between two nodes.
       When mapping to OWL, an edge represents either (a) s SubClassOf o (b) s SubClassOf p some o (c) s p o
       (where s and o are individuals)
```

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.6/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/search.py` & `oaklib-0.5.6/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.6/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.6/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.6/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/__init__.py` & `oaklib-0.5.6/src/oaklib/implementations/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,17 @@
 from oaklib.implementations.ontoportal.matportal_implementation import (
     MatPortalImplementation,
 )
 from oaklib.implementations.ontoportal.ontoportal_implementation_base import (
     OntoPortalImplementationBase,
 )
 from oaklib.implementations.pronto.pronto_implementation import ProntoImplementation
-from oaklib.implementations.rustsim.rustsim_implementation import RustSimImplementation
+from oaklib.implementations.semsimian.semsimian_implementation import (
+    SemSimianImplementation,
+)
 from oaklib.implementations.simpleobo.simple_obo_implementation import (
     SimpleOboImplementation,
 )
 from oaklib.implementations.sparql.lov_implementation import LovImplementation
 from oaklib.implementations.sparql.oak_metamodel_implementation import (
     OakMetaModelImplementation,
 )
@@ -79,15 +81,15 @@
     "WikidataImplementation",
     "PubMedImplementation",
     "FunOwlImplementation",
     "GildaImplementation",
     "KGXImplementation",
     "TranslatorImplementation",
     "OakMetaModelImplementation",
-    "RustSimImplementation",
+    "SemSimianImplementation",
 ]
 
 
 @cache
 def get_implementation_resolver() -> ClassResolver[OntologyInterface]:
     """
     Get a class resolver for all implementations (adapters).
@@ -126,15 +128,15 @@
             "prontolib": ProntoImplementation,
             "simpleobo": SimpleOboImplementation,
             "sqlite": SqlImplementation,
             "rdflib": SparqlImplementation,
             "oak": OakMetaModelImplementation,
             "cx": CXImplementation,
             "ndexbio": CXImplementation,
-            "rustsim": RustSimImplementation,
+            "semsimian": SemSimianImplementation,
         }
     )
 
     # Plugins which want to register an implementation should use
     # the entrypoint group "oaklib.plugins". The name of the entry
     # point will be used as a possible match against the input scheme
     # prefix. The value of the entry point should be an implementation
```

### Comparing `oaklib-0.5.5/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/gilda.py` & `oaklib-0.5.6/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.6/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.6/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/rustsim/rustsim_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import logging
 import math
 import statistics
 from collections import defaultdict
 from dataclasses import dataclass
 from typing import ClassVar, Iterable, Iterator, List, Optional, Tuple, Union
 
-from rustsim import get_intersection, jaccard_similarity, mrca_and_score
+from semsimian import get_intersection, jaccard_similarity, mrca_and_score
 
 from oaklib.datamodels.similarity import (
     BestMatch,
     TermInfo,
     TermPairwiseSimilarity,
     TermSetPairwiseSimilarity,
 )
@@ -21,20 +21,20 @@
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 wrapped_adapter: BasicOntologyInterface = None
 
 __all__ = [
-    "RustSimImplementation",
+    "SemSimianImplementation",
 ]
 
 
 @dataclass
-class RustSimImplementation(SearchInterface, SemanticSimilarityInterface, OboGraphInterface):
+class SemSimianImplementation(SearchInterface, SemanticSimilarityInterface, OboGraphInterface):
     """Rust implementation of semantic similarity measures."""
 
     delegated_methods: ClassVar[List[str]] = [
         BasicOntologyInterface.label,
         BasicOntologyInterface.curie_to_uri,
         BasicOntologyInterface.uri_to_curie,
         BasicOntologyInterface.ontologies,
@@ -43,21 +43,21 @@
         OboGraphInterface.node,
     ]
 
     def __post_init__(self):
         slug = self.resource.slug
         from oaklib.selector import get_adapter
 
-        slug = slug.replace("rustsim:", "")
+        slug = slug.replace("semsimian:", "")
         logging.info(f"Wrapping an existing OAK implementation to fetch {slug}")
         self.wrapped_adapter = get_adapter(slug)
         methods = dict(inspect.getmembers(self.wrapped_adapter))
         for m in self.delegated_methods:
             mn = m if isinstance(m, str) else m.__name__
-            setattr(RustSimImplementation, mn, methods[mn])
+            setattr(SemSimianImplementation, mn, methods[mn])
 
     def most_recent_common_ancestors(
         self,
         subject: CURIE,
         object: CURIE,
         predicates: List[PRED_CURIE] = None,
         include_owl_thing: bool = True,
```

### Comparing `oaklib-0.5.5/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.6/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.6/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.6/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.6/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.6/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.6/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.6/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/html_writer.py` & `oaklib-0.5.6/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.6/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.6/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.6/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.6/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.6/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/__init__.py` & `oaklib-0.5.6/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.6/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.6/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.6/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/resource.py` & `oaklib-0.5.6/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/selector.py` & `oaklib-0.5.6/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.6/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.6/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.6/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.6/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.6/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.6/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.6/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.6/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -298,25 +298,25 @@
     """
     Renders a report performing optional filtering and sorting
 
     Passing no options will just generate the input report in the desired format.
 
     Example:
 
-        boomerang filter tests/input/boomer-example.md  report.yaml
+        boomerang report tests/input/boomer-example.md  report.yaml
 
     The generic LinkML rendered can be used:
 
     Example:
 
-        boomerang filter tests/input/boomer-example.md -O html -o report.html
+        boomerang report tests/input/boomer-example.md -O html -o report.html
 
     To show the lowest confidence first:
 
-        boomerang filter tests/input/boomer-example.md --no-best-first
+        boomerang report tests/input/boomer-example.md --no-best-first
 
     """
     ben = BoomerEngine()
     ben.load(input_report, prefix_map=global_prefix_map)
     writer = _get_writer(
         output_type, None, StreamingYamlWriter, datamodel=mapping_cluster_datamodel
     )
@@ -347,41 +347,41 @@
     Compares boomer results with existing mappings.
 
     This assumes boomer has been executed in advance, and a markdown report generated.
     Pass in as an argument the same ontology used in the boomer run.
 
     Example:
 
-        boomerang foo-boomer.md -i foo.db
+        boomerang compare foo-boomer.md -i foo.db
 
     For any mapping marked NEW, this can be incorporated into the ontology.
 
     For any mapping marked CONFLICT, there is some action that needs to be taken
 
     By default any boomer resolved mapping beneath the default minimum confidence is ignored.
     To customize, e.g. stringent:
 
     Example:
 
-        boomerang foo-boomer.md -i foo.db -L 0.999
+        boomerang compare foo-boomer.md -i foo.db -L 0.999
 
     For each high confidence boomer mapping, this is compared against current mappings and
     a suggestion made.
 
     SPECIFIC SUGGESTIONS FOR OBO ONTOLOGIES:
 
     In many ontologies it is conventional to (a) model all mappings as xrefs (b) assume
     a default interpretation of exactMatch.
 
     In these cases, we want to REJECT any existing xref IF there is a high confidence
     boomer mapping FOR ANYTHING OTHER THAN exactMatch (including SiblingOf)
 
     Example:
 
-        boomerang foo-boomer.md -i foo.db -L 0.999 --reject-non-exact --promote-xref-to-exact
+        boomerang compare foo-boomer.md -i foo.db -L 0.999 --reject-non-exact --promote-xref-to-exact
 
     The results here are straightforward, either REJECT, NEW, or OK
 
     If this is NOT your workflow, then the results may include CONFLICT lines where
     the interpretation you state is different from the interpretation in
 
     See https://github.com/INCATools/boomer/issues/334
```

### Comparing `oaklib-0.5.5/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.6/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.6/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.6/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.6/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.6/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.6/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.6/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.6/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.6/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.6/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.6/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.6/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.6/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.6/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.6/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.5/PKG-INFO` & `oaklib-0.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.5
+Version: 0.5.6
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -19,30 +19,30 @@
 Requires-Dist: bioregistry (>=0.6.35)
 Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: click
 Requires-Dist: curies (>=0.4.0)
 Requires-Dist: eutils (>=0.6.0)
 Requires-Dist: funowl (>=0.1.12)
 Requires-Dist: gilda (>=0.10.1,<0.11.0) ; extra == "gilda"
-Requires-Dist: kgcl-rdflib (>=0.3.0,<0.4.0)
-Requires-Dist: kgcl-schema (>=0.3.5)
+Requires-Dist: kgcl-rdflib (==0.5.0)
+Requires-Dist: kgcl-schema (==0.5.0)
 Requires-Dist: lark (>=1.1.2)
 Requires-Dist: linkml-renderer (>=0.1.2)
 Requires-Dist: linkml-runtime (>=1.2.15)
 Requires-Dist: ndex2 (>=3.5.0,<4.0.0)
 Requires-Dist: networkx (>=2.7.1)
 Requires-Dist: ols-client (>=0.1.1)
 Requires-Dist: ontoportal-client (>=0.0.3)
 Requires-Dist: prefixmaps (>=0.1.2)
 Requires-Dist: pronto (>=2.5.0)
 Requires-Dist: pysolr (>=3.9.0,<4.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: ratelimit (>=2.2.1)
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
-Requires-Dist: rustsim (>=0.1.6)
+Requires-Dist: semsimian (>=0.1.13)
 Requires-Dist: semsql (>=0.3.1)
 Requires-Dist: sssom (>=0.3.26)
 Requires-Dist: sssom-schema (>=0.11.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
```

