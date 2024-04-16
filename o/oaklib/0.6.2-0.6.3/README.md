# Comparing `tmp/oaklib-0.6.2.tar.gz` & `tmp/oaklib-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.6.2.tar", max compression
+gzip compressed data, was "oaklib-0.6.3.tar", max compression
```

## Comparing `oaklib-0.6.2.tar` & `oaklib-0.6.3.tar`

### file list

```diff
@@ -1,312 +1,316 @@
--rw-r--r--   0        0        0    11357 2024-04-11 17:07:15.864147 oaklib-0.6.2/LICENSE
--rw-r--r--   0        0        0     7258 2024-04-11 17:07:15.864147 oaklib-0.6.2/README.md
--rw-r--r--   0        0        0     3441 2024-04-11 17:07:53.948223 oaklib-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      272 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/__init__.py
--rw-r--r--   0        0        0   227527 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      372 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      162 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     1011 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      529 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
--rw-r--r--   0        0        0      118 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4730 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      149 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1461 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2547 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2446 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12105 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     6889 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     6100 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    38339 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0    13058 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    13288 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     3262 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24250 2024-04-11 17:07:16.028147 oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35746 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    14566 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3560 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15776 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     6339 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17296 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26474 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    30133 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3634 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    51109 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    19600 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117221 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3348 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25157 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6684 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2024-04-11 17:07:16.032147 oaklib-0.6.2/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12826 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22645 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5690 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0    23481 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/synonymizer_datamodel.py
--rw-r--r--   0        0        0     2476 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/synonymizer_datamodel.yaml
--rw-r--r--   0        0        0     9909 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18432 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5880 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    21645 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4996 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    31347 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     8316 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     6595 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     6452 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     6377 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/agrkb/__init__.py
--rw-r--r--   0        0        0     8848 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/agrkb/agrkb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0    16195 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/amigo/amigo_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/eutils/__init__.py
--rw-r--r--   0        0        0     2180 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/eutils/eutils_implementation.py
--rw-r--r--   0        0        0     1055 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/eutils/pubmed_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     3565 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30523 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0    24539 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/llm_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/monarch/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/monarch/monarch_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ncbi/__init__.py
--rw-r--r--   0        0        0     7034 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    17122 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     8071 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2024-04-11 17:07:16.036147 oaklib-0.6.2/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     2641 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0     1250 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    13670 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/pantherdb/__init__.py
--rw-r--r--   0        0        0    12625 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    37863 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/semsimian/__init__.py
--rw-r--r--   0        0        0      247 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/semsimian/profiler.py
--rw-r--r--   0        0        0    11605 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/semsimian/semsimian_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    45330 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    22505 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    38067 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2325 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   115796 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/tabular/__init__.py
--rw-r--r--   0        0        0    19432 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/tabular/robot_template_implementation.py
--rw-r--r--   0        0        0     3279 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/tabular/tabular_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     5442 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    20090 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0    14740 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17267 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/indexes/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/indexes/edge_index.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/inference/__init__.py
--rw-r--r--   0        0        0      748 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/inference/owl_reasoner.py
--rw-r--r--   0        0        0      105 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/inference/reasoner.py
--rw-r--r--   0        0        0     6960 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/inference/relation_graph_reasoner.py
--rw-r--r--   0        0        0      913 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    28686 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    55465 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     9243 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    21219 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     3222 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0      788 2024-04-11 17:07:16.040147 oaklib-0.6.2/src/oaklib/interfaces/embedding_provider_interface.py
--rw-r--r--   0        0        0    13680 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    22241 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      786 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/ontology_generator_interface.py
--rw-r--r--   0        0        0      784 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    13645 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8606 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2287 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     3759 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    16173 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2113 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18295 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0    10076 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     4119 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     2091 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1565 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     9012 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0      785 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2672 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     4928 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5126 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1318 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3956 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1979 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2363 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0     1525 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4732 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     2148 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     2101 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0     1131 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0     1673 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/hpoa_g2d_association_parser.py
--rw-r--r--   0        0        0      603 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      654 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1672 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      526 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1433 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      708 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     8681 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/resource.py
--rw-r--r--   0        0        0    15958 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/selector.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/__init__.py
--rw-r--r--   0        0        0      589 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/chained_ontology_transformer.py
--rw-r--r--   0        0        0     2757 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/edge_filter_transformer.py
--rw-r--r--   0        0        0     1257 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/graph_transformer.py
--rw-r--r--   0        0        0     1804 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/node_filter_transformer.py
--rw-r--r--   0        0        0      470 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/ontology_transformer.py
--rw-r--r--   0        0        0     6353 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/sep_transformer.py
--rw-r--r--   0        0        0     1768 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/transformers/transformers_factory.py
--rw-r--r--   0        0        0      177 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0    13441 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     3427 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/axioms/__init__.py
--rw-r--r--   0        0        0     7694 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
--rw-r--r--   0        0        0     4093 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_analyzer.py
--rw-r--r--   0        0        0     8829 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_summarizer.py
--rw-r--r--   0        0        0     2436 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_utilities.py
--rw-r--r--   0        0        0     1540 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0     1356 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/format_utilities.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2491 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2857 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2024-04-11 17:07:16.044147 oaklib-0.6.2/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     1015 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/keyval_cache.py
--rw-r--r--   0        0        0     3425 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19249 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0    10235 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/lexical/patternizer.py
--rw-r--r--   0        0        0     6881 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/lexical/synonymizer.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14422 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15527 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0    10929 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2558 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      690 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    30409 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      380 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     2545 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2819 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    12015 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    18045 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0      122 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/writers/__init__.py
--rw-r--r--   0        0        0    16522 2024-04-11 17:07:16.048147 oaklib-0.6.2/src/oaklib/utilities/writers/change_handler.py
--rw-r--r--   0        0        0     9129 1970-01-01 00:00:00.000000 oaklib-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-16 00:05:41.065160 oaklib-0.6.3/LICENSE
+-rw-r--r--   0        0        0     7258 2024-04-16 00:05:41.065160 oaklib-0.6.3/README.md
+-rw-r--r--   0        0        0     3500 2024-04-16 00:06:13.765343 oaklib-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      272 2024-04-16 00:05:41.229161 oaklib-0.6.3/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   232022 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      162 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     1011 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      529 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      118 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4730 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      149 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1461 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2547 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2446 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12105 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     7719 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     6100 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    38339 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0    13058 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13288 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3262 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24250 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35746 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14566 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15776 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17296 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26474 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2024-04-16 00:05:41.233161 oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    30133 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3634 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    51109 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    19600 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   116914 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    31452 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3348 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25157 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6684 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12826 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22645 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5690 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0    23481 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.py
+-rw-r--r--   0        0        0     2476 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18432 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5880 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    21645 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4996 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    33912 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     9005 2024-04-16 00:05:41.237161 oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     6595 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     6452 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/agrkb/__init__.py
+-rw-r--r--   0        0        0     8848 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/agrkb/agrkb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0    16195 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2180 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1055 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     3565 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30523 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0    28777 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/llm_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/monarch/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/monarch/monarch_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ncbi/__init__.py
+-rw-r--r--   0        0        0     7034 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    17122 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     8071 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2641 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1250 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    13670 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pantherdb/__init__.py
+-rw-r--r--   0        0        0    12625 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pantherdb/pantherdb_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    37863 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/__init__.py
+-rw-r--r--   0        0        0      247 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/profiler.py
+-rw-r--r--   0        0        0    11605 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/semsimian/semsimian_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    46328 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    23081 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.241161 oaklib-0.6.3/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    38067 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2325 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   115796 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/__init__.py
+-rw-r--r--   0        0        0    19432 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/robot_template_implementation.py
+-rw-r--r--   0        0        0     3279 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tabular/tabular_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     5442 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    20090 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0    14740 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17267 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/indexes/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/indexes/edge_index.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/__init__.py
+-rw-r--r--   0        0        0      748 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/owl_reasoner.py
+-rw-r--r--   0        0        0      105 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/reasoner.py
+-rw-r--r--   0        0        0     6960 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/inference/relation_graph_reasoner.py
+-rw-r--r--   0        0        0      913 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    28686 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    55465 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     9243 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    21219 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     3222 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      788 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13680 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    22954 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      786 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/ontology_generator_interface.py
+-rw-r--r--   0        0        0      784 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    13645 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8606 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2287 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     3759 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    16173 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2113 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18295 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0    10076 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0    12915 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     2091 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1565 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2024-04-16 00:05:41.245161 oaklib-0.6.3/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     9012 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0      785 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2672 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3485 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5126 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1318 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3956 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1979 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2363 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1525 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4732 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     2148 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     2101 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0     1131 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0     1673 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_g2d_association_parser.py
+-rw-r--r--   0        0        0      603 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      654 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1672 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      526 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1433 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      708 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     8681 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/resource.py
+-rw-r--r--   0        0        0    15958 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/selector.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/__init__.py
+-rw-r--r--   0        0        0      589 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/chained_ontology_transformer.py
+-rw-r--r--   0        0        0     2757 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/edge_filter_transformer.py
+-rw-r--r--   0        0        0     1257 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/graph_transformer.py
+-rw-r--r--   0        0        0     1804 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/node_filter_transformer.py
+-rw-r--r--   0        0        0      470 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/ontology_transformer.py
+-rw-r--r--   0        0        0     6353 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/sep_transformer.py
+-rw-r--r--   0        0        0     1768 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/transformers/transformers_factory.py
+-rw-r--r--   0        0        0      177 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    13441 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3427 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/__init__.py
+-rw-r--r--   0        0        0     7694 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py
+-rw-r--r--   0        0        0     4093 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_analyzer.py
+-rw-r--r--   0        0        0     8829 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_summarizer.py
+-rw-r--r--   0        0        0     2436 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_utilities.py
+-rw-r--r--   0        0        0     1540 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0     1356 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/format_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2857 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     1015 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/keyval_cache.py
+-rw-r--r--   0        0        0     3425 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19249 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0    10235 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/patternizer.py
+-rw-r--r--   0        0        0     6881 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/lexical/synonymizer.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14422 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15527 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0    10929 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2558 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      690 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    30409 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/__init__.py
+-rw-r--r--   0        0        0     5283 2024-04-16 00:05:41.249161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/doi_wrapper.py
+-rw-r--r--   0        0        0      924 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubdb_wrapper.py
+-rw-r--r--   0        0        0     6575 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/publication_utils/pubmed_wrapper.py
+-rw-r--r--   0        0        0      380 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     2545 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2819 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    12015 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    18045 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    11118 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1275 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0      122 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/writers/__init__.py
+-rw-r--r--   0        0        0    16522 2024-04-16 00:05:41.253161 oaklib-0.6.3/src/oaklib/utilities/writers/change_handler.py
+-rw-r--r--   0        0        0     9171 1970-01-01 00:00:00.000000 oaklib-0.6.3/PKG-INFO
```

### Comparing `oaklib-0.6.2/LICENSE` & `oaklib-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/README.md` & `oaklib-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/pyproject.toml` & `oaklib-0.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.6.2"
+version = "v0.6.3"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -22,14 +22,15 @@
 kgcl-schema = "^0.6.8"
 
 funowl = ">=0.2.0"
 gilda = {version = ">=1.0.0", optional = true}
 semsimian = {version = ">=0.2.15", optional = true}
 kgcl-rdflib = "0.5.0"
 llm = {version = "*", optional = true}
+html2text = {version = "*", optional = true}
 aiohttp = {version = "*", optional = true}
 pystow = ">=0.5.0"
 class-resolver = ">=0.4.2"
 ontoportal-client = ">=0.0.3"
 prefixmaps = ">=0.1.2"
 ols-client = ">=0.1.1"
 airium = ">=0.2.5"
@@ -70,15 +71,15 @@
 runoak = "oaklib.cli:main"
 vskit = "oaklib.utilities.subsets.value_set_expander:main"
 boomerang = "oaklib.utilities.mapping.boomer_utils:main"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-mermaid", "sphinx-copybutton"]
 gilda = ["scipy", "gilda", "urllib3"]
-llm = ["llm", "aiohttp"]
+llm = ["llm", "aiohttp", "html2text"]
 seaborn = ["seaborn"]
 semsimian = ["semsimian"]
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310"]
 
@@ -122,8 +123,8 @@
 ]
 
 lint.unfixable = []
 target-version = "py310"
 
 [tool.ruff.lint.mccabe]
 # Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
+max-complexity = 10
```

### Comparing `oaklib-0.6.2/src/oaklib/cli.py` & `oaklib-0.6.3/src/oaklib/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,24 +186,22 @@
     default_stylemap_path,
     graph_to_d3viz_objects,
     graph_to_image,
     graph_to_tree_display,
     shortest_paths,
     trim_graph,
 )
+from oaklib.utilities.publication_utils.pubmed_wrapper import PubmedWrapper
 from oaklib.utilities.semsim.similarity_utils import load_information_content_map
 from oaklib.utilities.subsets.slimmer_utils import (
     filter_redundant,
     roll_up_to_named_subset,
 )
 from oaklib.utilities.table_filler import ColumnDependency, TableFiller, TableMetadata
 from oaklib.utilities.taxon.taxon_constraint_utils import parse_gain_loss_file
-from oaklib.utilities.validation.definition_ontology_rule import (
-    TextAndLogicalDefinitionMatchOntologyRule,
-)
 from oaklib.utilities.validation.lint_utils import lint_ontology
 from oaklib.utilities.validation.rule_runner import RuleRunner
 
 OBO_FORMAT = "obo"
 RDF_FORMAT = "rdf"
 MD_FORMAT = "md"
 HTML_FORMAT = "html"
@@ -430,14 +428,19 @@
     help='overrides for stylemap, specified as yaml. E.g. `-C "styles: [filled, rounded]" `',
 )
 configuration_file_option = click.option(
     "-C",
     "--configuration-file",
     help="Path to a configuration file. This is typically a YAML file, but may be a JSON file",
 )
+adapter_mapping_option = click.option(
+    "--adapter-mapping",
+    multiple=True,
+    help="Multiple prefix=selector pairs, e.g. --adapter-mapping uberon=db/uberon.db",
+)
 pivot_languages = click.option(
     "--pivot-languages/--no-pivot-languages",
     help="include one column per language",
 )
 all_languages = click.option(
     "--all-languages/--no-all-languages",
     help="if source is multi-lingual, show all languages rather than just default",
@@ -3291,36 +3294,46 @@
 @click.argument("terms", nargs=-1)
 @output_option
 @display_option
 @ontological_output_type_option
 @if_absent_option
 @additional_metadata_option
 @set_value_option
+@click.option(
+    "--lookup-references/--no-lookup-references",
+    "-P",
+    default=False,
+    show_default=True,
+    help="Lookup references for each term, e.g. PMIDs",
+)
 @autolabel_option
 def definitions(
     terms,
     output: TextIO,
     additional_metadata: bool,
     display: str,
     output_type: str,
     if_absent: bool,
     autolabel: bool,
+    lookup_references: bool,
     set_value,
 ):
     """
     Show textual definitions for term or set of terms
 
     Example:
     -------
+
         runoak -i sqlite:obo:envo definitions 'tropical biome' 'temperate biome'
 
     You can use the ".all" selector to show all definitions for all terms in the ontology:
 
     Example:
     -------
+
         runoak -i sqlite:obo:envo definitions .all
 
     You can also include definition metadata, such as provenance and source:
 
         runoak -i sqlite:obo:cl definitions --additional-metadata neuron
 
     Python API:
@@ -3328,14 +3341,17 @@
        https://incatools.github.io/ontology-access-kit/interfaces/basic
 
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingCsvWriter)
     writer.display_options = display.split(",")
     writer.file = output
+    if lookup_references and not additional_metadata:
+        logging.warning("Setting lookup_references to True implies additional_metadata=True")
+        additional_metadata = True
     if additional_metadata:
         writer.heterogeneous_keys = True
     changes = []
     if not isinstance(impl, BasicOntologyInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     all_curies = []
     for curie_it in chunk(query_terms_iterator(terms, impl)):
@@ -3346,14 +3362,24 @@
             labels = {curie: label for curie, label in impl.labels(curies)}
         for curie, defn, metadata in impl.definitions(
             curies, include_metadata=additional_metadata, include_missing=True
         ):
             if metadata is None:
                 metadata = {}
             obj = dict(id=curie, label=labels.get(curie, None), definition=defn, **metadata)
+            if lookup_references:
+                refs = []
+                obj["references"] = refs
+                pubmed_wrapper = PubmedWrapper()
+                for _k, vs in metadata.items():
+                    pmids = [v for v in vs if v.startswith("PMID:")]
+                    if pmids:
+                        objs = pubmed_wrapper.objects_by_ids(pmids)
+                        refs.extend(objs)
+
             if set_value is not None:
                 # set the value by creating a KGCL change object for applying later
                 obj["new_value"] = set_value
                 if set_value != defn:
                     changes.append(
                         kgcl.NodeTextDefinitionChange(
                             id="x", about_node=curie, old_value=defn, new_value=set_value
@@ -5327,40 +5353,51 @@
 @main.command()
 @click.option(
     "--skip-text-annotation/--no-skip-text-annotation",
     default=False,
     show_default=True,
     help="If true, do not parse text annotations",
 )
+@configuration_file_option
+@adapter_mapping_option
 @output_type_option
 @output_option
 @click.argument("terms", nargs=-1)
-def validate_definitions(terms, skip_text_annotation, output: str, output_type: str):
+def validate_definitions(
+    terms,
+    skip_text_annotation,
+    output: str,
+    output_type: str,
+    configuration_file: str,
+    adapter_mapping: List[str],
+):
     """
     Checks presence and structure of text definitions.
 
     To run:
 
         runoak validate-definitions -i db/uberon.db -o results.tsv
 
     By default this will apply basic text mining of text definitions to check
     against machine actionable OBO text definition guideline rules.
     This can result in an initial lag - to skip this, and ONLY perform
-    checks for presence of definitions, use --skip-text-annotation:
+    checks for *presence* of definitions, use --skip-text-annotation:
 
     Example:
     -------
+
         runoak validate-definitions -i db/uberon.db --skip-text-annotation
 
     Like most OAK commands, this accepts lists of terms or term queries
     as arguments. You can pass in a CURIE list to selectively validate
     individual classes
 
     Example:
     -------
+
          runoak validate-definitions -i db/cl.db CL:0002053
 
     Only on CL identifiers:
 
         runoak validate-definitions -i db/cl.db i^CL:
 
     Only on neuron hierarchy:
@@ -5373,46 +5410,51 @@
     See https://incatools.github.io/ontology-access-kit/datamodels for more
     on OAK datamodels.
 
     The default serialization of the datamodel is CSV.
 
     Notes:
     -----
+
     This command is largely redundant with the validate command, but is useful for
     targeted validation focused solely on definitions
 
     """
     impl = settings.impl
     writer = _get_writer(
         output_type, impl, StreamingCsvWriter, datamodel=datamodels.validation_datamodel
     )
+    writer.autolabel = True
     writer.output = output
-    if isinstance(impl, ValidatorInterface):
-        if terms:
-            entities = query_terms_iterator(terms, impl)
-        else:
-            entities = None
-        definition_rule = TextAndLogicalDefinitionMatchOntologyRule(
-            skip_text_annotation=skip_text_annotation
-        )
-        for vr in definition_rule.evaluate(impl, entities=entities):
-            writer.emit(vr)
-        writer.finish()
-    else:
+    if not isinstance(impl, ValidatorInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    if configuration_file:
+        config = yaml_loader.load(configuration_file, target_class=ValidationConfiguration)
+    else:
+        config = None
+    adapters = {}
+    for am in adapter_mapping:
+        prefix, selector = am.split("=")
+        adapters[prefix] = get_adapter(selector)
+        logging.info(f"Loaded adapter for {prefix} => {selector}")
+    if terms:
+        entities = query_terms_iterator(terms, impl)
+    else:
+        entities = None
+    for vr in impl.validate_definitions(
+        entities, adapters=adapters, configuration=config, skip_text_annotation=skip_text_annotation
+    ):
+        writer.emit(vr, label_fields=["subject"])
+    writer.finish()
 
 
 @main.command()
 @autolabel_option
 @output_type_option
-@click.option(
-    "--adapter-mapping",
-    multiple=True,
-    help="Multiple prefix=selector pairs, e.g. --adapter-mapping uberon=db/uberon.db",
-)
+@adapter_mapping_option
 @output_option
 @configuration_file_option
 @click.argument("terms", nargs=-1)
 def validate_mappings(
     terms, autolabel, adapter_mapping, output: str, output_type: str, configuration_file: str
 ):
     """
@@ -5473,14 +5515,112 @@
         logging.info(f"Loaded adapter for {prefix} => {selector}")
     for result in impl.validate_mappings(entities, adapters=adapters, configuration=config):
         writer.emit_obj(result)
     writer.finish()
 
 
 @main.command()
+@autolabel_option
+@output_type_option
+@adapter_mapping_option
+@output_option
+@configuration_file_option
+@click.option(
+    "--rules-file",
+    "-R",
+    help="path to rules file. Conforms to rules_datamodel.\
+        e.g. https://github.com/INCATools/ontology-access-kit/blob/main/tests/input/matcher_rules.yaml",
+)
+@click.argument("terms", nargs=-1)
+def validate_synonyms(
+    terms,
+    autolabel,
+    adapter_mapping,
+    output: str,
+    output_type: str,
+    rules_file: str,
+    configuration_file: str,
+):
+    """
+    Validates synonyms in ontology using additional ontologies.
+
+    To run:
+
+        runoak validate-synonyms -i db/uberon.db
+
+    You can customize this mapping:
+
+        runoak validate-synonyms -i db/uberon.db --adapter-mapping uberon=db/uberon.db \
+            --adapter-mapping zfa=sqlite:obo:zfa
+
+    This will use a remote sqlite file for ZFA:nnnnnnn IDs.
+
+    You can use "*" as a wildcard, in the case where you have an application ontology
+    with many mapped entities merged in:
+
+        runoak validate-synonyms -i db/uberon.db --adapter-mapping "*"=db/merged.db"
+
+    You can also pass synonymizer rules. For example:
+
+        runoak -i sqlite:obo:go  validate-synonyms \
+           -R go-strip-activity.synonymizer.yaml GO:0000010 \
+            --adapter-mapping ec=sqlite:obo:eccode
+
+    In this case if the synonymizer rule file contains:
+
+        \b
+        rules:
+          - match: " activity"
+            replacement: ""
+        \b
+
+    Then the GO synonyms will have the word "activity" stripped from them, prior to attempting
+    to match with EC.
+
+    The default behavior for this command is to perform deterministic rule-based
+    checks; for example, the mapped IDs should not be obsolete, and if the mapping
+    is skos:exactMatch, then the cardinality is expected to be 1:1.
+
+    Other adapters may choose to implement bespoke behaviors. In future there
+    might be a boomer adapter that will perform probabilistic reasoning on the
+    mappings. The experimental LLM backend will use an LLM to qualitatively
+    validate mappings (see the LLM how-to guide for more details).
+    """
+    impl = settings.impl
+    writer = _get_writer(output_type, impl, StreamingCsvWriter)
+    writer.output = output
+    writer.autolabel = autolabel
+    if not isinstance(impl, ValidatorInterface):
+        raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    if terms:
+        entities = query_terms_iterator(terms, impl)
+    else:
+        entities = None
+    if configuration_file:
+        config = yaml_loader.load(configuration_file, target_class=ValidationConfiguration)
+    else:
+        config = None
+    if rules_file:
+        ruleset = synonymizer_datamodel.RuleSet(**yaml.safe_load(open(rules_file)))
+    else:
+        ruleset = None
+
+    adapters = {}
+    for am in adapter_mapping:
+        prefix, selector = am.split("=")
+        adapters[prefix] = get_adapter(selector)
+        logging.info(f"Loaded adapter for {prefix} => {selector}")
+    for result in impl.validate_synonyms(
+        entities, adapters=adapters, configuration=config, synonymizer_rules=ruleset
+    ):
+        writer.emit_obj(result)
+    writer.finish()
+
+
+@main.command()
 @click.argument("curie_pairs", nargs=-1)
 @click.option(
     "--replace/--no-replace", default=False, show_default=True, help="If true, will update in place"
 )
 @output_type_option
 @output_option
 def migrate_curies(curie_pairs, replace: bool, output_type, output: str):
@@ -6472,20 +6612,22 @@
     Generate synonyms based on a set of synonymizer rules.
 
     If the `--apply-patch` flag is set, the output will be an ontology file with the changes
     applied. Pass the `--patch` argument to lso get the patch file in KGCL format.
 
     Example:
     -------
+
         runoak -i foo.obo generate-synonyms -R foo_rules.yaml --patch patch.kgcl --apply-patch -o foo_syn.obo
 
     If the `apply-patch` flag is NOT set then the main input will be KGCL commands
 
     Example:
     -------
+
         runoak -i foo.obo generate-synonyms -R foo_rules.yaml -o changes.kgcl
 
     see https://github.com/INCATools/kgcl.
 
     """
     impl = settings.impl
     if apply_patch:
```

### Comparing `oaklib-0.6.2/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.6.3/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.6.3/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml` & `oaklib-0.6.3/src/oaklib/conf/mondo-hpoa-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/conf/obograph-style.json` & `oaklib-0.6.3/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/converters/data_model_converter.py` & `oaklib-0.6.3/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.6.3/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 import sys
 from dataclasses import dataclass
 from io import BytesIO, StringIO
-from typing import Any, Dict, List, Tuple
+from typing import Any, Dict, List, Optional, Tuple, Union
 
 import rdflib
 
 from oaklib.converters.data_model_converter import DataModelConverter
 from oaklib.datamodels.obograph import Edge, Graph, GraphDocument, Node
 from oaklib.datamodels.vocabulary import IS_A, SYNONYM_PRED_TO_SCOPE_MAP
 from oaklib.implementations.simpleobo.simple_obo_parser import (
@@ -62,90 +62,121 @@
         obodoc = self.convert(source)
         if target is None:
             obodoc.dump(sys.stdout)
         else:
             with open(target, "w", encoding="UTF-8") as f:
                 obodoc.dump(f)
 
-    def dumps(self, source: GraphDocument, **kwargs) -> str:
+    def dumps(
+        self,
+        source: Union[GraphDocument, Graph],
+        aux_graphs: Optional[List[Graph]] = None,
+        **kwargs,
+    ) -> str:
         """
         Dump an OBO Graph Document to a string
 
         :param source:
         :return:
         """
-        obodoc = self.convert(source)
+        obodoc = self.convert(source, aux_graphs=aux_graphs)
         io = StringIO()
         obodoc.dump(io)
         return io.getvalue()
 
     def as_bytes_io(self, source: GraphDocument, **kwargs) -> BytesIO:
         """
         Dump an OBO Graph Document to a string
 
         :param source:
         :return:
         """
         s = self.dumps(source)
         return BytesIO(s.encode("UTF-8"))
 
-    def convert(self, source: GraphDocument, target: OboDocument = None, **kwargs) -> OboDocument:
+    def convert(
+        self,
+        source: Union[GraphDocument, Graph],
+        target: OboDocument = None,
+        aux_graphs: Optional[List[Graph]] = None,
+        **kwargs,
+    ) -> OboDocument:
         """
         Convert an OBO Format Document.
 
         :param source:
         :param target: if None, one will be created
+        :param aux_graphs: additional graphs to use for label lookup
         :return:
         """
         if target is None:
             target = OboDocument()
+        if isinstance(source, Graph):
+            source = GraphDocument(graphs=[source])
         for g in source.graphs:
             logging.info(f"Converting graph {g.id}, nodes: {len(g.nodes)}, edges: {len(g.edges)}")
-            self._convert_graph(g, target=target)
+            self._convert_graph(g, target=target, aux_graphs=aux_graphs)
         logging.info(f"Converted {len(target.stanzas)} stanzas")
         return target
 
+    def _commentify(
+        self, curie: CURIE, graph: Graph, aux_graphs: Optional[List[Graph]] = None
+    ) -> str:
+        graphs = [graph] + (aux_graphs or [])
+        for g in graphs:
+            for n in g.nodes:
+                if n.id == curie and n.lbl:
+                    return f"{curie} ! {n.lbl}"
+        return curie
+
     def _id(self, uri_or_curie: CURIE) -> CURIE:
         if not self.curie_converter:
             return uri_or_curie
         return self.curie_converter.compress(uri_or_curie, passthrough=True)
 
     def _predicate_id(self, uri_or_curie: CURIE, target: OboDocument) -> CURIE:
         curie = self._id(uri_or_curie)
         return target.curie_to_shorthand_map.get(curie, curie)
 
-    def _convert_graph(self, source: Graph, target: OboDocument) -> OboDocument:
+    def _convert_graph(
+        self, source: Graph, target: OboDocument, aux_graphs: Optional[List[Graph]] = None
+    ) -> OboDocument:
         edges_by_subject = index_graph_edges_by_subject(source)
         for n in source.nodes:
             if n.type == "PROPERTY" and n.lbl:
                 shorthand = n.lbl.replace(" ", "_")
                 target.curie_to_shorthand_map[self._id(n.id)] = shorthand
         for n in source.nodes:
             logging.debug(f"Converting node {n.id}")
-            self._convert_node(n, index=edges_by_subject, target=target, graph=source)
+            self._convert_node(
+                n, index=edges_by_subject, target=target, graph=source, aux_graphs=aux_graphs
+            )
         for lda in source.logicalDefinitionAxioms:
             defined_class_id = self._id(lda.definedClassId)
             if defined_class_id not in target.stanzas:
                 target.add_stanza(Stanza(id=defined_class_id, type="Term"))
             stanza = target.stanzas[defined_class_id]
             for g in lda.genusIds:
                 obj = self._id(g)
+                obj = self._commentify(obj, source, aux_graphs)
                 stanza.add_tag_value(TAG_INTERSECTION_OF, obj)
             for r in lda.restrictions:
                 filler = self._id(r.fillerId)
+                filler = self._commentify(filler, source, aux_graphs)
                 pred = self._id(r.propertyId)
                 stanza.add_tag_value_pair(TAG_INTERSECTION_OF, pred, filler)
         return target
 
     def _convert_node(
         self,
         source: Node,
         index: Dict[CURIE, List[Edge]],
         target: OboDocument,
         graph: Graph = None,
+        aux_graphs: Optional[List[Graph]] = None,
     ) -> None:
         id = self._id(source.id)
         shorthand_xref = None
         if id in target.curie_to_shorthand_map:
             shorthand_xref = id
             id = target.curie_to_shorthand_map[id]
         logging.debug(f"Converting node {id} from {source}")
@@ -164,28 +195,20 @@
             stanza.add_tag_value(TAG_NAME, source.lbl)
         if source.meta:
             self._convert_meta(source, target=stanza)
         if shorthand_xref:
             stanza.add_tag_value(TAG_XREF, shorthand_xref)
         for e in index.get(source.id, []):
             obj = self._id(e.obj)
-            obj_lbl = None
-            if graph:
-                nodes = [n for n in graph.nodes if n.id == e.obj]
-                if nodes:
-                    obj_lbl = nodes[0].lbl
-            if obj_lbl:
-                cmt = f" ! {obj_lbl}"
-            else:
-                cmt = ""
+            obj_labeled = self._commentify(obj, graph, aux_graphs)
             pred = self._predicate_id(e.pred, target)
             if e.pred in DIRECT_PREDICATE_MAP:
-                stanza.add_tag_value(DIRECT_PREDICATE_MAP[e.pred], f"{obj}{cmt}")
+                stanza.add_tag_value(DIRECT_PREDICATE_MAP[e.pred], f"{obj_labeled}")
             else:
-                stanza.add_tag_value(TAG_RELATIONSHIP, f"{pred} {obj}{cmt}")
+                stanza.add_tag_value(TAG_RELATIONSHIP, f"{pred} {obj_labeled}")
         return
 
     def _convert_meta(self, source: Node, target: Stanza):
         meta = source.meta
         logging.debug(f"ADDING DEF {target}")
         if meta.definition:
             xrefs = ", ".join(meta.definition.xrefs)
```

### Comparing `oaklib-0.6.2/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.6.3/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/association.py` & `oaklib-0.6.3/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/association.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/cx.py` & `oaklib-0.6.3/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/cx.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/fhir.py` & `oaklib-0.6.3/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/input_specification.py` & `oaklib-0.6.3/src/oaklib/datamodels/input_specification.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/input_specification.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/item_list.py` & `oaklib-0.6.3/src/oaklib/datamodels/item_list.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/item_list.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/obograph.py` & `oaklib-0.6.3/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,138 +1,117 @@
-# Auto generated from ontology_metadata.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-09T14:06:34
+# Auto generated from ontology_metadata.yaml by pythongen.py version: 0.0.1
+# Generation date: 2024-04-14T16:59:12
 # Schema: Ontology-Metadata
 #
-# id: http://purl.obolibrary.org/obo/omo/schema
+# id: https://w3id.org/oak/ontology-metadata
 # description: Schema for ontology metadata
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
-import sys
+from jsonasobj2 import JsonObj, as_dict
+from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from datetime import date, datetime
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
-from jsonasobj2 import JsonObj, as_dict
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-    PvFormulaOptions,
-)
-from linkml_runtime.linkml_model.types import Boolean, Integer, String, Uriorcurie
-from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
-from linkml_runtime.utils.enumerations import EnumDefinitionImpl
-from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import (
-    Bool,
-    URIorCURIE,
-    bnode,
-    empty_dict,
-    empty_list,
-)
 from linkml_runtime.utils.slot import Slot
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_float,
-    extended_int,
-    extended_str,
-)
+from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
+from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
+from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
+from linkml_runtime.utils.curienamespace import CurieNamespace
+from linkml_runtime.linkml_model.types import Boolean, Integer, String, Uriorcurie
+from linkml_runtime.utils.metamodelcore import Bool, URIorCURIE
 
 metamodel_version = "1.7.0"
 version = "0.0.1"
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-IAO = CurieNamespace("IAO", "http://purl.obolibrary.org/obo/IAO_")
-NCBITAXON = CurieNamespace("NCBITaxon", "http://purl.obolibrary.org/obo/NCBITaxon_")
-NCIT = CurieNamespace("NCIT", "http://purl.obolibrary.org/obo/NCIT_")
-OBI = CurieNamespace("OBI", "http://purl.obolibrary.org/obo/OBI_")
-OIO = CurieNamespace("OIO", "http://www.geneontology.org/formats/oboInOwl#")
-OMO = CurieNamespace("OMO", "http://purl.obolibrary.org/obo/OMO_")
-RO = CurieNamespace("RO", "http://purl.obolibrary.org/obo/RO_")
-BIOLINK = CurieNamespace("biolink", "https://w3id.org/biolink/vocab/")
-DCE = CurieNamespace("dce", "http://example.org/UNKNOWN/dce/")
-DCTERMS = CurieNamespace("dcterms", "http://purl.org/dc/terms/")
-FOAF = CurieNamespace("foaf", "http://xmlns.com/foaf/0.1/")
-LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-OBO = CurieNamespace("obo", "http://purl.obolibrary.org/obo/")
-OIO = CurieNamespace("oio", "http://www.geneontology.org/formats/oboInOwl#")
-OMOSCHEMA = CurieNamespace("omoschema", "http://purl.obolibrary.org/obo/omo/schema/")
-ORCID = CurieNamespace("orcid", "https://orcid.org/")
-OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
-PAV = CurieNamespace("pav", "http://purl.org/pav/")
-PROTEGE = CurieNamespace("protege", "http://example.org/UNKNOWN/protege/")
-PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov-o#")
-RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
-SDO = CurieNamespace("sdo", "http://schema.org/")
-SKOS = CurieNamespace("skos", "http://www.w3.org/2004/02/skos/core#")
-XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
+IAO = CurieNamespace('IAO', 'http://purl.obolibrary.org/obo/IAO_')
+NCBITAXON = CurieNamespace('NCBITaxon', 'http://purl.obolibrary.org/obo/NCBITaxon_')
+NCIT = CurieNamespace('NCIT', 'http://purl.obolibrary.org/obo/NCIT_')
+OBI = CurieNamespace('OBI', 'http://purl.obolibrary.org/obo/OBI_')
+OIO = CurieNamespace('OIO', 'http://www.geneontology.org/formats/oboInOwl#')
+OMO = CurieNamespace('OMO', 'http://purl.obolibrary.org/obo/OMO_')
+RO = CurieNamespace('RO', 'http://purl.obolibrary.org/obo/RO_')
+BIOLINK = CurieNamespace('biolink', 'https://w3id.org/biolink/vocab/')
+DCE = CurieNamespace('dce', 'http://example.org/UNKNOWN/dce/')
+DCTERMS = CurieNamespace('dcterms', 'http://purl.org/dc/terms/')
+FOAF = CurieNamespace('foaf', 'http://xmlns.com/foaf/0.1/')
+LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
+OBO = CurieNamespace('obo', 'http://purl.obolibrary.org/obo/')
+OIO = CurieNamespace('oio', 'http://www.geneontology.org/formats/oboInOwl#')
+OMOSCHEMA = CurieNamespace('omoschema', 'https://w3id.org/oak/ontology-metadata/')
+ORCID = CurieNamespace('orcid', 'https://orcid.org/')
+OWL = CurieNamespace('owl', 'http://www.w3.org/2002/07/owl#')
+PAV = CurieNamespace('pav', 'http://purl.org/pav/')
+PROTEGE = CurieNamespace('protege', 'http://example.org/UNKNOWN/protege/')
+PROV = CurieNamespace('prov', 'http://www.w3.org/ns/prov-o#')
+RDF = CurieNamespace('rdf', 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+RDFS = CurieNamespace('rdfs', 'http://www.w3.org/2000/01/rdf-schema#')
+SDO = CurieNamespace('sdo', 'http://schema.org/')
+SKOS = CurieNamespace('skos', 'http://www.w3.org/2004/02/skos/core#')
+XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = OMOSCHEMA
 
 
 # Types
 class IriType(Uriorcurie):
-    """An IRI"""
-
-    type_class_uri = XSD.anyURI
+    """ An IRI """
+    type_class_uri = XSD["anyURI"]
     type_class_curie = "xsd:anyURI"
     type_name = "iri type"
     type_model_uri = OMOSCHEMA.IriType
 
 
 class CURIELiteral(String):
-    """A string representation of a CURIE"""
-
-    type_class_uri = XSD.string
+    """ A string representation of a CURIE """
+    type_class_uri = XSD["string"]
     type_class_curie = "xsd:string"
     type_name = "CURIELiteral"
     type_model_uri = OMOSCHEMA.CURIELiteral
 
 
 class URLLiteral(String):
-    """A URL representation of a CURIE"""
-
-    type_class_uri = XSD.string
+    """ A URL representation of a CURIE """
+    type_class_uri = XSD["string"]
     type_class_curie = "xsd:string"
     type_name = "URLLiteral"
     type_model_uri = OMOSCHEMA.URLLiteral
 
 
 class TidyString(String):
-    type_class_uri = XSD.string
+    type_class_uri = XSD["string"]
     type_class_curie = "xsd:string"
     type_name = "tidy string"
     type_model_uri = OMOSCHEMA.TidyString
 
 
-class LabelType(TidyString):
-    """A string that provides a human-readable name for an entity"""
-
-    type_class_uri = XSD.string
-    type_class_curie = "xsd:string"
-    type_name = "label type"
-    type_model_uri = OMOSCHEMA.LabelType
-
-
 class NarrativeText(String):
-    """A string that provides a human-readable description of something"""
-
-    type_class_uri = XSD.string
+    """ A string that provides a human-readable description of something """
+    type_class_uri = XSD["string"]
     type_class_curie = "xsd:string"
     type_name = "narrative text"
     type_model_uri = OMOSCHEMA.NarrativeText
 
 
+class LabelType(TidyString):
+    """ A string that provides a human-readable name for an entity """
+    type_class_uri = XSD["string"]
+    type_class_curie = "xsd:string"
+    type_name = "label type"
+    type_model_uri = OMOSCHEMA.LabelType
+
+
 # Class references
 class NamedObjectId(URIorCURIE):
     pass
 
 
 class OntologyId(NamedObjectId):
     pass
@@ -180,243 +159,174 @@
 
 class SubsetId(AnnotationPropertyId):
     pass
 
 
 Any = Any
 
-
 class AnnotationPropertyMixin(YAMLRoot):
     """
     Groups all annotation property bundles
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.AnnotationPropertyMixin
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["AnnotationPropertyMixin"]
     class_class_curie: ClassVar[str] = "omoschema:AnnotationPropertyMixin"
     class_name: ClassVar[str] = "AnnotationPropertyMixin"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.AnnotationPropertyMixin
 
 
 @dataclass
 class HasMinimalMetadata(AnnotationPropertyMixin):
     """
     Absolute minimum metadata model
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasMinimalMetadata
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasMinimalMetadata"]
     class_class_curie: ClassVar[str] = "omoschema:HasMinimalMetadata"
     class_name: ClassVar[str] = "HasMinimalMetadata"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasMinimalMetadata
 
     label: Optional[Union[str, LabelType]] = None
-    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.label is not None and not isinstance(self.label, LabelType):
             self.label = LabelType(self.label)
 
         if not isinstance(self.definition, list):
             self.definition = [self.definition] if self.definition is not None else []
-        self.definition = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition
-        ]
+        self.definition = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasSynonyms(AnnotationPropertyMixin):
     """
     a mixin for a class whose members can have synonyms
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasSynonyms
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasSynonyms"]
     class_class_curie: ClassVar[str] = "omoschema:HasSynonyms"
     class_name: ClassVar[str] = "HasSynonyms"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasSynonyms
 
-    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_narrow_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_broad_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_related_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
+    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_narrow_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_broad_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_related_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
     alternative_term: Optional[Union[str, List[str]]] = empty_list()
     ISA_alternative_term: Optional[Union[str, List[str]]] = empty_list()
     IEDB_alternative_term: Optional[Union[str, List[str]]] = empty_list()
     editor_preferred_term: Optional[Union[str, List[str]]] = empty_list()
     OBO_foundry_unique_label: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.has_exact_synonym, list):
-            self.has_exact_synonym = (
-                [self.has_exact_synonym] if self.has_exact_synonym is not None else []
-            )
-        self.has_exact_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym
-        ]
+            self.has_exact_synonym = [self.has_exact_synonym] if self.has_exact_synonym is not None else []
+        self.has_exact_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym]
 
         if not isinstance(self.has_narrow_synonym, list):
-            self.has_narrow_synonym = (
-                [self.has_narrow_synonym] if self.has_narrow_synonym is not None else []
-            )
-        self.has_narrow_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_narrow_synonym
-        ]
+            self.has_narrow_synonym = [self.has_narrow_synonym] if self.has_narrow_synonym is not None else []
+        self.has_narrow_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_narrow_synonym]
 
         if not isinstance(self.has_broad_synonym, list):
-            self.has_broad_synonym = (
-                [self.has_broad_synonym] if self.has_broad_synonym is not None else []
-            )
-        self.has_broad_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_broad_synonym
-        ]
+            self.has_broad_synonym = [self.has_broad_synonym] if self.has_broad_synonym is not None else []
+        self.has_broad_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_broad_synonym]
 
         if not isinstance(self.has_related_synonym, list):
-            self.has_related_synonym = (
-                [self.has_related_synonym] if self.has_related_synonym is not None else []
-            )
-        self.has_related_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_related_synonym
-        ]
+            self.has_related_synonym = [self.has_related_synonym] if self.has_related_synonym is not None else []
+        self.has_related_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_related_synonym]
 
         if not isinstance(self.alternative_term, list):
-            self.alternative_term = (
-                [self.alternative_term] if self.alternative_term is not None else []
-            )
+            self.alternative_term = [self.alternative_term] if self.alternative_term is not None else []
         self.alternative_term = [v if isinstance(v, str) else str(v) for v in self.alternative_term]
 
         if not isinstance(self.ISA_alternative_term, list):
-            self.ISA_alternative_term = (
-                [self.ISA_alternative_term] if self.ISA_alternative_term is not None else []
-            )
-        self.ISA_alternative_term = [
-            v if isinstance(v, str) else str(v) for v in self.ISA_alternative_term
-        ]
+            self.ISA_alternative_term = [self.ISA_alternative_term] if self.ISA_alternative_term is not None else []
+        self.ISA_alternative_term = [v if isinstance(v, str) else str(v) for v in self.ISA_alternative_term]
 
         if not isinstance(self.IEDB_alternative_term, list):
-            self.IEDB_alternative_term = (
-                [self.IEDB_alternative_term] if self.IEDB_alternative_term is not None else []
-            )
-        self.IEDB_alternative_term = [
-            v if isinstance(v, str) else str(v) for v in self.IEDB_alternative_term
-        ]
+            self.IEDB_alternative_term = [self.IEDB_alternative_term] if self.IEDB_alternative_term is not None else []
+        self.IEDB_alternative_term = [v if isinstance(v, str) else str(v) for v in self.IEDB_alternative_term]
 
         if not isinstance(self.editor_preferred_term, list):
-            self.editor_preferred_term = (
-                [self.editor_preferred_term] if self.editor_preferred_term is not None else []
-            )
-        self.editor_preferred_term = [
-            v if isinstance(v, str) else str(v) for v in self.editor_preferred_term
-        ]
+            self.editor_preferred_term = [self.editor_preferred_term] if self.editor_preferred_term is not None else []
+        self.editor_preferred_term = [v if isinstance(v, str) else str(v) for v in self.editor_preferred_term]
 
         if not isinstance(self.OBO_foundry_unique_label, list):
-            self.OBO_foundry_unique_label = (
-                [self.OBO_foundry_unique_label] if self.OBO_foundry_unique_label is not None else []
-            )
-        self.OBO_foundry_unique_label = [
-            v if isinstance(v, str) else str(v) for v in self.OBO_foundry_unique_label
-        ]
+            self.OBO_foundry_unique_label = [self.OBO_foundry_unique_label] if self.OBO_foundry_unique_label is not None else []
+        self.OBO_foundry_unique_label = [v if isinstance(v, str) else str(v) for v in self.OBO_foundry_unique_label]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasMappings(AnnotationPropertyMixin):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasMappings
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasMappings"]
     class_class_curie: ClassVar[str] = "omoschema:HasMappings"
     class_name: ClassVar[str] = "HasMappings"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasMappings
 
     broadMatch: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
     closeMatch: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
     exactMatch: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
     narrowMatch: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
-    database_cross_reference: Optional[
-        Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]
-    ] = empty_list()
+    database_cross_reference: Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.broadMatch, list):
             self.broadMatch = [self.broadMatch] if self.broadMatch is not None else []
-        self.broadMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.broadMatch
-        ]
+        self.broadMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.broadMatch]
 
         if not isinstance(self.closeMatch, list):
             self.closeMatch = [self.closeMatch] if self.closeMatch is not None else []
-        self.closeMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.closeMatch
-        ]
+        self.closeMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.closeMatch]
 
         if not isinstance(self.exactMatch, list):
             self.exactMatch = [self.exactMatch] if self.exactMatch is not None else []
-        self.exactMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.exactMatch
-        ]
+        self.exactMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.exactMatch]
 
         if not isinstance(self.narrowMatch, list):
             self.narrowMatch = [self.narrowMatch] if self.narrowMatch is not None else []
-        self.narrowMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.narrowMatch
-        ]
+        self.narrowMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.narrowMatch]
 
         if not isinstance(self.database_cross_reference, list):
-            self.database_cross_reference = (
-                [self.database_cross_reference] if self.database_cross_reference is not None else []
-            )
-        self.database_cross_reference = [
-            v if isinstance(v, CURIELiteral) else CURIELiteral(v)
-            for v in self.database_cross_reference
-        ]
+            self.database_cross_reference = [self.database_cross_reference] if self.database_cross_reference is not None else []
+        self.database_cross_reference = [v if isinstance(v, CURIELiteral) else CURIELiteral(v) for v in self.database_cross_reference]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasProvenance(AnnotationPropertyMixin):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasProvenance
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasProvenance"]
     class_class_curie: ClassVar[str] = "omoschema:HasProvenance"
     class_name: ClassVar[str] = "HasProvenance"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasProvenance
 
     created_by: Optional[str] = None
     creation_date: Optional[Union[str, List[str]]] = empty_list()
     contributor: Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]] = empty_list()
     creator: Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]] = empty_list()
     created: Optional[str] = None
     date: Optional[Union[str, List[str]]] = empty_list()
     isDefinedBy: Optional[Union[str, OntologyId]] = None
-    editor_note: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    editor_note: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
     term_editor: Optional[Union[str, List[str]]] = empty_list()
     definition_source: Optional[Union[str, List[str]]] = empty_list()
     ontology_term_requester: Optional[str] = None
-    imported_from: Optional[
-        Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]
-    ] = empty_list()
+    imported_from: Optional[Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]] = empty_list()
     term_tracker_item: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.created_by is not None and not isinstance(self.created_by, str):
             self.created_by = str(self.created_by)
 
         if not isinstance(self.creation_date, list):
@@ -439,162 +349,123 @@
         self.date = [v if isinstance(v, str) else str(v) for v in self.date]
 
         if self.isDefinedBy is not None and not isinstance(self.isDefinedBy, OntologyId):
             self.isDefinedBy = OntologyId(self.isDefinedBy)
 
         if not isinstance(self.editor_note, list):
             self.editor_note = [self.editor_note] if self.editor_note is not None else []
-        self.editor_note = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.editor_note
-        ]
+        self.editor_note = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.editor_note]
 
         if not isinstance(self.term_editor, list):
             self.term_editor = [self.term_editor] if self.term_editor is not None else []
         self.term_editor = [v if isinstance(v, str) else str(v) for v in self.term_editor]
 
         if not isinstance(self.definition_source, list):
-            self.definition_source = (
-                [self.definition_source] if self.definition_source is not None else []
-            )
-        self.definition_source = [
-            v if isinstance(v, str) else str(v) for v in self.definition_source
-        ]
-
-        if self.ontology_term_requester is not None and not isinstance(
-            self.ontology_term_requester, str
-        ):
+            self.definition_source = [self.definition_source] if self.definition_source is not None else []
+        self.definition_source = [v if isinstance(v, str) else str(v) for v in self.definition_source]
+
+        if self.ontology_term_requester is not None and not isinstance(self.ontology_term_requester, str):
             self.ontology_term_requester = str(self.ontology_term_requester)
 
         if not isinstance(self.imported_from, list):
             self.imported_from = [self.imported_from] if self.imported_from is not None else []
-        self.imported_from = [
-            v if isinstance(v, NamedIndividualId) else NamedIndividualId(v)
-            for v in self.imported_from
-        ]
+        self.imported_from = [v if isinstance(v, NamedIndividualId) else NamedIndividualId(v) for v in self.imported_from]
 
         if not isinstance(self.term_tracker_item, list):
-            self.term_tracker_item = (
-                [self.term_tracker_item] if self.term_tracker_item is not None else []
-            )
-        self.term_tracker_item = [
-            v if isinstance(v, str) else str(v) for v in self.term_tracker_item
-        ]
+            self.term_tracker_item = [self.term_tracker_item] if self.term_tracker_item is not None else []
+        self.term_tracker_item = [v if isinstance(v, str) else str(v) for v in self.term_tracker_item]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasLifeCycle(AnnotationPropertyMixin):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasLifeCycle
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasLifeCycle"]
     class_class_curie: ClassVar[str] = "omoschema:HasLifeCycle"
     class_name: ClassVar[str] = "HasLifeCycle"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasLifeCycle
 
     deprecated: Optional[Union[bool, Bool]] = None
     has_obsolescence_reason: Optional[str] = None
     term_replaced_by: Optional[Union[dict, Any]] = None
     consider: Optional[Union[Union[dict, Any], List[Union[dict, Any]]]] = empty_list()
-    has_alternative_id: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = (
-        empty_list()
-    )
+    has_alternative_id: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = empty_list()
     excluded_from_QC_check: Optional[Union[dict, "Thing"]] = None
-    excluded_subClassOf: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = (
-        empty_list()
-    )
+    excluded_subClassOf: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     excluded_synonym: Optional[Union[str, List[str]]] = empty_list()
     should_conform_to: Optional[Union[dict, "Thing"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.deprecated is not None and not isinstance(self.deprecated, Bool):
             self.deprecated = Bool(self.deprecated)
 
-        if self.has_obsolescence_reason is not None and not isinstance(
-            self.has_obsolescence_reason, str
-        ):
+        if self.has_obsolescence_reason is not None and not isinstance(self.has_obsolescence_reason, str):
             self.has_obsolescence_reason = str(self.has_obsolescence_reason)
 
         if not isinstance(self.has_alternative_id, list):
-            self.has_alternative_id = (
-                [self.has_alternative_id] if self.has_alternative_id is not None else []
-            )
-        self.has_alternative_id = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.has_alternative_id
-        ]
-
-        if self.excluded_from_QC_check is not None and not isinstance(
-            self.excluded_from_QC_check, Thing
-        ):
+            self.has_alternative_id = [self.has_alternative_id] if self.has_alternative_id is not None else []
+        self.has_alternative_id = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.has_alternative_id]
+
+        if self.excluded_from_QC_check is not None and not isinstance(self.excluded_from_QC_check, Thing):
             self.excluded_from_QC_check = Thing(**as_dict(self.excluded_from_QC_check))
 
         if not isinstance(self.excluded_subClassOf, list):
-            self.excluded_subClassOf = (
-                [self.excluded_subClassOf] if self.excluded_subClassOf is not None else []
-            )
-        self.excluded_subClassOf = [
-            v if isinstance(v, ClassId) else ClassId(v) for v in self.excluded_subClassOf
-        ]
+            self.excluded_subClassOf = [self.excluded_subClassOf] if self.excluded_subClassOf is not None else []
+        self.excluded_subClassOf = [v if isinstance(v, ClassId) else ClassId(v) for v in self.excluded_subClassOf]
 
         if not isinstance(self.excluded_synonym, list):
-            self.excluded_synonym = (
-                [self.excluded_synonym] if self.excluded_synonym is not None else []
-            )
+            self.excluded_synonym = [self.excluded_synonym] if self.excluded_synonym is not None else []
         self.excluded_synonym = [v if isinstance(v, str) else str(v) for v in self.excluded_synonym]
 
         if self.should_conform_to is not None and not isinstance(self.should_conform_to, Thing):
             self.should_conform_to = Thing(**as_dict(self.should_conform_to))
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasCategory(AnnotationPropertyMixin):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasCategory
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasCategory"]
     class_class_curie: ClassVar[str] = "omoschema:HasCategory"
     class_name: ClassVar[str] = "HasCategory"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasCategory
 
     has_obo_namespace: Optional[Union[str, List[str]]] = empty_list()
     category: Optional[str] = None
     in_subset: Optional[Union[Union[str, SubsetId], List[Union[str, SubsetId]]]] = empty_list()
     conformsTo: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.has_obo_namespace, list):
-            self.has_obo_namespace = (
-                [self.has_obo_namespace] if self.has_obo_namespace is not None else []
-            )
-        self.has_obo_namespace = [
-            v if isinstance(v, str) else str(v) for v in self.has_obo_namespace
-        ]
+            self.has_obo_namespace = [self.has_obo_namespace] if self.has_obo_namespace is not None else []
+        self.has_obo_namespace = [v if isinstance(v, str) else str(v) for v in self.has_obo_namespace]
 
         if self.category is not None and not isinstance(self.category, str):
             self.category = str(self.category)
 
         if not isinstance(self.in_subset, list):
             self.in_subset = [self.in_subset] if self.in_subset is not None else []
         self.in_subset = [v if isinstance(v, SubsetId) else SubsetId(v) for v in self.in_subset]
 
         if not isinstance(self.conformsTo, list):
             self.conformsTo = [self.conformsTo] if self.conformsTo is not None else []
-        self.conformsTo = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.conformsTo
-        ]
+        self.conformsTo = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.conformsTo]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class HasUserInformation(AnnotationPropertyMixin):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.HasUserInformation
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["HasUserInformation"]
     class_class_curie: ClassVar[str] = "omoschema:HasUserInformation"
     class_name: ClassVar[str] = "HasUserInformation"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HasUserInformation
 
     comment: Optional[Union[str, List[str]]] = empty_list()
     seeAlso: Optional[Union[Union[dict, "Thing"], List[Union[dict, "Thing"]]]] = empty_list()
     image: Optional[Union[dict, "Thing"]] = None
@@ -613,17 +484,15 @@
             self.seeAlso = [self.seeAlso] if self.seeAlso is not None else []
         self.seeAlso = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.seeAlso]
 
         if self.image is not None and not isinstance(self.image, Thing):
             self.image = Thing(**as_dict(self.image))
 
         if not isinstance(self.example_of_usage, list):
-            self.example_of_usage = (
-                [self.example_of_usage] if self.example_of_usage is not None else []
-            )
+            self.example_of_usage = [self.example_of_usage] if self.example_of_usage is not None else []
         self.example_of_usage = [v if isinstance(v, str) else str(v) for v in self.example_of_usage]
 
         if not isinstance(self.curator_note, list):
             self.curator_note = [self.curator_note] if self.curator_note is not None else []
         self.curator_note = [v if isinstance(v, str) else str(v) for v in self.curator_note]
 
         if self.has_curation_status is not None and not isinstance(self.has_curation_status, str):
@@ -640,74 +509,98 @@
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Thing(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.Thing
+    class_class_uri: ClassVar[URIRef] = OWL["Thing"]
     class_class_curie: ClassVar[str] = "owl:Thing"
     class_name: ClassVar[str] = "Thing"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Thing
 
     type: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.type, list):
             self.type = [self.type] if self.type is not None else []
         self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
         super().__post_init__(**kwargs)
 
 
+    def __new__(cls, *args, **kwargs):
+
+        type_designator = "type"
+        if not type_designator in kwargs:
+            return super().__new__(cls,*args,**kwargs)
+        else:
+            type_designator_value = kwargs[type_designator]
+            target_cls = cls._class_for("class_class_curie", type_designator_value)
+
+
+            if target_cls is None:
+                target_cls = cls._class_for("class_class_uri", type_designator_value)
+
+
+            if target_cls is None:
+                target_cls = cls._class_for("class_model_uri", type_designator_value)
+
+
+            if target_cls is None:
+                raise ValueError(f"Wrong type designator value: class {cls.__name__} "
+                                 f"has no subclass with ['class_class_curie', 'class_class_uri', 'class_model_uri']='{kwargs[type_designator]}'")
+            return super().__new__(target_cls,*args,**kwargs)
+
+
+
 @dataclass
 class NamedObject(Thing):
     """
     Anything with an IRI
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.NamedObject
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["NamedObject"]
     class_class_curie: ClassVar[str] = "omoschema:NamedObject"
     class_name: ClassVar[str] = "NamedObject"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.NamedObject
 
     id: Union[str, NamedObjectId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NamedObjectId):
             self.id = NamedObjectId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Ontology(NamedObject):
     """
     An OWL ontology
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.Ontology
+    class_class_uri: ClassVar[URIRef] = OWL["Ontology"]
     class_class_curie: ClassVar[str] = "owl:Ontology"
     class_name: ClassVar[str] = "Ontology"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Ontology
 
     id: Union[str, OntologyId] = None
     title: Union[str, NarrativeText] = None
     license: Union[dict, Thing] = None
     versionIRI: Union[str, URIorCURIE] = None
     versionInfo: str = None
-    has_ontology_root_term: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = (
-        empty_list()
-    )
+    has_ontology_root_term: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     source: Optional[Union[str, List[str]]] = empty_list()
     comment: Optional[Union[str, List[str]]] = empty_list()
     creator: Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]] = empty_list()
     created: Optional[str] = None
     imports: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -733,20 +626,16 @@
 
         if self._is_empty(self.versionInfo):
             self.MissingRequiredField("versionInfo")
         if not isinstance(self.versionInfo, str):
             self.versionInfo = str(self.versionInfo)
 
         if not isinstance(self.has_ontology_root_term, list):
-            self.has_ontology_root_term = (
-                [self.has_ontology_root_term] if self.has_ontology_root_term is not None else []
-            )
-        self.has_ontology_root_term = [
-            v if isinstance(v, ClassId) else ClassId(v) for v in self.has_ontology_root_term
-        ]
+            self.has_ontology_root_term = [self.has_ontology_root_term] if self.has_ontology_root_term is not None else []
+        self.has_ontology_root_term = [v if isinstance(v, ClassId) else ClassId(v) for v in self.has_ontology_root_term]
 
         if not isinstance(self.source, list):
             self.source = [self.source] if self.source is not None else []
         self.source = [v if isinstance(v, str) else str(v) for v in self.source]
 
         if not isinstance(self.comment, list):
             self.comment = [self.comment] if self.comment is not None else []
@@ -759,205 +648,139 @@
         if self.created is not None and not isinstance(self.created, str):
             self.created = str(self.created)
 
         if self.imports is not None and not isinstance(self.imports, str):
             self.imports = str(self.imports)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Term(NamedObject):
     """
     A NamedThing that includes classes, properties, but not ontologies
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.Term
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["Term"]
     class_class_curie: ClassVar[str] = "omoschema:Term"
     class_name: ClassVar[str] = "Term"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Term
 
     id: Union[str, TermId] = None
-    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_narrow_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_broad_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_related_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
+    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_narrow_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_broad_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_related_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
     alternative_term: Optional[Union[str, List[str]]] = empty_list()
     ISA_alternative_term: Optional[Union[str, List[str]]] = empty_list()
     IEDB_alternative_term: Optional[Union[str, List[str]]] = empty_list()
     editor_preferred_term: Optional[Union[str, List[str]]] = empty_list()
     OBO_foundry_unique_label: Optional[Union[str, List[str]]] = empty_list()
     deprecated: Optional[Union[bool, Bool]] = None
     has_obsolescence_reason: Optional[str] = None
     term_replaced_by: Optional[Union[dict, Any]] = None
     consider: Optional[Union[Union[dict, Any], List[Union[dict, Any]]]] = empty_list()
-    has_alternative_id: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = (
-        empty_list()
-    )
+    has_alternative_id: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = empty_list()
     excluded_from_QC_check: Optional[Union[dict, Thing]] = None
-    excluded_subClassOf: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = (
-        empty_list()
-    )
+    excluded_subClassOf: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     excluded_synonym: Optional[Union[str, List[str]]] = empty_list()
     should_conform_to: Optional[Union[dict, Thing]] = None
     created_by: Optional[str] = None
     creation_date: Optional[Union[str, List[str]]] = empty_list()
     contributor: Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]] = empty_list()
     creator: Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]] = empty_list()
     created: Optional[str] = None
     date: Optional[Union[str, List[str]]] = empty_list()
     isDefinedBy: Optional[Union[str, OntologyId]] = None
-    editor_note: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    editor_note: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
     term_editor: Optional[Union[str, List[str]]] = empty_list()
     definition_source: Optional[Union[str, List[str]]] = empty_list()
     ontology_term_requester: Optional[str] = None
-    imported_from: Optional[
-        Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]
-    ] = empty_list()
+    imported_from: Optional[Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]] = empty_list()
     term_tracker_item: Optional[Union[str, List[str]]] = empty_list()
     broadMatch: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
     closeMatch: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
     exactMatch: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
     narrowMatch: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
-    database_cross_reference: Optional[
-        Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]
-    ] = empty_list()
+    database_cross_reference: Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]] = empty_list()
     has_obo_namespace: Optional[Union[str, List[str]]] = empty_list()
     category: Optional[str] = None
     in_subset: Optional[Union[Union[str, SubsetId], List[Union[str, SubsetId]]]] = empty_list()
     conformsTo: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
     comment: Optional[Union[str, List[str]]] = empty_list()
     seeAlso: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
     image: Optional[Union[dict, Thing]] = None
     example_of_usage: Optional[Union[str, List[str]]] = empty_list()
     curator_note: Optional[Union[str, List[str]]] = empty_list()
     has_curation_status: Optional[str] = None
     depicted_by: Optional[Union[Union[str, ImageId], List[Union[str, ImageId]]]] = empty_list()
     page: Optional[Union[str, List[str]]] = empty_list()
     label: Optional[Union[str, LabelType]] = None
-    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.has_exact_synonym, list):
-            self.has_exact_synonym = (
-                [self.has_exact_synonym] if self.has_exact_synonym is not None else []
-            )
-        self.has_exact_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym
-        ]
+            self.has_exact_synonym = [self.has_exact_synonym] if self.has_exact_synonym is not None else []
+        self.has_exact_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym]
 
         if not isinstance(self.has_narrow_synonym, list):
-            self.has_narrow_synonym = (
-                [self.has_narrow_synonym] if self.has_narrow_synonym is not None else []
-            )
-        self.has_narrow_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_narrow_synonym
-        ]
+            self.has_narrow_synonym = [self.has_narrow_synonym] if self.has_narrow_synonym is not None else []
+        self.has_narrow_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_narrow_synonym]
 
         if not isinstance(self.has_broad_synonym, list):
-            self.has_broad_synonym = (
-                [self.has_broad_synonym] if self.has_broad_synonym is not None else []
-            )
-        self.has_broad_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_broad_synonym
-        ]
+            self.has_broad_synonym = [self.has_broad_synonym] if self.has_broad_synonym is not None else []
+        self.has_broad_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_broad_synonym]
 
         if not isinstance(self.has_related_synonym, list):
-            self.has_related_synonym = (
-                [self.has_related_synonym] if self.has_related_synonym is not None else []
-            )
-        self.has_related_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_related_synonym
-        ]
+            self.has_related_synonym = [self.has_related_synonym] if self.has_related_synonym is not None else []
+        self.has_related_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_related_synonym]
 
         if not isinstance(self.alternative_term, list):
-            self.alternative_term = (
-                [self.alternative_term] if self.alternative_term is not None else []
-            )
+            self.alternative_term = [self.alternative_term] if self.alternative_term is not None else []
         self.alternative_term = [v if isinstance(v, str) else str(v) for v in self.alternative_term]
 
         if not isinstance(self.ISA_alternative_term, list):
-            self.ISA_alternative_term = (
-                [self.ISA_alternative_term] if self.ISA_alternative_term is not None else []
-            )
-        self.ISA_alternative_term = [
-            v if isinstance(v, str) else str(v) for v in self.ISA_alternative_term
-        ]
+            self.ISA_alternative_term = [self.ISA_alternative_term] if self.ISA_alternative_term is not None else []
+        self.ISA_alternative_term = [v if isinstance(v, str) else str(v) for v in self.ISA_alternative_term]
 
         if not isinstance(self.IEDB_alternative_term, list):
-            self.IEDB_alternative_term = (
-                [self.IEDB_alternative_term] if self.IEDB_alternative_term is not None else []
-            )
-        self.IEDB_alternative_term = [
-            v if isinstance(v, str) else str(v) for v in self.IEDB_alternative_term
-        ]
+            self.IEDB_alternative_term = [self.IEDB_alternative_term] if self.IEDB_alternative_term is not None else []
+        self.IEDB_alternative_term = [v if isinstance(v, str) else str(v) for v in self.IEDB_alternative_term]
 
         if not isinstance(self.editor_preferred_term, list):
-            self.editor_preferred_term = (
-                [self.editor_preferred_term] if self.editor_preferred_term is not None else []
-            )
-        self.editor_preferred_term = [
-            v if isinstance(v, str) else str(v) for v in self.editor_preferred_term
-        ]
+            self.editor_preferred_term = [self.editor_preferred_term] if self.editor_preferred_term is not None else []
+        self.editor_preferred_term = [v if isinstance(v, str) else str(v) for v in self.editor_preferred_term]
 
         if not isinstance(self.OBO_foundry_unique_label, list):
-            self.OBO_foundry_unique_label = (
-                [self.OBO_foundry_unique_label] if self.OBO_foundry_unique_label is not None else []
-            )
-        self.OBO_foundry_unique_label = [
-            v if isinstance(v, str) else str(v) for v in self.OBO_foundry_unique_label
-        ]
+            self.OBO_foundry_unique_label = [self.OBO_foundry_unique_label] if self.OBO_foundry_unique_label is not None else []
+        self.OBO_foundry_unique_label = [v if isinstance(v, str) else str(v) for v in self.OBO_foundry_unique_label]
 
         if self.deprecated is not None and not isinstance(self.deprecated, Bool):
             self.deprecated = Bool(self.deprecated)
 
-        if self.has_obsolescence_reason is not None and not isinstance(
-            self.has_obsolescence_reason, str
-        ):
+        if self.has_obsolescence_reason is not None and not isinstance(self.has_obsolescence_reason, str):
             self.has_obsolescence_reason = str(self.has_obsolescence_reason)
 
         if not isinstance(self.has_alternative_id, list):
-            self.has_alternative_id = (
-                [self.has_alternative_id] if self.has_alternative_id is not None else []
-            )
-        self.has_alternative_id = [
-            v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.has_alternative_id
-        ]
-
-        if self.excluded_from_QC_check is not None and not isinstance(
-            self.excluded_from_QC_check, Thing
-        ):
+            self.has_alternative_id = [self.has_alternative_id] if self.has_alternative_id is not None else []
+        self.has_alternative_id = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.has_alternative_id]
+
+        if self.excluded_from_QC_check is not None and not isinstance(self.excluded_from_QC_check, Thing):
             self.excluded_from_QC_check = Thing(**as_dict(self.excluded_from_QC_check))
 
         if not isinstance(self.excluded_subClassOf, list):
-            self.excluded_subClassOf = (
-                [self.excluded_subClassOf] if self.excluded_subClassOf is not None else []
-            )
-        self.excluded_subClassOf = [
-            v if isinstance(v, ClassId) else ClassId(v) for v in self.excluded_subClassOf
-        ]
+            self.excluded_subClassOf = [self.excluded_subClassOf] if self.excluded_subClassOf is not None else []
+        self.excluded_subClassOf = [v if isinstance(v, ClassId) else ClassId(v) for v in self.excluded_subClassOf]
 
         if not isinstance(self.excluded_synonym, list):
-            self.excluded_synonym = (
-                [self.excluded_synonym] if self.excluded_synonym is not None else []
-            )
+            self.excluded_synonym = [self.excluded_synonym] if self.excluded_synonym is not None else []
         self.excluded_synonym = [v if isinstance(v, str) else str(v) for v in self.excluded_synonym]
 
         if self.should_conform_to is not None and not isinstance(self.should_conform_to, Thing):
             self.should_conform_to = Thing(**as_dict(self.should_conform_to))
 
         if self.created_by is not None and not isinstance(self.created_by, str):
             self.created_by = str(self.created_by)
@@ -982,119 +805,83 @@
         self.date = [v if isinstance(v, str) else str(v) for v in self.date]
 
         if self.isDefinedBy is not None and not isinstance(self.isDefinedBy, OntologyId):
             self.isDefinedBy = OntologyId(self.isDefinedBy)
 
         if not isinstance(self.editor_note, list):
             self.editor_note = [self.editor_note] if self.editor_note is not None else []
-        self.editor_note = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.editor_note
-        ]
+        self.editor_note = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.editor_note]
 
         if not isinstance(self.term_editor, list):
             self.term_editor = [self.term_editor] if self.term_editor is not None else []
         self.term_editor = [v if isinstance(v, str) else str(v) for v in self.term_editor]
 
         if not isinstance(self.definition_source, list):
-            self.definition_source = (
-                [self.definition_source] if self.definition_source is not None else []
-            )
-        self.definition_source = [
-            v if isinstance(v, str) else str(v) for v in self.definition_source
-        ]
-
-        if self.ontology_term_requester is not None and not isinstance(
-            self.ontology_term_requester, str
-        ):
+            self.definition_source = [self.definition_source] if self.definition_source is not None else []
+        self.definition_source = [v if isinstance(v, str) else str(v) for v in self.definition_source]
+
+        if self.ontology_term_requester is not None and not isinstance(self.ontology_term_requester, str):
             self.ontology_term_requester = str(self.ontology_term_requester)
 
         if not isinstance(self.imported_from, list):
             self.imported_from = [self.imported_from] if self.imported_from is not None else []
-        self.imported_from = [
-            v if isinstance(v, NamedIndividualId) else NamedIndividualId(v)
-            for v in self.imported_from
-        ]
+        self.imported_from = [v if isinstance(v, NamedIndividualId) else NamedIndividualId(v) for v in self.imported_from]
 
         if not isinstance(self.term_tracker_item, list):
-            self.term_tracker_item = (
-                [self.term_tracker_item] if self.term_tracker_item is not None else []
-            )
-        self.term_tracker_item = [
-            v if isinstance(v, str) else str(v) for v in self.term_tracker_item
-        ]
+            self.term_tracker_item = [self.term_tracker_item] if self.term_tracker_item is not None else []
+        self.term_tracker_item = [v if isinstance(v, str) else str(v) for v in self.term_tracker_item]
 
         if not isinstance(self.broadMatch, list):
             self.broadMatch = [self.broadMatch] if self.broadMatch is not None else []
-        self.broadMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.broadMatch
-        ]
+        self.broadMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.broadMatch]
 
         if not isinstance(self.closeMatch, list):
             self.closeMatch = [self.closeMatch] if self.closeMatch is not None else []
-        self.closeMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.closeMatch
-        ]
+        self.closeMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.closeMatch]
 
         if not isinstance(self.exactMatch, list):
             self.exactMatch = [self.exactMatch] if self.exactMatch is not None else []
-        self.exactMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.exactMatch
-        ]
+        self.exactMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.exactMatch]
 
         if not isinstance(self.narrowMatch, list):
             self.narrowMatch = [self.narrowMatch] if self.narrowMatch is not None else []
-        self.narrowMatch = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.narrowMatch
-        ]
+        self.narrowMatch = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.narrowMatch]
 
         if not isinstance(self.database_cross_reference, list):
-            self.database_cross_reference = (
-                [self.database_cross_reference] if self.database_cross_reference is not None else []
-            )
-        self.database_cross_reference = [
-            v if isinstance(v, CURIELiteral) else CURIELiteral(v)
-            for v in self.database_cross_reference
-        ]
+            self.database_cross_reference = [self.database_cross_reference] if self.database_cross_reference is not None else []
+        self.database_cross_reference = [v if isinstance(v, CURIELiteral) else CURIELiteral(v) for v in self.database_cross_reference]
 
         if not isinstance(self.has_obo_namespace, list):
-            self.has_obo_namespace = (
-                [self.has_obo_namespace] if self.has_obo_namespace is not None else []
-            )
-        self.has_obo_namespace = [
-            v if isinstance(v, str) else str(v) for v in self.has_obo_namespace
-        ]
+            self.has_obo_namespace = [self.has_obo_namespace] if self.has_obo_namespace is not None else []
+        self.has_obo_namespace = [v if isinstance(v, str) else str(v) for v in self.has_obo_namespace]
 
         if self.category is not None and not isinstance(self.category, str):
             self.category = str(self.category)
 
         if not isinstance(self.in_subset, list):
             self.in_subset = [self.in_subset] if self.in_subset is not None else []
         self.in_subset = [v if isinstance(v, SubsetId) else SubsetId(v) for v in self.in_subset]
 
         if not isinstance(self.conformsTo, list):
             self.conformsTo = [self.conformsTo] if self.conformsTo is not None else []
-        self.conformsTo = [
-            v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.conformsTo
-        ]
+        self.conformsTo = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.conformsTo]
 
         if not isinstance(self.comment, list):
             self.comment = [self.comment] if self.comment is not None else []
         self.comment = [v if isinstance(v, str) else str(v) for v in self.comment]
 
         if not isinstance(self.seeAlso, list):
             self.seeAlso = [self.seeAlso] if self.seeAlso is not None else []
         self.seeAlso = [v if isinstance(v, Thing) else Thing(**as_dict(v)) for v in self.seeAlso]
 
         if self.image is not None and not isinstance(self.image, Thing):
             self.image = Thing(**as_dict(self.image))
 
         if not isinstance(self.example_of_usage, list):
-            self.example_of_usage = (
-                [self.example_of_usage] if self.example_of_usage is not None else []
-            )
+            self.example_of_usage = [self.example_of_usage] if self.example_of_usage is not None else []
         self.example_of_usage = [v if isinstance(v, str) else str(v) for v in self.example_of_usage]
 
         if not isinstance(self.curator_note, list):
             self.curator_note = [self.curator_note] if self.curator_note is not None else []
         self.curator_note = [v if isinstance(v, str) else str(v) for v in self.curator_note]
 
         if self.has_curation_status is not None and not isinstance(self.has_curation_status, str):
@@ -1109,47 +896,44 @@
         self.page = [v if isinstance(v, str) else str(v) for v in self.page]
 
         if self.label is not None and not isinstance(self.label, LabelType):
             self.label = LabelType(self.label)
 
         if not isinstance(self.definition, list):
             self.definition = [self.definition] if self.definition is not None else []
-        self.definition = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition
-        ]
+        self.definition = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition]
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Class(Term):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.Class
+    class_class_uri: ClassVar[URIRef] = OWL["Class"]
     class_class_curie: ClassVar[str] = "owl:Class"
     class_name: ClassVar[str] = "Class"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Class
 
     id: Union[str, ClassId] = None
     label: Union[str, LabelType] = None
     never_in_taxon: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     disconnected_from: Optional[Union[str, ClassId]] = None
     has_rank: Optional[Union[dict, Thing]] = None
-    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
     broadMatch: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     exactMatch: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     narrowMatch: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     closeMatch: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     subClassOf: Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]] = empty_list()
     disjointWith: Optional[Union[str, List[str]]] = empty_list()
-    equivalentClass: Optional[
-        Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]
-    ] = empty_list()
+    equivalentClass: Optional[Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]] = empty_list()
     intersectionOf: Optional[Union[dict, "ClassExpression"]] = None
     cardinality: Optional[str] = None
     complementOf: Optional[str] = None
     oneOf: Optional[Union[dict, "ClassExpression"]] = None
     unionOf: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -1161,29 +945,25 @@
         if self._is_empty(self.label):
             self.MissingRequiredField("label")
         if not isinstance(self.label, LabelType):
             self.label = LabelType(self.label)
 
         if not isinstance(self.never_in_taxon, list):
             self.never_in_taxon = [self.never_in_taxon] if self.never_in_taxon is not None else []
-        self.never_in_taxon = [
-            v if isinstance(v, ClassId) else ClassId(v) for v in self.never_in_taxon
-        ]
+        self.never_in_taxon = [v if isinstance(v, ClassId) else ClassId(v) for v in self.never_in_taxon]
 
         if self.disconnected_from is not None and not isinstance(self.disconnected_from, ClassId):
             self.disconnected_from = ClassId(self.disconnected_from)
 
         if self.has_rank is not None and not isinstance(self.has_rank, Thing):
             self.has_rank = Thing(**as_dict(self.has_rank))
 
         if not isinstance(self.definition, list):
             self.definition = [self.definition] if self.definition is not None else []
-        self.definition = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition
-        ]
+        self.definition = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition]
 
         if not isinstance(self.broadMatch, list):
             self.broadMatch = [self.broadMatch] if self.broadMatch is not None else []
         self.broadMatch = [v if isinstance(v, ClassId) else ClassId(v) for v in self.broadMatch]
 
         if not isinstance(self.exactMatch, list):
             self.exactMatch = [self.exactMatch] if self.exactMatch is not None else []
@@ -1202,21 +982,16 @@
         self.subClassOf = [v if isinstance(v, ClassId) else ClassId(v) for v in self.subClassOf]
 
         if not isinstance(self.disjointWith, list):
             self.disjointWith = [self.disjointWith] if self.disjointWith is not None else []
         self.disjointWith = [v if isinstance(v, str) else str(v) for v in self.disjointWith]
 
         if not isinstance(self.equivalentClass, list):
-            self.equivalentClass = (
-                [self.equivalentClass] if self.equivalentClass is not None else []
-            )
-        self.equivalentClass = [
-            v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v))
-            for v in self.equivalentClass
-        ]
+            self.equivalentClass = [self.equivalentClass] if self.equivalentClass is not None else []
+        self.equivalentClass = [v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v)) for v in self.equivalentClass]
 
         if self.intersectionOf is not None and not isinstance(self.intersectionOf, ClassExpression):
             self.intersectionOf = ClassExpression(**as_dict(self.intersectionOf))
 
         if self.cardinality is not None and not isinstance(self.cardinality, str):
             self.cardinality = str(self.cardinality)
 
@@ -1226,39 +1001,38 @@
         if self.oneOf is not None and not isinstance(self.oneOf, ClassExpression):
             self.oneOf = ClassExpression(**as_dict(self.oneOf))
 
         if self.unionOf is not None and not isinstance(self.unionOf, str):
             self.unionOf = str(self.unionOf)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Property(Term):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = RDF.Property
+    class_class_uri: ClassVar[URIRef] = RDF["Property"]
     class_class_curie: ClassVar[str] = "rdf:Property"
     class_name: ClassVar[str] = "Property"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Property
 
     id: Union[str, PropertyId] = None
     domain: Optional[Union[str, List[str]]] = empty_list()
     range: Optional[Union[str, List[str]]] = empty_list()
     is_class_level: Optional[Union[bool, Bool]] = None
     is_metadata_tag: Optional[Union[bool, Bool]] = None
     label: Optional[Union[str, LabelType]] = None
-    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = (
-        empty_list()
-    )
+    definition: Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]] = empty_list()
     broadMatch: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
     exactMatch: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
-    narrowMatch: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = (
-        empty_list()
-    )
+    narrowMatch: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
     closeMatch: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
     subClassOf: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.domain, list):
             self.domain = [self.domain] if self.domain is not None else []
         self.domain = [v if isinstance(v, str) else str(v) for v in self.domain]
@@ -1274,60 +1048,50 @@
             self.is_metadata_tag = Bool(self.is_metadata_tag)
 
         if self.label is not None and not isinstance(self.label, LabelType):
             self.label = LabelType(self.label)
 
         if not isinstance(self.definition, list):
             self.definition = [self.definition] if self.definition is not None else []
-        self.definition = [
-            v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition
-        ]
+        self.definition = [v if isinstance(v, NarrativeText) else NarrativeText(v) for v in self.definition]
 
         if not isinstance(self.broadMatch, list):
             self.broadMatch = [self.broadMatch] if self.broadMatch is not None else []
-        self.broadMatch = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.broadMatch
-        ]
+        self.broadMatch = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.broadMatch]
 
         if not isinstance(self.exactMatch, list):
             self.exactMatch = [self.exactMatch] if self.exactMatch is not None else []
-        self.exactMatch = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.exactMatch
-        ]
+        self.exactMatch = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.exactMatch]
 
         if not isinstance(self.narrowMatch, list):
             self.narrowMatch = [self.narrowMatch] if self.narrowMatch is not None else []
-        self.narrowMatch = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.narrowMatch
-        ]
+        self.narrowMatch = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.narrowMatch]
 
         if not isinstance(self.closeMatch, list):
             self.closeMatch = [self.closeMatch] if self.closeMatch is not None else []
-        self.closeMatch = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.closeMatch
-        ]
+        self.closeMatch = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.closeMatch]
 
         if not isinstance(self.subClassOf, list):
             self.subClassOf = [self.subClassOf] if self.subClassOf is not None else []
-        self.subClassOf = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.subClassOf
-        ]
+        self.subClassOf = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.subClassOf]
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class AnnotationProperty(Property):
     """
     A property used in non-logical axioms
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.AnnotationProperty
+    class_class_uri: ClassVar[URIRef] = OWL["AnnotationProperty"]
     class_class_curie: ClassVar[str] = "owl:AnnotationProperty"
     class_name: ClassVar[str] = "AnnotationProperty"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.AnnotationProperty
 
     id: Union[str, AnnotationPropertyId] = None
     shorthand: Optional[Union[str, List[str]]] = empty_list()
 
@@ -1338,142 +1102,138 @@
             self.id = AnnotationPropertyId(self.id)
 
         if not isinstance(self.shorthand, list):
             self.shorthand = [self.shorthand] if self.shorthand is not None else []
         self.shorthand = [v if isinstance(v, str) else str(v) for v in self.shorthand]
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class ObjectProperty(Property):
     """
     A property that connects two objects in logical axioms
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.ObjectProperty
+    class_class_uri: ClassVar[URIRef] = OWL["ObjectProperty"]
     class_class_curie: ClassVar[str] = "owl:ObjectProperty"
     class_name: ClassVar[str] = "ObjectProperty"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.ObjectProperty
 
     id: Union[str, ObjectPropertyId] = None
     temporal_interpretation: Optional[Union[str, NamedIndividualId]] = None
     is_cyclic: Optional[Union[bool, Bool]] = None
     is_transitive: Optional[Union[bool, Bool]] = None
     shorthand: Optional[Union[str, List[str]]] = empty_list()
-    equivalentProperty: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = (
-        empty_list()
-    )
+    equivalentProperty: Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]] = empty_list()
     inverseOf: Optional[Union[str, PropertyId]] = None
     propertyChainAxiom: Optional[Union[str, List[str]]] = empty_list()
     disjointWith: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ObjectPropertyId):
             self.id = ObjectPropertyId(self.id)
 
-        if self.temporal_interpretation is not None and not isinstance(
-            self.temporal_interpretation, NamedIndividualId
-        ):
+        if self.temporal_interpretation is not None and not isinstance(self.temporal_interpretation, NamedIndividualId):
             self.temporal_interpretation = NamedIndividualId(self.temporal_interpretation)
 
         if self.is_cyclic is not None and not isinstance(self.is_cyclic, Bool):
             self.is_cyclic = Bool(self.is_cyclic)
 
         if self.is_transitive is not None and not isinstance(self.is_transitive, Bool):
             self.is_transitive = Bool(self.is_transitive)
 
         if not isinstance(self.shorthand, list):
             self.shorthand = [self.shorthand] if self.shorthand is not None else []
         self.shorthand = [v if isinstance(v, str) else str(v) for v in self.shorthand]
 
         if not isinstance(self.equivalentProperty, list):
-            self.equivalentProperty = (
-                [self.equivalentProperty] if self.equivalentProperty is not None else []
-            )
-        self.equivalentProperty = [
-            v if isinstance(v, PropertyId) else PropertyId(v) for v in self.equivalentProperty
-        ]
+            self.equivalentProperty = [self.equivalentProperty] if self.equivalentProperty is not None else []
+        self.equivalentProperty = [v if isinstance(v, PropertyId) else PropertyId(v) for v in self.equivalentProperty]
 
         if self.inverseOf is not None and not isinstance(self.inverseOf, PropertyId):
             self.inverseOf = PropertyId(self.inverseOf)
 
         if not isinstance(self.propertyChainAxiom, list):
-            self.propertyChainAxiom = (
-                [self.propertyChainAxiom] if self.propertyChainAxiom is not None else []
-            )
-        self.propertyChainAxiom = [
-            v if isinstance(v, str) else str(v) for v in self.propertyChainAxiom
-        ]
+            self.propertyChainAxiom = [self.propertyChainAxiom] if self.propertyChainAxiom is not None else []
+        self.propertyChainAxiom = [v if isinstance(v, str) else str(v) for v in self.propertyChainAxiom]
 
         if not isinstance(self.disjointWith, list):
             self.disjointWith = [self.disjointWith] if self.disjointWith is not None else []
         self.disjointWith = [v if isinstance(v, str) else str(v) for v in self.disjointWith]
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class TransitiveProperty(ObjectProperty):
     """
     An ObjectProperty with the property of transitivity
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.TransitiveProperty
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["TransitiveProperty"]
     class_class_curie: ClassVar[str] = "omoschema:TransitiveProperty"
     class_name: ClassVar[str] = "TransitiveProperty"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.TransitiveProperty
 
     id: Union[str, TransitivePropertyId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, TransitivePropertyId):
             self.id = TransitivePropertyId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class NamedIndividual(Term):
     """
     An instance that has a IRI
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.NamedIndividual
+    class_class_uri: ClassVar[URIRef] = OWL["NamedIndividual"]
     class_class_curie: ClassVar[str] = "owl:NamedIndividual"
     class_name: ClassVar[str] = "NamedIndividual"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.NamedIndividual
 
     id: Union[str, NamedIndividualId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, NamedIndividualId):
             self.id = NamedIndividualId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class HomoSapiens(NamedIndividual):
     """
     An individual human being
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = NCBITAXON["9606"]
     class_class_curie: ClassVar[str] = "NCBITaxon:9606"
     class_name: ClassVar[str] = "HomoSapiens"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.HomoSapiens
 
@@ -1482,34 +1242,40 @@
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, HomoSapiensId):
             self.id = HomoSapiensId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Agent(NamedIndividual):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = PROV.Agent
+    class_class_uri: ClassVar[URIRef] = PROV["Agent"]
     class_class_curie: ClassVar[str] = "prov:Agent"
     class_name: ClassVar[str] = "Agent"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Agent
 
     id: Union[str, AgentId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, AgentId):
             self.id = AgentId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Image(NamedIndividual):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = IAO["0000101"]
@@ -1522,25 +1288,27 @@
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ImageId):
             self.id = ImageId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 @dataclass
 class Annotation(YAMLRoot):
     """
     A reified property-object pair
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.Annotation
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["Annotation"]
     class_class_curie: ClassVar[str] = "omoschema:Annotation"
     class_name: ClassVar[str] = "Annotation"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Annotation
 
     predicate: Optional[str] = None
     object: Optional[str] = None
 
@@ -1555,66 +1323,53 @@
 
 
 @dataclass
 class Axiom(YAMLRoot):
     """
     A logical or non-logical statement
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.Axiom
+    class_class_uri: ClassVar[URIRef] = OWL["Axiom"]
     class_class_curie: ClassVar[str] = "owl:Axiom"
     class_name: ClassVar[str] = "Axiom"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Axiom
 
     annotatedProperty: Optional[Union[str, AnnotationPropertyId]] = None
     annotatedSource: Optional[Union[str, NamedObjectId]] = None
     annotatedTarget: Optional[Union[dict, Any]] = None
-    annotations: Optional[Union[Union[dict, Annotation], List[Union[dict, Annotation]]]] = (
-        empty_list()
-    )
+    annotations: Optional[Union[Union[dict, Annotation], List[Union[dict, Annotation]]]] = empty_list()
     source: Optional[Union[str, List[str]]] = empty_list()
     is_inferred: Optional[Union[bool, Bool]] = None
     notes: Optional[Union[str, List[str]]] = empty_list()
     url: Optional[str] = None
     has_axiom_label: Optional[Union[dict, Thing]] = None
     is_a_defining_property_chain_axiom: Optional[str] = None
     is_a_defining_property_chain_axiom_where_second_argument_is_reflexive: Optional[str] = None
     created_by: Optional[str] = None
     date_retrieved: Optional[str] = None
     evidence: Optional[str] = None
     external_ontology: Optional[Union[str, List[str]]] = empty_list()
-    database_cross_reference: Optional[
-        Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]
-    ] = empty_list()
-    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = (
-        empty_list()
-    )
-    has_synonym_type: Optional[
-        Union[Union[str, AnnotationPropertyId], List[Union[str, AnnotationPropertyId]]]
-    ] = empty_list()
+    database_cross_reference: Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]] = empty_list()
+    has_exact_synonym: Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]] = empty_list()
+    has_synonym_type: Optional[Union[Union[str, AnnotationPropertyId], List[Union[str, AnnotationPropertyId]]]] = empty_list()
     comment: Optional[Union[str, List[str]]] = empty_list()
     label: Optional[Union[str, LabelType]] = None
     seeAlso: Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.annotatedProperty is not None and not isinstance(
-            self.annotatedProperty, AnnotationPropertyId
-        ):
+        if self.annotatedProperty is not None and not isinstance(self.annotatedProperty, AnnotationPropertyId):
             self.annotatedProperty = AnnotationPropertyId(self.annotatedProperty)
 
         if self.annotatedSource is not None and not isinstance(self.annotatedSource, NamedObjectId):
             self.annotatedSource = NamedObjectId(self.annotatedSource)
 
         if not isinstance(self.annotations, list):
             self.annotations = [self.annotations] if self.annotations is not None else []
-        self.annotations = [
-            v if isinstance(v, Annotation) else Annotation(**as_dict(v)) for v in self.annotations
-        ]
+        self.annotations = [v if isinstance(v, Annotation) else Annotation(**as_dict(v)) for v in self.annotations]
 
         if not isinstance(self.source, list):
             self.source = [self.source] if self.source is not None else []
         self.source = [v if isinstance(v, str) else str(v) for v in self.source]
 
         if self.is_inferred is not None and not isinstance(self.is_inferred, Bool):
             self.is_inferred = Bool(self.is_inferred)
@@ -1625,71 +1380,44 @@
 
         if self.url is not None and not isinstance(self.url, str):
             self.url = str(self.url)
 
         if self.has_axiom_label is not None and not isinstance(self.has_axiom_label, Thing):
             self.has_axiom_label = Thing(**as_dict(self.has_axiom_label))
 
-        if self.is_a_defining_property_chain_axiom is not None and not isinstance(
-            self.is_a_defining_property_chain_axiom, str
-        ):
+        if self.is_a_defining_property_chain_axiom is not None and not isinstance(self.is_a_defining_property_chain_axiom, str):
             self.is_a_defining_property_chain_axiom = str(self.is_a_defining_property_chain_axiom)
 
-        if (
-            self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive is not None
-            and not isinstance(
-                self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive, str
-            )
-        ):
-            self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive = str(
-                self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive
-            )
+        if self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive is not None and not isinstance(self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive, str):
+            self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive = str(self.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive)
 
         if self.created_by is not None and not isinstance(self.created_by, str):
             self.created_by = str(self.created_by)
 
         if self.date_retrieved is not None and not isinstance(self.date_retrieved, str):
             self.date_retrieved = str(self.date_retrieved)
 
         if self.evidence is not None and not isinstance(self.evidence, str):
             self.evidence = str(self.evidence)
 
         if not isinstance(self.external_ontology, list):
-            self.external_ontology = (
-                [self.external_ontology] if self.external_ontology is not None else []
-            )
-        self.external_ontology = [
-            v if isinstance(v, str) else str(v) for v in self.external_ontology
-        ]
+            self.external_ontology = [self.external_ontology] if self.external_ontology is not None else []
+        self.external_ontology = [v if isinstance(v, str) else str(v) for v in self.external_ontology]
 
         if not isinstance(self.database_cross_reference, list):
-            self.database_cross_reference = (
-                [self.database_cross_reference] if self.database_cross_reference is not None else []
-            )
-        self.database_cross_reference = [
-            v if isinstance(v, CURIELiteral) else CURIELiteral(v)
-            for v in self.database_cross_reference
-        ]
+            self.database_cross_reference = [self.database_cross_reference] if self.database_cross_reference is not None else []
+        self.database_cross_reference = [v if isinstance(v, CURIELiteral) else CURIELiteral(v) for v in self.database_cross_reference]
 
         if not isinstance(self.has_exact_synonym, list):
-            self.has_exact_synonym = (
-                [self.has_exact_synonym] if self.has_exact_synonym is not None else []
-            )
-        self.has_exact_synonym = [
-            v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym
-        ]
+            self.has_exact_synonym = [self.has_exact_synonym] if self.has_exact_synonym is not None else []
+        self.has_exact_synonym = [v if isinstance(v, LabelType) else LabelType(v) for v in self.has_exact_synonym]
 
         if not isinstance(self.has_synonym_type, list):
-            self.has_synonym_type = (
-                [self.has_synonym_type] if self.has_synonym_type is not None else []
-            )
-        self.has_synonym_type = [
-            v if isinstance(v, AnnotationPropertyId) else AnnotationPropertyId(v)
-            for v in self.has_synonym_type
-        ]
+            self.has_synonym_type = [self.has_synonym_type] if self.has_synonym_type is not None else []
+        self.has_synonym_type = [v if isinstance(v, AnnotationPropertyId) else AnnotationPropertyId(v) for v in self.has_synonym_type]
 
         if not isinstance(self.comment, list):
             self.comment = [self.comment] if self.comment is not None else []
         self.comment = [v if isinstance(v, str) else str(v) for v in self.comment]
 
         if self.label is not None and not isinstance(self.label, LabelType):
             self.label = LabelType(self.label)
@@ -1702,119 +1430,103 @@
 
 
 @dataclass
 class Subset(AnnotationProperty):
     """
     A collection of terms grouped for some purpose
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OIO.Subset
+    class_class_uri: ClassVar[URIRef] = OIO["Subset"]
     class_class_curie: ClassVar[str] = "oio:Subset"
     class_name: ClassVar[str] = "Subset"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Subset
 
     id: Union[str, SubsetId] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, SubsetId):
             self.id = SubsetId(self.id)
 
         super().__post_init__(**kwargs)
+        if not isinstance(self.type, list):
+            self.type = [self.type] if self.type is not None else []
+        self.type = [v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.type]
 
 
 class Anonymous(YAMLRoot):
     """
     Abstract root class for all anonymous (non-named; lacking an identifier) expressions
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.Anonymous
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["Anonymous"]
     class_class_curie: ClassVar[str] = "omoschema:Anonymous"
     class_name: ClassVar[str] = "Anonymous"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Anonymous
 
 
 class AnonymousClassExpression(Anonymous):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.AnonymousClassExpression
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["AnonymousClassExpression"]
     class_class_curie: ClassVar[str] = "omoschema:AnonymousClassExpression"
     class_name: ClassVar[str] = "AnonymousClassExpression"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.AnonymousClassExpression
 
 
 @dataclass
 class Restriction(AnonymousClassExpression):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OWL.Restriction
+    class_class_uri: ClassVar[URIRef] = OWL["Restriction"]
     class_class_curie: ClassVar[str] = "owl:Restriction"
     class_name: ClassVar[str] = "Restriction"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Restriction
 
-    onProperty: Optional[
-        Union[Union[dict, "PropertyExpression"], List[Union[dict, "PropertyExpression"]]]
-    ] = empty_list()
+    onProperty: Optional[Union[Union[dict, "PropertyExpression"], List[Union[dict, "PropertyExpression"]]]] = empty_list()
     someValuesFrom: Optional[Union[str, List[str]]] = empty_list()
     allValuesFrom: Optional[str] = None
     disjointWith: Optional[Union[str, List[str]]] = empty_list()
-    equivalentClass: Optional[
-        Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]
-    ] = empty_list()
+    equivalentClass: Optional[Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]] = empty_list()
     intersectionOf: Optional[Union[dict, "ClassExpression"]] = None
-    subClassOf: Optional[
-        Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]
-    ] = empty_list()
+    subClassOf: Optional[Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]] = empty_list()
     cardinality: Optional[str] = None
     complementOf: Optional[str] = None
     oneOf: Optional[Union[dict, "ClassExpression"]] = None
     unionOf: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.onProperty, list):
             self.onProperty = [self.onProperty] if self.onProperty is not None else []
-        self.onProperty = [
-            v if isinstance(v, PropertyExpression) else PropertyExpression(**as_dict(v))
-            for v in self.onProperty
-        ]
+        self.onProperty = [v if isinstance(v, PropertyExpression) else PropertyExpression(**as_dict(v)) for v in self.onProperty]
 
         if not isinstance(self.someValuesFrom, list):
             self.someValuesFrom = [self.someValuesFrom] if self.someValuesFrom is not None else []
         self.someValuesFrom = [v if isinstance(v, str) else str(v) for v in self.someValuesFrom]
 
         if self.allValuesFrom is not None and not isinstance(self.allValuesFrom, str):
             self.allValuesFrom = str(self.allValuesFrom)
 
         if not isinstance(self.disjointWith, list):
             self.disjointWith = [self.disjointWith] if self.disjointWith is not None else []
         self.disjointWith = [v if isinstance(v, str) else str(v) for v in self.disjointWith]
 
         if not isinstance(self.equivalentClass, list):
-            self.equivalentClass = (
-                [self.equivalentClass] if self.equivalentClass is not None else []
-            )
-        self.equivalentClass = [
-            v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v))
-            for v in self.equivalentClass
-        ]
+            self.equivalentClass = [self.equivalentClass] if self.equivalentClass is not None else []
+        self.equivalentClass = [v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v)) for v in self.equivalentClass]
 
         if self.intersectionOf is not None and not isinstance(self.intersectionOf, ClassExpression):
             self.intersectionOf = ClassExpression(**as_dict(self.intersectionOf))
 
         if not isinstance(self.subClassOf, list):
             self.subClassOf = [self.subClassOf] if self.subClassOf is not None else []
-        self.subClassOf = [
-            v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v))
-            for v in self.subClassOf
-        ]
+        self.subClassOf = [v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v)) for v in self.subClassOf]
 
         if self.cardinality is not None and not isinstance(self.cardinality, str):
             self.cardinality = str(self.cardinality)
 
         if self.complementOf is not None and not isinstance(self.complementOf, str):
             self.complementOf = str(self.complementOf)
 
@@ -1826,65 +1538,53 @@
 
         super().__post_init__(**kwargs)
 
 
 class Expression(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.Expression
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["Expression"]
     class_class_curie: ClassVar[str] = "omoschema:Expression"
     class_name: ClassVar[str] = "Expression"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.Expression
 
 
 @dataclass
 class ClassExpression(Expression):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.ClassExpression
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["ClassExpression"]
     class_class_curie: ClassVar[str] = "omoschema:ClassExpression"
     class_name: ClassVar[str] = "ClassExpression"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.ClassExpression
 
     disjointWith: Optional[Union[str, List[str]]] = empty_list()
-    equivalentClass: Optional[
-        Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]
-    ] = empty_list()
+    equivalentClass: Optional[Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]] = empty_list()
     intersectionOf: Optional[Union[dict, "ClassExpression"]] = None
-    subClassOf: Optional[
-        Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]
-    ] = empty_list()
+    subClassOf: Optional[Union[Union[dict, "ClassExpression"], List[Union[dict, "ClassExpression"]]]] = empty_list()
     cardinality: Optional[str] = None
     complementOf: Optional[str] = None
     oneOf: Optional[Union[dict, "ClassExpression"]] = None
     unionOf: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.disjointWith, list):
             self.disjointWith = [self.disjointWith] if self.disjointWith is not None else []
         self.disjointWith = [v if isinstance(v, str) else str(v) for v in self.disjointWith]
 
         if not isinstance(self.equivalentClass, list):
-            self.equivalentClass = (
-                [self.equivalentClass] if self.equivalentClass is not None else []
-            )
-        self.equivalentClass = [
-            v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v))
-            for v in self.equivalentClass
-        ]
+            self.equivalentClass = [self.equivalentClass] if self.equivalentClass is not None else []
+        self.equivalentClass = [v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v)) for v in self.equivalentClass]
 
         if self.intersectionOf is not None and not isinstance(self.intersectionOf, ClassExpression):
             self.intersectionOf = ClassExpression(**as_dict(self.intersectionOf))
 
         if not isinstance(self.subClassOf, list):
             self.subClassOf = [self.subClassOf] if self.subClassOf is not None else []
-        self.subClassOf = [
-            v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v))
-            for v in self.subClassOf
-        ]
+        self.subClassOf = [v if isinstance(v, ClassExpression) else ClassExpression(**as_dict(v)) for v in self.subClassOf]
 
         if self.cardinality is not None and not isinstance(self.cardinality, str):
             self.cardinality = str(self.cardinality)
 
         if self.complementOf is not None and not isinstance(self.complementOf, str):
             self.complementOf = str(self.complementOf)
 
@@ -1897,15 +1597,15 @@
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class PropertyExpression(Expression):
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.PropertyExpression
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["PropertyExpression"]
     class_class_curie: ClassVar[str] = "omoschema:PropertyExpression"
     class_name: ClassVar[str] = "PropertyExpression"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.PropertyExpression
 
     disjointWith: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -1917,18 +1617,17 @@
 
 
 @dataclass
 class ObsoleteAspect(YAMLRoot):
     """
     Auto-classifies anything that is obsolete
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.ObsoleteAspect
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["ObsoleteAspect"]
     class_class_curie: ClassVar[str] = "omoschema:ObsoleteAspect"
     class_name: ClassVar[str] = "ObsoleteAspect"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.ObsoleteAspect
 
     label: Optional[Union[str, LabelType]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
@@ -1938,1453 +1637,543 @@
         super().__post_init__(**kwargs)
 
 
 class NotObsoleteAspect(YAMLRoot):
     """
     Auto-classifies anything that is not obsolete
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
-    class_class_uri: ClassVar[URIRef] = OMOSCHEMA.NotObsoleteAspect
+    class_class_uri: ClassVar[URIRef] = OMOSCHEMA["NotObsoleteAspect"]
     class_class_curie: ClassVar[str] = "omoschema:NotObsoleteAspect"
     class_name: ClassVar[str] = "NotObsoleteAspect"
     class_model_uri: ClassVar[URIRef] = OMOSCHEMA.NotObsoleteAspect
 
 
 # Enumerations
 class DefinitionConstraintComponent(EnumDefinitionImpl):
     """
     An extension of SHACL constraint component for constraining definitions
     """
-
     DefinitionConstraint = PermissibleValue(
         text="DefinitionConstraint",
         description="A general problem with a definition",
-        meaning=OMOSCHEMA["DCC.Any"],
-    )
+        meaning=OMOSCHEMA["DCC.Any"])
     DefinitionPresence = PermissibleValue(
         text="DefinitionPresence",
         description="An entity must have a definition",
-        meaning=OMOSCHEMA["DCC.S0"],
-    )
+        meaning=OMOSCHEMA["DCC.S0"])
     Conventions = PermissibleValue(
         text="Conventions",
         description="Definitions should conform to conventions",
-        meaning=OMOSCHEMA["DCC.S1"],
-    )
+        meaning=OMOSCHEMA["DCC.S1"])
     Harmonized = PermissibleValue(
         text="Harmonized",
         description="Definitions should be harmonized",
-        meaning=OMOSCHEMA["DCC.S1.1"],
-    )
+        meaning=OMOSCHEMA["DCC.S1.1"])
     GenusDifferentiaForm = PermissibleValue(
         text="GenusDifferentiaForm",
         description="A definition should follow the genus-differentia form",
-        meaning=OMOSCHEMA["DCC.S3"],
-    )
+        meaning=OMOSCHEMA["DCC.S3"])
     SingleGenus = PermissibleValue(
         text="SingleGenus",
         description="An entity must have a single genus",
-        meaning=OMOSCHEMA["DCC.S3.1"],
-    )
+        meaning=OMOSCHEMA["DCC.S3.1"])
     Circularity = PermissibleValue(
         text="Circularity",
         description="A definition must not be circular",
-        meaning=OMOSCHEMA["DCC.S7"],
-    )
+        meaning=OMOSCHEMA["DCC.S7"])
     MatchTextAndLogical = PermissibleValue(
         text="MatchTextAndLogical",
         description="Text definitions and logical forms should match",
-        meaning=OMOSCHEMA["DCC.S11"],
-    )
+        meaning=OMOSCHEMA["DCC.S11"])
+    MatchTextAndLogicalGenusNotInText = PermissibleValue(
+        text="MatchTextAndLogicalGenusNotInText",
+        description="The genus in the logical definition should be in the text definition",
+        meaning=OMOSCHEMA["DCC.S11.1"])
+    MatchTextAndLogicalDifferentiaNotInText = PermissibleValue(
+        text="MatchTextAndLogicalDifferentiaNotInText",
+        description="The differentia in the logical definition should be in the text definition",
+        meaning=OMOSCHEMA["DCC.S11.2"])
+    MatchTextAndReference = PermissibleValue(
+        text="MatchTextAndReference",
+        description="Text definitions and cited references and provenance for the text definition should match",
+        meaning=OMOSCHEMA["DCC.S20"])
+    ReferenceNotFound = PermissibleValue(
+        text="ReferenceNotFound",
+        description="The citation for the reference cannot be found",
+        meaning=OMOSCHEMA["DCC.S20.1"])
+    ReferenceIsRetracted = PermissibleValue(
+        text="ReferenceIsRetracted",
+        description="The citation for the reference is retracted",
+        meaning=OMOSCHEMA["DCC.S20.2"])
 
     _defn = EnumDefinition(
         name="DefinitionConstraintComponent",
         description="An extension of SHACL constraint component for constraining definitions",
     )
 
-
 # Slots
 class slots:
     pass
 
+slots.core_property = Slot(uri=OMOSCHEMA.core_property, name="core_property", curie=OMOSCHEMA.curie('core_property'),
+                   model_uri=OMOSCHEMA.core_property, domain=None, range=Optional[str])
+
+slots.id = Slot(uri=OMOSCHEMA.id, name="id", curie=OMOSCHEMA.curie('id'),
+                   model_uri=OMOSCHEMA.id, domain=None, range=URIRef)
+
+slots.label = Slot(uri=RDFS.label, name="label", curie=RDFS.curie('label'),
+                   model_uri=OMOSCHEMA.label, domain=None, range=Optional[Union[str, LabelType]])
+
+slots.annotations = Slot(uri=OMOSCHEMA.annotations, name="annotations", curie=OMOSCHEMA.curie('annotations'),
+                   model_uri=OMOSCHEMA.annotations, domain=None, range=Optional[Union[Union[dict, Annotation], List[Union[dict, Annotation]]]])
+
+slots.definition = Slot(uri=IAO['0000115'], name="definition", curie=IAO.curie('0000115'),
+                   model_uri=OMOSCHEMA.definition, domain=None, range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]])
+
+slots.predicate = Slot(uri=OMOSCHEMA.predicate, name="predicate", curie=OMOSCHEMA.curie('predicate'),
+                   model_uri=OMOSCHEMA.predicate, domain=None, range=Optional[str])
+
+slots.object = Slot(uri=OMOSCHEMA.object, name="object", curie=OMOSCHEMA.curie('object'),
+                   model_uri=OMOSCHEMA.object, domain=None, range=Optional[str])
+
+slots.title = Slot(uri=DCTERMS.title, name="title", curie=DCTERMS.curie('title'),
+                   model_uri=OMOSCHEMA.title, domain=None, range=Optional[Union[str, NarrativeText]])
+
+slots.match_aspect = Slot(uri=OMOSCHEMA.match_aspect, name="match_aspect", curie=OMOSCHEMA.curie('match_aspect'),
+                   model_uri=OMOSCHEMA.match_aspect, domain=None, range=Optional[str])
+
+slots.match = Slot(uri=OMOSCHEMA.match, name="match", curie=OMOSCHEMA.curie('match'),
+                   model_uri=OMOSCHEMA.match, domain=None, range=Optional[str])
+
+slots.broadMatch = Slot(uri=SKOS.broadMatch, name="broadMatch", curie=SKOS.curie('broadMatch'),
+                   model_uri=OMOSCHEMA.broadMatch, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.closeMatch = Slot(uri=SKOS.closeMatch, name="closeMatch", curie=SKOS.curie('closeMatch'),
+                   model_uri=OMOSCHEMA.closeMatch, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.exactMatch = Slot(uri=SKOS.exactMatch, name="exactMatch", curie=SKOS.curie('exactMatch'),
+                   model_uri=OMOSCHEMA.exactMatch, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.narrowMatch = Slot(uri=SKOS.narrowMatch, name="narrowMatch", curie=SKOS.curie('narrowMatch'),
+                   model_uri=OMOSCHEMA.narrowMatch, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.database_cross_reference = Slot(uri=OIO.hasDbXref, name="database_cross_reference", curie=OIO.curie('hasDbXref'),
+                   model_uri=OMOSCHEMA.database_cross_reference, domain=None, range=Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]])
+
+slots.informative_property = Slot(uri=OMOSCHEMA.informative_property, name="informative_property", curie=OMOSCHEMA.curie('informative_property'),
+                   model_uri=OMOSCHEMA.informative_property, domain=None, range=Optional[str])
+
+slots.comment = Slot(uri=RDFS.comment, name="comment", curie=RDFS.curie('comment'),
+                   model_uri=OMOSCHEMA.comment, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.category = Slot(uri=BIOLINK.category, name="category", curie=BIOLINK.curie('category'),
+                   model_uri=OMOSCHEMA.category, domain=None, range=Optional[str])
+
+slots.image = Slot(uri=SDO.image, name="image", curie=SDO.curie('image'),
+                   model_uri=OMOSCHEMA.image, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.example_of_usage = Slot(uri=IAO['0000112'], name="example_of_usage", curie=IAO.curie('0000112'),
+                   model_uri=OMOSCHEMA.example_of_usage, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.changeNote = Slot(uri=SKOS.changeNote, name="changeNote", curie=SKOS.curie('changeNote'),
+                   model_uri=OMOSCHEMA.changeNote, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.has_curation_status = Slot(uri=IAO['0000114'], name="has_curation_status", curie=IAO.curie('0000114'),
+                   model_uri=OMOSCHEMA.has_curation_status, domain=None, range=Optional[str])
+
+slots.defaultLanguage = Slot(uri=PROTEGE.defaultLanguage, name="defaultLanguage", curie=PROTEGE.curie('defaultLanguage'),
+                   model_uri=OMOSCHEMA.defaultLanguage, domain=None, range=Optional[str])
+
+slots.language = Slot(uri=DCTERMS.language, name="language", curie=DCTERMS.curie('language'),
+                   model_uri=OMOSCHEMA.language, domain=None, range=Optional[str])
+
+slots.has_ontology_root_term = Slot(uri=IAO['0000700'], name="has_ontology_root_term", curie=IAO.curie('0000700'),
+                   model_uri=OMOSCHEMA.has_ontology_root_term, domain=None, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.conformsTo = Slot(uri=DCTERMS.conformsTo, name="conformsTo", curie=DCTERMS.curie('conformsTo'),
+                   model_uri=OMOSCHEMA.conformsTo, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.license = Slot(uri=DCTERMS.license, name="license", curie=DCTERMS.curie('license'),
+                   model_uri=OMOSCHEMA.license, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.depicted_by = Slot(uri=FOAF.depicted_by, name="depicted_by", curie=FOAF.curie('depicted_by'),
+                   model_uri=OMOSCHEMA.depicted_by, domain=None, range=Optional[Union[Union[str, ImageId], List[Union[str, ImageId]]]])
+
+slots.page = Slot(uri=FOAF.page, name="page", curie=FOAF.curie('page'),
+                   model_uri=OMOSCHEMA.page, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.version_property = Slot(uri=OMOSCHEMA.version_property, name="version_property", curie=OMOSCHEMA.curie('version_property'),
+                   model_uri=OMOSCHEMA.version_property, domain=None, range=Optional[str])
+
+slots.versionIRI = Slot(uri=OWL.versionIRI, name="versionIRI", curie=OWL.curie('versionIRI'),
+                   model_uri=OMOSCHEMA.versionIRI, domain=None, range=Optional[Union[str, URIorCURIE]])
+
+slots.versionInfo = Slot(uri=OWL.versionInfo, name="versionInfo", curie=OWL.curie('versionInfo'),
+                   model_uri=OMOSCHEMA.versionInfo, domain=None, range=Optional[str])
+
+slots.obsoletion_related_property = Slot(uri=OMOSCHEMA.obsoletion_related_property, name="obsoletion_related_property", curie=OMOSCHEMA.curie('obsoletion_related_property'),
+                   model_uri=OMOSCHEMA.obsoletion_related_property, domain=None, range=Optional[str])
+
+slots.deprecated = Slot(uri=OWL.deprecated, name="deprecated", curie=OWL.curie('deprecated'),
+                   model_uri=OMOSCHEMA.deprecated, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.term_replaced_by = Slot(uri=IAO['0100001'], name="term_replaced_by", curie=IAO.curie('0100001'),
+                   model_uri=OMOSCHEMA.term_replaced_by, domain=None, range=Optional[Union[dict, Any]])
+
+slots.has_obsolescence_reason = Slot(uri=IAO['0000231'], name="has_obsolescence_reason", curie=IAO.curie('0000231'),
+                   model_uri=OMOSCHEMA.has_obsolescence_reason, domain=None, range=Optional[str])
+
+slots.consider = Slot(uri=OIO.consider, name="consider", curie=OIO.curie('consider'),
+                   model_uri=OMOSCHEMA.consider, domain=None, range=Optional[Union[Union[dict, Any], List[Union[dict, Any]]]])
+
+slots.has_alternative_id = Slot(uri=OIO.hasAlternativeId, name="has_alternative_id", curie=OIO.curie('hasAlternativeId'),
+                   model_uri=OMOSCHEMA.has_alternative_id, domain=None, range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]])
+
+slots.temporal_interpretation = Slot(uri=RO['0001900'], name="temporal_interpretation", curie=RO.curie('0001900'),
+                   model_uri=OMOSCHEMA.temporal_interpretation, domain=None, range=Optional[Union[str, NamedIndividualId]])
+
+slots.never_in_taxon = Slot(uri=RO['0002161'], name="never_in_taxon", curie=RO.curie('0002161'),
+                   model_uri=OMOSCHEMA.never_in_taxon, domain=None, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.is_a_defining_property_chain_axiom = Slot(uri=RO['0002581'], name="is_a_defining_property_chain_axiom", curie=RO.curie('0002581'),
+                   model_uri=OMOSCHEMA.is_a_defining_property_chain_axiom, domain=None, range=Optional[str])
+
+slots.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive = Slot(uri=RO['0002582'], name="is_a_defining_property_chain_axiom_where_second_argument_is_reflexive", curie=RO.curie('0002582'),
+                   model_uri=OMOSCHEMA.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive, domain=None, range=Optional[str])
+
+slots.provenance_property = Slot(uri=OMOSCHEMA.provenance_property, name="provenance_property", curie=OMOSCHEMA.curie('provenance_property'),
+                   model_uri=OMOSCHEMA.provenance_property, domain=None, range=Optional[str])
+
+slots.contributor = Slot(uri=DCTERMS.contributor, name="contributor", curie=DCTERMS.curie('contributor'),
+                   model_uri=OMOSCHEMA.contributor, domain=None, range=Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]])
+
+slots.creator = Slot(uri=DCTERMS.creator, name="creator", curie=DCTERMS.curie('creator'),
+                   model_uri=OMOSCHEMA.creator, domain=None, range=Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]])
+
+slots.created = Slot(uri=DCTERMS.created, name="created", curie=DCTERMS.curie('created'),
+                   model_uri=OMOSCHEMA.created, domain=None, range=Optional[str])
+
+slots.date = Slot(uri=DCTERMS.date, name="date", curie=DCTERMS.curie('date'),
+                   model_uri=OMOSCHEMA.date, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.source = Slot(uri=DCTERMS.source, name="source", curie=DCTERMS.curie('source'),
+                   model_uri=OMOSCHEMA.source, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.created_by = Slot(uri=OIO.created_by, name="created_by", curie=OIO.curie('created_by'),
+                   model_uri=OMOSCHEMA.created_by, domain=None, range=Optional[str])
+
+slots.creation_date = Slot(uri=OIO.creation_date, name="creation_date", curie=OIO.curie('creation_date'),
+                   model_uri=OMOSCHEMA.creation_date, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.date_retrieved = Slot(uri=OIO.date_retrieved, name="date_retrieved", curie=OIO.curie('date_retrieved'),
+                   model_uri=OMOSCHEMA.date_retrieved, domain=None, range=Optional[str])
+
+slots.editor_note = Slot(uri=IAO['0000116'], name="editor_note", curie=IAO.curie('0000116'),
+                   model_uri=OMOSCHEMA.editor_note, domain=None, range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]])
+
+slots.term_editor = Slot(uri=IAO['0000117'], name="term_editor", curie=IAO.curie('0000117'),
+                   model_uri=OMOSCHEMA.term_editor, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.definition_source = Slot(uri=IAO['0000119'], name="definition_source", curie=IAO.curie('0000119'),
+                   model_uri=OMOSCHEMA.definition_source, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.curator_note = Slot(uri=IAO['0000232'], name="curator_note", curie=IAO.curie('0000232'),
+                   model_uri=OMOSCHEMA.curator_note, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.term_tracker_item = Slot(uri=IAO['0000233'], name="term_tracker_item", curie=IAO.curie('0000233'),
+                   model_uri=OMOSCHEMA.term_tracker_item, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.ontology_term_requester = Slot(uri=IAO['0000234'], name="ontology_term_requester", curie=IAO.curie('0000234'),
+                   model_uri=OMOSCHEMA.ontology_term_requester, domain=None, range=Optional[str])
+
+slots.imported_from = Slot(uri=IAO['0000412'], name="imported_from", curie=IAO.curie('0000412'),
+                   model_uri=OMOSCHEMA.imported_from, domain=None, range=Optional[Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]])
+
+slots.has_axiom_label = Slot(uri=IAO['0010000'], name="has_axiom_label", curie=IAO.curie('0010000'),
+                   model_uri=OMOSCHEMA.has_axiom_label, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.shortcut_annotation_property = Slot(uri=OMOSCHEMA.shortcut_annotation_property, name="shortcut_annotation_property", curie=OMOSCHEMA.curie('shortcut_annotation_property'),
+                   model_uri=OMOSCHEMA.shortcut_annotation_property, domain=None, range=Optional[str])
+
+slots.disconnected_from = Slot(uri=OMOSCHEMA.disconnected_from, name="disconnected_from", curie=OMOSCHEMA.curie('disconnected_from'),
+                   model_uri=OMOSCHEMA.disconnected_from, domain=None, range=Optional[Union[str, ClassId]])
+
+slots.excluded_axiom = Slot(uri=OMOSCHEMA.excluded_axiom, name="excluded_axiom", curie=OMOSCHEMA.curie('excluded_axiom'),
+                   model_uri=OMOSCHEMA.excluded_axiom, domain=None, range=Optional[str])
+
+slots.excluded_from_QC_check = Slot(uri=OMOSCHEMA.excluded_from_QC_check, name="excluded_from_QC_check", curie=OMOSCHEMA.curie('excluded_from_QC_check'),
+                   model_uri=OMOSCHEMA.excluded_from_QC_check, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.excluded_subClassOf = Slot(uri=OMOSCHEMA.excluded_subClassOf, name="excluded_subClassOf", curie=OMOSCHEMA.curie('excluded_subClassOf'),
+                   model_uri=OMOSCHEMA.excluded_subClassOf, domain=None, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.excluded_synonym = Slot(uri=OMOSCHEMA.excluded_synonym, name="excluded_synonym", curie=OMOSCHEMA.curie('excluded_synonym'),
+                   model_uri=OMOSCHEMA.excluded_synonym, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.should_conform_to = Slot(uri=OMOSCHEMA.should_conform_to, name="should_conform_to", curie=OMOSCHEMA.curie('should_conform_to'),
+                   model_uri=OMOSCHEMA.should_conform_to, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.has_rank = Slot(uri=OMOSCHEMA.has_rank, name="has_rank", curie=OMOSCHEMA.curie('has_rank'),
+                   model_uri=OMOSCHEMA.has_rank, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.alternative_term = Slot(uri=IAO['0000118'], name="alternative_term", curie=IAO.curie('0000118'),
+                   model_uri=OMOSCHEMA.alternative_term, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.ISA_alternative_term = Slot(uri=OBI['0001847'], name="ISA_alternative_term", curie=OBI.curie('0001847'),
+                   model_uri=OMOSCHEMA.ISA_alternative_term, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.IEDB_alternative_term = Slot(uri=OBI['9991118'], name="IEDB_alternative_term", curie=OBI.curie('9991118'),
+                   model_uri=OMOSCHEMA.IEDB_alternative_term, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.OBO_foundry_unique_label = Slot(uri=IAO['0000589'], name="OBO_foundry_unique_label", curie=IAO.curie('0000589'),
+                   model_uri=OMOSCHEMA.OBO_foundry_unique_label, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.synonym = Slot(uri=OIO.hasSynonym, name="synonym", curie=OIO.curie('hasSynonym'),
+                   model_uri=OMOSCHEMA.synonym, domain=None, range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]])
+
+slots.editor_preferred_term = Slot(uri=IAO['0000111'], name="editor_preferred_term", curie=IAO.curie('0000111'),
+                   model_uri=OMOSCHEMA.editor_preferred_term, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.has_exact_synonym = Slot(uri=OIO.hasExactSynonym, name="has_exact_synonym", curie=OIO.curie('hasExactSynonym'),
+                   model_uri=OMOSCHEMA.has_exact_synonym, domain=None, range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]])
+
+slots.has_narrow_synonym = Slot(uri=OIO.hasNarrowSynonym, name="has_narrow_synonym", curie=OIO.curie('hasNarrowSynonym'),
+                   model_uri=OMOSCHEMA.has_narrow_synonym, domain=None, range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]])
+
+slots.has_related_synonym = Slot(uri=OIO.hasRelatedSynonym, name="has_related_synonym", curie=OIO.curie('hasRelatedSynonym'),
+                   model_uri=OMOSCHEMA.has_related_synonym, domain=None, range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]])
+
+slots.has_broad_synonym = Slot(uri=OIO.hasBroadSynonym, name="has_broad_synonym", curie=OIO.curie('hasBroadSynonym'),
+                   model_uri=OMOSCHEMA.has_broad_synonym, domain=None, range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]])
+
+slots.has_synonym_type = Slot(uri=OIO.hasSynonymType, name="has_synonym_type", curie=OIO.curie('hasSynonymType'),
+                   model_uri=OMOSCHEMA.has_synonym_type, domain=None, range=Optional[Union[Union[str, AnnotationPropertyId], List[Union[str, AnnotationPropertyId]]]])
+
+slots.has_obo_namespace = Slot(uri=OIO.hasOBONamespace, name="has_obo_namespace", curie=OIO.curie('hasOBONamespace'),
+                   model_uri=OMOSCHEMA.has_obo_namespace, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.in_subset = Slot(uri=OIO.inSubset, name="in_subset", curie=OIO.curie('inSubset'),
+                   model_uri=OMOSCHEMA.in_subset, domain=None, range=Optional[Union[Union[str, SubsetId], List[Union[str, SubsetId]]]])
+
+slots.reification_predicate = Slot(uri=OMOSCHEMA.reification_predicate, name="reification_predicate", curie=OMOSCHEMA.curie('reification_predicate'),
+                   model_uri=OMOSCHEMA.reification_predicate, domain=None, range=Optional[str])
+
+slots.annotatedProperty = Slot(uri=OWL.annotatedProperty, name="annotatedProperty", curie=OWL.curie('annotatedProperty'),
+                   model_uri=OMOSCHEMA.annotatedProperty, domain=None, range=Optional[Union[str, AnnotationPropertyId]])
+
+slots.annotatedSource = Slot(uri=OWL.annotatedSource, name="annotatedSource", curie=OWL.curie('annotatedSource'),
+                   model_uri=OMOSCHEMA.annotatedSource, domain=None, range=Optional[Union[str, NamedObjectId]])
+
+slots.annotatedTarget = Slot(uri=OWL.annotatedTarget, name="annotatedTarget", curie=OWL.curie('annotatedTarget'),
+                   model_uri=OMOSCHEMA.annotatedTarget, domain=None, range=Optional[Union[dict, Any]])
+
+slots.imports = Slot(uri=OWL.imports, name="imports", curie=OWL.curie('imports'),
+                   model_uri=OMOSCHEMA.imports, domain=None, range=Optional[str])
+
+slots.logical_predicate = Slot(uri=OMOSCHEMA.logical_predicate, name="logical_predicate", curie=OMOSCHEMA.curie('logical_predicate'),
+                   model_uri=OMOSCHEMA.logical_predicate, domain=None, range=Optional[str])
+
+slots.cardinality = Slot(uri=OWL.cardinality, name="cardinality", curie=OWL.curie('cardinality'),
+                   model_uri=OMOSCHEMA.cardinality, domain=None, range=Optional[str])
+
+slots.complementOf = Slot(uri=OWL.complementOf, name="complementOf", curie=OWL.curie('complementOf'),
+                   model_uri=OMOSCHEMA.complementOf, domain=None, range=Optional[str])
+
+slots.disjointWith = Slot(uri=OWL.disjointWith, name="disjointWith", curie=OWL.curie('disjointWith'),
+                   model_uri=OMOSCHEMA.disjointWith, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.distinctMembers = Slot(uri=OWL.distinctMembers, name="distinctMembers", curie=OWL.curie('distinctMembers'),
+                   model_uri=OMOSCHEMA.distinctMembers, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.equivalentClass = Slot(uri=OWL.equivalentClass, name="equivalentClass", curie=OWL.curie('equivalentClass'),
+                   model_uri=OMOSCHEMA.equivalentClass, domain=None, range=Optional[Union[Union[dict, ClassExpression], List[Union[dict, ClassExpression]]]])
+
+slots.sameAs = Slot(uri=OWL.sameAs, name="sameAs", curie=OWL.curie('sameAs'),
+                   model_uri=OMOSCHEMA.sameAs, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.equivalentProperty = Slot(uri=OWL.equivalentProperty, name="equivalentProperty", curie=OWL.curie('equivalentProperty'),
+                   model_uri=OMOSCHEMA.equivalentProperty, domain=None, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.hasValue = Slot(uri=OWL.hasValue, name="hasValue", curie=OWL.curie('hasValue'),
+                   model_uri=OMOSCHEMA.hasValue, domain=None, range=Optional[Union[dict, Any]])
+
+slots.intersectionOf = Slot(uri=OWL.intersectionOf, name="intersectionOf", curie=OWL.curie('intersectionOf'),
+                   model_uri=OMOSCHEMA.intersectionOf, domain=None, range=Optional[Union[dict, ClassExpression]])
+
+slots.inverseOf = Slot(uri=OWL.inverseOf, name="inverseOf", curie=OWL.curie('inverseOf'),
+                   model_uri=OMOSCHEMA.inverseOf, domain=None, range=Optional[Union[str, PropertyId]])
+
+slots.maxQualifiedCardinality = Slot(uri=OWL.maxQualifiedCardinality, name="maxQualifiedCardinality", curie=OWL.curie('maxQualifiedCardinality'),
+                   model_uri=OMOSCHEMA.maxQualifiedCardinality, domain=None, range=Optional[int])
+
+slots.members = Slot(uri=OWL.members, name="members", curie=OWL.curie('members'),
+                   model_uri=OMOSCHEMA.members, domain=None, range=Optional[Union[dict, Thing]])
+
+slots.minCardinality = Slot(uri=OWL.minCardinality, name="minCardinality", curie=OWL.curie('minCardinality'),
+                   model_uri=OMOSCHEMA.minCardinality, domain=None, range=Optional[int])
+
+slots.minQualifiedCardinality = Slot(uri=OWL.minQualifiedCardinality, name="minQualifiedCardinality", curie=OWL.curie('minQualifiedCardinality'),
+                   model_uri=OMOSCHEMA.minQualifiedCardinality, domain=None, range=Optional[int])
+
+slots.onClass = Slot(uri=OWL.onClass, name="onClass", curie=OWL.curie('onClass'),
+                   model_uri=OMOSCHEMA.onClass, domain=None, range=Optional[Union[dict, ClassExpression]])
+
+slots.onProperty = Slot(uri=OWL.onProperty, name="onProperty", curie=OWL.curie('onProperty'),
+                   model_uri=OMOSCHEMA.onProperty, domain=None, range=Optional[Union[Union[dict, PropertyExpression], List[Union[dict, PropertyExpression]]]])
+
+slots.oneOf = Slot(uri=OWL.oneOf, name="oneOf", curie=OWL.curie('oneOf'),
+                   model_uri=OMOSCHEMA.oneOf, domain=None, range=Optional[Union[dict, ClassExpression]])
+
+slots.propertyChainAxiom = Slot(uri=OWL.propertyChainAxiom, name="propertyChainAxiom", curie=OWL.curie('propertyChainAxiom'),
+                   model_uri=OMOSCHEMA.propertyChainAxiom, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.qualifiedCardinality = Slot(uri=OWL.qualifiedCardinality, name="qualifiedCardinality", curie=OWL.curie('qualifiedCardinality'),
+                   model_uri=OMOSCHEMA.qualifiedCardinality, domain=None, range=Optional[str])
+
+slots.allValuesFrom = Slot(uri=OWL.allValuesFrom, name="allValuesFrom", curie=OWL.curie('allValuesFrom'),
+                   model_uri=OMOSCHEMA.allValuesFrom, domain=None, range=Optional[str])
+
+slots.someValuesFrom = Slot(uri=OWL.someValuesFrom, name="someValuesFrom", curie=OWL.curie('someValuesFrom'),
+                   model_uri=OMOSCHEMA.someValuesFrom, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.unionOf = Slot(uri=OWL.unionOf, name="unionOf", curie=OWL.curie('unionOf'),
+                   model_uri=OMOSCHEMA.unionOf, domain=None, range=Optional[str])
+
+slots.domain = Slot(uri=RDFS.domain, name="domain", curie=RDFS.curie('domain'),
+                   model_uri=OMOSCHEMA.domain, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.range = Slot(uri=RDFS.range, name="range", curie=RDFS.curie('range'),
+                   model_uri=OMOSCHEMA.range, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.isDefinedBy = Slot(uri=RDFS.isDefinedBy, name="isDefinedBy", curie=RDFS.curie('isDefinedBy'),
+                   model_uri=OMOSCHEMA.isDefinedBy, domain=None, range=Optional[Union[str, OntologyId]])
+
+slots.seeAlso = Slot(uri=RDFS.seeAlso, name="seeAlso", curie=RDFS.curie('seeAlso'),
+                   model_uri=OMOSCHEMA.seeAlso, domain=None, range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]])
+
+slots.type = Slot(uri=RDF.type, name="type", curie=RDF.curie('type'),
+                   model_uri=OMOSCHEMA.type, domain=None, range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]])
+
+slots.subClassOf = Slot(uri=RDFS.subClassOf, name="subClassOf", curie=RDFS.curie('subClassOf'),
+                   model_uri=OMOSCHEMA.subClassOf, domain=None, range=Optional[Union[Union[dict, ClassExpression], List[Union[dict, ClassExpression]]]])
+
+slots.oboInOwl_id = Slot(uri=OIO.id, name="oboInOwl_id", curie=OIO.curie('id'),
+                   model_uri=OMOSCHEMA.oboInOwl_id, domain=None, range=Optional[str])
+
+slots.oboInOwl_ontology = Slot(uri=OIO.ontology, name="oboInOwl_ontology", curie=OIO.curie('ontology'),
+                   model_uri=OMOSCHEMA.oboInOwl_ontology, domain=None, range=Optional[str])
+
+slots.is_class_level = Slot(uri=OIO.is_class_level, name="is_class_level", curie=OIO.curie('is_class_level'),
+                   model_uri=OMOSCHEMA.is_class_level, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.is_cyclic = Slot(uri=OIO.is_cyclic, name="is_cyclic", curie=OIO.curie('is_cyclic'),
+                   model_uri=OMOSCHEMA.is_cyclic, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.is_inferred = Slot(uri=OIO.is_inferred, name="is_inferred", curie=OIO.curie('is_inferred'),
+                   model_uri=OMOSCHEMA.is_inferred, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.is_metadata_tag = Slot(uri=OIO.is_metadata_tag, name="is_metadata_tag", curie=OIO.curie('is_metadata_tag'),
+                   model_uri=OMOSCHEMA.is_metadata_tag, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.is_transitive = Slot(uri=OIO.is_transitive, name="is_transitive", curie=OIO.curie('is_transitive'),
+                   model_uri=OMOSCHEMA.is_transitive, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.notes = Slot(uri=OIO.notes, name="notes", curie=OIO.curie('notes'),
+                   model_uri=OMOSCHEMA.notes, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.shorthand = Slot(uri=OIO.shorthand, name="shorthand", curie=OIO.curie('shorthand'),
+                   model_uri=OMOSCHEMA.shorthand, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.url = Slot(uri=OIO.url, name="url", curie=OIO.curie('url'),
+                   model_uri=OMOSCHEMA.url, domain=None, range=Optional[str])
+
+slots.evidence = Slot(uri=OIO.evidence, name="evidence", curie=OIO.curie('evidence'),
+                   model_uri=OMOSCHEMA.evidence, domain=None, range=Optional[str])
+
+slots.external_ontology = Slot(uri=OIO.external_ontology, name="external_ontology", curie=OIO.curie('external_ontology'),
+                   model_uri=OMOSCHEMA.external_ontology, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.NCIT_definition_source = Slot(uri=NCIT.P378, name="NCIT_definition_source", curie=NCIT.curie('P378'),
+                   model_uri=OMOSCHEMA.NCIT_definition_source, domain=None, range=Optional[str])
+
+slots.NCIT_term_type = Slot(uri=NCIT.P383, name="NCIT_term_type", curie=NCIT.curie('P383'),
+                   model_uri=OMOSCHEMA.NCIT_term_type, domain=None, range=Optional[str])
+
+slots.NCIT_term_source = Slot(uri=NCIT.P384, name="NCIT_term_source", curie=NCIT.curie('P384'),
+                   model_uri=OMOSCHEMA.NCIT_term_source, domain=None, range=Optional[str])
+
+slots.annotation__predicate = Slot(uri=OMOSCHEMA.predicate, name="annotation__predicate", curie=OMOSCHEMA.curie('predicate'),
+                   model_uri=OMOSCHEMA.annotation__predicate, domain=None, range=Optional[str])
+
+slots.annotation__object = Slot(uri=OMOSCHEMA.object, name="annotation__object", curie=OMOSCHEMA.curie('object'),
+                   model_uri=OMOSCHEMA.annotation__object, domain=None, range=Optional[str])
+
+slots.Ontology_title = Slot(uri=DCTERMS.title, name="Ontology_title", curie=DCTERMS.curie('title'),
+                   model_uri=OMOSCHEMA.Ontology_title, domain=Ontology, range=Union[str, NarrativeText])
+
+slots.Ontology_license = Slot(uri=DCTERMS.license, name="Ontology_license", curie=DCTERMS.curie('license'),
+                   model_uri=OMOSCHEMA.Ontology_license, domain=Ontology, range=Union[dict, Thing])
+
+slots.Ontology_versionIRI = Slot(uri=OWL.versionIRI, name="Ontology_versionIRI", curie=OWL.curie('versionIRI'),
+                   model_uri=OMOSCHEMA.Ontology_versionIRI, domain=Ontology, range=Union[str, URIorCURIE])
+
+slots.Ontology_versionInfo = Slot(uri=OWL.versionInfo, name="Ontology_versionInfo", curie=OWL.curie('versionInfo'),
+                   model_uri=OMOSCHEMA.Ontology_versionInfo, domain=Ontology, range=str)
+
+slots.Class_label = Slot(uri=RDFS.label, name="Class_label", curie=RDFS.curie('label'),
+                   model_uri=OMOSCHEMA.Class_label, domain=Class, range=Union[str, LabelType])
+
+slots.Class_definition = Slot(uri=IAO['0000115'], name="Class_definition", curie=IAO.curie('0000115'),
+                   model_uri=OMOSCHEMA.Class_definition, domain=Class, range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]])
+
+slots.Class_broadMatch = Slot(uri=SKOS.broadMatch, name="Class_broadMatch", curie=SKOS.curie('broadMatch'),
+                   model_uri=OMOSCHEMA.Class_broadMatch, domain=Class, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.Class_exactMatch = Slot(uri=SKOS.exactMatch, name="Class_exactMatch", curie=SKOS.curie('exactMatch'),
+                   model_uri=OMOSCHEMA.Class_exactMatch, domain=Class, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.Class_narrowMatch = Slot(uri=SKOS.narrowMatch, name="Class_narrowMatch", curie=SKOS.curie('narrowMatch'),
+                   model_uri=OMOSCHEMA.Class_narrowMatch, domain=Class, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.Class_closeMatch = Slot(uri=SKOS.closeMatch, name="Class_closeMatch", curie=SKOS.curie('closeMatch'),
+                   model_uri=OMOSCHEMA.Class_closeMatch, domain=Class, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.Class_subClassOf = Slot(uri=RDFS.subClassOf, name="Class_subClassOf", curie=RDFS.curie('subClassOf'),
+                   model_uri=OMOSCHEMA.Class_subClassOf, domain=Class, range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]])
+
+slots.Property_label = Slot(uri=RDFS.label, name="Property_label", curie=RDFS.curie('label'),
+                   model_uri=OMOSCHEMA.Property_label, domain=Property, range=Optional[Union[str, LabelType]])
+
+slots.Property_definition = Slot(uri=IAO['0000115'], name="Property_definition", curie=IAO.curie('0000115'),
+                   model_uri=OMOSCHEMA.Property_definition, domain=Property, range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]])
+
+slots.Property_broadMatch = Slot(uri=SKOS.broadMatch, name="Property_broadMatch", curie=SKOS.curie('broadMatch'),
+                   model_uri=OMOSCHEMA.Property_broadMatch, domain=Property, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.Property_exactMatch = Slot(uri=SKOS.exactMatch, name="Property_exactMatch", curie=SKOS.curie('exactMatch'),
+                   model_uri=OMOSCHEMA.Property_exactMatch, domain=Property, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.Property_narrowMatch = Slot(uri=SKOS.narrowMatch, name="Property_narrowMatch", curie=SKOS.curie('narrowMatch'),
+                   model_uri=OMOSCHEMA.Property_narrowMatch, domain=Property, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.Property_closeMatch = Slot(uri=SKOS.closeMatch, name="Property_closeMatch", curie=SKOS.curie('closeMatch'),
+                   model_uri=OMOSCHEMA.Property_closeMatch, domain=Property, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.Property_subClassOf = Slot(uri=RDFS.subClassOf, name="Property_subClassOf", curie=RDFS.curie('subClassOf'),
+                   model_uri=OMOSCHEMA.Property_subClassOf, domain=Property, range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]])
+
+slots.HomoSapiens_id = Slot(uri=OMOSCHEMA.id, name="HomoSapiens_id", curie=OMOSCHEMA.curie('id'),
+                   model_uri=OMOSCHEMA.HomoSapiens_id, domain=HomoSapiens, range=Union[str, HomoSapiensId],
+                   pattern=re.compile(r'^orcid:.*'))
+
+slots.Agent_id = Slot(uri=OMOSCHEMA.id, name="Agent_id", curie=OMOSCHEMA.curie('id'),
+                   model_uri=OMOSCHEMA.Agent_id, domain=Agent, range=Union[str, AgentId],
+                   pattern=re.compile(r'^orcid:.*'))
+
+slots.Axiom_database_cross_reference = Slot(uri=OIO.hasDbXref, name="Axiom_database_cross_reference", curie=OIO.curie('hasDbXref'),
+                   model_uri=OMOSCHEMA.Axiom_database_cross_reference, domain=Axiom, range=Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]])
 
-slots.core_property = Slot(
-    uri=OMOSCHEMA.core_property,
-    name="core_property",
-    curie=OMOSCHEMA.curie("core_property"),
-    model_uri=OMOSCHEMA.core_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.id = Slot(
-    uri=OMOSCHEMA.id,
-    name="id",
-    curie=OMOSCHEMA.curie("id"),
-    model_uri=OMOSCHEMA.id,
-    domain=None,
-    range=URIRef,
-)
-
-slots.label = Slot(
-    uri=RDFS.label,
-    name="label",
-    curie=RDFS.curie("label"),
-    model_uri=OMOSCHEMA.label,
-    domain=None,
-    range=Optional[Union[str, LabelType]],
-)
-
-slots.annotations = Slot(
-    uri=OMOSCHEMA.annotations,
-    name="annotations",
-    curie=OMOSCHEMA.curie("annotations"),
-    model_uri=OMOSCHEMA.annotations,
-    domain=None,
-    range=Optional[Union[Union[dict, Annotation], List[Union[dict, Annotation]]]],
-)
-
-slots.definition = Slot(
-    uri=IAO["0000115"],
-    name="definition",
-    curie=IAO.curie("0000115"),
-    model_uri=OMOSCHEMA.definition,
-    domain=None,
-    range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]],
-)
-
-slots.predicate = Slot(
-    uri=OMOSCHEMA.predicate,
-    name="predicate",
-    curie=OMOSCHEMA.curie("predicate"),
-    model_uri=OMOSCHEMA.predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.object = Slot(
-    uri=OMOSCHEMA.object,
-    name="object",
-    curie=OMOSCHEMA.curie("object"),
-    model_uri=OMOSCHEMA.object,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.title = Slot(
-    uri=DCTERMS.title,
-    name="title",
-    curie=DCTERMS.curie("title"),
-    model_uri=OMOSCHEMA.title,
-    domain=None,
-    range=Optional[Union[str, NarrativeText]],
-)
-
-slots.match_aspect = Slot(
-    uri=OMOSCHEMA.match_aspect,
-    name="match_aspect",
-    curie=OMOSCHEMA.curie("match_aspect"),
-    model_uri=OMOSCHEMA.match_aspect,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.match = Slot(
-    uri=OMOSCHEMA.match,
-    name="match",
-    curie=OMOSCHEMA.curie("match"),
-    model_uri=OMOSCHEMA.match,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.broadMatch = Slot(
-    uri=SKOS.broadMatch,
-    name="broadMatch",
-    curie=SKOS.curie("broadMatch"),
-    model_uri=OMOSCHEMA.broadMatch,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.closeMatch = Slot(
-    uri=SKOS.closeMatch,
-    name="closeMatch",
-    curie=SKOS.curie("closeMatch"),
-    model_uri=OMOSCHEMA.closeMatch,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.exactMatch = Slot(
-    uri=SKOS.exactMatch,
-    name="exactMatch",
-    curie=SKOS.curie("exactMatch"),
-    model_uri=OMOSCHEMA.exactMatch,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.narrowMatch = Slot(
-    uri=SKOS.narrowMatch,
-    name="narrowMatch",
-    curie=SKOS.curie("narrowMatch"),
-    model_uri=OMOSCHEMA.narrowMatch,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.database_cross_reference = Slot(
-    uri=OIO.hasDbXref,
-    name="database_cross_reference",
-    curie=OIO.curie("hasDbXref"),
-    model_uri=OMOSCHEMA.database_cross_reference,
-    domain=None,
-    range=Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]],
-)
-
-slots.informative_property = Slot(
-    uri=OMOSCHEMA.informative_property,
-    name="informative_property",
-    curie=OMOSCHEMA.curie("informative_property"),
-    model_uri=OMOSCHEMA.informative_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.comment = Slot(
-    uri=RDFS.comment,
-    name="comment",
-    curie=RDFS.curie("comment"),
-    model_uri=OMOSCHEMA.comment,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.category = Slot(
-    uri=BIOLINK.category,
-    name="category",
-    curie=BIOLINK.curie("category"),
-    model_uri=OMOSCHEMA.category,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.image = Slot(
-    uri=SDO.image,
-    name="image",
-    curie=SDO.curie("image"),
-    model_uri=OMOSCHEMA.image,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.example_of_usage = Slot(
-    uri=IAO["0000112"],
-    name="example_of_usage",
-    curie=IAO.curie("0000112"),
-    model_uri=OMOSCHEMA.example_of_usage,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.changeNote = Slot(
-    uri=SKOS.changeNote,
-    name="changeNote",
-    curie=SKOS.curie("changeNote"),
-    model_uri=OMOSCHEMA.changeNote,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.has_curation_status = Slot(
-    uri=IAO["0000114"],
-    name="has_curation_status",
-    curie=IAO.curie("0000114"),
-    model_uri=OMOSCHEMA.has_curation_status,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.defaultLanguage = Slot(
-    uri=PROTEGE.defaultLanguage,
-    name="defaultLanguage",
-    curie=PROTEGE.curie("defaultLanguage"),
-    model_uri=OMOSCHEMA.defaultLanguage,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.language = Slot(
-    uri=DCTERMS.language,
-    name="language",
-    curie=DCTERMS.curie("language"),
-    model_uri=OMOSCHEMA.language,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.has_ontology_root_term = Slot(
-    uri=IAO["0000700"],
-    name="has_ontology_root_term",
-    curie=IAO.curie("0000700"),
-    model_uri=OMOSCHEMA.has_ontology_root_term,
-    domain=None,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.conformsTo = Slot(
-    uri=DCTERMS.conformsTo,
-    name="conformsTo",
-    curie=DCTERMS.curie("conformsTo"),
-    model_uri=OMOSCHEMA.conformsTo,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.license = Slot(
-    uri=DCTERMS.license,
-    name="license",
-    curie=DCTERMS.curie("license"),
-    model_uri=OMOSCHEMA.license,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.depicted_by = Slot(
-    uri=FOAF.depicted_by,
-    name="depicted_by",
-    curie=FOAF.curie("depicted_by"),
-    model_uri=OMOSCHEMA.depicted_by,
-    domain=None,
-    range=Optional[Union[Union[str, ImageId], List[Union[str, ImageId]]]],
-)
-
-slots.page = Slot(
-    uri=FOAF.page,
-    name="page",
-    curie=FOAF.curie("page"),
-    model_uri=OMOSCHEMA.page,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.version_property = Slot(
-    uri=OMOSCHEMA.version_property,
-    name="version_property",
-    curie=OMOSCHEMA.curie("version_property"),
-    model_uri=OMOSCHEMA.version_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.versionIRI = Slot(
-    uri=OWL.versionIRI,
-    name="versionIRI",
-    curie=OWL.curie("versionIRI"),
-    model_uri=OMOSCHEMA.versionIRI,
-    domain=None,
-    range=Optional[Union[str, URIorCURIE]],
-)
-
-slots.versionInfo = Slot(
-    uri=OWL.versionInfo,
-    name="versionInfo",
-    curie=OWL.curie("versionInfo"),
-    model_uri=OMOSCHEMA.versionInfo,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.obsoletion_related_property = Slot(
-    uri=OMOSCHEMA.obsoletion_related_property,
-    name="obsoletion_related_property",
-    curie=OMOSCHEMA.curie("obsoletion_related_property"),
-    model_uri=OMOSCHEMA.obsoletion_related_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.deprecated = Slot(
-    uri=OWL.deprecated,
-    name="deprecated",
-    curie=OWL.curie("deprecated"),
-    model_uri=OMOSCHEMA.deprecated,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.term_replaced_by = Slot(
-    uri=IAO["0100001"],
-    name="term_replaced_by",
-    curie=IAO.curie("0100001"),
-    model_uri=OMOSCHEMA.term_replaced_by,
-    domain=None,
-    range=Optional[Union[dict, Any]],
-)
-
-slots.has_obsolescence_reason = Slot(
-    uri=IAO["0000231"],
-    name="has_obsolescence_reason",
-    curie=IAO.curie("0000231"),
-    model_uri=OMOSCHEMA.has_obsolescence_reason,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.consider = Slot(
-    uri=OIO.consider,
-    name="consider",
-    curie=OIO.curie("consider"),
-    model_uri=OMOSCHEMA.consider,
-    domain=None,
-    range=Optional[Union[Union[dict, Any], List[Union[dict, Any]]]],
-)
-
-slots.has_alternative_id = Slot(
-    uri=OIO.hasAlternativeId,
-    name="has_alternative_id",
-    curie=OIO.curie("hasAlternativeId"),
-    model_uri=OMOSCHEMA.has_alternative_id,
-    domain=None,
-    range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]],
-)
-
-slots.temporal_interpretation = Slot(
-    uri=RO["0001900"],
-    name="temporal_interpretation",
-    curie=RO.curie("0001900"),
-    model_uri=OMOSCHEMA.temporal_interpretation,
-    domain=None,
-    range=Optional[Union[str, NamedIndividualId]],
-)
-
-slots.never_in_taxon = Slot(
-    uri=RO["0002161"],
-    name="never_in_taxon",
-    curie=RO.curie("0002161"),
-    model_uri=OMOSCHEMA.never_in_taxon,
-    domain=None,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.is_a_defining_property_chain_axiom = Slot(
-    uri=RO["0002581"],
-    name="is_a_defining_property_chain_axiom",
-    curie=RO.curie("0002581"),
-    model_uri=OMOSCHEMA.is_a_defining_property_chain_axiom,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive = Slot(
-    uri=RO["0002582"],
-    name="is_a_defining_property_chain_axiom_where_second_argument_is_reflexive",
-    curie=RO.curie("0002582"),
-    model_uri=OMOSCHEMA.is_a_defining_property_chain_axiom_where_second_argument_is_reflexive,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.provenance_property = Slot(
-    uri=OMOSCHEMA.provenance_property,
-    name="provenance_property",
-    curie=OMOSCHEMA.curie("provenance_property"),
-    model_uri=OMOSCHEMA.provenance_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.contributor = Slot(
-    uri=DCTERMS.contributor,
-    name="contributor",
-    curie=DCTERMS.curie("contributor"),
-    model_uri=OMOSCHEMA.contributor,
-    domain=None,
-    range=Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]],
-)
-
-slots.creator = Slot(
-    uri=DCTERMS.creator,
-    name="creator",
-    curie=DCTERMS.curie("creator"),
-    model_uri=OMOSCHEMA.creator,
-    domain=None,
-    range=Optional[Union[Union[str, AgentId], List[Union[str, AgentId]]]],
-)
-
-slots.created = Slot(
-    uri=DCTERMS.created,
-    name="created",
-    curie=DCTERMS.curie("created"),
-    model_uri=OMOSCHEMA.created,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.date = Slot(
-    uri=DCTERMS.date,
-    name="date",
-    curie=DCTERMS.curie("date"),
-    model_uri=OMOSCHEMA.date,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.source = Slot(
-    uri=DCTERMS.source,
-    name="source",
-    curie=DCTERMS.curie("source"),
-    model_uri=OMOSCHEMA.source,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.created_by = Slot(
-    uri=OIO.created_by,
-    name="created_by",
-    curie=OIO.curie("created_by"),
-    model_uri=OMOSCHEMA.created_by,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.creation_date = Slot(
-    uri=OIO.creation_date,
-    name="creation_date",
-    curie=OIO.curie("creation_date"),
-    model_uri=OMOSCHEMA.creation_date,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.date_retrieved = Slot(
-    uri=OIO.date_retrieved,
-    name="date_retrieved",
-    curie=OIO.curie("date_retrieved"),
-    model_uri=OMOSCHEMA.date_retrieved,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.editor_note = Slot(
-    uri=IAO["0000116"],
-    name="editor_note",
-    curie=IAO.curie("0000116"),
-    model_uri=OMOSCHEMA.editor_note,
-    domain=None,
-    range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]],
-)
-
-slots.term_editor = Slot(
-    uri=IAO["0000117"],
-    name="term_editor",
-    curie=IAO.curie("0000117"),
-    model_uri=OMOSCHEMA.term_editor,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.definition_source = Slot(
-    uri=IAO["0000119"],
-    name="definition_source",
-    curie=IAO.curie("0000119"),
-    model_uri=OMOSCHEMA.definition_source,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.curator_note = Slot(
-    uri=IAO["0000232"],
-    name="curator_note",
-    curie=IAO.curie("0000232"),
-    model_uri=OMOSCHEMA.curator_note,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.term_tracker_item = Slot(
-    uri=IAO["0000233"],
-    name="term_tracker_item",
-    curie=IAO.curie("0000233"),
-    model_uri=OMOSCHEMA.term_tracker_item,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.ontology_term_requester = Slot(
-    uri=IAO["0000234"],
-    name="ontology_term_requester",
-    curie=IAO.curie("0000234"),
-    model_uri=OMOSCHEMA.ontology_term_requester,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.imported_from = Slot(
-    uri=IAO["0000412"],
-    name="imported_from",
-    curie=IAO.curie("0000412"),
-    model_uri=OMOSCHEMA.imported_from,
-    domain=None,
-    range=Optional[Union[Union[str, NamedIndividualId], List[Union[str, NamedIndividualId]]]],
-)
-
-slots.has_axiom_label = Slot(
-    uri=IAO["0010000"],
-    name="has_axiom_label",
-    curie=IAO.curie("0010000"),
-    model_uri=OMOSCHEMA.has_axiom_label,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.shortcut_annotation_property = Slot(
-    uri=OMOSCHEMA.shortcut_annotation_property,
-    name="shortcut_annotation_property",
-    curie=OMOSCHEMA.curie("shortcut_annotation_property"),
-    model_uri=OMOSCHEMA.shortcut_annotation_property,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.disconnected_from = Slot(
-    uri=OMOSCHEMA.disconnected_from,
-    name="disconnected_from",
-    curie=OMOSCHEMA.curie("disconnected_from"),
-    model_uri=OMOSCHEMA.disconnected_from,
-    domain=None,
-    range=Optional[Union[str, ClassId]],
-)
-
-slots.excluded_axiom = Slot(
-    uri=OMOSCHEMA.excluded_axiom,
-    name="excluded_axiom",
-    curie=OMOSCHEMA.curie("excluded_axiom"),
-    model_uri=OMOSCHEMA.excluded_axiom,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.excluded_from_QC_check = Slot(
-    uri=OMOSCHEMA.excluded_from_QC_check,
-    name="excluded_from_QC_check",
-    curie=OMOSCHEMA.curie("excluded_from_QC_check"),
-    model_uri=OMOSCHEMA.excluded_from_QC_check,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.excluded_subClassOf = Slot(
-    uri=OMOSCHEMA.excluded_subClassOf,
-    name="excluded_subClassOf",
-    curie=OMOSCHEMA.curie("excluded_subClassOf"),
-    model_uri=OMOSCHEMA.excluded_subClassOf,
-    domain=None,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.excluded_synonym = Slot(
-    uri=OMOSCHEMA.excluded_synonym,
-    name="excluded_synonym",
-    curie=OMOSCHEMA.curie("excluded_synonym"),
-    model_uri=OMOSCHEMA.excluded_synonym,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.should_conform_to = Slot(
-    uri=OMOSCHEMA.should_conform_to,
-    name="should_conform_to",
-    curie=OMOSCHEMA.curie("should_conform_to"),
-    model_uri=OMOSCHEMA.should_conform_to,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.has_rank = Slot(
-    uri=OMOSCHEMA.has_rank,
-    name="has_rank",
-    curie=OMOSCHEMA.curie("has_rank"),
-    model_uri=OMOSCHEMA.has_rank,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.alternative_term = Slot(
-    uri=IAO["0000118"],
-    name="alternative_term",
-    curie=IAO.curie("0000118"),
-    model_uri=OMOSCHEMA.alternative_term,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.ISA_alternative_term = Slot(
-    uri=OBI["0001847"],
-    name="ISA_alternative_term",
-    curie=OBI.curie("0001847"),
-    model_uri=OMOSCHEMA.ISA_alternative_term,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.IEDB_alternative_term = Slot(
-    uri=OBI["9991118"],
-    name="IEDB_alternative_term",
-    curie=OBI.curie("9991118"),
-    model_uri=OMOSCHEMA.IEDB_alternative_term,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.OBO_foundry_unique_label = Slot(
-    uri=IAO["0000589"],
-    name="OBO_foundry_unique_label",
-    curie=IAO.curie("0000589"),
-    model_uri=OMOSCHEMA.OBO_foundry_unique_label,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.synonym = Slot(
-    uri=OIO.hasSynonym,
-    name="synonym",
-    curie=OIO.curie("hasSynonym"),
-    model_uri=OMOSCHEMA.synonym,
-    domain=None,
-    range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]],
-)
-
-slots.editor_preferred_term = Slot(
-    uri=IAO["0000111"],
-    name="editor_preferred_term",
-    curie=IAO.curie("0000111"),
-    model_uri=OMOSCHEMA.editor_preferred_term,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.has_exact_synonym = Slot(
-    uri=OIO.hasExactSynonym,
-    name="has_exact_synonym",
-    curie=OIO.curie("hasExactSynonym"),
-    model_uri=OMOSCHEMA.has_exact_synonym,
-    domain=None,
-    range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]],
-)
-
-slots.has_narrow_synonym = Slot(
-    uri=OIO.hasNarrowSynonym,
-    name="has_narrow_synonym",
-    curie=OIO.curie("hasNarrowSynonym"),
-    model_uri=OMOSCHEMA.has_narrow_synonym,
-    domain=None,
-    range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]],
-)
-
-slots.has_related_synonym = Slot(
-    uri=OIO.hasRelatedSynonym,
-    name="has_related_synonym",
-    curie=OIO.curie("hasRelatedSynonym"),
-    model_uri=OMOSCHEMA.has_related_synonym,
-    domain=None,
-    range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]],
-)
-
-slots.has_broad_synonym = Slot(
-    uri=OIO.hasBroadSynonym,
-    name="has_broad_synonym",
-    curie=OIO.curie("hasBroadSynonym"),
-    model_uri=OMOSCHEMA.has_broad_synonym,
-    domain=None,
-    range=Optional[Union[Union[str, LabelType], List[Union[str, LabelType]]]],
-)
-
-slots.has_synonym_type = Slot(
-    uri=OIO.hasSynonymType,
-    name="has_synonym_type",
-    curie=OIO.curie("hasSynonymType"),
-    model_uri=OMOSCHEMA.has_synonym_type,
-    domain=None,
-    range=Optional[Union[Union[str, AnnotationPropertyId], List[Union[str, AnnotationPropertyId]]]],
-)
-
-slots.has_obo_namespace = Slot(
-    uri=OIO.hasOBONamespace,
-    name="has_obo_namespace",
-    curie=OIO.curie("hasOBONamespace"),
-    model_uri=OMOSCHEMA.has_obo_namespace,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.in_subset = Slot(
-    uri=OIO.inSubset,
-    name="in_subset",
-    curie=OIO.curie("inSubset"),
-    model_uri=OMOSCHEMA.in_subset,
-    domain=None,
-    range=Optional[Union[Union[str, SubsetId], List[Union[str, SubsetId]]]],
-)
-
-slots.reification_predicate = Slot(
-    uri=OMOSCHEMA.reification_predicate,
-    name="reification_predicate",
-    curie=OMOSCHEMA.curie("reification_predicate"),
-    model_uri=OMOSCHEMA.reification_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.annotatedProperty = Slot(
-    uri=OWL.annotatedProperty,
-    name="annotatedProperty",
-    curie=OWL.curie("annotatedProperty"),
-    model_uri=OMOSCHEMA.annotatedProperty,
-    domain=None,
-    range=Optional[Union[str, AnnotationPropertyId]],
-)
-
-slots.annotatedSource = Slot(
-    uri=OWL.annotatedSource,
-    name="annotatedSource",
-    curie=OWL.curie("annotatedSource"),
-    model_uri=OMOSCHEMA.annotatedSource,
-    domain=None,
-    range=Optional[Union[str, NamedObjectId]],
-)
-
-slots.annotatedTarget = Slot(
-    uri=OWL.annotatedTarget,
-    name="annotatedTarget",
-    curie=OWL.curie("annotatedTarget"),
-    model_uri=OMOSCHEMA.annotatedTarget,
-    domain=None,
-    range=Optional[Union[dict, Any]],
-)
-
-slots.imports = Slot(
-    uri=OWL.imports,
-    name="imports",
-    curie=OWL.curie("imports"),
-    model_uri=OMOSCHEMA.imports,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.logical_predicate = Slot(
-    uri=OMOSCHEMA.logical_predicate,
-    name="logical_predicate",
-    curie=OMOSCHEMA.curie("logical_predicate"),
-    model_uri=OMOSCHEMA.logical_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.cardinality = Slot(
-    uri=OWL.cardinality,
-    name="cardinality",
-    curie=OWL.curie("cardinality"),
-    model_uri=OMOSCHEMA.cardinality,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.complementOf = Slot(
-    uri=OWL.complementOf,
-    name="complementOf",
-    curie=OWL.curie("complementOf"),
-    model_uri=OMOSCHEMA.complementOf,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.disjointWith = Slot(
-    uri=OWL.disjointWith,
-    name="disjointWith",
-    curie=OWL.curie("disjointWith"),
-    model_uri=OMOSCHEMA.disjointWith,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.distinctMembers = Slot(
-    uri=OWL.distinctMembers,
-    name="distinctMembers",
-    curie=OWL.curie("distinctMembers"),
-    model_uri=OMOSCHEMA.distinctMembers,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.equivalentClass = Slot(
-    uri=OWL.equivalentClass,
-    name="equivalentClass",
-    curie=OWL.curie("equivalentClass"),
-    model_uri=OMOSCHEMA.equivalentClass,
-    domain=None,
-    range=Optional[Union[Union[dict, ClassExpression], List[Union[dict, ClassExpression]]]],
-)
-
-slots.sameAs = Slot(
-    uri=OWL.sameAs,
-    name="sameAs",
-    curie=OWL.curie("sameAs"),
-    model_uri=OMOSCHEMA.sameAs,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.equivalentProperty = Slot(
-    uri=OWL.equivalentProperty,
-    name="equivalentProperty",
-    curie=OWL.curie("equivalentProperty"),
-    model_uri=OMOSCHEMA.equivalentProperty,
-    domain=None,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.hasValue = Slot(
-    uri=OWL.hasValue,
-    name="hasValue",
-    curie=OWL.curie("hasValue"),
-    model_uri=OMOSCHEMA.hasValue,
-    domain=None,
-    range=Optional[Union[dict, Any]],
-)
-
-slots.intersectionOf = Slot(
-    uri=OWL.intersectionOf,
-    name="intersectionOf",
-    curie=OWL.curie("intersectionOf"),
-    model_uri=OMOSCHEMA.intersectionOf,
-    domain=None,
-    range=Optional[Union[dict, ClassExpression]],
-)
-
-slots.inverseOf = Slot(
-    uri=OWL.inverseOf,
-    name="inverseOf",
-    curie=OWL.curie("inverseOf"),
-    model_uri=OMOSCHEMA.inverseOf,
-    domain=None,
-    range=Optional[Union[str, PropertyId]],
-)
-
-slots.maxQualifiedCardinality = Slot(
-    uri=OWL.maxQualifiedCardinality,
-    name="maxQualifiedCardinality",
-    curie=OWL.curie("maxQualifiedCardinality"),
-    model_uri=OMOSCHEMA.maxQualifiedCardinality,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.members = Slot(
-    uri=OWL.members,
-    name="members",
-    curie=OWL.curie("members"),
-    model_uri=OMOSCHEMA.members,
-    domain=None,
-    range=Optional[Union[dict, Thing]],
-)
-
-slots.minCardinality = Slot(
-    uri=OWL.minCardinality,
-    name="minCardinality",
-    curie=OWL.curie("minCardinality"),
-    model_uri=OMOSCHEMA.minCardinality,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.minQualifiedCardinality = Slot(
-    uri=OWL.minQualifiedCardinality,
-    name="minQualifiedCardinality",
-    curie=OWL.curie("minQualifiedCardinality"),
-    model_uri=OMOSCHEMA.minQualifiedCardinality,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.onClass = Slot(
-    uri=OWL.onClass,
-    name="onClass",
-    curie=OWL.curie("onClass"),
-    model_uri=OMOSCHEMA.onClass,
-    domain=None,
-    range=Optional[Union[dict, ClassExpression]],
-)
-
-slots.onProperty = Slot(
-    uri=OWL.onProperty,
-    name="onProperty",
-    curie=OWL.curie("onProperty"),
-    model_uri=OMOSCHEMA.onProperty,
-    domain=None,
-    range=Optional[Union[Union[dict, PropertyExpression], List[Union[dict, PropertyExpression]]]],
-)
-
-slots.oneOf = Slot(
-    uri=OWL.oneOf,
-    name="oneOf",
-    curie=OWL.curie("oneOf"),
-    model_uri=OMOSCHEMA.oneOf,
-    domain=None,
-    range=Optional[Union[dict, ClassExpression]],
-)
-
-slots.propertyChainAxiom = Slot(
-    uri=OWL.propertyChainAxiom,
-    name="propertyChainAxiom",
-    curie=OWL.curie("propertyChainAxiom"),
-    model_uri=OMOSCHEMA.propertyChainAxiom,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.qualifiedCardinality = Slot(
-    uri=OWL.qualifiedCardinality,
-    name="qualifiedCardinality",
-    curie=OWL.curie("qualifiedCardinality"),
-    model_uri=OMOSCHEMA.qualifiedCardinality,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.allValuesFrom = Slot(
-    uri=OWL.allValuesFrom,
-    name="allValuesFrom",
-    curie=OWL.curie("allValuesFrom"),
-    model_uri=OMOSCHEMA.allValuesFrom,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.someValuesFrom = Slot(
-    uri=OWL.someValuesFrom,
-    name="someValuesFrom",
-    curie=OWL.curie("someValuesFrom"),
-    model_uri=OMOSCHEMA.someValuesFrom,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.unionOf = Slot(
-    uri=OWL.unionOf,
-    name="unionOf",
-    curie=OWL.curie("unionOf"),
-    model_uri=OMOSCHEMA.unionOf,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.domain = Slot(
-    uri=RDFS.domain,
-    name="domain",
-    curie=RDFS.curie("domain"),
-    model_uri=OMOSCHEMA.domain,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.range = Slot(
-    uri=RDFS.range,
-    name="range",
-    curie=RDFS.curie("range"),
-    model_uri=OMOSCHEMA.range,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.isDefinedBy = Slot(
-    uri=RDFS.isDefinedBy,
-    name="isDefinedBy",
-    curie=RDFS.curie("isDefinedBy"),
-    model_uri=OMOSCHEMA.isDefinedBy,
-    domain=None,
-    range=Optional[Union[str, OntologyId]],
-)
-
-slots.seeAlso = Slot(
-    uri=RDFS.seeAlso,
-    name="seeAlso",
-    curie=RDFS.curie("seeAlso"),
-    model_uri=OMOSCHEMA.seeAlso,
-    domain=None,
-    range=Optional[Union[Union[dict, Thing], List[Union[dict, Thing]]]],
-)
-
-slots.type = Slot(
-    uri=RDF.type,
-    name="type",
-    curie=RDF.curie("type"),
-    model_uri=OMOSCHEMA.type,
-    domain=None,
-    range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]],
-)
-
-slots.subClassOf = Slot(
-    uri=RDFS.subClassOf,
-    name="subClassOf",
-    curie=RDFS.curie("subClassOf"),
-    model_uri=OMOSCHEMA.subClassOf,
-    domain=None,
-    range=Optional[Union[Union[dict, ClassExpression], List[Union[dict, ClassExpression]]]],
-)
-
-slots.oboInOwl_id = Slot(
-    uri=OIO.id,
-    name="oboInOwl_id",
-    curie=OIO.curie("id"),
-    model_uri=OMOSCHEMA.oboInOwl_id,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.oboInOwl_ontology = Slot(
-    uri=OIO.ontology,
-    name="oboInOwl_ontology",
-    curie=OIO.curie("ontology"),
-    model_uri=OMOSCHEMA.oboInOwl_ontology,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.is_class_level = Slot(
-    uri=OIO.is_class_level,
-    name="is_class_level",
-    curie=OIO.curie("is_class_level"),
-    model_uri=OMOSCHEMA.is_class_level,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.is_cyclic = Slot(
-    uri=OIO.is_cyclic,
-    name="is_cyclic",
-    curie=OIO.curie("is_cyclic"),
-    model_uri=OMOSCHEMA.is_cyclic,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.is_inferred = Slot(
-    uri=OIO.is_inferred,
-    name="is_inferred",
-    curie=OIO.curie("is_inferred"),
-    model_uri=OMOSCHEMA.is_inferred,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.is_metadata_tag = Slot(
-    uri=OIO.is_metadata_tag,
-    name="is_metadata_tag",
-    curie=OIO.curie("is_metadata_tag"),
-    model_uri=OMOSCHEMA.is_metadata_tag,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.is_transitive = Slot(
-    uri=OIO.is_transitive,
-    name="is_transitive",
-    curie=OIO.curie("is_transitive"),
-    model_uri=OMOSCHEMA.is_transitive,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.notes = Slot(
-    uri=OIO.notes,
-    name="notes",
-    curie=OIO.curie("notes"),
-    model_uri=OMOSCHEMA.notes,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.shorthand = Slot(
-    uri=OIO.shorthand,
-    name="shorthand",
-    curie=OIO.curie("shorthand"),
-    model_uri=OMOSCHEMA.shorthand,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.url = Slot(
-    uri=OIO.url,
-    name="url",
-    curie=OIO.curie("url"),
-    model_uri=OMOSCHEMA.url,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.evidence = Slot(
-    uri=OIO.evidence,
-    name="evidence",
-    curie=OIO.curie("evidence"),
-    model_uri=OMOSCHEMA.evidence,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.external_ontology = Slot(
-    uri=OIO.external_ontology,
-    name="external_ontology",
-    curie=OIO.curie("external_ontology"),
-    model_uri=OMOSCHEMA.external_ontology,
-    domain=None,
-    range=Optional[Union[str, List[str]]],
-)
-
-slots.NCIT_definition_source = Slot(
-    uri=NCIT.P378,
-    name="NCIT_definition_source",
-    curie=NCIT.curie("P378"),
-    model_uri=OMOSCHEMA.NCIT_definition_source,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.NCIT_term_type = Slot(
-    uri=NCIT.P383,
-    name="NCIT_term_type",
-    curie=NCIT.curie("P383"),
-    model_uri=OMOSCHEMA.NCIT_term_type,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.NCIT_term_source = Slot(
-    uri=NCIT.P384,
-    name="NCIT_term_source",
-    curie=NCIT.curie("P384"),
-    model_uri=OMOSCHEMA.NCIT_term_source,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.annotation__predicate = Slot(
-    uri=OMOSCHEMA.predicate,
-    name="annotation__predicate",
-    curie=OMOSCHEMA.curie("predicate"),
-    model_uri=OMOSCHEMA.annotation__predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.annotation__object = Slot(
-    uri=OMOSCHEMA.object,
-    name="annotation__object",
-    curie=OMOSCHEMA.curie("object"),
-    model_uri=OMOSCHEMA.annotation__object,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.Ontology_title = Slot(
-    uri=DCTERMS.title,
-    name="Ontology_title",
-    curie=DCTERMS.curie("title"),
-    model_uri=OMOSCHEMA.Ontology_title,
-    domain=Ontology,
-    range=Union[str, NarrativeText],
-)
-
-slots.Ontology_license = Slot(
-    uri=DCTERMS.license,
-    name="Ontology_license",
-    curie=DCTERMS.curie("license"),
-    model_uri=OMOSCHEMA.Ontology_license,
-    domain=Ontology,
-    range=Union[dict, Thing],
-)
-
-slots.Ontology_versionIRI = Slot(
-    uri=OWL.versionIRI,
-    name="Ontology_versionIRI",
-    curie=OWL.curie("versionIRI"),
-    model_uri=OMOSCHEMA.Ontology_versionIRI,
-    domain=Ontology,
-    range=Union[str, URIorCURIE],
-)
-
-slots.Ontology_versionInfo = Slot(
-    uri=OWL.versionInfo,
-    name="Ontology_versionInfo",
-    curie=OWL.curie("versionInfo"),
-    model_uri=OMOSCHEMA.Ontology_versionInfo,
-    domain=Ontology,
-    range=str,
-)
-
-slots.Class_label = Slot(
-    uri=RDFS.label,
-    name="Class_label",
-    curie=RDFS.curie("label"),
-    model_uri=OMOSCHEMA.Class_label,
-    domain=Class,
-    range=Union[str, LabelType],
-)
-
-slots.Class_definition = Slot(
-    uri=IAO["0000115"],
-    name="Class_definition",
-    curie=IAO.curie("0000115"),
-    model_uri=OMOSCHEMA.Class_definition,
-    domain=Class,
-    range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]],
-)
-
-slots.Class_broadMatch = Slot(
-    uri=SKOS.broadMatch,
-    name="Class_broadMatch",
-    curie=SKOS.curie("broadMatch"),
-    model_uri=OMOSCHEMA.Class_broadMatch,
-    domain=Class,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.Class_exactMatch = Slot(
-    uri=SKOS.exactMatch,
-    name="Class_exactMatch",
-    curie=SKOS.curie("exactMatch"),
-    model_uri=OMOSCHEMA.Class_exactMatch,
-    domain=Class,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.Class_narrowMatch = Slot(
-    uri=SKOS.narrowMatch,
-    name="Class_narrowMatch",
-    curie=SKOS.curie("narrowMatch"),
-    model_uri=OMOSCHEMA.Class_narrowMatch,
-    domain=Class,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.Class_closeMatch = Slot(
-    uri=SKOS.closeMatch,
-    name="Class_closeMatch",
-    curie=SKOS.curie("closeMatch"),
-    model_uri=OMOSCHEMA.Class_closeMatch,
-    domain=Class,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.Class_subClassOf = Slot(
-    uri=RDFS.subClassOf,
-    name="Class_subClassOf",
-    curie=RDFS.curie("subClassOf"),
-    model_uri=OMOSCHEMA.Class_subClassOf,
-    domain=Class,
-    range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
-)
-
-slots.Property_label = Slot(
-    uri=RDFS.label,
-    name="Property_label",
-    curie=RDFS.curie("label"),
-    model_uri=OMOSCHEMA.Property_label,
-    domain=Property,
-    range=Optional[Union[str, LabelType]],
-)
-
-slots.Property_definition = Slot(
-    uri=IAO["0000115"],
-    name="Property_definition",
-    curie=IAO.curie("0000115"),
-    model_uri=OMOSCHEMA.Property_definition,
-    domain=Property,
-    range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]],
-)
-
-slots.Property_broadMatch = Slot(
-    uri=SKOS.broadMatch,
-    name="Property_broadMatch",
-    curie=SKOS.curie("broadMatch"),
-    model_uri=OMOSCHEMA.Property_broadMatch,
-    domain=Property,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.Property_exactMatch = Slot(
-    uri=SKOS.exactMatch,
-    name="Property_exactMatch",
-    curie=SKOS.curie("exactMatch"),
-    model_uri=OMOSCHEMA.Property_exactMatch,
-    domain=Property,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.Property_narrowMatch = Slot(
-    uri=SKOS.narrowMatch,
-    name="Property_narrowMatch",
-    curie=SKOS.curie("narrowMatch"),
-    model_uri=OMOSCHEMA.Property_narrowMatch,
-    domain=Property,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.Property_closeMatch = Slot(
-    uri=SKOS.closeMatch,
-    name="Property_closeMatch",
-    curie=SKOS.curie("closeMatch"),
-    model_uri=OMOSCHEMA.Property_closeMatch,
-    domain=Property,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.Property_subClassOf = Slot(
-    uri=RDFS.subClassOf,
-    name="Property_subClassOf",
-    curie=RDFS.curie("subClassOf"),
-    model_uri=OMOSCHEMA.Property_subClassOf,
-    domain=Property,
-    range=Optional[Union[Union[str, PropertyId], List[Union[str, PropertyId]]]],
-)
-
-slots.HomoSapiens_id = Slot(
-    uri=OMOSCHEMA.id,
-    name="HomoSapiens_id",
-    curie=OMOSCHEMA.curie("id"),
-    model_uri=OMOSCHEMA.HomoSapiens_id,
-    domain=HomoSapiens,
-    range=Union[str, HomoSapiensId],
-    pattern=re.compile(r"^orcid:.*"),
-)
-
-slots.Agent_id = Slot(
-    uri=OMOSCHEMA.id,
-    name="Agent_id",
-    curie=OMOSCHEMA.curie("id"),
-    model_uri=OMOSCHEMA.Agent_id,
-    domain=Agent,
-    range=Union[str, AgentId],
-    pattern=re.compile(r"^orcid:.*"),
-)
-
-slots.Axiom_database_cross_reference = Slot(
-    uri=OIO.hasDbXref,
-    name="Axiom_database_cross_reference",
-    curie=OIO.curie("hasDbXref"),
-    model_uri=OMOSCHEMA.Axiom_database_cross_reference,
-    domain=Axiom,
-    range=Optional[Union[Union[str, CURIELiteral], List[Union[str, CURIELiteral]]]],
-)
-
-slots.ObsoleteAspect_label = Slot(
-    uri=RDFS.label,
-    name="ObsoleteAspect_label",
-    curie=RDFS.curie("label"),
-    model_uri=OMOSCHEMA.ObsoleteAspect_label,
-    domain=None,
-    range=Optional[Union[str, LabelType]],
-    pattern=re.compile(r"^obsolete"),
-)
+slots.ObsoleteAspect_label = Slot(uri=RDFS.label, name="ObsoleteAspect_label", curie=RDFS.curie('label'),
+                   model_uri=OMOSCHEMA.ObsoleteAspect_label, domain=None, range=Optional[Union[str, LabelType]],
+                   pattern=re.compile(r'^obsolete'))
```

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-id: http://purl.obolibrary.org/obo/omo/schema
+id: https://w3id.org/oak/ontology-metadata
 name: Ontology-Metadata
 title: Ontology Metadata Ontology Schema
 description: >-
   Schema for ontology metadata
 license: https://creativecommons.org/publicdomain/zero/1.0/
 version: 0.0.1
 
 default_curi_maps:
   - obo_context
   - semweb_context
   
 prefixes:
-  omoschema: http://purl.obolibrary.org/obo/omo/schema/
+  omoschema: https://w3id.org/oak/ontology-metadata/
   obo: http://purl.obolibrary.org/obo/
   RO: http://purl.obolibrary.org/obo/RO_
   OMO: http://purl.obolibrary.org/obo/OMO_
   IAO: http://purl.obolibrary.org/obo/IAO_
   OBI: http://purl.obolibrary.org/obo/OBI_
   NCIT: http://purl.obolibrary.org/obo/NCIT_
   NCBITaxon: http://purl.obolibrary.org/obo/NCBITaxon_
@@ -1305,8 +1305,33 @@
           A definition must not be circular
         meaning: omoschema:DCC.S7
       MatchTextAndLogical:
         is_a: DefinitionConstraint
         description: >-
           Text definitions and logical forms should match
         meaning: omoschema:DCC.S11
+      MatchTextAndLogicalGenusNotInText:
+        is_a: DefinitionConstraint
+        description: >-
+          The genus in the logical definition should be in the text definition
+        meaning: omoschema:DCC.S11.1
+      MatchTextAndLogicalDifferentiaNotInText:
+        is_a: DefinitionConstraint
+        description: >-
+          The differentia in the logical definition should be in the text definition
+        meaning: omoschema:DCC.S11.2
+      MatchTextAndReference:
+        is_a: DefinitionConstraint
+        description: >-
+          Text definitions and cited references and provenance for the text definition should match
+        meaning: omoschema:DCC.S20
+      ReferenceNotFound:
+        is_a: MatchTextAndReference
+        description: >-
+          The citation for the reference cannot be found
+        meaning: omoschema:DCC.S20.1
+      ReferenceIsRetracted:
+        is_a: MatchTextAndReference
+        description: >-
+          The citation for the reference is retracted
+        meaning: omoschema:DCC.S20.2
```

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/oxo.py` & `oaklib-0.6.3/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/search.py` & `oaklib-0.6.3/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/similarity.py` & `oaklib-0.6.3/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/synonymizer_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/synonymizer_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/synonymizer_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,78 +1,56 @@
 # Auto generated from validation_datamodel.yaml by pythongen.py version: 0.0.1
-# Generation date: 2024-03-07T21:21:02
+# Generation date: 2024-04-14T16:59:08
 # Schema: validaton-results
 #
 # id: https://w3id.org/linkml/validation_results
 # description: A datamodel for data validation results.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
+from jsonasobj2 import JsonObj, as_dict
+from typing import Optional, List, Union, Dict, ClassVar, Any
 from dataclasses import dataclass
-from typing import Any, ClassVar, Dict, List, Optional, Union
+from datetime import date, datetime
+from linkml_runtime.linkml_model.meta import EnumDefinition, PermissibleValue, PvFormulaOptions
 
-from jsonasobj2 import JsonObj, as_dict
-from linkml_runtime.linkml_model.meta import (
-    EnumDefinition,
-    PermissibleValue,
-    PvFormulaOptions,
-)
-from linkml_runtime.linkml_model.types import (
-    Boolean,
-    Float,
-    Integer,
-    String,
-    Uriorcurie,
-)
-from linkml_runtime.utils.curienamespace import CurieNamespace
-from linkml_runtime.utils.dataclass_extensions_376 import (
-    dataclasses_init_fn_with_kwargs,
-)
-from linkml_runtime.utils.enumerations import EnumDefinitionImpl
-from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import (
-    Bool,
-    URIorCURIE,
-    bnode,
-    empty_dict,
-    empty_list,
-)
 from linkml_runtime.utils.slot import Slot
-from linkml_runtime.utils.yamlutils import (
-    YAMLRoot,
-    extended_float,
-    extended_int,
-    extended_str,
-)
+from linkml_runtime.utils.metamodelcore import empty_list, empty_dict, bnode
+from linkml_runtime.utils.yamlutils import YAMLRoot, extended_str, extended_float, extended_int
+from linkml_runtime.utils.dataclass_extensions_376 import dataclasses_init_fn_with_kwargs
+from linkml_runtime.utils.formatutils import camelcase, underscore, sfx
+from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from rdflib import Namespace, URIRef
+from linkml_runtime.utils.curienamespace import CurieNamespace
+from linkml_runtime.linkml_model.types import Boolean, Float, Integer, String, Uriorcurie
+from linkml_runtime.utils.metamodelcore import Bool, URIorCURIE
 
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
-LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
-OWL = CurieNamespace("owl", "http://www.w3.org/2002/07/owl#")
-PAV = CurieNamespace("pav", "http://purl.org/pav/")
-RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
-RDFS = CurieNamespace("rdfs", "http://www.w3.org/2000/01/rdf-schema#")
-SCHEMA = CurieNamespace("schema", "http://schema.org/")
-SH = CurieNamespace("sh", "http://www.w3.org/ns/shacl#")
-SKOS = CurieNamespace("skos", "http://www.w3.org/2004/02/skos/core#")
-VM = CurieNamespace("vm", "https://w3id.org/linkml/validation-model/")
-XSD = CurieNamespace("xsd", "http://www.w3.org/2001/XMLSchema#")
+LINKML = CurieNamespace('linkml', 'https://w3id.org/linkml/')
+OWL = CurieNamespace('owl', 'http://www.w3.org/2002/07/owl#')
+PAV = CurieNamespace('pav', 'http://purl.org/pav/')
+RDF = CurieNamespace('rdf', 'http://www.w3.org/1999/02/22-rdf-syntax-ns#')
+RDFS = CurieNamespace('rdfs', 'http://www.w3.org/2000/01/rdf-schema#')
+SCHEMA = CurieNamespace('schema', 'http://schema.org/')
+SH = CurieNamespace('sh', 'http://www.w3.org/ns/shacl#')
+SKOS = CurieNamespace('skos', 'http://www.w3.org/2004/02/skos/core#')
+VM = CurieNamespace('vm', 'https://w3id.org/linkml/validation-model/')
+XSD = CurieNamespace('xsd', 'http://www.w3.org/2001/XMLSchema#')
 DEFAULT_ = VM
 
 
 # Types
 
-
 # Class references
 class NamedResourceId(URIorCURIE):
     pass
 
 
 class ConstraintComponentId(NamedResourceId):
     pass
@@ -147,90 +125,80 @@
 
 
 @dataclass
 class ValidationConfiguration(YAMLRoot):
     """
     Configuration parameters for execution of a validation report
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["ValidationConfiguration"]
     class_class_curie: ClassVar[str] = "vm:ValidationConfiguration"
     class_name: ClassVar[str] = "ValidationConfiguration"
     class_model_uri: ClassVar[URIRef] = VM.ValidationConfiguration
 
     max_number_results_per_type: Optional[int] = None
-    type_severity_map: Optional[
-        Union[
-            Dict[Union[str, TypeSeverityKeyValueType], Union[dict, "TypeSeverityKeyValue"]],
-            List[Union[dict, "TypeSeverityKeyValue"]],
-        ]
-    ] = empty_dict()
+    type_severity_map: Optional[Union[Dict[Union[str, TypeSeverityKeyValueType], Union[dict, "TypeSeverityKeyValue"]], List[Union[dict, "TypeSeverityKeyValue"]]]] = empty_dict()
     schema_path: Optional[str] = None
+    lookup_references: Optional[Union[bool, Bool]] = None
     prompt_info: Optional[str] = None
+    documentation_objects: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.max_number_results_per_type is not None and not isinstance(
-            self.max_number_results_per_type, int
-        ):
+        if self.max_number_results_per_type is not None and not isinstance(self.max_number_results_per_type, int):
             self.max_number_results_per_type = int(self.max_number_results_per_type)
 
-        self._normalize_inlined_as_dict(
-            slot_name="type_severity_map",
-            slot_type=TypeSeverityKeyValue,
-            key_name="type",
-            keyed=True,
-        )
+        self._normalize_inlined_as_dict(slot_name="type_severity_map", slot_type=TypeSeverityKeyValue, key_name="type", keyed=True)
 
         if self.schema_path is not None and not isinstance(self.schema_path, str):
             self.schema_path = str(self.schema_path)
 
+        if self.lookup_references is not None and not isinstance(self.lookup_references, Bool):
+            self.lookup_references = Bool(self.lookup_references)
+
         if self.prompt_info is not None and not isinstance(self.prompt_info, str):
             self.prompt_info = str(self.prompt_info)
 
+        if not isinstance(self.documentation_objects, list):
+            self.documentation_objects = [self.documentation_objects] if self.documentation_objects is not None else []
+        self.documentation_objects = [v if isinstance(v, str) else str(v) for v in self.documentation_objects]
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RepairConfiguration(YAMLRoot):
     """
     Configuration parameters for execution of validation repairs
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["RepairConfiguration"]
     class_class_curie: ClassVar[str] = "vm:RepairConfiguration"
     class_name: ClassVar[str] = "RepairConfiguration"
     class_model_uri: ClassVar[URIRef] = VM.RepairConfiguration
 
     validation_configuration: Optional[Union[dict, ValidationConfiguration]] = None
     dry_run: Optional[Union[bool, Bool]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.validation_configuration is not None and not isinstance(
-            self.validation_configuration, ValidationConfiguration
-        ):
-            self.validation_configuration = ValidationConfiguration(
-                **as_dict(self.validation_configuration)
-            )
+        if self.validation_configuration is not None and not isinstance(self.validation_configuration, ValidationConfiguration):
+            self.validation_configuration = ValidationConfiguration(**as_dict(self.validation_configuration))
 
         if self.dry_run is not None and not isinstance(self.dry_run, Bool):
             self.dry_run = Bool(self.dry_run)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class TypeSeverityKeyValue(YAMLRoot):
     """
     key-value pair that maps a validation result type to a severity setting, for overriding default severity
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["TypeSeverityKeyValue"]
     class_class_curie: ClassVar[str] = "vm:TypeSeverityKeyValue"
     class_name: ClassVar[str] = "TypeSeverityKeyValue"
     class_model_uri: ClassVar[URIRef] = VM.TypeSeverityKeyValue
 
@@ -250,15 +218,14 @@
 
 
 @dataclass
 class Report(YAMLRoot):
     """
     A report object that is a holder to multiple report results
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["Report"]
     class_class_curie: ClassVar[str] = "vm:Report"
     class_name: ClassVar[str] = "Report"
     class_model_uri: ClassVar[URIRef] = VM.Report
 
@@ -273,84 +240,70 @@
 
 
 @dataclass
 class ValidationReport(Report):
     """
     A report that consists of validation results
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SH["ValidationReport"]
     class_class_curie: ClassVar[str] = "sh:ValidationReport"
     class_name: ClassVar[str] = "ValidationReport"
     class_model_uri: ClassVar[URIRef] = VM.ValidationReport
 
-    results: Optional[
-        Union[Union[dict, "ValidationResult"], List[Union[dict, "ValidationResult"]]]
-    ] = empty_list()
+    results: Optional[Union[Union[dict, "ValidationResult"], List[Union[dict, "ValidationResult"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.results, list):
             self.results = [self.results] if self.results is not None else []
-        self.results = [
-            v if isinstance(v, ValidationResult) else ValidationResult(**as_dict(v))
-            for v in self.results
-        ]
+        self.results = [v if isinstance(v, ValidationResult) else ValidationResult(**as_dict(v)) for v in self.results]
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RepairReport(Report):
     """
     A report that consists of repair operation results
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["RepairReport"]
     class_class_curie: ClassVar[str] = "vm:RepairReport"
     class_name: ClassVar[str] = "RepairReport"
     class_model_uri: ClassVar[URIRef] = VM.RepairReport
 
-    results: Optional[
-        Union[Union[dict, "RepairOperation"], List[Union[dict, "RepairOperation"]]]
-    ] = empty_list()
+    results: Optional[Union[Union[dict, "RepairOperation"], List[Union[dict, "RepairOperation"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.results, list):
             self.results = [self.results] if self.results is not None else []
-        self.results = [
-            v if isinstance(v, RepairOperation) else RepairOperation(**as_dict(v))
-            for v in self.results
-        ]
+        self.results = [v if isinstance(v, RepairOperation) else RepairOperation(**as_dict(v)) for v in self.results]
 
         super().__post_init__(**kwargs)
 
 
 class Result(YAMLRoot):
     """
     Abstract base class for any individual report result
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["Result"]
     class_class_curie: ClassVar[str] = "vm:Result"
     class_name: ClassVar[str] = "Result"
     class_model_uri: ClassVar[URIRef] = VM.Result
 
 
 @dataclass
 class ValidationResult(Result):
     """
     An individual result arising from validation of a data instance using a particular rule
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SH["ValidationResult"]
     class_class_curie: ClassVar[str] = "sh:ValidationResult"
     class_name: ClassVar[str] = "ValidationResult"
     class_model_uri: ClassVar[URIRef] = VM.ValidationResult
 
@@ -396,19 +349,46 @@
         if self.info is not None and not isinstance(self.info, str):
             self.info = str(self.info)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
+class DefinitionValidationResult(ValidationResult):
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = VM["DefinitionValidationResult"]
+    class_class_curie: ClassVar[str] = "vm:DefinitionValidationResult"
+    class_name: ClassVar[str] = "DefinitionValidationResult"
+    class_model_uri: ClassVar[URIRef] = VM.DefinitionValidationResult
+
+    type: Union[str, ConstraintComponentId] = None
+    subject: Union[str, NodeId] = None
+    definition: Optional[str] = None
+    definition_source: Optional[str] = None
+    proposed_new_definition: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.definition is not None and not isinstance(self.definition, str):
+            self.definition = str(self.definition)
+
+        if self.definition_source is not None and not isinstance(self.definition_source, str):
+            self.definition_source = str(self.definition_source)
+
+        if self.proposed_new_definition is not None and not isinstance(self.proposed_new_definition, str):
+            self.proposed_new_definition = str(self.proposed_new_definition)
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
 class MappingValidationResult(Result):
     """
     A validation result where the check is to determine if a mapping is correct
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["MappingValidationResult"]
     class_class_curie: ClassVar[str] = "vm:MappingValidationResult"
     class_name: ClassVar[str] = "MappingValidationResult"
     class_model_uri: ClassVar[URIRef] = VM.MappingValidationResult
 
@@ -451,28 +431,25 @@
 
         if self.confidence is not None and not isinstance(self.confidence, float):
             self.confidence = float(self.confidence)
 
         if self.suggested_predicate is not None and not isinstance(self.suggested_predicate, str):
             self.suggested_predicate = str(self.suggested_predicate)
 
-        if self.suggested_modifications is not None and not isinstance(
-            self.suggested_modifications, str
-        ):
+        if self.suggested_modifications is not None and not isinstance(self.suggested_modifications, str):
             self.suggested_modifications = str(self.suggested_modifications)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class RepairOperation(Result):
     """
     The result of performing an individual repair
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["RepairOperation"]
     class_class_curie: ClassVar[str] = "vm:RepairOperation"
     class_name: ClassVar[str] = "RepairOperation"
     class_model_uri: ClassVar[URIRef] = VM.RepairOperation
 
@@ -498,15 +475,14 @@
 
 
 @dataclass
 class ExternalReferenceValidationResult(ValidationResult):
     """
     A validation result where the check is to determine if a link to an external resource is still valid
     """
-
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = VM["ExternalReferenceValidationResult"]
     class_class_curie: ClassVar[str] = "vm:ExternalReferenceValidationResult"
     class_name: ClassVar[str] = "ExternalReferenceValidationResult"
     class_model_uri: ClassVar[URIRef] = VM.ExternalReferenceValidationResult
 
@@ -533,437 +509,201 @@
         super().__post_init__(**kwargs)
 
 
 # Enumerations
 class SeverityOptions(EnumDefinitionImpl):
 
     FATAL = PermissibleValue(text="FATAL")
-    ERROR = PermissibleValue(text="ERROR", meaning=SH["Violation"])
-    WARNING = PermissibleValue(text="WARNING", meaning=SH["Warning"])
-    INFO = PermissibleValue(text="INFO", meaning=SH["Info"])
+    ERROR = PermissibleValue(
+        text="ERROR",
+        meaning=SH["Violation"])
+    WARNING = PermissibleValue(
+        text="WARNING",
+        meaning=SH["Warning"])
+    INFO = PermissibleValue(
+        text="INFO",
+        meaning=SH["Info"])
 
     _defn = EnumDefinition(
         name="SeverityOptions",
     )
 
-
 class ValidationResultType(EnumDefinitionImpl):
 
     DatatypeConstraintComponent = PermissibleValue(
         text="DatatypeConstraintComponent",
         description="constraint in which the range is a type, and the slot value must conform to the type",
-        meaning=SH["DatatypeConstraintComponent"],
-    )
+        meaning=SH["DatatypeConstraintComponent"])
     MinCountConstraintComponent = PermissibleValue(
         text="MinCountConstraintComponent",
         description="cardinality constraint where the slot value must be greater or equal to a specified minimum",
-        meaning=SH["MinCountConstraintComponent"],
-    )
+        meaning=SH["MinCountConstraintComponent"])
     MaxCountConstraintComponent = PermissibleValue(
         text="MaxCountConstraintComponent",
         description="cardinality constraint where the slot value must be less than or equal to a specified maximum",
-        meaning=SH["MaxCountConstraintComponent"],
-    )
+        meaning=SH["MaxCountConstraintComponent"])
     DeprecatedPropertyComponent = PermissibleValue(
         text="DeprecatedPropertyComponent",
         description="constraint where the instance slot should not be deprecated",
-        meaning=VM["DeprecatedPropertyComponent"],
-    )
+        meaning=VM["DeprecatedPropertyComponent"])
     MaxLengthConstraintComponent = PermissibleValue(
         text="MaxLengthConstraintComponent",
         description="constraint where the slot value must have a length equal to or less than a specified maximum",
-        meaning=SH["MaxLengthConstraintComponent"],
-    )
+        meaning=SH["MaxLengthConstraintComponent"])
     MinLengthConstraintComponent = PermissibleValue(
         text="MinLengthConstraintComponent",
         description="constraint where the slot value must have a length equal to or less than a specified maximum",
-        meaning=SH["MinLengthConstraintComponent"],
-    )
+        meaning=SH["MinLengthConstraintComponent"])
     PatternConstraintComponent = PermissibleValue(
         text="PatternConstraintComponent",
         description="constraint where the slot value must match a given regular expression pattern",
-        meaning=SH["PatternConstraintComponent"],
-    )
+        meaning=SH["PatternConstraintComponent"])
     ClosedConstraintComponent = PermissibleValue(
         text="ClosedConstraintComponent",
         description="constraint where the slot value must be allowable for the type of an instance",
-        meaning=SH["ClosedConstraintComponent"],
-    )
+        meaning=SH["ClosedConstraintComponent"])
     RuleConstraintComponent = PermissibleValue(
         text="RuleConstraintComponent",
-        description="constraint where the structure of an object must conform to a specified rule",
-    )
+        description="constraint where the structure of an object must conform to a specified rule")
 
     _defn = EnumDefinition(
         name="ValidationResultType",
     )
 
-
 # Slots
 class slots:
     pass
 
+slots.type = Slot(uri=SH.sourceConstraintComponent, name="type", curie=SH.curie('sourceConstraintComponent'),
+                   model_uri=VM.type, domain=None, range=Union[str, ConstraintComponentId])
+
+slots.subject = Slot(uri=SH.focusNode, name="subject", curie=SH.curie('focusNode'),
+                   model_uri=VM.subject, domain=None, range=Union[str, NodeId])
+
+slots.instantiates = Slot(uri=VM.instantiates, name="instantiates", curie=VM.curie('instantiates'),
+                   model_uri=VM.instantiates, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.predicate = Slot(uri=VM.predicate, name="predicate", curie=VM.curie('predicate'),
+                   model_uri=VM.predicate, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.object = Slot(uri=SH.value, name="object", curie=SH.curie('value'),
+                   model_uri=VM.object, domain=None, range=Optional[Union[str, NodeId]])
+
+slots.object_str = Slot(uri=VM.object_str, name="object_str", curie=VM.curie('object_str'),
+                   model_uri=VM.object_str, domain=None, range=Optional[str])
+
+slots.source = Slot(uri=VM.source, name="source", curie=VM.curie('source'),
+                   model_uri=VM.source, domain=None, range=Optional[str])
+
+slots.severity = Slot(uri=SH.resultSeverity, name="severity", curie=SH.curie('resultSeverity'),
+                   model_uri=VM.severity, domain=None, range=Optional[Union[str, "SeverityOptions"]])
+
+slots.info = Slot(uri=SH.resultMessage, name="info", curie=SH.curie('resultMessage'),
+                   model_uri=VM.info, domain=None, range=Optional[str])
+
+slots.results = Slot(uri=SH.result, name="results", curie=SH.curie('result'),
+                   model_uri=VM.results, domain=None, range=Optional[Union[Union[dict, Result], List[Union[dict, Result]]]])
+
+slots.namedResource__id = Slot(uri=VM.id, name="namedResource__id", curie=VM.curie('id'),
+                   model_uri=VM.namedResource__id, domain=None, range=URIRef)
+
+slots.validationConfiguration__max_number_results_per_type = Slot(uri=VM.max_number_results_per_type, name="validationConfiguration__max_number_results_per_type", curie=VM.curie('max_number_results_per_type'),
+                   model_uri=VM.validationConfiguration__max_number_results_per_type, domain=None, range=Optional[int])
+
+slots.validationConfiguration__type_severity_map = Slot(uri=VM.type_severity_map, name="validationConfiguration__type_severity_map", curie=VM.curie('type_severity_map'),
+                   model_uri=VM.validationConfiguration__type_severity_map, domain=None, range=Optional[Union[Dict[Union[str, TypeSeverityKeyValueType], Union[dict, TypeSeverityKeyValue]], List[Union[dict, TypeSeverityKeyValue]]]])
+
+slots.validationConfiguration__schema_path = Slot(uri=VM.schema_path, name="validationConfiguration__schema_path", curie=VM.curie('schema_path'),
+                   model_uri=VM.validationConfiguration__schema_path, domain=None, range=Optional[str])
+
+slots.validationConfiguration__lookup_references = Slot(uri=VM.lookup_references, name="validationConfiguration__lookup_references", curie=VM.curie('lookup_references'),
+                   model_uri=VM.validationConfiguration__lookup_references, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.validationConfiguration__prompt_info = Slot(uri=VM.prompt_info, name="validationConfiguration__prompt_info", curie=VM.curie('prompt_info'),
+                   model_uri=VM.validationConfiguration__prompt_info, domain=None, range=Optional[str])
+
+slots.validationConfiguration__documentation_objects = Slot(uri=VM.documentation_objects, name="validationConfiguration__documentation_objects", curie=VM.curie('documentation_objects'),
+                   model_uri=VM.validationConfiguration__documentation_objects, domain=None, range=Optional[Union[str, List[str]]])
+
+slots.repairConfiguration__validation_configuration = Slot(uri=VM.validation_configuration, name="repairConfiguration__validation_configuration", curie=VM.curie('validation_configuration'),
+                   model_uri=VM.repairConfiguration__validation_configuration, domain=None, range=Optional[Union[dict, ValidationConfiguration]])
+
+slots.repairConfiguration__dry_run = Slot(uri=VM.dry_run, name="repairConfiguration__dry_run", curie=VM.curie('dry_run'),
+                   model_uri=VM.repairConfiguration__dry_run, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.typeSeverityKeyValue__type = Slot(uri=VM.type, name="typeSeverityKeyValue__type", curie=VM.curie('type'),
+                   model_uri=VM.typeSeverityKeyValue__type, domain=None, range=URIRef)
+
+slots.typeSeverityKeyValue__severity = Slot(uri=VM.severity, name="typeSeverityKeyValue__severity", curie=VM.curie('severity'),
+                   model_uri=VM.typeSeverityKeyValue__severity, domain=None, range=Optional[Union[str, "SeverityOptions"]])
+
+slots.definitionValidationResult__definition = Slot(uri=VM.definition, name="definitionValidationResult__definition", curie=VM.curie('definition'),
+                   model_uri=VM.definitionValidationResult__definition, domain=None, range=Optional[str])
+
+slots.definitionValidationResult__definition_source = Slot(uri=VM.definition_source, name="definitionValidationResult__definition_source", curie=VM.curie('definition_source'),
+                   model_uri=VM.definitionValidationResult__definition_source, domain=None, range=Optional[str])
+
+slots.definitionValidationResult__proposed_new_definition = Slot(uri=VM.proposed_new_definition, name="definitionValidationResult__proposed_new_definition", curie=VM.curie('proposed_new_definition'),
+                   model_uri=VM.definitionValidationResult__proposed_new_definition, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__subject_id = Slot(uri=VM.subject_id, name="mappingValidationResult__subject_id", curie=VM.curie('subject_id'),
+                   model_uri=VM.mappingValidationResult__subject_id, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__subject_info = Slot(uri=VM.subject_info, name="mappingValidationResult__subject_info", curie=VM.curie('subject_info'),
+                   model_uri=VM.mappingValidationResult__subject_info, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__object_id = Slot(uri=VM.object_id, name="mappingValidationResult__object_id", curie=VM.curie('object_id'),
+                   model_uri=VM.mappingValidationResult__object_id, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__object_info = Slot(uri=VM.object_info, name="mappingValidationResult__object_info", curie=VM.curie('object_info'),
+                   model_uri=VM.mappingValidationResult__object_info, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__predicate_id = Slot(uri=VM.predicate_id, name="mappingValidationResult__predicate_id", curie=VM.curie('predicate_id'),
+                   model_uri=VM.mappingValidationResult__predicate_id, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__category = Slot(uri=VM.category, name="mappingValidationResult__category", curie=VM.curie('category'),
+                   model_uri=VM.mappingValidationResult__category, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__problem = Slot(uri=VM.problem, name="mappingValidationResult__problem", curie=VM.curie('problem'),
+                   model_uri=VM.mappingValidationResult__problem, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.mappingValidationResult__info = Slot(uri=VM.info, name="mappingValidationResult__info", curie=VM.curie('info'),
+                   model_uri=VM.mappingValidationResult__info, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__confidence = Slot(uri=VM.confidence, name="mappingValidationResult__confidence", curie=VM.curie('confidence'),
+                   model_uri=VM.mappingValidationResult__confidence, domain=None, range=Optional[float])
+
+slots.mappingValidationResult__suggested_predicate = Slot(uri=VM.suggested_predicate, name="mappingValidationResult__suggested_predicate", curie=VM.curie('suggested_predicate'),
+                   model_uri=VM.mappingValidationResult__suggested_predicate, domain=None, range=Optional[str])
+
+slots.mappingValidationResult__suggested_modifications = Slot(uri=VM.suggested_modifications, name="mappingValidationResult__suggested_modifications", curie=VM.curie('suggested_modifications'),
+                   model_uri=VM.mappingValidationResult__suggested_modifications, domain=None, range=Optional[str])
+
+slots.repairOperation__repairs = Slot(uri=VM.repairs, name="repairOperation__repairs", curie=VM.curie('repairs'),
+                   model_uri=VM.repairOperation__repairs, domain=None, range=Optional[Union[dict, ValidationResult]])
+
+slots.repairOperation__modified = Slot(uri=VM.modified, name="repairOperation__modified", curie=VM.curie('modified'),
+                   model_uri=VM.repairOperation__modified, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.repairOperation__successful = Slot(uri=VM.successful, name="repairOperation__successful", curie=VM.curie('successful'),
+                   model_uri=VM.repairOperation__successful, domain=None, range=Optional[Union[bool, Bool]])
+
+slots.repairOperation__info = Slot(uri=VM.info, name="repairOperation__info", curie=VM.curie('info'),
+                   model_uri=VM.repairOperation__info, domain=None, range=Optional[str])
+
+slots.externalReferenceValidationResult__url = Slot(uri=VM.url, name="externalReferenceValidationResult__url", curie=VM.curie('url'),
+                   model_uri=VM.externalReferenceValidationResult__url, domain=None, range=Optional[str])
+
+slots.externalReferenceValidationResult__time_checked = Slot(uri=VM.time_checked, name="externalReferenceValidationResult__time_checked", curie=VM.curie('time_checked'),
+                   model_uri=VM.externalReferenceValidationResult__time_checked, domain=None, range=Optional[str])
+
+slots.externalReferenceValidationResult__number_of_attempts = Slot(uri=VM.number_of_attempts, name="externalReferenceValidationResult__number_of_attempts", curie=VM.curie('number_of_attempts'),
+                   model_uri=VM.externalReferenceValidationResult__number_of_attempts, domain=None, range=Optional[int])
+
+slots.externalReferenceValidationResult__http_response_code = Slot(uri=VM.http_response_code, name="externalReferenceValidationResult__http_response_code", curie=VM.curie('http_response_code'),
+                   model_uri=VM.externalReferenceValidationResult__http_response_code, domain=None, range=Optional[int])
+
+slots.ValidationReport_results = Slot(uri=SH.result, name="ValidationReport_results", curie=SH.curie('result'),
+                   model_uri=VM.ValidationReport_results, domain=ValidationReport, range=Optional[Union[Union[dict, "ValidationResult"], List[Union[dict, "ValidationResult"]]]])
 
-slots.type = Slot(
-    uri=SH.sourceConstraintComponent,
-    name="type",
-    curie=SH.curie("sourceConstraintComponent"),
-    model_uri=VM.type,
-    domain=None,
-    range=Union[str, ConstraintComponentId],
-)
-
-slots.subject = Slot(
-    uri=SH.focusNode,
-    name="subject",
-    curie=SH.curie("focusNode"),
-    model_uri=VM.subject,
-    domain=None,
-    range=Union[str, NodeId],
-)
-
-slots.instantiates = Slot(
-    uri=VM.instantiates,
-    name="instantiates",
-    curie=VM.curie("instantiates"),
-    model_uri=VM.instantiates,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.predicate = Slot(
-    uri=VM.predicate,
-    name="predicate",
-    curie=VM.curie("predicate"),
-    model_uri=VM.predicate,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.object = Slot(
-    uri=SH.value,
-    name="object",
-    curie=SH.curie("value"),
-    model_uri=VM.object,
-    domain=None,
-    range=Optional[Union[str, NodeId]],
-)
-
-slots.object_str = Slot(
-    uri=VM.object_str,
-    name="object_str",
-    curie=VM.curie("object_str"),
-    model_uri=VM.object_str,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.source = Slot(
-    uri=VM.source,
-    name="source",
-    curie=VM.curie("source"),
-    model_uri=VM.source,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.severity = Slot(
-    uri=SH.resultSeverity,
-    name="severity",
-    curie=SH.curie("resultSeverity"),
-    model_uri=VM.severity,
-    domain=None,
-    range=Optional[Union[str, "SeverityOptions"]],
-)
-
-slots.info = Slot(
-    uri=SH.resultMessage,
-    name="info",
-    curie=SH.curie("resultMessage"),
-    model_uri=VM.info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.results = Slot(
-    uri=SH.result,
-    name="results",
-    curie=SH.curie("result"),
-    model_uri=VM.results,
-    domain=None,
-    range=Optional[Union[Union[dict, Result], List[Union[dict, Result]]]],
-)
-
-slots.namedResource__id = Slot(
-    uri=VM.id,
-    name="namedResource__id",
-    curie=VM.curie("id"),
-    model_uri=VM.namedResource__id,
-    domain=None,
-    range=URIRef,
-)
-
-slots.validationConfiguration__max_number_results_per_type = Slot(
-    uri=VM.max_number_results_per_type,
-    name="validationConfiguration__max_number_results_per_type",
-    curie=VM.curie("max_number_results_per_type"),
-    model_uri=VM.validationConfiguration__max_number_results_per_type,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.validationConfiguration__type_severity_map = Slot(
-    uri=VM.type_severity_map,
-    name="validationConfiguration__type_severity_map",
-    curie=VM.curie("type_severity_map"),
-    model_uri=VM.validationConfiguration__type_severity_map,
-    domain=None,
-    range=Optional[
-        Union[
-            Dict[Union[str, TypeSeverityKeyValueType], Union[dict, TypeSeverityKeyValue]],
-            List[Union[dict, TypeSeverityKeyValue]],
-        ]
-    ],
-)
-
-slots.validationConfiguration__schema_path = Slot(
-    uri=VM.schema_path,
-    name="validationConfiguration__schema_path",
-    curie=VM.curie("schema_path"),
-    model_uri=VM.validationConfiguration__schema_path,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.validationConfiguration__prompt_info = Slot(
-    uri=VM.prompt_info,
-    name="validationConfiguration__prompt_info",
-    curie=VM.curie("prompt_info"),
-    model_uri=VM.validationConfiguration__prompt_info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.repairConfiguration__validation_configuration = Slot(
-    uri=VM.validation_configuration,
-    name="repairConfiguration__validation_configuration",
-    curie=VM.curie("validation_configuration"),
-    model_uri=VM.repairConfiguration__validation_configuration,
-    domain=None,
-    range=Optional[Union[dict, ValidationConfiguration]],
-)
-
-slots.repairConfiguration__dry_run = Slot(
-    uri=VM.dry_run,
-    name="repairConfiguration__dry_run",
-    curie=VM.curie("dry_run"),
-    model_uri=VM.repairConfiguration__dry_run,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.typeSeverityKeyValue__type = Slot(
-    uri=VM.type,
-    name="typeSeverityKeyValue__type",
-    curie=VM.curie("type"),
-    model_uri=VM.typeSeverityKeyValue__type,
-    domain=None,
-    range=URIRef,
-)
-
-slots.typeSeverityKeyValue__severity = Slot(
-    uri=VM.severity,
-    name="typeSeverityKeyValue__severity",
-    curie=VM.curie("severity"),
-    model_uri=VM.typeSeverityKeyValue__severity,
-    domain=None,
-    range=Optional[Union[str, "SeverityOptions"]],
-)
-
-slots.mappingValidationResult__subject_id = Slot(
-    uri=VM.subject_id,
-    name="mappingValidationResult__subject_id",
-    curie=VM.curie("subject_id"),
-    model_uri=VM.mappingValidationResult__subject_id,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__subject_info = Slot(
-    uri=VM.subject_info,
-    name="mappingValidationResult__subject_info",
-    curie=VM.curie("subject_info"),
-    model_uri=VM.mappingValidationResult__subject_info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__object_id = Slot(
-    uri=VM.object_id,
-    name="mappingValidationResult__object_id",
-    curie=VM.curie("object_id"),
-    model_uri=VM.mappingValidationResult__object_id,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__object_info = Slot(
-    uri=VM.object_info,
-    name="mappingValidationResult__object_info",
-    curie=VM.curie("object_info"),
-    model_uri=VM.mappingValidationResult__object_info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__predicate_id = Slot(
-    uri=VM.predicate_id,
-    name="mappingValidationResult__predicate_id",
-    curie=VM.curie("predicate_id"),
-    model_uri=VM.mappingValidationResult__predicate_id,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__category = Slot(
-    uri=VM.category,
-    name="mappingValidationResult__category",
-    curie=VM.curie("category"),
-    model_uri=VM.mappingValidationResult__category,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__problem = Slot(
-    uri=VM.problem,
-    name="mappingValidationResult__problem",
-    curie=VM.curie("problem"),
-    model_uri=VM.mappingValidationResult__problem,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.mappingValidationResult__info = Slot(
-    uri=VM.info,
-    name="mappingValidationResult__info",
-    curie=VM.curie("info"),
-    model_uri=VM.mappingValidationResult__info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__confidence = Slot(
-    uri=VM.confidence,
-    name="mappingValidationResult__confidence",
-    curie=VM.curie("confidence"),
-    model_uri=VM.mappingValidationResult__confidence,
-    domain=None,
-    range=Optional[float],
-)
-
-slots.mappingValidationResult__suggested_predicate = Slot(
-    uri=VM.suggested_predicate,
-    name="mappingValidationResult__suggested_predicate",
-    curie=VM.curie("suggested_predicate"),
-    model_uri=VM.mappingValidationResult__suggested_predicate,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.mappingValidationResult__suggested_modifications = Slot(
-    uri=VM.suggested_modifications,
-    name="mappingValidationResult__suggested_modifications",
-    curie=VM.curie("suggested_modifications"),
-    model_uri=VM.mappingValidationResult__suggested_modifications,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.repairOperation__repairs = Slot(
-    uri=VM.repairs,
-    name="repairOperation__repairs",
-    curie=VM.curie("repairs"),
-    model_uri=VM.repairOperation__repairs,
-    domain=None,
-    range=Optional[Union[dict, ValidationResult]],
-)
-
-slots.repairOperation__modified = Slot(
-    uri=VM.modified,
-    name="repairOperation__modified",
-    curie=VM.curie("modified"),
-    model_uri=VM.repairOperation__modified,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.repairOperation__successful = Slot(
-    uri=VM.successful,
-    name="repairOperation__successful",
-    curie=VM.curie("successful"),
-    model_uri=VM.repairOperation__successful,
-    domain=None,
-    range=Optional[Union[bool, Bool]],
-)
-
-slots.repairOperation__info = Slot(
-    uri=VM.info,
-    name="repairOperation__info",
-    curie=VM.curie("info"),
-    model_uri=VM.repairOperation__info,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.externalReferenceValidationResult__url = Slot(
-    uri=VM.url,
-    name="externalReferenceValidationResult__url",
-    curie=VM.curie("url"),
-    model_uri=VM.externalReferenceValidationResult__url,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.externalReferenceValidationResult__time_checked = Slot(
-    uri=VM.time_checked,
-    name="externalReferenceValidationResult__time_checked",
-    curie=VM.curie("time_checked"),
-    model_uri=VM.externalReferenceValidationResult__time_checked,
-    domain=None,
-    range=Optional[str],
-)
-
-slots.externalReferenceValidationResult__number_of_attempts = Slot(
-    uri=VM.number_of_attempts,
-    name="externalReferenceValidationResult__number_of_attempts",
-    curie=VM.curie("number_of_attempts"),
-    model_uri=VM.externalReferenceValidationResult__number_of_attempts,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.externalReferenceValidationResult__http_response_code = Slot(
-    uri=VM.http_response_code,
-    name="externalReferenceValidationResult__http_response_code",
-    curie=VM.curie("http_response_code"),
-    model_uri=VM.externalReferenceValidationResult__http_response_code,
-    domain=None,
-    range=Optional[int],
-)
-
-slots.ValidationReport_results = Slot(
-    uri=SH.result,
-    name="ValidationReport_results",
-    curie=SH.curie("result"),
-    model_uri=VM.ValidationReport_results,
-    domain=ValidationReport,
-    range=Optional[Union[Union[dict, "ValidationResult"], List[Union[dict, "ValidationResult"]]]],
-)
-
-slots.RepairReport_results = Slot(
-    uri=SH.result,
-    name="RepairReport_results",
-    curie=SH.curie("result"),
-    model_uri=VM.RepairReport_results,
-    domain=RepairReport,
-    range=Optional[Union[Union[dict, "RepairOperation"], List[Union[dict, "RepairOperation"]]]],
-)
+slots.RepairReport_results = Slot(uri=SH.result, name="RepairReport_results", curie=SH.curie('result'),
+                   model_uri=VM.RepairReport_results, domain=RepairReport, range=Optional[Union[Union[dict, "RepairOperation"], List[Union[dict, "RepairOperation"]]]])
```

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 id: https://w3id.org/linkml/validation_results
-title: Validation Results Datamodel
+title: Validation Results Data Model
 name: validaton-results
 description: |-
   A datamodel for data validation results.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
   linkml: https://w3id.org/linkml/
@@ -56,17 +56,26 @@
         description: Allows overriding of severity of a particular type
         range: TypeSeverityKeyValue
         inlined: true
         multivalued: true
       schema_path:
         range: string
         description: allows overriding the default OMO schema
+      lookup_references:
+        range: boolean
+        description: if true, then look up references used as provenance (axiom annotation).
+          This may include looking up the PMID and checking if a publication is retracted.
       prompt_info:
         range: string
         description: for AI agents, this allows passing through of additional info to the prompt
+      documentation_objects:
+        range: string
+        multivalued: true
+        description: paths or URLs to files containing best practice documentation, SOPs, etc. Primarily for AI
+          agents to read when performing validation.
 
   RepairConfiguration:
     description: Configuration parameters for execution of validation repairs
     attributes:
       validation_configuration:
         description: repair configurations include validation configurations
         range: ValidationConfiguration
@@ -122,14 +131,24 @@
       - instantiates
       - predicate
       - object
       - object_str
       - source
       - info
 
+  DefinitionValidationResult:
+    is_a: ValidationResult
+    attributes:
+      definition:
+        range: string
+      definition_source:
+        range: string
+      proposed_new_definition:
+        range: string
+
   MappingValidationResult:
     is_a: Result
     description: A validation result where the check is to determine if a mapping is correct
     attributes:
       subject_id:
         range: string
       subject_info:
```

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.6.3/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.6.3/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/__init__.py` & `oaklib-0.6.3/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/agrkb/agrkb_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/agrkb/agrkb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/amigo/amigo_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/amigo/amigo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/eutils/eutils_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/eutils/eutils_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/eutils/pubmed_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/eutils/pubmed_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/gilda.py` & `oaklib-0.6.3/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/llm_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/llm_implementation.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,47 +4,53 @@
 import json
 import logging
 import re
 import time
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Dict, Iterable, Iterator, List, Optional, Tuple
 
+import pystow
+from linkml_runtime.dumpers import yaml_dumper
 from sssom_schema import Mapping
 from tenacity import (
     retry,
     retry_if_exception,
     stop_after_attempt,
     wait_random_exponential,
 )
 
 from oaklib import BasicOntologyInterface
 from oaklib.datamodels.class_enrichment import ClassEnrichmentResult
 from oaklib.datamodels.item_list import ItemList
 from oaklib.datamodels.obograph import DefinitionPropertyValue
+from oaklib.datamodels.ontology_metadata import DefinitionConstraintComponent
 from oaklib.datamodels.similarity import TermPairwiseSimilarity
 from oaklib.datamodels.text_annotator import TextAnnotation, TextAnnotationConfiguration
 from oaklib.datamodels.validation_datamodel import (
+    DefinitionValidationResult,
     MappingValidationResult,
+    SeverityOptions,
     ValidationConfiguration,
 )
-from oaklib.datamodels.vocabulary import HAS_DBXREF, SKOS_EXACT_MATCH
+from oaklib.datamodels.vocabulary import HAS_DBXREF, HAS_DEFINITION_CURIE, SKOS_EXACT_MATCH
 from oaklib.interfaces import (
     MappingProviderInterface,
     OboGraphInterface,
     SearchInterface,
     TextAnnotatorInterface,
     ValidatorInterface,
 )
 from oaklib.interfaces.class_enrichment_calculation_interface import (
     ClassEnrichmentCalculationInterface,
 )
 from oaklib.interfaces.ontology_generator_interface import OntologyGenerationInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.interfaces.text_annotator_interface import TEXT
 from oaklib.types import CURIE, PRED_CURIE
+from oaklib.utilities.iterator_utils import chunk
 
 if TYPE_CHECKING:
     import llm
 
 __all__ = [
     "LLMImplementation",
 ]
@@ -126,14 +132,35 @@
 def query_model_to_json(model, *args, **kwargs):
     response = query_model(model, *args, **kwargs)
     text = json.loads(response.text())
     logger.debug(f"Response: {text}")
     return text
 
 
+def config_to_prompt(configuration: Optional[ValidationConfiguration]) -> Optional[str]:
+    if not configuration:
+        return None
+    prompt = ""
+    if configuration:
+        if configuration.prompt_info:
+            prompt += configuration.prompt_info
+        if configuration.documentation_objects:
+            import html2text
+
+            for obj in configuration.documentation_objects:
+                if obj.startswith("http:") or obj.startswith("https:"):
+                    path = pystow.ensure("oaklib", "documents", url=obj)
+                else:
+                    path = obj
+                with open(path) as f:
+                    html = f.read()
+                    prompt += html2text.html2text(html)
+    return prompt
+
+
 @dataclass
 class LLMImplementation(
     OboGraphInterface,
     ClassEnrichmentCalculationInterface,
     TextAnnotatorInterface,
     SearchInterface,
     MappingProviderInterface,
@@ -495,14 +522,87 @@
                 problem=obj.get("problem", None),
                 confidence=cmap.get(obj.get("confidence", None), 0.5),
                 info=obj.get("comment", None),
                 suggested_predicate=obj.get("predicate_modifications", None),
                 suggested_modifications=mods,
             )
 
+    def validate_definitions(
+        self,
+        entities: Iterable[CURIE] = None,
+        configuration: ValidationConfiguration = None,
+        skip_text_annotation=False,
+        **kwargs,
+    ) -> Iterable[DefinitionValidationResult]:
+        """
+        Validate text definitions for a set of entities.
+
+        :param entities:
+        :param configuration:
+        :param kwargs:
+        :return:
+        """
+        model = self.get_model()
+        system_prompt = (
+            "Your job is to evaluate how well aligned an ontology term's definition "
+            "to the reference cited in that definition. Rank the level of alignment between LOW, "
+            "MEDIUM, and HIGH. If the definition is too specific, say this. "
+            "Highlight sections from the abstract that align with, or misalign with the definition."
+        )
+        extra = config_to_prompt(configuration)
+        if extra:
+            system_prompt += "\n" + extra
+
+        if entities is None:
+            entities = self.entities(filter_obsoletes=True)
+
+        wrapped = self.wrapped_adapter
+        if not isinstance(wrapped, ValidatorInterface):
+            raise NotImplementedError("Wrapped adapter must support validation")
+        for entity_it in chunk(entities):
+            for entity, defn, metadata in wrapped.definitions(
+                entity_it,
+                include_metadata=True,
+            ):
+                for _, vs in metadata.items():
+                    ref_map = wrapped.lookup_references(vs)
+                    if not ref_map:
+                        continue
+                    node = wrapped.node(entity)
+                    for ref, ref_obj in ref_map.items():
+                        ref_obj_str = yaml_dumper.dumps(ref_obj)
+                        prompt = (
+                            "Term:\n"
+                            f"{yaml_dumper.dumps(node)}"
+                            "Definition references:\n"
+                            f"{ref_obj_str}"
+                        )
+                        resp = query_model(model, prompt, system_prompt).text()
+                        if "HIGH" in resp:
+                            severity = SeverityOptions.INFO
+                        elif "MEDIUM" in resp:
+                            severity = SeverityOptions.WARNING
+                        elif "LOW" in resp:
+                            severity = SeverityOptions.ERROR
+                        else:
+                            severity = SeverityOptions.INFO
+                            logger.warning(f"Unknown severity: {resp}")
+                            resp += " (defaulting to INFO as no ranking found)"
+                        result = DefinitionValidationResult(
+                            subject=entity,
+                            severity=SeverityOptions(severity),
+                            predicate=HAS_DEFINITION_CURIE,
+                            object_str=ref_obj_str,
+                            definition=defn,
+                            definition_source=ref,
+                            type=DefinitionConstraintComponent.MatchTextAndReference.meaning,
+                            info=resp,
+                        )
+                        yield result
+
     def enriched_classes(
         self,
         subjects: Optional[Iterable[CURIE]] = None,
         item_list: Optional[ItemList] = None,
         predicates: Iterable[CURIE] = None,
         object_closure_predicates: Optional[List[PRED_CURIE]] = None,
         background: Iterable[CURIE] = None,
```

### Comparing `oaklib-0.6.2/src/oaklib/implementations/monarch/monarch_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/monarch/monarch_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/ncbi/ncbi_gene_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.6.3/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.6.3/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/pantherdb/pantherdb_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/pantherdb/pantherdb_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/semsimian/semsimian_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/semsimian/semsimian_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     _synonym_scope_pred,
     parse_obo_document,
 )
 from oaklib.inference.relation_graph_reasoner import RelationGraphReasoner
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
+    DEFINITION,
     LANGUAGE_TAG,
     METADATA_MAP,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.differ_interface import DiffConfiguration, DifferInterface
 from oaklib.interfaces.dumper_interface import DumperInterface
@@ -444,14 +445,37 @@
         self._clear_relationship_index()
 
     def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         s = self._stanza(curie, strict=False)
         if s:
             return s.quoted_value(TAG_DEFINITION)
 
+    def definitions(
+        self,
+        curies: Iterable[CURIE],
+        include_metadata=False,
+        include_missing=False,
+        lang: Optional[LANGUAGE_TAG] = None,
+    ) -> Iterator[DEFINITION]:
+        for curie in curies:
+            s = self._stanza(curie, strict=False)
+            if s:
+                d = s.quoted_value(TAG_DEFINITION)
+                if d:
+                    if include_metadata:
+                        defn_tvs = [tv for tv in s.tag_values if tv.tag == TAG_DEFINITION]
+                        if defn_tvs:
+                            defn_tv = defn_tvs[0]
+                            defn, xrefs = defn_tv.as_definition()
+                            yield curie, defn, {HAS_DBXREF: xrefs}
+                    else:
+                        yield curie, d, None
+                elif include_missing:
+                    yield curie, None, None
+
     def comments(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, str]]:
         for curie in curies:
             s = self._stanza(curie)
             if s:
                 yield curie, s.singular_value(TAG_COMMENT)
 
     def entity_alias_map(self, curie: CURIE) -> ALIAS_MAP:
@@ -470,19 +494,22 @@
 
     def synonym_property_values(
         self, subject: Union[CURIE, Iterable[CURIE]]
     ) -> Iterator[Tuple[CURIE, SynonymPropertyValue]]:
         if isinstance(subject, str):
             subject = [subject]
         for curie in subject:
-            for p, vs in self.entity_alias_map(curie).items():
-                if p == LABEL_PREDICATE:
-                    continue
-                for v in vs:
-                    yield curie, SynonymPropertyValue(pred=p.replace("oio:", ""), val=v)
+            s = self._stanza(curie, strict=False)
+            if not s:
+                continue
+            for syn in s.synonyms():
+                pred = _synonym_scope_pred(syn[1]).replace("oio:", "")
+                yield curie, SynonymPropertyValue(
+                    pred=pred, val=syn[0], synonymType=syn[2], xrefs=syn[3]
+                )
 
     def map_shorthand_to_curie(self, rel_code: PRED_CODE) -> PRED_CURIE:
         """
         Maps either a true relationship type CURIE or a shorthand packages to a CURIE.
 
         See `section 5.9 <https://owlcollab.github.io/oboformat/doc/obo-syntax.html#5.9>`_
```

### Comparing `oaklib-0.6.2/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.6.3/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
 from oaklib.datamodels.vocabulary import SCOPE_TO_SYNONYM_PRED_MAP
 from oaklib.types import CURIE, PRED_CURIE
 
 re_tag_value = re.compile(r"^(\S+):\s*(.*)$")
 re_stanza_type = re.compile(r"^\[(\w+)\]$")
 re_empty = re.compile(r"^\S*$")
+re_def = re.compile(r"^\"(.*)\"\s+\[(.*)\](?:\s+\{(.*)\})?$")
 re_synonym1 = re.compile(r"^\"(.*)\"\s+(\w+)\s+\[(.*)\](?:\s+\{(.*)\})?$")
 re_synonym2 = re.compile(r"^\"(.*)\"\s+(\w+)\s+(\S)+\s\[(.*)\](?:\s+\{(.*)\})?$")
 re_quoted_simple = re.compile(r'^"(.*)"\s+\[')
 re_property_value1 = re.compile(r"^(\S+)\s+(.*)\s+(\S+)(?:\s+\{(.*)\})?$")
 re_property_value2 = re.compile(r"^(\S+)\s+(\S+)(?:\s+\{(.*)\})?$")
 
 
@@ -185,14 +186,31 @@
             m = re_synonym1.match(self.value)
             if m:
                 syn = m.group(1), m.group(2), None, m.group(3)
             else:
                 raise ValueError(f"Bad synonym: {self.value}")
         return syn[0], syn[1], syn[2], _parse_list(syn[3])
 
+    def as_definition(self) -> Optional[Tuple[str, List[str]]]:
+        """
+        Cast a tag-value pair as a definition
+
+        Returns None if this is not a definition TV
+
+        :return: definition tuple structure
+        """
+        if self.tag != TAG_DEF:
+            return
+        m = re_def.match(self.value)
+        if m:
+            xrefs = _parse_list(m.group(2)) if m.group(2) else []
+            return m.group(1), xrefs
+        else:
+            raise ValueError(f"Bad definition: {self.value}")
+
     def as_property_value(self) -> Optional[PROPERTY_VALUE_TUPLE]:
         """
         Cast a tag-value pair as a property value
 
         Returns None if this is not a property value TV
 
         :return: property value tuple structure
```

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.6.3/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.6.3/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/tabular/robot_template_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/tabular/robot_template_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/tabular/tabular_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/tabular/tabular_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.6.3/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/indexes/edge_index.py` & `oaklib-0.6.3/src/oaklib/indexes/edge_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/inference/owl_reasoner.py` & `oaklib-0.6.3/src/oaklib/inference/owl_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/inference/relation_graph_reasoner.py` & `oaklib-0.6.3/src/oaklib/inference/relation_graph_reasoner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/__init__.py` & `oaklib-0.6.3/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/embedding_provider_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/embedding_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/obograph_interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,14 +178,37 @@
                 node_map[p] = p_node
             if o not in node_map:
                 node_map[o] = self.node(o)
             edges.append(Edge(sub=s, pred=p, obj=o))
         graph_id = "test"
         return Graph(id=graph_id, nodes=list(node_map.values()), edges=edges)
 
+    def direct_graph(
+        self,
+        curies: Union[CURIE, List[CURIE]],
+        **kwargs,
+    ) -> Graph:
+        """
+        Return a graph object that consists of all the nodes specified in the curies list,
+        extended with all direct relationships
+
+        :param curies:
+        :return: direct graph
+        """
+        if not isinstance(curies, list):
+            curies = [curies]
+        g = self._graph(self.relationships(subjects=curies))
+        for curie in curies:
+            n = self.node(curie, include_metadata=True)
+            if n:
+                g.nodes.append(n)
+        ldefs = list(self.logical_definitions(curies))
+        g.logicalDefinitionAxioms = ldefs
+        return g
+
     def ancestor_graph(
         self, start_curies: Union[CURIE, List[CURIE]], predicates: List[PRED_CURIE] = None
     ) -> Graph:
         """
         Return a graph object that consists of all the nodes specified in the start_curies list,
         extended with an interactive walk up the graph following all relationships (optionally filtered by the predicate
         list)
```

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/ontology_generator_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/ontology_generator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/search_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.6.3/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/heatmap_writer.py` & `oaklib-0.6.3/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/html_writer.py` & `oaklib-0.6.3/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/obograph_writer.py` & `oaklib-0.6.3/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.6.3/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_obo_writer.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,82 +1,50 @@
 import logging
 from dataclasses import dataclass
 from typing import Any, Iterable
 
-from sssom.constants import OWL_EQUIVALENT_CLASS
-
 from oaklib.converters.obo_graph_to_obo_format_converter import (
     OboGraphToOboFormatConverter,
 )
 from oaklib.datamodels.obograph import (
     DisjointClassExpressionsAxiom,
+    Graph,
     GraphDocument,
     LogicalDefinitionAxiom,
 )
-from oaklib.datamodels.vocabulary import IS_A, RDF_TYPE, SYNONYM_PRED_TO_SCOPE_MAP
-from oaklib.interfaces.metadata_interface import MetadataInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.io.streaming_writer import StreamingWriter
 from oaklib.types import CURIE
 
 
 @dataclass
 class StreamingOboWriter(StreamingWriter):
     """
     A writer that emits one OBO stanza at a time in one stream
     """
 
+    converter: OboGraphToOboFormatConverter = None
+
     def tag_val(self, k: str, v: Any, xrefs=None):
         self.file.write(f"{k}: {v}")
         if xrefs is not None:
             self.file.write(f' [{", ".join(xrefs)}]')
         self.file.write("\n")
 
     def emit_curie(self, curie: CURIE, label=None):
         oi = self.ontology_interface
-        self.line("[Term]")
-        self.line(f"id: {curie}")
-        if label is None:
-            label = oi.label(curie)
-        self.tag_val("name", label)
-        defn = oi.definition(curie)
-        if defn:
-            if isinstance(oi, MetadataInterface):
-                _, anns = oi.definition_with_annotations(curie)
-            else:
-                anns = []
-            self.tag_val("def", f'"{defn}"', xrefs=[ann.object for ann in anns])
-        for _, x in oi.simple_mappings_by_curie(curie):
-            self.line(f"xref: {x}")
-        amap = oi.entity_alias_map(curie)
-        for a, vs in amap.items():
-            if a in SYNONYM_PRED_TO_SCOPE_MAP:
-                scope = SYNONYM_PRED_TO_SCOPE_MAP[a]
-                for v in vs:
-                    self.line(f'synonym: "{v}" {scope} []')
-        if isinstance(oi, OboGraphInterface):
-            rmap = oi.outgoing_relationship_map(curie)
-            for p in rmap.get(IS_A, []):
-                self.line(f"is_a: {p} ! {oi.label(p)}")
-            for r, ps in rmap.items():
-                if r != IS_A and r != RDF_TYPE and r != OWL_EQUIVALENT_CLASS:
-                    for p in ps:
-                        self.line(f"relationship: {r} {p} ! {oi.label(p)}")
-            try:
-                for ldef in oi.logical_definitions([curie]):
-                    for p in ldef.genusIds:
-                        self.line(f"intersection_of: {p} ! {oi.label(p)}")
-                    for r in ldef.restrictions:
-                        self.line(
-                            f"intersection_of: {r.propertyId} {r.fillerId} ! {oi.label(r.fillerId)}"
-                        )
-            except NotImplementedError:
-                logging.info("Logical definitions not implemented")
-
-        self.line("\n")
+        if self.converter is None:
+            self.converter = OboGraphToOboFormatConverter()
+        if not isinstance(oi, OboGraphInterface):
+            raise NotImplementedError
+        graph = oi.direct_graph(curie)
+        ext_graph = Graph(id="ext", nodes=[n for n in graph.nodes if n.id != curie])
+        graph.nodes = [n for n in graph.nodes if n.id == curie]
+        text = self.converter.dumps(graph, aux_graphs=[ext_graph])
+        self.file.write(text)
 
     def emit_multiple(self, entities: Iterable[CURIE], **kwargs):
         oi = self.ontology_interface
         if isinstance(oi, OboGraphInterface):
             logging.info("Extracting graph")
             g = oi.extract_graph(list(entities), include_metadata=True)
             gd = GraphDocument(graphs=[g])
```

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.6.3/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/mappers/base_mapper.py` & `oaklib-0.6.3/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.6.3/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/__init__.py` & `oaklib-0.6.3/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.6.3/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/hpoa_g2d_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/hpoa_g2d_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/parser_base.py` & `oaklib-0.6.3/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.6.3/src/oaklib/parsers/xaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/resource.py` & `oaklib-0.6.3/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/selector.py` & `oaklib-0.6.3/src/oaklib/selector.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/chained_ontology_transformer.py` & `oaklib-0.6.3/src/oaklib/transformers/chained_ontology_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/edge_filter_transformer.py` & `oaklib-0.6.3/src/oaklib/transformers/edge_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/graph_transformer.py` & `oaklib-0.6.3/src/oaklib/transformers/graph_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/node_filter_transformer.py` & `oaklib-0.6.3/src/oaklib/transformers/node_filter_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/sep_transformer.py` & `oaklib-0.6.3/src/oaklib/transformers/sep_transformer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/transformers/transformers_factory.py` & `oaklib-0.6.3/src/oaklib/transformers/transformers_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.6.3/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.6.3/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.6.3/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py` & `oaklib-0.6.3/src/oaklib/utilities/axioms/disjointness_axiom_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_analyzer.py` & `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_analyzer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_summarizer.py` & `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_summarizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/axioms/logical_definition_utilities.py` & `oaklib-0.6.3/src/oaklib/utilities/axioms/logical_definition_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/basic_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/format_utilities.py` & `oaklib-0.6.3/src/oaklib/utilities/format_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.6.3/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.6.3/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/keyval_cache.py` & `oaklib-0.6.3/src/oaklib/utilities/keyval_cache.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.6.3/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/label_utilities.py` & `oaklib-0.6.3/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.6.3/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/lexical/patternizer.py` & `oaklib-0.6.3/src/oaklib/utilities/lexical/patternizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/lexical/synonymizer.py` & `oaklib-0.6.3/src/oaklib/utilities/lexical/synonymizer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.6.3/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.6.3/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.6.3/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.6.3/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.6.3/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.6.3/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.6.3/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.6.3/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.6.3/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/table_filler.py` & `oaklib-0.6.3/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.6.3/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from dataclasses import dataclass
-from typing import Iterable, Iterator, List, Optional
+from typing import Dict, Iterable, Iterator, List, Optional
 
 from oaklib import BasicOntologyInterface
 from oaklib.datamodels.obograph import LogicalDefinitionAxiom
 from oaklib.datamodels.ontology_metadata import OMOSCHEMA, DefinitionConstraintComponent
+from oaklib.datamodels.text_annotator import TextAnnotation
 from oaklib.datamodels.validation_datamodel import SeverityOptions, ValidationResult
 from oaklib.datamodels.vocabulary import HAS_DEFINITION_CURIE
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE
 from oaklib.utilities.validation.ontology_rule import OntologyRule
 
@@ -47,28 +48,30 @@
     """If the definition follows 'A <genus> that <differentia>, this is the differentia"""
 
     that_marker_index: Optional[int] = None
     """If the definition follows genus-differentia form, this is the position of the that/which."""
 
 
 @dataclass
-class TextAndLogicalDefinitionMatchOntologyRule(OntologyRule):
+class DefinitionOntologyRule(OntologyRule):
     """
     Text and logical definitions should match.
 
     This is a highly sensitive test and many textual definitions
     are expected not to conform due to natural lexical variation.
 
     The tests are based on a subset of the criteria in, in particular:
 
     - S1: conform to conventions (do not include definiendum)
     - S3: Use the genus differentia form
     - S7: Avoid circularity
     - S11: Match text and logical definitions
 
+    See `<https://w3id.org/oak/ontology-metadata/DefinitionConstraintComponent>`_ for more details.
+
     """
 
     name: str = "text and logical definition match rule"
     severity = SeverityOptions(SeverityOptions.INFO)
     skip_text_annotation: bool = False
 
     def process_text_definition(self, tdef: str) -> ProcessedTextDefinition:
@@ -103,79 +106,68 @@
         return ptd
 
     def check_against_logical_definition(
         self,
         oi: BasicOntologyInterface,
         pdef: ProcessedTextDefinition,
         ldef: LogicalDefinitionAxiom,
+        anns_by_object: Dict[CURIE, TextAnnotation] = None,
     ) -> Iterator[ValidationResult]:
         """
         Check a text definition against a logical definition.
 
         :param oi:
         :param pdef:
         :param ldef:
+        :param anns_by_object: text annotations of the text definition by object
         :return:
         """
         subject = ldef.definedClassId
-        if isinstance(oi, TextAnnotatorInterface) and not self.skip_text_annotation:
-            anns = list(oi.annotate_text(pdef.main_definition))
-            anns_by_object = {ann.object_id: ann for ann in anns}
-
-            def _check(
-                expected_id: CURIE, expected_in_text: str, is_genus=False
-            ) -> Iterator[ValidationResult]:
-                if expected_id in anns_by_object:
-                    if not expected_in_text:
-                        pass
-                    else:
-                        ann = anns_by_object[expected_id]
-                        if ann.match_string in expected_in_text:
-                            if is_genus and len(ann.match_string) < len(expected_in_text):
-                                yield ValidationResult(
-                                    subject=subject,
-                                    predicate=HAS_DEFINITION_CURIE,
-                                    type=DefinitionConstraintComponent.GenusDifferentiaForm.meaning,
-                                    object_str=expected_in_text,
-                                    info=f"Did not match whole text: {ann.match_string} < {expected_in_text}",
-                                )
-                        else:
+
+        def _check(
+            expected_id: CURIE, expected_in_text: str, is_genus=False
+        ) -> Iterator[ValidationResult]:
+            if expected_id in anns_by_object:
+                if not expected_in_text:
+                    pass
+                else:
+                    ann = anns_by_object[expected_id]
+                    if ann.match_string in expected_in_text:
+                        if is_genus and len(ann.match_string) < len(expected_in_text):
                             yield ValidationResult(
-                                type=DefinitionConstraintComponent.MatchTextAndLogical.meaning,
                                 subject=subject,
                                 predicate=HAS_DEFINITION_CURIE,
+                                type=DefinitionConstraintComponent.GenusDifferentiaForm.meaning,
                                 object_str=expected_in_text,
-                                info=f"Wrong position, '{ann.match_string}' not in '{expected_in_text}'",
+                                info=f"Did not match whole text: {ann.match_string} < {expected_in_text}",
                             )
-                else:
-                    yield ValidationResult(
-                        type=DefinitionConstraintComponent.MatchTextAndLogical.meaning,
-                        # object=expected_id,
-                        predicate=HAS_DEFINITION_CURIE,
-                        object_str=expected_in_text,
-                        subject=subject,
-                        info=f"Not found: {expected_id}",
-                    )
-
-            for genus in ldef.genusIds:
-                for result in _check(genus, pdef.genus_text, is_genus=True):
-                    yield result
-            for restr in ldef.restrictions:
-                for result in _check(restr.fillerId, pdef.differentia_text):
-                    yield result
-            if subject in anns_by_object:
+                    else:
+                        yield ValidationResult(
+                            type=DefinitionConstraintComponent.MatchTextAndLogical.meaning,
+                            subject=subject,
+                            predicate=HAS_DEFINITION_CURIE,
+                            object_str=expected_in_text,
+                            info=f"Wrong position, '{ann.match_string}' not in '{expected_in_text}'",
+                        )
+            else:
                 yield ValidationResult(
-                    type=DefinitionConstraintComponent.Circularity.meaning,
-                    subject=subject,
+                    type=DefinitionConstraintComponent.MatchTextAndLogical.meaning,
+                    # object=expected_id,
                     predicate=HAS_DEFINITION_CURIE,
-                    object_str=pdef.main_definition,
-                    info=f"Circular, {anns_by_object[subject].match_string} in definition",
+                    object_str=expected_in_text,
+                    subject=subject,
+                    info=f"Logical definition element not found in text: {expected_id}",
                 )
-        else:
-            logging.info(f"Skipping text annotation for {subject}")
+
+        for genus in ldef.genusIds:
+            for result in _check(genus, pdef.genus_text, is_genus=True):
+                yield result
+        for restr in ldef.restrictions:
+            for result in _check(restr.fillerId, pdef.differentia_text):
+                yield result
 
     def evaluate(
         self, oi: BasicOntologyInterface, entities: Iterable[CURIE] = None
     ) -> Iterable[ValidationResult]:
         """
         Implements the OntologyRule.evaluate() method.
 
@@ -191,40 +183,70 @@
             logging.info(f"Checking {subject}")
             problem_count = 0
             # TODO: leakage of quoted URIs into CURIEs should be fixed upstream.
             # these currently come from SWRL URIs from rdftab
             if subject.startswith("<"):
                 continue
             tdef = oi.definition(subject)
+
+            anns_by_object = {}
             if tdef:
                 pdef = self.process_text_definition(tdef)
                 if not pdef.genus_text or not pdef.differentia_text:
                     yield ValidationResult(
                         subject=subject,
                         object_str=tdef,
                         severity=SeverityOptions(SeverityOptions.WARNING),
                         predicate=HAS_DEFINITION_CURIE,
                         type=DefinitionConstraintComponent.GenusDifferentiaForm.meaning,
                         info="Cannot parse genus and differentia",
                     )
                     problem_count += 1
+                if isinstance(oi, TextAnnotatorInterface) and not self.skip_text_annotation:
+                    anns = list(oi.annotate_text(pdef.main_definition))
+                    anns_by_object = {ann.object_id: ann for ann in anns}
+                    logging.debug(f"ANNS {tdef} ==> {len(anns)}")
             else:
                 pdef = None
                 yield ValidationResult(
                     subject=subject,
                     severity=SeverityOptions(SeverityOptions.ERROR),
                     predicate=HAS_DEFINITION_CURIE,
                     type=DefinitionConstraintComponent.DefinitionPresence.meaning,
                     info="Missing text definition",
                 )
                 problem_count += 1
+            if subject in anns_by_object:
+                ann = anns_by_object[subject]
+                text_before = tdef[0 : ann.subject_start]
+                text_after = tdef[ann.subject_end :]
+                is_terms = [" is ", " are ", " were "]
+                if len(text_before) < 5 or any(t for t in is_terms if text_after.startswith(t)):
+                    yield ValidationResult(
+                        subject=subject,
+                        predicate=HAS_DEFINITION_CURIE,
+                        type=DefinitionConstraintComponent.Conventions.meaning,
+                        info="Definiendum should not appear at the start",
+                    )
+                    problem_count += 1
+                else:
+                    yield ValidationResult(
+                        type=DefinitionConstraintComponent.Circularity.meaning,
+                        subject=subject,
+                        predicate=HAS_DEFINITION_CURIE,
+                        object_str=pdef.main_definition,
+                        info=f"Circular, {ann.match_string} ({subject} in definition",
+                    )
+                    problem_count += 1
             if isinstance(oi, OboGraphInterface):
                 for ldef in oi.logical_definitions([subject]):
                     if pdef:
-                        for result in self.check_against_logical_definition(oi, pdef, ldef):
+                        for result in self.check_against_logical_definition(
+                            oi, pdef, ldef, anns_by_object
+                        ):
                             yield result
                             problem_count += 1
                     if len(ldef.genusIds) != 1:
                         yield ValidationResult(
                             subject=subject,
                             type=DefinitionConstraintComponent.SingleGenus.meaning,
                             info=f"expected one genus; got {len(ldef.genusIds)}.",
```

### Comparing `oaklib-0.6.2/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.6.3/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.6.3/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.6.3/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.6.3/src/oaklib/utilities/validation/rule_runner.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import logging
 from dataclasses import dataclass, field
 from typing import Iterable, List, Type
 
 from oaklib import BasicOntologyInterface
 from oaklib.datamodels.validation_datamodel import ValidationResult
 from oaklib.utilities.validation.definition_ontology_rule import (
-    TextAndLogicalDefinitionMatchOntologyRule,
+    DefinitionOntologyRule,
 )
 from oaklib.utilities.validation.disjointness_rule import DisjointnessRule
 from oaklib.utilities.validation.ontology_rule import OntologyRule
 
-RULES = [TextAndLogicalDefinitionMatchOntologyRule, DisjointnessRule]
+RULES = [DefinitionOntologyRule, DisjointnessRule]
 
 
 @dataclass
 class RuleRunner:
     rules: List[Type[OntologyRule]] = field(default_factory=lambda: RULES)
 
     def run(self, oi: BasicOntologyInterface) -> Iterable[ValidationResult]:
```

### Comparing `oaklib-0.6.2/src/oaklib/utilities/writers/change_handler.py` & `oaklib-0.6.3/src/oaklib/utilities/writers/change_handler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.6.2/PKG-INFO` & `oaklib-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.6.2
+Version: 0.6.3
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,14 +22,15 @@
 Requires-Dist: appdirs (>=1.4.4)
 Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: click
 Requires-Dist: curies (>=0.6.6)
 Requires-Dist: eutils (>=0.6.0)
 Requires-Dist: funowl (>=0.2.0)
 Requires-Dist: gilda (>=1.0.0) ; extra == "gilda"
+Requires-Dist: html2text ; extra == "llm"
 Requires-Dist: jsonlines (>=4.0.0,<5.0.0)
 Requires-Dist: kgcl-rdflib (==0.5.0)
 Requires-Dist: kgcl-schema (>=0.6.8,<0.7.0)
 Requires-Dist: linkml-renderer (>=0.3.0)
 Requires-Dist: linkml-runtime (>=1.5.3)
 Requires-Dist: llm ; extra == "llm"
 Requires-Dist: ndex2 (>=3.5.0,<4.0.0)
```

