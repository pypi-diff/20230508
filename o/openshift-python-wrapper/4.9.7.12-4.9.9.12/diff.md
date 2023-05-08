# Comparing `tmp/openshift-python-wrapper-4.9.7.12.tar.gz` & `tmp/openshift-python-wrapper-4.9.9.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-python-wrapper-4.9.7.12.tar", last modified: Tue Nov  8 11:58:29 2022, max compression
+gzip compressed data, was "openshift-python-wrapper-4.9.9.12.tar", last modified: Mon Nov 14 11:31:50 2022, max compression
```

## Comparing `openshift-python-wrapper-4.9.7.12.tar` & `openshift-python-wrapper-4.9.9.12.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 11:58:29.394793 openshift-python-wrapper-4.9.7.12/
--rw-r--r--   0 root         (0) root         (0)    11357 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4380 2022-11-08 11:58:29.394793 openshift-python-wrapper-4.9.7.12/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3589 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 11:58:29.391793 openshift-python-wrapper-4.9.7.12/ocp_resources/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/__init__.py
--rw-r--r--   0 root         (0) root         (0)      171 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/api_service.py
--rw-r--r--   0 root         (0) root         (0)     2880 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/benchmark.py
--rw-r--r--   0 root         (0) root         (0)     1160 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/catalog_source.py
--rw-r--r--   0 root         (0) root         (0)     2756 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/catalog_source_config.py
--rw-r--r--   0 root         (0) root         (0)      248 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cdi.py
--rw-r--r--   0 root         (0) root         (0)     1573 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cdi_config.py
--rw-r--r--   0 root         (0) root         (0)      959 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/chaos_engine.py
--rw-r--r--   0 root         (0) root         (0)      133 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_operator.py
--rw-r--r--   0 root         (0) root         (0)     1096 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_role.py
--rw-r--r--   0 root         (0) root         (0)      215 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_role_binding.py
--rw-r--r--   0 root         (0) root         (0)      250 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_service_version.py
--rw-r--r--   0 root         (0) root         (0)      132 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_version.py
--rw-r--r--   0 root         (0) root         (0)      739 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/configmap.py
--rw-r--r--   0 root         (0) root         (0)      210 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/console_cli_download.py
--rw-r--r--   0 root         (0) root         (0)      183 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/console_quick_start.py
--rw-r--r--   0 root         (0) root         (0)      207 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/constants.py
--rw-r--r--   0 root         (0) root         (0)      161 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/csidriver.py
--rw-r--r--   0 root         (0) root         (0)      143 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/custom_resource_definition.py
--rw-r--r--   0 root         (0) root         (0)     1955 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/daemonset.py
--rw-r--r--   0 root         (0) root         (0)      811 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/data_source.py
--rw-r--r--   0 root         (0) root         (0)     7378 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/datavolume.py
--rw-r--r--   0 root         (0) root         (0)     1861 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/deployment.py
--rw-r--r--   0 root         (0) root         (0)      234 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/destination_rule.py
--rw-r--r--   0 root         (0) root         (0)     4017 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/event.py
--rw-r--r--   0 root         (0) root         (0)      217 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/gateway.py
--rw-r--r--   0 root         (0) root         (0)     1792 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/host.py
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/hostpath_provisioner.py
--rw-r--r--   0 root         (0) root         (0)      978 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/hyperconverged.py
--rw-r--r--   0 root         (0) root         (0)      203 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/image_content_source_policy.py
--rw-r--r--   0 root         (0) root         (0)      205 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/imagestreamtag.py
--rw-r--r--   0 root         (0) root         (0)      373 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/infrastructure.py
--rw-r--r--   0 root         (0) root         (0)      236 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/installplan.py
--rw-r--r--   0 root         (0) root         (0)     1916 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kube_descheduler.py
--rw-r--r--   0 root         (0) root         (0)      148 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kubevirt.py
--rw-r--r--   0 root         (0) root         (0)      173 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kubevirt_common_templates_bundle.py
--rw-r--r--   0 root         (0) root         (0)      170 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kubevirt_metrics_aggregation.py
--rw-r--r--   0 root         (0) root         (0)      170 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kubevirt_node_labeller_bundle.py
--rw-r--r--   0 root         (0) root         (0)      169 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/kubevirt_template_validaotr.py
--rw-r--r--   0 root         (0) root         (0)     2445 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/logger.py
--rw-r--r--   0 root         (0) root         (0)     1062 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/machine.py
--rw-r--r--   0 root         (0) root         (0)      243 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/machine_config_pool.py
--rw-r--r--   0 root         (0) root         (0)     2501 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/machine_health_check.py
--rw-r--r--   0 root         (0) root         (0)     6215 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/machine_set.py
--rw-r--r--   0 root         (0) root         (0)     1510 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/migration.py
--rw-r--r--   0 root         (0) root         (0)     5281 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/mtv.py
--rw-r--r--   0 root         (0) root         (0)      213 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/mutating_webhook_config.py
--rw-r--r--   0 root         (0) root         (0)     1144 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/namespace.py
--rw-r--r--   0 root         (0) root         (0)      125 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/network.py
--rw-r--r--   0 root         (0) root         (0)      253 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/network_addons_config.py
--rw-r--r--   0 root         (0) root         (0)      792 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/network_attachment_definition.py
--rw-r--r--   0 root         (0) root         (0)     2095 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/network_map.py
--rw-r--r--   0 root         (0) root         (0)      202 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/network_policy.py
--rw-r--r--   0 root         (0) root         (0)     1124 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/node.py
--rw-r--r--   0 root         (0) root         (0)      912 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/node_maintenance.py
--rw-r--r--   0 root         (0) root         (0)      142 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/node_network_configuration_enactment.py
--rw-r--r--   0 root         (0) root         (0)    14405 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/node_network_configuration_policy.py
--rw-r--r--   0 root         (0) root         (0)     3264 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/node_network_state.py
--rw-r--r--   0 root         (0) root         (0)      158 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/oauth.py
--rw-r--r--   0 root         (0) root         (0)      166 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/operator_condition.py
--rw-r--r--   0 root         (0) root         (0)      934 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/operator_group.py
--rw-r--r--   0 root         (0) root         (0)      129 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/operator_hub.py
--rw-r--r--   0 root         (0) root         (0)     1327 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/operator_source.py
--rw-r--r--   0 root         (0) root         (0)      173 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/package_manifest.py
--rw-r--r--   0 root         (0) root         (0)      344 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/peer_authentication.py
--rw-r--r--   0 root         (0) root         (0)      603 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/persistent_volume.py
--rw-r--r--   0 root         (0) root         (0)     2564 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/persistent_volume_claim.py
--rw-r--r--   0 root         (0) root         (0)     4004 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/plan.py
--rw-r--r--   0 root         (0) root         (0)     4609 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/pod.py
--rw-r--r--   0 root         (0) root         (0)     1246 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/pod_disruption_budget.py
--rw-r--r--   0 root         (0) root         (0)     1169 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/priority_class.py
--rw-r--r--   0 root         (0) root         (0)     1131 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/project.py
--rw-r--r--   0 root         (0) root         (0)      209 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/prometheus_rule.py
--rw-r--r--   0 root         (0) root         (0)     1423 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/provider.py
--rw-r--r--   0 root         (0) root         (0)      215 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/replicaset.py
--rw-r--r--   0 root         (0) root         (0)    37181 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/resource.py
--rw-r--r--   0 root         (0) root         (0)      217 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/role.py
--rw-r--r--   0 root         (0) root         (0)     1872 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/role_binding.py
--rw-r--r--   0 root         (0) root         (0)     1790 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/route.py
--rw-r--r--   0 root         (0) root         (0)     1684 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/secret.py
--rw-r--r--   0 root         (0) root         (0)      204 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/security_context_constraints.py
--rw-r--r--   0 root         (0) root         (0)      295 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/service.py
--rw-r--r--   0 root         (0) root         (0)      193 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/service_account.py
--rw-r--r--   0 root         (0) root         (0)      243 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/service_mesh_control_plane.py
--rw-r--r--   0 root         (0) root         (0)      292 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/service_mesh_member_roll.py
--rw-r--r--   0 root         (0) root         (0)      209 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/service_monitor.py
--rw-r--r--   0 root         (0) root         (0)     1155 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network.py
--rw-r--r--   0 root         (0) root         (0)     1780 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network_node_policy.py
--rw-r--r--   0 root         (0) root         (0)     1250 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network_node_state.py
--rw-r--r--   0 root         (0) root         (0)      180 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/ssp.py
--rw-r--r--   0 root         (0) root         (0)     1397 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/storage_class.py
--rw-r--r--   0 root         (0) root         (0)     2251 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/storage_map.py
--rw-r--r--   0 root         (0) root         (0)     1853 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/subscription.py
--rw-r--r--   0 root         (0) root         (0)     2738 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/template.py
--rw-r--r--   0 root         (0) root         (0)      826 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/upload_token_request.py
--rw-r--r--   0 root         (0) root         (0)     7197 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/utils.py
--rw-r--r--   0 root         (0) root         (0)      217 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/validating_webhook_config.py
--rw-r--r--   0 root         (0) root         (0)     4691 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine.py
--rw-r--r--   0 root         (0) root         (0)      523 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_Instance_replica_set.py
--rw-r--r--   0 root         (0) root         (0)    10464 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_import.py
--rw-r--r--   0 root         (0) root         (0)     9815 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance.py
--rw-r--r--   0 root         (0) root         (0)      905 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance_migration.py
--rw-r--r--   0 root         (0) root         (0)      560 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance_preset.py
--rw-r--r--   0 root         (0) root         (0)     2152 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_restore.py
--rw-r--r--   0 root         (0) root         (0)     2072 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_snapshot.py
--rw-r--r--   0 root         (0) root         (0)      232 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_service.py
--rw-r--r--   0 root         (0) root         (0)      188 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/vm_import_config.py
--rw-r--r--   0 root         (0) root         (0)      210 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/volume_snapshot.py
--rw-r--r--   0 root         (0) root         (0)      190 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/ocp_resources/volume_snapshot_class.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 11:58:29.392793 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4380 2022-11-08 11:58:29.000000 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4022 2022-11-08 11:58:29.000000 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-08 11:58:29.000000 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       45 2022-11-08 11:58:29.000000 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2022-11-08 11:58:29.000000 openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       30 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      753 2022-11-08 11:58:29.395793 openshift-python-wrapper-4.9.7.12/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      418 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-08 11:58:29.393793 openshift-python-wrapper-4.9.7.12/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      827 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/tests/test_resources.py
--rw-r--r--   0 root         (0) root         (0)     4795 2022-11-08 11:58:21.000000 openshift-python-wrapper-4.9.7.12/tests/test_validate_resources.py
--rw-r--r--   0 root         (0) root         (0)     1136 2022-11-08 11:58:20.000000 openshift-python-wrapper-4.9.7.12/tests/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 11:31:50.086546 openshift-python-wrapper-4.9.9.12/
+-rw-r--r--   0 root         (0) root         (0)    11357 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4380 2022-11-14 11:31:50.087546 openshift-python-wrapper-4.9.9.12/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3589 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 11:31:50.085546 openshift-python-wrapper-4.9.9.12/ocp_resources/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      171 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/api_service.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/benchmark.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/catalog_source.py
+-rw-r--r--   0 root         (0) root         (0)     2756 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/catalog_source_config.py
+-rw-r--r--   0 root         (0) root         (0)      248 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cdi.py
+-rw-r--r--   0 root         (0) root         (0)     1573 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cdi_config.py
+-rw-r--r--   0 root         (0) root         (0)      959 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/chaos_engine.py
+-rw-r--r--   0 root         (0) root         (0)      133 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_operator.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_role.py
+-rw-r--r--   0 root         (0) root         (0)      215 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_role_binding.py
+-rw-r--r--   0 root         (0) root         (0)      250 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_service_version.py
+-rw-r--r--   0 root         (0) root         (0)      132 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_version.py
+-rw-r--r--   0 root         (0) root         (0)      739 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/configmap.py
+-rw-r--r--   0 root         (0) root         (0)      210 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/console_cli_download.py
+-rw-r--r--   0 root         (0) root         (0)      183 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/console_quick_start.py
+-rw-r--r--   0 root         (0) root         (0)      230 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/constants.py
+-rw-r--r--   0 root         (0) root         (0)      161 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/csidriver.py
+-rw-r--r--   0 root         (0) root         (0)      143 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/custom_resource_definition.py
+-rw-r--r--   0 root         (0) root         (0)     1955 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/daemonset.py
+-rw-r--r--   0 root         (0) root         (0)      811 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/data_source.py
+-rw-r--r--   0 root         (0) root         (0)     7378 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/datavolume.py
+-rw-r--r--   0 root         (0) root         (0)     1861 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/deployment.py
+-rw-r--r--   0 root         (0) root         (0)      234 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/destination_rule.py
+-rw-r--r--   0 root         (0) root         (0)     4017 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/event.py
+-rw-r--r--   0 root         (0) root         (0)      217 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/gateway.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/host.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/hostpath_provisioner.py
+-rw-r--r--   0 root         (0) root         (0)      978 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/hyperconverged.py
+-rw-r--r--   0 root         (0) root         (0)      203 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/image_content_source_policy.py
+-rw-r--r--   0 root         (0) root         (0)      205 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/imagestreamtag.py
+-rw-r--r--   0 root         (0) root         (0)      373 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/infrastructure.py
+-rw-r--r--   0 root         (0) root         (0)      236 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/installplan.py
+-rw-r--r--   0 root         (0) root         (0)     1916 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kube_descheduler.py
+-rw-r--r--   0 root         (0) root         (0)      148 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kubevirt.py
+-rw-r--r--   0 root         (0) root         (0)      173 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kubevirt_common_templates_bundle.py
+-rw-r--r--   0 root         (0) root         (0)      170 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kubevirt_metrics_aggregation.py
+-rw-r--r--   0 root         (0) root         (0)      170 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kubevirt_node_labeller_bundle.py
+-rw-r--r--   0 root         (0) root         (0)      169 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/kubevirt_template_validaotr.py
+-rw-r--r--   0 root         (0) root         (0)     2445 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/machine.py
+-rw-r--r--   0 root         (0) root         (0)      243 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/machine_config_pool.py
+-rw-r--r--   0 root         (0) root         (0)     2501 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/machine_health_check.py
+-rw-r--r--   0 root         (0) root         (0)     6215 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/machine_set.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/migration.py
+-rw-r--r--   0 root         (0) root         (0)     5281 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/mtv.py
+-rw-r--r--   0 root         (0) root         (0)      213 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/mutating_webhook_config.py
+-rw-r--r--   0 root         (0) root         (0)     1144 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/namespace.py
+-rw-r--r--   0 root         (0) root         (0)      125 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/network.py
+-rw-r--r--   0 root         (0) root         (0)      253 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/network_addons_config.py
+-rw-r--r--   0 root         (0) root         (0)      792 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/network_attachment_definition.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/network_map.py
+-rw-r--r--   0 root         (0) root         (0)      202 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/network_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/node.py
+-rw-r--r--   0 root         (0) root         (0)      912 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/node_maintenance.py
+-rw-r--r--   0 root         (0) root         (0)      142 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/node_network_configuration_enactment.py
+-rw-r--r--   0 root         (0) root         (0)    14405 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/node_network_configuration_policy.py
+-rw-r--r--   0 root         (0) root         (0)     3264 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/node_network_state.py
+-rw-r--r--   0 root         (0) root         (0)      158 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/oauth.py
+-rw-r--r--   0 root         (0) root         (0)      166 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/operator_condition.py
+-rw-r--r--   0 root         (0) root         (0)      934 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/operator_group.py
+-rw-r--r--   0 root         (0) root         (0)      129 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/operator_hub.py
+-rw-r--r--   0 root         (0) root         (0)     1327 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/operator_source.py
+-rw-r--r--   0 root         (0) root         (0)      173 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/package_manifest.py
+-rw-r--r--   0 root         (0) root         (0)      344 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/peer_authentication.py
+-rw-r--r--   0 root         (0) root         (0)      603 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/persistent_volume.py
+-rw-r--r--   0 root         (0) root         (0)     2564 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/persistent_volume_claim.py
+-rw-r--r--   0 root         (0) root         (0)     4004 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/plan.py
+-rw-r--r--   0 root         (0) root         (0)     4609 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/pod.py
+-rw-r--r--   0 root         (0) root         (0)     1246 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/pod_disruption_budget.py
+-rw-r--r--   0 root         (0) root         (0)     1169 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/priority_class.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/project.py
+-rw-r--r--   0 root         (0) root         (0)      209 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/prometheus_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1423 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/provider.py
+-rw-r--r--   0 root         (0) root         (0)      215 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/replicaset.py
+-rw-r--r--   0 root         (0) root         (0)    37181 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/resource.py
+-rw-r--r--   0 root         (0) root         (0)      217 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/role.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/role_binding.py
+-rw-r--r--   0 root         (0) root         (0)     1790 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/route.py
+-rw-r--r--   0 root         (0) root         (0)     1684 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/secret.py
+-rw-r--r--   0 root         (0) root         (0)      204 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/security_context_constraints.py
+-rw-r--r--   0 root         (0) root         (0)      295 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/service.py
+-rw-r--r--   0 root         (0) root         (0)      193 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/service_account.py
+-rw-r--r--   0 root         (0) root         (0)      243 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/service_mesh_control_plane.py
+-rw-r--r--   0 root         (0) root         (0)      292 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/service_mesh_member_roll.py
+-rw-r--r--   0 root         (0) root         (0)      209 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/service_monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network_node_policy.py
+-rw-r--r--   0 root         (0) root         (0)     1250 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network_node_state.py
+-rw-r--r--   0 root         (0) root         (0)      180 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/ssp.py
+-rw-r--r--   0 root         (0) root         (0)     1397 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/storage_class.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/storage_map.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/subscription.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/template.py
+-rw-r--r--   0 root         (0) root         (0)      826 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/upload_token_request.py
+-rw-r--r--   0 root         (0) root         (0)     7197 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/utils.py
+-rw-r--r--   0 root         (0) root         (0)      217 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/validating_webhook_config.py
+-rw-r--r--   0 root         (0) root         (0)     5156 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine.py
+-rw-r--r--   0 root         (0) root         (0)      523 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_Instance_replica_set.py
+-rw-r--r--   0 root         (0) root         (0)    10464 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_import.py
+-rw-r--r--   0 root         (0) root         (0)     9815 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance.py
+-rw-r--r--   0 root         (0) root         (0)      905 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance_migration.py
+-rw-r--r--   0 root         (0) root         (0)      560 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance_preset.py
+-rw-r--r--   0 root         (0) root         (0)     2975 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_restore.py
+-rw-r--r--   0 root         (0) root         (0)     2907 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      232 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_service.py
+-rw-r--r--   0 root         (0) root         (0)      188 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/vm_import_config.py
+-rw-r--r--   0 root         (0) root         (0)      210 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/volume_snapshot.py
+-rw-r--r--   0 root         (0) root         (0)      190 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/ocp_resources/volume_snapshot_class.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 11:31:50.086546 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4380 2022-11-14 11:31:50.000000 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4022 2022-11-14 11:31:50.000000 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-14 11:31:50.000000 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       45 2022-11-14 11:31:50.000000 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2022-11-14 11:31:50.000000 openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      753 2022-11-14 11:31:50.087546 openshift-python-wrapper-4.9.9.12/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      418 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-14 11:31:50.086546 openshift-python-wrapper-4.9.9.12/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      827 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/tests/test_resources.py
+-rw-r--r--   0 root         (0) root         (0)     4795 2022-11-14 11:31:42.000000 openshift-python-wrapper-4.9.9.12/tests/test_validate_resources.py
+-rw-r--r--   0 root         (0) root         (0)     1136 2022-11-14 11:31:41.000000 openshift-python-wrapper-4.9.9.12/tests/utils.py
```

### Comparing `openshift-python-wrapper-4.9.7.12/LICENSE` & `openshift-python-wrapper-4.9.9.12/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/PKG-INFO` & `openshift-python-wrapper-4.9.9.12/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: openshift-python-wrapper
-Version: 4.9.7.12
+Version: 4.9.9.12
 Summary: Wrapper around https://github.com/openshift/openshift-restclient-python
 Home-page: https://github.com/RedHatQE/openshift-python-wrapper
-Download-URL: https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.7.12.tar.gz
+Download-URL: https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.9.12.tar.gz
 Author: Meni Yakove, Ruth Netser
 Author-email: myakove@redhat.com
 License: apache-2.0
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-wrapper/issues
 Project-URL: Documentation, https://openshift-python-wrapper.readthedocs.io/en/latest/
 Keywords: Openshift,Kubevirt,CNV
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openshift-python-wrapper-4.9.7.12/README.md` & `openshift-python-wrapper-4.9.9.12/README.md`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/benchmark.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/benchmark.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/catalog_source.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/catalog_source.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/catalog_source_config.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/catalog_source_config.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/cdi_config.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/cdi_config.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/chaos_engine.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/chaos_engine.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/cluster_role.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/cluster_role.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/configmap.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/configmap.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/daemonset.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/daemonset.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/data_source.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/data_source.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/datavolume.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/datavolume.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/deployment.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/deployment.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/event.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/event.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/host.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/host.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/hostpath_provisioner.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/hostpath_provisioner.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/hyperconverged.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/hyperconverged.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/kube_descheduler.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/kube_descheduler.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/logger.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/logger.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/machine.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/machine.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/machine_health_check.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/machine_health_check.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/machine_set.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/machine_set.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/migration.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/migration.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/mtv.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/mtv.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/namespace.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/namespace.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/network_attachment_definition.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/network_attachment_definition.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/network_map.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/network_map.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/node.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/node.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/node_maintenance.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/node_maintenance.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/node_network_configuration_policy.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/node_network_configuration_policy.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/node_network_state.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/node_network_state.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/operator_group.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/operator_group.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/operator_source.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/operator_source.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/persistent_volume.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/persistent_volume.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/persistent_volume_claim.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/persistent_volume_claim.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/plan.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/plan.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/pod.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/pod.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/pod_disruption_budget.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/pod_disruption_budget.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/priority_class.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/priority_class.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/project.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/project.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/provider.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/provider.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/resource.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/resource.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/role_binding.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/role_binding.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/route.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/route.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/secret.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/secret.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network_node_policy.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network_node_policy.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/sriov_network_node_state.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/sriov_network_node_state.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/storage_class.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/storage_class.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/storage_map.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/storage_map.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/subscription.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/subscription.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/template.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/template.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/upload_token_request.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/upload_token_request.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/utils.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/utils.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 
-from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT
+from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT, TIMEOUT_4MINUTES
 from ocp_resources.resource import TIMEOUT, NamespacedResource
 from ocp_resources.utils import TimeoutSampler
 from ocp_resources.virtual_machine_instance import VirtualMachineInstance
 
 
 class VirtualMachine(NamespacedResource):
     """
@@ -149,7 +149,18 @@
         """
         Get VM printableStatus
 
         Returns:
             VM printableStatus if VM.status.printableStatus else None
         """
         return self.instance.get("status", {}).get("printableStatus")
+
+    def wait_for_status_none(self, status, timeout=TIMEOUT_4MINUTES):
+        self.logger.info(f"Wait for {self.kind} {self.name} status {status} to be None")
+        for sample in TimeoutSampler(
+            wait_timeout=timeout,
+            sleep=1,
+            exceptions_dict=PROTOCOL_ERROR_EXCEPTION_DICT,
+            func=lambda: self.instance.get("status", {}).get(status),
+        ):
+            if sample is None:
+                return
```

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_Instance_replica_set.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_Instance_replica_set.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_import.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_import.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance_migration.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance_migration.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_instance_preset.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_instance_preset.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_restore.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_restore.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # -*- coding: utf-8 -*-
 
+from openshift.dynamic.exceptions import ResourceNotFoundError
 
-from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT
+from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT, TIMEOUT_4MINUTES
 from ocp_resources.resource import TIMEOUT, NamespacedResource
 from ocp_resources.utils import TimeoutSampler
 from ocp_resources.virtual_machine import VirtualMachine
 
 
 class VirtualMachineRestore(NamespacedResource):
     """
@@ -69,7 +70,30 @@
             exceptions_dict=PROTOCOL_ERROR_EXCEPTION_DICT,
             func=lambda: self.instance.get("status", {}).get("complete", None)
             == status,
         )
         for sample in samples:
             if sample:
                 return
+
+    def wait_restore_done(self, timeout=TIMEOUT_4MINUTES):
+        """
+        Wait for the the restore to be done. This check 2 parameters, the restore status to be complete
+        and the VM status restoreInProgress to be None.
+
+        Args:
+            timeout (int): Time to wait.
+
+        Raises:
+            TimeoutExpiredError: If timeout reached.
+        """
+        self.wait_complete(timeout=timeout)
+
+        vm = VirtualMachine(
+            client=self.client,
+            namespace=self.namespace,
+            name=self.vm_name,
+        )
+
+        if vm.exists:
+            return vm.wait_for_status_none(status="restoreInProgress", timeout=timeout)
+        raise ResourceNotFoundError(f"VirtualMachine: {vm.name} not found")
```

### Comparing `openshift-python-wrapper-4.9.7.12/ocp_resources/virtual_machine_snapshot.py` & `openshift-python-wrapper-4.9.9.12/ocp_resources/virtual_machine_snapshot.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # -*- coding: utf-8 -*-
 
 
-from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT
+from openshift.dynamic.exceptions import ResourceNotFoundError
+
+from ocp_resources.constants import PROTOCOL_ERROR_EXCEPTION_DICT, TIMEOUT_4MINUTES
 from ocp_resources.resource import TIMEOUT, NamespacedResource
 from ocp_resources.utils import TimeoutSampler
 from ocp_resources.virtual_machine import VirtualMachine
 
 
 class VirtualMachineSnapshot(NamespacedResource):
     """
@@ -66,7 +68,30 @@
             exceptions_dict=PROTOCOL_ERROR_EXCEPTION_DICT,
             func=lambda: self.instance.get("status", {}).get("readyToUse", None)
             == status,
         )
         for sample in samples:
             if sample:
                 return
+
+    def wait_snapshot_done(self, timeout=TIMEOUT_4MINUTES):
+        """
+        Wait for the the snapshot to be done. This check 2 parameters, the snapshot status to be readyToUse
+        and the VM status snapshotInProgress to be None.
+
+        Args:
+            timeout (int): Time to wait.
+
+        Raises:
+            TimeoutExpiredError: If timeout reached.
+        """
+        self.wait_ready_to_use(timeout=timeout)
+
+        vm = VirtualMachine(
+            client=self.client,
+            namespace=self.namespace,
+            name=self.vm_name,
+        )
+
+        if vm.exists:
+            return vm.wait_for_status_none(status="snapshotInProgress", timeout=timeout)
+        raise ResourceNotFoundError(f"VirtualMachine: {vm.name} not found")
```

### Comparing `openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/PKG-INFO` & `openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: openshift-python-wrapper
-Version: 4.9.7.12
+Version: 4.9.9.12
 Summary: Wrapper around https://github.com/openshift/openshift-restclient-python
 Home-page: https://github.com/RedHatQE/openshift-python-wrapper
-Download-URL: https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.7.12.tar.gz
+Download-URL: https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.9.12.tar.gz
 Author: Meni Yakove, Ruth Netser
 Author-email: myakove@redhat.com
 License: apache-2.0
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-wrapper/issues
 Project-URL: Documentation, https://openshift-python-wrapper.readthedocs.io/en/latest/
 Keywords: Openshift,Kubevirt,CNV
 Classifier: Programming Language :: Python :: 3
```

### Comparing `openshift-python-wrapper-4.9.7.12/openshift_python_wrapper.egg-info/SOURCES.txt` & `openshift-python-wrapper-4.9.9.12/openshift_python_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/setup.cfg` & `openshift-python-wrapper-4.9.9.12/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [metadata]
 name = openshift-python-wrapper
-version = 4.9.7.12
+version = 4.9.9.12
 author = Meni Yakove, Ruth Netser
 author_email = myakove@redhat.com
 description = Wrapper around https://github.com/openshift/openshift-restclient-python
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/RedHatQE/openshift-python-wrapper
-download_url = https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.7.12.tar.gz
+download_url = https://github.com/RedHatQE/openshift-python-wrapper/archive/refs/tags/v4.9.9.12.tar.gz
 project_urls = 
 	Bug Tracker = https://github.com/RedHatQE/openshift-python-wrapper/issues
 	Documentation = https://openshift-python-wrapper.readthedocs.io/en/latest/
 classifiers = 
 	Programming Language :: Python :: 3
 	Operating System :: OS Independent
```

### Comparing `openshift-python-wrapper-4.9.7.12/tests/test_resources.py` & `openshift-python-wrapper-4.9.9.12/tests/test_resources.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/tests/test_validate_resources.py` & `openshift-python-wrapper-4.9.9.12/tests/test_validate_resources.py`

 * *Files identical despite different names*

### Comparing `openshift-python-wrapper-4.9.7.12/tests/utils.py` & `openshift-python-wrapper-4.9.9.12/tests/utils.py`

 * *Files identical despite different names*

