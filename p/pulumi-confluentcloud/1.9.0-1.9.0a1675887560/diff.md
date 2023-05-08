# Comparing `tmp/pulumi_confluentcloud-1.9.0.tar.gz` & `tmp/pulumi_confluentcloud-1.9.0a1675887560.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_confluentcloud-1.9.0.tar", last modified: Wed Feb  8 21:56:11 2023, max compression
+gzip compressed data, was "pulumi_confluentcloud-1.9.0a1675887560.tar", last modified: Wed Feb  8 20:24:18 2023, max compression
```

## Comparing `pulumi_confluentcloud-1.9.0.tar` & `pulumi_confluentcloud-1.9.0a1675887560.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100537 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/cluster_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_identity_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_client_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_ksql_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_organization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_peering.py
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_private_link_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_subject_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_subject_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_transit_gateway_attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/identity_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/identity_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_client_quota.py
--rw-r--r--   0 runner    (1001) docker     (123)    33519 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_mirror_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/ksql_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    40999 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   113459 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/peering.py
--rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/private_link_access.py
--rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/role_binding.py
--rw-r--r--   0 runner    (1001) docker     (123)    36209 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/subject_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/subject_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/transit_gateway_attachment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 21:56:11.000000 pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 21:56:11.111232 pulumi_confluentcloud-1.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-02-08 21:56:10.000000 pulumi_confluentcloud-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100537 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19647 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19136 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/cluster_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20138 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9024 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8500 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_identity_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7167 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_client_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14412 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11418 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_ksql_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14767 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_private_link_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4975 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10300 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9458 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6096 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6645 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_subject_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_subject_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7766 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_transit_gateway_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6772 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25441 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/identity_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17163 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/identity_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32396 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20987 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_client_quota.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33519 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14429 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17720 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_mirror_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26637 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/ksql_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40999 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   113459 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16042 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/peering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17038 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/private_link_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18381 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13684 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/role_binding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36209 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20193 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17004 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14910 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10937 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19167 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/subject_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17121 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/subject_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15898 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/transit_gateway_attachment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-08 20:24:18.000000 pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-08 20:24:18.079669 pulumi_confluentcloud-1.9.0a1675887560/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-02-08 20:24:17.000000 pulumi_confluentcloud-1.9.0a1675887560/setup.py
```

### Comparing `pulumi_confluentcloud-1.9.0/PKG-INFO` & `pulumi_confluentcloud-1.9.0a1675887560/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_confluentcloud
-Version: 1.9.0
+Version: 1.9.0a1675887560
 Summary: A Pulumi package for creating and managing Confluent cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-confluentcloud
 Keywords: pulumi confluentcloud category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_confluentcloud-1.9.0/README.md` & `pulumi_confluentcloud-1.9.0a1675887560/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/__init__.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/_inputs.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/_utilities.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/api_key.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/api_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/cluster_link.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/cluster_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/config/vars.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/connector.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/connector.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/environment.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_environment.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_identity_pool.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_identity_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_identity_provider.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_client_quota.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_client_quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_kafka_topic.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_ksql_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_ksql_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_network.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_organization.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_organization.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_peering.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_private_link_access.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_private_link_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_role_binding.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster_config.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_cluster_mode.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_cluster_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_schema_registry_region.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_schema_registry_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_service_account.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_subject_config.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_subject_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_subject_mode.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_subject_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_transit_gateway_attachment.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_transit_gateway_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/get_user.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/identity_pool.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/identity_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/identity_provider.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/identity_provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_acl.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_acl.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_client_quota.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_client_quota.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_cluster_config.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_cluster_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_mirror_topic.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_mirror_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/kafka_topic.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/kafka_topic.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/ksql_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/ksql_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/network.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/outputs.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/peering.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/peering.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/private_link_access.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/private_link_access.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/provider.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/role_binding.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/role_binding.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster_config.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/schema_registry_cluster_mode.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/schema_registry_cluster_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/service_account.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/service_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/subject_config.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/subject_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/subject_mode.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/subject_mode.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud/transit_gateway_attachment.py` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud/transit_gateway_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/PKG-INFO` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-confluentcloud
-Version: 1.9.0
+Version: 1.9.0a1675887560
 Summary: A Pulumi package for creating and managing Confluent cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-confluentcloud
 Keywords: pulumi confluentcloud category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_confluentcloud-1.9.0/pulumi_confluentcloud.egg-info/SOURCES.txt` & `pulumi_confluentcloud-1.9.0a1675887560/pulumi_confluentcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_confluentcloud-1.9.0/setup.py` & `pulumi_confluentcloud-1.9.0a1675887560/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.9.0"
-PLUGIN_VERSION = "1.9.0"
+VERSION = "1.9.0a1675887560"
+PLUGIN_VERSION = "1.9.0-alpha.1675887560+735db8c0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'confluentcloud', PLUGIN_VERSION])
         except OSError as error:
```

