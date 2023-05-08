# Comparing `tmp/demisto_sdk-1.8.3.tar.gz` & `tmp/demisto_sdk-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demisto_sdk-1.8.3.tar", max compression
+gzip compressed data, was "demisto_sdk-1.9.0.tar", max compression
```

## Comparing `demisto_sdk-1.8.3.tar` & `demisto_sdk-1.9.0.tar`

### file list

```diff
@@ -1,890 +1,876 @@
--rw-r--r--   0        0        0     1064 2023-01-08 14:17:44.276975 demisto_sdk-1.8.3/LICENSE
--rw-r--r--   0        0        0     8146 2023-01-08 14:17:44.276975 demisto_sdk-1.8.3/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/__init__.py
--rw-r--r--   0        0        0    99796 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/__main__.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/__init__.py
--rw-r--r--   0        0        0     4150 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/MDXServer.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/__init__.py
--rw-r--r--   0        0        0      878 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/configuration.py
--rw-r--r--   0        0        0    60552 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/constants.py
--rw-r--r--   0        0        0     5016 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/README.md
--rw-r--r--   0        0        0      451 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/__init__.py
--rw-r--r--   0        0        0     4670 2023-01-08 14:17:44.280975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/content.py
--rw-r--r--   0        0        0     3671 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/docs/CONTRIBUTION.md
--rw-r--r--   0        0        0     3339 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/errors.py
--rw-r--r--   0        0        0      324 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/__init__.py
--rw-r--r--   0        0        0     2499 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/dictionary_based_object.py
--rw-r--r--   0        0        0     3264 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/general_object.py
--rw-r--r--   0        0        0     2195 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/json_object.py
--rw-r--r--   0        0        0     1439 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/text_object.py
--rw-r--r--   0        0        0     2440 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/yaml_object.py
--rw-r--r--   0        0        0     2346 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/__init__.py
--rw-r--r--   0        0        0     4544 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/json_content_object.py
--rw-r--r--   0        0        0     4521 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_content_object.py
--rw-r--r--   0        0        0     6360 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_unify_content_object.py
--rw-r--r--   0        0        0      256 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/author_image/author_image.py
--rw-r--r--   0        0        0      389 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/change_log/change_log.py
--rw-r--r--   0        0        0     1969 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/classifier/classifier.py
--rw-r--r--   0        0        0      447 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/connection/connection.py
--rw-r--r--   0        0        0      481 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/contributors/contributors.py
--rw-r--r--   0        0        0     2862 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/corrlation_rule/correlation_rule.py
--rw-r--r--   0        0        0      832 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/dashboard/dashboard.py
--rw-r--r--   0        0        0      252 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/doc_file/doc_file.py
--rw-r--r--   0        0        0      568 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_definition/generic_definition.py
--rw-r--r--   0        0        0      548 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_field/generic_field.py
--rw-r--r--   0        0        0      552 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_module/generic_module.py
--rw-r--r--   0        0        0      544 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_type/generic_type.py
--rw-r--r--   0        0        0     1495 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/incident_field/incident_field.py
--rw-r--r--   0        0        0     1483 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/incident_type/incident_type.py
--rw-r--r--   0        0        0     3015 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/indicator_field/indicator_field.py
--rw-r--r--   0        0        0     2048 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/indicator_type/indicator_type.py
--rw-r--r--   0        0        0     2260 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/integration/integration.py
--rw-r--r--   0        0        0      967 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/job/job.py
--rw-r--r--   0        0        0     3949 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/layout/layout.py
--rw-r--r--   0        0        0     1109 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/lists/lists.py
--rw-r--r--   0        0        0    10845 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/modeling_rule/modeling_rule.py
--rw-r--r--   0        0        0    20618 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pack.py
--rw-r--r--   0        0        0      255 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pack_ignore/pack_ignore.py
--rw-r--r--   0        0        0    19280 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pack_metadata/pack_metadata.py
--rw-r--r--   0        0        0     2877 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/parsing_rule/parsing_rule.py
--rw-r--r--   0        0        0      938 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/playbook/playbook.py
--rw-r--r--   0        0        0      925 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pre_process_rule/pre_process_rule.py
--rw-r--r--   0        0        0     2090 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/readme/readme.py
--rw-r--r--   0        0        0      374 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/release_note/release_note.py
--rw-r--r--   0        0        0      387 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/release_note_config/release_note_config.py
--rw-r--r--   0        0        0      819 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/report/report.py
--rw-r--r--   0        0        0     1710 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/script/script.py
--rw-r--r--   0        0        0      257 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/secret_ignore/secret_ignore.py
--rw-r--r--   0        0        0     2847 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/tool/agent_tool.py
--rw-r--r--   0        0        0     2800 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/trigger/trigger.py
--rw-r--r--   0        0        0      814 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/widget/widget.py
--rw-r--r--   0        0        0      430 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/wizard/wizard.py
--rw-r--r--   0        0        0     3603 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xdrc_template/xdrc_template.py
--rw-r--r--   0        0        0     3746 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard/xsiam_dashboard.py
--rw-r--r--   0        0        0      936 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image.py
--rw-r--r--   0        0        0     3707 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report/xsiam_report.py
--rw-r--r--   0        0        0      930 2023-01-08 14:17:44.284975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report_image/xsiam_report_image.py
--rw-r--r--   0        0        0      309 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/root_objects/__init__.py
--rw-r--r--   0        0        0      283 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/root_objects/content_descriptor/content_descriptor.py
--rw-r--r--   0        0        0      358 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/root_objects/documentation/documentation.py
--rw-r--r--   0        0        0     4506 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects_factory.py
--rw-r--r--   0        0        0     1535 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/content_test.py
--rw-r--r--   0        0        0     2119 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/json_object_test.py
--rw-r--r--   0        0        0      696 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/text_object_test.py
--rw-r--r--   0        0        0     2114 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/yaml_object_test.py
--rw-r--r--   0        0        0     1773 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/json_content_object_test.py
--rw-r--r--   0        0        0     1628 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/yaml_content_object_test.py
--rw-r--r--   0        0        0      704 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/author_image/author_image_test.py
--rw-r--r--   0        0        0      743 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/change_log/change_log_test.py
--rw-r--r--   0        0        0       45 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test/classifier_mapper.json
--rw-r--r--   0        0        0       51 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test/old_classifier.json
--rw-r--r--   0        0        0     1611 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test.py
--rw-r--r--   0        0        0      790 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/connection/connection_test.py
--rw-r--r--   0        0        0     1228 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/correlation_rule/correlation_rule_test.py
--rw-r--r--   0        0        0      732 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/dashboard/dashboard_test.py
--rw-r--r--   0        0        0      695 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/doc_file/doc_file_test.py
--rw-r--r--   0        0        0      778 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_field/incident_field_test.py
--rw-r--r--   0        0        0      768 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_type/incident_type_test.py
--rw-r--r--   0        0        0      601 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_field/indicator_field_test.py
--rw-r--r--   0        0        0       28 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test/reputations.json
--rw-r--r--   0        0        0     1374 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample.py
--rw-r--r--   0        0        0       17 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample.yml
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample_description.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample_image.png
--rw-r--r--   0        0        0       17 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample.yml
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample_CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample_README.md
--rw-r--r--   0        0        0     1834 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test.py
--rw-r--r--   0        0        0     1717 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test/Jobs/sample-job.json
--rw-r--r--   0        0        0      692 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test.py
--rw-r--r--   0        0        0       43 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/layout/layout_test/layoutscontainer-Zimperium_event.json
--rw-r--r--   0        0        0      924 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/layout/layout_test.py
--rw-r--r--   0        0        0      999 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/lists/lists_test.py
--rw-r--r--   0        0        0    13581 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/modeling_rule/modeling_rule_test.py
--rw-r--r--   0        0        0      673 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_ignore/pack_ignore_test.py
--rw-r--r--   0        0        0    11272 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_metadata/pack_metadata_test.py
--rw-r--r--   0        0        0     5630 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_test.py
--rw-r--r--   0        0        0     2749 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/parsing_rule/parsing_rule_test.py
--rw-r--r--   0        0        0      721 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/playbook/playbook_test.py
--rw-r--r--   0        0        0     1227 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pre_process_rule/pre_process_rule_test.py
--rw-r--r--   0        0        0     2286 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/readme/readme_test.py
--rw-r--r--   0        0        0      723 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note/release_note_test.py
--rw-r--r--   0        0        0     1046 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note_config/release_note_config_test.py
--rw-r--r--   0        0        0      686 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/report/report_test.py
--rw-r--r--   0        0        0      189 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/CHANGELOG.md
--rw-r--r--   0        0        0     7106 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.py
--rw-r--r--   0        0        0       15 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.yml
--rw-r--r--   0        0        0       15 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestUnifiedScript/script-FindSimilarIncidentsByText.yml
--rw-r--r--   0        0        0      189 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestUnifiedScript/script-FindSimilarIncidentsByText_CHANGELOG.md
--rw-r--r--   0        0        0     1868 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test.py
--rw-r--r--   0        0        0      694 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/secret_ignore/secret_ignore_test.py
--rw-r--r--   0        0        0      886 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/trigger/trigger_test.py
--rw-r--r--   0        0        0      686 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/widget/widget_test.py
--rw-r--r--   0        0        0     3855 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test/Wizards/sample-wizard.json
--rw-r--r--   0        0        0      743 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test.py
--rw-r--r--   0        0        0     1255 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xdrctemplate/xdrc_template_test.py
--rw-r--r--   0        0        0     1209 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard/xsiam_dashboard_test.py
--rw-r--r--   0        0        0      651 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image_test.py
--rw-r--r--   0        0        0     1107 2023-01-08 14:17:44.288975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report/xsiam_report_test.py
--rw-r--r--   0        0        0      608 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report_image/xsiam_report_image_test.py
--rw-r--r--   0        0        0      448 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/root_objects/content_descriptor/content_descriptor_test.py
--rw-r--r--   0        0        0      471 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/root_objects/documentation/documentation_test.py
--rw-r--r--   0        0        0      474 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/content_constant_paths.py
--rw-r--r--   0        0        0      402 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/cpu_count.py
--rw-r--r--   0        0        0      292 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/default_additional_info.json
--rw-r--r--   0        0        0      322 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/default_additional_info_loader.py
--rw-r--r--   0        0        0    13750 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/default_output_descriptions.json
--rw-r--r--   0        0        0     9522 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/docker_helper.py
--rw-r--r--   0        0        0   147686 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/errors.py
--rw-r--r--   0        0        0    14200 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/git_content_config.py
--rw-r--r--   0        0        0    31280 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/git_util.py
--rw-r--r--   0        0        0      258 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/__init__.py
--rw-r--r--   0        0        0      177 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/handlers_utils.py
--rw-r--r--   0        0        0     1200 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/json/orjson_handler.py
--rw-r--r--   0        0        0     1631 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/json/ujson_handler.py
--rw-r--r--   0        0        0      922 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/tests/json_test.py
--rw-r--r--   0        0        0      456 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/xsoar_handler.py
--rw-r--r--   0        0        0     1781 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/yaml/ruamel_handler.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/__init__.py
--rw-r--r--   0        0        0     2416 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/author_image.py
--rw-r--r--   0        0        0    16414 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/base_validator.py
--rw-r--r--   0        0        0     9918 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/classifier.py
--rw-r--r--   0        0        0     7937 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/conf_json.py
--rw-r--r--   0        0        0    23428 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/content_entity_validator.py
--rw-r--r--   0        0        0     2734 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/correlation_rule.py
--rw-r--r--   0        0        0     5322 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/dashboard.py
--rw-r--r--   0        0        0    11133 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/deprecation.py
--rw-r--r--   0        0        0    11600 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/description.py
--rw-r--r--   0        0        0    20586 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/docker.py
--rw-r--r--   0        0        0    19923 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/field_base_validator.py
--rw-r--r--   0        0        0      714 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_definition.py
--rw-r--r--   0        0        0     2876 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_field.py
--rw-r--r--   0        0        0      698 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_module.py
--rw-r--r--   0        0        0      690 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_type.py
--rw-r--r--   0        0        0    39761 2023-01-08 14:17:44.292975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/id.py
--rw-r--r--   0        0        0     9781 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/image.py
--rw-r--r--   0        0        0     3000 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/incident_field.py
--rw-r--r--   0        0        0     7866 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/incident_type.py
--rw-r--r--   0        0        0     3560 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/indicator_field.py
--rw-r--r--   0        0        0    93032 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/integration.py
--rw-r--r--   0        0        0     4393 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/job.py
--rw-r--r--   0        0        0    12968 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/layout.py
--rw-r--r--   0        0        0     2565 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/lists.py
--rw-r--r--   0        0        0     9981 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/mapper.py
--rw-r--r--   0        0        0     7931 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/modeling_rule.py
--rw-r--r--   0        0        0     7430 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/old_release_notes.py
--rw-r--r--   0        0        0    45509 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/pack_unique_files.py
--rw-r--r--   0        0        0     2290 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/parsing_rule.py
--rw-r--r--   0        0        0    45447 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/playbook.py
--rw-r--r--   0        0        0     6043 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/pre_process_rule.py
--rw-r--r--   0        0        0     2087 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/python_file.py
--rw-r--r--   0        0        0    32971 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/readme.py
--rw-r--r--   0        0        0    20094 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/release_notes.py
--rw-r--r--   0        0        0     1968 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/release_notes_config.py
--rw-r--r--   0        0        0      708 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/report.py
--rw-r--r--   0        0        0     4395 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/reputation.py
--rw-r--r--   0        0        0    19526 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/script.py
--rw-r--r--   0        0        0    20363 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/structure.py
--rw-r--r--   0        0        0     3681 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/test_playbook.py
--rw-r--r--   0        0        0     1016 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/triggers.py
--rw-r--r--   0        0        0     1921 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/widget.py
--rw-r--r--   0        0        0     8213 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/wizard.py
--rw-r--r--   0        0        0     1993 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xdrc_templates.py
--rw-r--r--   0        0        0     1996 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsiam_dashboard.py
--rw-r--r--   0        0        0     1983 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsiam_report.py
--rw-r--r--   0        0        0     4312 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsoar_config_json.py
--rw-r--r--   0        0        0    16565 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/legacy_git_tools.py
--rw-r--r--   0        0        0     5238 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/logger.py
--rw-r--r--   0        0        0      896 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/mdx-parse-server.js
--rw-r--r--   0        0        0      445 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/mdx-parse.js
--rw-r--r--   0        0        0     6242 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/native_image.py
--rw-r--r--   0        0        0      482 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/canvas-context-connections.yml
--rw-r--r--   0        0        0      950 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/classifier.yml
--rw-r--r--   0        0        0      741 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/classifier_5_9_9.yml
--rw-r--r--   0        0        0      988 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/dashboard.yml
--rw-r--r--   0        0        0      357 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/genericdefinition.yml
--rw-r--r--   0        0        0     1527 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/genericfield.yml
--rw-r--r--   0        0        0     1193 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/genericmodule.yml
--rw-r--r--   0        0        0     1156 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/generictype.yml
--rw-r--r--   0        0        0     2062 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidentfield.yml
--rw-r--r--   0        0        0     1957 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidentfields.yml
--rw-r--r--   0        0        0     1158 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidenttype.yml
--rw-r--r--   0        0        0     1366 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/indicatorfield.yml
--rw-r--r--   0        0        0     4771 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/integration.yml
--rw-r--r--   0        0        0     4455 2023-01-08 14:17:44.296975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/job.yml
--rw-r--r--   0        0        0     1569 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/layout.yml
--rw-r--r--   0        0        0     3389 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/layoutscontainer.yml
--rw-r--r--   0        0        0     1073 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/list.yml
--rw-r--r--   0        0        0      606 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/mapper.yml
--rw-r--r--   0        0        0     8150 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/playbook.yml
--rw-r--r--   0        0        0     1434 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/pre-process-rules.yml
--rw-r--r--   0        0        0      131 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/releasenotesconfig.yml
--rw-r--r--   0        0        0     3356 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/report.yml
--rw-r--r--   0        0        0     1133 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/reputation.yml
--rw-r--r--   0        0        0     2822 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/script.yml
--rw-r--r--   0        0        0      637 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/widget.yml
--rw-r--r--   0        0        0     2059 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/wizard.yml
--rw-r--r--   0        0        0     4251 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/xsoar_config.json
--rw-r--r--   0        0        0      203 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/singleton.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/__init__.py
--rw-r--r--   0        0        0     3305 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/author_image_validator_test.py
--rw-r--r--   0        0        0    23120 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/base_validator_test.py
--rw-r--r--   0        0        0     4801 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/classifier_test.py
--rw-r--r--   0        0        0     8959 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/conf_test.py
--rw-r--r--   0        0        0    11318 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/content_entity_validator_test.py
--rw-r--r--   0        0        0     1203 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/correlation_rules_test.py
--rw-r--r--   0        0        0      457 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/cpu_count_test.py
--rw-r--r--   0        0        0     3578 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/dashboard_test.py
--rw-r--r--   0        0        0    42912 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/dependencies_test.py
--rw-r--r--   0        0        0    17068 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/deprecation_test.py
--rw-r--r--   0        0        0     6648 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/description_test.py
--rw-r--r--   0        0        0    27939 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/docker_test.py
--rw-r--r--   0        0        0     8580 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/errors_test.py
--rw-r--r--   0        0        0    23020 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/field_validator_test.py
--rw-r--r--   0        0        0     2233 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/generic_field_test.py
--rw-r--r--   0        0        0    13122 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/git_config_test.py
--rw-r--r--   0        0        0     1734 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/git_util_test.py
--rw-r--r--   0        0        0    61328 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/id_test.py
--rw-r--r--   0        0        0     7473 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/image_test.py
--rw-r--r--   0        0        0     1862 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/incident_field_test.py
--rw-r--r--   0        0        0     8373 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/incident_type_test.py
--rw-r--r--   0        0        0     4004 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/indicator_field_test.py
--rw-r--r--   0        0        0    91854 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/integration_test.py
--rw-r--r--   0        0        0     4590 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/layout_test.py
--rw-r--r--   0        0        0     6851 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/legacy_git_tools_test.py
--rw-r--r--   0        0        0     2358 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/lists_test.py
--rw-r--r--   0        0        0     3142 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/mapper_test.py
--rw-r--r--   0        0        0     7370 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/modeling_rules_test.py
--rw-r--r--   0        0        0     3416 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/native_image_test.py
--rw-r--r--   0        0        0     4391 2023-01-08 14:17:44.300975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/old_release_notes_test.py
--rw-r--r--   0        0        0    18689 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pack_metadata_validator_test.py
--rw-r--r--   0        0        0    47313 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pack_unique_files_test.py
--rw-r--r--   0        0        0    31317 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/playbook_test.py
--rw-r--r--   0        0        0      657 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pre_process_rule_test.py
--rw-r--r--   0        0        0      767 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/python_file_test.py
--rw-r--r--   0        0        0    25149 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/readme_test.py
--rw-r--r--   0        0        0     2021 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/release_notes_config_test.py
--rw-r--r--   0        0        0    28486 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/release_notes_test.py
--rw-r--r--   0        0        0     2599 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/reputation_test.py
--rw-r--r--   0        0        0    21395 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/script_test.py
--rw-r--r--   0        0        0    24431 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/structure_test.py
--rw-r--r--   0        0        0     1093 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/docker_native_image_config.json
--rw-r--r--   0        0        0      880 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/invalid_correlation_rule.yml
--rw-r--r--   0        0        0     1140 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/rn_header_test_data
--rw-r--r--   0        0        0    79543 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/test_changelog.md
--rw-r--r--   0        0        0     1842 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/timers_test.py
--rw-r--r--   0        0        0    77885 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/tools_test.py
--rw-r--r--   0        0        0   137669 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/update_id_set_test.py
--rw-r--r--   0        0        0     1521 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/widget_test.py
--rw-r--r--   0        0        0     6753 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/wizards_test.py
--rw-r--r--   0        0        0     8057 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/xsoar_config_file_test.py
--rw-r--r--   0        0        0     7562 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/timers.py
--rw-r--r--   0        0        0   110475 2023-01-08 14:17:44.304975 demisto_sdk-1.8.3/demisto_sdk/commands/common/tools.py
--rwxr-xr-x   0        0        0   133258 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/common/update_id_set.py
--rw-r--r--   0        0        0     2480 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/__init__.py
--rw-r--r--   0        0        0    20437 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/common.py
--rw-r--r--   0        0        0     3019 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/content_graph_builder.py
--rw-r--r--   0        0        0     4105 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/content_graph_commands.py
--rw-r--r--   0        0        0   292334 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/architecture.png
--rw-r--r--   0        0        0   244414 2023-01-08 14:17:44.308976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/models.png
--rw-r--r--   0        0        0   236398 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/parsers.png
--rw-r--r--   0        0        0     3465 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/graph.py
--rw-r--r--   0        0        0     3675 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/import_utils.py
--rw-r--r--   0        0        0    15188 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/neo4j_graph.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/__init__.py
--rw-r--r--   0        0        0     1943 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/common.py
--rw-r--r--   0        0        0     2253 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/constraints.py
--rw-r--r--   0        0        0    11223 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/dependencies.py
--rw-r--r--   0        0        0     3604 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/import_export.py
--rw-r--r--   0        0        0     1692 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/indexes.py
--rw-r--r--   0        0        0     4999 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/nodes.py
--rw-r--r--   0        0        0     7829 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/relationships.py
--rw-r--r--   0        0        0     5232 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/neo4j_service.py
--rw-r--r--   0        0        0     2904 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/__init__.py
--rw-r--r--   0        0        0     6605 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/base_content.py
--rw-r--r--   0        0        0      474 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/classifier.py
--rw-r--r--   0        0        0     6507 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/content_item.py
--rw-r--r--   0        0        0     1227 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/content_item_xsiam.py
--rw-r--r--   0        0        0      384 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/correlation_rule.py
--rw-r--r--   0        0        0      331 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/dashboard.py
--rw-r--r--   0        0        0      363 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_definition.py
--rw-r--r--   0        0        0      704 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_field.py
--rw-r--r--   0        0        0      471 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_module.py
--rw-r--r--   0        0        0      702 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_type.py
--rw-r--r--   0        0        0      551 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/incident_field.py
--rw-r--r--   0        0        0      569 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/incident_type.py
--rw-r--r--   0        0        0      512 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/indicator_field.py
--rw-r--r--   0        0        0      697 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/indicator_type.py
--rw-r--r--   0        0        0     3100 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/integration.py
--rw-r--r--   0        0        0     1911 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/integration_script.py
--rw-r--r--   0        0        0      409 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/job.py
--rw-r--r--   0        0        0      686 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/layout.py
--rw-r--r--   0        0        0      336 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/list.py
--rw-r--r--   0        0        0      529 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/mapper.py
--rw-r--r--   0        0        0      901 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/modeling_rule.py
--rw-r--r--   0        0        0    13218 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/pack.py
--rw-r--r--   0        0        0      899 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/parsing_rule.py
--rw-r--r--   0        0        0      344 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/playbook.py
--rw-r--r--   0        0        0     1157 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/relationship.py
--rw-r--r--   0        0        0      340 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/report.py
--rw-r--r--   0        0        0     1563 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/repository.py
--rw-r--r--   0        0        0     1147 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/script.py
--rw-r--r--   0        0        0      406 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/test_playbook.py
--rw-r--r--   0        0        0      367 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/trigger.py
--rw-r--r--   0        0        0      496 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/widget.py
--rw-r--r--   0        0        0      421 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/wizard.py
--rw-r--r--   0        0        0      900 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/xdrc_template.py
--rw-r--r--   0        0        0      854 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/xsiam_dashboard.py
--rw-r--r--   0        0        0      376 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/xsiam_report.py
--rw-r--r--   0        0        0     3114 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/__init__.py
--rw-r--r--   0        0        0      718 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/base_content.py
--rw-r--r--   0        0        0     3074 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/classifier.py
--rw-r--r--   0        0        0    10399 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/content_item.py
--rw-r--r--   0        0        0     1094 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/content_items_list.py
--rw-r--r--   0        0        0      778 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/correlation_rule.py
--rw-r--r--   0        0        0     1193 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/dashboard.py
--rw-r--r--   0        0        0      680 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_definition.py
--rw-r--r--   0        0        0     1386 2023-01-08 14:17:44.312976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_field.py
--rw-r--r--   0        0        0      738 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_module.py
--rw-r--r--   0        0        0     1018 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_type.py
--rw-r--r--   0        0        0     2008 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/incident_field.py
--rw-r--r--   0        0        0     1672 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/incident_type.py
--rw-r--r--   0        0        0     1945 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/indicator_field.py
--rw-r--r--   0        0        0     2314 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/indicator_type.py
--rw-r--r--   0        0        0     4832 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/integration.py
--rw-r--r--   0        0        0      979 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/integration_script.py
--rw-r--r--   0        0        0     1248 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/job.py
--rw-r--r--   0        0        0     2360 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/json_content_item.py
--rw-r--r--   0        0        0     3138 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/layout.py
--rw-r--r--   0        0        0      729 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/list.py
--rw-r--r--   0        0        0     4684 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/mapper.py
--rw-r--r--   0        0        0      778 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/modeling_rule.py
--rw-r--r--   0        0        0     7573 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/pack.py
--rw-r--r--   0        0        0      776 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/parsing_rule.py
--rw-r--r--   0        0        0     8189 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/playbook.py
--rw-r--r--   0        0        0     1201 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/report.py
--rw-r--r--   0        0        0     2309 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/repository.py
--rw-r--r--   0        0        0     2660 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/script.py
--rw-r--r--   0        0        0     1530 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/test_playbook.py
--rw-r--r--   0        0        0     1177 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/trigger.py
--rw-r--r--   0        0        0     1101 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/widget.py
--rw-r--r--   0        0        0     1698 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/wizard.py
--rw-r--r--   0        0        0      983 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xdrc_template.py
--rw-r--r--   0        0        0      895 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xsiam_dashboard.py
--rw-r--r--   0        0        0      983 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xsiam_report.py
--rw-r--r--   0        0        0     3210 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/yaml_content_item.py
--rw-r--r--   0        0        0      428 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/common_test.py
--rw-r--r--   0        0        0    27789 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/create_content_graph_test.py
--rw-r--r--   0        0        0     2177 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/neo4j_interface_test.py
--rw-r--r--   0        0        0    59626 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/parsers_and_models_test.py
--rw-r--r--   0        0        0     2249 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/classifier.json
--rw-r--r--   0        0        0       76 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/correlation_rule.yml
--rw-r--r--   0        0        0     4803 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/dashboard.json
--rw-r--r--   0        0        0      207 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/generic_definition.json
--rw-r--r--   0        0        0    17251 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/generic_module.json
--rw-r--r--   0        0        0      289 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/generic_type.json
--rw-r--r--   0        0        0      842 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/incident_field.json
--rw-r--r--   0        0        0      474 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/incident_type.json
--rw-r--r--   0        0        0     1399 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/incoming_mapper.json
--rw-r--r--   0        0        0      621 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/indicator_field.json
--rw-r--r--   0        0        0     7920 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/indicator_type.json
--rw-r--r--   0        0        0     5499 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/layout_old.json
--rw-r--r--   0        0        0    12433 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/layoutscontainer.json
--rw-r--r--   0        0        0      806 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/list.json
--rw-r--r--   0        0        0      178 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.nodes.BaseContent.CommandOrScript.Command.csv
--rw-r--r--   0        0        0      597 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.nodes.BaseContent.Integration.csv
--rw-r--r--   0        0        0      930 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.nodes.BaseContent.Pack.csv
--rw-r--r--   0        0        0       80 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.nodes.Classifier.csv
--rw-r--r--   0        0        0       93 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.relationships.HAS_COMMAND.csv
--rw-r--r--   0        0        0       38 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.relationships.IN_PACK.csv
--rw-r--r--   0        0        0       60 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content-private.relationships.USES.csv
--rw-r--r--   0        0        0      178 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.nodes.BaseContent.CommandOrScript.Command.csv
--rw-r--r--   0        0        0      589 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.nodes.BaseContent.Integration.csv
--rw-r--r--   0        0        0      929 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.nodes.BaseContent.Pack.csv
--rw-r--r--   0        0        0      431 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.nodes.Classifier.csv
--rw-r--r--   0        0        0       93 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.relationships.HAS_COMMAND.csv
--rw-r--r--   0        0        0       38 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.relationships.IN_PACK.csv
--rw-r--r--   0        0        0       60 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/content.relationships.USES.csv
--rw-r--r--   0        0        0       96 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/modeling_rule.yml
--rw-r--r--   0        0        0     1841 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/outgoing_mapper.json
--rw-r--r--   0        0        0      774 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata.json
--rw-r--r--   0        0        0      775 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata2.json
--rw-r--r--   0        0        0     1467 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/parsing_rule.yml
--rw-r--r--   0        0        0    23137 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/report.json
--rw-r--r--   0        0        0      695 2023-01-08 14:17:44.316976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/trigger.json
--rw-r--r--   0        0        0    16961 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/unified_integration.yml
--rw-r--r--   0        0        0      824 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/widget.json
--rw-r--r--   0        0        0     3084 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/wizard.json
--rw-r--r--   0        0        0     6951 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/xsiam_dashboard.json
--rw-r--r--   0        0        0      115 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/xsiam_report.json
--rw-r--r--   0        0        0      664 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_tools.py
--rw-r--r--   0        0        0    17715 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/update_content_graph_test.py
--rw-r--r--   0        0        0     1594 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/__init__.py
--rw-r--r--   0        0        0     2785 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/convert_manager.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/__init__.py
--rw-r--r--   0        0        0     2449 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/base_converter.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/__init__.py
--rw-r--r--   0        0        0     4745 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/classifier_6_0_0_converter.py
--rw-r--r--   0        0        0     2887 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/classifier_base_converter.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/__init__.py
--rw-r--r--   0        0        0     5903 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/classifier_6_0_0_converter_test.py
--rw-r--r--   0        0        0     2340 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/classifier_base_converter_test.py
--rw-r--r--   0        0        0      841 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate.json
--rw-r--r--   0        0        0     1849 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate_5_9_9.json
--rw-r--r--   0        0        0     1241 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-mapper-incoming-Cymulate.json
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/__init__.py
--rw-r--r--   0        0        0     6443 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_6_0_0_converter.py
--rw-r--r--   0        0        0     2539 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_base_converter.py
--rw-r--r--   0        0        0     7131 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_up_to_5_9_9_converter.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/__init__.py
--rw-r--r--   0        0        0     8149 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_6_0_0_converter_test.py
--rw-r--r--   0        0        0     2159 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_base_converter_test.py
--rw-r--r--   0        0        0    10995 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_up_to_5_9_9_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/__init__.py
--rw-r--r--   0        0        0      481 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/incidenttype-ExtraHop_Detection.json
--rw-r--r--   0        0        0      485 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/incidenttype-ExtraHop_Detection_2.json
--rw-r--r--   0        0        0      917 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-close-ExtraHop_Detection.json
--rw-r--r--   0        0        0     6982 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-details-ExtraHop_Detection.json
--rw-r--r--   0        0        0     3830 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-edit-ExtraHop_Detection.json
--rw-r--r--   0        0        0    19862 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-indicatorsDetails-Cryptocurrency_Address-V3.json
--rw-r--r--   0        0        0     5567 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-mobile-ExtraHop_Detection.json
--rw-r--r--   0        0        0     6001 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-quickView-ExtraHop_Detection.json
--rw-r--r--   0        0        0    23821 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout_up_to_5_9_9_expected_convert_dir_test_file_output.json
--rw-r--r--   0        0        0    21844 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layoutscontainer-ExtraHop_Detection.json
--rw-r--r--   0        0        0      670 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/reputation-cryptocurrency.json
--rw-r--r--   0        0        0     6054 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/tests/base_converter_test.py
--rw-r--r--   0        0        0     4754 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/dir_convert_managers.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/tests/__init__.py
--rw-r--r--   0        0        0     1119 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/convert/tests/convert_manager_test.py
--rw-r--r--   0        0        0     1168 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/README.md
--rw-r--r--   0        0        0     5091 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/coverage_report.py
--rw-r--r--   0        0        0     7708 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/helpers.py
--rw-r--r--   0        0        0    10564 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/coverage_report_test.py
--rw-r--r--   0        0        0     3802 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/HealthCheckAnalyzeLargeInvestigations_py
--rw-r--r--   0        0        0      516 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage-min.json
--rw-r--r--   0        0        0    11130 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage.json
--rw-r--r--   0        0        0      767 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage.txt
--rw-r--r--   0        0        0    53248 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/HealthCheckAnalyzeLargeInvestigations
--rw-r--r--   0        0        0    53248 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/Vertica
--rw-r--r--   0        0        0    53248 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotalV3
--rw-r--r--   0        0        0    53248 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotal_V3_Premium
--rw-r--r--   0        0        0    17038 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/helpers_test.py
--rw-r--r--   0        0        0     1368 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/tools_test.py
--rw-r--r--   0        0        0     2925 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tools.py
--rw-r--r--   0        0        0     2237 2023-01-08 14:17:44.320976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/README.md
--rw-r--r--   0        0        0     3877 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/artifacts_report.py
--rw-r--r--   0        0        0    65600 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/content_artifacts_creator.py
--rw-r--r--   0        0        0    13680 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/content_artifacts_creator_test.py
--rw-r--r--   0        0        0      111 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/common_server/CommonServerPython.py
--rw-r--r--   0        0        0      111 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/common_server/CommonServerPython_modified.py
--rw-r--r--   0        0        0      660 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/id_set_alrenative_fields.json
--rw-r--r--   0        0        0     1488 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/id_set_missing_packs_and_items.json
--rw-r--r--   0        0        0      683 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/__init__.py
--rw-r--r--   0        0        0     5577 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/create_id_set.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/__init__.py
--rw-r--r--   0        0        0    19169 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/create_id_set_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/__init__.py
--rw-r--r--   0        0        0      457 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test-complex-value.json
--rw-r--r--   0        0        0      197 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test-no-types-fields.json
--rw-r--r--   0        0        0      924 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test.json
--rw-r--r--   0        0        0      274 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-to-test-no-incidenttypes.json
--rw-r--r--   0        0        0      373 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-to-test.json
--rw-r--r--   0        0        0      875 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test-no-types_scripts.json
--rw-r--r--   0        0        0     1007 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test.json
--rw-r--r--   0        0        0      431 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidenttype-to-test-no-playbook-script.json
--rw-r--r--   0        0        0      457 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidenttype-to-test.json
--rw-r--r--   0        0        0     6115 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test-no-types-fields.json
--rw-r--r--   0        0        0     6035 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test.json
--rw-r--r--   0        0        0    11992 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layoutscontainer-to-test.json
--rw-r--r--   0        0        0     9827 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/playbook-no-incident-fields.yml
--rw-r--r--   0        0        0     9861 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/playbook-with-incident-fields.yml
--rw-r--r--   0        0        0     4938 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype.json
--rw-r--r--   0        0        0     4890 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype_no_script_no_integration.json
--rw-r--r--   0        0        0      544 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/widget-no-scripts.json
--rw-r--r--   0        0        0      569 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/widget-with-scripts.json
--rw-r--r--   0        0        0     2136 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/README.md
--rw-r--r--   0        0        0    22135 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/doc_reviewer.py
--rw-r--r--   0        0        0      470 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/known_words.py
--rw-r--r--   0        0        0     8661 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/rn_checker.py
--rw-r--r--   0        0        0     1940 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/tests/conftest.py
--rw-r--r--   0        0        0    38584 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/tests/doc_reviewer_test.py
--rw-r--r--   0        0        0     3147 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/tests/rn_checker_test.py
--rw-r--r--   0        0        0     5315 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/__init__.py
--rw-r--r--   0        0        0    54065 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/downloader.py
--rw-r--r--   0        0        0      369 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/README.md
--rw-r--r--   0        0        0    47802 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/downloader_test.py
--rw-r--r--   0        0        0      442 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/automation-TestScript.yml
--rw-r--r--   0        0        0    17356 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-DummyJSIntegration.yml
--rw-r--r--   0        0        0     4947 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-Test_Integration.yml
--rw-r--r--   0        0        0     8401 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/layout-details-TestLayout.json
--rw-r--r--   0        0        0     5308 2023-01-08 14:17:44.324976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/playbook-DummyPlaybook.yml
--rw-r--r--   0        0        0       18 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/README.md
--rw-r--r--   0        0        0       96 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.py
--rw-r--r--   0        0        0      760 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml
--rw-r--r--   0        0        0       34 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_description.md
--rw-r--r--   0        0        0     3125 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png
--rw-r--r--   0        0        0       37 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_testt.py
--rw-r--r--   0        0        0    21416 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json
--rw-r--r--   0        0        0     5303 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml
--rw-r--r--   0        0        0       18 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/README.md
--rw-r--r--   0        0        0       91 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.py
--rw-r--r--   0        0        0      366 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.yml
--rw-r--r--   0        0        0      416 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/automation-TestScript.yml
--rw-r--r--   0        0        0     4947 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/integration-Test_Integration.yml
--rw-r--r--   0        0        0     8401 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/layout-details-TestLayout.json
--rw-r--r--   0        0        0     5308 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/playbook-DummyPlaybook.yml
--rw-r--r--   0        0        0       18 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/README.md
--rw-r--r--   0        0        0       96 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.py
--rw-r--r--   0        0        0      655 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml
--rw-r--r--   0        0        0       34 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_description.md
--rw-r--r--   0        0        0     3125 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png
--rw-r--r--   0        0        0       37 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_testt.py
--rw-r--r--   0        0        0    21416 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json
--rw-r--r--   0        0        0     5303 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml
--rw-r--r--   0        0        0       18 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/CHANGELOG.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/README.md
--rw-r--r--   0        0        0       91 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.py
--rw-r--r--   0        0        0      366 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.yml
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/error_code_info/__init__.py
--rw-r--r--   0        0        0     2163 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/error_code_info/error_code_info.py
--rw-r--r--   0        0        0      699 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/error_code_info/tests/error_code_info_test.py
--rw-r--r--   0        0        0      801 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/extract_outputs.py
--rw-r--r--   0        0        0     1393 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/__init__.py
--rw-r--r--   0        0        0   145506 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/find_dependencies.py
--rw-r--r--   0        0        0     1022 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/find_dependencies_command.md
--rw-r--r--   0        0        0   132576 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/tests/find_dependencies_test.py
--rw-r--r--   0        0        0     3896 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/format/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/format/__init__.py
--rw-r--r--   0        0        0     1627 2023-01-08 14:17:44.328976 demisto_sdk-1.8.3/demisto_sdk/commands/format/format_constants.py
--rw-r--r--   0        0        0    15547 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/format_module.py
--rw-r--r--   0        0        0     9643 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_generic_test.py
--rw-r--r--   0        0        0     2720 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_job_test.py
--rw-r--r--   0        0        0    67611 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_json_test.py
--rw-r--r--   0        0        0     1551 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_md_test.py
--rw-r--r--   0        0        0     5490 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_readme_test.py
--rw-r--r--   0        0        0    68194 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_yml_test.py
--rw-r--r--   0        0        0     4256 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_classifier.py
--rw-r--r--   0        0        0     2472 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_connection.py
--rw-r--r--   0        0        0     2234 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_dashboard.py
--rw-r--r--   0        0        0     3653 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_description.py
--rw-r--r--   0        0        0    19425 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic.py
--rw-r--r--   0        0        0     6455 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic_json.py
--rw-r--r--   0        0        0    15234 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic_yml.py
--rw-r--r--   0        0        0     2294 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericdefinition.py
--rw-r--r--   0        0        0     3265 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericfield.py
--rw-r--r--   0        0        0     2264 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericmodule.py
--rw-r--r--   0        0        0     2254 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generictype.py
--rw-r--r--   0        0        0     5200 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_incidentfields.py
--rw-r--r--   0        0        0     4192 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_incidenttype.py
--rw-r--r--   0        0        0     2544 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_indicatorfields.py
--rw-r--r--   0        0        0     2054 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_indicatortype.py
--rw-r--r--   0        0        0    12268 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_integration.py
--rw-r--r--   0        0        0     3026 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_job.py
--rw-r--r--   0        0        0    15796 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_layout.py
--rw-r--r--   0        0        0     2065 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_lists.py
--rw-r--r--   0        0        0     3862 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_mapper.py
--rw-r--r--   0        0        0     2828 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pack_metadata.py
--rw-r--r--   0        0        0    12621 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_playbook.py
--rw-r--r--   0        0        0     2115 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pre_process_rules.py
--rw-r--r--   0        0        0     3396 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pythonfile.py
--rw-r--r--   0        0        0     4878 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_readme.py
--rw-r--r--   0        0        0     4467 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_report.py
--rw-r--r--   0        0        0     5152 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_script.py
--rw-r--r--   0        0        0     2734 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/format/update_widget.py
--rw-r--r--   0        0        0     3190 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/__init__.py
--rw-r--r--   0        0        0    11686 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/common.py
--rw-r--r--   0        0        0      373 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/default_additional_information.json
--rw-r--r--   0        0        0    30183 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_integration_doc.py
--rw-r--r--   0        0        0    10587 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_playbook_doc.py
--rw-r--r--   0        0        0    10382 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_script_doc.py
--rw-r--r--   0        0        0    59418 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/generate_docs_test.py
--rw-r--r--   0        0        0     1704 2023-01-08 14:17:44.332976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow
--rw-r--r--   0        0        0     1263 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow_missing
--rw-r--r--   0        0        0      139 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/README.md
--rwxr-xr-x   0        0        0     6751 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/XSOARIntegration.py
--rwxr-xr-x   0        0        0     3113 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/base_code.py
--rw-r--r--   0        0        0    24367 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/code_generator.py
--rw-r--r--   0        0        0     9744 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/code_generator_test.py
--rw-r--r--   0        0        0    40767 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotal-autogen-config.json
--rw-r--r--   0        0        0     4180 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.py
--rw-r--r--   0        0        0    24386 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.yml
--rw-r--r--   0        0        0     3747 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/__init__.py
--rw-r--r--   0        0        0     5136 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/generate_integration_context.py
--rw-r--r--   0        0        0     6492 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/tests/generate_integration_context_test.py
--rw-r--r--   0        0        0       57 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_examples.txt
--rw-r--r--   0        0        0    15750 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_integration_empty_output.yml
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/__init__.py
--rw-r--r--   0        0        0    12101 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/generate_descriptions.py
--rw-r--r--   0        0        0     6507 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/generate_descriptions_test.py
--rw-r--r--   0        0        0     1931 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/ai21_response.json
--rw-r--r--   0        0        0     1127 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration.yml
--rw-r--r--   0        0        0     1125 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration_similar_paths.yml
--rw-r--r--   0        0        0      630 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/logprob_res.json
--rw-r--r--   0        0        0     3849 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_outputs.py
--rw-r--r--   0        0        0     1822 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_outputs_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/json_to_outputs/__init__.py
--rw-r--r--   0        0        0     8597 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/json_to_outputs/json_to_outputs.py
--rw-r--r--   0        0        0     8695 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/json_to_outputs/tests/json_to_outputs_test.py
--rw-r--r--   0        0        0     2543 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/__init__.py
--rw-r--r--   0        0        0    14092 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/test_playbook_generator.py
--rw-r--r--   0        0        0    10888 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/tests/test_playbook_generator_test.py
--rw-r--r--   0        0        0     4101 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/README.md
--rw-r--r--   0        0        0      604 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/common.py
--rw-r--r--   0        0        0    13848 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/generate_unit_tests.py
--rw-r--r--   0        0        0    15400 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/test_case_builder.py
--rw-r--r--   0        0        0     5852 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/test_module_builder.py
--rw-r--r--   0        0        0     3828 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/generate_unit_tests_test.py
--rw-r--r--   0        0        0      209 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/client_class_test_cases.py
--rwxr-xr-x   0        0        0      453 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/command_examples
--rw-r--r--   0        0        0    12549 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/malwarebazaar.py
--rw-r--r--   0        0        0     4061 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_all.py
--rw-r--r--   0        0        0     1525 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_specific_command.py
--rw-r--r--   0        0        0      714 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/__init__.py
--rw-r--r--   0        0        0    30914 2023-01-08 14:17:44.336976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/generate_yml.py
--rw-r--r--   0        0        0    69211 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/tests/generate_yml_from_python_test.py
--rw-r--r--   0        0        0     8897 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/yml_metadata_collector.py
--rw-r--r--   0        0        0     3478 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/__init__.py
--rw-r--r--   0        0        0    32826 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/contribution_converter.py
--rw-r--r--   0        0        0    36854 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/initiator.py
--rw-r--r--   0        0        0     5381 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.py
--rw-r--r--   0        0        0     1826 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.yml
--rw-r--r--   0        0        0      355 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_description.md
--rw-r--r--   0        0        0     2507 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_image.png
--rw-r--r--   0        0        0     1226 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_test.py
--rw-r--r--   0        0        0      238 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile
--rw-r--r--   0        0        0    11143 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile.lock
--rw-r--r--   0        0        0      297 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/command_examples
--rw-r--r--   0        0        0     1944 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript.py
--rw-r--r--   0        0        0      798 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript.yml
--rw-r--r--   0        0        0     1055 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript_test.py
--rw-r--r--   0        0        0      283 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/README.md
--rw-r--r--   0        0        0       44 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/test_data/basescript-dummy.json
--rw-r--r--   0        0        0    15312 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.py
--rw-r--r--   0        0        0     3029 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.yml
--rw-r--r--   0        0        0      133 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_description.md
--rw-r--r--   0        0        0     2507 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_image.png
--rw-r--r--   0        0        0     4784 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_test.py
--rw-r--r--   0        0        0      257 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile
--rw-r--r--   0        0        0    19972 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile.lock
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/README_example.md
--rw-r--r--   0        0        0       37 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/command_examples
--rw-r--r--   0        0        0       85 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/FeedHelloWorld_mock.txt
--rw-r--r--   0        0        0      547 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/build_iterator_results.json
--rw-r--r--   0        0        0     1392 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/get_indicators_command_results.json
--rw-r--r--   0        0        0    12224 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.py
--rw-r--r--   0        0        0     8505 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.yml
--rw-r--r--   0        0        0      109 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_description.md
--rw-r--r--   0        0        0     2507 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_image.png
--rw-r--r--   0        0        0    13322 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_test.py
--rw-r--r--   0        0        0      251 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile
--rw-r--r--   0        0        0    13560 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile.lock
--rw-r--r--   0        0        0      297 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/README.md
--rw-r--r--   0        0        0      344 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/command_examples
--rw-r--r--   0        0        0    59284 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.py
--rw-r--r--   0        0        0    20319 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.yml
--rw-r--r--   0        0        0      124 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_description.md
--rw-r--r--   0        0        0     8029 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_image.png
--rw-r--r--   0        0        0    15248 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_test.py
--rw-r--r--   0        0        0      251 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/Pipfile
--rw-r--r--   0        0        0    14864 2023-01-08 14:17:44.340976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/Pipfile.lock
--rw-r--r--   0        0        0      297 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/README.md
--rw-r--r--   0        0        0      477 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/command_examples
--rw-r--r--   0        0        0     1976 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/domain_reputation.json
--rw-r--r--   0        0        0      293 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/get_alert.json
--rw-r--r--   0        0        0     1928 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/ip_reputation.json
--rw-r--r--   0        0        0    14664 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/scan_results.json
--rw-r--r--   0        0        0      524 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/search_alerts.json
--rw-r--r--   0        0        0      110 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/update_alert_status.json
--rw-r--r--   0        0        0     2937 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.py
--rw-r--r--   0        0        0      554 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.yml
--rw-r--r--   0        0        0     1887 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript_test.py
--rw-r--r--   0        0        0     7393 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.py
--rw-r--r--   0        0        0     2912 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.yml
--rw-r--r--   0        0        0      124 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_description.md
--rw-r--r--   0        0        0     8029 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_image.png
--rw-r--r--   0        0        0     2955 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_test.py
--rw-r--r--   0        0        0      251 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile
--rw-r--r--   0        0        0    14864 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile.lock
--rw-r--r--   0        0        0      297 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/README.md
--rw-r--r--   0        0        0      162 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/command_examples
--rw-r--r--   0        0        0      293 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/test_data/get_alert.json
--rw-r--r--   0        0        0      110 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/test_data/update_alert_status.json
--rw-r--r--   0        0        0      426 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/RN/1_0_1.md
--rw-r--r--   0        0        0      504 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/RN/1_0_1_expected.md
--rw-r--r--   0        0        0      303 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/RN_ENTITY/1_0_1.md
--rw-r--r--   0        0        0      221 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/RN_ENTITY/1_0_1_expected.md
--rw-r--r--   0        0        0    39245 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/contribution_converter_test.py
--rw-r--r--   0        0        0    26253 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/initiator_test.py
--rw-r--r--   0        0        0     4980 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_and_incidentfield.zip
--rw-r--r--   0        0        0     4297 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_only.zip
--rw-r--r--   0        0        0     1168 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/__init__.py
--rw-r--r--   0        0        0    19994 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/integration_diff_detector.py
--rw-r--r--   0        0        0    24585 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/tests/integration_diff_test.py
--rw-r--r--   0        0        0     2797 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/__init__.py
--rw-r--r--   0        0        0    11104 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/commands_builder.py
--rw-r--r--   0        0        0    21054 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/helpers.py
--rw-r--r--   0        0        0    57435 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/lint_manager.py
--rw-r--r--   0        0        0    55180 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/linter.py
--rwxr-xr-x   0        0        0      546 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/installation_scripts/powershell_image.sh
--rwxr-xr-x   0        0        0      676 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/installation_scripts/python_image.sh
--rw-r--r--   0        0        0      243 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pipfile_python2/dev-requirements.txt
--rw-r--r--   0        0        0      374 2023-01-08 14:17:44.344976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile
--rw-r--r--   0        0        0    42977 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile.lock
--rw-r--r--   0        0        0    20693 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/base_checker.py
--rw-r--r--   0        0        0     8826 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/certified_partner_level_checker.py
--rw-r--r--   0        0        0     1482 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/community_level_checker.py
--rw-r--r--   0        0        0     7350 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/partner_level_checker.py
--rw-r--r--   0        0        0     9345 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/xsoar_level_checker.py
--rw-r--r--   0        0        0     8227 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/command_builder_test.py
--rw-r--r--   0        0        0      632 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/docker_helper_test.py
--rw-r--r--   0        0        0     9870 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/helper_test.py
--rw-r--r--   0        0        0    29058 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/linter_manager_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/__init__.py
--rw-r--r--   0        0        0     5476 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/conftest.py
--rw-r--r--   0        0        0     6700 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/docker_runner_test.py
--rw-r--r--   0        0        0    10530 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/gather_facts_test.py
--rw-r--r--   0        0        0    13781 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/os_runner_test.py
--rw-r--r--   0        0        0    28146 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/base_checker_test.py
--rw-r--r--   0        0        0    13515 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/certified_partner_level_checker_test.py
--rw-r--r--   0        0        0     8076 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/partner_level_checker_test.py
--rw-r--r--   0        0        0    12885 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/xsoar_level_checker_test.py
--rwxr-xr-x   0        0        0    51672 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/openapi_codegen.py
--rw-r--r--   0        0        0       91 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/resources/Generated_description.md
--rw-r--r--   0        0        0     2507 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/resources/Generated_image.png
--rwxr-xr-x   0        0        0     9784 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/tests/openapi_codegen_test.py
--rw-r--r--   0        0        0      133 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/README.md
--rw-r--r--   0        0        0    17722 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/postman_codegen.py
--rw-r--r--   0        0        0    26947 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/config-urlscanio.json
--rw-r--r--   0        0        0    17896 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/integration-urlscanio.yml
--rw-r--r--   0        0        0    21705 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/urlscan.io.postman_collection.json
--rw-r--r--   0        0        0    32356 2023-01-08 14:17:44.348976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/postman_codegen_test.py
--rw-r--r--   0        0        0    40745 2023-01-08 14:17:44.352976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal-autogen-config.json
--rw-r--r--   0        0        0   791658 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal.postman_collection.json
--rw-r--r--   0        0        0     6642 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/arguments_check_collection.json
--rw-r--r--   0        0        0     2351 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/shared_args_path.json
--rw-r--r--   0        0        0     4411 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/__init__.py
--rw-r--r--   0        0        0     4537 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/generic_module_unifier.py
--rw-r--r--   0        0        0    22505 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/integration_script_unifier.py
--rw-r--r--   0        0        0     2107 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/prepare_upload_manager.py
--rw-r--r--   0        0        0     2131 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/preparers/marketplace_suffix_preparer.py
--rw-r--r--   0        0        0     2426 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/rule_unifier.py
--rw-r--r--   0        0        0     9407 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/generic_module_unifier_test.py
--rw-r--r--   0        0        0     1312 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/xdrc_template_unifier_test.py
--rw-r--r--   0        0        0    45408 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/yml_unifier_test.py
--rw-r--r--   0        0        0      488 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/unifier.py
--rw-r--r--   0        0        0      971 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/xdrc_template_unifier.py
--rw-r--r--   0        0        0     4098 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/__init__.py
--rw-r--r--   0        0        0    12112 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/runner.py
--rw-r--r--   0        0        0     3912 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/runner_test.py
--rw-r--r--   0        0        0     1251 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component.txt
--rw-r--r--   0        0        0      944 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component_no_context.txt
--rw-r--r--   0        0        0     2882 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_playbook/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_playbook/__init__.py
--rw-r--r--   0        0        0     5599 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_playbook/playbook_runner.py
--rw-r--r--   0        0        0     2584 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/__init__.py
--rw-r--r--   0        0        0    10393 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/test_playbook_runner.py
--rw-r--r--   0        0        0    10298 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/tests/test_playbook_runner_test.py
--rw-r--r--   0        0        0     7050 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/secrets/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/secrets/__init__.py
--rw-r--r--   0        0        0    27451 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/secrets/secrets.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/secrets/tests/__init__.py
--rw-r--r--   0        0        0    15918 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/secrets/tests/secrets_test.py
--rw-r--r--   0        0        0     2960 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/__init__.py
--rw-r--r--   0        0        0     5129 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/jsonsplitter.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/tests/__init__.py
--rw-r--r--   0        0        0     1514 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/tests/jsonsplitter_test.py
--rw-r--r--   0        0        0    16476 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/tests/ymlsplitter_test.py
--rw-r--r--   0        0        0    24148 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/split/ymlsplitter.py
--rw-r--r--   0        0        0    14619 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/Docker.py
--rw-r--r--   0        0        0    12745 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/IntegrationsLock.py
--rw-r--r--   0        0        0    13388 2023-01-08 14:17:44.356976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/ParallelLoggingManager.py
--rw-r--r--   0        0        0   121785 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/TestContentClasses.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/__init__.py
--rw-r--r--   0        0        0      116 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/constants.py
--rw-r--r--   0        0        0     4899 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/execute_test_content.py
--rw-r--r--   0        0        0    27123 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/mock_server.py
--rw-r--r--   0        0        0     6269 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/init_test_data.py
--rw-r--r--   0        0        0    26859 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/test_modeling_rule.py
--rw-r--r--   0        0        0    12811 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/init_test_data_test.py
--rw-r--r--   0        0        0     6710 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_data/fake_test_data_file.json
--rw-r--r--   0        0        0    45234 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_modeling_rule_test.py
--rw-r--r--   0        0        0     5115 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/DemistoClientMock.py
--rw-r--r--   0        0        0     8056 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/ParallelLoggingManager_test.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/__init__.py
--rw-r--r--   0        0        0    19346 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/build_context_test.py
--rw-r--r--   0        0        0     3122 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/execute_test_content_test.py
--rw-r--r--   0        0        0     3912 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/integration_test.py
--rw-r--r--   0        0        0     2563 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/mock_unit_test.py
--rw-r--r--   0        0        0     5172 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/server_context_test.py
--rw-r--r--   0        0        0    39339 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/test_context_test.py
--rw-r--r--   0        0        0      587 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/test_tools.py
--rw-r--r--   0        0        0     3299 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/testplaybook_test.py
--rw-r--r--   0        0        0    12754 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/timestamp_replacer_test.py
--rw-r--r--   0        0        0    24153 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/timestamp_replacer.py
--rw-r--r--   0        0        0     3271 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tools.py
--rw-r--r--   0        0        0     1813 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/xsiam_tools/test_data.py
--rw-r--r--   0        0        0    10639 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/test_content/xsiam_tools/xsiam_client.py
--rw-r--r--   0        0        0     2959 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/__init__.py
--rw-r--r--   0        0        0     9456 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests/update_rn_manager_test.py
--rw-r--r--   0        0        0    97754 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests/update_rn_test.py
--rw-r--r--   0        0        0      329 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests_data/Packs/Test/pack_metadata.json
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests_data/Packs/release_notes/1_0_0.md
--rw-r--r--   0        0        0       60 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests_data/modeling_rules_yml_mock.yml
--rw-r--r--   0        0        0    41707 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/update_rn.py
--rw-r--r--   0        0        0    14209 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/update_rn_manager.py
--rw-r--r--   0        0        0     1677 2023-01-08 14:17:44.360976 demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/__init__.py
--rw-r--r--   0        0        0    12847 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/tests/update_xsoar_config_file_test.py
--rw-r--r--   0        0        0     6230 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/update_xsoar_config_file.py
--rw-r--r--   0        0        0     5460 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/__init__.py
--rw-r--r--   0        0        0     1135 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/data/TestPack.zip
--rw-r--r--   0        0        0     1284 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/data/content_packs.zip
--rw-r--r--   0        0        0      445 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/data/xsoar_config.json
--rw-r--r--   0        0        0    53120 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/uploader_test.py
--rw-r--r--   0        0        0     1899 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/upload.py
--rw-r--r--   0        0        0    26203 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/upload/uploader.py
--rw-r--r--   0        0        0     6112 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/validate/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/validate/__init__.py
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/validate/tests/__init__.py
--rw-r--r--   0        0        0    97792 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/validate/tests/validators_test.py
--rw-r--r--   0        0        0   107988 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/validate/validate_manager.py
--rw-r--r--   0        0        0     1087 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/README.md
--rw-r--r--   0        0        0        0 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/__init__.py
--rw-r--r--   0        0        0     8009 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/packs_zipper.py
--rw-r--r--   0        0        0     5098 2023-01-08 14:17:44.364977 demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/tests/packs_zipper_test.py
--rw-r--r--   0        0        0     5227 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_client.py
--rw-r--r--   0        0        0    10750 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier.py
--rw-r--r--   0        0        0     7185 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier_test.py
--rwxr-xr-x   0        0        0      615 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/deploy.sh
--rw-r--r--   0        0        0     5880 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/server_schema_change_slack_notifier.py
--rwxr-xr-x   0        0        0      475 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/trigger_against_content_branch.sh
--rwxr-xr-x   0        0        0      434 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/trigger_against_content_master.sh
--rw-r--r--   0        0        0     2473 2023-01-08 14:17:44.520979 demisto_sdk-1.8.3/demisto_sdk/utils/utils.py
--rw-r--r--   0        0        0     3574 2023-01-08 14:17:44.524979 demisto_sdk-1.8.3/pyproject.toml
--rw-r--r--   0        0        0    27462 1970-01-01 00:00:00.000000 demisto_sdk-1.8.3/setup.py
--rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 demisto_sdk-1.8.3/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-01-22 12:54:10.834396 demisto_sdk-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8146 2023-01-22 12:54:10.834396 demisto_sdk-1.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/__init__.py
+-rw-r--r--   0        0        0   100414 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/__init__.py
+-rw-r--r--   0        0        0     4150 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/MDXServer.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/__init__.py
+-rw-r--r--   0        0        0      878 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/configuration.py
+-rw-r--r--   0        0        0    60939 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/constants.py
+-rw-r--r--   0        0        0     5016 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/README.md
+-rw-r--r--   0        0        0      451 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/__init__.py
+-rw-r--r--   0        0        0     4670 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/content.py
+-rw-r--r--   0        0        0     3671 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/docs/CONTRIBUTION.md
+-rw-r--r--   0        0        0     3339 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/errors.py
+-rw-r--r--   0        0        0      324 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/__init__.py
+-rw-r--r--   0        0        0     2499 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/dictionary_based_object.py
+-rw-r--r--   0        0        0     3264 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/general_object.py
+-rw-r--r--   0        0        0     2195 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/json_object.py
+-rw-r--r--   0        0        0     1439 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/text_object.py
+-rw-r--r--   0        0        0     2440 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/yaml_object.py
+-rw-r--r--   0        0        0     2346 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/__init__.py
+-rw-r--r--   0        0        0     5472 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/json_content_object.py
+-rw-r--r--   0        0        0     4521 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_content_object.py
+-rw-r--r--   0        0        0     6360 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_unify_content_object.py
+-rw-r--r--   0        0        0      256 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/author_image/author_image.py
+-rw-r--r--   0        0        0      389 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/change_log/change_log.py
+-rw-r--r--   0        0        0     1969 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/classifier/classifier.py
+-rw-r--r--   0        0        0      447 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/connection/connection.py
+-rw-r--r--   0        0        0      481 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/contributors/contributors.py
+-rw-r--r--   0        0        0     2862 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/corrlation_rule/correlation_rule.py
+-rw-r--r--   0        0        0      832 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/dashboard/dashboard.py
+-rw-r--r--   0        0        0      252 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/doc_file/doc_file.py
+-rw-r--r--   0        0        0      568 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_definition/generic_definition.py
+-rw-r--r--   0        0        0      548 2023-01-22 12:54:10.838396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_field/generic_field.py
+-rw-r--r--   0        0        0      552 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_module/generic_module.py
+-rw-r--r--   0        0        0      544 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_type/generic_type.py
+-rw-r--r--   0        0        0     1495 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/incident_field/incident_field.py
+-rw-r--r--   0        0        0     1483 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/incident_type/incident_type.py
+-rw-r--r--   0        0        0     3015 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/indicator_field/indicator_field.py
+-rw-r--r--   0        0        0     2048 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/indicator_type/indicator_type.py
+-rw-r--r--   0        0        0     2260 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/integration/integration.py
+-rw-r--r--   0        0        0      967 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/job/job.py
+-rw-r--r--   0        0        0     4152 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/layout/layout.py
+-rw-r--r--   0        0        0     1109 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/lists/lists.py
+-rw-r--r--   0        0        0    10845 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/modeling_rule/modeling_rule.py
+-rw-r--r--   0        0        0    20618 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pack.py
+-rw-r--r--   0        0        0      255 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pack_ignore/pack_ignore.py
+-rw-r--r--   0        0        0    19280 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pack_metadata/pack_metadata.py
+-rw-r--r--   0        0        0     2877 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/parsing_rule/parsing_rule.py
+-rw-r--r--   0        0        0      938 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/playbook/playbook.py
+-rw-r--r--   0        0        0      925 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pre_process_rule/pre_process_rule.py
+-rw-r--r--   0        0        0     2090 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/readme/readme.py
+-rw-r--r--   0        0        0      374 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/release_note/release_note.py
+-rw-r--r--   0        0        0      387 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/release_note_config/release_note_config.py
+-rw-r--r--   0        0        0      819 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/report/report.py
+-rw-r--r--   0        0        0     1710 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/script/script.py
+-rw-r--r--   0        0        0      257 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/secret_ignore/secret_ignore.py
+-rw-r--r--   0        0        0     2847 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/tool/agent_tool.py
+-rw-r--r--   0        0        0     2800 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/trigger/trigger.py
+-rw-r--r--   0        0        0      814 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/widget/widget.py
+-rw-r--r--   0        0        0      430 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/wizard/wizard.py
+-rw-r--r--   0        0        0     3245 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xdrc_template/xdrc_template.py
+-rw-r--r--   0        0        0     3746 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard/xsiam_dashboard.py
+-rw-r--r--   0        0        0      936 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image.py
+-rw-r--r--   0        0        0     3707 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report/xsiam_report.py
+-rw-r--r--   0        0        0      930 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report_image/xsiam_report_image.py
+-rw-r--r--   0        0        0      309 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/root_objects/__init__.py
+-rw-r--r--   0        0        0      283 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/root_objects/content_descriptor/content_descriptor.py
+-rw-r--r--   0        0        0      358 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/root_objects/documentation/documentation.py
+-rw-r--r--   0        0        0     4506 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects_factory.py
+-rw-r--r--   0        0        0     1535 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/content_test.py
+-rw-r--r--   0        0        0     2119 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/json_object_test.py
+-rw-r--r--   0        0        0      696 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/text_object_test.py
+-rw-r--r--   0        0        0     2114 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/yaml_object_test.py
+-rw-r--r--   0        0        0     1773 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/json_content_object_test.py
+-rw-r--r--   0        0        0     1628 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/yaml_content_object_test.py
+-rw-r--r--   0        0        0      704 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/author_image/author_image_test.py
+-rw-r--r--   0        0        0      743 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/change_log/change_log_test.py
+-rw-r--r--   0        0        0       45 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test/classifier_mapper.json
+-rw-r--r--   0        0        0       51 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test/old_classifier.json
+-rw-r--r--   0        0        0     1611 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test.py
+-rw-r--r--   0        0        0      790 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/connection/connection_test.py
+-rw-r--r--   0        0        0     1228 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/correlation_rule/correlation_rule_test.py
+-rw-r--r--   0        0        0      732 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/dashboard/dashboard_test.py
+-rw-r--r--   0        0        0      695 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/doc_file/doc_file_test.py
+-rw-r--r--   0        0        0      778 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_field/incident_field_test.py
+-rw-r--r--   0        0        0      768 2023-01-22 12:54:10.842396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_type/incident_type_test.py
+-rw-r--r--   0        0        0      601 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_field/indicator_field_test.py
+-rw-r--r--   0        0        0       28 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test/reputations.json
+-rw-r--r--   0        0        0     1374 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample.py
+-rw-r--r--   0        0        0       17 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample.yml
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample_description.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestNotUnifiedIntegration/sample_image.png
+-rw-r--r--   0        0        0       17 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample.yml
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample_CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test/TestUnifiedIntegration/integration-sample_README.md
+-rw-r--r--   0        0        0     1834 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test.py
+-rw-r--r--   0        0        0     1717 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test/Jobs/sample-job.json
+-rw-r--r--   0        0        0      692 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test.py
+-rw-r--r--   0        0        0       43 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/layout/layout_test/layoutscontainer-Zimperium_event.json
+-rw-r--r--   0        0        0     2124 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/layout/layout_test.py
+-rw-r--r--   0        0        0      999 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/lists/lists_test.py
+-rw-r--r--   0        0        0    13581 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/modeling_rule/modeling_rule_test.py
+-rw-r--r--   0        0        0      673 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_ignore/pack_ignore_test.py
+-rw-r--r--   0        0        0    11272 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_metadata/pack_metadata_test.py
+-rw-r--r--   0        0        0     5630 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_test.py
+-rw-r--r--   0        0        0     2749 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/parsing_rule/parsing_rule_test.py
+-rw-r--r--   0        0        0      721 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/playbook/playbook_test.py
+-rw-r--r--   0        0        0     1227 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pre_process_rule/pre_process_rule_test.py
+-rw-r--r--   0        0        0     2286 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/readme/readme_test.py
+-rw-r--r--   0        0        0      723 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note/release_note_test.py
+-rw-r--r--   0        0        0     1046 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note_config/release_note_config_test.py
+-rw-r--r--   0        0        0      686 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/report/report_test.py
+-rw-r--r--   0        0        0      189 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/CHANGELOG.md
+-rw-r--r--   0        0        0     7106 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.py
+-rw-r--r--   0        0        0       15 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.yml
+-rw-r--r--   0        0        0       15 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestUnifiedScript/script-FindSimilarIncidentsByText.yml
+-rw-r--r--   0        0        0      189 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestUnifiedScript/script-FindSimilarIncidentsByText_CHANGELOG.md
+-rw-r--r--   0        0        0     1868 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test.py
+-rw-r--r--   0        0        0      694 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/secret_ignore/secret_ignore_test.py
+-rw-r--r--   0        0        0      886 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/trigger/trigger_test.py
+-rw-r--r--   0        0        0      686 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/widget/widget_test.py
+-rw-r--r--   0        0        0     3855 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test/Wizards/sample-wizard.json
+-rw-r--r--   0        0        0      743 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test.py
+-rw-r--r--   0        0        0     1255 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xdrctemplate/xdrc_template_test.py
+-rw-r--r--   0        0        0     1209 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard/xsiam_dashboard_test.py
+-rw-r--r--   0        0        0      651 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image_test.py
+-rw-r--r--   0        0        0     1107 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report/xsiam_report_test.py
+-rw-r--r--   0        0        0      608 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report_image/xsiam_report_image_test.py
+-rw-r--r--   0        0        0      448 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/root_objects/content_descriptor/content_descriptor_test.py
+-rw-r--r--   0        0        0      471 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/root_objects/documentation/documentation_test.py
+-rw-r--r--   0        0        0      474 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/content_constant_paths.py
+-rw-r--r--   0        0        0      402 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/cpu_count.py
+-rw-r--r--   0        0        0      292 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/default_additional_info.json
+-rw-r--r--   0        0        0      322 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/default_additional_info_loader.py
+-rw-r--r--   0        0        0    13750 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/default_output_descriptions.json
+-rw-r--r--   0        0        0     9522 2023-01-22 12:54:10.846396 demisto_sdk-1.9.0/demisto_sdk/commands/common/docker_helper.py
+-rw-r--r--   0        0        0   147686 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/errors.py
+-rw-r--r--   0        0        0    14200 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/git_content_config.py
+-rw-r--r--   0        0        0    31621 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/git_util.py
+-rw-r--r--   0        0        0      258 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/__init__.py
+-rw-r--r--   0        0        0      177 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/handlers_utils.py
+-rw-r--r--   0        0        0     1200 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/json/orjson_handler.py
+-rw-r--r--   0        0        0     1631 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/json/ujson_handler.py
+-rw-r--r--   0        0        0      922 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/tests/json_test.py
+-rw-r--r--   0        0        0      456 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/xsoar_handler.py
+-rw-r--r--   0        0        0     1781 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/yaml/ruamel_handler.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/__init__.py
+-rw-r--r--   0        0        0     2416 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/author_image.py
+-rw-r--r--   0        0        0    16632 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/base_validator.py
+-rw-r--r--   0        0        0     9918 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/classifier.py
+-rw-r--r--   0        0        0     8048 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/conf_json.py
+-rw-r--r--   0        0        0    23428 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/content_entity_validator.py
+-rw-r--r--   0        0        0     2734 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/correlation_rule.py
+-rw-r--r--   0        0        0     5322 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/dashboard.py
+-rw-r--r--   0        0        0    11133 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/deprecation.py
+-rw-r--r--   0        0        0    11600 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/description.py
+-rw-r--r--   0        0        0    20586 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/docker.py
+-rw-r--r--   0        0        0    19923 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/field_base_validator.py
+-rw-r--r--   0        0        0      714 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_definition.py
+-rw-r--r--   0        0        0     2876 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_field.py
+-rw-r--r--   0        0        0      698 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_module.py
+-rw-r--r--   0        0        0      690 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_type.py
+-rw-r--r--   0        0        0    39761 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/id.py
+-rw-r--r--   0        0        0     9781 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/image.py
+-rw-r--r--   0        0        0     3000 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/incident_field.py
+-rw-r--r--   0        0        0     7866 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/incident_type.py
+-rw-r--r--   0        0        0     3560 2023-01-22 12:54:10.850396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/indicator_field.py
+-rw-r--r--   0        0        0    93032 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/integration.py
+-rw-r--r--   0        0        0     4393 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/job.py
+-rw-r--r--   0        0        0    12968 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/layout.py
+-rw-r--r--   0        0        0     2565 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/lists.py
+-rw-r--r--   0        0        0     9981 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/mapper.py
+-rw-r--r--   0        0        0     7931 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/modeling_rule.py
+-rw-r--r--   0        0        0     7430 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/old_release_notes.py
+-rw-r--r--   0        0        0    45509 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/pack_unique_files.py
+-rw-r--r--   0        0        0     2290 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/parsing_rule.py
+-rw-r--r--   0        0        0    45447 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/playbook.py
+-rw-r--r--   0        0        0     6043 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/pre_process_rule.py
+-rw-r--r--   0        0        0     2087 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/python_file.py
+-rw-r--r--   0        0        0    32971 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/readme.py
+-rw-r--r--   0        0        0    20044 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/release_notes.py
+-rw-r--r--   0        0        0     1968 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/release_notes_config.py
+-rw-r--r--   0        0        0      708 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/report.py
+-rw-r--r--   0        0        0     4395 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/reputation.py
+-rw-r--r--   0        0        0    19526 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/script.py
+-rw-r--r--   0        0        0    20363 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/structure.py
+-rw-r--r--   0        0        0     3681 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/test_playbook.py
+-rw-r--r--   0        0        0     1016 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/triggers.py
+-rw-r--r--   0        0        0     1921 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/widget.py
+-rw-r--r--   0        0        0     8213 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/wizard.py
+-rw-r--r--   0        0        0     1993 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xdrc_templates.py
+-rw-r--r--   0        0        0     1996 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsiam_dashboard.py
+-rw-r--r--   0        0        0     1983 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsiam_report.py
+-rw-r--r--   0        0        0     4312 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsoar_config_json.py
+-rw-r--r--   0        0        0    16565 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/legacy_git_tools.py
+-rw-r--r--   0        0        0     5238 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/logger.py
+-rw-r--r--   0        0        0      896 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/mdx-parse-server.js
+-rw-r--r--   0        0        0      445 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/mdx-parse.js
+-rw-r--r--   0        0        0     6996 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/native_image.py
+-rw-r--r--   0        0        0      482 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/canvas-context-connections.yml
+-rw-r--r--   0        0        0      961 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/classifier.yml
+-rw-r--r--   0        0        0      741 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/classifier_5_9_9.yml
+-rw-r--r--   0        0        0     1103 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/dashboard.yml
+-rw-r--r--   0        0        0      357 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/genericdefinition.yml
+-rw-r--r--   0        0        0     1527 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/genericfield.yml
+-rw-r--r--   0        0        0     1193 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/genericmodule.yml
+-rw-r--r--   0        0        0     1156 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/generictype.yml
+-rw-r--r--   0        0        0     2073 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidentfield.yml
+-rw-r--r--   0        0        0     1957 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidentfields.yml
+-rw-r--r--   0        0        0     1169 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidenttype.yml
+-rw-r--r--   0        0        0     1377 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/indicatorfield.yml
+-rw-r--r--   0        0        0     4771 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/integration.yml
+-rw-r--r--   0        0        0     4455 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/job.yml
+-rw-r--r--   0        0        0     1569 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/layout.yml
+-rw-r--r--   0        0        0     3504 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/layoutscontainer.yml
+-rw-r--r--   0        0        0     1073 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/list.yml
+-rw-r--r--   0        0        0      617 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/mapper.yml
+-rw-r--r--   0        0        0     8150 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/playbook.yml
+-rw-r--r--   0        0        0     1434 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/pre-process-rules.yml
+-rw-r--r--   0        0        0      131 2023-01-22 12:54:10.854396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/releasenotesconfig.yml
+-rw-r--r--   0        0        0     3356 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/report.yml
+-rw-r--r--   0        0        0     1144 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/reputation.yml
+-rw-r--r--   0        0        0     2822 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/script.yml
+-rw-r--r--   0        0        0      637 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/widget.yml
+-rw-r--r--   0        0        0     2059 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/wizard.yml
+-rw-r--r--   0        0        0     4251 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/xsoar_config.json
+-rw-r--r--   0        0        0      203 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/singleton.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/__init__.py
+-rw-r--r--   0        0        0     3305 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/author_image_validator_test.py
+-rw-r--r--   0        0        0    23120 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/base_validator_test.py
+-rw-r--r--   0        0        0     4801 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/classifier_test.py
+-rw-r--r--   0        0        0     8959 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/conf_test.py
+-rw-r--r--   0        0        0    11318 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/content_entity_validator_test.py
+-rw-r--r--   0        0        0     1203 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/correlation_rules_test.py
+-rw-r--r--   0        0        0      457 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/cpu_count_test.py
+-rw-r--r--   0        0        0     3578 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/dashboard_test.py
+-rw-r--r--   0        0        0    42912 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/dependencies_test.py
+-rw-r--r--   0        0        0    17068 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/deprecation_test.py
+-rw-r--r--   0        0        0     6648 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/description_test.py
+-rw-r--r--   0        0        0    27939 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/docker_test.py
+-rw-r--r--   0        0        0     8580 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/errors_test.py
+-rw-r--r--   0        0        0    23020 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/field_validator_test.py
+-rw-r--r--   0        0        0     2233 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/generic_field_test.py
+-rw-r--r--   0        0        0    13122 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/git_config_test.py
+-rw-r--r--   0        0        0     1734 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/git_util_test.py
+-rw-r--r--   0        0        0    61328 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/id_test.py
+-rw-r--r--   0        0        0     7473 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/image_test.py
+-rw-r--r--   0        0        0     1862 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/incident_field_test.py
+-rw-r--r--   0        0        0     8373 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/incident_type_test.py
+-rw-r--r--   0        0        0     4004 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/indicator_field_test.py
+-rw-r--r--   0        0        0    91854 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/integration_test.py
+-rw-r--r--   0        0        0     4590 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/layout_test.py
+-rw-r--r--   0        0        0     6851 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/legacy_git_tools_test.py
+-rw-r--r--   0        0        0     2358 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/lists_test.py
+-rw-r--r--   0        0        0     3142 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/mapper_test.py
+-rw-r--r--   0        0        0     7370 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/modeling_rules_test.py
+-rw-r--r--   0        0        0     4311 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/native_image_test.py
+-rw-r--r--   0        0        0     4391 2023-01-22 12:54:10.858396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/old_release_notes_test.py
+-rw-r--r--   0        0        0    18689 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pack_metadata_validator_test.py
+-rw-r--r--   0        0        0    47639 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pack_unique_files_test.py
+-rw-r--r--   0        0        0    31317 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/playbook_test.py
+-rw-r--r--   0        0        0      657 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pre_process_rule_test.py
+-rw-r--r--   0        0        0      767 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/python_file_test.py
+-rw-r--r--   0        0        0    25149 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/readme_test.py
+-rw-r--r--   0        0        0     2021 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/release_notes_config_test.py
+-rw-r--r--   0        0        0    28451 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/release_notes_test.py
+-rw-r--r--   0        0        0     2599 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/reputation_test.py
+-rw-r--r--   0        0        0    21395 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/script_test.py
+-rw-r--r--   0        0        0    24431 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/structure_test.py
+-rw-r--r--   0        0        0      880 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/invalid_correlation_rule.yml
+-rw-r--r--   0        0        0     1195 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/rn_header_test_data
+-rw-r--r--   0        0        0    79543 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/test_changelog.md
+-rw-r--r--   0        0        0     1842 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/timers_test.py
+-rw-r--r--   0        0        0    77885 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/tools_test.py
+-rw-r--r--   0        0        0   137669 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/update_id_set_test.py
+-rw-r--r--   0        0        0     1521 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/widget_test.py
+-rw-r--r--   0        0        0     6753 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/wizards_test.py
+-rw-r--r--   0        0        0     8057 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/xsoar_config_file_test.py
+-rw-r--r--   0        0        0     7562 2023-01-22 12:54:10.862396 demisto_sdk-1.9.0/demisto_sdk/commands/common/timers.py
+-rw-r--r--   0        0        0   111928 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/common/tools.py
+-rwxr-xr-x   0        0        0   133258 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/common/update_id_set.py
+-rw-r--r--   0        0        0     2558 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/__init__.py
+-rw-r--r--   0        0        0    20437 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/common.py
+-rw-r--r--   0        0        0     3019 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/content_graph_builder.py
+-rw-r--r--   0        0        0     4299 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/content_graph_commands.py
+-rw-r--r--   0        0        0   292334 2023-01-22 12:54:10.866396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/architecture.png
+-rw-r--r--   0        0        0   244414 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/models.png
+-rw-r--r--   0        0        0   236398 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/parsers.png
+-rw-r--r--   0        0        0     4695 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/graph.py
+-rw-r--r--   0        0        0     3719 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/import_utils.py
+-rw-r--r--   0        0        0    15554 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/neo4j_graph.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/__init__.py
+-rw-r--r--   0        0        0     1943 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/common.py
+-rw-r--r--   0        0        0     2253 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/constraints.py
+-rw-r--r--   0        0        0    11314 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/dependencies.py
+-rw-r--r--   0        0        0     3604 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/import_export.py
+-rw-r--r--   0        0        0     1692 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/indexes.py
+-rw-r--r--   0        0        0     4999 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/nodes.py
+-rw-r--r--   0        0        0     7829 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/relationships.py
+-rw-r--r--   0        0        0     5232 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/neo4j_service.py
+-rw-r--r--   0        0        0     2904 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/__init__.py
+-rw-r--r--   0        0        0     6605 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/base_content.py
+-rw-r--r--   0        0        0      474 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/classifier.py
+-rw-r--r--   0        0        0     6608 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/content_item.py
+-rw-r--r--   0        0        0     1227 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/content_item_xsiam.py
+-rw-r--r--   0        0        0      384 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/correlation_rule.py
+-rw-r--r--   0        0        0      331 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/dashboard.py
+-rw-r--r--   0        0        0      363 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_definition.py
+-rw-r--r--   0        0        0      704 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_field.py
+-rw-r--r--   0        0        0      471 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_module.py
+-rw-r--r--   0        0        0      702 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_type.py
+-rw-r--r--   0        0        0      551 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/incident_field.py
+-rw-r--r--   0        0        0      569 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/incident_type.py
+-rw-r--r--   0        0        0      512 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/indicator_field.py
+-rw-r--r--   0        0        0      697 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/indicator_type.py
+-rw-r--r--   0        0        0     3100 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/integration.py
+-rw-r--r--   0        0        0     1911 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/integration_script.py
+-rw-r--r--   0        0        0      409 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/job.py
+-rw-r--r--   0        0        0     1072 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/layout.py
+-rw-r--r--   0        0        0      336 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/list.py
+-rw-r--r--   0        0        0      529 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/mapper.py
+-rw-r--r--   0        0        0      901 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/modeling_rule.py
+-rw-r--r--   0        0        0    13407 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/pack.py
+-rw-r--r--   0        0        0      899 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/parsing_rule.py
+-rw-r--r--   0        0        0      344 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/playbook.py
+-rw-r--r--   0        0        0     1225 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/relationship.py
+-rw-r--r--   0        0        0      340 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/report.py
+-rw-r--r--   0        0        0     1563 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/repository.py
+-rw-r--r--   0        0        0     1475 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/script.py
+-rw-r--r--   0        0        0      406 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/test_playbook.py
+-rw-r--r--   0        0        0      367 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/trigger.py
+-rw-r--r--   0        0        0      496 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/widget.py
+-rw-r--r--   0        0        0      421 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/wizard.py
+-rw-r--r--   0        0        0      900 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/xdrc_template.py
+-rw-r--r--   0        0        0      854 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/xsiam_dashboard.py
+-rw-r--r--   0        0        0      376 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/xsiam_report.py
+-rw-r--r--   0        0        0     3114 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/__init__.py
+-rw-r--r--   0        0        0      718 2023-01-22 12:54:10.870396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/base_content.py
+-rw-r--r--   0        0        0     3074 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/classifier.py
+-rw-r--r--   0        0        0    10399 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/content_item.py
+-rw-r--r--   0        0        0     1094 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/content_items_list.py
+-rw-r--r--   0        0        0      778 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/correlation_rule.py
+-rw-r--r--   0        0        0     1193 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/dashboard.py
+-rw-r--r--   0        0        0      680 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_definition.py
+-rw-r--r--   0        0        0     1386 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_field.py
+-rw-r--r--   0        0        0      738 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_module.py
+-rw-r--r--   0        0        0     1018 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_type.py
+-rw-r--r--   0        0        0     2008 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/incident_field.py
+-rw-r--r--   0        0        0     1672 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/incident_type.py
+-rw-r--r--   0        0        0     1945 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/indicator_field.py
+-rw-r--r--   0        0        0     2314 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/indicator_type.py
+-rw-r--r--   0        0        0     4832 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/integration.py
+-rw-r--r--   0        0        0      979 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/integration_script.py
+-rw-r--r--   0        0        0     1248 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/job.py
+-rw-r--r--   0        0        0     2360 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/json_content_item.py
+-rw-r--r--   0        0        0     3138 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/layout.py
+-rw-r--r--   0        0        0      729 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/list.py
+-rw-r--r--   0        0        0     4684 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/mapper.py
+-rw-r--r--   0        0        0      778 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/modeling_rule.py
+-rw-r--r--   0        0        0     7573 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/pack.py
+-rw-r--r--   0        0        0      776 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/parsing_rule.py
+-rw-r--r--   0        0        0     8189 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/playbook.py
+-rw-r--r--   0        0        0     1201 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/report.py
+-rw-r--r--   0        0        0     2309 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/repository.py
+-rw-r--r--   0        0        0     2660 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/script.py
+-rw-r--r--   0        0        0     1530 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/test_playbook.py
+-rw-r--r--   0        0        0     1177 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/trigger.py
+-rw-r--r--   0        0        0     1101 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/widget.py
+-rw-r--r--   0        0        0     1698 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/wizard.py
+-rw-r--r--   0        0        0      983 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xdrc_template.py
+-rw-r--r--   0        0        0      895 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xsiam_dashboard.py
+-rw-r--r--   0        0        0      983 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xsiam_report.py
+-rw-r--r--   0        0        0     3210 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/yaml_content_item.py
+-rw-r--r--   0        0        0      428 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/common_test.py
+-rw-r--r--   0        0        0    28445 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/create_content_graph_test.py
+-rw-r--r--   0        0        0     2177 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/neo4j_interface_test.py
+-rw-r--r--   0        0        0    59626 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/parsers_and_models_test.py
+-rw-r--r--   0        0        0     2249 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/classifier.json
+-rw-r--r--   0        0        0       76 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/correlation_rule.yml
+-rw-r--r--   0        0        0     4803 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/dashboard.json
+-rw-r--r--   0        0        0      207 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/generic_definition.json
+-rw-r--r--   0        0        0    17251 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/generic_module.json
+-rw-r--r--   0        0        0      289 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/generic_type.json
+-rw-r--r--   0        0        0      842 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/incident_field.json
+-rw-r--r--   0        0        0      474 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/incident_type.json
+-rw-r--r--   0        0        0     1399 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/incoming_mapper.json
+-rw-r--r--   0        0        0      621 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/indicator_field.json
+-rw-r--r--   0        0        0     7920 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/indicator_type.json
+-rw-r--r--   0        0        0     5499 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/layout_old.json
+-rw-r--r--   0        0        0    12433 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/layoutscontainer.json
+-rw-r--r--   0        0        0      806 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/list.json
+-rw-r--r--   0        0        0     5834 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/mock_import_files_multiple_repos__valid/valid_graph.zip
+-rw-r--r--   0        0        0       96 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/modeling_rule.yml
+-rw-r--r--   0        0        0     1841 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/outgoing_mapper.json
+-rw-r--r--   0        0        0      774 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata.json
+-rw-r--r--   0        0        0      775 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata2.json
+-rw-r--r--   0        0        0     1467 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/parsing_rule.yml
+-rw-r--r--   0        0        0    23137 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/report.json
+-rw-r--r--   0        0        0      695 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/trigger.json
+-rw-r--r--   0        0        0    16961 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/unified_integration.yml
+-rw-r--r--   0        0        0      824 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/widget.json
+-rw-r--r--   0        0        0     3084 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/wizard.json
+-rw-r--r--   0        0        0     6951 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/xsiam_dashboard.json
+-rw-r--r--   0        0        0      115 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/xsiam_report.json
+-rw-r--r--   0        0        0      664 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_tools.py
+-rw-r--r--   0        0        0    17585 2023-01-22 12:54:10.874396 demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/update_content_graph_test.py
+-rw-r--r--   0        0        0     1594 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/__init__.py
+-rw-r--r--   0        0        0     2785 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/convert_manager.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/__init__.py
+-rw-r--r--   0        0        0     2449 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/base_converter.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/__init__.py
+-rw-r--r--   0        0        0     4745 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/classifier_6_0_0_converter.py
+-rw-r--r--   0        0        0     2887 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/classifier_base_converter.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/__init__.py
+-rw-r--r--   0        0        0     5903 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/classifier_6_0_0_converter_test.py
+-rw-r--r--   0        0        0     2340 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/classifier_base_converter_test.py
+-rw-r--r--   0        0        0      841 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate.json
+-rw-r--r--   0        0        0     1849 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate_5_9_9.json
+-rw-r--r--   0        0        0     1241 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-mapper-incoming-Cymulate.json
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/__init__.py
+-rw-r--r--   0        0        0     6443 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_6_0_0_converter.py
+-rw-r--r--   0        0        0     2539 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_base_converter.py
+-rw-r--r--   0        0        0     7131 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_up_to_5_9_9_converter.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/__init__.py
+-rw-r--r--   0        0        0     8149 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_6_0_0_converter_test.py
+-rw-r--r--   0        0        0     2159 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_base_converter_test.py
+-rw-r--r--   0        0        0    10995 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_up_to_5_9_9_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      481 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/incidenttype-ExtraHop_Detection.json
+-rw-r--r--   0        0        0      485 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/incidenttype-ExtraHop_Detection_2.json
+-rw-r--r--   0        0        0      917 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-close-ExtraHop_Detection.json
+-rw-r--r--   0        0        0     6982 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-details-ExtraHop_Detection.json
+-rw-r--r--   0        0        0     3830 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-edit-ExtraHop_Detection.json
+-rw-r--r--   0        0        0    19862 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-indicatorsDetails-Cryptocurrency_Address-V3.json
+-rw-r--r--   0        0        0     5567 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-mobile-ExtraHop_Detection.json
+-rw-r--r--   0        0        0     6001 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-quickView-ExtraHop_Detection.json
+-rw-r--r--   0        0        0    23821 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout_up_to_5_9_9_expected_convert_dir_test_file_output.json
+-rw-r--r--   0        0        0    21844 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layoutscontainer-ExtraHop_Detection.json
+-rw-r--r--   0        0        0      670 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/reputation-cryptocurrency.json
+-rw-r--r--   0        0        0     6054 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/tests/base_converter_test.py
+-rw-r--r--   0        0        0     4754 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/dir_convert_managers.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/tests/__init__.py
+-rw-r--r--   0        0        0     1119 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/convert/tests/convert_manager_test.py
+-rw-r--r--   0        0        0     1168 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/README.md
+-rw-r--r--   0        0        0     5091 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/coverage_report.py
+-rw-r--r--   0        0        0     7708 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/helpers.py
+-rw-r--r--   0        0        0    10564 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/coverage_report_test.py
+-rw-r--r--   0        0        0     3802 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/HealthCheckAnalyzeLargeInvestigations_py
+-rw-r--r--   0        0        0      516 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage-min.json
+-rw-r--r--   0        0        0    11130 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage.json
+-rw-r--r--   0        0        0      767 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage.txt
+-rw-r--r--   0        0        0    53248 2023-01-22 12:54:10.878396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/HealthCheckAnalyzeLargeInvestigations
+-rw-r--r--   0        0        0    53248 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/Vertica
+-rw-r--r--   0        0        0    53248 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotalV3
+-rw-r--r--   0        0        0    53248 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotal_V3_Premium
+-rw-r--r--   0        0        0    17038 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/helpers_test.py
+-rw-r--r--   0        0        0     1368 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/tools_test.py
+-rw-r--r--   0        0        0     2925 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tools.py
+-rw-r--r--   0        0        0     2237 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/README.md
+-rw-r--r--   0        0        0     3877 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/artifacts_report.py
+-rw-r--r--   0        0        0    65600 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/content_artifacts_creator.py
+-rw-r--r--   0        0        0    13490 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/content_artifacts_creator_test.py
+-rw-r--r--   0        0        0      111 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/common_server/CommonServerPython.py
+-rw-r--r--   0        0        0      111 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/common_server/CommonServerPython_modified.py
+-rw-r--r--   0        0        0      660 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/id_set_alrenative_fields.json
+-rw-r--r--   0        0        0     1488 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/id_set_missing_packs_and_items.json
+-rw-r--r--   0        0        0      683 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/__init__.py
+-rw-r--r--   0        0        0     5577 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/create_id_set.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/__init__.py
+-rw-r--r--   0        0        0    19169 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/create_id_set_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/__init__.py
+-rw-r--r--   0        0        0      457 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test-complex-value.json
+-rw-r--r--   0        0        0      197 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test-no-types-fields.json
+-rw-r--r--   0        0        0      924 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test.json
+-rw-r--r--   0        0        0      274 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-to-test-no-incidenttypes.json
+-rw-r--r--   0        0        0      373 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-to-test.json
+-rw-r--r--   0        0        0      875 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test-no-types_scripts.json
+-rw-r--r--   0        0        0     1007 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test.json
+-rw-r--r--   0        0        0      431 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidenttype-to-test-no-playbook-script.json
+-rw-r--r--   0        0        0      457 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidenttype-to-test.json
+-rw-r--r--   0        0        0     6115 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test-no-types-fields.json
+-rw-r--r--   0        0        0     6035 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test.json
+-rw-r--r--   0        0        0    11992 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layoutscontainer-to-test.json
+-rw-r--r--   0        0        0     9827 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/playbook-no-incident-fields.yml
+-rw-r--r--   0        0        0     9861 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/playbook-with-incident-fields.yml
+-rw-r--r--   0        0        0     4938 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype.json
+-rw-r--r--   0        0        0     4890 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype_no_script_no_integration.json
+-rw-r--r--   0        0        0      544 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/widget-no-scripts.json
+-rw-r--r--   0        0        0      569 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/widget-with-scripts.json
+-rw-r--r--   0        0        0     2136 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/README.md
+-rw-r--r--   0        0        0    22618 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/doc_reviewer.py
+-rw-r--r--   0        0        0      470 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/known_words.py
+-rw-r--r--   0        0        0     8661 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/rn_checker.py
+-rw-r--r--   0        0        0     7028 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/tests/conftest.py
+-rw-r--r--   0        0        0    44918 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/tests/doc_reviewer_test.py
+-rw-r--r--   0        0        0     3147 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/tests/rn_checker_test.py
+-rw-r--r--   0        0        0     5315 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/download/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/download/__init__.py
+-rw-r--r--   0        0        0    54065 2023-01-22 12:54:10.882396 demisto_sdk-1.9.0/demisto_sdk/commands/download/downloader.py
+-rw-r--r--   0        0        0      369 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/README.md
+-rw-r--r--   0        0        0    47802 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/downloader_test.py
+-rw-r--r--   0        0        0      442 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/automation-TestScript.yml
+-rw-r--r--   0        0        0    17356 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-DummyJSIntegration.yml
+-rw-r--r--   0        0        0     4947 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-Test_Integration.yml
+-rw-r--r--   0        0        0     8401 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/layout-details-TestLayout.json
+-rw-r--r--   0        0        0     5308 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/playbook-DummyPlaybook.yml
+-rw-r--r--   0        0        0       18 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/README.md
+-rw-r--r--   0        0        0       96 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.py
+-rw-r--r--   0        0        0      760 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml
+-rw-r--r--   0        0        0       34 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_description.md
+-rw-r--r--   0        0        0     3125 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png
+-rw-r--r--   0        0        0       37 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_testt.py
+-rw-r--r--   0        0        0    21416 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json
+-rw-r--r--   0        0        0     5303 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml
+-rw-r--r--   0        0        0       18 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/README.md
+-rw-r--r--   0        0        0       91 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.py
+-rw-r--r--   0        0        0      366 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.yml
+-rw-r--r--   0        0        0      416 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/automation-TestScript.yml
+-rw-r--r--   0        0        0     4947 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/integration-Test_Integration.yml
+-rw-r--r--   0        0        0     8401 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/layout-details-TestLayout.json
+-rw-r--r--   0        0        0     5308 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/playbook-DummyPlaybook.yml
+-rw-r--r--   0        0        0       18 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/README.md
+-rw-r--r--   0        0        0       96 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.py
+-rw-r--r--   0        0        0      655 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml
+-rw-r--r--   0        0        0       34 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_description.md
+-rw-r--r--   0        0        0     3125 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png
+-rw-r--r--   0        0        0       37 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_testt.py
+-rw-r--r--   0        0        0    21416 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json
+-rw-r--r--   0        0        0     5303 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml
+-rw-r--r--   0        0        0       18 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/README.md
+-rw-r--r--   0        0        0       91 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.py
+-rw-r--r--   0        0        0      366 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Scripts/TestScript/TestScript.yml
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/error_code_info/__init__.py
+-rw-r--r--   0        0        0     2163 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/error_code_info/error_code_info.py
+-rw-r--r--   0        0        0      699 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/error_code_info/tests/error_code_info_test.py
+-rw-r--r--   0        0        0      801 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/extract_outputs.py
+-rw-r--r--   0        0        0     1393 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/__init__.py
+-rw-r--r--   0        0        0   145506 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/find_dependencies.py
+-rw-r--r--   0        0        0     1022 2023-01-22 12:54:10.886396 demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/find_dependencies_command.md
+-rw-r--r--   0        0        0   132576 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/tests/find_dependencies_test.py
+-rw-r--r--   0        0        0     3896 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/__init__.py
+-rw-r--r--   0        0        0     1627 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/format_constants.py
+-rw-r--r--   0        0        0    15547 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/format_module.py
+-rw-r--r--   0        0        0     9643 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_generic_test.py
+-rw-r--r--   0        0        0     2720 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_job_test.py
+-rw-r--r--   0        0        0    67611 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_json_test.py
+-rw-r--r--   0        0        0     1551 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_md_test.py
+-rw-r--r--   0        0        0     5490 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_readme_test.py
+-rw-r--r--   0        0        0    68194 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_yml_test.py
+-rw-r--r--   0        0        0     4256 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_classifier.py
+-rw-r--r--   0        0        0     2472 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_connection.py
+-rw-r--r--   0        0        0     2234 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_dashboard.py
+-rw-r--r--   0        0        0     3653 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_description.py
+-rw-r--r--   0        0        0    19425 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic.py
+-rw-r--r--   0        0        0     6455 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic_json.py
+-rw-r--r--   0        0        0    15234 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic_yml.py
+-rw-r--r--   0        0        0     2294 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericdefinition.py
+-rw-r--r--   0        0        0     3265 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericfield.py
+-rw-r--r--   0        0        0     2264 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericmodule.py
+-rw-r--r--   0        0        0     2254 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generictype.py
+-rw-r--r--   0        0        0     5200 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_incidentfields.py
+-rw-r--r--   0        0        0     4192 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_incidenttype.py
+-rw-r--r--   0        0        0     2544 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_indicatorfields.py
+-rw-r--r--   0        0        0     2054 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_indicatortype.py
+-rw-r--r--   0        0        0    12268 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_integration.py
+-rw-r--r--   0        0        0     3026 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_job.py
+-rw-r--r--   0        0        0    15796 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_layout.py
+-rw-r--r--   0        0        0     2065 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_lists.py
+-rw-r--r--   0        0        0     3862 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_mapper.py
+-rw-r--r--   0        0        0     2828 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pack_metadata.py
+-rw-r--r--   0        0        0    12621 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_playbook.py
+-rw-r--r--   0        0        0     2115 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pre_process_rules.py
+-rw-r--r--   0        0        0     3396 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pythonfile.py
+-rw-r--r--   0        0        0     4878 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_readme.py
+-rw-r--r--   0        0        0     4467 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_report.py
+-rw-r--r--   0        0        0     5152 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_script.py
+-rw-r--r--   0        0        0     2734 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/format/update_widget.py
+-rw-r--r--   0        0        0     3190 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/__init__.py
+-rw-r--r--   0        0        0    11686 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/common.py
+-rw-r--r--   0        0        0      373 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/default_additional_information.json
+-rw-r--r--   0        0        0    30183 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_integration_doc.py
+-rw-r--r--   0        0        0    10587 2023-01-22 12:54:10.890396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_playbook_doc.py
+-rw-r--r--   0        0        0    10382 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_script_doc.py
+-rw-r--r--   0        0        0    59418 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/generate_docs_test.py
+-rw-r--r--   0        0        0     1704 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow
+-rw-r--r--   0        0        0     1263 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow_missing
+-rw-r--r--   0        0        0      139 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/README.md
+-rwxr-xr-x   0        0        0     6751 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/XSOARIntegration.py
+-rwxr-xr-x   0        0        0     3113 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/base_code.py
+-rw-r--r--   0        0        0    24367 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/code_generator.py
+-rw-r--r--   0        0        0     9744 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/code_generator_test.py
+-rw-r--r--   0        0        0    40767 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotal-autogen-config.json
+-rw-r--r--   0        0        0     4180 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.py
+-rw-r--r--   0        0        0    24386 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.yml
+-rw-r--r--   0        0        0     3747 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/__init__.py
+-rw-r--r--   0        0        0     5136 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/generate_integration_context.py
+-rw-r--r--   0        0        0     6492 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/tests/generate_integration_context_test.py
+-rw-r--r--   0        0        0       57 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_examples.txt
+-rw-r--r--   0        0        0    15750 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_integration_empty_output.yml
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/__init__.py
+-rw-r--r--   0        0        0    12101 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/generate_descriptions.py
+-rw-r--r--   0        0        0     6507 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/generate_descriptions_test.py
+-rw-r--r--   0        0        0     1931 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/ai21_response.json
+-rw-r--r--   0        0        0     1127 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration.yml
+-rw-r--r--   0        0        0     1125 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration_similar_paths.yml
+-rw-r--r--   0        0        0      630 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/logprob_res.json
+-rw-r--r--   0        0        0     3849 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_outputs.py
+-rw-r--r--   0        0        0     1822 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_outputs_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/json_to_outputs/__init__.py
+-rw-r--r--   0        0        0     8597 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/json_to_outputs/json_to_outputs.py
+-rw-r--r--   0        0        0     8695 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/json_to_outputs/tests/json_to_outputs_test.py
+-rw-r--r--   0        0        0     2543 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/__init__.py
+-rw-r--r--   0        0        0    14092 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/test_playbook_generator.py
+-rw-r--r--   0        0        0    10888 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/tests/test_playbook_generator_test.py
+-rw-r--r--   0        0        0     4101 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/README.md
+-rw-r--r--   0        0        0      604 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/common.py
+-rw-r--r--   0        0        0    13848 2023-01-22 12:54:10.894396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/generate_unit_tests.py
+-rw-r--r--   0        0        0    15400 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/test_case_builder.py
+-rw-r--r--   0        0        0     5852 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/test_module_builder.py
+-rw-r--r--   0        0        0     3828 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/generate_unit_tests_test.py
+-rw-r--r--   0        0        0      209 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/client_class_test_cases.py
+-rwxr-xr-x   0        0        0      453 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/command_examples
+-rw-r--r--   0        0        0    12549 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/malwarebazaar.py
+-rw-r--r--   0        0        0     4061 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_all.py
+-rw-r--r--   0        0        0     1525 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_specific_command.py
+-rw-r--r--   0        0        0      714 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/__init__.py
+-rw-r--r--   0        0        0    30914 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/generate_yml.py
+-rw-r--r--   0        0        0    69211 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/tests/generate_yml_from_python_test.py
+-rw-r--r--   0        0        0     8897 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/yml_metadata_collector.py
+-rw-r--r--   0        0        0     3478 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/__init__.py
+-rw-r--r--   0        0        0    32826 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/contribution_converter.py
+-rw-r--r--   0        0        0    36854 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/initiator.py
+-rw-r--r--   0        0        0     5381 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.py
+-rw-r--r--   0        0        0     1826 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.yml
+-rw-r--r--   0        0        0      355 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_description.md
+-rw-r--r--   0        0        0     2507 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_image.png
+-rw-r--r--   0        0        0     1226 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_test.py
+-rw-r--r--   0        0        0      238 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile
+-rw-r--r--   0        0        0    11143 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile.lock
+-rw-r--r--   0        0        0      297 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/command_examples
+-rw-r--r--   0        0        0     1944 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript.py
+-rw-r--r--   0        0        0      798 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript.yml
+-rw-r--r--   0        0        0     1055 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript_test.py
+-rw-r--r--   0        0        0      283 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/README.md
+-rw-r--r--   0        0        0       44 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/test_data/basescript-dummy.json
+-rw-r--r--   0        0        0    15312 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.py
+-rw-r--r--   0        0        0     3029 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.yml
+-rw-r--r--   0        0        0      133 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_description.md
+-rw-r--r--   0        0        0     2507 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_image.png
+-rw-r--r--   0        0        0     4784 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_test.py
+-rw-r--r--   0        0        0      257 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile
+-rw-r--r--   0        0        0    19972 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile.lock
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/README_example.md
+-rw-r--r--   0        0        0       37 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/command_examples
+-rw-r--r--   0        0        0       85 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/FeedHelloWorld_mock.txt
+-rw-r--r--   0        0        0      547 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/build_iterator_results.json
+-rw-r--r--   0        0        0     1392 2023-01-22 12:54:10.898396 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/get_indicators_command_results.json
+-rw-r--r--   0        0        0    12224 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.py
+-rw-r--r--   0        0        0     8505 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.yml
+-rw-r--r--   0        0        0      109 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_description.md
+-rw-r--r--   0        0        0     2507 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_image.png
+-rw-r--r--   0        0        0    13322 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_test.py
+-rw-r--r--   0        0        0      251 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile
+-rw-r--r--   0        0        0    13560 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile.lock
+-rw-r--r--   0        0        0      297 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/README.md
+-rw-r--r--   0        0        0      344 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/command_examples
+-rw-r--r--   0        0        0    59284 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.py
+-rw-r--r--   0        0        0    20319 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.yml
+-rw-r--r--   0        0        0      124 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_description.md
+-rw-r--r--   0        0        0     8029 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_image.png
+-rw-r--r--   0        0        0    15248 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_test.py
+-rw-r--r--   0        0        0      251 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/Pipfile
+-rw-r--r--   0        0        0    14864 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/Pipfile.lock
+-rw-r--r--   0        0        0      297 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/README.md
+-rw-r--r--   0        0        0      477 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/command_examples
+-rw-r--r--   0        0        0     1976 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/domain_reputation.json
+-rw-r--r--   0        0        0      293 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/get_alert.json
+-rw-r--r--   0        0        0     1928 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/ip_reputation.json
+-rw-r--r--   0        0        0    14664 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/scan_results.json
+-rw-r--r--   0        0        0      524 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/search_alerts.json
+-rw-r--r--   0        0        0      110 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/update_alert_status.json
+-rw-r--r--   0        0        0     2937 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.py
+-rw-r--r--   0        0        0      554 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.yml
+-rw-r--r--   0        0        0     1887 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript_test.py
+-rw-r--r--   0        0        0     7393 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.py
+-rw-r--r--   0        0        0     2912 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.yml
+-rw-r--r--   0        0        0      124 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_description.md
+-rw-r--r--   0        0        0     8029 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_image.png
+-rw-r--r--   0        0        0     2955 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_test.py
+-rw-r--r--   0        0        0      251 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile
+-rw-r--r--   0        0        0    14864 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile.lock
+-rw-r--r--   0        0        0      297 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/README.md
+-rw-r--r--   0        0        0      162 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/command_examples
+-rw-r--r--   0        0        0      293 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/test_data/get_alert.json
+-rw-r--r--   0        0        0      110 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/test_data/update_alert_status.json
+-rw-r--r--   0        0        0      426 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/RN/1_0_1.md
+-rw-r--r--   0        0        0      504 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/RN/1_0_1_expected.md
+-rw-r--r--   0        0        0      303 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/RN_ENTITY/1_0_1.md
+-rw-r--r--   0        0        0      221 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/RN_ENTITY/1_0_1_expected.md
+-rw-r--r--   0        0        0    39245 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/contribution_converter_test.py
+-rw-r--r--   0        0        0    26253 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/initiator_test.py
+-rw-r--r--   0        0        0     4980 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_and_incidentfield.zip
+-rw-r--r--   0        0        0     4297 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_only.zip
+-rw-r--r--   0        0        0     1168 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/__init__.py
+-rw-r--r--   0        0        0    19994 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/integration_diff_detector.py
+-rw-r--r--   0        0        0    24585 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/tests/integration_diff_test.py
+-rw-r--r--   0        0        0     3045 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/lint/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/lint/__init__.py
+-rw-r--r--   0        0        0    11104 2023-01-22 12:54:10.902397 demisto_sdk-1.9.0/demisto_sdk/commands/lint/commands_builder.py
+-rw-r--r--   0        0        0    21054 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/helpers.py
+-rw-r--r--   0        0        0    59102 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/lint_manager.py
+-rw-r--r--   0        0        0    70069 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/linter.py
+-rwxr-xr-x   0        0        0      546 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/installation_scripts/powershell_image.sh
+-rwxr-xr-x   0        0        0      676 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/installation_scripts/python_image.sh
+-rw-r--r--   0        0        0      243 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pipfile_python2/dev-requirements.txt
+-rw-r--r--   0        0        0      374 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile
+-rw-r--r--   0        0        0    42977 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile.lock
+-rw-r--r--   0        0        0    20693 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/base_checker.py
+-rw-r--r--   0        0        0     8826 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/certified_partner_level_checker.py
+-rw-r--r--   0        0        0     1482 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/community_level_checker.py
+-rw-r--r--   0        0        0     7350 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/partner_level_checker.py
+-rw-r--r--   0        0        0     9345 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/xsoar_level_checker.py
+-rw-r--r--   0        0        0     8227 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/command_builder_test.py
+-rw-r--r--   0        0        0      632 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/docker_helper_test.py
+-rw-r--r--   0        0        0     9870 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/helper_test.py
+-rw-r--r--   0        0        0    35392 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/linter_manager_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/__init__.py
+-rw-r--r--   0        0        0     5476 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/conftest.py
+-rw-r--r--   0        0        0     6700 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/docker_runner_test.py
+-rw-r--r--   0        0        0    27436 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/gather_facts_test.py
+-rw-r--r--   0        0        0    13781 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/os_runner_test.py
+-rw-r--r--   0        0        0    28146 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/base_checker_test.py
+-rw-r--r--   0        0        0    13515 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/certified_partner_level_checker_test.py
+-rw-r--r--   0        0        0     8076 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/partner_level_checker_test.py
+-rw-r--r--   0        0        0    12885 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/xsoar_level_checker_test.py
+-rwxr-xr-x   0        0        0    51672 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/openapi_codegen.py
+-rw-r--r--   0        0        0       91 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/resources/Generated_description.md
+-rw-r--r--   0        0        0     2507 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/resources/Generated_image.png
+-rwxr-xr-x   0        0        0     9784 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/tests/openapi_codegen_test.py
+-rw-r--r--   0        0        0      133 2023-01-22 12:54:10.906396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/README.md
+-rw-r--r--   0        0        0    17722 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/postman_codegen.py
+-rw-r--r--   0        0        0    26947 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/config-urlscanio.json
+-rw-r--r--   0        0        0    17896 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/integration-urlscanio.yml
+-rw-r--r--   0        0        0    21705 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/urlscan.io.postman_collection.json
+-rw-r--r--   0        0        0    32356 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/postman_codegen_test.py
+-rw-r--r--   0        0        0    40745 2023-01-22 12:54:10.910396 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal-autogen-config.json
+-rw-r--r--   0        0        0   791658 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal.postman_collection.json
+-rw-r--r--   0        0        0     6642 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/arguments_check_collection.json
+-rw-r--r--   0        0        0     2351 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/shared_args_path.json
+-rw-r--r--   0        0        0     4411 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/__init__.py
+-rw-r--r--   0        0        0     4537 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/generic_module_unifier.py
+-rw-r--r--   0        0        0    22505 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/integration_script_unifier.py
+-rw-r--r--   0        0        0     2107 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/prepare_upload_manager.py
+-rw-r--r--   0        0        0     2263 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/preparers/marketplace_suffix_preparer.py
+-rw-r--r--   0        0        0     2426 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/rule_unifier.py
+-rw-r--r--   0        0        0     9407 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/generic_module_unifier_test.py
+-rw-r--r--   0        0        0     1312 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/xdrc_template_unifier_test.py
+-rw-r--r--   0        0        0    45408 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/yml_unifier_test.py
+-rw-r--r--   0        0        0      488 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/unifier.py
+-rw-r--r--   0        0        0      971 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/xdrc_template_unifier.py
+-rw-r--r--   0        0        0     4098 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/__init__.py
+-rw-r--r--   0        0        0    12112 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/runner.py
+-rw-r--r--   0        0        0     3912 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/runner_test.py
+-rw-r--r--   0        0        0     1251 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component.txt
+-rw-r--r--   0        0        0      944 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component_no_context.txt
+-rw-r--r--   0        0        0     2882 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_playbook/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_playbook/__init__.py
+-rw-r--r--   0        0        0     5599 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_playbook/playbook_runner.py
+-rw-r--r--   0        0        0     2584 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/__init__.py
+-rw-r--r--   0        0        0    10393 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/test_playbook_runner.py
+-rw-r--r--   0        0        0    10298 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/tests/test_playbook_runner_test.py
+-rw-r--r--   0        0        0     7050 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/secrets/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/secrets/__init__.py
+-rw-r--r--   0        0        0    27451 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/secrets/secrets.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/secrets/tests/__init__.py
+-rw-r--r--   0        0        0    15918 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/secrets/tests/secrets_test.py
+-rw-r--r--   0        0        0     2960 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/__init__.py
+-rw-r--r--   0        0        0     5129 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/jsonsplitter.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/tests/__init__.py
+-rw-r--r--   0        0        0     1514 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/tests/jsonsplitter_test.py
+-rw-r--r--   0        0        0    16476 2023-01-22 12:54:10.914397 demisto_sdk-1.9.0/demisto_sdk/commands/split/tests/ymlsplitter_test.py
+-rw-r--r--   0        0        0    24158 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/split/ymlsplitter.py
+-rw-r--r--   0        0        0    14619 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/Docker.py
+-rw-r--r--   0        0        0    12745 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/IntegrationsLock.py
+-rw-r--r--   0        0        0    13388 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/ParallelLoggingManager.py
+-rw-r--r--   0        0        0   121793 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/TestContentClasses.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/__init__.py
+-rw-r--r--   0        0        0      116 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/constants.py
+-rw-r--r--   0        0        0     4899 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/execute_test_content.py
+-rw-r--r--   0        0        0    27123 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/mock_server.py
+-rw-r--r--   0        0        0     6269 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/init_test_data.py
+-rw-r--r--   0        0        0    27553 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/test_modeling_rule.py
+-rw-r--r--   0        0        0    12811 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/init_test_data_test.py
+-rw-r--r--   0        0        0     6710 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_data/fake_test_data_file.json
+-rw-r--r--   0        0        0    45234 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_modeling_rule_test.py
+-rw-r--r--   0        0        0     5115 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/DemistoClientMock.py
+-rw-r--r--   0        0        0     8056 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/ParallelLoggingManager_test.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/__init__.py
+-rw-r--r--   0        0        0    19346 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/build_context_test.py
+-rw-r--r--   0        0        0     3122 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/execute_test_content_test.py
+-rw-r--r--   0        0        0     3912 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/integration_test.py
+-rw-r--r--   0        0        0     2563 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/mock_unit_test.py
+-rw-r--r--   0        0        0     5172 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/server_context_test.py
+-rw-r--r--   0        0        0    39339 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/test_context_test.py
+-rw-r--r--   0        0        0      587 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/test_tools.py
+-rw-r--r--   0        0        0     3299 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/testplaybook_test.py
+-rw-r--r--   0        0        0    12754 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/timestamp_replacer_test.py
+-rw-r--r--   0        0        0    24153 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/timestamp_replacer.py
+-rw-r--r--   0        0        0     3271 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tools.py
+-rw-r--r--   0        0        0     1813 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/xsiam_tools/test_data.py
+-rw-r--r--   0        0        0    10639 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/test_content/xsiam_tools/xsiam_client.py
+-rw-r--r--   0        0        0     2959 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/__init__.py
+-rw-r--r--   0        0        0     9456 2023-01-22 12:54:10.918397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests/update_rn_manager_test.py
+-rw-r--r--   0        0        0    97754 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests/update_rn_test.py
+-rw-r--r--   0        0        0      329 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests_data/Packs/Test/pack_metadata.json
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests_data/Packs/release_notes/1_0_0.md
+-rw-r--r--   0        0        0       60 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests_data/modeling_rules_yml_mock.yml
+-rw-r--r--   0        0        0    41653 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/update_rn.py
+-rw-r--r--   0        0        0    14209 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/update_rn_manager.py
+-rw-r--r--   0        0        0     1677 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/__init__.py
+-rw-r--r--   0        0        0    12847 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/tests/update_xsoar_config_file_test.py
+-rw-r--r--   0        0        0     6230 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/update_xsoar_config_file.py
+-rw-r--r--   0        0        0     5460 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/__init__.py
+-rw-r--r--   0        0        0     1135 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/data/TestPack.zip
+-rw-r--r--   0        0        0     1284 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/data/content_packs.zip
+-rw-r--r--   0        0        0      445 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/data/xsoar_config.json
+-rw-r--r--   0        0        0    54365 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/uploader_test.py
+-rw-r--r--   0        0        0     1899 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/upload.py
+-rw-r--r--   0        0        0    26203 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/upload/uploader.py
+-rw-r--r--   0        0        0     6112 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/validate/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/validate/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/validate/tests/__init__.py
+-rw-r--r--   0        0        0    98451 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/validate/tests/validators_test.py
+-rw-r--r--   0        0        0   110161 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/validate/validate_manager.py
+-rw-r--r--   0        0        0     1087 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/README.md
+-rw-r--r--   0        0        0        0 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/__init__.py
+-rw-r--r--   0        0        0     8009 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/packs_zipper.py
+-rw-r--r--   0        0        0     5098 2023-01-22 12:54:10.922397 demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/tests/packs_zipper_test.py
+-rw-r--r--   0        0        0     5227 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_client.py
+-rw-r--r--   0        0        0    10723 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier.py
+-rw-r--r--   0        0        0     7185 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier_test.py
+-rwxr-xr-x   0        0        0      615 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/deploy.sh
+-rw-r--r--   0        0        0     5880 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/server_schema_change_slack_notifier.py
+-rwxr-xr-x   0        0        0      475 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/trigger_against_content_branch.sh
+-rwxr-xr-x   0        0        0      434 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/trigger_against_content_master.sh
+-rw-r--r--   0        0        0     2473 2023-01-22 12:54:11.082398 demisto_sdk-1.9.0/demisto_sdk/utils/utils.py
+-rw-r--r--   0        0        0     3574 2023-01-22 12:54:11.086398 demisto_sdk-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0    27462 1970-01-01 00:00:00.000000 demisto_sdk-1.9.0/setup.py
+-rw-r--r--   0        0        0    12581 1970-01-01 00:00:00.000000 demisto_sdk-1.9.0/PKG-INFO
```

### Comparing `demisto_sdk-1.8.3/LICENSE` & `demisto_sdk-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/README.md` & `demisto_sdk-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/__main__.py` & `demisto_sdk-1.9.0/demisto_sdk/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,20 +888,20 @@
     "-dt",
     "--docker-timeout",
     default=60,
     help="The timeout (in seconds) for requests done by the docker client.",
     type=int,
 )
 @click.option(
-    "-idp",
-    "--id-set-path",
-    help="Path to id_set.json, relevant for when using the "
-    "--check-dependent-api-module flag.",
-    type=click.Path(resolve_path=True),
-    default="Tests/id_set.json",
+    "-di",
+    "--docker-image",
+    default="from-yml",
+    help="The docker image to check package on. Possible values: 'native:maintenance', 'native:ga', 'native:dev',"
+    " 'all', a specific docker image from Docker Hub (e.g devdemisto/python3:3.10.9.12345) or the default"
+    " 'from-yml'.",
 )
 @click.option(
     "-cdam",
     "--check-dependent-api-module",
     is_flag=True,
     help="Run unit tests and lint on all packages that "
     "are dependent on the found "
@@ -915,15 +915,15 @@
 )
 def lint(**kwargs):
     """Lint command will perform:
     1. Package in host checks - flake8, bandit, mypy, vulture.
     2. Package in docker image checks -  pylint, pytest, powershell - test, powershell - analyze.
     Meant to be used with integrations/scripts that use the folder (package) structure.
     Will lookup up what docker image to use and will setup the dev dependencies and file in the target folder.
-    If no additional flags specifying the packs are given,will lint only changed files.
+    If no additional flags specifying the packs are given, will lint only changed files.
     """
     from demisto_sdk.commands.common.logger import logging_setup
     from demisto_sdk.commands.lint.lint_manager import LintManager
 
     logging_setup(
         verbose=kwargs.get("verbose"),  # type: ignore[arg-type]
         quiet=kwargs.get("quiet"),  # type: ignore[arg-type]
@@ -935,15 +935,14 @@
         input=kwargs.get("input"),  # type: ignore[arg-type]
         git=kwargs.get("git"),  # type: ignore[arg-type]
         all_packs=kwargs.get("all_packs"),  # type: ignore[arg-type]
         verbose=kwargs.get("verbose"),  # type: ignore[arg-type]
         quiet=kwargs.get("quiet"),  # type: ignore[arg-type]
         prev_ver=kwargs.get("prev_ver"),  # type: ignore[arg-type]
         json_file_path=kwargs.get("json_file"),  # type: ignore[arg-type]
-        id_set_path=kwargs.get("id_set_path"),  # type: ignore[arg-type]
         check_dependent_api_module=kwargs.get("check_dependent_api_module"),  # type: ignore[arg-type]
     )
     return lint_manager.run(
         parallel=kwargs.get("parallel"),  # type: ignore[arg-type]
         no_flake8=kwargs.get("no_flake8"),  # type: ignore[arg-type]
         no_bandit=kwargs.get("no_bandit"),  # type: ignore[arg-type]
         no_mypy=kwargs.get("no_mypy"),  # type: ignore[arg-type]
@@ -955,14 +954,15 @@
         no_pwsh_test=kwargs.get("no_pwsh_test"),  # type: ignore[arg-type]
         keep_container=kwargs.get("keep_container"),  # type: ignore[arg-type]
         test_xml=kwargs.get("test_xml"),  # type: ignore[arg-type]
         failure_report=kwargs.get("failure_report"),  # type: ignore[arg-type]
         no_coverage=kwargs.get("no_coverage"),  # type: ignore[arg-type]
         coverage_report=kwargs.get("coverage_report"),  # type: ignore[arg-type]
         docker_timeout=kwargs.get("docker_timeout"),  # type: ignore[arg-type]
+        docker_image_flag=kwargs.get("docker_image"),  # type: ignore[arg-type]
         time_measurements_dir=kwargs.get("time_measurements_dir"),  # type: ignore[arg-type]
     )
 
 
 # ====================== coverage-analyze ====================== #
 @main.command()
 @click.help_option("-h", "--help")
@@ -2615,14 +2615,21 @@
     help="The branch against which changes will be detected "
     "if '-g' flag is set. Default is 'demisto/master'",
 )
 @click.option(
     "-rn", "--release-notes", is_flag=True, help="Will run only on release notes files"
 )
 @click.option(
+    "-xs",
+    "--xsoar-only",
+    is_flag=True,
+    help="Run only on files from XSOAR-supported Packs.",
+    default=False,
+)
+@click.option(
     "-pkw",
     "--use-packs-known-words",
     is_flag=True,
     help="Will find and load the known_words file from the pack. "
     "To use this option make sure you are running from the "
     "content directory.",
     default=False,
@@ -2637,14 +2644,15 @@
         no_camel_case=kwargs.get("no_camel_case"),
         no_failure=kwargs.get("always_true"),
         expand_dictionary=kwargs.get("expand_dictionary"),
         templates=kwargs.get("templates"),
         use_git=kwargs.get("use_git"),
         prev_ver=kwargs.get("prev_ver"),
         release_notes_only=kwargs.get("release_notes"),
+        xsoar_only=kwargs.get("xsoar_only"),
         load_known_words_from_pack=kwargs.get("use_packs_known_words"),
     )
     result = doc_reviewer.run_doc_review()
     if result:
         sys.exit(0)
 
     sys.exit(1)
@@ -2988,14 +2996,19 @@
     type=click.Path(
         path_type=Path, resolve_path=True, exists=True, file_okay=True, dir_okay=False
     ),
     default=None,
     help="Path to content graph zip file to import",
 )
 @click.option(
+    "--use-current",
+    help="Whether to use the current content graph to update",
+    default=False,
+)
+@click.option(
     "-p",
     "--packs",
     help="A comma-separated list of packs to update",
     multiple=True,
     default=None,
 )
 @click.option(
@@ -3029,14 +3042,15 @@
     "--log-path",
     help="Path to store all levels of logs",
     type=click.Path(resolve_path=True),
 )
 def update_content_graph(
     use_git: bool = False,
     marketplace: MarketplaceVersions = MarketplaceVersions.XSOAR,
+    use_current: bool = False,
     imported_path: Path = None,
     packs: list = None,
     no_dependencies: bool = False,
     output_path: Path = None,
     **kwargs,
 ):
     from demisto_sdk.commands.common.logger import logging_setup
@@ -3048,21 +3062,24 @@
     )
 
     logging_setup(
         verbose=kwargs.get("verbose"),  # type: ignore[arg-type]
         quiet=kwargs.get("quiet"),  # type: ignore[arg-type]
         log_path=kwargs.get("log_path"),
     )  # type: ignore[arg-type]
-
+    if packs and not isinstance(packs, list):
+        # for some reason packs provided as tuple from click interface
+        packs = list(packs)
     with Neo4jContentGraphInterface() as content_graph_interface:
         update_content_graph_command(
             content_graph_interface,
             marketplace=MarketplaceVersions(marketplace),
             use_git=use_git,
             imported_path=imported_path,
+            use_current=use_current,
             packs_to_update=packs or [],
             dependencies=not no_dependencies,
             output_path=output_path,
         )
 
 
 @main.result_callback()
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/MDXServer.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/MDXServer.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/configuration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/configuration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/constants.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,14 @@
 MODELING_RULE = "modelingrule"
 CORRELATION_RULE = "correlationrule"
 XSIAM_DASHBOARD = "xsiamdashboard"
 XSIAM_REPORT = "xsiamreport"
 TRIGGER = "trigger"
 WIZARD = "wizard"
 XDRC_TEMPLATE = "xdrctemplate"
-
 MARKETPLACE_KEY_PACK_METADATA = "marketplaces"
 
 # ENV VARIABLES
 
 ENV_DEMISTO_SDK_MARKETPLACE = "DEMISTO_SDK_MARKETPLACE"
 
 
@@ -160,14 +159,22 @@
     SECRET_IGNORE = ".secrets-ignore"
     DOC_FILE = "doc_files"
     XDRC_TEMPLATE = "xdrctemplate"
     XDRC_TEMPLATE_YML = "xdrctemplateyml"
     INDICATOR_TYPE = "indicatortype"
     TOOL = "tools"
     PACK_METADATA = "packmetadata"
+    PIPFILE = "pipfile"
+    TXT = "txt"
+    PIPFILE_LOCK = "pipfilelock"
+    PYLINTRC = "pylintrc"
+    LICENSE = "license"
+    UNIFIED_YML = "unified_yml"
+    INI = "ini"
+    PEM = "pem"
 
 
 RN_HEADER_BY_FILE_TYPE = {
     FileType.PLAYBOOK: "Playbooks",
     FileType.INTEGRATION: "Integrations",
     FileType.BETA_INTEGRATION: "Integrations",
     FileType.SCRIPT: "Scripts",
@@ -198,14 +205,18 @@
     FileType.XSIAM_DASHBOARD: "XSIAM Dashboards",
     FileType.XSIAM_REPORT: "XSIAM Reports",
     FileType.TRIGGER: "Triggers Recommendations",  # https://github.com/demisto/etc/issues/48153#issuecomment-1111988526
     FileType.WIZARD: "Wizards",
     FileType.XDRC_TEMPLATE: "XDRC Templates",
 }
 
+FILE_TYPE_BY_RN_HEADER = {
+    header: file_type for file_type, header in RN_HEADER_BY_FILE_TYPE.items()
+}
+
 ENTITY_TYPE_TO_DIR = {
     FileType.INTEGRATION.value: INTEGRATIONS_DIR,
     FileType.PLAYBOOK.value: PLAYBOOKS_DIR,
     FileType.SCRIPT.value: SCRIPTS_DIR,
     AUTOMATION: SCRIPTS_DIR,
     FileType.LAYOUT.value: LAYOUTS_DIR,
     FileType.LAYOUTS_CONTAINER.value: LAYOUTS_DIR,
@@ -230,14 +241,16 @@
     FileType.JOB.value: JOBS_DIR,
     FileType.PARSING_RULE.value: PARSING_RULES_DIR,
     FileType.MODELING_RULE.value: MODELING_RULES_DIR,
     FileType.WIZARD.value: WIZARDS_DIR,
     FileType.XDRC_TEMPLATE.value: XDRC_TEMPLATE_DIR,
     FileType.CORRELATION_RULE.value: CORRELATION_RULES_DIR,
     FileType.XSIAM_DASHBOARD.value: XSIAM_DASHBOARDS_DIR,
+    FileType.TRIGGER.value: TRIGGER_DIR,
+    FileType.OLD_CLASSIFIER.value: CLASSIFIERS_DIR,
 }
 
 SIEM_ONLY_ENTITIES = [
     FileType.PARSING_RULE.value,
     FileType.MODELING_RULE.value,
     FileType.CORRELATION_RULE.value,
     FileType.XSIAM_DASHBOARD.value,
@@ -307,14 +320,15 @@
 RN_CONTENT_ENTITY_WITH_STARS = [
     FileType.CONNECTION,
     FileType.INCIDENT_TYPE,
     FileType.REPUTATION,
     FileType.LAYOUT,
     FileType.INCIDENT_FIELD,
     FileType.INDICATOR_FIELD,
+    FileType.TRIGGER,
     FileType.GENERIC_DEFINITION,
     FileType.GENERIC_MODULE,
     FileType.GENERIC_TYPE,
     FileType.GENERIC_FIELD,
 ]
 
 DEFAULT_IMAGE_PREFIX = "data:image/png;base64,"
@@ -1469,15 +1483,14 @@
     FileType.TEST_PLAYBOOK,
     FileType.TEST_SCRIPT,
     FileType.DOC_IMAGE,
     FileType.AUTHOR_IMAGE,
     None,
     FileType.RELEASE_NOTES_CONFIG,
     FileType.CONTRIBUTORS,
-    FileType.TRIGGER,
 )
 
 LAYOUT_AND_MAPPER_BUILT_IN_FIELDS = [
     "indicatortype",
     "source",
     "comment",
     "aggregatedreliability",
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/content.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/content.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/docs/CONTRIBUTION.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/docs/CONTRIBUTION.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/errors.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/errors.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/dictionary_based_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/dictionary_based_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/general_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/general_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/json_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/json_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/text_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/text_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/abstract_objects/yaml_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/abstract_objects/yaml_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/__init__.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/__init__.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/json_content_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/json_content_object.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from demisto_sdk.commands.common.content.objects.pack_objects.change_log.change_log import (
     ChangeLog,
 )
 from demisto_sdk.commands.common.content.objects.pack_objects.readme.readme import (
     Readme,
 )
 from demisto_sdk.commands.common.tools import get_json
+from demisto_sdk.commands.prepare_content.prepare_upload_manager import (
+    PrepareUploadManager,
+)
 
 
 class JSONContentObject(JSONObject):
     def __init__(self, path: Union[Path, str], file_name_prefix):
         """JSON content object.
 
         Built from:
@@ -129,7 +132,33 @@
     def is_file_structure_list(self) -> bool:
         """
         Checks whether the content of the file has a structure of a list.
         Assuming the file is a valid json file, use this to determine whether the file holds a list of values or a dictionary.
         """
         data = get_json(str(self.path))
         return isinstance(data, list)
+
+    def _unify(
+        self, dest_dir: Optional[Union[Path, str]] = None, output: str = ""
+    ) -> List[Path]:
+        """Unify JSONBasedContentObject in destination dir.
+
+        Args:
+            dest_dir: Destination directory, if not provided the destination directory will be the current working dir.
+            output: output suffix to add the destination directory.
+
+        Returns:
+            List[Path]: List of new created unified json files.
+        """
+        if dest_dir is None:
+            dest_dir = ""
+
+        # Unify step
+        return [
+            Path(
+                str(
+                    PrepareUploadManager.prepare_for_upload(
+                        input=self.path, output=Path(dest_dir, output)  # type: ignore[arg-type]
+                    )
+                )
+            )
+        ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_content_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_content_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_unify_content_object.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/abstract_pack_objects/yaml_unify_content_object.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/classifier/classifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/classifier/classifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/corrlation_rule/correlation_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/corrlation_rule/correlation_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/dashboard/dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_definition/generic_definition.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_definition/generic_definition.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_field/generic_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_field/generic_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_module/generic_module.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_module/generic_module.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/generic_type/generic_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/generic_type/generic_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/incident_field/incident_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/incident_field/incident_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/incident_type/incident_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/incident_type/incident_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/indicator_field/indicator_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/indicator_field/indicator_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/indicator_type/indicator_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/indicator_type/indicator_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/integration/integration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/integration/integration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/job/job.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/job/job.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/layout/layout.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/layout/layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import tempfile
 from abc import abstractmethod
 from typing import List, Optional, Union
 
 import demisto_client
 from wcmatch.pathlib import Path
 
 from demisto_sdk.commands.common.constants import FileType
@@ -20,14 +21,18 @@
         Upload the Layout object to demisto_client.
         Args:
             client (demisto_client): The Demisto client object of the desired XSOAR machine to upload to.
 
         Returns:
             The result of the upload command from demisto_client.
         """
+        if self.layout_type == FileType.LAYOUTS_CONTAINER:
+            with tempfile.TemporaryDirectory() as _dir:
+                return client.import_layout(file=self._unify(_dir)[0])
+
         return client.import_layout(file=self.path)
 
     @abstractmethod
     def layout_id(self) -> Optional[str]:
         """
         Returns the layout ID of the given layout.
         Returns:
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/lists/lists.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/lists/lists.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/modeling_rule/modeling_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/modeling_rule/modeling_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pack.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pack.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pack_metadata/pack_metadata.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pack_metadata/pack_metadata.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/parsing_rule/parsing_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/parsing_rule/parsing_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/playbook/playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/playbook/playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/pre_process_rule/pre_process_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/pre_process_rule/pre_process_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/readme/readme.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/readme/readme.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/report/report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/report/report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/script/script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/script/script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/tool/agent_tool.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/tool/agent_tool.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/trigger/trigger.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/trigger/trigger.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/widget/widget.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/widget/widget.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xdrc_template/xdrc_template.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xdrc_template/xdrc_template.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,17 +5,14 @@
 
 import demisto_sdk.commands.common.content.errors as exc
 from demisto_sdk.commands.common.constants import XDRC_TEMPLATE, FileType
 from demisto_sdk.commands.common.content.objects.pack_objects.abstract_pack_objects.json_content_object import (
     JSONContentObject,
 )
 from demisto_sdk.commands.common.tools import generate_xsiam_normalized_name
-from demisto_sdk.commands.prepare_content.prepare_upload_manager import (
-    PrepareUploadManager,
-)
 
 
 class XDRCTemplate(JSONContentObject):
     def __init__(self, path: Union[Path, str]):
         super().__init__(path, XDRC_TEMPLATE)
 
     def normalize_file_name(self) -> str:
@@ -32,35 +29,26 @@
         """
         # return client.import_parsing_rules(file=self.path)
         pass
 
     def type(self):
         return FileType.XDRC_TEMPLATE
 
-    def _unify(self, dest_dir: Path = None) -> List[Path]:
+    def _unify(self, dest_dir: Path = None, output: str = "") -> List[Path]:
         """Unify XDRCTemplate in destination dir.
 
         Args:
             dest_dir: Destination directory.
 
         Returns:
             List[Path]: List of new created files.
         """
-        if isinstance(dest_dir, str):
-            dest_dir = Path(dest_dir)
-        # Unify step
-        return [
-            Path(
-                str(
-                    PrepareUploadManager.prepare_for_upload(
-                        input=self.path, output=dest_dir / self.normalize_file_name()  # type: ignore[operator]
-                    )
-                )
-            )
-        ]
+        return super()._unify(
+            dest_dir=dest_dir, output=output or self.normalize_file_name()
+        )
 
     def _create_target_dump_dir(
         self, dest_dir: Optional[Union[Path, str]] = None
     ) -> Path:
         """Create destination directory, Destination must be valid directory, If not specified dump in
          path of origin object.
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard/xsiam_dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard/xsiam_dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report/xsiam_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report/xsiam_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report_image/xsiam_report_image.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects/pack_objects/xsiam_report_image/xsiam_report_image.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/objects_factory.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/objects_factory.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/content_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/content_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/json_object_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/json_object_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/text_object_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/text_object_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/abstract_objects/yaml_object_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/abstract_objects/yaml_object_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/json_content_object_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/json_content_object_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/yaml_content_object_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/abstract_pack_objects/yaml_content_object_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/author_image/author_image_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/author_image/author_image_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/change_log/change_log_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/change_log/change_log_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/classifier/classifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/connection/connection_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/connection/connection_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/correlation_rule/correlation_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/correlation_rule/correlation_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/dashboard/dashboard_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/dashboard/dashboard_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/doc_file/doc_file_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/doc_file/doc_file_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_field/incident_field_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_field/incident_field_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_type/incident_type_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/incident_type/incident_type_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_field/indicator_field_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_field/indicator_field_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/indicator_type/indicator_type_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/integration/integration_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test/Jobs/sample-job.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test/Jobs/sample-job.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/job/job_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/lists/lists_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/lists/lists_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/modeling_rule/modeling_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/modeling_rule/modeling_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_ignore/pack_ignore_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_ignore/pack_ignore_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_metadata/pack_metadata_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_metadata/pack_metadata_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pack_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/parsing_rule/parsing_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/parsing_rule/parsing_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/playbook/playbook_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/playbook/playbook_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/pre_process_rule/pre_process_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/pre_process_rule/pre_process_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/readme/readme_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/readme/readme_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note/release_note_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note/release_note_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note_config/release_note_config_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/release_note_config/release_note_config_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/report/report_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/report/report_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test/TestNotUnifiedScript/FindSimilarIncidentsByText.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/script/script_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/secret_ignore/secret_ignore_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/secret_ignore/secret_ignore_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/trigger/trigger_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/trigger/trigger_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/widget/widget_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/widget/widget_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test/Wizards/sample-wizard.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test/Wizards/sample-wizard.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/wizard/wizard_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xdrctemplate/xdrc_template_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xdrctemplate/xdrc_template_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard/xsiam_dashboard_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard/xsiam_dashboard_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_dashboard_image/xsiam_dashboard_image_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report/xsiam_report_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report/xsiam_report_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report_image/xsiam_report_image_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/content/tests/objects/pack_objects/xsiam_report_image/xsiam_report_image_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/default_output_descriptions.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/default_output_descriptions.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/docker_helper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/docker_helper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/errors.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/errors.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/git_content_config.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/git_content_config.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/git_util.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/git_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,15 +459,15 @@
 
         return all_renamed_files
 
     def get_all_changed_pack_ids(self, prev_ver: str) -> Set[str]:
         return {
             file.parts[1]
             for file in self.get_all_changed_files(prev_ver)
-            if PACKS_FOLDER in file.parts
+            if file.parts[0] == PACKS_FOLDER
         }
 
     def _get_untracked_files(self, requested_status: str) -> set:
         """return all untracked files of the given requested status.
         Args:
             requested_status (str): M, A, R, D - the git status to return
         Returns:
@@ -791,7 +791,16 @@
             committed_only=committed_only,  # type: ignore[assignment]
             staged_only=staged_only,
             debug=debug,
             include_untracked=include_untracked,
             get_only_current_file_names=True,
         )
         return modified_files.union(added_files).union(renamed_files)
+
+    def _is_file_git_ignored(self, file_path: str) -> bool:
+        """return wether the file is in .gitignore file or not.
+        Args:
+            file_path (str): the file to check.
+        Returns:
+            bool: True if the file is ignored. Otherwise, return False.
+        """
+        return bool(self.repo.ignored(file_path))
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/json/orjson_handler.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/json/orjson_handler.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/json/ujson_handler.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/json/ujson_handler.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/tests/json_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/tests/json_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/handlers/yaml/ruamel_handler.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/handlers/yaml/ruamel_handler.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/author_image.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/author_image.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/base_validator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/base_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,30 +150,35 @@
         error_message,
         error_code,
         file_path,
         should_print=True,
         suggested_fix=None,
         warning=False,
         drop_line=False,
+        ignored_errors=None,
     ):
         """
         Handle an error that occurred during validation.
 
         Args:
             drop_line (bool): Whether to drop a line at the beginning of the error message
             warning (bool): Print the error as a warning
             suggested_fix (str): A suggested fix
             error_message (str): The error message
             file_path (str): The file from which the error occurred
             error_code (str): The error code
             should_print (bool): whether the command should be printed
+            ignored_errors (dict): if there are any ignored_errors, will override the ignored_errors attribute.
 
         Returns:
             str: formatted error message, None in case validation should be skipped or can be ignored.
         """
+        if ignored_errors:
+            self.ignored_errors = ignored_errors
+
         if self.specific_validations:
             if not self.should_run_validation(error_code):
                 # if the error code is not specified in the
                 # specific_validations list, we exit the function and return None
                 return None
 
         def formatted_error_str(error_type):
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/classifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/classifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/conf_json.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/conf_json.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,16 +96,20 @@
                 return True
 
         error_message, error_code = Errors.test_not_in_conf_json(file_id)
         if self.handle_error(error_message, error_code, file_path=CONF_PATH):
             return False
         return True
 
-    def is_valid_file_in_conf_json(self, current_file, file_type, file_path):
+    def is_valid_file_in_conf_json(
+        self, current_file, file_type, file_path, ignored_errors=None
+    ):
         """Check if the file is valid in the conf.json"""
+        if ignored_errors:
+            self.ignored_errors = ignored_errors
         entity_id = _get_file_id(file_type.value, current_file)
         if file_type in {FileType.INTEGRATION, FileType.BETA_INTEGRATION}:
             return self.integration_has_unskipped_test_playbook(
                 current_file, entity_id, file_path
             )
         if file_type == FileType.SCRIPT:
             return self.has_unskipped_test_playbook(
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/content_entity_validator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/content_entity_validator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/correlation_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/correlation_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/deprecation.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/deprecation.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/description.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/description.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/docker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/docker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/field_base_validator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/field_base_validator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_definition.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_definition.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_module.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_module.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/generic_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/generic_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/id.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/id.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/image.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/image.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/incident_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/incident_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/incident_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/incident_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/indicator_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/indicator_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/integration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/integration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/job.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/job.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/layout.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/layout.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/lists.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/lists.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/mapper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/mapper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/modeling_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/modeling_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/old_release_notes.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/old_release_notes.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/pack_unique_files.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/pack_unique_files.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/parsing_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/parsing_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/pre_process_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/pre_process_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/python_file.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/python_file.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/readme.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/readme.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/release_notes.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/release_notes.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import re
 from typing import Dict, List, Tuple, Union
 
 from demisto_sdk.commands.common.constants import (
     CUSTOM_CONTENT_FILE_ENDINGS,
     ENTITY_TYPE_TO_DIR,
+    FILE_TYPE_BY_RN_HEADER,
     PACKS_DIR,
     RN_HEADER_BY_FILE_TYPE,
     SKIP_RELEASE_NOTES_FOR_TYPES,
 )
 from demisto_sdk.commands.common.errors import Errors
 from demisto_sdk.commands.common.hook_validations.base_validator import (
     BaseValidator,
@@ -182,18 +183,17 @@
         Args:
             content_type: (str) - The content type to validate.(e.g. Integrations, Playbooks, etc.)
             content_items: (Dict) - The content items headers to validate.
         Return:
             True if the content item is valid, False otherwise.
         """
         is_valid = True
-        entity_type = content_type.replace(" ", "")
-        entity_type = entity_type[:-1] if entity_type.endswith("s") else entity_type
+        entity_type = FILE_TYPE_BY_RN_HEADER.get(content_type, "")
 
-        content_type_dir_name = ENTITY_TYPE_TO_DIR.get(entity_type.lower(), entity_type)
+        content_type_dir_name = ENTITY_TYPE_TO_DIR.get(entity_type, entity_type)
         content_type_path = os.path.join(self.pack_path, content_type_dir_name)
 
         content_type_dir_list = get_files_in_dir(
             content_type_path,
             CUSTOM_CONTENT_FILE_ENDINGS,
             recursive=True,
             ignore_test_files=True,
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/release_notes_config.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/release_notes_config.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/reputation.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/reputation.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/structure.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/structure.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/test_playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/test_playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/triggers.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/triggers.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/widget.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/widget.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/wizard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/wizard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xdrc_templates.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xdrc_templates.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsiam_dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsiam_dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsiam_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsiam_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/hook_validations/xsoar_config_json.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/hook_validations/xsoar_config_json.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/legacy_git_tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/legacy_git_tools.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/logger.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/logger.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/mdx-parse-server.js` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/mdx-parse-server.js`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/native_image.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/native_image.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 json = JSON_Handler()
 logger = logging.getLogger("demisto-sdk")
 
 
 class NativeImage(BaseModel):
     supported_docker_images: List[str]
-    docker_ref: str
+    docker_ref: Optional[str]
 
 
 class IgnoredContentItem(BaseModel):
     id: str
     reason: str
     ignored_native_images: List[str]
 
@@ -29,14 +29,15 @@
 def _extract_native_image_version_for_server(native_image: str) -> str:
     return native_image.replace("native:", "")
 
 
 class NativeImageConfig(Singleton, BaseModel):
     native_images: Dict[str, NativeImage]
     ignored_content_items: List[IgnoredContentItem]
+    flags_versions_mapping: Dict[str, str] = {}
     docker_images_to_native_images_mapping: Dict[str, List] = {}
 
     def __init__(
         self, native_image_config_file_path: str = f"Tests/{NATIVE_IMAGE_FILE_NAME}"
     ):
         super().__init__(**self.load(native_image_config_file_path))
         self.docker_images_to_native_images_mapping = (
@@ -76,33 +77,49 @@
         Load the native image configuration file
         """
         native_image_config_content, _ = get_dict_from_file(
             native_image_config_file_path
         )
         return native_image_config_content
 
+    def get_native_image_reference(self, native_image) -> Optional[str]:
+        """
+        Gets the docker reference of the given native image
+
+        Args:
+            native_image (str): native image (for example: 'native:8.1')
+
+        Returns: The docker ref
+        """
+        if native_image_obj := self.native_images.get(native_image):
+            return native_image_obj.docker_ref
+
+        return None
+
 
 class ScriptIntegrationSupportedNativeImages:
 
     """
     Class that defines which native images should be supported in a script/integration by the following criteria(s):
 
     1) if the docker-image that the integration/script uses is supported in the native image(s)
     2) if the integration/script is not ignored in the configuration file.
 
     Args:
         _id (str): the ID that the script/integration has.
         docker_image (str): the docker image that the integration/script uses. (dockerimage key in the yml).
     """
 
+    NATIVE_DEV = "native:dev"
+
     def __init__(
         self,
         _id: str,
-        docker_image: Optional[str],
         native_image_config: NativeImageConfig,
+        docker_image: Optional[str] = None,
     ):
         self.id = _id
         self.docker_image = (
             extract_docker_image_from_text(text=docker_image, with_no_tag=True)
             if docker_image
             else docker_image
         )
@@ -132,33 +149,37 @@
                     f"content item ID: {self.id} cannot run with these native "
                     f"images: {ignored_native_images}, reason: {reason}"
                 )
                 return ignored_native_images
         return []
 
     def get_supported_native_image_versions(
-        self, get_raw_version: bool = False
+        self, get_raw_version: bool = False, only_production_tags: bool = True
     ) -> List[str]:
         """
-        Get the native-images that the integration/script supports. Disregards native-images that are supported which
-        should be ignored.
+        Get the native-images that the integration/script supports. Disregards native-images that should be ignored.
 
         Args:
             get_raw_version (bool): whether to extract the raw server version from the native image name, for example:
-              'native:8.2' will become '8.2' for each one of the native-images that are supported.
+                                    'native:8.2' will become '8.2' for each one of the native-images that are supported.
+            only_production_tags (bool): whether to ignore the latest native image.
         """
         if native_images := self.__docker_image_to_native_images_support():
             # in case there is a script/integration that should be ignored on a specific native image,
-            # the native image(s) which doesn't support him will be removed.
+            # the native image(s) which doesn't support it will be removed.
             ignored_native_images = self.__get_ignored_native_images()
             native_images = [
                 native_image
                 for native_image in native_images
                 if native_image not in ignored_native_images
             ]
+
+            if only_production_tags and self.NATIVE_DEV in native_images:
+                native_images.remove(self.NATIVE_DEV)
+
             if get_raw_version:
                 return list(
                     map(_extract_native_image_version_for_server, native_images)
                 )
             return native_images
         return []
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/classifier.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/classifier.yml`

 * *Files 0% similar despite different names*

```diff
@@ -54,8 +54,8 @@
     type: bool
   definitionId:
     type: str
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: ['xsoar', 'marketplacev2']
+        enum: ['xsoar', 'marketplacev2', 'xpanse' ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/classifier_5_9_9.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/classifier_5_9_9.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/dashboard.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/dashboard.yml`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,19 @@
   period:
     type: map
     allowempty: True
   layout:
     type: seq
     sequence:
       - include: layout_schema
+  marketplaces:
+    type: seq
+    sequence:
+      - type: str
+        enum: [ 'xsoar', 'marketplacev2', 'xpanse' ]
 
 
 
 schema;layout_schema:
   type: map
   mapping:
     id:
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/genericfield.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/genericfield.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/genericmodule.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/genericmodule.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/generictype.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/generictype.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidentfield.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidentfield.yml`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
     type: str
   openEnded:
     type: bool
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: [ 'xsoar', 'marketplacev2' ]
+        enum: [ 'xsoar', 'marketplacev2', 'xpanse'  ]
   Aliases:
     type: seq
     sequence:
       - include: aliases_schema
   x2_fields:
     type: str
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidentfields.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidentfields.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/incidenttype.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/incidenttype.yml`

 * *Files 8% similar despite different names*

```diff
@@ -73,8 +73,8 @@
         type: any
       mode:
         type: str
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: ['xsoar', 'marketplacev2']
+        enum: ['xsoar', 'marketplacev2', 'xpanse' ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/indicatorfield.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/indicatorfield.yml`

 * *Files 5% similar despite different names*

```diff
@@ -86,8 +86,8 @@
     type: any
   openEnded:
     type: bool
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: ['xsoar', 'marketplacev2']
+        enum: ['xsoar', 'marketplacev2', 'xpanse' ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/integration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/integration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/job.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/job.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/layout.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/layout.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/layoutscontainer.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/layoutscontainer.yml`

 * *Files 1% similar despite different names*

```diff
@@ -20,14 +20,19 @@
     required: True
   toVersion:
     type: str
   description:
     type: str
   system:
     type: bool
+  marketplaces:
+    type: seq
+    sequence:
+      - type: str
+        enum: [ 'xsoar', 'marketplacev2', 'xpanse' ]
   edit:
     type: map
     mapping:
       tabs:
         type: seq
         sequence:
         - include: tabs_schema
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/list.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/list.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/mapper.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/mapper.yml`

 * *Files 1% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     type: bool
   definitionId:
     type: str
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: ['xsoar', 'marketplacev2']
+        enum: ['xsoar', 'marketplacev2', 'xpanse' ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/playbook.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/playbook.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/pre-process-rules.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/pre-process-rules.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/report.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/report.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/reputation.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/reputation.yml`

 * *Files 7% similar despite different names*

```diff
@@ -68,8 +68,8 @@
     type: seq
     sequence:
       - type: str
   marketplaces:
     type: seq
     sequence:
       - type: str
-        enum: ['xsoar', 'marketplacev2']
+        enum: ['xsoar', 'marketplacev2', 'xpanse' ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/script.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/script.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/widget.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/widget.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/wizard.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/wizard.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/schemas/xsoar_config.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/schemas/xsoar_config.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/author_image_validator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/author_image_validator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/base_validator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/base_validator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/classifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/classifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/conf_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/conf_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/content_entity_validator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/content_entity_validator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/correlation_rules_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/correlation_rules_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/dashboard_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/dashboard_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/dependencies_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/deprecation_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/deprecation_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/description_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/description_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/docker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/docker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/errors_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/errors_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/field_validator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/field_validator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/generic_field_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/generic_field_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/git_config_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/git_config_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/git_util_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/git_util_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/id_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/id_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/image_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/image_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/incident_field_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/incident_field_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/incident_type_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/incident_type_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/indicator_field_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/indicator_field_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/integration_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/layout_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/layout_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/legacy_git_tools_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/legacy_git_tools_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/lists_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/lists_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/mapper_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/mapper_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/modeling_rules_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/modeling_rules_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/native_image_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/native_image_test.py`

 * *Files 25% similar despite different names*

```diff
@@ -38,24 +38,51 @@
     When
     - mapping docker images into native images
 
     Then
     - make sure each docker image is getting mapped correctly
     """
     assert native_image_config.docker_images_to_native_images_mapping == {
-        "python3": ["native:8.1", "native:8.2"],
-        "py3-tools": ["native:8.1", "native:8.2"],
-        "unzip": ["native:8.1", "native:8.2"],
-        "chromium": ["native:8.1", "native:8.2"],
-        "tesseract": ["native:8.1", "native:8.2"],
+        "python3": ["native:8.1", "native:8.2", "native:dev"],
+        "py3-tools": ["native:8.1", "native:8.2", "native:dev"],
+        "unzip": ["native:8.1", "native:8.2", "native:dev"],
+        "chromium": ["native:8.1", "native:8.2", "native:dev"],
+        "tesseract": ["native:8.1", "native:8.2", "native:dev"],
         "pan-os-python": ["native:8.2"],
-        "tld": ["native:8.1"],
+        "tld": ["native:8.1", "native:dev"],
     }
 
 
+@pytest.mark.parametrize(
+    "native_image, expected_image_reference",
+    [("native:8.1", "demisto/py3-native:8.1.0.12345"), ("native:8.4", None)],
+)
+def test_get_native_image_reference(
+    native_image_config, native_image, expected_image_reference
+):
+    """
+    Given
+    - native image configuration file, native image name:
+        1. A native image that exists in the configuration file
+        2. A native image that doesn't exist in the configuration file
+
+    When
+    - running the get_native_image_reference() function
+
+    Then
+    - make sure the right docker references is extracted
+        1. The matched reference from the configuration file
+        2. None
+    """
+    assert (
+        native_image_config.get_native_image_reference(native_image)
+        == expected_image_reference
+    )
+
+
 class TestScriptIntegrationSupportedNativeImages:
     @pytest.mark.parametrize(
         "_id, docker_image, expected_native_images",
         [
             (
                 "UnzipFile",
                 "demisto/unzip:1.0.0.23423",
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/old_release_notes_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/old_release_notes_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pack_metadata_validator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pack_metadata_validator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pack_unique_files_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pack_unique_files_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from demisto_sdk.commands.common.errors import Errors
 from demisto_sdk.commands.common.handlers import JSON_Handler
 from demisto_sdk.commands.common.hook_validations.base_validator import BaseValidator
 from demisto_sdk.commands.common.hook_validations.pack_unique_files import (
     PackUniqueFilesValidator,
 )
 from demisto_sdk.commands.common.legacy_git_tools import git_path
+from demisto_sdk.commands.validate.validate_manager import ValidateManager
 from TestSuite.test_tools import ChangeCWD
 
 json = JSON_Handler()
 
 
 VALIDATE_CMD = "validate"
 PACK_METADATA_PARTNER = {
@@ -178,14 +179,15 @@
         When
         - Running validate on it.
 
         Then
         - Ensure validate found errors.
         """
         pack_metadata_no_email_and_url = PACK_METADATA_PARTNER.copy()
+        mocker.patch.object(ValidateManager, "setup_git_params", return_value=True)
         pack_metadata_no_email_and_url["email"] = ""
         pack_metadata_no_email_and_url["url"] = ""
         mocker.patch.object(tools, "is_external_repository", return_value=True)
         mocker.patch.object(
             PackUniqueFilesValidator, "_is_pack_file_exists", return_value=True
         )
         mocker.patch.object(
@@ -231,22 +233,22 @@
         - Running validate on it.
 
         Then
         - Ensure validate finds errors accordingly.
         """
         pack_metadata_changed_url = PACK_METADATA_PARTNER.copy()
         pack_metadata_changed_url["url"] = url
-
         mocker.patch.object(tools, "is_external_repository", return_value=True)
         mocker.patch.object(
             PackUniqueFilesValidator, "_is_pack_file_exists", return_value=True
         )
         mocker.patch.object(
             PackUniqueFilesValidator, "validate_pack_name", return_value=True
         )
+        mocker.patch.object(ValidateManager, "setup_git_params", return_value=True)
         mocker.patch.object(
             PackUniqueFilesValidator,
             "get_master_private_repo_meta_file",
             return_value=None,
         )
         mocker.patch.object(
             PackUniqueFilesValidator,
@@ -303,14 +305,15 @@
             "_read_file_content",
             return_value=json.dumps(pack_metadata_price_changed),
         )
         mocker.patch.object(BaseValidator, "check_file_flags", return_value=None)
         mocker.patch.object(
             tools, "get_dict_from_file", return_value=({"approved_list": {}}, "json")
         )
+        mocker.patch.object(ValidateManager, "setup_git_params", return_value=True)
         pack = repo.create_pack("PackName")
         pack.pack_metadata.write_json(pack_metadata_price_changed)
         with ChangeCWD(repo.path):
             runner = CliRunner(mix_stderr=False)
             result = runner.invoke(
                 main, [VALIDATE_CMD, "-i", pack.path], catch_exceptions=False
             )
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/playbook_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/playbook_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/pre_process_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/pre_process_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/python_file_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/python_file_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/readme_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/readme_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/release_notes_config_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/release_notes_config_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/release_notes_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/release_notes_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -728,14 +728,15 @@
     pack.create_indicator_field("test")
     pack.create_indicator_type("test")
     pack.create_layout("test")
     pack.create_mapper("test")
     pack.create_classifier("test")
     pack.create_widget("test")
     pack.create_xsiam_dashboard("xsiam-dashboard-test")
+    pack.create_trigger("trigger-test")
     assert validator.validate_release_notes_headers()
 
 
 TEST_RELEASE_NOTES_INVALID_HEADERS = [
     (
         """#### Integrations
 ##### integration-test
@@ -744,20 +745,18 @@
         {
             "rn_valid_header_format": True,
             "validate_content_type_header": True,
             "validate_content_item_header": False,
         },
     ),
     (
-        """#### FakeContentType
-                                      ##### Test
-                                      - Added x y z""",
+        """#### FakeContentType\n##### Test\n- Added x y z""",
         "FakeContentType",
         {
-            "rn_valid_header_format": False,
+            "rn_valid_header_format": True,
             "validate_content_type_header": False,
             "validate_content_item_header": False,
         },
     ),
     (
         """#### Incident Fields
                                       ##### Test
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/reputation_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/reputation_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/script_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/script_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/structure_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/structure_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/invalid_correlation_rule.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/invalid_correlation_rule.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/rn_header_test_data` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/rn_header_test_data`

 * *Files 5% similar despite different names*

```diff
@@ -52,7 +52,10 @@
 - Added x y z
 
 #### XSIAM Dashboards
 ##### New: xsiam-dashboard-test.json
 - Added x y z
 - Ignore the json suffix, it is not a real dashboard.
 
+#### Triggers Recommendations
+- **trigger-test.json**
+
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/test_files/test_changelog.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/test_files/test_changelog.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/timers_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/timers_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/tools_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/tools_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/update_id_set_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/update_id_set_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/widget_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/widget_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/wizards_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/wizards_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tests/xsoar_config_file_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tests/xsoar_config_file_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/timers.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/timers.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,14 +58,15 @@
     METADATA_FILE_NAME,
     MODELING_RULES_DIR,
     NON_LETTERS_OR_NUMBERS_PATTERN,
     OFFICIAL_CONTENT_GRAPH_PATH,
     OFFICIAL_CONTENT_ID_SET_PATH,
     OFFICIAL_INDEX_JSON_PATH,
     PACK_METADATA_IRON_BANK_TAG,
+    PACK_METADATA_SUPPORT,
     PACKAGE_SUPPORTING_DIRECTORIES,
     PACKAGE_YML_FILE_REGEX,
     PACKS_DIR,
     PACKS_DIR_REGEX,
     PACKS_PACK_IGNORE_FILE_NAME,
     PACKS_PACK_META_FILE_NAME,
     PACKS_README_FILE_NAME,
@@ -84,14 +85,15 @@
     UNRELEASE_HEADER,
     UUID_REGEX,
     WIDGETS_DIR,
     XDRC_TEMPLATE_DIR,
     XSIAM_DASHBOARDS_DIR,
     XSIAM_REPORTS_DIR,
     XSOAR_CONFIG_FILE,
+    XSOAR_SUPPORT,
     FileType,
     IdSetKeys,
     MarketplaceVersions,
     urljoin,
 )
 from demisto_sdk.commands.common.git_content_config import GitContentConfig, GitProvider
 from demisto_sdk.commands.common.git_util import GitUtil
@@ -1345,22 +1347,24 @@
         if any(ignore_code == "auto-test" for ignore_code in ignore_list):
             test_id, test_pack = get_test_playbook_id(test_playbooks, file_name)
             if test_id:
                 ignored_tests_set.add(test_id)
     return ignored_tests_set
 
 
-def get_all_docker_images(script_obj) -> List[str]:
-    """Gets a yml as dict and returns a list of all 'dockerimage' values in the yml.
+def get_docker_images_from_yml(script_obj) -> List[str]:
+    """
+    Gets a yml as dict of the script/integration that lint runs on, and returns a list of all 'dockerimage' values
+    in the yml (including 'alt_dockerimages' if the key exist).
 
     Args:
-        script_obj (dict): A yml dict.
+        script_obj (dict): A yml as dict of the integration/script that lint runs on.
 
     Returns:
-        List. A list of all docker images.
+        (List): A list including all the docker images of the integration/script.
     """
     # this makes sure the first docker in the list is the main docker image.
     def_docker_image = DEF_DOCKER
     if script_obj.get("type") == TYPE_PWSH:
         def_docker_image = DEF_DOCKER_PWSH
     imgs = [script_obj.get("dockerimage") or def_docker_image]
 
@@ -1592,14 +1596,38 @@
 
     elif path.name == FileType.SECRET_IGNORE:
         return FileType.SECRET_IGNORE
 
     elif path.parent.name == DOC_FILES_DIR:
         return FileType.DOC_FILE
 
+    elif path.name.lower() == "pipfile":
+        return FileType.PIPFILE
+
+    elif path.name.lower() == "pipfile.lock":
+        return FileType.PIPFILE_LOCK
+
+    elif path.suffix.lower() == ".ini":
+        return FileType.INI
+
+    elif path.suffix.lower() == ".pem":
+        return FileType.PEM
+
+    elif (
+        path.name.lower()
+        in ("commands_example", "commands_examples", "command_examples")
+        or path.suffix.lower() == ".txt"
+    ):
+        return FileType.TXT
+    elif path.name == ".pylintrc":
+        return FileType.PYLINTRC
+
+    elif path.name == "LICENSE":
+        return FileType.LICENSE
+
     return None
 
 
 # flake8: noqa: C901
 
 
 def find_type(
@@ -1639,14 +1667,17 @@
         if ignore_invalid_schema_file:
             # invalid file schema
             logger.debug(str(err))
             return None
         raise err
 
     if file_type == "yml" or path.lower().endswith(".yml"):
+        if path.lower().endswith("_unified.yml"):
+            return FileType.UNIFIED_YML
+
         if "category" in _dict:
             if _dict.get("beta") and not ignore_sub_categories:
                 return FileType.BETA_INTEGRATION
 
             return FileType.INTEGRATION
 
         if "script" in _dict:
@@ -2249,14 +2280,17 @@
         the server version of the Demisto instance.
     """
     try:
         resp = client.generic_request("/about", "GET")
         about_data = json.loads(resp[0].replace("'", '"'))
         return parse(about_data.get("demistoVersion"))  # type: ignore
     except Exception:
+        logger.warning(
+            "Could not parse Xsoar version, please make sure the environment is properly configured."
+        )
         return parse("0")
 
 
 def arg_to_list(arg: Union[str, List[str]], separator: str = ",") -> List[str]:
     """
     Converts a string representation of lists to a python list
     Args:
@@ -2624,14 +2658,30 @@
         (bool):
         - True if the input path is for a given pack.
         - False if the input path is not for a given pack.
     """
     return os.path.basename(os.path.dirname(input_path)) == PACKS_DIR
 
 
+def is_xsoar_supported_pack(file_path: str) -> bool:
+
+    """
+    Takes a path to a file and returns a boolean indicating
+    whether this file belongs to an XSOAR-supported Pack.
+
+    Args:
+        - `file_path` (`str`): The path of the file.
+
+    Returns:
+        - `bool`
+    """
+
+    return get_pack_metadata(file_path).get(PACK_METADATA_SUPPORT) == XSOAR_SUPPORT
+
+
 def get_relative_path_from_packs_dir(file_path: str) -> str:
     """Get the relative path for a given file_path starting in the Packs directory"""
     if PACKS_DIR not in file_path or file_path.startswith(PACKS_DIR):
         return file_path
 
     return file_path[file_path.find(PACKS_DIR) :]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/common/update_id_set.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/common/update_id_set.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -71,14 +71,18 @@
 
     A comma-separated list of packs to update.
 
 * **-i, --imported_path**
 
     Path to content graph zip file to import.
 
+* **--use-current**
+
+    Whether to use the current content graph to update.
+
 * **-nd, --no-dependencies**
 
     Whether skip dependencies should be included in the graph.
 
 * **-v, --verbose**
 
     Verbosity level -v / -vv / .. / -vvv.
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/common.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/common.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/content_graph_builder.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/content_graph_builder.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/content_graph_commands.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/content_graph_commands.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import List, Optional
 
 import demisto_sdk.commands.content_graph.neo4j_service as neo4j_service
 from demisto_sdk.commands.common.constants import MarketplaceVersions
 from demisto_sdk.commands.common.git_util import GitUtil
-from demisto_sdk.commands.common.tools import (
-    download_content_graph,
-    get_latest_upload_flow_commit_hash,
-)
+from demisto_sdk.commands.common.tools import download_content_graph
 from demisto_sdk.commands.content_graph.content_graph_builder import ContentGraphBuilder
 from demisto_sdk.commands.content_graph.interface.graph import ContentGraphInterface
 
 logger = logging.getLogger("demisto-sdk")
 
 
 def create_content_graph(
@@ -39,62 +36,69 @@
 
 
 def update_content_graph(
     content_graph_interface: ContentGraphInterface,
     marketplace: MarketplaceVersions = MarketplaceVersions.XSOAR,
     use_git: bool = False,
     imported_path: Optional[Path] = None,
+    use_current: bool = False,
     packs_to_update: Optional[List[str]] = None,
     dependencies: bool = True,
     output_path: Optional[Path] = None,
 ) -> None:
     """This function creates a new content graph database in neo4j from the content path
     Args:
         content_graph_interface (ContentGraphInterface): The content graph interface.
         marketplace (MarketplaceVersions): The marketplace to update.
         use_git (bool): Whether to use git to get the packs to update.
         imported_path (Path): The path to the imported graph.
+        use_current (bool): Whether to use the current graph.
         packs_to_update (List[str]): The packs to update.
         dependencies (bool): Whether to create the dependencies.
         output_path (Path): The path to export the graph zip to.
     """
-    if use_git and imported_path:
-        raise ValueError("Cannot use both git and imported path")
-    if packs_to_update is None and not imported_path:
-        # If no arguments were given, we will use the git diff to get the packs to update
-        use_git = True
-
     if packs_to_update is None:
         packs_to_update = []
     builder = ContentGraphBuilder(content_graph_interface)
+    if not imported_path and not use_current:
+        # getting the graph from remote, so we need to clean the import dir
+        content_graph_interface.clean_import_dir()
+        extract_remote_import_files(content_graph_interface, builder)
+
+    if use_git and (commit := content_graph_interface.commit):
+        packs_to_update.extend(GitUtil().get_all_changed_pack_ids(commit))
+
+    content_graph_interface.import_graph(imported_path)
 
-    if use_git:
-        get_or_create_graph(content_graph_interface, builder)
-        latest_commit = get_latest_upload_flow_commit_hash()
-        packs_to_update.extend(GitUtil().get_all_changed_pack_ids(latest_commit))
-    else:
-        content_graph_interface.import_graph(imported_path)
     logger.info(f"Updating the following packs: {packs_to_update}")
     builder.update_graph(packs_to_update)
     if dependencies:
         content_graph_interface.create_pack_dependencies()
     if output_path:
         output_path = output_path / marketplace.value
     content_graph_interface.export_graph(output_path)
 
 
-def get_or_create_graph(
+def extract_remote_import_files(
     content_graph_interface: ContentGraphInterface, builder: ContentGraphBuilder
-):
+) -> None:
+    """Get or create a content graph.
+    If the graph is not in the bucket or there are network issues, it will create a new one.
+
+    Args:
+        content_graph_interface (ContentGraphInterface)
+        builder (ContentGraphBuilder)
+
+    """
     try:
         with NamedTemporaryFile() as temp_file:
             official_content_graph = download_content_graph(Path(temp_file.name))
-            content_graph_interface.import_graph(official_content_graph)
+            content_graph_interface.move_to_import_dir(official_content_graph)
     except Exception as e:
-        logger.info("Failed to download from bucket. Will create a new graph")
+        logger.warning("Failed to download from bucket. Will create a new graph")
         logger.debug(f"Error: {e}")
         builder.create_graph()
 
 
 def stop_content_graph() -> None:
     """
     This function stops the neo4j service if it is running.
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/architecture.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/architecture.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/models.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/models.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/images/parsers.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/images/parsers.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/import_utils.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/import_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,36 +3,42 @@
 import os
 import shutil
 from pathlib import Path
 from tempfile import NamedTemporaryFile
 from typing import List, Optional, Set
 from zipfile import ZipFile
 
+from demisto_sdk.commands.common.handlers import JSON_Handler
 from demisto_sdk.commands.content_graph.neo4j_service import get_neo4j_import_path
 
+json = JSON_Handler()
+
 logger = logging.getLogger("demisto-sdk")
 
 
 class Neo4jImportHandler:
-    def __init__(self, imported_path: Optional[Path] = None) -> None:
+    def __init__(self) -> None:
         """This class handles the import of data to neo4j.
         import_path is the path to the directory where the data is located.
 
 
         Args:
             imported_path (Optional[Path], optional): A zip file path to import the graph from. Defaults to None.
                                                       If not given, the graph will use the content in the `import_path` directory.
         """
         self.import_path: Path = get_neo4j_import_path()
+        self.import_path.mkdir(parents=True, exist_ok=True)
         logger.debug(f"Import path: {self.import_path}")
-        if imported_path:
-            self.clean_import_dir()
-            logger.info(f"Importing from {imported_path}")
-            with ZipFile(imported_path, "r") as zip_obj:
-                zip_obj.extractall(self.import_path)
+
+    def extract_files_from_path(self, imported_path: Optional[Path] = None) -> None:
+        if not imported_path:
+            return None
+        logger.info(f"Importing from {imported_path}")
+        with ZipFile(imported_path, "r") as zip_obj:
+            zip_obj.extractall(self.import_path)
 
     def clean_import_dir(self) -> None:
         for file in self.import_path.iterdir():
             os.remove(file)
 
     def get_nodes_files(self) -> List[str]:
         return [
@@ -84,10 +90,7 @@
                             if "relationships" in filename.name
                             else row[1]
                         )
                         writer.writerow(row)
                 shutil.move(
                     tempfile.name, (self.import_path / filename.name).as_posix()
                 )
-
-    def zip_import_dir(self, output_file: Path) -> None:
-        shutil.make_archive(str(output_file), "zip", self.import_path)
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/neo4j_graph.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/neo4j_graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,14 +91,15 @@
     pass
 
 
 class Neo4jContentGraphInterface(ContentGraphInterface):
 
     # this is used to save cache of packs and integrations which queried
     _id_to_obj: Dict[int, BaseContent] = {}
+    _import_handler = Neo4jImportHandler()
 
     def __init__(
         self,
     ) -> None:
         self.driver: Neo4jDriver = GraphDatabase.driver(
             NEO4J_DATABASE_URL,
             auth=(NEO4J_USERNAME, NEO4J_PASSWORD),
@@ -108,14 +109,24 @@
         if not neo4j_service.is_alive():
             neo4j_service.start()
         return self
 
     def __exit__(self, *args) -> None:
         self.driver.close()
 
+    @property
+    def import_path(self) -> Path:
+        return self._import_handler.import_path
+
+    def clean_import_dir(self) -> None:
+        return self._import_handler.clean_import_dir()
+
+    def move_to_import_dir(self, imported_path: Path) -> None:
+        return self._import_handler.extract_files_from_path(imported_path)
+
     def close(self) -> None:
         self.driver.close()
 
     def _add_relationships_to_objects(
         self,
         session: Session,
         result: Dict[int, Neo4jRelationshipResult],
@@ -323,36 +334,36 @@
         4. Merging duplicate nodes (conmmands/content items)
         5. Recreating the constraints
 
         Args:
             external_import_paths (List[Path]): A list of external repositories' import paths.
             imported_path (Path): The path to import the graph from.
         """
-        import_handler = Neo4jImportHandler(imported_path)
-        import_handler.ensure_data_uniqueness()
-        node_files = import_handler.get_nodes_files()
-        relationship_files = import_handler.get_relationships_files()
+        self._import_handler.extract_files_from_path(imported_path)
+        self._import_handler.ensure_data_uniqueness()
+        node_files = self._import_handler.get_nodes_files()
+        relationship_files = self._import_handler.get_relationships_files()
         with self.driver.session() as session:
             session.write_transaction(drop_constraints)
             session.write_transaction(import_csv, node_files, relationship_files)
             session.write_transaction(post_import_write_queries)
             session.write_transaction(merge_duplicate_commands)
             session.write_transaction(merge_duplicate_content_items)
             session.write_transaction(create_constraints)
             session.write_transaction(remove_empty_properties)
 
     def export_graph(self, output_path: Optional[Path] = None) -> None:
-        import_handler = Neo4jImportHandler()
-        import_handler.clean_import_dir()
+        self.clean_import_dir()
         with self.driver.session() as session:
             session.write_transaction(pre_export_write_queries)
             session.write_transaction(export_to_csv, self.repo_path.name)
             session.write_transaction(post_export_write_queries)
+        self.dump_metadata()
         if output_path:
-            import_handler.zip_import_dir(output_path)
+            self.zip_import_dir(output_path)
 
     def clean_graph(self):
         with self.driver.session() as session:
             session.write_transaction(delete_all_graph_nodes)
         Neo4jContentGraphInterface._id_to_obj = {}
         super().clean_graph()
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/common.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/common.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/constraints.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/constraints.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/dependencies.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/dependencies.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,18 +223,21 @@
     query = f"""
         MATCH (pack_a:{ContentType.BASE_CONTENT})<-[:{RelationshipType.IN_PACK}]-(a)
             -[r:{RelationshipType.USES}]->(b)-[:{RelationshipType.IN_PACK}]->(pack_b:{ContentType.BASE_CONTENT})
         WHERE ANY(marketplace IN pack_a.marketplaces WHERE marketplace IN pack_b.marketplaces)
         AND id(pack_a) <> id(pack_b)
         AND NOT pack_a.name IN {IGNORED_PACKS_IN_DEPENDENCY_CALC}
         AND NOT pack_b.name IN {IGNORED_PACKS_IN_DEPENDENCY_CALC}
-        AND a.is_test <> true
-        AND b.is_test <> true
         WITH pack_a, a, r, b, pack_b
-        MERGE (pack_a)-[dep:DEPENDS_ON]->(pack_b)
+        MERGE (pack_a)-[dep:{RelationshipType.DEPENDS_ON}]->(pack_b)
+        ON CREATE
+            SET dep.is_test = a.is_test
+        ON MATCH
+            SET dep.is_test = dep.is_test AND a.is_test
+
         WITH dep, pack_a, a, r, b, pack_b, REDUCE(
             marketplaces = [], mp IN pack_a.marketplaces |
             CASE WHEN mp IN pack_b.marketplaces THEN marketplaces + mp ELSE marketplaces END
         ) AS common_marketplaces
         SET dep.marketplaces = common_marketplaces,
             dep.mandatorily = r.mandatorily OR dep.mandatorily
         WITH
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/import_export.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/import_export.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/indexes.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/indexes.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/nodes.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/nodes.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/interface/neo4j/queries/relationships.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/interface/neo4j/queries/relationships.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/neo4j_service.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/neo4j_service.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/__init__.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/base_content.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/base_content.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/content_item.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/content_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,17 @@
 
 from pydantic import DirectoryPath, validator
 
 from demisto_sdk.commands.common.constants import MarketplaceVersions
 from demisto_sdk.commands.common.tools import get_content_path
 from demisto_sdk.commands.content_graph.common import ContentType, RelationshipType
 from demisto_sdk.commands.content_graph.objects.base_content import BaseContent
-
-# from demisto_sdk.commands.prepare_content.preparers.marketplace_suffix_preparer import MarketplaceSuffixPreparer
+from demisto_sdk.commands.prepare_content.preparers.marketplace_suffix_preparer import (
+    MarketplaceSuffixPreparer,
+)
 
 logger = logging.getLogger("demisto-sdk")
 
 
 class ContentItem(BaseContent):
     path: Path
     marketplaces: List[MarketplaceVersions]
@@ -98,27 +99,31 @@
             r.content_item  # type: ignore[misc]
             for r in self.relationships_data[RelationshipType.TESTED_BY]
             if r.content_item == r.target
         ]
 
     @property
     def handler(self) -> XSOAR_Handler:
-        return JSON_Handler() if self.path.suffix.lower() == ".json" else YAML_Handler()
+        # we use a high value so the code lines will not break
+        return (
+            JSON_Handler()
+            if self.path.suffix.lower() == ".json"
+            else YAML_Handler(50_000)
+        )
 
     @property
     def data(self) -> dict:
         with self.path.open() as f:
             return self.handler.load(f)
 
     def prepare_for_upload(
         self, marketplace: MarketplaceVersions = MarketplaceVersions.XSOAR, **kwargs
     ) -> dict:
         data = self.data
-        # data = MarketplaceSuffixPreparer.prepare(data, marketplace)
-        return data
+        return MarketplaceSuffixPreparer.prepare(data, marketplace)
 
     def summary(self, marketplace: Optional[MarketplaceVersions] = None) -> dict:
         """Summary of a content item (the most important metadata fields)
 
         Args:
             marketplace: The marketplace to get the summary for.
         Returns:
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/content_item_xsiam.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/content_item_xsiam.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/generic_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/generic_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/incident_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/incident_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/incident_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/incident_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/indicator_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/indicator_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/indicator_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/indicator_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/integration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/integration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/integration_script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/integration_script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/mapper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/mapper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/modeling_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/modeling_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/pack.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/pack.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 from packaging.version import parse
 from pydantic import BaseModel, Field, validator
 
 from demisto_sdk.commands.common.constants import (
     BASE_PACK,
     CONTRIBUTORS_README_TEMPLATE,
+    MARKETPLACE_MIN_VERSION,
     MarketplaceVersions,
 )
 from demisto_sdk.commands.common.handlers import JSON_Handler
 from demisto_sdk.commands.common.tools import MarketplaceTagParser, get_content_path
 from demisto_sdk.commands.content_graph.common import (
     PACK_METADATA_FILENAME,
     ContentType,
@@ -196,17 +197,20 @@
             if r.content_item == r.source
         ]
         content_item_dct = defaultdict(list)
         for c in content_items:
             content_item_dct[c.content_type.value].append(c)
 
         # If there is no server_min_version, set it to the maximum of its content items fromversion
-        self.server_min_version = self.server_min_version or str(
-            max(parse(content_item.fromversion) for content_item in content_items)
-        )
+        max_content_items_version = MARKETPLACE_MIN_VERSION
+        if content_items:
+            max_content_items_version = str(
+                max(parse(content_item.fromversion) for content_item in content_items)
+            )
+        self.server_min_version = self.server_min_version or max_content_items_version
         self.content_items = PackContentItems(**content_item_dct)
 
     def dump_metadata(self, path: Path, marketplace: MarketplaceVersions) -> None:
         metadata = self.dict(exclude={"path", "node_id", "content_type"})
         metadata["contentItems"] = {}
         for content_item in self.content_items:
             try:
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/parsing_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/parsing_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/relationship.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/relationship.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,14 +15,17 @@
     content_item: BaseContent
 
     is_direct: bool = True
 
     # USES, DEPENDS_ON relationship properties
     mandatorily: bool = False
 
+    # DEPENDS_ON relationship properties
+    is_test: bool = False
+
     # HAS_COMMAND relationship properties
     description: Optional[str] = None
     deprecated: bool = False
 
     def __hash__(self):
         """This is the unique identifier of the relationship"""
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/repository.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/repository.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/script.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from typing import List, Set
 
 from demisto_sdk.commands.common.constants import MarketplaceVersions
-from demisto_sdk.commands.content_graph.common import ContentType
+from demisto_sdk.commands.content_graph.common import ContentType, RelationshipType
+from demisto_sdk.commands.content_graph.objects.base_content import BaseContent
 from demisto_sdk.commands.content_graph.objects.integration_script import (
     IntegrationScript,
 )
 
 logger = logging.getLogger("demisto-sdk")
 
 
@@ -27,7 +28,15 @@
         ):
             logger.debug(
                 f"Adding the following native images {supported_native_images} to script {self.object_id}"
             )
             data["nativeimage"] = supported_native_images
 
         return data
+
+    @property
+    def imported_by(self) -> List[BaseContent]:
+        return [
+            r.content_item
+            for r in self.relationships_data[RelationshipType.IMPORTS]
+            if r.content_item == r.source
+        ]
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/xdrc_template.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/xdrc_template.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/objects/xsiam_dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/objects/xsiam_dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/__init__.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/base_content.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/base_content.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/classifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/classifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/content_item.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/content_item.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/content_items_list.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/content_items_list.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/correlation_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/correlation_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_definition.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_definition.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_module.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_module.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/generic_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/generic_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/incident_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/incident_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/incident_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/incident_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/indicator_field.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/indicator_field.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/indicator_type.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/indicator_type.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/integration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/integration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/integration_script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/integration_script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/job.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/job.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/json_content_item.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/json_content_item.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/layout.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/layout.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/list.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/list.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/mapper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/mapper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/modeling_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/modeling_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/pack.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/pack.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/parsing_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/parsing_rule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/repository.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/repository.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/test_playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/test_playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/trigger.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/trigger.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/widget.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/widget.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/wizard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/wizard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xdrc_template.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xdrc_template.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xsiam_dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xsiam_dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/xsiam_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/xsiam_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/parsers/yaml_content_item.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/parsers/yaml_content_item.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/create_content_graph_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/create_content_graph_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -290,14 +290,20 @@
             mock_relationship(
                 "TestApiModule",
                 ContentType.SCRIPT,
                 "SampleScript2",
                 ContentType.SCRIPT,
                 mandatorily=True,
             ),
+            mock_relationship(
+                "SampleTestPlaybook",
+                ContentType.TEST_PLAYBOOK,
+                "SampleIntegration",
+                ContentType.INTEGRATION,
+            ),
         ],
     }
     relationship_pack3 = {
         RelationshipType.IN_PACK: [
             mock_relationship(
                 "SamplePlaybook",
                 ContentType.PLAYBOOK,
@@ -406,15 +412,18 @@
         # make sure that the output file zip is created
         assert Path.exists(tmp_path / "xsoar.zip")
         with ZipFile(tmp_path / "xsoar.zip", "r") as zip_obj:
             zip_obj.extractall(tmp_path / "extracted")
             # make sure that the extracted files are all .csv
             extracted_files = list(tmp_path.glob("extracted/*"))
             assert extracted_files
-            assert all(file.suffix == ".csv" for file in extracted_files)
+            assert all(
+                file.suffix == ".csv" or file.name == "metadata.json"
+                for file in extracted_files
+            )
 
     def test_create_content_graph_relationships(
         self,
         repository: ContentDTO,
     ):
         """
         Given:
@@ -462,16 +471,28 @@
                                 == content_item_target.object_id
                             )
                         if relationship_type == RelationshipType.TESTED_BY:
                             assert (
                                 content_item_source.tested_by[0].object_id
                                 == content_item_target.object_id
                             )
+
             assert packs[0].depends_on[0].content_item == packs[1]
-            assert packs[1].depends_on[0].content_item == packs[2]
+            assert not packs[0].depends_on[0].is_test  # this is not a test dependency
+
+            for p in packs[1].depends_on:
+                if p.content_item == packs[2]:
+                    # regular dependency
+                    assert not p.is_test
+                elif p.content_item == packs[0]:
+                    # test dependency
+                    assert p.is_test
+                else:
+
+                    assert False
 
             # now with all levels
             packs = interface.search(
                 MarketplaceVersions.XSOAR,
                 content_type=ContentType.PACK,
                 all_level_dependencies=True,
             )
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/neo4j_interface_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/neo4j_interface_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/parsers_and_models_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/parsers_and_models_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/classifier.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/classifier.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/dashboard.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/dashboard.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/generic_module.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/generic_module.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/incident_field.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/incident_field.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/incoming_mapper.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/incoming_mapper.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/indicator_field.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/indicator_field.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/indicator_type.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/indicator_type.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/layout_old.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/layout_old.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/layoutscontainer.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/layoutscontainer.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/list.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/list.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/outgoing_mapper.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/outgoing_mapper.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata2.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/pack_metadata2.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/parsing_rule.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/parsing_rule.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/report.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/report.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/trigger.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/trigger.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/unified_integration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/unified_integration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/widget.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/widget.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/wizard.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/wizard.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_data/xsiam_dashboard.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_data/xsiam_dashboard.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/test_tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/content_graph/tests/update_content_graph_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/content_graph/tests/update_content_graph_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-import shutil
-from distutils.dir_util import copy_tree
 from pathlib import Path
 from typing import Any, Callable, Dict, List
 from zipfile import ZipFile
 
 import pytest
 
 import demisto_sdk.commands.content_graph.neo4j_service as neo4j_service
@@ -203,21 +201,14 @@
 def _get_pack_by_id(repository: ContentDTO, pack_id: str) -> Pack:
     for pack in repository.packs:
         if pack.object_id == pack_id:
             return pack
     raise ValueError(f"Pack {pack_id} does not exist in the repository.")
 
 
-def dump_csv_import_files(csv_files_dir: Path) -> None:
-    import_path = neo4j_service.get_neo4j_import_path().as_posix()
-    if Path(import_path).is_dir():
-        shutil.rmtree(import_path)
-        copy_tree(csv_files_dir.as_posix(), import_path)
-
-
 # COMPARISON HELPER FUNCTIONS
 
 
 def compare(
     packs_from_content_dto: List[Pack],
     packs_from_graph: List[Pack],
     expected_added_dependencies: List[Dict[str, Any]],
@@ -384,18 +375,21 @@
                 interface.search(
                     marketplace=MarketplaceVersions.XSOAR,
                     content_type=content_type,
                 )
             )
 
         with ContentGraphInterface() as interface:
-            dump_csv_import_files(
-                TEST_DATA_PATH / "mock_import_files_multiple_repos__valid"
+            update_content_graph(
+                interface,
+                packs_to_update=[],
+                imported_path=TEST_DATA_PATH
+                / "mock_import_files_multiple_repos__valid"
+                / "valid_graph.zip",
             )
-            update_content_graph(interface, packs_to_update=[])
             assert get_nodes_count_by_type(interface, ContentType.PACK) == 2
             assert get_nodes_count_by_type(interface, ContentType.INTEGRATION) == 2
             assert get_nodes_count_by_type(interface, ContentType.COMMAND) == 1
             assert get_nodes_count_by_type(interface, ContentType.CLASSIFIER) == 1
 
     @pytest.mark.parametrize(
         "commit_func, expected_added_dependencies, expected_removed_dependencies",
@@ -461,14 +455,15 @@
 
             # update the graph accordingly
             update_content_graph(
                 interface,
                 packs_to_update=pack_ids_to_update,
                 dependencies=True,
                 output_path=tmp_path,
+                use_current=True,
             )
             packs_from_graph = interface.search(
                 marketplace=MarketplaceVersions.XSOAR,
                 content_type=ContentType.PACK,
                 all_level_dependencies=True,
             )
             compare(
@@ -481,8 +476,11 @@
         # make sure that the output file zip is created
         assert Path.exists(tmp_path / "xsoar.zip")
         with ZipFile(tmp_path / "xsoar.zip", "r") as zip_obj:
             zip_obj.extractall(tmp_path / "extracted")
             # make sure that the extracted files are all .csv
             extracted_files = list(tmp_path.glob("extracted/*"))
             assert extracted_files
-            assert all(file.suffix == ".csv" for file in extracted_files)
+            assert all(
+                file.suffix == ".csv" or file.name == "metadata.json"
+                for file in extracted_files
+            )
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/convert_manager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/convert_manager.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/base_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/base_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/classifier_6_0_0_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/classifier_6_0_0_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/classifier_base_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/classifier_base_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/classifier_6_0_0_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/classifier_6_0_0_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/classifier_base_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/classifier_base_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate_5_9_9.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-Cymulate_5_9_9.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-mapper-incoming-Cymulate.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/classifier/tests/test_data/classifier-mapper-incoming-Cymulate.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_6_0_0_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_6_0_0_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_base_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_base_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/layout_up_to_5_9_9_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/layout_up_to_5_9_9_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_6_0_0_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_6_0_0_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_base_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_base_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/layout_up_to_5_9_9_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/layout_up_to_5_9_9_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-close-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-close-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-details-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-details-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-edit-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-edit-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-indicatorsDetails-Cryptocurrency_Address-V3.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-indicatorsDetails-Cryptocurrency_Address-V3.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-mobile-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-mobile-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-quickView-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout-quickView-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout_up_to_5_9_9_expected_convert_dir_test_file_output.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layout_up_to_5_9_9_expected_convert_dir_test_file_output.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/layoutscontainer-ExtraHop_Detection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/layoutscontainer-ExtraHop_Detection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/layout/tests/test_data/reputation-cryptocurrency.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/layout/tests/test_data/reputation-cryptocurrency.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/converters/tests/base_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/converters/tests/base_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/dir_convert_managers.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/dir_convert_managers.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/convert/tests/convert_manager_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/convert/tests/convert_manager_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/coverage_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/coverage_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/helpers.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/helpers.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/coverage_report_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/coverage_report_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/HealthCheckAnalyzeLargeInvestigations_py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/HealthCheckAnalyzeLargeInvestigations_py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage-min.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage-min.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage.txt` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage.txt`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/HealthCheckAnalyzeLargeInvestigations` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/HealthCheckAnalyzeLargeInvestigations`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/Vertica` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/Vertica`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotalV3` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotalV3`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotal_V3_Premium` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/data/coverage_data_files/VirusTotal_V3_Premium`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/helpers_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/helpers_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tests/tools_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tests/tools_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/coverage_analyze/tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/coverage_analyze/tools.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/artifacts_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/artifacts_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/content_artifacts_creator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/content_artifacts_creator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/content_artifacts_creator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/content_artifacts_creator_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 from contextlib import contextmanager
 from filecmp import dircmp
 from pathlib import Path
 from shutil import copyfile, copytree, rmtree
+from typing import List
 
 import pytest
 
-from demisto_sdk.commands.common.constants import PACKS_DIR, TEST_PLAYBOOKS_DIR
+from demisto_sdk.commands.common.constants import (
+    PACKS_DIR,
+    TEST_PLAYBOOKS_DIR,
+    MarketplaceVersions,
+)
 from demisto_sdk.commands.common.handlers import JSON_Handler, YAML_Handler
 from demisto_sdk.commands.common.logger import logging_setup
 from demisto_sdk.commands.common.tools import src_root
-
-# from demisto_sdk.commands.prepare_content.prepare_upload_manager import PrepareUploadManager
+from demisto_sdk.commands.prepare_content.prepare_upload_manager import (
+    PrepareUploadManager,
+)
 from TestSuite.test_tools import ChangeCWD
 
 json = JSON_Handler()
 
 
 TEST_DATA = src_root() / "tests" / "test_files"
 TEST_CONTENT_REPO = TEST_DATA / "content_slim"
@@ -423,34 +429,48 @@
         if key in rv:
             rv = rv[key]
         else:
             raise Exception(f"Value {path} not found in object")
     return rv
 
 
-# @pytest.mark.parametrize(argnames="artifact, keys_paths",
-#                          argvalues=[
-#                              ('demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/'
-#                               'DummyPackAlternativeFields/IncidentFields/incidentfield-sample_packs.json',
-#                               ['name']),
-#                              ('demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/'
-#                               'DummyPackAlternativeFields/Integrations/integration-sample_packs.yml',
-#                               ['name']),
-#                              ('demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/'
-#                               'DummyPackAlternativeFields/Playbooks/playbook-sample_packs.yml',
-#                               ['name', 'tasks.task_num.task.scriptName']
-#                               ),
-#                              ('demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/'
-#                               'DummyPackAlternativeFields/Scripts/script-sample_packs.yml',
-#                               ['commonfields.id', 'name', 'comment']
-#                               )
-#                          ])
-# def test_use_alternative_fields(artifact: str, keys_paths: List[str]):
-#     with temp_dir() as temp:
-#         PrepareUploadManager.prepare_for_upload(artifact, output=temp, marketplace=MarketplaceVersions.MarketplaceV2,
-#                                                 force=True,
-#                                                 )
-#         filename = artifact.split('/')[-1]
-#         original_data = load_file(artifact)
-#         modified_data = load_file(temp / filename)
-#         for current_key_path in keys_paths:
-#             assert get_value_from_dict(original_data, current_key_path + '_x2') == get_value_from_dict(modified_data, current_key_path)
+@pytest.mark.parametrize(
+    argnames="artifact, keys_paths",
+    argvalues=[
+        (
+            "demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/"
+            "DummyPackAlternativeFields/IncidentFields/incidentfield-sample_packs.json",
+            ["name"],
+        ),
+        (
+            "demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/"
+            "DummyPackAlternativeFields/Integrations/integration-sample_packs.yml",
+            ["name"],
+        ),
+        (
+            "demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/"
+            "DummyPackAlternativeFields/Playbooks/playbook-sample_packs.yml",
+            ["name", "tasks.task_num.task.scriptName"],
+        ),
+        (
+            "demisto_sdk/tests/test_files/content_repo_with_alternative_fields/Packs/"
+            "DummyPackAlternativeFields/Scripts/script-sample_packs.yml",
+            ["commonfields.id", "name", "comment"],
+        ),
+    ],
+)
+def test_use_alternative_fields(artifact: str, keys_paths: List[str]):
+    filename = artifact.split("/")[-1]
+    with temp_dir() as temp:
+        output_file = temp / filename
+        PrepareUploadManager.prepare_for_upload(
+            artifact,
+            output=output_file,
+            marketplace=MarketplaceVersions.MarketplaceV2,
+            force=True,
+        )
+        original_data = load_file(artifact)
+        modified_data = load_file(output_file)
+        for current_key_path in keys_paths:
+            assert get_value_from_dict(
+                original_data, current_key_path + "_x2"
+            ) == get_value_from_dict(modified_data, current_key_path)
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/id_set_alrenative_fields.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/id_set_alrenative_fields.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_artifacts/tests/data/id_set_missing_packs_and_items.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_artifacts/tests/data/id_set_missing_packs_and_items.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/create_id_set.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/create_id_set.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/create_id_set_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/create_id_set_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/classifier-mapper-to-test.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test-no-types_scripts.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test-no-types_scripts.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/incidentfield-to-test.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test-no-types-fields.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test-no-types-fields.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layout-to-test.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/layoutscontainer-to-test.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/layoutscontainer-to-test.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/playbook-no-incident-fields.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/playbook-no-incident-fields.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/playbook-with-incident-fields.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/playbook-with-incident-fields.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype_no_script_no_integration.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/reputation-indicatortype_no_script_no_integration.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/widget-no-scripts.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/widget-no-scripts.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/create_id_set/tests/test_data/widget-with-scripts.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/create_id_set/tests/test_data/widget-with-scripts.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/doc_reviewer.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/doc_reviewer.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,19 @@
     path_to_pack_object,
 )
 from demisto_sdk.commands.common.content.objects.abstract_objects import TextObject
 from demisto_sdk.commands.common.content.objects.pack_objects.abstract_pack_objects.yaml_content_object import (
     YAMLContentObject,
 )
 from demisto_sdk.commands.common.git_util import GitUtil
-from demisto_sdk.commands.common.tools import add_default_pack_known_words, find_type
+from demisto_sdk.commands.common.tools import (
+    add_default_pack_known_words,
+    find_type,
+    is_xsoar_supported_pack,
+)
 from demisto_sdk.commands.doc_reviewer.known_words import KNOWN_WORDS
 from demisto_sdk.commands.doc_reviewer.rn_checker import ReleaseNotesChecker
 
 
 class DocReviewer:
     """Perform a spell check on the given .yml or .md file."""
 
@@ -53,14 +57,15 @@
         no_camel_case: bool = False,
         no_failure: bool = False,
         expand_dictionary: bool = False,
         templates: bool = False,
         use_git: bool = False,
         prev_ver: str = None,
         release_notes_only: bool = False,
+        xsoar_only: bool = False,
         load_known_words_from_pack: bool = False,
     ):
         if templates:
             ReleaseNotesChecker(template_examples=True)
             sys.exit(0)
 
         # if nothing entered will default to use git
@@ -85,16 +90,17 @@
 
         self.known_words_file_paths = (
             known_words_file_paths if known_words_file_paths else []
         )
         self.load_known_words_from_pack = load_known_words_from_pack
         self.known_pack_words_file_path = ""
 
+        self.is_xsoar_supported_rn_only: bool = xsoar_only
         self.current_pack = None
-        self.files: list = []
+        self.files: List[str] = []
         self.spellchecker = SpellChecker()
         self.unknown_words: dict = {}
         self.no_camel_case = no_camel_case
         self.found_misspelled = False
         self.no_failure = no_failure
         self.expand_dictionary = expand_dictionary
         self.files_with_misspells: set = set()
@@ -291,14 +297,23 @@
             click.secho("Could not find any relevant files - Aborting.")
             return True
 
         self.add_known_words()
 
         for file in self.files:
             click.echo(f"\nChecking file {file}")
+
+            # --xsoar-only flag is specified.
+            if self.is_xsoar_supported_rn_only and not is_xsoar_supported_pack(file):
+                click.secho(
+                    f"File '{file}' was skipped because it does not belong to an XSOAR-supported Pack",
+                    fg="yellow",
+                )
+                continue
+
             restarted_spellchecker = self.update_known_words_from_pack(file)
             if restarted_spellchecker:
                 self.add_known_words()
             self.unknown_words = {}
             if file.endswith(".md"):
                 self.check_md_file(file)
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/rn_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/rn_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/tests/doc_reviewer_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/tests/doc_reviewer_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 import os
+import re
+from enum import Enum
 from os import path
 from pathlib import Path
 from typing import List
 
 import pytest
+from click.testing import CliRunner, Result
 
+from demisto_sdk import __main__
 from demisto_sdk.commands.common.constants import FileType
-from demisto_sdk.commands.common.tools import find_type, get_yaml
+from demisto_sdk.commands.common.tools import (
+    find_type,
+    get_yaml,
+    is_xsoar_supported_pack,
+)
 from demisto_sdk.commands.doc_reviewer.doc_reviewer import DocReviewer
 from demisto_sdk.tests.integration_tests.validate_integration_test import (
     AZURE_FEED_PACK_PATH,
 )
 from TestSuite.json_based import JSONBased
+from TestSuite.pack import Pack
 from TestSuite.test_tools import ChangeCWD
 
 
 class TestDocReviewFilesAreFound:
     """
     Tests scenarios in which files are found before performing doc-review.
     """
@@ -307,23 +316,186 @@
         doc_reviewer = DocReviewer(file_paths=[pack.path])
         result = doc_reviewer.run_doc_review()
         assert rn.path in doc_reviewer.malformed_rn_files
         assert not doc_reviewer.found_misspelled
         assert not result
 
 
+class TestDocReviewXSOAROnly:
+
+    """
+    Tests for the `--xsoar-only` flag.
+    """
+
+    default_args = ["--xsoar-only"]
+
+    class CommandResultCode(Enum):
+
+        """
+        Holds result code for the execution of `doc-review` command.
+        """
+
+        SUCCESS = 0
+        FAIL = 1
+
+    def run_doc_review_cmd(self, cmd_args: List[str]) -> Result:
+
+        """
+        Uses the Click CLI runner to invoke a command with input arguments and returns the result
+        """
+
+        args: List[str] = self.default_args + cmd_args
+
+        return CliRunner().invoke(__main__.doc_review, args)
+
+    def test_valid_supported_pack(self, supported_pack: Pack):
+
+        """
+        Given -
+            An XSOAR-supported Pack with correct spelling.
+
+        When -
+            Running `doc-review` on XSOAR-supported Pack with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` succeeds.
+        """
+
+        cmd_args: List[str] = [
+            "--input",
+            supported_pack.path,
+        ]
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.SUCCESS.value
+
+    def test_valid_non_supported_pack(self, non_supported_pack: Pack):
+
+        """
+        Given -
+            A non-XSOAR-supported Pack with correct spelling.
+
+        When -
+            Running `doc-review` on a non-XSOAR-supported Pack with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` succeeds.
+        """
+
+        cmd_args: List[str] = [
+            "--input",
+            non_supported_pack.path,
+        ]
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.SUCCESS.value
+
+    def test_valid_multiple_supported_packs(self, supported_packs: List[Pack]):
+
+        """
+        Given -
+            2 XSOAR-supported Packs with correct spelling.
+
+        When -
+            Running `doc-review` on XSOAR-supported Pack with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` succeeds.
+        """
+
+        cmd_args: List[str] = ["--xsoar-only"]
+        for pack in supported_packs:
+            cmd_args.append("--input")
+            cmd_args.append(pack.path)
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.SUCCESS.value
+
+    def test_invalid_non_supported_pack(self, non_supported_pack_mispelled: Pack):
+
+        """
+        Given -
+            A non-XSOAR-supported Pack with incorrect spelling.
+
+        When -
+            Running `doc-review` on a non-XSOAR-supported Pack with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` succeeds.
+        """
+
+        cmd_args: List[str] = [
+            "--input",
+            non_supported_pack_mispelled.path,
+        ]
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.SUCCESS.value
+
+    def test_invalid_supported_pack(self, supported_pack_mispelled: Pack):
+
+        """
+        Given -
+            A XSOAR-supported Pack with incorrect spelling.
+
+        When -
+            Running `doc-review` on a non-XSOAR-supported Pack with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` succeeds.
+        """
+
+        cmd_args: List[str] = [
+            "--input",
+            supported_pack_mispelled.path,
+        ]
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.FAIL.value
+
+    def test_invalid_mix_packs(self, mix_invalid_packs: List[Pack]):
+
+        """
+        Given -
+            2 Packs, one community, one XSOAR-supported with incorrect spelling.
+
+        When -
+            Running `doc-review` on both Packs with `--xsoar-only` flag set.
+
+        Then -
+            Ensure `doc-review` fails.
+        """
+
+        cmd_args: List[str] = ["--xsoar-only"]
+        for pack in mix_invalid_packs:
+            cmd_args.append("--input")
+            cmd_args.append(pack.path)
+
+        result = self.run_doc_review_cmd(cmd_args)
+
+        assert result.exit_code == self.CommandResultCode.FAIL.value
+
+
 @pytest.mark.usefixtures("are_mock_calls_supported_in_python_version")
 class TestDocReviewPrinting:
     """
     Test scenarios of doc-review printing.
     """
 
     MOCKED_FILES = ["file1", "file2"]
     GREEN_FG = {"fg": "green"}
     BRIGHT_RED_FG = {"fg": "bright_red"}
+    README_SKIPPED_REGEX = r"^File '.*/README.md' was skipped because it does not belong to an XSOAR-supported Pack"
+    RN_SKIPPED_REGEX = r"^File '.*/ReleaseNotes/.*.md' was skipped because it does not belong to an XSOAR-supported Pack"
+    FILE_MISSPELL_FOUND_REGEX = r"Words that might be misspelled were found in .*:"
 
     class SpelledFileType:
         """
         INVALID = invalid spelled files.
         VALID - valid spelled files.
         BOTH_INVALID_AND_VALID - both invalid spelled files and valid spelled files are required.
         INVALID_RELEASE_NOTES - invalid release-notes files.
@@ -467,14 +639,58 @@
         assert "Files With Misspells" in third_call.args[0]
         assert third_call.kwargs == self.BRIGHT_RED_FG
 
         forth_call = secho_mocker.mock_calls[3]
         assert "file1\nfile2" in forth_call.args[0]
         assert forth_call.kwargs == self.BRIGHT_RED_FG
 
+    def test_printing_skip_non_xsoar_supported_file(
+        self, mix_invalid_packs: List[Pack], mocker
+    ):
+        """
+        Given:
+            - A list of Packs (1 XSOAR-supported and 1 community-supported).
+
+        When -
+            Printing doc review report.
+
+        Then:
+            - Ensure that misspelled file in XSOAR-supported Pack is printed in report.
+            - Ensure that misspelled file in community-supported Pack is skipped in report
+        """
+
+        t = TestDocReviewXSOAROnly()
+
+        cmd_args: List[str] = []
+        for pack in mix_invalid_packs:
+            cmd_args.append("--input")
+            cmd_args.append(pack.path)
+
+            if is_xsoar_supported_pack(pack.path):
+                expected_supported = (
+                    f"Words that might be misspelled were found in {pack.path}"
+                )
+            else:
+                expected_not_supported_readme = f"File '{pack.readme.path}' was skipped because it does not belong to an XSOAR-supported Pack"
+                expected_not_supported_rn = f"File '{pack.release_notes[0].path}' was skipped because it does not belong to an XSOAR-supported Pack"
+
+        doc_review_report = t.run_doc_review_cmd(cmd_args)
+
+        report_output_lines = doc_review_report.output.splitlines()
+
+        for line in report_output_lines:
+            if re.match(self.README_SKIPPED_REGEX, line):
+                assert expected_not_supported_readme == line
+
+            if re.match(self.RN_SKIPPED_REGEX, line):
+                assert expected_not_supported_rn == line
+
+            if re.match(self.FILE_MISSPELL_FOUND_REGEX, line):
+                assert expected_supported == line
+
 
 WORDS = [
     ("invalidd", True, False),
     ("wordd", True, False),
     ("bizzaree", True, False),
     ("Heloo", True, False),
     ("tellllllllll", True, False),
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/doc_reviewer/tests/rn_checker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/doc_reviewer/tests/rn_checker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/downloader.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/downloader.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/downloader_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/downloader_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-DummyJSIntegration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-DummyJSIntegration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-Test_Integration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/integration-Test_Integration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/layout-details-TestLayout.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/layout-details-TestLayout.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_data/custom_content/playbook-DummyPlaybook.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_data/custom_content/playbook-DummyPlaybook.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/integration-Test_Integration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/integration-Test_Integration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/layout-details-TestLayout.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/layout-details-TestLayout.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/playbook-DummyPlaybook.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_data/custom_content/playbook-DummyPlaybook.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Integrations/TestIntegration/TestIntegration_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Layouts/layout-details-TestLayout.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/download/tests_backup/tests_env/content/Packs/TestPack/Playbooks/playbook-DummyPlaybook.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/error_code_info/error_code_info.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/error_code_info/error_code_info.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/error_code_info/tests/error_code_info_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/error_code_info/tests/error_code_info_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/extract_outputs.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/extract_outputs.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/find_dependencies.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/find_dependencies.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/find_dependencies_command.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/find_dependencies_command.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/find_dependencies/tests/find_dependencies_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/find_dependencies/tests/find_dependencies_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/format_constants.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/format_constants.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/format_module.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/format_module.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_generic_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_generic_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_job_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_job_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_json_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_json_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_md_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_md_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_readme_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_readme_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/tests/test_formatting_yml_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/tests/test_formatting_yml_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_classifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_classifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_connection.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_connection.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_dashboard.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_dashboard.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_description.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_description.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic_json.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic_json.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generic_yml.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generic_yml.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericdefinition.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericdefinition.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericfield.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericfield.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_genericmodule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_genericmodule.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_generictype.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_generictype.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_incidentfields.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_incidentfields.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_incidenttype.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_incidenttype.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_indicatorfields.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_indicatorfields.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_indicatortype.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_indicatortype.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_integration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_integration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_job.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_job.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_layout.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_layout.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_lists.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_lists.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_mapper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_mapper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pack_metadata.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pack_metadata.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_playbook.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_playbook.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pre_process_rules.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pre_process_rules.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_pythonfile.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_pythonfile.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_readme.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_readme.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_report.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_report.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_script.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_script.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/format/update_widget.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/format/update_widget.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/common.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/common.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_integration_doc.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_integration_doc.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_playbook_doc.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_playbook_doc.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/generate_script_doc.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/generate_script_doc.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/generate_docs_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/generate_docs_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow_missing` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_docs/tests/test_files/mirroring_test_markdow_missing`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/XSOARIntegration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/XSOARIntegration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/base_code.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/base_code.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/code_generator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/code_generator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/code_generator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/code_generator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotal-autogen-config.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotal-autogen-config.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_integration/tests/test_files/VirusTotalTest/VirusTotalTest.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/generate_integration_context.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/generate_integration_context.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/tests/generate_integration_context_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/tests/generate_integration_context_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_integration_empty_output.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_context/tests/test_data/fake_integration_empty_output.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/generate_descriptions.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/generate_descriptions.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/generate_descriptions_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/generate_descriptions_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/ai21_response.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/ai21_response.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration_similar_paths.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/input_integration_similar_paths.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/logprob_res.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_descriptions/tests/test_data/logprob_res.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_outputs.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_outputs.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/generate_outputs_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/generate_outputs_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/json_to_outputs/json_to_outputs.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/json_to_outputs/json_to_outputs.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_outputs/json_to_outputs/tests/json_to_outputs_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_outputs/json_to_outputs/tests/json_to_outputs_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/test_playbook_generator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/test_playbook_generator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_test_playbook/tests/test_playbook_generator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_test_playbook/tests/test_playbook_generator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/common.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/common.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/generate_unit_tests.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/generate_unit_tests.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/test_case_builder.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/test_case_builder.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/test_module_builder.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/test_module_builder.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/generate_unit_tests_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/generate_unit_tests_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/malwarebazaar.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/inputs/malwarebazaar.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_all.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_all.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_specific_command.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_unit_tests/tests/test_files/outputs/malwarebazaar_specific_command.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/generate_yml.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/generate_yml.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/tests/generate_yml_from_python_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/tests/generate_yml_from_python_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/generate_yml_from_python/yml_metadata_collector.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/generate_yml_from_python/yml_metadata_collector.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/contribution_converter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/contribution_converter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/initiator.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/initiator.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/BaseIntegration_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseIntegration/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/BaseScript/BaseScript_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/BaseScript/BaseScript_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/FeedHelloWorld_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/build_iterator_results.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/build_iterator_results.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/get_indicators_command_results.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/FeedHelloWorld/test_data/get_indicators_command_results.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/HelloIAMWorld_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloIAMWorld/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/HelloWorld_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/domain_reputation.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/domain_reputation.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/ip_reputation.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/ip_reputation.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/scan_results.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/scan_results.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorld/test_data/search_alerts.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorld/test_data/search_alerts.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldScript/HelloWorldScript_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/HelloWorldSlim_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/templates/HelloWorldSlim/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/contribution_converter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/contribution_converter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/initiator_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/initiator_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_and_incidentfield.zip` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_and_incidentfield.zip`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_only.zip` & `demisto_sdk-1.9.0/demisto_sdk/commands/init/tests/test_files/contribution_indicatorfield_only.zip`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/integration_diff_detector.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/integration_diff_detector.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/integration_diff/tests/integration_diff_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/integration_diff/tests/integration_diff_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,17 @@
     The JSON file path to which to output the command results
 *  **--no-coverage**
     Do NOT report coverage
 *  **--coverage-report**
     Specify directory for the coverage report files
 *  **-dt, --docker-timeout**
     The timeout (in seconds) for requests done by the docker client
+*  **-di, --docker-image**
+    The docker image to check package on. Possible values: 'native:maintenance', 'native:ga', 'native:dev', 'all', a specific docker image from Docker Hub (e.g devdemisto/python3:3.10.9.12345) or the default 'from-yml'.
+
 
 
 **Examples**:
 ---
 `demisto-sdk lint -i Integrations/PaloAltoNetworks_XDR,Scripts/HellowWorldScript --no-mypy`
 Details:
 1. lint and test check will execute on Packages `Integrations/PaloAltoNetworks_XDR,Scripts/HellowWorldScript`
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/commands_builder.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/commands_builder.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/helpers.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/helpers.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/lint_manager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/lint_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,36 +13,42 @@
 import git
 import requests.exceptions
 import urllib3.exceptions
 from packaging.version import Version
 from wcmatch.pathlib import Path, PosixPath
 
 from demisto_sdk.commands.common.constants import (
+    API_MODULES_PACK,
     PACKS_PACK_META_FILE_NAME,
     TYPE_PWSH,
     TYPE_PYTHON,
     DemistoException,
 )
 from demisto_sdk.commands.common.docker_helper import init_global_docker_client
 from demisto_sdk.commands.common.handlers import JSON_Handler
 from demisto_sdk.commands.common.logger import Colors
 from demisto_sdk.commands.common.timers import report_time_measurements
 from demisto_sdk.commands.common.tools import (
     find_file,
     find_type,
-    get_api_module_dependencies,
     get_content_path,
     get_file_displayed_name,
     get_json,
     is_external_repository,
     print_error,
     print_v,
     print_warning,
     retrieve_file_ending,
 )
+from demisto_sdk.commands.content_graph.content_graph_commands import (
+    update_content_graph,
+)
+from demisto_sdk.commands.content_graph.interface.neo4j.neo4j_graph import (
+    Neo4jContentGraphInterface,
+)
 from demisto_sdk.commands.lint.helpers import (
     EXIT_CODES,
     FAIL,
     PWSH_CHECKS,
     PY_CHCEKS,
     SUCCESS,
     build_skipped_exit_code,
@@ -83,15 +89,14 @@
         input: str,
         git: bool,
         all_packs: bool,
         quiet: bool,
         verbose: int,
         prev_ver: str,
         json_file_path: str = "",
-        id_set_path: str = None,
         check_dependent_api_module: bool = False,
     ):
 
         # Verbosity level
         self._verbose = not quiet if quiet else verbose
         # Gather facts for manager
         self._facts: dict = self._gather_facts()
@@ -105,38 +110,64 @@
             content_repo=self._facts["content_repo"],
             input=input,
             git=git,
             all_packs=all_packs,
             base_branch=self._prev_ver,
         )
 
-        self._id_set_path = id_set_path
         if check_dependent_api_module:
-            print(
-                "Checking for packages dependent on the modified API module", end="... "
-            )
-            dependent_on_api_module = get_api_module_dependencies(
-                self._pkgs, self._id_set_path, self._verbose
-            )
+            dependent_on_api_module = self._get_api_module_dependent_items()
+            self._pkgs = list(set(self._pkgs + dependent_on_api_module))
+
+        if json_file_path:
+            if os.path.isdir(json_file_path):
+                json_file_path = os.path.join(json_file_path, "lint_outputs.json")
+        self.json_file_path = json_file_path
+        self.linters_error_list: list = []
+
+    def _get_api_module_dependent_items(self) -> list:
+        changed_api_modules = {
+            pkg.name for pkg in self._pkgs if API_MODULES_PACK in pkg.parts
+        }
+        if changed_api_modules:
+            dependent_items = []
+            for changed_api_module in changed_api_modules:
+                print(
+                    f"Checking for packages dependent on the modified API module {changed_api_module}..."
+                )
+
+                with Neo4jContentGraphInterface() as graph:
+                    print("Updating graph...")
+                    update_content_graph(graph, use_git=True, dependencies=True)
+
+                    api_module_nodes = graph.search(object_id=changed_api_module)
+                    api_module_node = api_module_nodes[0] if api_module_nodes else None
+                    if not api_module_node:
+                        raise ValueError(
+                            f"The modified API module `{changed_api_module}` was not found in the "
+                            f"content graph. Please check that it is up to date, and run"
+                            f" `demisto-sdk update-content-graph` if necessary."
+                        )
+
+                    dependent_items += [
+                        dependency.path for dependency in api_module_node.imported_by
+                    ]
+
             dependent_on_api_module = self._get_packages(
-                content_repo=self._facts["content_repo"], input=dependent_on_api_module
+                content_repo=self._facts["content_repo"], input=dependent_items
             )
-            self._pkgs = list(set(self._pkgs + dependent_on_api_module))
+
             if dependent_on_api_module:
                 print(
                     f"Found {Colors.Fg.cyan}{len(dependent_on_api_module)}{Colors.reset} dependent packages. "
                     f"Executing lint and test on those as well."
                 )
-            else:
-                print("No dependent packages found.")
-        if json_file_path:
-            if os.path.isdir(json_file_path):
-                json_file_path = os.path.join(json_file_path, "lint_outputs.json")
-        self.json_file_path = json_file_path
-        self.linters_error_list: list = []
+                return dependent_on_api_module
+            print("No dependent packages found.")
+        return []
 
     @staticmethod
     def _gather_facts() -> Dict[str, Any]:
         """Gather shared required facts for lint command execution - Also perform mandatory resource checkup.
             1. Content repo object.
             2. Requirements file for docker images.
             3. Mandatory test modules - demisto-mock.py etc
@@ -415,14 +446,15 @@
         no_vulture: bool,
         no_test: bool,
         no_pwsh_analyze: bool,
         no_pwsh_test: bool,
         keep_container: bool,
         test_xml: str,
         docker_timeout: int,
+        docker_image_flag: str,
         lint_status: dict,
         pkgs_status: dict,
         pkgs_type: list,
     ) -> Tuple[int, int]:
         """Runs the Lint command on all given packages.
 
         Args:
@@ -436,14 +468,15 @@
             no_coverage(bool): Run pytest without coverage report
             no_test(bool): Whether to skip pytest
             no_pwsh_analyze(bool): Whether to skip powershell code analyzing
             no_pwsh_test(bool): whether to skip powershell tests
             keep_container(bool): Whether to keep the test container
             test_xml(str): Path for saving pytest xml results
             docker_timeout(int): timeout for docker requests
+            docker_image_flag(str): indicates the desirable docker image to run lint on
             pkgs_type: List of the pack types
             pkgs_status: Dictionary for pack status (keys are packs, the values are their status)
             lint_status: Dictionary for the lint status  (the keys are the linters, the values are a list of packs)
 
         Returns:
             Tuple[int, int]: exit code, warning code
         """
@@ -463,14 +496,15 @@
                         else Path(  # type: ignore
                             self._facts["content_repo"].working_dir
                         ),
                         req_2=self._facts["requirements_2"],
                         req_3=self._facts["requirements_3"],
                         docker_engine=self._facts["docker_engine"],
                         docker_timeout=docker_timeout,
+                        docker_image_flag=docker_image_flag,
                     )
                     results.append(
                         executor.submit(
                             linter.run_pack,
                             no_flake8=no_flake8,
                             no_bandit=no_bandit,
                             no_mypy=no_mypy,
@@ -552,14 +586,15 @@
         no_test: bool,
         no_pwsh_analyze: bool,
         no_pwsh_test: bool,
         keep_container: bool,
         test_xml: str,
         failure_report: str,
         docker_timeout: int,
+        docker_image_flag: str,
         time_measurements_dir: str = None,
     ) -> int:
         """Runs the Lint command on all given packages.
 
         Args:
             parallel(int): Whether to run command on multiple threads
             no_flake8(bool): Whether to skip flake8
@@ -573,14 +608,15 @@
             no_test(bool): Whether to skip pytest
             no_pwsh_analyze(bool): Whether to skip powershell code analyzing
             no_pwsh_test(bool): whether to skip powershell tests
             keep_container(bool): Whether to keep the test container
             test_xml(str): Path for saving pytest xml results
             failure_report(str): Path for store failed packs report
             docker_timeout(int): timeout for docker requests
+            docker_image_flag(str): indicates the desirable docker image to run lint on
             time_measurements_dir(str): the directory fo exporting the time measurements info
             total_timeout (int): amount of seconds for the task
 
         Returns:
             int: exit code by fail exit codes by var EXIT_CODES
         """
         lint_status: Dict = {
@@ -608,15 +644,15 @@
 
         # Python or powershell or both
         pkgs_type: list = []
 
         # Detailed packages status
         pkgs_status: dict = {}
 
-        # Skiped lint and test codes
+        # Skipped lint and test codes
         skipped_code = build_skipped_exit_code(
             no_flake8=no_flake8,
             no_bandit=no_bandit,
             no_mypy=no_mypy,
             no_vulture=no_vulture,
             no_xsoar_linter=no_xsoar_linter,
             no_pylint=no_pylint,
@@ -636,14 +672,15 @@
             no_coverage=no_coverage,
             no_vulture=no_vulture,
             no_test=no_test,
             no_pwsh_test=no_pwsh_test,
             keep_container=keep_container,
             test_xml=test_xml,
             docker_timeout=docker_timeout,
+            docker_image_flag=docker_image_flag,
             no_pwsh_analyze=no_pwsh_analyze,
             lint_status=lint_status,
             pkgs_status=pkgs_status,
             pkgs_type=pkgs_type,
         )
 
         if time_measurements_dir:
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/linter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/linter.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,45 @@
 # STD python packages
 import copy
 import hashlib
 import logging
 import os
 import platform
 import traceback
-from typing import Any, Dict, List, Tuple
+from enum import Enum
+from typing import Any, Dict, List, Set, Tuple, Union
 
 import docker
 import docker.errors
 import docker.models.containers
 import git
 import requests.exceptions
 import urllib3.exceptions
 from packaging.version import parse
 from wcmatch.pathlib import NEGATE, Path
 
 from demisto_sdk.commands.common.constants import (
     INTEGRATIONS_DIR,
+    NATIVE_IMAGE_FILE_NAME,
     PACKS_PACK_META_FILE_NAME,
     TYPE_PWSH,
     TYPE_PYTHON,
 )
 from demisto_sdk.commands.common.docker_helper import (
     get_docker,
     init_global_docker_client,
 )
 from demisto_sdk.commands.common.handlers import JSON_Handler, YAML_Handler
+from demisto_sdk.commands.common.hook_validations.docker import DockerImageValidator
+from demisto_sdk.commands.common.native_image import (
+    NativeImageConfig,
+    ScriptIntegrationSupportedNativeImages,
+)
 from demisto_sdk.commands.common.timers import timer
-from demisto_sdk.commands.common.tools import get_all_docker_images, run_command_os
+from demisto_sdk.commands.common.tools import get_docker_images_from_yml, run_command_os
 from demisto_sdk.commands.lint.commands_builder import (
     build_bandit_command,
     build_flake8_command,
     build_mypy_command,
     build_pwsh_analyze_command,
     build_pwsh_test_command,
     build_pylint_command,
@@ -62,44 +69,59 @@
 
 # 3-rd party packages
 
 # Local packages
 
 logger = logging.getLogger("demisto-sdk")
 
+NATIVE_IMAGE_DOCKER_NAME = "demisto/py3-native"
+
+
+class DockerImageFlagOption(Enum):
+    FROM_YML = "from-yml"
+    NATIVE = "native:"
+    NATIVE_DEV = "native:dev"
+    NATIVE_GA = "native:ga"
+    NATIVE_MAINTENANCE = "native:maintenance"
+    ALL_IMAGES = "all"
+
 
 class Linter:
     """Linter used to activate lint command on single package
 
     Attributes:
         pack_dir(Path): Pack to run lint on.
         content_repo(Path): Git repo object of content repo.
         req_2(list): requirements for docker using python2.
         req_3(list): requirements for docker using python3.
         docker_engine(bool):  Whether docker engine detected by docker-sdk.
+        docker_timeout(int): Timeout for docker requests.
+        docker_image_flag(str): Indicates the desirable docker image to run lint on (default value is 'from-yml).
     """
 
     def __init__(
         self,
         pack_dir: Path,
         content_repo: Path,
         req_3: list,
         req_2: list,
         docker_engine: bool,
         docker_timeout: int,
+        docker_image_flag: str = DockerImageFlagOption.FROM_YML.value,
     ):
         self._req_3 = req_3
         self._req_2 = req_2
         self._content_repo = content_repo
 
         # For covering the case when a path file is sent instead of a directory
         self._pack_abs_dir = pack_dir if pack_dir.is_dir() else pack_dir.parent
 
         self._pack_name = None
         self.docker_timeout = docker_timeout
+        self.docker_image_flag = docker_image_flag
         # Docker client init
         if docker_engine:
             self._docker_client: docker.DockerClient = init_global_docker_client(
                 timeout=docker_timeout, log_prompt="Linter"
             )
             self._docker_hub_login = self._docker_login()
         # Facts gathered regarding pack lint and test
@@ -282,17 +304,32 @@
                 f" {self._pkg_lint_status['pack_type']}"
             )
             return True
 
         # Docker images
         if self._facts["docker_engine"]:
             logger.info(f"{log_prompt} - Collecting all docker images to pull")
-            self._facts["images"] = [
-                [image, -1] for image in get_all_docker_images(script_obj=script_obj)
-            ]
+            yml_obj_id = (
+                yml_obj.get("commonfields", {}).get("id", "")
+                if isinstance(yml_obj, dict)
+                else ""
+            )
+            images = self._get_docker_images_for_lint(
+                script_obj=script_obj,
+                script_id=yml_obj_id,
+                docker_image_flag=self.docker_image_flag,
+            )
+            if not images:
+                # If no docker images to run on - skip checks in both docker and host
+                logger.info(
+                    f"{log_prompt} - No docker images to run on - Skipping run lint in host as well."
+                )
+                return True
+            self._facts["images"] = [[image, -1] for image in images]
+
             if os.getenv("GITLAB_CI", False):
                 self._facts["images"] = [
                     [f"docker-io.art.code.pan.run/{image[0]}", -1]
                     for image in self._facts["images"]
                 ]
             # Gather environment variables for docker execution
             self._facts["env_vars"] = {
@@ -677,20 +714,23 @@
             no_pwsh_analyze(bool): Whether to skip powershell code analyzing
             no_pwsh_test(bool): whether to skip powershell tests
             keep_container(bool): Whether to keep the test container
             test_xml(str): Path for saving pytest xml results
             no_coverage(bool): Run pytest without coverage report
 
         """
-        log_promopt = f"{self._pack_name} - Run Lint On Docker Image"
-        logger.info(
-            f'{log_promopt} - Running lint: Number of images={self._facts["images"]}'
-        )
+        log_prompt = f"{self._pack_name} - Run Lint On Docker Image"
+        if self._facts["images"]:
+            logger.info(
+                f'{log_prompt} - Running lint: Number of images={self._facts["images"]}'
+            )
+        else:
+            logger.info(f"{log_prompt} - Skipped")
         for image in self._facts["images"]:
-            logger.info(f"{log_promopt} - Running lint on docker image {image[0]}")
+            logger.info(f"{log_prompt} - Running lint on docker image {image[0]}")
             # Docker image status - visualize
             status = {
                 "image": image[0],
                 "image_errors": "",
                 "pylint_errors": "",
                 "pytest_errors": "",
                 "pytest_json": {},
@@ -777,15 +817,15 @@
                                     test_image=image_id, keep_container=keep_container
                                 )
                             # Perform powershell test
                             elif not no_pwsh_test and check == "pwsh_test":
                                 exit_code, output = self._docker_run_pwsh_test(
                                     test_image=image_id, keep_container=keep_container
                                 )
-                        # If lint check perfrom and failed on reason related to enviorment will run twice,
+                        # If lint check perform and failed on reason related to environment will run twice,
                         # But it failing in second time it will count as test failure.
                         if (
                             (exit_code == RERUN and trial == 1)
                             or exit_code == FAIL
                             or exit_code == SUCCESS
                         ):
                             if exit_code in [RERUN, FAIL]:
@@ -798,19 +838,20 @@
                                     status[f"{check}_errors"] = output
                             break
             else:
                 status["image_errors"] = str(errors)
                 self._pkg_lint_status["exit_code"] += EXIT_CODES["image"]
             # Add image status to images
             self._pkg_lint_status["images"].append(status)
-            logger.info(f"{log_promopt} - Finished linting on docker image {image[0]}")
+            logger.info(f"{log_prompt} - Finished linting on docker image {image[0]}")
 
-        logger.info(
-            f'{log_promopt} - Finished linting. Number of images={self._facts["images"]}'
-        )
+        if self._facts["images"]:
+            logger.info(
+                f'{log_prompt} - Finished linting. Number of images={self._facts["images"]}'
+            )
 
     def _docker_login(self) -> bool:
         """Login to docker-hub using environment variables:
                 1. DOCKERHUB_USER - User for docker hub.
                 2. DOCKERHUB_PASSWORD - Password for docker-hub.
             Used in Circle-CI for pushing into repo devtestdemisto
 
@@ -1302,7 +1343,306 @@
         try:
             commands_obj = script_obj.get("commands", {})
             for command in commands_obj:
                 commands_list.append(command.get("name", ""))
         except Exception:
             logger.debug("Failed getting the commands from the yml file")
         return commands_list
+
+    def _is_native_image_support_script(
+        self,
+        native_image: str,
+        supported_native_images: Set[str],
+        script_id: str,
+    ) -> bool:
+        """
+        Gets a native image name (flag) and checks if it supports the integration/script that lint runs on.
+
+        Args:
+            native_image (str): Name of the Native image to run on.
+            supported_native_images (set): A set including the names of the native images that support the
+                                           script/integration that lint runs on.
+            script_id (str): The ID of the integration/script that lint runs on.
+        Returns (bool): True - if the native image supports the integration/script that lint runs on.
+                        False - Otherwise.
+        """
+        if native_image not in supported_native_images:
+            # Integration/Script isn't supported by the requested native image
+            logger.info(
+                f"{script_id} - Skipping checks on docker for {native_image} - {script_id} is not supported by the "
+                f"requested native image: {native_image}"
+            )
+            return False
+
+        return True
+
+    def _check_native_image_flag(self, docker_image_flag):
+        """
+        Gets a native docker image flag and verify that it is one of the following: 'native:ga', 'native:maintenance'
+        or 'native:dev'.
+        If it isn't, raises a suitable exception.
+        Args:
+            docker_image_flag (str): Requested docker image flag.
+        Returns (None): None
+        """
+
+        if docker_image_flag not in (
+            DockerImageFlagOption.NATIVE_DEV.value,
+            DockerImageFlagOption.NATIVE_GA.value,
+            DockerImageFlagOption.NATIVE_MAINTENANCE.value,
+        ):
+            err_msg = (
+                f"The requested native image: '{docker_image_flag}' is not supported. The possible options are: "
+                f"'native:ga', 'native:maintenance' and 'native:dev'. For supported native image"
+                f" versions please see: 'Tests/{NATIVE_IMAGE_FILE_NAME}'"
+            )
+            logger.error(
+                f"Skipping checks on docker for '{docker_image_flag}' - {err_msg}"
+            )
+            raise ValueError(err_msg)
+
+    def _get_native_image_name_from_config_file(
+        self,
+        docker_image_flag: str,
+    ) -> Union[str, None]:
+        """
+        Gets a native docker image flag and returns its mapped native image name from the
+        'docker_native_image_config.json' file.
+
+        If the requested docker image flag doesn't have a mapped native image in the config file - write to the logs.
+
+        Args:
+            docker_image_flag (str): Requested docker image flag.
+        Returns (None): None
+        """
+        native_image_config = (
+            NativeImageConfig()
+        )  # parsed docker_native_image_config.json file (a singleton obj)
+
+        if native_image := native_image_config.flags_versions_mapping.get(
+            docker_image_flag
+        ):
+            return native_image
+
+        else:
+            # The requested native image doesn't exist in the native config file
+            logger.info(
+                f"Skipping checks on docker for '{docker_image_flag}' - The requested native image: "
+                f"'{docker_image_flag}' is not supported. For supported native image versions please see:"
+                f" 'Tests/{NATIVE_IMAGE_FILE_NAME}'"
+            )
+            return None
+
+    def _get_dev_native_image(self, script_id: str) -> Union[str, None]:
+        """
+        Gets the development (dev) native image, which is the latest tag of the native image from Docker Hub.
+        Args:
+            script_id (str): The ID of the integration/script that lint runs on.
+        Returns: The reference of the dev native image.
+        """
+        log_prompt = f"{self._pack_name} - Get Dev Native Image"
+        logger.info(f"{log_prompt} - Started")
+
+        # Get the latest tag of the native image from Docker Hub
+        latest_native_image_tag = (
+            DockerImageValidator.get_docker_image_latest_tag_request(
+                NATIVE_IMAGE_DOCKER_NAME
+            )
+        )
+
+        if latest_native_image_tag:
+            dev_native_image_full_name = (
+                f"{NATIVE_IMAGE_DOCKER_NAME}:{latest_native_image_tag}"
+            )
+            return dev_native_image_full_name
+
+        else:  # latest tag not found
+            err_msg = (
+                f"{log_prompt} - {script_id} - Error: Failed getting the native image latest tag from"
+                f" Docker Hub."
+            )
+            logger.error(err_msg)
+            raise RuntimeError(err_msg)
+
+    def _get_versioned_native_image(
+        self,
+        native_image: str,
+    ) -> Union[str, None]:
+        """
+        Gets a versioned native image name, and finds it's reference (tag) in the docker_native_image_config.json file.
+        Args:
+            native_image (str): Name of the Native image to run on.
+        Returns (str): The native image reference (tag).
+        """
+        logger.info(
+            f"{self._pack_name} - Get Versioned Native Image - {native_image} - Started"
+        )
+
+        native_image_config = (
+            NativeImageConfig()
+        )  # parsed docker_native_image_config.json file (a singleton obj)
+
+        return native_image_config.get_native_image_reference(native_image)
+
+    def _get_all_docker_images(
+        self,
+        script_obj: Dict,
+        script_id: str,
+        supported_native_images: Set[str],
+    ) -> List[str]:
+        """
+        Gets the following docker images references:
+            1. Native GA - the native image of the current server version.
+            2. Native Maintenance - the native image of the previous server version.
+            3. Native Dev - The latest tag of the native image for Docker Hub.
+            4. The docker images that appear in the YML file of the integration/script that lint runs on.
+        Args:
+            script_obj (Dict): A yml as dict of the integration/script that lint runs on.
+            script_id (str): The ID of the integration/script that lint runs on.
+            supported_native_images (set): A set including the names of the native images supported for the
+                                           script/integration that lint runs on.
+        Returns (List): A list including all the docker images to run on.
+        """
+        logger.info(f"{self._pack_name} - Get All Docker Images Started")
+
+        # Get docker images from yml:
+        logger.info(f"{self._pack_name} - Get Docker Image from YML - Started")
+        imgs = get_docker_images_from_yml(script_obj)
+
+        # Get native images:
+        native_image_config = (
+            NativeImageConfig()
+        )  # parsed docker_native_image_config.json file (a singleton obj)
+
+        for native_image in native_image_config.native_images:
+            if self._is_native_image_support_script(
+                native_image, supported_native_images, script_id
+            ):
+
+                if native_image == DockerImageFlagOption.NATIVE_DEV.value:
+                    #  Get native latest from Docker Hub
+                    native_image_ref = self._get_dev_native_image(script_id)
+                else:  # versioned native image
+                    native_image_ref = self._get_versioned_native_image(native_image)
+
+                if native_image_ref:
+                    imgs.append(native_image_ref)
+
+        return imgs
+
+    def _get_docker_images_for_lint(
+        self, script_obj: Dict, script_id: str, docker_image_flag: str
+    ) -> List[str]:
+        """Gets a yml as dict of the current integration/script that lint runs on, and a flag indicates on which docker
+         images lint should run.
+         Creates a list including all the desirable docker images according to the following logic:
+            - If docker_image_flag is 'native:ga', lint will run on the native image of the ga server version.
+
+            - If docker_image_flag is 'native:maintenance', lint will run on the native image of the previous
+              server version.
+
+            - If docker_image_flag is 'native:dev', lint will find the latest tag of the native image (in Docker Hub)
+              and will run on it.
+
+            ** If the integration/script that lint runs on not support the requested native image - the checks on
+               docker and in host will be skipped.
+
+            - If docker_image_flag is 'from-yml', lint will run on the docker images appearing in the YML file of the
+              integration/script.
+
+            - If docker_image_flag is 'all', lint will run on:
+                1. Native GA - the native image of the current server version.
+                2. Native Maintenance - the native image of the previous server version.
+                3. Native Dev - The latest tag of the native image for Docker Hub.
+                4. The docker images that appear in the YML file of the integration/script that lint runs on.
+
+            - If the docker_image_flag is a specific docker image tag, lint will try to run on it.
+        Args:
+            script_obj (dict): A yml dict of the integration/script that lint runs on.
+            script_id (str): The ID of the integration/script that lint runs on.
+            docker_image_flag (str): A flag indicates on which docker images lint should run.
+        Returns:
+            List. A list of all desirable docker images references.
+        """
+        log_prompt = f"{self._pack_name} - Get All Docker Images For Lint"
+        logger.info(
+            f"{log_prompt} - Requested docker image flag is: '{docker_image_flag}'"
+        )
+        imgs = []
+
+        if (
+            docker_image_flag == DockerImageFlagOption.FROM_YML.value
+        ):  # the default option
+            # Desirable docker images are the docker images from the yml file (alt-dockerimages included)
+            logger.info(f"{self._pack_name} - Get Docker Image from YML - Started")
+            if imgs := get_docker_images_from_yml(script_obj):
+                logger.info(
+                    f"{log_prompt} - Docker images to run on are: {', '.join(imgs)}"
+                )
+            return imgs
+
+        di_from_yml = script_obj.get("dockerimage")
+        # If the 'dockerimage' key does not exist in yml - run on native image checks will be skipped
+        native_image_config = (
+            NativeImageConfig()
+        )  # parsed docker_native_image_config.json file (a singleton obj)
+        supported_native_images_obj = ScriptIntegrationSupportedNativeImages(
+            _id=script_id,
+            native_image_config=native_image_config,
+            docker_image=di_from_yml,
+        )
+        supported_native_images = set(
+            supported_native_images_obj.get_supported_native_image_versions(
+                only_production_tags=False
+            )
+        )
+
+        if docker_image_flag.startswith(DockerImageFlagOption.NATIVE.value):
+            # Desirable docker image to run on is a native image
+
+            self._check_native_image_flag(docker_image_flag)
+
+            if native_image := self._get_native_image_name_from_config_file(
+                docker_image_flag
+            ):
+
+                if self._is_native_image_support_script(
+                    native_image, supported_native_images, script_id
+                ):  # Integration/Script is supported by the requested native image
+
+                    if docker_image_flag == DockerImageFlagOption.NATIVE_DEV.value:
+                        # Desirable docker image to run on is the dev native image - get the latest tag from Docker Hub
+                        native_image_ref = self._get_dev_native_image(script_id)
+
+                    else:
+                        # Desirable docker image to run on is a versioned native image - get the docker ref from the
+                        # docker_native_image_config.json
+                        native_image_ref = self._get_versioned_native_image(
+                            native_image
+                        )
+
+                    if native_image_ref:
+                        imgs.append(native_image_ref)
+                        logger.info(
+                            f"{log_prompt} - Native image to run on is: {native_image_ref}"
+                        )
+
+        elif docker_image_flag == DockerImageFlagOption.ALL_IMAGES.value:
+            # Desirable docker images are the docker images from the yml file, the supported versioned native images
+            # and the dev native image
+            if imgs := self._get_all_docker_images(
+                script_obj, script_id, supported_native_images
+            ):
+                logger.info(
+                    f"{log_prompt} - Docker images to run on are: {', '.join(imgs)}"
+                )
+
+        else:
+            # The flag is a specific docker image (from Docker Hub) or an invalid input -
+            # In both cases we will try to run on the given input, if it does not exist in docker hub the run of lint
+            # will fail later on.
+            imgs.append(docker_image_flag)
+            logger.info(
+                f"{log_prompt} - Docker image to run on is: {docker_image_flag}"
+            )
+
+        return imgs
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/installation_scripts/powershell_image.sh` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/installation_scripts/powershell_image.sh`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/installation_scripts/python_image.sh` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/installation_scripts/python_image.sh`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile.lock` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pipfile_python3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/base_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/base_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/certified_partner_level_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/certified_partner_level_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/community_level_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/community_level_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/partner_level_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/partner_level_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/resources/pylint_plugins/xsoar_level_checker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/resources/pylint_plugins/xsoar_level_checker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/command_builder_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/command_builder_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/docker_helper_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/docker_helper_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/helper_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/helper_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/linter_manager_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/linter_manager_test.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from pathlib import PosixPath
 from unittest.mock import MagicMock, patch
 
 import pytest
 
 from demisto_sdk.commands.common.constants import TYPE_PWSH, TYPE_PYTHON, FileType
 from demisto_sdk.commands.common.legacy_git_tools import git_path
+from demisto_sdk.commands.content_graph.interface.neo4j.neo4j_graph import (
+    Neo4jContentGraphInterface,
+)
 from demisto_sdk.commands.lint.lint_manager import LintManager
 from TestSuite.test_tools import ChangeCWD
 
 
 def mock_lint_manager(mocker):
     mocker.patch.object(LintManager, "_get_packages", return_value=[])
     mocker.patch.object(LintManager, "_gather_facts", return_value={"content_repo": ""})
@@ -759,7 +762,197 @@
             "errorCode": "E9001",
             "message": "FileShareLink.prepare_request_object: Sys.exit use is found, Please use return instead.",
             "row": "105",
             "col": "8",
         }
     ]
     assert json_contents == expected_format
+
+
+class NodeDependencyMock:
+    def __init__(self, path):
+        self.path = path
+
+
+class NodeMock:
+    def __init__(self, imported_by):
+        self.imported_by = imported_by
+
+
+@pytest.mark.parametrize(
+    "changed_files, api_module_nodes, dependent_items, packages_of_dependent_items, cdam_flag",
+    [
+        pytest.param(
+            [PosixPath("Packs/ApiModules/Scripts/SomeApiModule")],
+            [
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomePack/Scripts/SomeScript/SomeScript.py"
+                            )
+                        ]
+                    )
+                ]
+            ],
+            ["Packs/SomePack/Scripts/SomeScript/SomeScript.py"],
+            [PosixPath("Packs/SomePack/Scripts/SomeScript")],
+            True,
+            id="single api module change with dependency",
+        ),
+        pytest.param(
+            [PosixPath("Packs/ApiModules/Scripts/SomeApiModule")],
+            [[NodeMock(imported_by=[])]],
+            [],
+            [],
+            True,
+            id="single api module change with no dependencies",
+        ),
+        pytest.param(
+            [PosixPath("Packs/SomePack/Scripts/SomePackScript")],
+            [
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomeOtherPack/Scripts/SomeScript/SomeScript.py"
+                            )
+                        ]
+                    )
+                ]
+            ],
+            [],
+            [],
+            True,
+            id="non api module change with dependency",
+        ),
+        pytest.param(
+            [PosixPath("Packs/ApiModules/Scripts/SomeApiModule")],
+            [
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomePack1/Scripts/SomeScript1/SomeScript1.py"
+                            ),
+                            NodeDependencyMock(
+                                path="Packs/SomePack2/Scripts/SomeScript2/SomeScript2.py"
+                            ),
+                        ]
+                    )
+                ]
+            ],
+            [
+                "Packs/SomePack1/Scripts/SomeScript1/SomeScript1.py",
+                "Packs/SomePack2/Scripts/SomeScript2/SomeScript2.py",
+            ],
+            [
+                PosixPath("Packs/SomePack1/Scripts/SomeScript1"),
+                PosixPath("Packs/SomePack2/Scripts/SomeScript2"),
+            ],
+            True,
+            id="single api module change with 2 dependencies",
+        ),
+        pytest.param(
+            [
+                PosixPath("Packs/ApiModules/Scripts/SomeApiModule1"),
+                PosixPath("Packs/ApiModules/Scripts/SomeApiModule2"),
+            ],
+            [
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomePack1/Scripts/SomeScript1/SomeScript1.py"
+                            )
+                        ]
+                    )
+                ],
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomePack2/Scripts/SomeScript2/SomeScript2.py"
+                            )
+                        ]
+                    )
+                ],
+            ],
+            [
+                "Packs/SomePack1/Scripts/SomeScript1/SomeScript1.py",
+                "Packs/SomePack2/Scripts/SomeScript2/SomeScript2.py",
+            ],
+            [
+                PosixPath("Packs/SomePack1/Scripts/SomeScript1"),
+                PosixPath("Packs/SomePack2/Scripts/SomeScript2"),
+            ],
+            True,
+            id="2 api module changes with 1 dependency each",
+        ),
+        pytest.param(
+            [PosixPath("Packs/ApiModules/Scripts/SomeApiModule")],
+            [
+                [
+                    NodeMock(
+                        imported_by=[
+                            NodeDependencyMock(
+                                path="Packs/SomePack/Scripts/SomeScript/SomeScript.py"
+                            )
+                        ]
+                    )
+                ]
+            ],
+            [],
+            [],
+            False,
+            id="single api module change with dependency, no cdam flag",
+        ),
+    ],
+)
+def test_get_api_module_dependent_items(
+    mocker,
+    changed_files,
+    api_module_nodes,
+    dependent_items,
+    packages_of_dependent_items,
+    cdam_flag,
+):
+    """
+    Given:
+        - Changed API modules with various dependencies.
+
+    When:
+        - Running lint on API modules
+
+    Then:
+        - Ensure that lint runs on all relevant dependencies as well.
+    """
+    get_packages_mock = mocker.patch.object(
+        LintManager,
+        "_get_packages",
+        side_effect=[changed_files, packages_of_dependent_items],
+    )
+    mocker.patch.object(LintManager, "_gather_facts", return_value={"content_repo": ""})
+
+    mocker.patch.object(Neo4jContentGraphInterface, "__init__", return_value=None)
+    mocker.patch.object(
+        Neo4jContentGraphInterface, "__enter__", return_value=Neo4jContentGraphInterface
+    )
+    mocker.patch.object(Neo4jContentGraphInterface, "__exit__", return_value=None)
+    mocker.patch("demisto_sdk.commands.lint.lint_manager.update_content_graph")
+    mocker.patch.object(
+        Neo4jContentGraphInterface, "search", side_effect=api_module_nodes
+    )
+    lint_manager = LintManager(
+        input="",
+        git=False,
+        all_packs=False,
+        quiet=False,
+        verbose=False,
+        prev_ver="master",
+        json_file_path="path",
+        check_dependent_api_module=cdam_flag,
+    )
+
+    assert set(lint_manager._pkgs) == set(packages_of_dependent_items + changed_files)
+    if packages_of_dependent_items:
+        get_packages_mock.assert_called_with(content_repo="", input=dependent_items)
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/conftest.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/conftest.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/docker_runner_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/docker_runner_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_linter/os_runner_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_linter/os_runner_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/base_checker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/base_checker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/certified_partner_level_checker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/certified_partner_level_checker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/partner_level_checker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/partner_level_checker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/lint/tests/test_pylint_plugin/xsoar_level_checker_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/lint/tests/test_pylint_plugin/xsoar_level_checker_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/openapi_codegen.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/openapi_codegen.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/resources/Generated_image.png` & `demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/resources/Generated_image.png`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/openapi_codegen/tests/openapi_codegen_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/openapi_codegen/tests/openapi_codegen_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/postman_codegen.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/postman_codegen.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/config-urlscanio.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/config-urlscanio.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/integration-urlscanio.yml` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/integration-urlscanio.yml`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/resources/urlscan.io.postman_collection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/resources/urlscan.io.postman_collection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/postman_codegen_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/postman_codegen_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal-autogen-config.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal-autogen-config.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal.postman_collection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/VirusTotal.postman_collection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/arguments_check_collection.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/arguments_check_collection.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/postman_codegen/tests/test_files/shared_args_path.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/postman_codegen/tests/test_files/shared_args_path.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/generic_module_unifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/generic_module_unifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/integration_script_unifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/integration_script_unifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/prepare_upload_manager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/prepare_upload_manager.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/rule_unifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/rule_unifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/generic_module_unifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/generic_module_unifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/xdrc_template_unifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/xdrc_template_unifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/tests/yml_unifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/tests/yml_unifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/prepare_content/xdrc_template_unifier.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/prepare_content/xdrc_template_unifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/runner.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/runner.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/runner_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/runner_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component.txt` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component.txt`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component_no_context.txt` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_cmd/tests/test_data/kl-get-component_no_context.txt`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_playbook/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_playbook/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_playbook/playbook_runner.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_playbook/playbook_runner.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/test_playbook_runner.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/test_playbook_runner.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/run_test_playbook/tests/test_playbook_runner_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/run_test_playbook/tests/test_playbook_runner_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/secrets/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/secrets/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/secrets/secrets.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/secrets/secrets.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/secrets/tests/secrets_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/secrets/tests/secrets_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/split/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/split/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/split/jsonsplitter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/split/jsonsplitter.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/split/tests/jsonsplitter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/split/tests/jsonsplitter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/split/tests/ymlsplitter_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/split/tests/ymlsplitter_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/split/ymlsplitter.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/split/ymlsplitter.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     TYPE_PWSH,
     TYPE_PYTHON,
     TYPE_TO_EXTENSION,
 )
 from demisto_sdk.commands.common.handlers import YAML_Handler
 from demisto_sdk.commands.common.tools import (
     LOG_COLORS,
-    get_all_docker_images,
+    get_docker_images_from_yml,
     get_pipenv_dir,
     get_python_version,
     get_yaml,
     pascal_case,
     print_color,
     print_error,
 )
@@ -239,15 +239,15 @@
                         )
                 if self.pipenv:
                     try:
                         self.print_logs(
                             "Detecting python version and setting up pipenv files ...",
                             log_color=LOG_COLORS.NATIVE,
                         )
-                        docker = get_all_docker_images(script_obj)[0]
+                        docker = get_docker_images_from_yml(script_obj)[0]
                         py_ver = get_python_version(docker, self.config.log_verbose)
                         pip_env_dir = get_pipenv_dir(py_ver, self.config.envs_dirs_base)
                         self.print_logs(
                             f"Copying pipenv files from: {pip_env_dir}",
                             log_color=LOG_COLORS.NATIVE,
                         )
                         shutil.copy(f"{pip_env_dir}/Pipfile", output_path)
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/Docker.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/Docker.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/IntegrationsLock.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/IntegrationsLock.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/ParallelLoggingManager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/ParallelLoggingManager.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/TestContentClasses.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/TestContentClasses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1536,15 +1536,15 @@
                     if param_conf["display"] in params
                     else param_conf["name"]
                 )
                 if key == "credentials":
                     credentials = params[key]
                     param_value = {
                         "credential": "",
-                        "identifier": credentials["identifier"],
+                        "identifier": credentials.get("identifier", ""),
                         "password": credentials["password"],
                         "passwordChanged": False,
                     }
                 else:
                     param_value = params[key]
 
                 param_conf["value"] = param_value
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/execute_test_content.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/execute_test_content.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/mock_server.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/mock_server.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/init_test_data.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/init_test_data.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/test_modeling_rule.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/test_modeling_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,16 +150,16 @@
         str: The XQL query.
     """
     fields = ", ".join([field for field in rule.fields])
     td_event_ids = ", ".join(
         [f'"{td_event_id}"' for td_event_id in test_data_event_ids]
     )
     query = (
-        f"datamodel dataset in({rule.dataset}) | filter {rule.dataset}.test_data_event_id in({td_event_ids}) "
-        f"| dedup {rule.dataset}.test_data_event_id by desc _insert_time | fields "
+        f"config timeframe = 10y | datamodel dataset in({rule.dataset}) | filter {rule.dataset}.test_data_event_id "
+        f"in({td_event_ids}) | dedup {rule.dataset}.test_data_event_id by desc _insert_time | fields "
         f"{rule.dataset}.test_data_event_id, {fields}"
     )
     return query
 
 
 def validate_expected_values(
     xsiam_client: XsiamApiClient, mr: ModelingRule, test_data: init_test_data.TestData
@@ -214,25 +214,34 @@
         typer.Exit: If the dataset does not exist after the timeout.
     """
     dataset = test_data.data[0].dataset
     logger.info(
         f'[cyan]Checking if dataset "{dataset}" exists on the tenant...[/cyan]',
         extra={"markup": True},
     )
-    query = f"dataset = {dataset}"
+    query = f"config timeframe = 10y | dataset = {dataset}"
     for i in range(timeout // interval):
         logger.debug(f"Check #{i+1}...")
         try:
             execution_id = xsiam_client.start_xql_query(query)
             results = xsiam_client.get_xql_query_result(execution_id)
             if results:
                 logger.info(
                     f"[green]Dataset {dataset} exists[/green]", extra={"markup": True}
                 )
                 return
+            else:
+                err = (
+                    f"[red]Dataset {dataset} exists but no results were returned. This could mean that your testdata "
+                    "does not meet the criteria for an associated Parsing Rule and is therefore being dropped from "
+                    "the dataset. Check to see if a Parsing Rule exists for your dataset and that your testdata "
+                    "meets the criteria for that rule.[/red]"
+                )
+                logger.error(err, extra={"markup": True})
+                raise typer.Exit(1)
         except requests.exceptions.HTTPError:
             pass
         sleep(interval)
     logger.error(
         f"[red]Dataset {dataset} does not exist after {timeout} seconds[/red]",
         extra={"markup": True},
     )
@@ -331,14 +340,16 @@
                 }
                 upload_result = upload_cmd(**upload_kwargs)
                 if upload_result != 0:
                     logger.error(
                         f"[red]Failed to upload pack {containing_pack_id} to tenant[/red]",
                         extra={"markup": True},
                     )
+                # wait for pack to finish installing
+                sleep(1)
             else:
                 upload_result = 1
         if not interactive or not upload_result == 0:
             logger.error(
                 "[red]Please install or upload the pack to the tenant and try again[/red]",
                 extra={"markup": True},
             )
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/init_test_data_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/init_test_data_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_data/fake_test_data_file.json` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_data/fake_test_data_file.json`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_modeling_rule_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/test_modeling_rule/tests/test_modeling_rule_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/DemistoClientMock.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/DemistoClientMock.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/ParallelLoggingManager_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/ParallelLoggingManager_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/build_context_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/build_context_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/execute_test_content_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/execute_test_content_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/integration_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/integration_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/mock_unit_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/mock_unit_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/server_context_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/server_context_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/test_context_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/test_context_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/test_tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/testplaybook_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/testplaybook_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tests/timestamp_replacer_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tests/timestamp_replacer_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/timestamp_replacer.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/timestamp_replacer.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/tools.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/tools.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/xsiam_tools/test_data.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/xsiam_tools/test_data.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/test_content/xsiam_tools/xsiam_client.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/test_content/xsiam_tools/xsiam_client.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests/update_rn_manager_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests/update_rn_manager_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/tests/update_rn_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/tests/update_rn_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/update_rn.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/update_rn.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from demisto_sdk.commands.common.constants import (
     ALL_FILES_VALIDATION_IGNORE_WHITELIST,
     DEPRECATED_DESC_REGEX,
     DEPRECATED_NO_REPLACE_DESC_REGEX,
     IGNORED_PACK_NAMES,
     RN_CONTENT_ENTITY_WITH_STARS,
     RN_HEADER_BY_FILE_TYPE,
-    SKIP_RELEASE_NOTES_FOR_TYPES,
     XSIAM_DASHBOARDS_DIR,
     XSIAM_REPORTS_DIR,
     FileType,
 )
 from demisto_sdk.commands.common.content import Content
 from demisto_sdk.commands.common.content.objects.pack_objects import (
     Integration,
@@ -250,16 +249,14 @@
         rn_path = self.get_release_notes_path(new_version)
         self.check_rn_dir(rn_path)
         self.rn_path = rn_path
         self.find_added_pack_files()
         changed_files = {}
         for packfile in self.modified_files_in_pack:
             file_name, file_type = self.get_changed_file_name_and_type(packfile)
-            if file_type in SKIP_RELEASE_NOTES_FOR_TYPES:
-                continue
             if (
                 "yml" in packfile
                 and file_type
                 in [FileType.INTEGRATION, FileType.BETA_INTEGRATION, FileType.SCRIPT]
                 and packfile not in self.added_files
             ):
                 docker_image_name: Optional[str] = check_docker_image_changed(
@@ -818,24 +815,26 @@
             key=lambda x: x[0][0] if x[0][0] else "",
             reverse=True,
         ):
             is_new_file = data.get("is_new_file")
             desc = data.get("description", "")
             docker_image = data.get("dockerimage")
             rn_desc = ""
+            path = data.get("path")
             if _type is None:
                 continue
 
             _header_by_type = RN_HEADER_BY_FILE_TYPE.get(_type)
             rn_desc += "\n" + self.build_rn_desc(
                 _type=_type,
                 content_name=content_name,
                 desc=desc,
                 is_new_file=is_new_file,
                 docker_image=docker_image,
+                path=path,
             )
             if _header_by_type and _header_by_type in current_rn_without_docker_images:
                 if self.does_content_item_header_exist_in_rns(
                     current_rn_without_docker_images, content_name
                 ):
                     if docker_image:
                         new_rn = self.handle_existing_rn_with_docker_image(
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_release_notes/update_rn_manager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_release_notes/update_rn_manager.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/tests/update_xsoar_config_file_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/tests/update_xsoar_config_file_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/update_xsoar_config_file/update_xsoar_config_file.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/update_xsoar_config_file/update_xsoar_config_file.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/data/TestPack.zip` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/data/TestPack.zip`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/data/content_packs.zip` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/data/content_packs.zip`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/tests/uploader_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/tests/uploader_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,27 +202,68 @@
 
     When
         - Uploading a layout
 
     Then
         - Ensure layout is uploaded successfully
         - Ensure success upload message is printed as expected
+        - Ensure that _unify isn't called.
     """
+    from demisto_sdk.commands.common.content.objects.pack_objects.layout.layout import (
+        LayoutObject,
+    )
+
     mocker.patch.object(demisto_client, "configure", return_value="object")
+    unify_mocker = mocker.patch.object(LayoutObject, "_unify")
+
     layout_name = "layout-details-test_bla-V2.json"
     layout_path = f"{git_path()}/demisto_sdk/tests/test_files/Packs/DummyPack/Layouts/{layout_name}"
+
     uploader = Uploader(input=layout_path, insecure=False, verbose=False)
     mocker.patch.object(uploader, "client")
     uploader.upload()
 
+    assert not unify_mocker.called
     assert [
         (layout_name, FileType.LAYOUT.value)
     ] == uploader.successfully_uploaded_files
 
 
+def test_upload_layout_container_positive(demisto_client_configure, mocker):
+    """
+    Given
+        - layout container
+
+    When
+        - Uploading a layout-container
+
+    Then
+        - Ensure layout-container is uploaded successfully
+        - Ensure that _unify is called.
+    """
+    from demisto_sdk.commands.common.content.objects.pack_objects.layout.layout import (
+        LayoutObject,
+    )
+
+    mocker.patch.object(demisto_client, "configure", return_value="object")
+    unify_mocker = mocker.patch.object(LayoutObject, "_unify")
+
+    layout_name = "layoutscontainer-test.json"
+    layout_path = f"{git_path()}/demisto_sdk/tests/test_files/Packs/DummyPack/Layouts/{layout_name}"
+
+    uploader = Uploader(input=layout_path, insecure=False, verbose=False)
+    mocker.patch.object(uploader, "client")
+    uploader.upload()
+
+    assert unify_mocker.called
+    assert [
+        (layout_name, FileType.LAYOUTS_CONTAINER.value)
+    ] == uploader.successfully_uploaded_files
+
+
 def test_upload_incident_type_positive(demisto_client_configure, mocker):
     """
     Given
         - An incident type named Hello_World_Alert to upload
 
     When
         - Uploading incident type
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/upload.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/upload.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/upload/uploader.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/upload/uploader.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/validate/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/validate/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/validate/tests/validators_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/validate/tests/validators_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from demisto_sdk.commands.common import tools
 from demisto_sdk.commands.common.constants import (
     FILETYPE_TO_DEFAULT_FROMVERSION,
     PACKS_PACK_META_FILE_NAME,
     TEST_PLAYBOOK,
     FileType,
 )
+from demisto_sdk.commands.common.content.content import Content
 from demisto_sdk.commands.common.content_constant_paths import CONF_PATH
 from demisto_sdk.commands.common.errors import Errors
 from demisto_sdk.commands.common.git_util import GitUtil
 from demisto_sdk.commands.common.handlers import JSON_Handler
 from demisto_sdk.commands.common.hook_validations.base_validator import BaseValidator
 from demisto_sdk.commands.common.hook_validations.content_entity_validator import (
     ContentEntityValidator,
@@ -132,14 +133,29 @@
 )
 from TestSuite.pack import Pack
 from TestSuite.test_tools import ChangeCWD
 
 json = JSON_Handler()
 
 
+class MyRepo:
+    active_branch = "not-master"
+
+    def remote(self):
+        return "remote_path"
+
+
+@pytest.fixture(autouse=False)
+def set_git_test_env(mocker):
+    mocker.patch.object(ValidateManager, "setup_git_params", return_value=True)
+    mocker.patch.object(Content, "git", return_value=MyRepo())
+    mocker.patch.object(ValidateManager, "setup_prev_ver", return_value="origin/master")
+    mocker.patch.object(GitUtil, "_is_file_git_ignored", return_value=False)
+
+
 class TestValidators:
     CREATED_DIRS: List[str] = list()
 
     @classmethod
     def setup_class(cls):
         for dir_to_create in DIR_LIST:
             if not os.path.exists(dir_to_create):
@@ -630,15 +646,17 @@
         INVALID_REPUTATION_PATH,
         INVALID_SCRIPT_PATH,
         INVALID_WIDGET_PATH,
         INVALID_BETA_INTEGRATION,
     ]
 
     @pytest.mark.parametrize("file_path", INVALID_FILES_PATHS_FOR_ALL_VALIDATIONS)
-    def test_run_all_validations_on_file_failed(self, mocker, file_path):
+    def test_run_all_validations_on_file_failed(
+        self, set_git_test_env, mocker, file_path
+    ):
         """
         Given
         - An invalid file inside a pack
 
         When
         - running run_all_validations_on_file on that file
 
@@ -657,15 +675,17 @@
         )
         mocker.patch.object(
             IntegrationValidator, "is_valid_category", return_value=True
         )
         validate_manager = ValidateManager(file_path=file_path, skip_conf_json=True)
         assert not validate_manager.run_validation_on_specific_files()
 
-    def test_run_all_validations_on_file_with_modified_id(self, mocker, integration):
+    def test_run_all_validations_on_file_with_modified_id(
+        self, set_git_test_env, mocker, integration
+    ):
         """
         Given
         - Integration with a modified ID.
 
         When
         - running 'run_all_validations_on_file' on that file.
 
@@ -996,15 +1016,15 @@
         -  validator should ignore those files
         """
         validate_manager = ValidateManager()
         assert validate_manager.run_validations_on_file(
             INVALID_IGNORED_UNIFIED_INTEGRATION, None
         )
 
-    def test_non_integration_png_files_ignored(self):
+    def test_non_integration_png_files_ignored(self, set_git_test_env):
         """
         Given
         - A png file
         When
         - Validating it
         Then
         -  validator should ignore those files and return False
@@ -1104,15 +1124,15 @@
             "BA115",
             "BC101",
             "BC102",
             "BC103",
             "BC104",
         }.issubset(error_list)
 
-    def test_added_files_type_using_function(self, repo, mocker):
+    def test_added_files_type_using_function(self, set_git_test_env, repo, mocker):
         """
         Given:
             - A list of errors that should be checked
         When:
             - Running create_ignored_errors_list from validate manager
         Then:
             - verify that the ignored error list that comes out is correct
@@ -1592,15 +1612,15 @@
         modified_files = {
             "Packs/CortexXDR/Integrations/PaloAltoNetworks_XDR/PaloAltoNetworks_XDR.yml"
         }
         mocker.patch.object(ReleaseNotesValidator, "__init__", return_value=None)
         mocker.patch.object(ReleaseNotesValidator, "is_file_valid", return_value=True)
         validate_manager = ValidateManager(skip_conf_json=True)
         assert validate_manager.validate_release_notes(
-            file_path, {}, modified_files, None, False
+            file_path, {}, modified_files, None
         )
 
     def test_validate_release_notes__invalid_rn_for_new_pack(self, mocker):
         """
         Given
             - A release note file for a newly created pack.
         When
@@ -1620,15 +1640,15 @@
             "handle_error",
             return_value="ReleaseNotes for newly created pack",
         )
         validate_manager = ValidateManager(skip_conf_json=True)
         validate_manager.new_packs = {"CortexXDR"}
         assert (
             validate_manager.validate_release_notes(
-                file_path, {file_path}, modified_files, None, False
+                file_path, {file_path}, modified_files, None
             )
             is False
         )
 
     def test_run_validations_on_file_release_notes_config(self, pack):
         """
         Sanity test for running validation on RN config file
@@ -2646,24 +2666,24 @@
     When:
         Checking if the pack name of the file is valid (the pack name is not changed).
     Then:
         If new file or unchanged pack then `true`, else `false`.
 
     """
     validator_obj = ValidateManager()
-    assert validator_obj.is_valid_pack_name("Packs/original_pack/file", None)
+    assert validator_obj.is_valid_pack_name("Packs/original_pack/file", None, None)
     assert validator_obj.is_valid_pack_name(
-        "Packs/original_pack/file", "Packs/original_pack/file"
+        "Packs/original_pack/file", "Packs/original_pack/file", None
     )
     assert not validator_obj.is_valid_pack_name(
-        "Packs/original_pack/file", "Packs/original_pack_v2/file"
+        "Packs/original_pack/file", "Packs/original_pack_v2/file", None
     )
 
 
-def test_image_error(capsys):
+def test_image_error(set_git_test_env, capsys):
     """
     Given
             a image that isn't located in the right folder.
     When
             Validating the file
     Then
             Ensure an error is raised, and  the right error is given.
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/validate/validate_manager.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/validate/validate_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,21 +145,19 @@
     get_pack_ignore_file_path,
     get_pack_name,
     get_pack_names_from_files,
     get_relative_path_from_packs_dir,
     get_remote_file,
     get_yaml,
     open_id_set_file,
-    print_warning,
     run_command_os,
 )
 from demisto_sdk.commands.create_id_set.create_id_set import IDSetCreator
 
 SKIPPED_FILES = [
-    "CommonServerPython.py",
     "CommonServerUserPython.py",
     "demistomock.py",
     "DemistoClassApiModule.py",
 ]
 
 
 class ValidateManager:
@@ -286,14 +284,27 @@
         self.ignored_files = set()
         self.new_packs = set()
         self.skipped_file_types = (
             FileType.CHANGELOG,
             FileType.DOC_IMAGE,
             FileType.MODELING_RULE_SCHEMA,
             FileType.XSIAM_REPORT_IMAGE,
+            FileType.PIPFILE,
+            FileType.PIPFILE_LOCK,
+            FileType.TXT,
+            FileType.JAVASCRIPT_FILE,
+            FileType.POWERSHELL_FILE,
+            FileType.PYLINTRC,
+            FileType.SECRET_IGNORE,
+            FileType.LICENSE,
+            FileType.UNIFIED_YML,
+            FileType.PACK_IGNORE,
+            FileType.INI,
+            FileType.PEM,
+            FileType.METADATA,
         )
 
         self.is_external_repo = is_external_repo
         if is_external_repo:
             if not self.no_configuration_prints:
                 click.echo("Running in a private repository")
             self.skip_conf_json = True
@@ -407,14 +418,15 @@
 
         else:
             return PathLevel.PACKAGE
 
     def run_validation_on_specific_files(self):
         """Run validations only on specific files"""
         files_validation_result = set()
+        self.setup_git_params()
 
         for path in self.file_path.split(","):
             error_ignore_list = self.get_error_ignore_list(get_pack_name(path))
             file_level = self.detect_file_level(path)
 
             if file_level == PathLevel.FILE:
                 click.secho(
@@ -627,35 +639,19 @@
         return (
             parent_name in {"XSIAMDashboards", "XSIAMReports"}
             or dir_name == "XDRCTemplates"
         )
 
     def run_validation_on_package(self, package_path, pack_error_ignore_list):
         package_entities_validation_results = set()
-
         for file_name in os.listdir(package_path):
             file_path = os.path.join(package_path, file_name)
-            should_validate_xsiam_item = self.should_validate_xsiam_content(
-                package_path
-            )
-            should_validate_py_file = (
-                file_path.endswith(".py") and file_name not in SKIPPED_FILES
+            package_entities_validation_results.add(
+                self.run_validations_on_file(file_path, pack_error_ignore_list)
             )
-            if (
-                file_path.endswith(".yml")
-                or file_path.endswith(".md")
-                or should_validate_py_file
-                or should_validate_xsiam_item
-            ):
-                package_entities_validation_results.add(
-                    self.run_validations_on_file(file_path, pack_error_ignore_list)
-                )
-
-            else:
-                self.ignored_files.add(file_path)
 
         return all(package_entities_validation_results)
 
     def run_validation_on_generic_entities(self, dir_path, pack_error_ignore_list):
         """
         Gets a generic content entity directory (i.e a sub-directory of GenericTypes or GenericFields)
         and runs validation within it.
@@ -673,15 +669,15 @@
                 )
             else:
                 self.ignored_files.add(file_path)
 
         return all(package_entities_validation_results)
 
     @error_codes("BA114")
-    def is_valid_pack_name(self, file_path, old_file_path):
+    def is_valid_pack_name(self, file_path, old_file_path, ignored_errors):
         """
         Valid pack name is currently considered to be a new pack name or an existing pack.
         If pack name is changed, will return `False`.
         """
         if not old_file_path:
             return True
         original_pack_name = get_pack_name(old_file_path)
@@ -689,39 +685,57 @@
         if original_pack_name != new_pack_name:
             error_message, error_code = Errors.changed_pack_name(original_pack_name)
             if self.handle_error(
                 error_message=error_message,
                 error_code=error_code,
                 file_path=file_path,
                 drop_line=True,
+                ignored_errors=ignored_errors,
             ):
                 return False
         return True
 
     @error_codes("BA102,IM110")
-    def is_valid_file_type(self, file_type: FileType, file_path: str):
+    def is_valid_file_type(
+        self, file_type: FileType, file_path: str, ignored_errors: dict
+    ):
         """
         If a file_type is unsupported, will return `False`.
         """
         if not file_type:
             error_message, error_code = Errors.file_type_not_supported(
                 file_type, file_path
             )
             if str(file_path).endswith(".png"):
                 error_message, error_code = Errors.invalid_image_name_or_location()
             if self.handle_error(
                 error_message=error_message,
                 error_code=error_code,
                 file_path=file_path,
                 drop_line=True,
+                ignored_errors=ignored_errors,
             ):
                 return False
 
         return True
 
+    def is_skipped_file(self, file_path: str) -> bool:
+        """check wether the file in the given file_path is in the SKIPPED_FILES list.
+
+        Args:
+            file_path: the file on which to run.
+
+        Returns:
+            bool. true if file is in SKIPPED_FILES list, false otherwise.
+        """
+        path = Path(file_path)
+        return path.name in SKIPPED_FILES or (
+            path.name == "CommonServerPython.py" and path.parent.parent.name != "Base"
+        )
+
     # flake8: noqa: C901
     def run_validations_on_file(
         self,
         file_path,
         pack_error_ignore_list,
         is_modified=False,
         old_file_path=None,
@@ -737,29 +751,42 @@
             pack_error_ignore_list: A dictionary of all pack ignored errors
             file_path: the file on which to run.
             is_modified: whether the file is modified or added.
 
         Returns:
             bool. true if file is valid, false otherwise.
         """
-        if not self.is_valid_pack_name(file_path, old_file_path):
+        if not self.is_valid_pack_name(
+            file_path, old_file_path, pack_error_ignore_list
+        ):
             return False
         file_type = find_type(file_path)
 
         is_added_file = file_path in added_files if added_files else False
-
-        if file_type in self.skipped_file_types or file_path.endswith("_unified.yml"):
+        if file_type == FileType.MODELING_RULE_TEST_DATA:
+            file_path = file_path.replace("_testdata.json", ".yml")
+        if file_path.endswith(".xif"):
+            file_path = file_path.replace(".xif", ".yml")
+        if (
+            file_type in self.skipped_file_types
+            or self.is_skipped_file(file_path)
+            or self.git_util._is_file_git_ignored(file_path)
+            or self.detect_file_level(file_path)
+            in (PathLevel.PACKAGE, PathLevel.CONTENT_ENTITY_DIR)
+        ):
             self.ignored_files.add(file_path)
             return True
-        elif not self.is_valid_file_type(file_type, file_path):
+        elif not self.is_valid_file_type(file_type, file_path, pack_error_ignore_list):
             return False
 
         if file_type == FileType.XSOAR_CONFIG:
             xsoar_config_validator = XSOARConfigJsonValidator(
-                file_path, specific_validations=self.specific_validations
+                file_path,
+                specific_validations=self.specific_validations,
+                ignored_errors=pack_error_ignore_list,
             )
             return xsoar_config_validator.is_valid_xsoar_config_file()
 
         if not self.check_only_schema:
             validation_print = f"\nValidating {file_path} as {file_type.value}"
             if self.print_percent:
                 if FOUND_FILES_AND_ERRORS:
@@ -816,15 +843,18 @@
         valid_in_conf = True
         if self.check_is_unskipped and file_type in {
             FileType.INTEGRATION,
             FileType.SCRIPT,
             FileType.BETA_INTEGRATION,
         }:
             if not self.conf_json_validator.is_valid_file_in_conf_json(
-                structure_validator.current_file, file_type, file_path
+                structure_validator.current_file,
+                file_type,
+                file_path,
+                pack_error_ignore_list,
             ):
                 valid_in_conf = False
 
         # Note: these file are not ignored but there are no additional validators for connections
         if file_type == FileType.CONNECTION:
             return True
 
@@ -837,15 +867,14 @@
         elif file_type == FileType.RELEASE_NOTES:
             if not self.skip_pack_rn_validation:
                 return self.validate_release_notes(
                     file_path,
                     added_files,
                     modified_files,
                     pack_error_ignore_list,
-                    is_modified,
                 )
             else:
                 click.secho("Skipping release notes validation", fg="yellow")
 
         elif file_type == FileType.RELEASE_NOTES_CONFIG:
             return self.validate_release_notes_config(file_path, pack_error_ignore_list)
 
@@ -855,14 +884,15 @@
         elif file_type == FileType.README:
             if not self.is_possible_validate_readme:
                 error_message, error_code = Errors.error_uninstall_node()
                 if self.handle_error(
                     error_message=error_message,
                     error_code=error_code,
                     file_path=file_path,
+                    ignored_errors=pack_error_ignore_list,
                 ):
                     return False
             if not self.validate_all:
                 ReadMeValidator.add_node_env_vars()
                 if (
                     not ReadMeValidator.are_modules_installed_for_verify(
                         get_content_path()  # type: ignore
@@ -1044,22 +1074,29 @@
             return self.validate_job(structure_validator, pack_error_ignore_list)
 
         elif file_type == FileType.CONTRIBUTORS:
             # This is temporarily - need to add a proper contributors validations
             return True
 
         else:
-            return self.file_type_not_supported(file_type, file_path)
+            return self.file_type_not_supported(
+                file_type, file_path, pack_error_ignore_list
+            )
         return True
 
     @error_codes("BA102")
-    def file_type_not_supported(self, file_type: FileType, file_path: str):
+    def file_type_not_supported(
+        self, file_type: FileType, file_path: str, ignored_errors: dict
+    ):
         error_message, error_code = Errors.file_type_not_supported(file_type, file_path)
         if self.handle_error(
-            error_message=error_message, error_code=error_code, file_path=file_path
+            error_message=error_message,
+            error_code=error_code,
+            file_path=file_path,
+            ignored_errors=ignored_errors,
         ):
             return False
         return True
 
     @staticmethod
     def get_file_by_status(
         modified_files: Set, old_format_files: Set, file_path: str
@@ -1271,37 +1308,43 @@
             ignored_errors=pack_error_ignore_list,
             print_as_warnings=self.print_ignored_errors,
             json_file_path=self.json_file_path,
         )
         return test_playbook_validator.is_valid_test_playbook(validate_rn=False)
 
     @error_codes("RN108")
-    def validate_no_release_notes_for_new_pack(self, pack_name, file_path):
+    def validate_no_release_notes_for_new_pack(
+        self, pack_name, file_path, ignored_errors
+    ):
         if pack_name in self.new_packs:
             error_message, error_code = Errors.added_release_notes_for_new_pack(
                 pack_name
             )
             if self.handle_error(
-                error_message=error_message, error_code=error_code, file_path=file_path
+                error_message=error_message,
+                error_code=error_code,
+                file_path=file_path,
+                ignored_errors=ignored_errors,
             ):
                 return False
         return True
 
     def validate_release_notes(
         self,
         file_path,
         added_files,
         modified_files,
         pack_error_ignore_list,
-        is_modified,
     ):
         pack_name = get_pack_name(file_path)
 
         # added new RN to a new pack
-        if not self.validate_no_release_notes_for_new_pack(pack_name, file_path):
+        if not self.validate_no_release_notes_for_new_pack(
+            pack_name, file_path, pack_error_ignore_list
+        ):
             return False
 
         if pack_name != "NonSupported":
             if not added_files:
                 added_files = {file_path}
 
             release_notes_validator = ReleaseNotesValidator(
@@ -1965,31 +2008,39 @@
             f"\n================= Checking for prohibited deleted files =================",
             fg="bright_cyan",
         )
 
         is_valid = True
         for file_path in deleted_files:
             file_path = Path(file_path)
+            ignored_errors = self.get_error_ignore_list(get_pack_name(str(file_path)))
             if "Packs" not in file_path.absolute().parts:
                 # not allowed to delete non-content files
                 file_path = str(file_path)
                 error_message, error_code = Errors.file_cannot_be_deleted(file_path)
-                if self.handle_error(error_message, error_code, file_path):
+                if self.handle_error(
+                    error_message, error_code, file_path, ignored_errors=ignored_errors
+                ):
                     is_valid = False
 
             else:
                 if not self.was_file_renamed_but_labeled_as_deleted(
                     file_path, added_files
                 ):
                     if not self.is_file_allowed_to_be_deleted(file_path):
                         file_path = str(file_path)
                         error_message, error_code = Errors.file_cannot_be_deleted(
                             file_path
                         )
-                        if self.handle_error(error_message, error_code, file_path):
+                        if self.handle_error(
+                            error_message,
+                            error_code,
+                            file_path,
+                            ignored_errors=ignored_errors,
+                        ):
                             is_valid = False
 
         return is_valid
 
     def validate_changed_packs_unique_files(
         self, modified_files, added_files, old_format_files, changed_meta_files
     ):
@@ -2039,15 +2090,21 @@
         handle_error = True
         for file_path in old_format_files:
             click.echo(f"Validating old-format file {file_path}")
             yaml_data = get_yaml(file_path)
             # we only fail on old format if no toversion (meaning it is latest) or if the ynl is not deprecated.
             if "toversion" not in yaml_data and not yaml_data.get("deprecated"):
                 error_message, error_code = Errors.invalid_package_structure()
-                if self.handle_error(error_message, error_code, file_path=file_path):
+                ignored_errors = self.get_error_ignore_list(get_pack_name(file_path))
+                if self.handle_error(
+                    error_message,
+                    error_code,
+                    file_path=file_path,
+                    ignored_errors=ignored_errors,
+                ):
                     handle_error = False
         return handle_error
 
     @error_codes("RN105")
     def validate_no_duplicated_release_notes(self, added_files):
         """Validated that among the added files - there are no duplicated RN for the same pack.
 
@@ -2065,16 +2122,20 @@
         for file in added_files:
             if find_type(file) == FileType.RELEASE_NOTES:
                 pack_name = get_pack_name(file)
                 if pack_name not in added_rn:
                     added_rn.add(pack_name)
                 else:
                     error_message, error_code = Errors.multiple_release_notes_files()
+                    ignored_errors = self.get_error_ignore_list(pack_name)
                     if self.handle_error(
-                        error_message, error_code, file_path=pack_name
+                        error_message,
+                        error_code,
+                        file_path=pack_name,
+                        ignored_errors=ignored_errors,
                     ):
                         return False
 
         click.secho("\nNo duplicated release notes found.\n", fg="bright_green")
         return True
 
     @error_codes("RN106")
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/README.md` & `demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/README.md`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/packs_zipper.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/packs_zipper.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/commands/zip_packs/tests/packs_zipper_test.py` & `demisto_sdk-1.9.0/demisto_sdk/commands/zip_packs/tests/packs_zipper_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_client.py` & `demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_client.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier.py` & `demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,15 +293,14 @@
         circle_client=circle_ci_client, workflow_id=circle_ci_workflow_id
     )
 
     if slack_message := construct_failed_jobs_slack_message(parser=circle_ci_parser):
         slack_client = WebClient(token=slack_token)
         slack_client.chat_postMessage(
             channel=slack_channel,
-            as_user=False,
             attachments=slack_message,
             username="Demisto-SDK CircleCI",
         )
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier_test.py` & `demisto_sdk-1.9.0/demisto_sdk/utils/circle-ci/circle_ci_slack_notifier_test.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/deploy.sh` & `demisto_sdk-1.9.0/demisto_sdk/utils/deploy.sh`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/server_schema_change_slack_notifier.py` & `demisto_sdk-1.9.0/demisto_sdk/utils/server_schema_change_slack_notifier.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/demisto_sdk/utils/utils.py` & `demisto_sdk-1.9.0/demisto_sdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `demisto_sdk-1.8.3/pyproject.toml` & `demisto_sdk-1.9.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "demisto-sdk"
-version = "1.8.3"
+version = "1.9.0"
 description = "\"A Python library for the Demisto SDK\""
 authors = ["Demisto"]
 license = "MIT"
 readme = "README.md"
 classifiers=[
     'Intended Audience :: Developers',
     'Natural Language :: English',
```

### Comparing `demisto_sdk-1.8.3/setup.py` & `demisto_sdk-1.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 {'build': ['gsutil==5.17']}
 
 entry_points = \
 {'console_scripts': ['demisto-sdk = demisto_sdk.__main__:main']}
 
 setup_kwargs = {
     'name': 'demisto-sdk',
-    'version': '1.8.3',
+    'version': '1.9.0',
     'description': '"A Python library for the Demisto SDK"',
     'long_description': '# Demisto SDK\n\n[![PyPI version](https://badge.fury.io/py/demisto-sdk.svg)](https://badge.fury.io/py/demisto-sdk)\n[![CircleCI](https://circleci.com/gh/demisto/demisto-sdk/tree/master.svg?style=svg)](https://circleci.com/gh/demisto/demisto-sdk/tree/master)\n[![Coverage Status](https://coveralls.io/repos/github/demisto/demisto-sdk/badge.svg?branch=master)](https://coveralls.io/github/demisto/demisto-sdk?branch=master)\n\nThe Demisto SDK library can be used to manage your Cortex XSOAR content with ease and efficiency.\nThe library uses python 3.8+.\n\n## Usage\n\n### Installation\n\n1. **Install** - `pip3 install demisto-sdk`\n2. **Upgrade** - `pip3 install --upgrade demisto-sdk`\n3. **Connect demisto-sdk with Cortex XSOAR server** - In order that demisto-sdk and Cortex XSOAR server communicate, perfrom the following steps:\n\n   1. Get an API key for Cortex XSOAR/XSIAM-server - `Settings` -> `Integrations` -> `API keys` -> `Get your Key` (copy it)\n   2. Add the following parameters to your environment. You can also use a [.env file](https://pypi.org/project/python-dotenv/), the demisto-sdk will automatically load that file.:\n\n      ```bash\n      export DEMISTO_BASE_URL=<http or https>://<demisto-server url or ip>:<port>\n      export DEMISTO_API_KEY=<API key>\n      ```\n      To use on Cortex XSIAM the `XSIAM_AUTH_ID` environment variable should also be set.\n      ```bash\n      export XSIAM_AUTH_ID=<auth id>\n      ```\n\n      for example:\n      ```bash\n      export DEMISTO_BASE_URL=http://127.0.0.1:8080\n      export DEMISTO_API_KEY=XXXXXXXXXXXXXXXXXXXXXX\n      ```\n      As long as `XSIAM_AUTH_ID` environment variable is set, SDK commands will be configured to work with an XSIAM instance.\n      In order to set Demisto SDK to work with Cortex XSOAR instance, you need to delete the XSIAM_AUTH_ID parameter from your environment.\n      ```bash\n      unset XSIAM_AUTH_ID\n      ```\n\n      >For more configurations, check the [demisto-py](https://github.com/demisto/demisto-py) repo (the SDK uses demisto-py to communicate with Cortex XSOAR).\n\n   3. For the **Validate** and **Format** commands to work properly:\n     - Install node.js, and make sure `@mdx-js/mdx`, `fs-extra` and `commander` are installed in node-modules folder (`npm install ...`).\n     - Set the `DEMISTO_README_VALIDATION` environment variable to True.\n\n       MDX is used to validate markdown files, and make sure they render properly on XSOAR and [xsoar.pan.dev](https://xsoar.pan.dev).\n\n   4. Reload your terminal.\n\n---\n\n### Content path\n\nThe **demisto-sdk** is made to work with Cortex content, structured similar to the [official Cortex content repo](https://github.com/demisto/content).\n\nDemisto-SDK commands work best when called from the content directory or any of its subfolders.\nTo run Demisto-SDK commands from other folders, you may set the `DEMISTO_SDK_CONTENT_PATH` environment variable.\n\nWe recommend running all demisto-SDK commands from a folder with a git repo, or any of its subfolders. To suppress warnings about running commands outside of a content repo folder, set the `DEMISTO_SDK_IGNORE_CONTENT_WARNING` environment variable.\n\n### CLI usage\n\nYou can use the SDK in the CLI as follows:\n\n```bash\ndemisto-sdk <command> <args>\n```\n\nFor more information, run `demisto-sdk -h`.\nFor more information on a specific command execute `demisto-sdk <command> -h`.\n\n### Version Check\n\n`demisto-sdk` will check against the GitHub repository releases for a new version every time it runs and will issue a warning if you are not using the latest and greatest. If you wish to skip this check you can set the environment variable: `DEMISTO_SDK_SKIP_VERSION_CHECK`. For example:\n\n```bash\nexport DEMISTO_SDK_SKIP_VERSION_CHECK=yes\n```\n\n---\n\n## Commands\n\nSupported commands:\n\n1. [init](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/init/README.md)\n1. [Validate](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/validate/README.md)\n1. [Lint](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/lint/README.md)\n1. [Secrets](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/secrets/README.md)\n2. [Unify](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/prepare_content/README.md#Unify)\n3. [Prepare-Content](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/prepare_content/README.md#prepare-content)\n4. [Split](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/split/README.md)\n5. [Format](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/format/README.md)\n6. [Run](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/run_cmd/README.md)\n7. [Run-playbook](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/run_playbook/README.md)\n8. [Upload](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/upload/README.md)\n9. [Download](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/download/README.md)\n10. [Generate-docs](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/generate_docs/README.md)\n11. [Generate-test-playbook](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/generate_test_playbook/README.md)\n12. [Generate-outputs](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/generate_outputs/README.md)\n13. [Update-release-notes](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/update_release_notes/README.md)\n14. [Zip-packs](https://github.com/demisto/demisto-sdk/blob/master/demisto_sdk/commands/zip_packs/README.md)\n15. [openapi-codegen](https://xsoar.pan.dev/docs/integrations/openapi-codegen)\n16. [postman-codegen](https://xsoar.pan.dev/docs/integrations/postman-codegen)\n17. [generate-integration](https://xsoar.pan.dev/docs/integrations/code-generator)\n18. [generate-yml-from-python](https://xsoar.pan.dev/docs/integrations/yml-from-python-code-gen)\n---\n\n### Customizable command configuration\n\nYou can create your own configuration for the `demisto-sdk` commands by creating a file named `.demisto-sdk-conf` within the directory from which you run the commands.\nThis file will enable you to set a default value to the existing command flags that will take effect whenever the command is run.\nThis can be done by entering the following structure into the file:\n\n```INI\n[command_name]\nflag_name=flag_default_value\n```\n\nNote: Make sure to use the flag\'s full name and input `_` instead of a `-` if it exists in the flag name (e.g. instead of `no-docker-checks` use `no_docker_checks`).\n\nHere are a few examples:\n\n- As a user, I would like to not use the `mypy` linter in my environment when using the `lint` command. In the `.demisto-sdk-conf` file I\'ll enter:\n\n ```INI\n[lint]\nno_mypy=true\n```\n\n- As a user, I would like to include untracked git files in my validation when running the `validate` command. In the `.demisto-sdk-conf` file I\'ll enter:\n\n```INI\n[validate]\ninclude_untracked=true\n```\n\n- As a user, I would like to automatically use minor version changes when running the `update-release-notes` command. In the `.demisto-sdk-conf` file I\'ll enter:\n\n```INI\n[update-release-notes]\nupdate_type=minor\n```\n\n---\n\n### Autocomplete\n\nOur CLI supports autocomplete for Linux/MacOS machines, you can turn this feature on by running one of the following:\nfor zsh users run in the terminal\n\n```bash\neval "$(_DEMISTO_SDK_COMPLETE=source_zsh demisto-sdk)"\n```\n\nfor regular bashrc users run in the terminal\n\n```bash\neval "$(_DEMISTO_SDK_COMPLETE=source demisto-sdk)"\n```\n\n---\n\n## License\n\nMIT - See [LICENSE](LICENSE) for more information.\n\n---\n\n## How to setup development environment?\n\nFollow the guide found [here](CONTRIBUTION.md#2-install-demisto-sdk-dev-environment) to setup your `demisto-sdk` dev environment.\nThe development environment is connected to the branch you are currently using in the SDK repository.\n\n---\n\n## Contributions\n\nContributions are welcome and appreciated.\nFor information regarding contributing, press [here](CONTRIBUTION.md).\nFor release guide, press [here](docs/release_guide.md)\n',
     'author': 'Demisto',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `demisto_sdk-1.8.3/PKG-INFO` & `demisto_sdk-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demisto-sdk
-Version: 1.8.3
+Version: 1.9.0
 Summary: "A Python library for the Demisto SDK"
 License: MIT
 Author: Demisto
 Requires-Python: >=3.8,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

