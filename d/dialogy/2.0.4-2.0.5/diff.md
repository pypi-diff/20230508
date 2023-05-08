# Comparing `tmp/dialogy-2.0.4.tar.gz` & `tmp/dialogy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dialogy-2.0.4.tar", max compression
+gzip compressed data, was "dialogy-2.0.5.tar", max compression
```

## Comparing `dialogy-2.0.4.tar` & `dialogy-2.0.5.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0     1069 2023-05-04 05:57:52.557232 dialogy-2.0.4/LICENSE.md
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/__init__.py
--rw-r--r--   0        0        0      183 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/base/__init__.py
--rw-r--r--   0        0        0     4949 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/base/entity_extractor/__init__.py
--rw-r--r--   0        0        0     9794 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/base/input/__init__.py
--rw-r--r--   0        0        0     4595 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/base/output/__init__.py
--rw-r--r--   0        0        0    15662 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/base/plugin/__init__.py
--rw-r--r--   0        0        0     3908 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/cli/__init__.py
--rw-r--r--   0        0        0     2587 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/cli/project.py
--rw-r--r--   0        0        0     1865 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/cli/workflow.py
--rw-r--r--   0        0        0     5017 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/constants/__init__.py
--rw-r--r--   0        0        0     2011 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/registry.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/__init__.py
--rw-r--r--   0        0        0     3995 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/address_parser/__init__.py
--rw-r--r--   0        0        0     1406 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/address_parser/mapmyindia.py
--rw-r--r--   0        0        0     4978 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/address_parser/maps.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/calibration/__init__.py
--rw-r--r--   0        0        0     8868 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/calibration/xgb.py
--rw-r--r--   0        0        0     3790 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/canonicalization/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/classification/__init__.py
--rw-r--r--   0        0        0    11805 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/classification/mlp.py
--rw-r--r--   0        0        0     1179 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/classification/retain_intent.py
--rw-r--r--   0        0        0       58 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/classification/tokenizers.py
--rw-r--r--   0        0        0    17246 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/classification/xlmr.py
--rw-r--r--   0        0        0     7676 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/combine_date_time/__init__.py
--rw-r--r--   0        0        0    39327 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/duckling_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/error_recovery/__init__.py
--rw-r--r--   0        0        0    20334 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/error_recovery/error_recovery.py
--rw-r--r--   0        0        0    12300 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/__init__.py
--rw-r--r--   0        0        0      743 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
--rw-r--r--   0        0        0      797 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/const.py
--rw-r--r--   0        0        0      313 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/registry.py
--rw-r--r--   0        0        0     1792 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/lb_plugin/__init__.py
--rw-r--r--   0        0        0    14123 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/list_entity_plugin/__init__.py
--rw-r--r--   0        0        0    11523 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/list_search_plugin/__init__.py
--rw-r--r--   0        0        0     4841 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/list_search_plugin/sample_config.yaml
--rw-r--r--   0        0        0     4699 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/merge_asr_output/__init__.py
--rw-r--r--   0        0        0     1565 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/oos_filter/__init__.py
--rw-r--r--   0        0        0     4247 2023-05-04 05:57:52.557232 dialogy-2.0.4/dialogy/plugins/text/qc_plugin/__init__.py
--rw-r--r--   0        0        0      833 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/plugins/text/slot_filler/__init__.py
--rw-r--r--   0        0        0     4148 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/plugins/text/slot_filler/rule_slot_filler.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/plugins/text/voting/__init__.py
--rw-r--r--   0        0        0     1862 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/__init__.py
--rw-r--r--   0        0        0      170 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/__init__.py
--rw-r--r--   0        0        0      914 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/address/__init__.py
--rw-r--r--   0        0        0     1811 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/amount_of_money/__init__.py
--rw-r--r--   0        0        0     7338 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/base_entity/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/credit_card_number/__init__.py
--rw-r--r--   0        0        0     3637 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/deserialize/__init__.py
--rw-r--r--   0        0        0     4317 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/duration/__init__.py
--rw-r--r--   0        0        0      975 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/keyword/__init__.py
--rw-r--r--   0        0        0     4698 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/numerical/__init__.py
--rw-r--r--   0        0        0     2271 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/people/__init__.py
--rw-r--r--   0        0        0      910 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/pincode/__init__.py
--rw-r--r--   0        0        0    13534 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/time/__init__.py
--rw-r--r--   0        0        0     8803 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/entity/time_interval/__init__.py
--rw-r--r--   0        0        0     8893 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/intent/__init__.py
--rw-r--r--   0        0        0      154 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/signal/__init__.py
--rw-r--r--   0        0        0      194 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/signal/signal.py
--rw-r--r--   0        0        0      991 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/slots/__init__.py
--rw-r--r--   0        0        0      191 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/types/utterances/__init__.py
--rw-r--r--   0        0        0      638 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/__init__.py
--rw-r--r--   0        0        0    10469 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/config.py
--rw-r--r--   0        0        0     2180 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/datetime.py
--rw-r--r--   0        0        0     3437 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/file_handler.py
--rw-r--r--   0        0        0      808 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/logger.py
--rw-r--r--   0        0        0     2687 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/misc.py
--rw-r--r--   0        0        0      584 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/naive_lang_detect.py
--rw-r--r--   0        0        0     8236 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/normalize_utterance.py
--rw-r--r--   0        0        0     3605 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/utils/temperature_scaling.py
--rw-r--r--   0        0        0       47 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/workflow/__init__.py
--rw-r--r--   0        0        0     6795 2023-05-04 05:57:52.561231 dialogy-2.0.4/dialogy/workflow/workflow.py
--rw-r--r--   0        0        0     1425 2023-05-04 05:58:08.461347 dialogy-2.0.4/pyproject.toml
--rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 dialogy-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-08 05:01:39.708229 dialogy-2.0.5/LICENSE.md
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/__init__.py
+-rw-r--r--   0        0        0      183 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/__init__.py
+-rw-r--r--   0        0        0     4949 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/entity_extractor/__init__.py
+-rw-r--r--   0        0        0     9777 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/input/__init__.py
+-rw-r--r--   0        0        0     4595 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/output/__init__.py
+-rw-r--r--   0        0        0    15662 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/base/plugin/__init__.py
+-rw-r--r--   0        0        0     3908 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/__init__.py
+-rw-r--r--   0        0        0     2587 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/project.py
+-rw-r--r--   0        0        0     1865 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/cli/workflow.py
+-rw-r--r--   0        0        0     5017 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/constants/__init__.py
+-rw-r--r--   0        0        0     2011 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/registry.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/__init__.py
+-rw-r--r--   0        0        0     3995 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/__init__.py
+-rw-r--r--   0        0        0     1406 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/mapmyindia.py
+-rw-r--r--   0        0        0     4978 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/address_parser/maps.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/calibration/__init__.py
+-rw-r--r--   0        0        0     8868 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/calibration/xgb.py
+-rw-r--r--   0        0        0     3790 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/canonicalization/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/__init__.py
+-rw-r--r--   0        0        0    11805 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/mlp.py
+-rw-r--r--   0        0        0     1179 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/retain_intent.py
+-rw-r--r--   0        0        0       58 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/tokenizers.py
+-rw-r--r--   0        0        0    17246 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/classification/xlmr.py
+-rw-r--r--   0        0        0     7676 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/combine_date_time/__init__.py
+-rw-r--r--   0        0        0    39327 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/duckling_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/error_recovery/__init__.py
+-rw-r--r--   0        0        0    20334 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/error_recovery/error_recovery.py
+-rw-r--r--   0        0        0    12300 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/__init__.py
+-rw-r--r--   0        0        0      743 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py
+-rw-r--r--   0        0        0      797 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/const.py
+-rw-r--r--   0        0        0      313 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/registry.py
+-rw-r--r--   0        0        0     1792 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/lb_plugin/__init__.py
+-rw-r--r--   0        0        0    14123 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_entity_plugin/__init__.py
+-rw-r--r--   0        0        0    11523 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/__init__.py
+-rw-r--r--   0        0        0     4841 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/sample_config.yaml
+-rw-r--r--   0        0        0     4699 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/merge_asr_output/__init__.py
+-rw-r--r--   0        0        0     1565 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/oos_filter/__init__.py
+-rw-r--r--   0        0        0     4247 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/qc_plugin/__init__.py
+-rw-r--r--   0        0        0      833 2023-05-08 05:01:39.708229 dialogy-2.0.5/dialogy/plugins/text/slot_filler/__init__.py
+-rw-r--r--   0        0        0     4148 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/plugins/text/slot_filler/rule_slot_filler.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/plugins/text/voting/__init__.py
+-rw-r--r--   0        0        0     1862 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/__init__.py
+-rw-r--r--   0        0        0      170 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/__init__.py
+-rw-r--r--   0        0        0      914 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/address/__init__.py
+-rw-r--r--   0        0        0     1811 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/amount_of_money/__init__.py
+-rw-r--r--   0        0        0     7338 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/base_entity/__init__.py
+-rw-r--r--   0        0        0     2281 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/credit_card_number/__init__.py
+-rw-r--r--   0        0        0     3637 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/deserialize/__init__.py
+-rw-r--r--   0        0        0     4317 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/duration/__init__.py
+-rw-r--r--   0        0        0      975 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/keyword/__init__.py
+-rw-r--r--   0        0        0     4698 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/numerical/__init__.py
+-rw-r--r--   0        0        0     2271 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/people/__init__.py
+-rw-r--r--   0        0        0      910 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/pincode/__init__.py
+-rw-r--r--   0        0        0    13534 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/time/__init__.py
+-rw-r--r--   0        0        0     8803 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/entity/time_interval/__init__.py
+-rw-r--r--   0        0        0     8893 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/intent/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/signal/__init__.py
+-rw-r--r--   0        0        0      194 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/signal/signal.py
+-rw-r--r--   0        0        0      991 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/slots/__init__.py
+-rw-r--r--   0        0        0      191 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/types/utterances/__init__.py
+-rw-r--r--   0        0        0      638 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/__init__.py
+-rw-r--r--   0        0        0    10469 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/config.py
+-rw-r--r--   0        0        0     2180 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/datetime.py
+-rw-r--r--   0        0        0     3437 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/file_handler.py
+-rw-r--r--   0        0        0      808 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/logger.py
+-rw-r--r--   0        0        0     2687 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/misc.py
+-rw-r--r--   0        0        0      584 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/naive_lang_detect.py
+-rw-r--r--   0        0        0     8236 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/normalize_utterance.py
+-rw-r--r--   0        0        0     3605 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/utils/temperature_scaling.py
+-rw-r--r--   0        0        0       47 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/workflow/__init__.py
+-rw-r--r--   0        0        0     6795 2023-05-08 05:01:39.712229 dialogy-2.0.5/dialogy/workflow/workflow.py
+-rw-r--r--   0        0        0     1425 2023-05-08 05:01:56.172423 dialogy-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1611 1970-01-01 00:00:00.000000 dialogy-2.0.5/PKG-INFO
```

### Comparing `dialogy-2.0.4/LICENSE.md` & `dialogy-2.0.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/base/entity_extractor/__init__.py` & `dialogy-2.0.5/dialogy/base/entity_extractor/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/base/input/__init__.py` & `dialogy-2.0.5/dialogy/base/input/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,14 @@
         for k, d in defaults.items():
             data[k] = data.get(k, d) or d
 
         super().__init__(**data)
 
     @validator("reference_time")
     def check_reference_time(cls, v):  # type: ignore
-        print(v)
         if not v:
             return None
         if not is_unix_ts(v):
             raise ValueError(f"`reference_time` must be a unix timestamp but got {v}.")
         return v
 
     @classmethod
```

### Comparing `dialogy-2.0.4/dialogy/base/output/__init__.py` & `dialogy-2.0.5/dialogy/base/output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/base/plugin/__init__.py` & `dialogy-2.0.5/dialogy/base/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/cli/__init__.py` & `dialogy-2.0.5/dialogy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/cli/project.py` & `dialogy-2.0.5/dialogy/cli/project.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/cli/workflow.py` & `dialogy-2.0.5/dialogy/cli/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/constants/__init__.py` & `dialogy-2.0.5/dialogy/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/registry.py` & `dialogy-2.0.5/dialogy/plugins/registry.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/address_parser/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/address_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/address_parser/mapmyindia.py` & `dialogy-2.0.5/dialogy/plugins/text/address_parser/mapmyindia.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/address_parser/maps.py` & `dialogy-2.0.5/dialogy/plugins/text/address_parser/maps.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/calibration/xgb.py` & `dialogy-2.0.5/dialogy/plugins/text/calibration/xgb.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/canonicalization/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/canonicalization/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/classification/mlp.py` & `dialogy-2.0.5/dialogy/plugins/text/classification/mlp.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/classification/retain_intent.py` & `dialogy-2.0.5/dialogy/plugins/text/classification/retain_intent.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/classification/xlmr.py` & `dialogy-2.0.5/dialogy/plugins/text/classification/xlmr.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/combine_date_time/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/combine_date_time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/duckling_plugin/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/duckling_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/error_recovery/error_recovery.py` & `dialogy-2.0.5/dialogy/plugins/text/error_recovery/error_recovery.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py` & `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/actions_on_primitives.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/intent_entity_mutator/const.py` & `dialogy-2.0.5/dialogy/plugins/text/intent_entity_mutator/const.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/lb_plugin/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/lb_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/list_entity_plugin/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/list_entity_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/list_search_plugin/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/list_search_plugin/sample_config.yaml` & `dialogy-2.0.5/dialogy/plugins/text/list_search_plugin/sample_config.yaml`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/merge_asr_output/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/merge_asr_output/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/oos_filter/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/oos_filter/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/qc_plugin/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/qc_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/slot_filler/__init__.py` & `dialogy-2.0.5/dialogy/plugins/text/slot_filler/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/plugins/text/slot_filler/rule_slot_filler.py` & `dialogy-2.0.5/dialogy/plugins/text/slot_filler/rule_slot_filler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/__init__.py` & `dialogy-2.0.5/dialogy/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/address/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/address/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/amount_of_money/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/amount_of_money/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/base_entity/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/base_entity/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/credit_card_number/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/credit_card_number/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/deserialize/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/deserialize/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/duration/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/duration/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/keyword/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/keyword/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/numerical/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/numerical/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/people/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/people/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/pincode/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/pincode/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/time/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/time/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/entity/time_interval/__init__.py` & `dialogy-2.0.5/dialogy/types/entity/time_interval/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/intent/__init__.py` & `dialogy-2.0.5/dialogy/types/intent/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/types/slots/__init__.py` & `dialogy-2.0.5/dialogy/types/slots/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/__init__.py` & `dialogy-2.0.5/dialogy/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/config.py` & `dialogy-2.0.5/dialogy/utils/config.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/datetime.py` & `dialogy-2.0.5/dialogy/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/file_handler.py` & `dialogy-2.0.5/dialogy/utils/file_handler.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/logger.py` & `dialogy-2.0.5/dialogy/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/misc.py` & `dialogy-2.0.5/dialogy/utils/misc.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/naive_lang_detect.py` & `dialogy-2.0.5/dialogy/utils/naive_lang_detect.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/normalize_utterance.py` & `dialogy-2.0.5/dialogy/utils/normalize_utterance.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/utils/temperature_scaling.py` & `dialogy-2.0.5/dialogy/utils/temperature_scaling.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/dialogy/workflow/workflow.py` & `dialogy-2.0.5/dialogy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `dialogy-2.0.4/pyproject.toml` & `dialogy-2.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dialogy"
-version = "2.0.4"
+version = "2.0.5"
 description = "Dialogy is a library for building and managing SLU applications."
 authors = ["Amresh Venugopal <amresh.venugopal@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/skit-ai/dialogy"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
```

### Comparing `dialogy-2.0.4/PKG-INFO` & `dialogy-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dialogy
-Version: 2.0.4
+Version: 2.0.5
 Summary: Dialogy is a library for building and managing SLU applications.
 Home-page: https://github.com/skit-ai/dialogy
 License: MIT
 Author: Amresh Venugopal
 Author-email: amresh.venugopal@gmail.com
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

