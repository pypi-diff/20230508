# Comparing `tmp/robusta-cli-0.9.7.tar.gz` & `tmp/robusta-cli-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robusta-cli-0.9.7.tar", max compression
+gzip compressed data, was "robusta-cli-0.9.9.tar", max compression
```

## Comparing `robusta-cli-0.9.7.tar` & `robusta-cli-0.9.9.tar`

### file list

```diff
@@ -1,169 +1,174 @@
--rw-r--r--   0        0        0     1072 2022-04-16 21:23:00.149878 robusta-cli-0.9.7/LICENSE
--rw-r--r--   0        0        0     2621 2022-04-16 21:23:17.318072 robusta-cli-0.9.7/pyproject.toml
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/__init__.py
--rw-r--r--   0        0        0       74 2022-04-16 21:23:17.318072 robusta-cli-0.9.7/src/robusta/_version.py
--rw-r--r--   0        0        0     1901 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/api/__init__.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/__init__.py
--rw-r--r--   0        0        0     1078 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/backend_profile.py
--rw-r--r--   0        0        0     2045 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/integrations_cmd.py
--rwxr-xr-x   0        0        0    14626 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/main.py
--rw-r--r--   0        0        0    10995 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/playbooks_cmd.py
--rw-r--r--   0        0        0     2834 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/slack_verification.py
--rw-r--r--   0        0        0     2831 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/cli/utils.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/__init__.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/discovery/__init__.py
--rw-r--r--   0        0        0     2480 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/discovery/top_service_resolver.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/__init__.py
--rw-r--r--   0        0        0     4130 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/base_params.py
--rw-r--r--   0        0        0      172 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/cluster_status.py
--rw-r--r--   0        0        0     2599 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/env_vars.py
--rw-r--r--   0        0        0     3166 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/events.py
--rw-r--r--   0        0        0      120 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/k8s_operation_type.py
--rw-r--r--   0        0        0     2375 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/nodes.py
--rw-r--r--   0        0        0     1749 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/runner_config.py
--rw-r--r--   0        0        0      670 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/model/services.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/persistency/__init__.py
--rw-r--r--   0        0        0      585 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/persistency/in_memory.py
--rw-r--r--   0        0        0     2789 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/persistency/scheduled_jobs_states_dal.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/__init__.py
--rw-r--r--   0        0        0     3930 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/actions_registry.py
--rw-r--r--   0        0        0      806 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/base_trigger.py
--rw-r--r--   0        0        0     1831 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/common.py
--rw-r--r--   0        0        0     6526 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/generation.py
--rw-r--r--   0        0        0     2774 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/internal/discovery_events.py
--rw-r--r--   0        0        0     1179 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/playbook_utils.py
--rw-r--r--   0        0        0     1386 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/playbooks_event_handler.py
--rw-r--r--   0        0        0     9444 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/playbooks_event_handler_impl.py
--rw-r--r--   0        0        0     6698 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/prometheus_enrichment_utils.py
--rw-r--r--   0        0        0     1065 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/playbooks/trigger.py
--rw-r--r--   0        0        0      236 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/__init__.py
--rw-r--r--   0        0        0     1404 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/action_requests.py
--rw-r--r--   0        0        0     4513 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/base.py
--rw-r--r--   0        0        0     9781 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/blocks.py
--rw-r--r--   0        0        0     1954 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/callbacks.py
--rw-r--r--   0        0        0     1362 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/consts.py
--rw-r--r--   0        0        0      457 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/custom_rendering.py
--rw-r--r--   0        0        0     1421 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/finding_subjects.py
--rw-r--r--   0        0        0     1109 2022-04-16 21:23:00.209879 robusta-cli-0.9.7/src/robusta/core/reporting/utils.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/schedule/__init__.py
--rw-r--r--   0        0        0      932 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/schedule/model.py
--rw-r--r--   0        0        0     6113 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/schedule/scheduler.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/__init__.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/datadog/__init__.py
--rw-r--r--   0        0        0     4540 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/datadog/datadog_sink.py
--rw-r--r--   0        0        0      312 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/datadog/datadog_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/kafka/__init__.py
--rw-r--r--   0        0        0     2757 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/kafka/kafka_sink.py
--rw-r--r--   0        0        0      318 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/kafka/kafka_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/msteams/__init__.py
--rw-r--r--   0        0        0      626 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/msteams/msteams_sink.py
--rw-r--r--   0        0        0      318 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/msteams/msteams_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/opsgenie/__init__.py
--rw-r--r--   0        0        0     2558 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/opsgenie/opsgenie_sink.py
--rw-r--r--   0        0        0      393 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/opsgenie/opsgenie_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/robusta/__init__.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/robusta/dal/__init__.py
--rw-r--r--   0        0        0    14856 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/robusta/dal/supabase_dal.py
--rw-r--r--   0        0        0    13834 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/robusta/robusta_sink.py
--rw-r--r--   0        0        0      468 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/robusta/robusta_sink_params.py
--rw-r--r--   0        0        0      894 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/sink_base.py
--rw-r--r--   0        0        0      359 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/sink_base_params.py
--rw-r--r--   0        0        0      320 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/sink_config.py
--rw-r--r--   0        0        0     2094 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/sink_factory.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/slack/__init__.py
--rw-r--r--   0        0        0      816 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/slack/slack_sink.py
--rw-r--r--   0        0        0      324 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/slack/slack_sink_params.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/telegram/__init__.py
--rw-r--r--   0        0        0     1685 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/telegram/telegram_client.py
--rw-r--r--   0        0        0     3396 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/telegram/telegram_sink.py
--rw-r--r--   0        0        0      409 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/telegram/telegram_sink_params.py
--rw-r--r--   0        0        0     5260 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/transformer.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/webhook/__init__.py
--rw-r--r--   0        0        0     2708 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/webhook/webhook_sink.py
--rw-r--r--   0        0        0      335 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/sinks/webhook/webhook_sink_params.py
--rw-r--r--   0        0        0      564 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/triggers/custom_triggers.py
--rw-r--r--   0        0        0     3718 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/core/triggers/error_event_trigger.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/__init__.py
--rw-r--r--   0        0        0      859 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/argocd/argocd_client.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/git/__init__.py
--rw-r--r--   0        0        0     9793 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/git/git_repo.py
--rw-r--r--   0        0        0     3648 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/grafana.py
--rw-r--r--   0        0        0      394 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/helper.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/__init__.py
--rw-r--r--   0        0        0     8041 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/api_client_utils.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/__init__.py
--rw-r--r--   0        0        0    26674 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/events.py
--rw-r--r--   0        0        0      474 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/models.py
--rw-r--r--   0        0        0    36770 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/triggers.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v1/__init__.py
--rw-r--r--   0        0        0      657 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v1/models.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta1/__init__.py
--rw-r--r--   0        0        0      662 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta1/models.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta2/__init__.py
--rw-r--r--   0        0        0      662 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta2/models.py
--rw-r--r--   0        0        0     1283 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/base_event.py
--rw-r--r--   0        0        0     5144 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/base_triggers.py
--rw-r--r--   0        0        0    12715 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/custom_models.py
--rw-r--r--   0        0        0       88 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/model_not_found_exception.py
--rw-r--r--   0        0        0     5100 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/process_utils.py
--rw-r--r--   0        0        0      578 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/kubernetes/templates.py
--rw-r--r--   0        0        0        1 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/__init__.py
--rw-r--r--   0        0        0     1216 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files.py
--rw-r--r--   0        0        0     2504 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files_image.py
--rw-r--r--   0        0        0     7202 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files_text.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/__init__.py
--rw-r--r--   0        0        0     1088 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_action.py
--rw-r--r--   0        0        0      167 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_base.py
--rw-r--r--   0        0        0      759 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_card.py
--rw-r--r--   0        0        0     1115 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_column.py
--rw-r--r--   0        0        0      707 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_container.py
--rw-r--r--   0        0        0      941 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_images.py
--rw-r--r--   0        0        0     1141 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_table.py
--rw-r--r--   0        0        0     2056 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_text_block.py
--rw-r--r--   0        0        0      602 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_mark_down_fix_url.py
--rw-r--r--   0        0        0     6685 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_msg.py
--rw-r--r--   0        0        0     2223 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/msteams/sender.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/prometheus/__init__.py
--rw-r--r--   0        0        0     5098 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/prometheus/models.py
--rw-r--r--   0        0        0     5207 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/prometheus/trigger.py
--rw-r--r--   0        0        0      851 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/prometheus/utils.py
--rw-r--r--   0        0        0     5944 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/receiver.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/resource_analysis/__init__.py
--rwxr-xr-x   0        0        0     5148 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/resource_analysis/memory_analyzer.py
--rw-r--r--   0        0        0     4825 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/resource_analysis/node_cpu_analyzer.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/__init__.py
--rw-r--r--   0        0        0      384 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/event.py
--rw-r--r--   0        0        0      128 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/models.py
--rw-r--r--   0        0        0      555 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/playbook_scheduler.py
--rw-r--r--   0        0        0      330 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/playbook_scheduler_manager.py
--rw-r--r--   0        0        0     5193 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/playbook_scheduler_manager_impl.py
--rw-r--r--   0        0        0     1318 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/scheduled/trigger.py
--rw-r--r--   0        0        0       22 2022-04-16 21:23:00.213879 robusta-cli-0.9.7/src/robusta/integrations/slack/__init__.py
--rw-r--r--   0        0        0     9949 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/integrations/slack/sender.py
--rw-r--r--   0        0        0     8402 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/model/config.py
--rw-r--r--   0        0        0      644 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/model/playbook_action.py
--rw-r--r--   0        0        0     1423 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/model/playbook_definition.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/__init__.py
--rw-r--r--   0        0        0    12233 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/config_loader.py
--rw-r--r--   0        0        0      927 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/log_init.py
--rw-r--r--   0        0        0     1361 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/main.py
--rw-r--r--   0        0        0      162 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/not_found_exception.py
--rw-r--r--   0        0        0      517 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/object_updater.py
--rw-r--r--   0        0        0      531 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/telemetry.py
--rw-r--r--   0        0        0     2116 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/telemetry_service.py
--rw-r--r--   0        0        0     3081 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/web.py
--rw-r--r--   0        0        0     1234 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/runner/web_api.py
--rw-r--r--   0        0        0        0 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/__init__.py
--rw-r--r--   0        0        0     1337 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/common.py
--rw-r--r--   0        0        0      562 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/decorators.py
--rw-r--r--   0        0        0     1681 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/docs.py
--rw-r--r--   0        0        0     2424 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/documented_pydantic.py
--rw-r--r--   0        0        0     1648 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/file_system_watcher.py
--rw-r--r--   0        0        0      950 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/function_hashes.py
--rw-r--r--   0        0        0     6176 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/json_schema.py
--rw-r--r--   0        0        0      374 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/parsing.py
--rw-r--r--   0        0        0     1253 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/rate_limiter.py
--rw-r--r--   0        0        0      892 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/service_discovery.py
--rw-r--r--   0        0        0     2356 2022-04-16 21:23:00.217879 robusta-cli-0.9.7/src/robusta/utils/task_queue.py
--rw-r--r--   0        0        0     2972 2022-04-16 21:26:47.897353 robusta-cli-0.9.7/setup.py
--rw-r--r--   0        0        0     1854 2022-04-16 21:26:47.897752 robusta-cli-0.9.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-04-27 08:11:50.425188 robusta-cli-0.9.9/LICENSE
+-rw-r--r--   0        0        0     2719 2022-04-27 08:12:06.645269 robusta-cli-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/__init__.py
+-rw-r--r--   0        0        0       74 2022-04-27 08:12:06.645269 robusta-cli-0.9.9/src/robusta/_version.py
+-rw-r--r--   0        0        0     1933 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/api/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/__init__.py
+-rw-r--r--   0        0        0     4933 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/auth.py
+-rw-r--r--   0        0        0     1189 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/backend_profile.py
+-rw-r--r--   0        0        0     2045 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/integrations_cmd.py
+-rwxr-xr-x   0        0        0    16946 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/main.py
+-rw-r--r--   0        0        0    10995 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/playbooks_cmd.py
+-rw-r--r--   0        0        0     3030 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/slack_feedback_message.py
+-rw-r--r--   0        0        0     2838 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/slack_verification.py
+-rw-r--r--   0        0        0     2831 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/cli/utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/discovery/__init__.py
+-rw-r--r--   0        0        0     2480 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/discovery/top_service_resolver.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/__init__.py
+-rw-r--r--   0        0        0     4130 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/base_params.py
+-rw-r--r--   0        0        0      172 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/cluster_status.py
+-rw-r--r--   0        0        0     2750 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/env_vars.py
+-rw-r--r--   0        0        0     3457 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/events.py
+-rw-r--r--   0        0        0      120 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/k8s_operation_type.py
+-rw-r--r--   0        0        0      939 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/nodes.py
+-rw-r--r--   0        0        0     2549 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/pods.py
+-rw-r--r--   0        0        0     1749 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/runner_config.py
+-rw-r--r--   0        0        0      670 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/model/services.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/__init__.py
+-rw-r--r--   0        0        0      585 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/in_memory.py
+-rw-r--r--   0        0        0     2789 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/persistency/scheduled_jobs_states_dal.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/__init__.py
+-rw-r--r--   0        0        0     3930 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/actions_registry.py
+-rw-r--r--   0        0        0      806 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/base_trigger.py
+-rw-r--r--   0        0        0     1831 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/common.py
+-rw-r--r--   0        0        0     6526 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/generation.py
+-rw-r--r--   0        0        0     2774 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/internal/discovery_events.py
+-rw-r--r--   0        0        0     1179 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbook_utils.py
+-rw-r--r--   0        0        0     1523 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler.py
+-rw-r--r--   0        0        0    11530 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler_impl.py
+-rw-r--r--   0        0        0     6698 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/prometheus_enrichment_utils.py
+-rw-r--r--   0        0        0     1065 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/playbooks/trigger.py
+-rw-r--r--   0        0        0      236 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/__init__.py
+-rw-r--r--   0        0        0     2070 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/action_requests.py
+-rw-r--r--   0        0        0     4513 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/base.py
+-rw-r--r--   0        0        0     9952 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/blocks.py
+-rw-r--r--   0        0        0     1954 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/callbacks.py
+-rw-r--r--   0        0        0     1250 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/consts.py
+-rw-r--r--   0        0        0      457 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/custom_rendering.py
+-rw-r--r--   0        0        0     1421 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/finding_subjects.py
+-rw-r--r--   0        0        0     1109 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/reporting/utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/schedule/__init__.py
+-rw-r--r--   0        0        0      932 2022-04-27 08:11:50.485189 robusta-cli-0.9.9/src/robusta/core/schedule/model.py
+-rw-r--r--   0        0        0     6113 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/schedule/scheduler.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/__init__.py
+-rw-r--r--   0        0        0     4540 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/datadog_sink.py
+-rw-r--r--   0        0        0      312 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/datadog/datadog_sink_params.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/__init__.py
+-rw-r--r--   0        0        0     2757 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/kafka_sink.py
+-rw-r--r--   0        0        0      318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/kafka/kafka_sink_params.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/__init__.py
+-rw-r--r--   0        0        0      626 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/msteams_sink.py
+-rw-r--r--   0        0        0      318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/msteams/msteams_sink_params.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/__init__.py
+-rw-r--r--   0        0        0     2558 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/opsgenie_sink.py
+-rw-r--r--   0        0        0      393 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/opsgenie_sink_params.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/__init__.py
+-rw-r--r--   0        0        0     5350 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/model_conversion.py
+-rw-r--r--   0        0        0    10151 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/supabase_dal.py
+-rw-r--r--   0        0        0    12836 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/robusta_sink.py
+-rw-r--r--   0        0        0      468 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/robusta/robusta_sink_params.py
+-rw-r--r--   0        0        0      894 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_base.py
+-rw-r--r--   0        0        0      359 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_base_params.py
+-rw-r--r--   0        0        0      320 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_config.py
+-rw-r--r--   0        0        0     2094 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/sink_factory.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/__init__.py
+-rw-r--r--   0        0        0      816 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/slack_sink.py
+-rw-r--r--   0        0        0      324 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/slack/slack_sink_params.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/__init__.py
+-rw-r--r--   0        0        0     1685 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_client.py
+-rw-r--r--   0        0        0     3473 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_sink.py
+-rw-r--r--   0        0        0      409 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_sink_params.py
+-rw-r--r--   0        0        0     5260 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/transformer.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/__init__.py
+-rw-r--r--   0        0        0     2708 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/webhook_sink.py
+-rw-r--r--   0        0        0      335 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/sinks/webhook/webhook_sink_params.py
+-rw-r--r--   0        0        0      564 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/triggers/custom_triggers.py
+-rw-r--r--   0        0        0     3718 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/core/triggers/error_event_trigger.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/__init__.py
+-rw-r--r--   0        0        0      859 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/argocd/argocd_client.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/git/__init__.py
+-rw-r--r--   0        0        0     9793 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/git/git_repo.py
+-rw-r--r--   0        0        0     3648 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/grafana.py
+-rw-r--r--   0        0        0      394 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/helper.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/__init__.py
+-rw-r--r--   0        0        0     8041 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/api_client_utils.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/__init__.py
+-rw-r--r--   0        0        0    26674 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/events.py
+-rw-r--r--   0        0        0      474 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/models.py
+-rw-r--r--   0        0        0    36770 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/triggers.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v1/__init__.py
+-rw-r--r--   0        0        0      657 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v1/models.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta1/__init__.py
+-rw-r--r--   0        0        0      662 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta1/models.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta2/__init__.py
+-rw-r--r--   0        0        0      662 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta2/models.py
+-rw-r--r--   0        0        0     1283 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_event.py
+-rw-r--r--   0        0        0     5144 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_triggers.py
+-rw-r--r--   0        0        0    13383 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/custom_models.py
+-rw-r--r--   0        0        0       88 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/model_not_found_exception.py
+-rw-r--r--   0        0        0     5100 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/process_utils.py
+-rw-r--r--   0        0        0      578 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/kubernetes/templates.py
+-rw-r--r--   0        0        0        1 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/__init__.py
+-rw-r--r--   0        0        0     1216 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files.py
+-rw-r--r--   0        0        0     2504 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_image.py
+-rw-r--r--   0        0        0     7202 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_text.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/__init__.py
+-rw-r--r--   0        0        0     1088 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_action.py
+-rw-r--r--   0        0        0      167 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_base.py
+-rw-r--r--   0        0        0      759 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_card.py
+-rw-r--r--   0        0        0     1115 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_column.py
+-rw-r--r--   0        0        0      707 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_container.py
+-rw-r--r--   0        0        0      941 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_images.py
+-rw-r--r--   0        0        0     1141 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_table.py
+-rw-r--r--   0        0        0     2056 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_text_block.py
+-rw-r--r--   0        0        0      602 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_mark_down_fix_url.py
+-rw-r--r--   0        0        0     6685 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_msg.py
+-rw-r--r--   0        0        0     2223 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/msteams/sender.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/__init__.py
+-rw-r--r--   0        0        0     5098 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/models.py
+-rw-r--r--   0        0        0     5207 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/trigger.py
+-rw-r--r--   0        0        0      851 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/prometheus/utils.py
+-rw-r--r--   0        0        0    10011 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/receiver.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/__init__.py
+-rwxr-xr-x   0        0        0     5148 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/memory_analyzer.py
+-rw-r--r--   0        0        0     4825 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/node_cpu_analyzer.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/__init__.py
+-rw-r--r--   0        0        0      384 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/event.py
+-rw-r--r--   0        0        0      128 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/models.py
+-rw-r--r--   0        0        0      555 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler.py
+-rw-r--r--   0        0        0      330 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler_manager.py
+-rw-r--r--   0        0        0     5193 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler_manager_impl.py
+-rw-r--r--   0        0        0     1318 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/scheduled/trigger.py
+-rw-r--r--   0        0        0       22 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/slack/__init__.py
+-rw-r--r--   0        0        0    10632 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/integrations/slack/sender.py
+-rw-r--r--   0        0        0     8402 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/config.py
+-rw-r--r--   0        0        0      644 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/playbook_action.py
+-rw-r--r--   0        0        0     1423 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/model/playbook_definition.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/__init__.py
+-rw-r--r--   0        0        0    12233 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/config_loader.py
+-rw-r--r--   0        0        0      927 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/log_init.py
+-rw-r--r--   0        0        0     1341 2022-04-27 08:11:50.489189 robusta-cli-0.9.9/src/robusta/runner/main.py
+-rw-r--r--   0        0        0      162 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/not_found_exception.py
+-rw-r--r--   0        0        0      517 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/object_updater.py
+-rw-r--r--   0        0        0      531 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/telemetry.py
+-rw-r--r--   0        0        0     2088 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/telemetry_service.py
+-rw-r--r--   0        0        0     3081 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/web.py
+-rw-r--r--   0        0        0     1234 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/runner/web_api.py
+-rw-r--r--   0        0        0        0 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/__init__.py
+-rw-r--r--   0        0        0     1700 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/auth_provider.py
+-rw-r--r--   0        0        0     1337 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/common.py
+-rw-r--r--   0        0        0      562 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/decorators.py
+-rw-r--r--   0        0        0     1681 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/docs.py
+-rw-r--r--   0        0        0     2424 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/documented_pydantic.py
+-rw-r--r--   0        0        0     1648 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/file_system_watcher.py
+-rw-r--r--   0        0        0      950 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/function_hashes.py
+-rw-r--r--   0        0        0     6176 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/json_schema.py
+-rw-r--r--   0        0        0      374 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/parsing.py
+-rw-r--r--   0        0        0     1253 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/rate_limiter.py
+-rw-r--r--   0        0        0      892 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/service_discovery.py
+-rw-r--r--   0        0        0     2356 2022-04-27 08:11:50.493189 robusta-cli-0.9.9/src/robusta/utils/task_queue.py
+-rw-r--r--   0        0        0     3048 2022-04-27 08:15:35.708116 robusta-cli-0.9.9/setup.py
+-rw-r--r--   0        0        0     1966 2022-04-27 08:15:35.708514 robusta-cli-0.9.9/PKG-INFO
```

### Comparing `robusta-cli-0.9.7/LICENSE` & `robusta-cli-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/pyproject.toml` & `robusta-cli-0.9.9/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robusta-cli"
-version = "0.9.7"
+version = "0.9.9"
 description = ""
 authors = ["Natan Yellin <aantn@users.noreply.github.com>"]
 packages = [
     { include = "robusta", from = "src"},
 ]
 
 [tool.poetry.scripts]
@@ -28,28 +28,30 @@
 watchdog =  { version = "^2.1.0", optional = true }
 better-exceptions = { version =  "^0.3.3", optional = true }
 CairoSVG = { version = "^2.5.2", optional = true }
 kafka-python = { version = "^2.0.2", optional = true }
 prometheus-api-client = { version = "^0.4.2", optional = true }
 datadog-api-client = { version = "^1.2.0", optional = true }
 dpath = "^2.0.5"
+websocket-client = "^1.3.2"
 prometheus-client = "^0.12.0"
 pyyaml = "^6.0"
 pytz = "^2021.3"
 docutils="^0.17.0"
-sentry-sdk = "^1.5.2"
+sentry-sdk = { version = "^1.5.2", optional = true }
 opsgenie-sdk = "^2.1.5"
 markdown2 = "^2.4.2"
 toml = "^0.10.2"
 watchgod = "^0.7"
 
 # we're freezing a specific version here because the latest version doesn't have prebuilt wheels on pypi
 # and therefore requires gcc to install which we'd like to avoid
 # this is similar to the issue at https://github.com/dulwich/dulwich/issues/839
 dulwich =  { version = "0.20.28", optional = true }
+cryptography = "^36.0.0"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^2.13.0"
 pytest = "^6.2.4"
 python-dotenv = "^0.18.0"
 Sphinx = "^4.3.2"
 furo = "^2021.11.12"
@@ -67,15 +69,15 @@
 pygal = "^3.0.0"
 tinycss = "^0.4"
 rsa = "^4.8"
 
 
 
 [tool.poetry.extras]
-all = ["Flask", "grafana-api", "manhole", "watchdog", "dulwich", "better-exceptions", "CairoSVG", "tabulate", "kafka-python", "prometheus-api-client", "supabase-py", "datadog-api-client", "pygal", "tinycss", "cssselect", "rsa"]
+all = ["Flask", "grafana-api", "manhole", "watchdog", "dulwich", "better-exceptions", "CairoSVG", "tabulate", "kafka-python", "prometheus-api-client", "supabase-py", "datadog-api-client", "pygal", "tinycss", "cssselect", "rsa", "sentry-sdk"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 # https://github.com/mtkennerly/poetry-dynamic-versioning
 # we can use this in github actions by running `poetry run poetry-dynamic-versioning`
```

### Comparing `robusta-cli-0.9.7/src/robusta/api/__init__.py` & `robusta-cli-0.9.9/src/robusta/api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from ..core.model.base_params import *
+from ..core.model.pods import *
 from ..core.sinks import *
 from ..core.sinks.sink_base import *
 from ..core.sinks.sink_config import *
 from ..core.sinks.kafka import *
 from ..core.reporting.consts import *
 from ..core.reporting.callbacks import *
 from ..core.reporting.custom_rendering import *
```

### Comparing `robusta-cli-0.9.7/src/robusta/cli/backend_profile.py` & `robusta-cli-0.9.9/src/robusta/cli/backend_profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 class BackendProfile(BaseModel):
     robusta_cloud_api_host: str = ""
     robusta_ui_domain: str = ""
     robusta_relay_ws_address: str = ""
     robusta_relay_external_actions_url: str = ""
     robusta_telemetry_endpoint: str = ""
+    robusta_store_token_url: str = ""
     custom_profile: bool = False
 
 
 # default values
 backend_profile = BackendProfile(
     robusta_cloud_api_host="https://api.robusta.dev",
     robusta_ui_domain="https://platform.robusta.dev",
+    robusta_store_token_url="https://api.robusta.dev/auth/server/tokens"
 )
 
 if ROBUSTA_BACKEND_PROFILE:
     typer.secho(
         f"Using Robusta backend profile: {ROBUSTA_BACKEND_PROFILE}",
         color="blue",
     )
```

### Comparing `robusta-cli-0.9.7/src/robusta/cli/integrations_cmd.py` & `robusta-cli-0.9.9/src/robusta/cli/integrations_cmd.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/cli/main.py` & `robusta-cli-0.9.9/src/robusta/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,47 +5,54 @@
 import time
 import urllib.request
 import uuid
 import click_spinner
 from distutils.version import StrictVersion
 from typing import Optional, List, Union, Dict
 from zipfile import ZipFile
+import traceback
 
 import requests
 import typer
 import yaml
 from kubernetes import config
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 
 # TODO - separate shared classes to a separated shared repo, to remove dependencies between the cli and runner
+from .auth import gen_rsa_pair, RSAKeyPair
 from .backend_profile import backend_profile
 from ..core.sinks.msteams.msteams_sink_params import (
     MsTeamsSinkConfigWrapper,
     MsTeamsSinkParams,
 )
 from ..core.sinks.robusta.robusta_sink_params import (
     RobustaSinkConfigWrapper,
     RobustaSinkParams,
 )
 from ..core.sinks.slack.slack_sink_params import SlackSinkConfigWrapper, SlackSinkParams
 from robusta._version import __version__
 from .integrations_cmd import app as integrations_commands, get_slack_key
+from .auth import app as auth_commands
 from .slack_verification import verify_slack_channel
+from .slack_feedback_message import SlackFeedbackMessagesSender, SlackFeedbackConfig
 from .playbooks_cmd import app as playbooks_commands
 from .utils import log_title, replace_in_file, namespace_to_kubectl
 
 FORWARDER_CONFIG_FOR_SMALL_CLUSTERS = "64Mi"
 RUNNER_CONFIG_FOR_SMALL_CLUSTERS = "512Mi"
 GRAFANA_RENDERER_CONFIG_FOR_SMALL_CLUSTERS = "64Mi"
 
 app = typer.Typer()
 app.add_typer(playbooks_commands, name="playbooks", help="Playbooks commands menu")
 app.add_typer(
     integrations_commands, name="integrations", help="Integrations commands menu"
 )
+app.add_typer(
+    auth_commands, name="auth", help="Authentication commands menu"
+)
 
 
 def get_runner_url(runner_version=None):
     if runner_version is None:
         runner_version = __version__
     return f"https://gist.githubusercontent.com/robusta-lab/6b809d508dfc3d8d92afc92c7bbbe88e/raw/robusta-{runner_version}.yaml"
 
@@ -59,29 +66,30 @@
     __root__: Dict[str, Dict[str, Dict[str, str]]]
 
     @classmethod
     def gen_config(cls, memory_size: str) -> Dict:
         return {"resources": {"requests": {"memory": memory_size}}}
 
 
-class HelmValues(BaseModel):
+class HelmValues(BaseModel, extra=Extra.allow):
     globalConfig: GlobalConfig
     sinksConfig: List[
         Union[
             SlackSinkConfigWrapper, RobustaSinkConfigWrapper, MsTeamsSinkConfigWrapper
         ]
     ]
     clusterName: str
     enablePrometheusStack: bool = False
     disableCloudRouting: bool = False
     enablePlatformPlaybooks: bool = False
     playbooksPersistentVolumeSize: str = None
     kubewatch: Dict = None
     grafanaRenderer: Dict = None
     runner: Dict = None
+    rsa: RSAKeyPair = None
 
     def set_pod_configs_for_small_clusters(self):
         self.kubewatch = PodConfigs.gen_config(FORWARDER_CONFIG_FOR_SMALL_CLUSTERS)
         self.runner = PodConfigs.gen_config(RUNNER_CONFIG_FOR_SMALL_CLUSTERS)
         self.grafanaRenderer = PodConfigs.gen_config(
             GRAFANA_RENDERER_CONFIG_FOR_SMALL_CLUSTERS
         )
@@ -110,14 +118,27 @@
             prompt_suffix="#",
         )
         .strip()
         .strip("#")
     )
 
 
+def write_values_file(output_path: str, values: HelmValues):
+    with open(output_path, "w") as output_file:
+        yaml.safe_dump(values.dict(exclude_defaults=True), output_file, sort_keys=False)
+        typer.secho(
+            f"Saved configuration to {output_path}",
+            fg="green",
+        )
+        typer.secho(
+            f"Save this file for future use. It contains your account credentials",
+            fg="red",
+        )
+
+
 @app.command()
 def gen_config(
     cluster_name: str = typer.Option(
         None,
         help="Cluster Name",
     ),
     is_small_cluster: bool = typer.Option(None),
@@ -167,14 +188,15 @@
         default=True,
     ):
         slack_api_key, slack_workspace = get_slack_key()
 
     if slack_api_key and not slack_channel:
         slack_channel = get_slack_channel()
 
+    slack_integration_configured = False
     if slack_api_key and slack_channel:
         while not verify_slack_channel(
             slack_api_key, cluster_name, slack_channel, slack_workspace, debug
         ):
             slack_channel = get_slack_channel()
 
         sinks_config.append(
@@ -183,14 +205,16 @@
                     name="main_slack_sink",
                     api_key=slack_api_key,
                     slack_channel=slack_channel,
                 )
             )
         )
 
+        slack_integration_configured = True
+
     if msteams_webhook is None and typer.confirm(
         "Do you want to configure MsTeams integration ?",
         default=False,
     ):
         msteams_webhook = typer.prompt(
             "Please insert your MsTeams webhook url",
             default=None,
@@ -271,14 +295,27 @@
                     name="robusta_ui_sink", token=robusta_api_key
                 )
             )
         )
         enable_platform_playbooks = True
         require_eula_approval = True
 
+    slack_feedback_heads_up_message: Optional[str] = None
+    if slack_integration_configured:
+        try:
+            slack_feedback_heads_up_message = SlackFeedbackMessagesSender(
+                slack_api_key,
+                slack_channel,
+                account_id,
+                debug
+            ).schedule_feedback_messages()
+        except Exception as e:
+            if debug:
+                typer.secho(traceback.format_exc())
+
     if enable_prometheus_stack is None:
         enable_prometheus_stack = typer.confirm(
             "If you haven't installed Prometheus yet, Robusta can install a pre-configured Prometheus. Would you like to do so?"
         )
 
     if disable_cloud_routing is None:
         disable_cloud_routing = not typer.confirm(
@@ -307,14 +344,15 @@
     values = HelmValues(
         clusterName=cluster_name,
         globalConfig=GlobalConfig(signing_key=signing_key, account_id=account_id),
         sinksConfig=sinks_config,
         enablePrometheusStack=enable_prometheus_stack,
         disableCloudRouting=disable_cloud_routing,
         enablePlatformPlaybooks=enable_platform_playbooks,
+        rsa=gen_rsa_pair()
     )
 
     if is_small_cluster:
         values.set_pod_configs_for_small_clusters()
         values.playbooksPersistentVolumeSize = "128Mi"
 
     if backend_profile.custom_profile:
@@ -332,31 +370,57 @@
             {"name": "ROBUSTA_UI_DOMAIN", "value": backend_profile.robusta_ui_domain},
             {
                 "name": "ROBUSTA_TELEMETRY_ENDPOINT",
                 "value": backend_profile.robusta_telemetry_endpoint
             }
         ]
 
-    with open(output_path, "w") as output_file:
-        yaml.safe_dump(values.dict(exclude_defaults=True), output_file, sort_keys=False)
-        typer.secho(
-            f"Saved configuration to {output_path}",
-            fg="green",
-        )
-        typer.secho(
-            f"Save this file for future use. It contains your account credentials",
-            fg="red",
-        )
+    write_values_file(output_path, values)
 
     if robusta_api_key:
         typer.secho(
             f"Finish the Helm install and then login to Robusta UI at {backend_profile.robusta_ui_domain}\n",
             fg="green",
         )
 
+    if slack_feedback_heads_up_message:
+        typer.secho(slack_feedback_heads_up_message)
+
+
+@app.command()
+def update_config(
+    existing_values: str = typer.Option(
+        ...,
+        help="Existing values.yaml file name. You can run `helm get values` to get it from the cluster.",
+    ),
+):
+    """
+        Update an existing values.yaml file.
+        Add RSA key-pair if it doesn't exist
+        Add a signing key if it doesn't exist, or replace with a valid one if the key has an invalid format
+    """
+    with open(existing_values, "r") as existing_values_file:
+        values: HelmValues = HelmValues(**yaml.safe_load(existing_values_file))
+        if not values.rsa:
+            typer.secho("Generating RSA key-pair", fg="green")
+            values.rsa = gen_rsa_pair()
+
+        if not values.globalConfig.signing_key:
+            typer.secho("Generating signing key", fg="green")
+            values.globalConfig.signing_key = str(uuid.uuid4())
+
+        try:
+            uuid.UUID(values.globalConfig.signing_key)
+        except:
+            typer.secho("Invalid signing key. Generating a new one", fg="green")
+            values.globalConfig.signing_key = str(uuid.uuid4())
+
+        write_values_file("updated_values.yaml", values)
+        typer.secho("Run `helm upgrade robusta -f ./updated_values.yaml`", fg="green")
+
 
 @app.command()
 def playground():
     """Open a python playground - useful when writing playbooks"""
     typer.echo(
         "this command is temporarily disabled due to recent changes to python:3.8-slim"
     )
```

### Comparing `robusta-cli-0.9.7/src/robusta/cli/playbooks_cmd.py` & `robusta-cli-0.9.9/src/robusta/cli/playbooks_cmd.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/cli/slack_verification.py` & `robusta-cli-0.9.9/src/robusta/cli/slack_verification.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     slack_api_key: str,
     cluster_name: str,
     channel_name: str,
     workspace: str,
     debug: bool,
 ) -> bool:
     try:
-        output_welcome_message_blocks = gen_robusta_test_welcome_message(cluster_name)
+        output_welcome_message_blocks = __gen_robusta_test_welcome_message(cluster_name)
         slack_client = WebClient(token=slack_api_key)
         slack_client.chat_postMessage(
             channel=channel_name,
             text="Welcome to Robusta",
             blocks=output_welcome_message_blocks,
             display_as_bot=True,
             unfurl_links=True,
@@ -49,15 +49,15 @@
     typer.secho(
         f"There was an unknown exception setting up Slack, please contact Robusta support.",
         fg=typer.colors.RED,
     )
     return False
 
 
-def gen_robusta_test_welcome_message(cluster_name: str):
+def __gen_robusta_test_welcome_message(cluster_name: str):
     return [
         {
             "type": "header",
             "text": {
                 "type": "plain_text",
                 "text": SLACK_WELCOME_MESSAGE_TITLE,
                 "emoji": True,
```

### Comparing `robusta-cli-0.9.7/src/robusta/cli/utils.py` & `robusta-cli-0.9.9/src/robusta/cli/utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/discovery/top_service_resolver.py` & `robusta-cli-0.9.9/src/robusta/core/discovery/top_service_resolver.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/model/base_params.py` & `robusta-cli-0.9.9/src/robusta/core/model/base_params.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/model/env_vars.py` & `robusta-cli-0.9.9/src/robusta/core/model/env_vars.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,8 +54,11 @@
 TEAMS_IMAGE_WIDTH = os.environ.get("TEAMS_IMAGE_WIDTH", "700px")
 
 ROBUSTA_UI_DOMAIN = os.environ.get("ROBUSTA_UI_DOMAIN", "https://platform.robusta.dev")
 
 ROBUSTA_TELEMETRY_ENDPOINT = os.environ.get("ROBUSTA_TELEMETRY_ENDPOINT", "https://api.robusta.dev/telemetry")
 ENABLE_TELEMETRY = os.environ.get("ENABLE_TELEMETRY", "true").lower() == "true"
 SEND_ADDITIONAL_TELEMETRY = os.environ.get("SEND_ADDITIONAL_TELEMETRY", "false").lower() == "true"
-TELEMETRY_PERIODIC_SEC = int(os.environ.get("TELEMETRY_PERIODIC_SEC", 60 * 60 * 24)) # 24H
+TELEMETRY_PERIODIC_SEC = int(os.environ.get("TELEMETRY_PERIODIC_SEC", 60 * 60 * 24)) # 24H
+
+SLACK_TABLE_COLUMNS_LIMIT = int(os.environ.get("SLACK_TABLE_COLUMNS_LIMIT", 4))
+RSA_KEYS_PATH = os.environ.get("RSA_KEYS_PATH", "/etc/robusta/auth")
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/model/events.py` & `robusta-cli-0.9.9/src/robusta/core/model/events.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,19 @@
     SCHEDULED_TRIGGER = 4
 
 
 class ExecutionEventBaseParams(BaseModel):
     named_sinks: Optional[List[str]] = None
 
 
+class ExecutionContext(BaseModel):
+    account_id: str
+    cluster_name: str
+
+
 # Right now:
 # 1. this is a dataclass but we need to make all fields optional in subclasses because of https://stackoverflow.com/questions/51575931/
 # 2. this can't be a pydantic BaseModel because of various pydantic bugs (see https://github.com/samuelcolvin/pydantic/pull/2557)
 # once the pydantic PR that addresses those issues is merged, this should be a pydantic class
 # (note that we need to integrate with dataclasses because of hikaru)
 @dataclass
 class ExecutionBaseEvent:
@@ -37,14 +42,21 @@
     # Target sinks for this execution event. Each playbook may have a different list of target sinks.
     named_sinks: Optional[List[str]] = None
     response: Dict[
         str, Any
     ] = None  # Response returned to caller. For admission or manual triggers for example
     stop_processing: bool = False
     _scheduler: Optional[PlaybooksScheduler] = None
+    _context: Optional[ExecutionContext] = None
+
+    def set_context(self, context: ExecutionContext):
+        self._context = context
+
+    def get_context(self) -> ExecutionContext:
+        return self._context
 
     def set_scheduler(self, scheduler: PlaybooksScheduler):
         self._scheduler = scheduler
 
     def get_scheduler(self) -> PlaybooksScheduler:
         return self._scheduler
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/model/runner_config.py` & `robusta-cli-0.9.9/src/robusta/core/model/runner_config.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/model/services.py` & `robusta-cli-0.9.9/src/robusta/core/model/services.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/persistency/in_memory.py` & `robusta-cli-0.9.9/src/robusta/core/persistency/in_memory.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/persistency/scheduled_jobs_states_dal.py` & `robusta-cli-0.9.9/src/robusta/core/persistency/scheduled_jobs_states_dal.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/actions_registry.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/actions_registry.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/base_trigger.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/base_trigger.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/common.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/common.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/generation.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/generation.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/internal/discovery_events.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/internal/discovery_events.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/playbook_utils.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/playbook_utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/playbooks_event_handler.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,24 +16,28 @@
         pass
 
     @abstractmethod
     def run_actions(
         self,
         execution_event: ExecutionBaseEvent,
         actions: List[PlaybookAction],
+        sync_response: bool = False,
+        no_sinks: bool = False,
     ) -> Optional[Dict[str, Any]]:
         """Run list of actions using the provided execution event"""
         pass
 
     @abstractmethod
     def run_external_action(
         self,
         action_name: str,
         action_params: Optional[dict],
         sinks: Optional[List[str]],
+        sync_response: bool = False,
+        no_sinks: bool = False
     ) -> Optional[Dict[str, Any]]:
         """Execute an external action"""
         pass
 
     @abstractmethod
     def get_global_config(
         self,
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/playbooks_event_handler_impl.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/playbooks_event_handler_impl.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import traceback
 from collections import defaultdict
 from typing import Any, Dict, Optional, List
 
 from .base_trigger import TriggerEvent, BaseTrigger
 from .playbook_utils import merge_global_params
 from .playbooks_event_handler import PlaybooksEventHandler
-from ..model.events import ExecutionBaseEvent
+from ..model.events import ExecutionBaseEvent, ExecutionContext
 from ..reporting import MarkdownBlock
 from ..reporting.base import Finding
+from ..reporting.consts import SYNC_RESPONSE_SINK
+from ..sinks.robusta.dal.model_conversion import ModelConversion
 from ...model.playbook_action import PlaybookAction
 from ...model.config import Registry
 from .trigger import Trigger
 from ...runner.telemetry import Telemetry
 
 
 class PlaybooksEventHandlerImpl(PlaybooksEventHandler):
@@ -59,47 +61,87 @@
 
         return execution_response
 
     def run_actions(
         self,
         execution_event: ExecutionBaseEvent,
         actions: List[PlaybookAction],
+        sync_response: bool = False,
+        no_sinks: bool = False,
     ) -> Optional[Dict[str, Any]]:
-        if execution_event.named_sinks is None:
+        if not no_sinks and execution_event.named_sinks is None:  # take the default sinks only if sinks not excluded
             execution_event.named_sinks = (
                 self.registry.get_playbooks().get_default_sinks()
             )
 
+        if sync_response:  # if we need to return sync response, we'll collect the findings under this sink name
+            if execution_event.named_sinks:
+                execution_event.named_sinks.append(SYNC_RESPONSE_SINK)
+            else:
+                execution_event.named_sinks = [SYNC_RESPONSE_SINK]
+
         execution_response = self.__run_playbook_actions(
             execution_event,
             actions,
         )
         self.__handle_findings(execution_event)
 
+        if sync_response:  # add the findings to the response
+            execution_response["findings"] = [
+                self.__to_finding_json(finding)
+                for finding in execution_event.sink_findings[SYNC_RESPONSE_SINK]
+            ]
+
         return execution_response
 
+    def __to_finding_json(self, finding: Finding) -> Dict:
+        account_id = self.registry.get_global_config().get("account_id", "")
+        cluster_id = self.registry.get_global_config().get("cluster_name", "")
+        signing_key = self.registry.get_global_config().get("signing_key", "")
+
+        finding_json = ModelConversion.to_finding_json(account_id, cluster_id, finding)
+
+        finding_json["evidence"] = [
+            ModelConversion.to_evidence_json(
+                account_id,
+                cluster_id,
+                SYNC_RESPONSE_SINK,
+                signing_key,
+                finding.id,
+                enrichment
+            )
+            for enrichment in finding.enrichments
+        ]
+        return finding_json
+
     def __prepare_execution_event(self, execution_event: ExecutionBaseEvent):
         execution_event.set_scheduler(self.registry.get_scheduler())
+        execution_event.set_context(ExecutionContext(
+            account_id=self.registry.get_global_config().get("account_id", ""),
+            cluster_name=self.registry.get_global_config().get("cluster_name", "")
+        ))
 
     def run_external_action(
         self,
         action_name: str,
         action_params: Optional[dict],
         sinks: Optional[List[str]],
+        sync_response: bool = False,
+        no_sinks: bool = False,
     ) -> Optional[Dict[str, Any]]:
         action_def = self.registry.get_actions().get_action(action_name)
         if not action_def:
             return self.__error_resp(f"External action not found {action_name}")
 
         if not action_def.from_params_func:
             return self.__error_resp(
                 f"Action {action_name} cannot run using external event"
             )
 
-        if sinks:
+        if not no_sinks and sinks:
             if action_params:
                 action_params["named_sinks"] = sinks
             else:
                 action_params = {"named_sinks": sinks}
         try:
             instantiation_params = action_def.from_params_parameter_class(
                 **action_params
@@ -117,15 +159,15 @@
                 f"Failed to create execution event for "
                 f"{action_name} {action_params}"
             )
 
         playbook_action = PlaybookAction(
             action_name=action_name, action_params=action_params
         )
-        return self.run_actions(execution_event, [playbook_action])
+        return self.run_actions(execution_event, [playbook_action], sync_response, no_sinks)
 
     @classmethod
     def __error_resp(cls, msg: str) -> dict:
         logging.error(msg)
         return {"success": False, "msg": msg}
 
     def __run_playbook_actions(
@@ -202,14 +244,17 @@
                 return trigger.get()
         return None
 
     def __handle_findings(self, execution_event: ExecutionBaseEvent):
         sinks_info = self.registry.get_telemetry().sinks_info
 
         for sink_name in execution_event.named_sinks:
+            if SYNC_RESPONSE_SINK == sink_name:
+                continue  # not a real sink, just container for findings that needs to be returned synchronously
+
             for finding in execution_event.sink_findings[sink_name]:
                 try:
                     sink = self.registry.get_sinks().sinks.get(sink_name)
                     if not sink:
                         logging.error(
                             f"sink {sink_name} not found. Skipping event finding {finding}"
                         )
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/prometheus_enrichment_utils.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/prometheus_enrichment_utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/playbooks/trigger.py` & `robusta-cli-0.9.9/src/robusta/core/playbooks/trigger.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/base.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/base.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/blocks.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/blocks.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,16 @@
         """
         super().__init__(json_str=json_str)
 
 
 class TableBlock(BaseBlock):
     """
     Table display of a list of lists.
+
+    Note: Wider tables appears as a file attachment on Slack, because they aren't rendered properly inline
     """
 
     rows: List[List]
     headers: Sequence[str] = ()
     column_renderers: Dict = {}
     table_name: str = ""
 
@@ -198,52 +200,52 @@
         """
         :param rows: a list of rows. each row is a list of columns
         :param headers: names of each column
         """
         super().__init__(rows=rows, headers=headers, column_renderers=column_renderers, table_name=table_name)
 
     @classmethod
-    def __calc_max_width(cls, headers, rendered_rows) -> List[int]:
+    def __calc_max_width(cls, headers, rendered_rows, table_max_width: int) -> List[int]:
         # We need to make sure the total table width, doesn't exceed the max width,
         # otherwise, the table is printed corrupted
         columns_max_widths = [len(header) for header in headers]
         for row in rendered_rows:
             for idx, val in enumerate(row):
                 columns_max_widths[idx] = max(len(str(val)), columns_max_widths[idx])
 
         if (
-            sum(columns_max_widths) > PRINTED_TABLE_MAX_WIDTH
+            sum(columns_max_widths) > table_max_width
         ):  # We want to limit the widest column
             largest_width = max(columns_max_widths)
             widest_column_idx = columns_max_widths.index(largest_width)
-            diff = sum(columns_max_widths) - PRINTED_TABLE_MAX_WIDTH
+            diff = sum(columns_max_widths) - table_max_width
             columns_max_widths[widest_column_idx] = largest_width - diff
             if (
                 columns_max_widths[widest_column_idx] < 0
             ):  # in case the diff is bigger than the largest column
                 # just divide equally
                 columns_max_widths = [
-                    int(PRINTED_TABLE_MAX_WIDTH / len(columns_max_widths))
+                    int(table_max_width / len(columns_max_widths))
                     for i in range(0, len(columns_max_widths))
                 ]
 
         return columns_max_widths
 
     @classmethod
     def __to_strings_rows(cls, rows):
         # This is just to assert all row column values are strings. Tabulate might fail on other types
         return [list(map(lambda column_value: str(column_value), row)) for row in rows]
 
     def to_markdown(self) -> MarkdownBlock:
         table_header = f"{self.table_name}\n" if self.table_name else ""
         return MarkdownBlock(f"{table_header}```\n{self.to_table_string()}\n```")
 
-    def to_table_string(self) -> str:
+    def to_table_string(self, table_max_width: int = PRINTED_TABLE_MAX_WIDTH) -> str:
         rendered_rows = self.__to_strings_rows(self.render_rows())
-        col_max_width = self.__calc_max_width(self.headers, rendered_rows)
+        col_max_width = self.__calc_max_width(self.headers, rendered_rows, table_max_width)
         return tabulate(
             rendered_rows,
             headers=self.headers,
             tablefmt="presto",
             maxcolwidths=col_max_width,
         )
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/callbacks.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/callbacks.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/consts.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/consts.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,10 @@
 from enum import Enum
 
-# sink types
-# TODO: can we remove?
-class SinkType(Enum):
-    ROBUSTA = "robusta"
-    SLACK = "slack"
-    MSTEAMS = "msteams"
-    KAFKA = "kafka"
-    DATADOG = "datadog"
+SYNC_RESPONSE_SINK = "robusta-synchronized-response-sink"
 
 
 class FindingType(Enum):
     ISSUE = "issue"
     CONF_CHANGE = "configuration_change"
     HEALTH_CHECK = "health_check"
     REPORT = "report"
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/finding_subjects.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/finding_subjects.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/reporting/utils.py` & `robusta-cli-0.9.9/src/robusta/core/reporting/utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/schedule/model.py` & `robusta-cli-0.9.9/src/robusta/core/schedule/model.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/schedule/scheduler.py` & `robusta-cli-0.9.9/src/robusta/core/schedule/scheduler.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/datadog/datadog_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/datadog/datadog_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/kafka/kafka_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/kafka/kafka_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/msteams/msteams_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/msteams/msteams_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/opsgenie/opsgenie_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/opsgenie/opsgenie_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/robusta/dal/supabase_dal.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/robusta/dal/supabase_dal.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,21 @@
-import base64
 import json
 import logging
 import threading
 import time
 import traceback
-import uuid
 from typing import List, Dict, Any
 from supabase_py.lib.auth_client import SupabaseAuthClient
 
-from ...transformer import Transformer
+from .model_conversion import ModelConversion
 from ....model.cluster_status import ClusterStatus
 from ....model.nodes import NodeInfo
 from ....model.services import ServiceInfo
-from ....reporting.blocks import (
-    MarkdownBlock,
-    KubernetesDiffBlock,
-    DividerBlock,
-    FileBlock,
-    HeaderBlock,
-    CallbackBlock,
-    ListBlock,
-    TableBlock,
-)
-from ....reporting.base import (
-    Finding,
-    Enrichment,
-)
+from ....reporting.base import Finding
 from ....model.env_vars import SUPABASE_LOGIN_RATE_LIMIT_SEC
-from ....reporting.callbacks import ExternalActionRequestBuilder
 from supabase_py import Client
 
 SERVICES_TABLE = "Services"
 NODES_TABLE = "Nodes"
 EVIDENCE_TABLE = "Evidence"
 ISSUES_TABLE = "Issues"
 CLUSTERS_STATUS_TABLE = "ClustersStatus"
@@ -102,140 +86,36 @@
         self.email = email
         self.password = password
         self.sign_in_time = 0
         self.sign_in()
         self.sink_name = sink_name
         self.signing_key = signing_key
 
-    def to_issue(self, finding: Finding):
-        issue_obj = {
-            "id": str(finding.id),
-            "title": finding.title,
-            "description": finding.description,
-            "source": finding.source.value,
-            "aggregation_key": finding.aggregation_key,
-            "failure": finding.failure,
-            "finding_type": finding.finding_type.value,
-            "category": finding.category,
-            "priority": finding.severity.name,
-            "subject_type": finding.subject.subject_type.value,
-            "subject_name": finding.subject.name,
-            "subject_namespace": finding.subject.namespace,
-            "subject_node": finding.subject.node,
-            "service_key": finding.service_key,
-            "cluster": self.cluster,
-            "account_id": self.account_id,
-        }
-
-        if finding.creation_date:
-            issue_obj["creation_date"] = finding.creation_date
-
-        return issue_obj
-
-    def to_evidence(self, finding_id: uuid, enrichment: Enrichment) -> Dict[Any, Any]:
-        structured_data = []
-        for block in enrichment.blocks:
-            if isinstance(block, MarkdownBlock):
-                if not block.text:
-                    continue
-                structured_data.append(
-                    {
-                        "type": "markdown",
-                        "data": Transformer.to_github_markdown(block.text),
-                    }
-                )
-            elif isinstance(block, DividerBlock):
-                structured_data.append({"type": "divider"})
-            elif isinstance(block, FileBlock):
-                last_dot_idx = block.filename.rindex(".")
-                structured_data.append(
-                    {
-                        "type": block.filename[last_dot_idx + 1 :],
-                        "data": str(base64.b64encode(block.contents)),
-                    }
-                )
-            elif isinstance(block, HeaderBlock):
-                structured_data.append({"type": "header", "data": block.text})
-            elif isinstance(block, ListBlock):
-                structured_data.append({"type": "list", "data": block.items})
-            elif isinstance(block, TableBlock):
-                if block.table_name:
-                    structured_data.append({
-                            "type": "markdown",
-                            "data": Transformer.to_github_markdown(block.table_name),
-                    })
-                structured_data.append(
-                    {
-                        "type": "table",
-                        "data": {
-                            "headers": block.headers,
-                            "rows": [row for row in block.rows],
-                            "column_renderers": block.column_renderers,
-                        },
-                    }
-                )
-            elif isinstance(block, KubernetesDiffBlock):
-                structured_data.append(
-                    {
-                        "type": "diff",
-                        "data": {
-                            "old": block.old,
-                            "new": block.new,
-                            "resource_name": block.resource_name,
-                            "num_additions": block.num_additions,
-                            "num_deletions": block.num_deletions,
-                            "num_modifications": block.num_modifications,
-                            "updated_paths": [d.formatted_path for d in block.diffs],
-                        },
-                    }
-                )
-            elif isinstance(block, CallbackBlock):
-                callbacks = []
-                for (text, callback) in block.choices.items():
-                    callbacks.append(
-                        {
-                            "text": text,
-                            "callback": ExternalActionRequestBuilder.create_for_func(
-                                callback,
-                                self.sink_name,
-                                text,
-                                self.account_id,
-                                self.cluster,
-                                self.signing_key,
-                            ).json(),
-                        }
-                    )
-
-                structured_data.append({"type": "callbacks", "data": callbacks})
-            else:
-                logging.error(
-                    f"cannot convert block of type {type(block)} to robusta platform format block: {block}"
-                )
-                continue  # no reason to crash the entire report
-
-        return {
-            "issue_id": str(finding_id),
-            "file_type": "structured_data",
-            "data": json.dumps(structured_data),
-            "account_id": self.account_id,
-        }
-
     def persist_finding(self, finding: Finding):
         for enrichment in finding.enrichments:
             res = (
                 self.client.table(EVIDENCE_TABLE)
-                .insert(self.to_evidence(finding.id, enrichment))
+                .insert(ModelConversion.to_evidence_json(
+                    account_id=self.account_id,
+                    cluster_id=self.cluster,
+                    sink_name=self.sink_name,
+                    signing_key=self.signing_key,
+                    finding_id=finding.id,
+                    enrichment=enrichment
+                ))
                 .execute()
             )
             if res.get("status_code") != 201:
                 logging.error(
                     f"Failed to persist finding {finding.id} enrichment {enrichment} error: {res.get('data')}"
                 )
 
-        res = self.client.table(ISSUES_TABLE).insert(self.to_issue(finding)).execute()
+        res = self.client.table(ISSUES_TABLE).insert(
+            ModelConversion.to_finding_json(self.account_id, self.cluster, finding)
+        ).execute()
         if res.get("status_code") != 201:
             logging.error(
                 f"Failed to persist finding {finding.id} error: {res.get('data')}"
             )
             self.handle_supabase_error()
 
     def to_service(self, service: ServiceInfo) -> Dict[Any, Any]:
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/robusta/robusta_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/robusta/robusta_sink.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     Pod,
 )
 from typing import List, Dict
 
 from robusta.runner.web_api import WebApi
 from .robusta_sink_params import RobustaSinkConfigWrapper, RobustaToken
 from ...model.env_vars import DISCOVERY_PERIOD_SEC, PERIODIC_LONG_SEC
-from ...model.nodes import NodeInfo, PodRequests
+from ...model.nodes import NodeInfo
+from ...model.pods import PodResources, pod_requests
 from ...model.services import ServiceInfo
 from ...reporting.base import Finding
 from .dal.supabase_dal import SupabaseDal
 from ..sink_base import SinkBase
 from ...discovery.top_service_resolver import TopServiceResolver
 from ...model.cluster_status import ClusterStatus
 
@@ -187,15 +188,15 @@
         node_info["labels"] = node.metadata.labels
         node_info["annotations"] = node.metadata.annotations
         node_info["addresses"] = [addr.address for addr in node.status.addresses]
         return node_info
 
     @classmethod
     def __from_api_server_node(
-        cls, api_server_node: Node, pod_requests: List[PodRequests]
+        cls, api_server_node: Node, pod_requests_list: List[PodResources]
     ) -> NodeInfo:
         addresses = api_server_node.status.addresses
         external_addresses = [
             address for address in addresses if "externalip" in address.type.lower()
         ]
         external_ip = ",".join([addr.address for addr in external_addresses])
         internal_addresses = [
@@ -211,35 +212,35 @@
             node_creation_time=api_server_node.metadata.creationTimestamp,
             internal_ip=internal_ip,
             external_ip=external_ip,
             taints=taints,
             conditions=cls.__to_active_conditions_str(
                 api_server_node.status.conditions
             ),
-            memory_capacity=PodRequests.parse_mem(
+            memory_capacity=PodResources.parse_mem(
                 api_server_node.status.capacity.get("memory", "0Mi")
             ),
-            memory_allocatable=PodRequests.parse_mem(
+            memory_allocatable=PodResources.parse_mem(
                 api_server_node.status.allocatable.get("memory", "0Mi")
             ),
-            memory_allocated=sum([req.memory for req in pod_requests]),
-            cpu_capacity=PodRequests.parse_cpu(
+            memory_allocated=sum([req.memory for req in pod_requests_list]),
+            cpu_capacity=PodResources.parse_cpu(
                 api_server_node.status.capacity.get("cpu", "0")
             ),
-            cpu_allocatable=PodRequests.parse_cpu(
+            cpu_allocatable=PodResources.parse_cpu(
                 api_server_node.status.allocatable.get("cpu", "0")
             ),
-            cpu_allocated=round(sum([req.cpu for req in pod_requests]), 3),
-            pods_count=len(pod_requests),
-            pods=",".join([pod_req.pod_name for pod_req in pod_requests]),
+            cpu_allocated=round(sum([req.cpu for req in pod_requests_list]), 3),
+            pods_count=len(pod_requests_list),
+            pods=",".join([pod_req.pod_name for pod_req in pod_requests_list]),
             node_info=cls.__to_node_info(api_server_node),
         )
 
     def __publish_new_nodes(
-        self, current_nodes: NodeList, node_requests: Dict[str, List[PodRequests]]
+        self, current_nodes: NodeList, node_requests: Dict[str, List[PodResources]]
     ):
         # convert to map
         curr_nodes = {}
         for node in current_nodes.items:
             curr_nodes[node.metadata.name] = node
 
         # handle deleted nodes
@@ -268,37 +269,16 @@
             node_requests = defaultdict(list)
             for status in ["Running", "Unknown", "Pending"]:
                 pods: PodList = Pod.listPodForAllNamespaces(
                     field_selector=f"status.phase={status}"
                 ).obj
                 for pod in pods.items:
                     if pod.spec.nodeName:
-                        pod_cpu_req: float = 0.0
-                        pod_mem_req: int = 0
-                        for container in pod.spec.containers:
-                            try:
-                                requests = container.object_at_path(
-                                    ["resources", "requests"]
-                                )
-                                pod_cpu_req += PodRequests.parse_cpu(
-                                    requests.get("cpu", 0.0)
-                                )
-                                pod_mem_req += PodRequests.parse_mem(
-                                    requests.get("memory", "0Mi")
-                                )
-                            except Exception:
-                                pass  # no requests on container, object_at_path throws error
-
-                        node_requests[pod.spec.nodeName].append(
-                            PodRequests(
-                                pod_name=pod.metadata.name,
-                                cpu=pod_cpu_req,
-                                memory=pod_mem_req,
-                            )
-                        )
+                        node_requests[pod.spec.nodeName].append(pod_requests(pod))
+
             self.__publish_new_nodes(current_nodes, node_requests)
         except Exception as e:
             logging.error(
                 f"Failed to run periodic nodes discovery for {self.sink_name}",
                 exc_info=True,
             )
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/sink_base.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/sink_base.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/sink_factory.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/sink_factory.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/slack/slack_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/slack/slack_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/telegram/telegram_client.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_client.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/telegram/telegram_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/telegram/telegram_sink.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,16 +39,17 @@
             for enrichment in finding.enrichments:
                 file_blocks = [block for block in enrichment.blocks if isinstance(block, FileBlock)]
                 for block in file_blocks:
                     self.client.send_file(file_name=block.filename, contents=block.contents)
                 table_blocks = [block for block in enrichment.blocks if isinstance(block, TableBlock)]
                 for block in table_blocks:
                     table_text = tabulate(block.render_rows(), headers=block.headers, tablefmt="presto")
+                    table_name = block.table_name if block.table_name else "table"
                     self.client.send_file(
-                        file_name=f"{block.table_name}.txt",
+                        file_name=f"{table_name}.txt",
                         contents=table_text.encode("utf-8")
                     )
 
     def __get_message_text(self, finding: Finding, platform_enabled: bool):
         message_content = self.__build_telegram_title(finding.title, finding.severity)
 
         if platform_enabled:
```

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/transformer.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/transformer.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/sinks/webhook/webhook_sink.py` & `robusta-cli-0.9.9/src/robusta/core/sinks/webhook/webhook_sink.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/triggers/custom_triggers.py` & `robusta-cli-0.9.9/src/robusta/core/triggers/custom_triggers.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/core/triggers/error_event_trigger.py` & `robusta-cli-0.9.9/src/robusta/core/triggers/error_event_trigger.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/argocd/argocd_client.py` & `robusta-cli-0.9.9/src/robusta/integrations/argocd/argocd_client.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/git/git_repo.py` & `robusta-cli-0.9.9/src/robusta/integrations/git/git_repo.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/grafana.py` & `robusta-cli-0.9.9/src/robusta/integrations/grafana.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/api_client_utils.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/api_client_utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/events.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/events.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/triggers.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/triggers.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v1/models.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v1/models.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta1/models.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta1/models.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/autogenerated/v2beta2/models.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/autogenerated/v2beta2/models.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/base_event.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_event.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/base_triggers.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/base_triggers.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/custom_models.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/custom_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,32 @@
     cmdline: List[str]
 
 
 class ProcessList(BaseModel):
     processes: List[Process]
 
 
+def _get_match_expression_filter(expression: LabelSelectorRequirement) -> str:
+    if expression.operator.lower() == "exists":
+        return expression.key
+    elif expression.operator.lower() == "doesnotexist":
+        return f"!{expression.key}"
+
+    values = ",".join(expression.values)
+    return f"{expression.key} {expression.operator} ({values})"
+
+
+def build_selector_query(selector: LabelSelector) -> str:
+    label_filters = [f"{label[0]}={label[1]}" for label in selector.matchLabels.items()]
+    label_filters.extend([
+        _get_match_expression_filter(expression) for expression in selector.matchExpressions
+    ])
+    return ",".join(label_filters)
+
+
 def get_images(containers: List[Container]) -> Dict[str, str]:
     """
     Takes a list of containers and returns a dict mapping image name to image tag.
     """
     name_to_version = {}
     for container in containers:
         if ":" in container.image:
```

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/process_utils.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/process_utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/kubernetes/templates.py` & `robusta-cli-0.9.9/src/robusta/integrations/kubernetes/templates.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files_image.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_image.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_adaptive_card_files_text.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_adaptive_card_files_text.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_action.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_action.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_card.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_card.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_column.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_column.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_container.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_container.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_images.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_images.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_table.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_table.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_elements/msteams_text_block.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_elements/msteams_text_block.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_mark_down_fix_url.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_mark_down_fix_url.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/msteams_msg.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/msteams_msg.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/msteams/sender.py` & `robusta-cli-0.9.9/src/robusta/integrations/msteams/sender.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/prometheus/models.py` & `robusta-cli-0.9.9/src/robusta/integrations/prometheus/models.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/prometheus/trigger.py` & `robusta-cli-0.9.9/src/robusta/integrations/prometheus/trigger.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/prometheus/utils.py` & `robusta-cli-0.9.9/src/robusta/integrations/prometheus/utils.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/resource_analysis/memory_analyzer.py` & `robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/memory_analyzer.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/resource_analysis/node_cpu_analyzer.py` & `robusta-cli-0.9.9/src/robusta/integrations/resource_analysis/node_cpu_analyzer.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/scheduled/playbook_scheduler.py` & `robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/scheduled/playbook_scheduler_manager_impl.py` & `robusta-cli-0.9.9/src/robusta/integrations/scheduled/playbook_scheduler_manager_impl.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/scheduled/trigger.py` & `robusta-cli-0.9.9/src/robusta/integrations/scheduled/trigger.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/integrations/slack/sender.py` & `robusta-cli-0.9.9/src/robusta/integrations/slack/sender.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import logging
 import tempfile
 from slack_sdk import WebClient
 from slack_sdk.errors import SlackApiError
 
+from ...core.model.env_vars import SLACK_TABLE_COLUMNS_LIMIT
 from ...core.model.events import *
 from ...core.reporting.blocks import *
 from ...core.reporting.base import *
 from ...core.reporting.utils import add_pngs_for_all_svgs
 from ...core.reporting.callbacks import ExternalActionRequestBuilder
 from ...core.reporting.consts import SlackAnnotations
 
@@ -185,14 +186,23 @@
         severity: FindingSeverity,
     ):
         file_blocks = add_pngs_for_all_svgs(
             [b for b in report_blocks if isinstance(b, FileBlock)]
         )
         other_blocks = [b for b in report_blocks if not isinstance(b, FileBlock)]
 
+        # wide tables aren't displayed properly on slack. looks better in a text file
+        table_blocks = [b for b in other_blocks if isinstance(b, TableBlock)]
+        for table_block in table_blocks:
+            if len(table_block.headers) > SLACK_TABLE_COLUMNS_LIMIT:
+                table_name = table_block.table_name if table_block.table_name else "data"
+                table_content = table_block.to_table_string(table_max_width=250)  # bigger max width for file
+                file_blocks.append(FileBlock(f"{table_name}.txt", bytes(table_content, "utf-8")))
+                other_blocks.remove(table_block)
+
         message = self.prepare_slack_text(title, file_blocks)
 
         output_blocks = []
         if title:
             title = self.__add_slack_severity(title, severity)
             output_blocks.extend(self.__to_slack(HeaderBlock(title), sink_name))
         for block in other_blocks:
```

### Comparing `robusta-cli-0.9.7/src/robusta/model/config.py` & `robusta-cli-0.9.9/src/robusta/model/config.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/model/playbook_action.py` & `robusta-cli-0.9.9/src/robusta/model/playbook_action.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/model/playbook_definition.py` & `robusta-cli-0.9.9/src/robusta/model/playbook_definition.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/config_loader.py` & `robusta-cli-0.9.9/src/robusta/runner/config_loader.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/log_init.py` & `robusta-cli-0.9.9/src/robusta/runner/log_init.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/main.py` & `robusta-cli-0.9.9/src/robusta/runner/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import os
 import os.path
 from inspect import getmembers
 import manhole
 
-from src.robusta.runner.telemetry_service import TelemetryService, TelemetryLevel
-
-
+from .telemetry_service import TelemetryService, TelemetryLevel
 from .log_init import logging, init_logging
 from .web import Web
 from ..core.playbooks.playbooks_event_handler_impl import PlaybooksEventHandlerImpl
 from .. import api as robusta_api
 from .config_loader import ConfigLoader
 from ..model.config import Registry
 from ..core.model.env_vars import ROBUSTA_TELEMETRY_ENDPOINT, SEND_ADDITIONAL_TELEMETRY, \
```

### Comparing `robusta-cli-0.9.7/src/robusta/runner/object_updater.py` & `robusta-cli-0.9.9/src/robusta/runner/object_updater.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/telemetry.py` & `robusta-cli-0.9.9/src/robusta/runner/telemetry.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/telemetry_service.py` & `robusta-cli-0.9.9/src/robusta/runner/telemetry_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 import os
 from collections import defaultdict
 from enum import Enum
 from time import sleep
 import sentry_sdk
 import requests
 import threading
-from src.robusta.model.config import Registry, Telemetry
-from src.robusta.runner.telemetry import SinkInfo
+from ..model.config import Registry, Telemetry
+from .telemetry import SinkInfo
 
 from hikaru.model import NodeList
 
 class TelemetryLevel(Enum):
     NONE = 0,
     USAGE = 1,
     ERROR = 2
```

### Comparing `robusta-cli-0.9.7/src/robusta/runner/web.py` & `robusta-cli-0.9.9/src/robusta/runner/web.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/runner/web_api.py` & `robusta-cli-0.9.9/src/robusta/runner/web_api.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/common.py` & `robusta-cli-0.9.9/src/robusta/utils/common.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/decorators.py` & `robusta-cli-0.9.9/src/robusta/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/docs.py` & `robusta-cli-0.9.9/src/robusta/utils/docs.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/documented_pydantic.py` & `robusta-cli-0.9.9/src/robusta/utils/documented_pydantic.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/file_system_watcher.py` & `robusta-cli-0.9.9/src/robusta/utils/file_system_watcher.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/function_hashes.py` & `robusta-cli-0.9.9/src/robusta/utils/function_hashes.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/json_schema.py` & `robusta-cli-0.9.9/src/robusta/utils/json_schema.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/rate_limiter.py` & `robusta-cli-0.9.9/src/robusta/utils/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/service_discovery.py` & `robusta-cli-0.9.9/src/robusta/utils/service_discovery.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/src/robusta/utils/task_queue.py` & `robusta-cli-0.9.9/src/robusta/utils/task_queue.py`

 * *Files identical despite different names*

### Comparing `robusta-cli-0.9.7/setup.py` & `robusta-cli-0.9.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,51 +47,53 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['click-spinner>=0.1.10,<0.2.0',
  'colorlog>=5.0.1,<6.0.0',
+ 'cryptography>=36.0.0,<37.0.0',
  'docutils>=0.17.0,<0.18.0',
  'dpath>=2.0.5,<3.0.0',
  'hikaru>=0.5.1-beta.0,<0.6.0',
  'kubernetes>=12.0.1,<13.0.0',
  'markdown2>=2.4.2,<3.0.0',
  'opsgenie-sdk>=2.1.5,<3.0.0',
  'prometheus-client>=0.12.0,<0.13.0',
  'pydantic>=1.8.1,<2.0.0',
  'pymsteams>=0.1.16,<0.2.0',
  'pytz>=2021.3,<2022.0',
  'pyyaml>=6.0,<7.0',
- 'sentry-sdk>=1.5.2,<2.0.0',
  'slack-sdk>=3.7.0,<4.0.0',
  'toml>=0.10.2,<0.11.0',
  'typer>=0.3.2,<0.4.0',
- 'watchgod>=0.7,<0.8']
+ 'watchgod>=0.7,<0.8',
+ 'websocket-client>=1.3.2,<2.0.0']
 
 extras_require = \
 {':extra == "all"': ['tabulate>=0.8.9,<0.9.0'],
  'all': ['supabase-py>=0.0.2,<0.0.3',
          'Flask>=1.1.2,<2.0.0',
          'grafana-api>=1.0.3,<2.0.0',
          'manhole>=1.8.0,<2.0.0',
          'watchdog>=2.1.0,<3.0.0',
          'better-exceptions>=0.3.3,<0.4.0',
          'CairoSVG>=2.5.2,<3.0.0',
          'kafka-python>=2.0.2,<3.0.0',
          'prometheus-api-client>=0.4.2,<0.5.0',
          'datadog-api-client>=1.2.0,<2.0.0',
+         'sentry-sdk>=1.5.2,<2.0.0',
          'dulwich==0.20.28']}
 
 entry_points = \
 {'console_scripts': ['robusta = robusta.cli.main:app']}
 
 setup_kwargs = {
     'name': 'robusta-cli',
-    'version': '0.9.7',
+    'version': '0.9.9',
     'description': '',
     'long_description': None,
     'author': 'Natan Yellin',
     'author_email': 'aantn@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `robusta-cli-0.9.7/PKG-INFO` & `robusta-cli-0.9.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: robusta-cli
-Version: 0.9.7
+Version: 0.9.9
 Summary: 
 Author: Natan Yellin
 Author-email: aantn@users.noreply.github.com
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Provides-Extra: all
 Requires-Dist: CairoSVG (>=2.5.2,<3.0.0); extra == "all"
 Requires-Dist: Flask (>=1.1.2,<2.0.0); extra == "all"
 Requires-Dist: better-exceptions (>=0.3.3,<0.4.0); extra == "all"
 Requires-Dist: click-spinner (>=0.1.10,<0.2.0)
 Requires-Dist: colorlog (>=5.0.1,<6.0.0)
+Requires-Dist: cryptography (>=36.0.0,<37.0.0)
 Requires-Dist: datadog-api-client (>=1.2.0,<2.0.0); extra == "all"
 Requires-Dist: docutils (>=0.17.0,<0.18.0)
 Requires-Dist: dpath (>=2.0.5,<3.0.0)
 Requires-Dist: dulwich (==0.20.28); extra == "all"
 Requires-Dist: grafana-api (>=1.0.3,<2.0.0); extra == "all"
 Requires-Dist: hikaru (>=0.5.1-beta.0,<0.6.0)
 Requires-Dist: kafka-python (>=2.0.2,<3.0.0); extra == "all"
@@ -28,15 +29,16 @@
 Requires-Dist: opsgenie-sdk (>=2.1.5,<3.0.0)
 Requires-Dist: prometheus-api-client (>=0.4.2,<0.5.0); extra == "all"
 Requires-Dist: prometheus-client (>=0.12.0,<0.13.0)
 Requires-Dist: pydantic (>=1.8.1,<2.0.0)
 Requires-Dist: pymsteams (>=0.1.16,<0.2.0)
 Requires-Dist: pytz (>=2021.3,<2022.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
-Requires-Dist: sentry-sdk (>=1.5.2,<2.0.0)
+Requires-Dist: sentry-sdk (>=1.5.2,<2.0.0); extra == "all"
 Requires-Dist: slack-sdk (>=3.7.0,<4.0.0)
 Requires-Dist: supabase-py (>=0.0.2,<0.0.3); extra == "all"
 Requires-Dist: tabulate (>=0.8.9,<0.9.0); extra == "all"
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.3.2,<0.4.0)
 Requires-Dist: watchdog (>=2.1.0,<3.0.0); extra == "all"
 Requires-Dist: watchgod (>=0.7,<0.8)
+Requires-Dist: websocket-client (>=1.3.2,<2.0.0)
```

