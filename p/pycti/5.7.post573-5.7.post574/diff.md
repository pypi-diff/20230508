# Comparing `tmp/pycti-5.7.post573.tar.gz` & `tmp/pycti-5.7.post574.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.7.post573.tar", last modified: Mon May  8 08:28:40 2023, max compression
+gzip compressed data, was "pycti-5.7.post574.tar", last modified: Mon May  8 08:28:53 2023, max compression
```

## Comparing `pycti-5.7.post573.tar` & `pycti-5.7.post574.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.768725 pycti-5.7.post573/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-08 08:28:26.000000 pycti-5.7.post573/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:40.768725 pycti-5.7.post573/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3141 2023-05-08 08:28:26.000000 pycti-5.7.post573/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.760725 pycti-5.7.post573/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.760725 pycti-5.7.post573/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28104 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.760725 pycti-5.7.post573/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42485 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.768725 pycti-5.7.post573/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23837 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23845 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    63935 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.768725 pycti-5.7.post573/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   101676 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-05-08 08:28:26.000000 pycti-5.7.post573/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.760725 pycti-5.7.post573/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:40.000000 pycti-5.7.post573/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-05-08 08:28:40.000000 pycti-5.7.post573/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 08:28:40.000000 pycti-5.7.post573/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-05-08 08:28:40.000000 pycti-5.7.post573/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-08 08:28:40.000000 pycti-5.7.post573/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-08 08:28:26.000000 pycti-5.7.post573/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-05-08 08:28:40.768725 pycti-5.7.post573/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-05-08 08:28:40.000000 pycti-5.7.post574/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:53.747594 pycti-5.7.post574/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3141 2023-05-08 08:28:40.000000 pycti-5.7.post574/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3724 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28104 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6824 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42485 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18873 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13395 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24396 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23837 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23845 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13878 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14531 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14618 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14175 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14023 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10890 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24602 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22933 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17579 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14043 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23075 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15937 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14475 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7853 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7349 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13002 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14543 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16314 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12155 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13968 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22349 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22661 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20977 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23801 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32054 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41821 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    63935 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18392 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14229 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17702 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.747594 pycti-5.7.post574/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3308 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   101676 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-05-08 08:28:40.000000 pycti-5.7.post574/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-08 08:28:53.739594 pycti-5.7.post574/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4057 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2250 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-05-08 08:28:53.000000 pycti-5.7.post574/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-05-08 08:28:40.000000 pycti-5.7.post574/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-05-08 08:28:53.751594 pycti-5.7.post574/setup.cfg
```

### Comparing `pycti-5.7.post573/LICENSE` & `pycti-5.7.post574/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/PKG-INFO` & `pycti-5.7.post574/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post573
+Version: 5.7.post574
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post573 Summary: Python API
+Metadata-Version: 2.1 Name: pycti Version: 5.7.post574 Summary: Python API
 client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
 python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
 License: Apache Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Natural Language :: French Classifier:
```

### Comparing `pycti-5.7.post573/README.md` & `pycti-5.7.post574/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/__init__.py` & `pycti-5.7.post574/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "5.7.post573"
+__version__ = "5.7.post574"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-5.7.post573/pycti/api/opencti_api_client.py` & `pycti-5.7.post574/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/api/opencti_api_connector.py` & `pycti-5.7.post574/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/api/opencti_api_work.py` & `pycti-5.7.post574/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/connector/opencti_connector.py` & `pycti-5.7.post574/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/connector/opencti_connector_helper.py` & `pycti-5.7.post574/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_attack_pattern.py` & `pycti-5.7.post574/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_campaign.py` & `pycti-5.7.post574/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_case_incident.py` & `pycti-5.7.post574/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_case_rfi.py` & `pycti-5.7.post574/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_case_rft.py` & `pycti-5.7.post574/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_channel.py` & `pycti-5.7.post574/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_course_of_action.py` & `pycti-5.7.post574/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_data_component.py` & `pycti-5.7.post574/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_data_source.py` & `pycti-5.7.post574/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_event.py` & `pycti-5.7.post574/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_external_reference.py` & `pycti-5.7.post574/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_feedback.py` & `pycti-5.7.post574/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_grouping.py` & `pycti-5.7.post574/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_identity.py` & `pycti-5.7.post574/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_incident.py` & `pycti-5.7.post574/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_indicator.py` & `pycti-5.7.post574/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_infrastructure.py` & `pycti-5.7.post574/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_intrusion_set.py` & `pycti-5.7.post574/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.7.post574/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_label.py` & `pycti-5.7.post574/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_language.py` & `pycti-5.7.post574/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_location.py` & `pycti-5.7.post574/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_malware.py` & `pycti-5.7.post574/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_marking_definition.py` & `pycti-5.7.post574/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_narrative.py` & `pycti-5.7.post574/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_note.py` & `pycti-5.7.post574/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_observed_data.py` & `pycti-5.7.post574/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_opinion.py` & `pycti-5.7.post574/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_report.py` & `pycti-5.7.post574/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix.py` & `pycti-5.7.post574/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_core_object.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.7.post574/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_threat_actor.py` & `pycti-5.7.post574/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_tool.py` & `pycti-5.7.post574/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_vocabulary.py` & `pycti-5.7.post574/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/entities/opencti_vulnerability.py` & `pycti-5.7.post574/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/utils/constants.py` & `pycti-5.7.post574/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/utils/opencti_stix2.py` & `pycti-5.7.post574/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.7.post574/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/utils/opencti_stix2_update.py` & `pycti-5.7.post574/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti/utils/opencti_stix2_utils.py` & `pycti-5.7.post574/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti.egg-info/PKG-INFO` & `pycti-5.7.post574/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.7.post573
+Version: 5.7.post574
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.7.post573 Summary: Python API
+Metadata-Version: 2.1 Name: pycti Version: 5.7.post574 Summary: Python API
 client for OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-
 python Author: Filigran Author-email: contact@filigran.io Maintainer: Filigran
 License: Apache Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Information Technology Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Natural Language :: French Classifier:
```

### Comparing `pycti-5.7.post573/pycti.egg-info/SOURCES.txt` & `pycti-5.7.post574/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pycti.egg-info/requires.txt` & `pycti-5.7.post574/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/pyproject.toml` & `pycti-5.7.post574/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.7.post573/setup.cfg` & `pycti-5.7.post574/setup.cfg`

 * *Files identical despite different names*

