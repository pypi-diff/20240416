# Comparing `tmp/dialogy-2.1.0.tar.gz` & `tmp/dialogy-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.1.0.tar", max compression
+gzip compressed data, was "dialogy-2.2.0.tar", max compression
```

## Comparing `dialogy-2.1.0.tar` & `dialogy-2.2.0.tar`

### file list

```diff
@@ -1,75 +1,76 @@
--rw-r--r--   0        0        0     1069 2023-07-31 08:48:29.934474 dialogy-2.1.0/LICENSE.md
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9777 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15830 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     4001 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8880 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3802 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11811 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1185 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    16950 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7682 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39031 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20340 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12466 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1804 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14137 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11529 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4711 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     3041 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4259 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4154 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7361 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4432 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    11979 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2880 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     8010 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1560 2023-07-31 08:48:48.898860 dialogy-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 dialogy-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-01-10 10:05:16.948528 dialogy-2.2.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.948528 dialogy-2.2.0/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2024-01-10 10:05:16.948528 dialogy-2.2.0/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2024-01-10 10:05:16.948528 dialogy-2.2.0/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2024-01-10 10:05:16.948528 dialogy-2.2.0/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15830 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2092 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     4001 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8880 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3802 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11811 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1185 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    16950 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7682 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    10162 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/dob_plugin/__init__.py
+-rw-r--r--   0        0        0    39031 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20340 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12466 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1804 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14137 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11529 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4711 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     3041 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4259 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4154 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7361 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4432 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2024-01-10 10:05:16.952528 dialogy-2.2.0/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    11979 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2880 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     8010 2024-01-10 10:05:16.956528 dialogy-2.2.0/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1581 2024-01-10 10:05:30.740490 dialogy-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1775 1970-01-01 00:00:00.000000 dialogy-2.2.0/PKG-INFO
```

### Comparing `dialogy-2.1.0/LICENSE.md` & `dialogy-2.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.2.0/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/base/input/__init__.py` & `dialogy-2.2.0/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/base/output/__init__.py` & `dialogy-2.2.0/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/base/plugin/__init__.py` & `dialogy-2.2.0/dialogy/base/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/cli/__init__.py` & `dialogy-2.2.0/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/cli/project.py` & `dialogy-2.2.0/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/cli/workflow.py` & `dialogy-2.2.0/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/constants/__init__.py` & `dialogy-2.2.0/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/registry.py` & `dialogy-2.2.0/dialogy/plugins/registry.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 from dialogy.plugins.text.calibration.xgb import CalibrationModel
 from dialogy.plugins.text.canonicalization import CanonicalizationPlugin
 from dialogy.plugins.text.classification.mlp import MLPMultiClass
 from dialogy.plugins.text.classification.retain_intent import RetainOriginalIntentPlugin
 from dialogy.plugins.text.classification.xlmr import XLMRMultiClass
 from dialogy.plugins.text.combine_date_time import CombineDateTimeOverSlots
+from dialogy.plugins.text.dob_plugin import DOBPlugin
 from dialogy.plugins.text.duckling_plugin import DucklingPlugin
 from dialogy.plugins.text.lb_plugin import DucklingPluginLB
 from dialogy.plugins.text.list_entity_plugin import ListEntityPlugin
 from dialogy.plugins.text.list_search_plugin import ListSearchPlugin
 from dialogy.plugins.text.merge_asr_output import MergeASROutputPlugin
 from dialogy.plugins.text.slot_filler.rule_slot_filler import RuleBasedSlotFillerPlugin
 from dialogy.plugins.text.address_parser import AddressParserPlugin
@@ -19,14 +20,15 @@
 
 
 plugin_cls_lib = {
     "CalibrationModel": CalibrationModel,
     "CanonicalizationPlugin": CanonicalizationPlugin,
     "MLPMultiClass": MLPMultiClass,
     "MergeASROutputPlugin": MergeASROutputPlugin,
+    "DOBPlugin":DOBPlugin,
     "DucklingPlugin": DucklingPlugin,
     "ListEntityPlugin": ListEntityPlugin,
     "XLMRMultiClass": XLMRMultiClass,
     "RuleBasedSlotFillerPlugin": RuleBasedSlotFillerPlugin,
     "AddressParserPlugin": AddressParserPlugin,
     "RetainOriginalIntentPlugin": RetainOriginalIntentPlugin,
     "CombineDateTimeOverSlots": CombineDateTimeOverSlots,
```

### Comparing `dialogy-2.1.0/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.2.0/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.2.0/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.2.0/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.2.0/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.2.0/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.2.0/dialogy/plugins/text/classification/xlmr.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.2.0/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.2.0/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.2.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.2.0/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.2.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/__init__.py` & `dialogy-2.2.0/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/address/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/duration/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/people/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/time/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.2.0/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/intent/__init__.py` & `dialogy-2.2.0/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/types/slots/__init__.py` & `dialogy-2.2.0/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/__init__.py` & `dialogy-2.2.0/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/config.py` & `dialogy-2.2.0/dialogy/utils/config.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/datetime.py` & `dialogy-2.2.0/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/file_handler.py` & `dialogy-2.2.0/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/logger.py` & `dialogy-2.2.0/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/misc.py` & `dialogy-2.2.0/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/naive_lang_detect.py` & `dialogy-2.2.0/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/normalize_utterance.py` & `dialogy-2.2.0/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/utils/temperature_scaling.py` & `dialogy-2.2.0/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/dialogy/workflow/workflow.py` & `dialogy-2.2.0/dialogy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.1.0/pyproject.toml` & `dialogy-2.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.1.0"
+version = "2.2.0"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>", "Daksh Varshneya <dakshvar22@gmail.com"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -32,14 +32,15 @@
 black = "^22.8.0"
 googlemaps = "^4.6.0"
 torch = "1.12.1"
 pydantic = "^1.10.2"
 aiohttp = "^3.8.4"
 nest-asyncio = "^1.5.6"
 transformers = "4.30.2"
+word2number = "^1.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^2.10.1"
 copier = "^6.0.0"
 mypy = "^0.982"
```

### Comparing `dialogy-2.1.0/PKG-INFO` & `dialogy-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.1.0
+Version: 2.2.0
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -35,9 +35,10 @@
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: torch (==1.12.1)
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
 Requires-Dist: transformers (==4.30.2)
 Requires-Dist: types-pytz (>=2021.3.5,<2022.0.0)
 Requires-Dist: types-requests (>=2.27.11,<3.0.0)
 Requires-Dist: types-setuptools (>=57.4.10,<58.0.0)
+Requires-Dist: word2number (>=1.1,<2.0)
 Requires-Dist: xgboost (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/skit-ai/dialogy
```

