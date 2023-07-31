# Comparing `tmp/dialogy-2.0.9.tar.gz` & `tmp/dialogy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.9.tar", max compression
+gzip compressed data, was "dialogy-2.1.0.tar", max compression
```

## Comparing `dialogy-2.0.9.tar` & `dialogy-2.1.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-06-12 09:05:22.602009 dialogy-2.0.9/LICENSE.md
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9777 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15685 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     4001 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8880 2023-06-12 09:05:22.602009 dialogy-2.0.9/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3802 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11811 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1185 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    16717 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7682 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    38996 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20340 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12306 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1804 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14135 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11529 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4711 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     3013 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4259 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4154 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7361 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4432 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    11174 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2880 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     7069 2023-06-12 09:05:22.606009 dialogy-2.0.9/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1536 2023-06-12 09:05:40.886143 dialogy-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     1696 1970-01-01 00:00:00.000000 dialogy-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-31 08:48:29.934474 dialogy-2.1.0/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15830 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     4001 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8880 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3802 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11811 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1185 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    16950 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7682 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39031 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20340 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12466 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1804 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14137 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11529 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4711 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     3041 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4259 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4154 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7361 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4432 2023-07-31 08:48:29.934474 dialogy-2.1.0/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    11979 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2880 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     8010 2023-07-31 08:48:29.938474 dialogy-2.1.0/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1560 2023-07-31 08:48:48.898860 dialogy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1735 1970-01-01 00:00:00.000000 dialogy-2.1.0/PKG-INFO
```

### Comparing `dialogy-2.0.9/LICENSE.md` & `dialogy-2.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.1.0/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/base/input/__init__.py` & `dialogy-2.1.0/dialogy/base/input/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/base/output/__init__.py` & `dialogy-2.1.0/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/base/plugin/__init__.py` & `dialogy-2.1.0/dialogy/base/plugin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         :type input: Input
         :param output: The workflow's output.
         :type output: Output
         :return: The value returned by the plugin.
         :rtype: Any
         """
 
-    async def __call__(self, input, output):  # type: ignore
+    async def __call__(self, input, output, **kwargs):  # type: ignore
         """
         Set workflow with output.
 
         This important book-keeping method is called by the workflow.
 
         - If the plugin guards evaluate to :code:`True`, we don't run the plugin's business logic.
         - Otherwise, we obtain the plugins transformation and set it on :code:`self.dest` path within the workflow.
@@ -281,15 +281,15 @@
         - The workflow takes care of keeping its :ref:`input<Input>` and :ref:`output<Output>` immutable.
 
         .. _PluginBookkeeping:
 
         :param workflow: An instance of :ref:`Workflow <WorkflowClass>`.
         :type workflow: Workflow
         """
-        logger.enable(str(self)) if self.debug else logger.disable(str(self))
+        logger.enable(self.__module__) if self.debug and not kwargs.pop("is_sensitive", False) else logger.disable(self.__module__)
         if input is None:
             return input, output
 
         if output is None:
             return input, output
 
         if self.prevent(input, output):
@@ -304,14 +304,16 @@
             value, dest = return_value[0], return_value[1]
         else:
             value, dest = return_value, self.dest
         # update
         if value is not None and isinstance(dest, str):
             input, output = self.set(dest, value, input, output)
 
+        # logger.enable("dialogy") if self.debug else logger.disable("dialogy")
+
         return input, output
 
     def set(  # type: ignore
         self,
         path: str,
         value: Any,
         input,
```

### Comparing `dialogy-2.0.9/dialogy/cli/__init__.py` & `dialogy-2.1.0/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/cli/project.py` & `dialogy-2.1.0/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/cli/workflow.py` & `dialogy-2.1.0/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/constants/__init__.py` & `dialogy-2.1.0/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/registry.py` & `dialogy-2.1.0/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.1.0/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.1.0/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.1.0/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.1.0/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.1.0/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.1.0/dialogy/plugins/text/classification/xlmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,20 @@
         if args_map:
             self.args_map = args_map[self.purpose]
         else:
             self.args_map = {}
 
         self.use_calibration = self.args_map.get(const.MODEL_CALIBRATION, False)
 
-        self.ts_parameter: float = self.args_map.get("ts_parameter") or 1.0
+        self.model_dir = self.args_map.get("best_model_dir")
+
+        if self.model_dir:
+            self.ts_parameter: float = read_from_json([const.TS_PARAMETER], self.model_dir,
+                                                      const.CALIBRATION_CONFIG_FILE).get(
+                const.TS_PARAMETER) or self.args_map.get(const.TS_PARAMETER) or 1.0
 
         # flag that specifies whether plugin is being imported externally solely for model
         imported = kwargs.get("imported", False)
 
         if self.purpose in [const.TRAIN, const.TEST] or imported:
             self.use_cuda = torch.cuda.is_available()
             try:
@@ -102,20 +107,19 @@
                     importlib.import_module(const.XLMR_MODULE), const.XLMR_MULTI_CLASS_MODEL
                 )
             except ModuleNotFoundError as error:
                 raise ModuleNotFoundError(
                     "Plugin requires simpletransformers -- https://simpletransformers.ai/docs/installation/"
                 ) from error
 
-            self.model_dir = self.args_map.get("best_model_dir")
             if not self.model_dir:
                 raise ValueError(
                     f"'best_model_dir' missing in passed args_map."
                 )
-            
+
             self.labelencoder = preprocessing.LabelEncoder()
             self.classifier = classifer
             self.model: Any = None
 
             self.labelencoder_file_path = os.path.join(
                 self.model_dir, const.LABELENCODER_FILE
             )
@@ -139,15 +143,14 @@
                     "production or testing, then this should be checked!"
                 )
 
         elif self.purpose == const.PRODUCTION:
             # model inference service session configuration
             self.url = url
             self.timeout = timeout
-            self.session = aiohttp.ClientSession()
             self.headers: Dict[str, str] = {
                 "Content-Type": "application/json"
             }
 
         self.debug = debug
 
     def init_model(self, label_count: Optional[int] = None) -> None:
@@ -191,21 +194,22 @@
     @property
     def valid_labelencoder(self) -> bool:
         return hasattr(self.labelencoder, "classes_")
 
     async def _request_model_inference(self, texts: List[str]) -> Tuple[Any, Any]:
         payload = {"transcripts": texts}
         try:
-            async with self.session.post(self.url, data=json.dumps(payload), headers=self.headers) as resp:
-                status_code = resp.status
-                if status_code == 200:
-                    result = await resp.json()
-                    return result.get("intents", []), result.get("logits", [])
-                else:
-                    result = await resp.text()
+            async with aiohttp.ClientSession() as session:
+                async with session.post(self.url, data=json.dumps(payload), headers=self.headers) as resp:
+                    status_code = resp.status
+                    if status_code == 200:
+                        result = await resp.json()
+                        return result.get("intents", []), result.get("logits", [])
+                    else:
+                        result = await resp.text()
         except ClientConnectorError as connection_error:
             logger.error(f"Model Inference Service is turned off?: {connection_error}")
             logger.error(pformat(payload))
             raise requests.exceptions.ConnectionError from connection_error
 
         # Control flow reaching here would mean the API call wasn't successful.
         # To prevent rest of the things from crashing, we will raise an exception.
```

### Comparing `dialogy-2.0.9/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -979,15 +979,15 @@
         :type args: Tuple(Union[str, List[str]], int, str)
         :return: A list of duckling entities.
         :rtype: List[BaseEntity]
         """
         transcripts = input.transcripts
         self.reference_time = input.reference_time
         self.locale = input.locale or self.locale
-        use_latent = input.latent_entities
+        use_latent = input.latent_entities or self.activate_latent_entities
 
         return await self.parse(
             transcripts,
             locale=self.locale,
             reference_time=self.reference_time,
             use_latent=use_latent,
             intents=output.intents,
@@ -1002,15 +1002,15 @@
         :return: Transformed training data.
         :rtype: pd.DataFrame
         """
         if not self.use_transform:
             return training_data
 
         logger.debug(f"Transforming dataset via {self.__class__.__name__}")
-        logger.disable("dialogy")
+        # logger.disable("dialogy")
         training_data = training_data.copy()
         if self.output_column not in training_data.columns:
             training_data[self.output_column] = None
 
         for i, row in tqdm(training_data.iterrows(), total=len(training_data)):
             reference_time = row[self.reference_time_column]
             if isinstance(reference_time, str):
```

### Comparing `dialogy-2.0.9/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.1.0/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,15 +288,19 @@
                 and passed_not_in_conditions
                 and passed_functional_conditions
             ):
                 if rule[const.MUTATE] == const.INTENT:
                     intents[0].name = mutate_to
                     return intents, const.OUTPUT_DEST_INTENT
                 else:
-                    mutate_entities = [BaseEntity.from_dict(mutate_to)]
+                    mutate_entities = entities
+                    if mutate_to:
+                        mutate_entities.append(BaseEntity.from_dict(mutate_to))
+                    else:
+                        mutate_entities = []
                     return mutate_entities, const.OUTPUT_DEST_ENTITY
 
         return intents, const.OUTPUT_DEST_INTENT
 
     async def utility(
         self, input_: Input, output: Output
     ) -> Tuple[Union[List[Intent], List[BaseEntity]], str]:
```

### Comparing `dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.1.0/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -374,15 +374,15 @@
             return training_data
 
         logger.debug(f"Transforming dataset via {self.__class__.__name__}")
         training_data = training_data.copy()
         if self.output_column not in training_data.columns:
             training_data[self.output_column] = None
 
-        logger.disable("dialogy")
+        # logger.disable("dialogy")
         for i, row in tqdm(training_data.iterrows(), total=len(training_data)):
             transcripts = self.make_transform_values(row[self.input_column])
             entities = self.get_entities(transcripts)
             is_empty_series = isinstance(row[self.output_column], pd.Series) and (
                 row[self.output_column].isnull()
             )
             is_row_nonetype = row[self.output_column] is None
```

### Comparing `dialogy-2.0.9/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.1.0/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
                 Please give either one."
             )
 
         self.threshold = threshold
         self.intent_oos = intent_oos
 
         self.intent_threshold_map = None
-        if intent_threshold_map_path:
+        if intent_threshold_map_path and self.purpose != "train":
             with open(intent_threshold_map_path, "r") as f:
                 self.intent_threshold_map = yaml.safe_load(f)
 
         if self.threshold and self.intent_threshold_map:
             self.threshold = None
             logger.warning(
                 "Both threshold and the intent_threshold_map have been instantiated \
```

### Comparing `dialogy-2.0.9/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.1.0/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.1.0/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/__init__.py` & `dialogy-2.1.0/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/address/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/duration/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/people/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/time/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.1.0/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/intent/__init__.py` & `dialogy-2.1.0/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/types/slots/__init__.py` & `dialogy-2.1.0/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/__init__.py` & `dialogy-2.1.0/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/config.py` & `dialogy-2.1.0/dialogy/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -68,15 +68,15 @@
     def update_paths(self, project_config_path: str) -> None:
         for purpose in self.model_args:
             purpose_args = self.model_args[purpose]
             purpose_args[const.BEST_MODEL_DIR] = os.path.join(
                 project_config_path, purpose_args[const.BEST_MODEL]
             )
             purpose_args[const.OUTPUT_DIR] = os.path.join(
-                project_config_path, purpose_args[const.BEST_MODEL]
+                project_config_path, purpose_args[const.OUTPUT_DIR]
             )
 
 
 @attr.s
 class Tasks(BaseConfig):
     classification = attr.ib(
         type=Task, kw_only=True, validator=attr.validators.instance_of(dict)
@@ -171,14 +171,20 @@
             self.project_artifacts_root_path,
             self._get_data_dir(task_name),
             const.METRICS,
         )
 
     def get_dataset_dir(self, task_name: str) -> str:
         return os.path.join(self.project_artifacts_root_path, self._get_data_dir(task_name), const.DATASETS)
+    
+    def get_model_dir(self, task_name: str) -> str:
+        return os.path.join(
+            self.project_artifacts_root_path,
+            self.model_config.get_model_dir(task_name)
+        )
 
     def get_skip_list(self, task_name: str) -> Set[str]:
         if task_name == const.CLASSIFICATION:
             return set(self.model_config.tasks.classification.skip)
         raise NotImplementedError(f"Model for {task_name} is not defined!")
 
     def get_dataset(self, task_name: str, file_name: str) -> Any:
@@ -230,15 +236,22 @@
                 value = value.replace("\n", "")
                 if value.startswith("{{") and value.endswith("}}"):
                     # python expression detected
                     value = eval(value[2:-2])
             if isinstance(value, dict): # type: ignore
                 if "fetch_from_config" in value.keys(): # type: ignore
                     if isinstance(value["fetch_from_config"], str):
-                        value = config.get(value["fetch_from_config"])
+                        resolved_value = config.get(value["fetch_from_config"])
+                        if resolved_value is None:
+                            logger.error(
+                                f"Value fetched for "
+                                f"{value['fetch_from_config']} "
+                                f"resolves to {resolved_value}"
+                            )
+                        value = resolved_value
             parser[key] = value
         config.pipeline_config.parsers[index] = parser
     return config
 
 
 def get_project_artifacts_path_by_name(project_name: str, project_artifacts_root: str) -> str:
     return os.path.join(project_artifacts_root, project_name, "configs")
@@ -257,15 +270,17 @@
         elif const.CORE_PLUGINS_CONFIG_FILE in file:
             core_plugins_config = yaml_contents
         elif const.MODEL_CONFIG_FILE in file:
             model_config = yaml_contents
         else:
             misc_config.update(yaml_contents)
     if pipeline_config is None or core_plugins_config is None or not model_config:
-        return None
+        raise RuntimeError("One of pipeline config, core_plugins_config or model "
+                           "config is not found. Config for this project won't "
+                           "be loaded")
     # TODO: raise exception for both kind of configs not found
     config = Config(
         **{ # type: ignore
             "project_artifacts_root_path": os.path.join(
                 all_project_artifacts_root, project
             ),
             "pipeline_config": pipeline_config,
@@ -279,14 +294,15 @@
 
 
 def read_project_configs(
     project_artifacts_root: str, filter_list: Optional[List[str]] = None
 ) -> Dict[str, Config]:
     # TODO: raise exception if root is empty
     all_project_configs = {}
+    # logger.enable("dialogy")
     logger.debug(f"Loading configs from {project_artifacts_root}")
     for project in os.listdir(project_artifacts_root):
         # hidden files from editors / OS like .idea
         if project.startswith("."):
             continue
         if filter_list and project not in filter_list:
             continue
@@ -296,9 +312,9 @@
             config = fetch_project_config(project, project_artifacts_root)
         except Exception as e:
             traceback.print_exception(*sys.exc_info())
             logger.debug(f"Failed to load config for {project}")
         if not config:
             continue
         all_project_configs.update({project: config})
-
+    # logger.disable("dialogy")
     return all_project_configs
```

### Comparing `dialogy-2.0.9/dialogy/utils/datetime.py` & `dialogy-2.1.0/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/file_handler.py` & `dialogy-2.1.0/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/logger.py` & `dialogy-2.1.0/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/misc.py` & `dialogy-2.1.0/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/naive_lang_detect.py` & `dialogy-2.1.0/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/normalize_utterance.py` & `dialogy-2.1.0/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/utils/temperature_scaling.py` & `dialogy-2.1.0/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.9/dialogy/workflow/workflow.py` & `dialogy-2.1.0/dialogy/workflow/workflow.py`

 * *Files 8% similar despite different names*

```diff
@@ -111,29 +111,30 @@
         end
 
 """
 from __future__ import annotations
 
 import time
 
+import typing
 from typing import List
 
 import attr
 import pandas as pd
 
 from threading import Lock
 from pprint import pformat
 import asyncio, nest_asyncio
+from collections import OrderedDict
 
 from dialogy import constants as const
 from dialogy.base.input import Input
 from dialogy.base.output import Output
 from dialogy.base.plugin import Plugin
 from dialogy.utils.logger import logger
-from dialogy.utils.misc import _to_task
 
 
 @attr.s
 class Workflow:
     """
     SLU API blackbox.
 
@@ -165,19 +166,35 @@
     NON_SERIALIZABLE_FIELDS = [const.PLUGINS, const.DEBUG, const.LOCK]
 
     def __attrs_post_init__(self) -> None:
         """
         Post init hook.
         """
         self.lock = Lock()
-        for plugin in self.plugins:
-            if isinstance(plugin, Plugin):
-                plugin.debug = self.debug & plugin.debug
 
-    async def run(self, input: Input, output: Output = None):  # type: ignore
+    @typing.no_type_check
+    def log_output(self, executed_plugin: Plugin, input: Input, output: Output) -> None:
+        # PluginProxy
+        if hasattr(executed_plugin, "plugin_name"):
+            plugins_executed_names = executed_plugin.plugin_name
+        # PluginProxyFused
+        elif hasattr(executed_plugin, "plugins"):
+            plugins_executed_names = executed_plugin.plugins
+        else:
+            plugins_executed_names = str(executed_plugin)
+
+        output = {
+            "Resultant Transcripts": input.utterances,
+            "Resultant Feature Input to Classifier": input.clf_feature,
+            "Resultant Output intent": [] if not output.intents else output.intents[0],
+            "Resultant Output entities": output.entities
+        }
+        logger.debug(f"Executed plugin(s) - {plugins_executed_names} \n {pformat(output, sort_dicts=False)}")
+
+    async def run(self, input: Input, output: Output = None, **kwargs):  # type: ignore
         """
         .. _workflow_run:
 
         Get final results from the workflow.
 
         The current workflow exhibits the following simple procedure:
         pre-processing -> inference -> post-processing.
@@ -206,28 +223,29 @@
                     },
                 }
 
             start = time.perf_counter()
             # with self.lock:
             # Removing the lock as plugins are
             # expected to be implemented in a thread safe manner
-            input, output = await plugin(input, output)
+            input, output = await plugin(input, output, **kwargs)
             end = time.perf_counter()
-
+            try:
+                self.log_output(plugin, input, output)
+            except Exception as e:
+                logger.debug(f"logging resultant output after "
+                             f"plugin execution failed because of {e}")
             # logs are available only when debug=False during class initialization
             if self.debug:
                 history["after"] = {
                     "input": input.dict(),
                     "output": output.dict(),
                 }
                 history["perf"] = round(end - start, 4)
 
-            if history:
-                logger.debug(pformat(history))
-
         return input, output
 
     def train(self, training_data: pd.DataFrame) -> Workflow:
         """
         Train all the plugins in the workflow.
 
         Plugin's have a no-op train method by default. The one's that do require training
```

### Comparing `dialogy-2.0.9/pyproject.toml` & `dialogy-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.9"
+version = "2.1.0"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>", "Daksh Varshneya <dakshvar22@gmail.com"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
@@ -31,14 +31,15 @@
 types-setuptools = "^57.4.10"
 black = "^22.8.0"
 googlemaps = "^4.6.0"
 torch = "1.12.1"
 pydantic = "^1.10.2"
 aiohttp = "^3.8.4"
 nest-asyncio = "^1.5.6"
+transformers = "4.30.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.3.1"
 pytest-asyncio = "^0.21.0"
 pytest-cov = "^2.10.1"
 copier = "^6.0.0"
 mypy = "^0.982"
```

### Comparing `dialogy-2.0.9/PKG-INFO` & `dialogy-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.9
+Version: 2.1.0
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -31,12 +31,13 @@
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
 Requires-Dist: scipy (>=1.7.1,<2.0.0)
 Requires-Dist: stanza (>=1.3.0,<2.0.0)
 Requires-Dist: thefuzz (>=0.19.0,<0.20.0)
 Requires-Dist: torch (==1.12.1)
 Requires-Dist: tqdm (>=4.62.2,<5.0.0)
+Requires-Dist: transformers (==4.30.2)
 Requires-Dist: types-pytz (>=2021.3.5,<2022.0.0)
 Requires-Dist: types-requests (>=2.27.11,<3.0.0)
 Requires-Dist: types-setuptools (>=57.4.10,<58.0.0)
 Requires-Dist: xgboost (>=1.5.2,<2.0.0)
 Project-URL: Repository, https://github.com/skit-ai/dialogy
```

