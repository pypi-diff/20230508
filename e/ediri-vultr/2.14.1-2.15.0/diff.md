# Comparing `tmp/ediri_vultr-2.14.1.tar.gz` & `tmp/ediri_vultr-2.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_vultr-2.14.1.tar", last modified: Thu May  4 12:15:31 2023, max compression
+gzip compressed data, was "ediri_vultr-2.15.0.tar", last modified: Mon May  8 13:30:47 2023, max compression
```

## Comparing `ediri_vultr-2.14.1.tar` & `ediri_vultr-2.15.0.tar`

### file list

```diff
@@ -1,74 +1,80 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.027830 ediri_vultr-2.14.1/ediri_vultr/
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48976 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/block_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/ediri_vultr/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/dns_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/firewall_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_backup.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_block_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_dns_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_firewall_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_iso_public.py
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_os.py
--rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/instance_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/iso_private.py
--rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/kubernetes_node_pools.py
--rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    47909 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/private_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reserved_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reverse_ipv4.py
--rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/reverse_ipv6.py
--rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/snapshot_from_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/startup_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/ediri_vultr/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/ediri_vultr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 12:15:31.000000 ediri_vultr-2.14.1/ediri_vultr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 12:15:31.031830 ediri_vultr-2.14.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-04 12:15:30.000000 ediri_vultr-2.14.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/ediri_vultr/
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62475 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56372 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22078 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/block_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/ediri_vultr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38086 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11447 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/database_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6287 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/database_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33012 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/database_replica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/database_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/dns_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21767 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/firewall_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_backup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_bare_metal_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12578 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_bare_metal_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_block_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14784 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_dns_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_firewall_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18081 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5695 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_iso_public.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12356 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7815 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_os.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7665 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6114 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5002 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6184 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6105 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5690 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5662 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81215 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12872 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/instance_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9029 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/iso_private.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26831 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25686 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/kubernetes_node_pools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41761 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16291 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64790 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15077 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/private_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15244 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/reserved_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12813 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/reverse_ipv4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9869 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/reverse_ipv6.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14099 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12898 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/snapshot_from_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12267 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/startup_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15601 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14407 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/ediri_vultr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/ediri_vultr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:30:47.407019 ediri_vultr-2.15.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-08 13:30:47.000000 ediri_vultr-2.15.0/setup.py
```

### Comparing `ediri_vultr-2.14.1/PKG-INFO` & `ediri_vultr-2.15.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri_vultr
-Version: 2.14.1
+Version: 2.15.0
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_vultr-2.14.1/README.md` & `ediri_vultr-2.15.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/__init__.py` & `ediri_vultr-2.15.0/ediri_vultr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,24 +3,30 @@
 # *** Do not edit by hand unless you're certain you know what you are doing! ***
 
 from . import _utilities
 import typing
 # Export this package's modules as members:
 from .bare_metal_server import *
 from .block_storage import *
+from .database import *
+from .database_connection_pool import *
+from .database_db import *
+from .database_replica import *
+from .database_user import *
 from .dns_domain import *
 from .dns_record import *
 from .firewall_group import *
 from .firewall_rule import *
 from .get_account import *
 from .get_application import *
 from .get_backup import *
 from .get_bare_metal_plan import *
 from .get_bare_metal_server import *
 from .get_block_storage import *
+from .get_database import *
 from .get_dns_domain import *
 from .get_firewall_group import *
 from .get_instance import *
 from .get_instance_ipv4 import *
 from .get_iso_private import *
 from .get_iso_public import *
 from .get_kubernetes import *
@@ -84,14 +90,54 @@
   "fqn": "ediri_vultr",
   "classes": {
    "vultr:index/blockStorage:BlockStorage": "BlockStorage"
   }
  },
  {
   "pkg": "vultr",
+  "mod": "index/database",
+  "fqn": "ediri_vultr",
+  "classes": {
+   "vultr:index/database:Database": "Database"
+  }
+ },
+ {
+  "pkg": "vultr",
+  "mod": "index/databaseConnectionPool",
+  "fqn": "ediri_vultr",
+  "classes": {
+   "vultr:index/databaseConnectionPool:DatabaseConnectionPool": "DatabaseConnectionPool"
+  }
+ },
+ {
+  "pkg": "vultr",
+  "mod": "index/databaseDb",
+  "fqn": "ediri_vultr",
+  "classes": {
+   "vultr:index/databaseDb:DatabaseDb": "DatabaseDb"
+  }
+ },
+ {
+  "pkg": "vultr",
+  "mod": "index/databaseReplica",
+  "fqn": "ediri_vultr",
+  "classes": {
+   "vultr:index/databaseReplica:DatabaseReplica": "DatabaseReplica"
+  }
+ },
+ {
+  "pkg": "vultr",
+  "mod": "index/databaseUser",
+  "fqn": "ediri_vultr",
+  "classes": {
+   "vultr:index/databaseUser:DatabaseUser": "DatabaseUser"
+  }
+ },
+ {
+  "pkg": "vultr",
   "mod": "index/dnsDomain",
   "fqn": "ediri_vultr",
   "classes": {
    "vultr:index/dnsDomain:DnsDomain": "DnsDomain"
   }
  },
  {
```

### Comparing `ediri_vultr-2.14.1/ediri_vultr/_inputs.py` & `ediri_vultr-2.15.0/ediri_vultr/_inputs.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,26 +6,28 @@
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 
 __all__ = [
+    'DatabaseReadReplicaArgs',
     'InstanceBackupsScheduleArgs',
     'KubernetesNodePoolsArgs',
     'KubernetesNodePoolsNodeArgs',
     'LoadBalancerFirewallRuleArgs',
     'LoadBalancerForwardingRuleArgs',
     'LoadBalancerHealthCheckArgs',
     'LoadBalancerSslArgs',
     'GetApplicationFilterArgs',
     'GetBackupFilterArgs',
     'GetBareMetalPlanFilterArgs',
     'GetBareMetalServerFilterArgs',
     'GetBlockStorageFilterArgs',
+    'GetDatabaseFilterArgs',
     'GetFirewallGroupFilterArgs',
     'GetInstanceFilterArgs',
     'GetInstanceIpv4FilterArgs',
     'GetIsoPrivateFilterArgs',
     'GetIsoPublicFilterArgs',
     'GetKubernetesFilterArgs',
     'GetLoadBalancerFilterArgs',
@@ -42,14 +44,353 @@
     'GetSshKeyFilterArgs',
     'GetStartupScriptFilterArgs',
     'GetUserFilterArgs',
     'GetVpcFilterArgs',
 ]
 
 @pulumi.input_type
+class DatabaseReadReplicaArgs:
+    def __init__(__self__, *,
+                 label: pulumi.Input[str],
+                 region: pulumi.Input[str],
+                 cluster_time_zone: Optional[pulumi.Input[str]] = None,
+                 database_engine: Optional[pulumi.Input[str]] = None,
+                 database_engine_version: Optional[pulumi.Input[str]] = None,
+                 date_created: Optional[pulumi.Input[str]] = None,
+                 dbname: Optional[pulumi.Input[str]] = None,
+                 host: Optional[pulumi.Input[str]] = None,
+                 id: Optional[pulumi.Input[str]] = None,
+                 latest_backup: Optional[pulumi.Input[str]] = None,
+                 maintenance_dow: Optional[pulumi.Input[str]] = None,
+                 maintenance_time: Optional[pulumi.Input[str]] = None,
+                 mysql_long_query_time: Optional[pulumi.Input[int]] = None,
+                 mysql_require_primary_key: Optional[pulumi.Input[bool]] = None,
+                 mysql_slow_query_log: Optional[pulumi.Input[bool]] = None,
+                 mysql_sql_modes: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 password: Optional[pulumi.Input[str]] = None,
+                 plan: Optional[pulumi.Input[str]] = None,
+                 plan_disk: Optional[pulumi.Input[int]] = None,
+                 plan_ram: Optional[pulumi.Input[int]] = None,
+                 plan_replicas: Optional[pulumi.Input[int]] = None,
+                 plan_vcpus: Optional[pulumi.Input[int]] = None,
+                 port: Optional[pulumi.Input[str]] = None,
+                 redis_eviction_policy: Optional[pulumi.Input[str]] = None,
+                 status: Optional[pulumi.Input[str]] = None,
+                 tag: Optional[pulumi.Input[str]] = None,
+                 trusted_ips: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
+                 user: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "region", region)
+        if cluster_time_zone is not None:
+            pulumi.set(__self__, "cluster_time_zone", cluster_time_zone)
+        if database_engine is not None:
+            pulumi.set(__self__, "database_engine", database_engine)
+        if database_engine_version is not None:
+            pulumi.set(__self__, "database_engine_version", database_engine_version)
+        if date_created is not None:
+            pulumi.set(__self__, "date_created", date_created)
+        if dbname is not None:
+            pulumi.set(__self__, "dbname", dbname)
+        if host is not None:
+            pulumi.set(__self__, "host", host)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if latest_backup is not None:
+            pulumi.set(__self__, "latest_backup", latest_backup)
+        if maintenance_dow is not None:
+            pulumi.set(__self__, "maintenance_dow", maintenance_dow)
+        if maintenance_time is not None:
+            pulumi.set(__self__, "maintenance_time", maintenance_time)
+        if mysql_long_query_time is not None:
+            pulumi.set(__self__, "mysql_long_query_time", mysql_long_query_time)
+        if mysql_require_primary_key is not None:
+            pulumi.set(__self__, "mysql_require_primary_key", mysql_require_primary_key)
+        if mysql_slow_query_log is not None:
+            pulumi.set(__self__, "mysql_slow_query_log", mysql_slow_query_log)
+        if mysql_sql_modes is not None:
+            pulumi.set(__self__, "mysql_sql_modes", mysql_sql_modes)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if plan is not None:
+            pulumi.set(__self__, "plan", plan)
+        if plan_disk is not None:
+            pulumi.set(__self__, "plan_disk", plan_disk)
+        if plan_ram is not None:
+            pulumi.set(__self__, "plan_ram", plan_ram)
+        if plan_replicas is not None:
+            pulumi.set(__self__, "plan_replicas", plan_replicas)
+        if plan_vcpus is not None:
+            pulumi.set(__self__, "plan_vcpus", plan_vcpus)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if redis_eviction_policy is not None:
+            pulumi.set(__self__, "redis_eviction_policy", redis_eviction_policy)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if tag is not None:
+            pulumi.set(__self__, "tag", tag)
+        if trusted_ips is not None:
+            pulumi.set(__self__, "trusted_ips", trusted_ips)
+        if user is not None:
+            pulumi.set(__self__, "user", user)
+
+    @property
+    @pulumi.getter
+    def label(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "label")
+
+    @label.setter
+    def label(self, value: pulumi.Input[str]):
+        pulumi.set(self, "label", value)
+
+    @property
+    @pulumi.getter
+    def region(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "region")
+
+    @region.setter
+    def region(self, value: pulumi.Input[str]):
+        pulumi.set(self, "region", value)
+
+    @property
+    @pulumi.getter(name="clusterTimeZone")
+    def cluster_time_zone(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "cluster_time_zone")
+
+    @cluster_time_zone.setter
+    def cluster_time_zone(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "cluster_time_zone", value)
+
+    @property
+    @pulumi.getter(name="databaseEngine")
+    def database_engine(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "database_engine")
+
+    @database_engine.setter
+    def database_engine(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "database_engine", value)
+
+    @property
+    @pulumi.getter(name="databaseEngineVersion")
+    def database_engine_version(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "database_engine_version")
+
+    @database_engine_version.setter
+    def database_engine_version(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "database_engine_version", value)
+
+    @property
+    @pulumi.getter(name="dateCreated")
+    def date_created(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "date_created")
+
+    @date_created.setter
+    def date_created(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "date_created", value)
+
+    @property
+    @pulumi.getter
+    def dbname(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "dbname")
+
+    @dbname.setter
+    def dbname(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "dbname", value)
+
+    @property
+    @pulumi.getter
+    def host(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "host")
+
+    @host.setter
+    def host(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "host", value)
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "id")
+
+    @id.setter
+    def id(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "id", value)
+
+    @property
+    @pulumi.getter(name="latestBackup")
+    def latest_backup(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "latest_backup")
+
+    @latest_backup.setter
+    def latest_backup(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "latest_backup", value)
+
+    @property
+    @pulumi.getter(name="maintenanceDow")
+    def maintenance_dow(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "maintenance_dow")
+
+    @maintenance_dow.setter
+    def maintenance_dow(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "maintenance_dow", value)
+
+    @property
+    @pulumi.getter(name="maintenanceTime")
+    def maintenance_time(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "maintenance_time")
+
+    @maintenance_time.setter
+    def maintenance_time(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "maintenance_time", value)
+
+    @property
+    @pulumi.getter(name="mysqlLongQueryTime")
+    def mysql_long_query_time(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "mysql_long_query_time")
+
+    @mysql_long_query_time.setter
+    def mysql_long_query_time(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "mysql_long_query_time", value)
+
+    @property
+    @pulumi.getter(name="mysqlRequirePrimaryKey")
+    def mysql_require_primary_key(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "mysql_require_primary_key")
+
+    @mysql_require_primary_key.setter
+    def mysql_require_primary_key(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mysql_require_primary_key", value)
+
+    @property
+    @pulumi.getter(name="mysqlSlowQueryLog")
+    def mysql_slow_query_log(self) -> Optional[pulumi.Input[bool]]:
+        return pulumi.get(self, "mysql_slow_query_log")
+
+    @mysql_slow_query_log.setter
+    def mysql_slow_query_log(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "mysql_slow_query_log", value)
+
+    @property
+    @pulumi.getter(name="mysqlSqlModes")
+    def mysql_sql_modes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "mysql_sql_modes")
+
+    @mysql_sql_modes.setter
+    def mysql_sql_modes(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "mysql_sql_modes", value)
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "password")
+
+    @password.setter
+    def password(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "password", value)
+
+    @property
+    @pulumi.getter
+    def plan(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "plan")
+
+    @plan.setter
+    def plan(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "plan", value)
+
+    @property
+    @pulumi.getter(name="planDisk")
+    def plan_disk(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "plan_disk")
+
+    @plan_disk.setter
+    def plan_disk(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "plan_disk", value)
+
+    @property
+    @pulumi.getter(name="planRam")
+    def plan_ram(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "plan_ram")
+
+    @plan_ram.setter
+    def plan_ram(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "plan_ram", value)
+
+    @property
+    @pulumi.getter(name="planReplicas")
+    def plan_replicas(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "plan_replicas")
+
+    @plan_replicas.setter
+    def plan_replicas(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "plan_replicas", value)
+
+    @property
+    @pulumi.getter(name="planVcpus")
+    def plan_vcpus(self) -> Optional[pulumi.Input[int]]:
+        return pulumi.get(self, "plan_vcpus")
+
+    @plan_vcpus.setter
+    def plan_vcpus(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "plan_vcpus", value)
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "port")
+
+    @port.setter
+    def port(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "port", value)
+
+    @property
+    @pulumi.getter(name="redisEvictionPolicy")
+    def redis_eviction_policy(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redis_eviction_policy")
+
+    @redis_eviction_policy.setter
+    def redis_eviction_policy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redis_eviction_policy", value)
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "status")
+
+    @status.setter
+    def status(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "status", value)
+
+    @property
+    @pulumi.getter
+    def tag(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "tag")
+
+    @tag.setter
+    def tag(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "tag", value)
+
+    @property
+    @pulumi.getter(name="trustedIps")
+    def trusted_ips(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
+        return pulumi.get(self, "trusted_ips")
+
+    @trusted_ips.setter
+    def trusted_ips(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
+        pulumi.set(self, "trusted_ips", value)
+
+    @property
+    @pulumi.getter
+    def user(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "user")
+
+    @user.setter
+    def user(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "user", value)
+
+
+@pulumi.input_type
 class InstanceBackupsScheduleArgs:
     def __init__(__self__, *,
                  type: pulumi.Input[str],
                  dom: Optional[pulumi.Input[int]] = None,
                  dow: Optional[pulumi.Input[int]] = None,
                  hour: Optional[pulumi.Input[int]] = None):
         """
@@ -876,14 +1217,41 @@
         return pulumi.get(self, "values")
 
     @values.setter
     def values(self, value: Sequence[str]):
         pulumi.set(self, "values", value)
 
 
+@pulumi.input_type
+class GetDatabaseFilterArgs:
+    def __init__(__self__, *,
+                 name: str,
+                 values: Sequence[str]):
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "values", values)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @name.setter
+    def name(self, value: str):
+        pulumi.set(self, "name", value)
+
+    @property
+    @pulumi.getter
+    def values(self) -> Sequence[str]:
+        return pulumi.get(self, "values")
+
+    @values.setter
+    def values(self, value: Sequence[str]):
+        pulumi.set(self, "values", value)
+
+
 @pulumi.input_type
 class GetFirewallGroupFilterArgs:
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str]):
         """
         :param str name: Attribute name to filter with.
```

### Comparing `ediri_vultr-2.14.1/ediri_vultr/_utilities.py` & `ediri_vultr-2.15.0/ediri_vultr/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/bare_metal_server.py` & `ediri_vultr-2.15.0/ediri_vultr/bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/block_storage.py` & `ediri_vultr-2.15.0/ediri_vultr/block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/config/vars.py` & `ediri_vultr-2.15.0/ediri_vultr/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/dns_domain.py` & `ediri_vultr-2.15.0/ediri_vultr/dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/dns_record.py` & `ediri_vultr-2.15.0/ediri_vultr/dns_record.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/firewall_group.py` & `ediri_vultr-2.15.0/ediri_vultr/firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/firewall_rule.py` & `ediri_vultr-2.15.0/ediri_vultr/firewall_rule.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_account.py` & `ediri_vultr-2.15.0/ediri_vultr/get_account.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_application.py` & `ediri_vultr-2.15.0/ediri_vultr/get_application.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_backup.py` & `ediri_vultr-2.15.0/ediri_vultr/get_backup.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_plan.py` & `ediri_vultr-2.15.0/ediri_vultr/get_bare_metal_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_bare_metal_server.py` & `ediri_vultr-2.15.0/ediri_vultr/get_bare_metal_server.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_block_storage.py` & `ediri_vultr-2.15.0/ediri_vultr/get_block_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_dns_domain.py` & `ediri_vultr-2.15.0/ediri_vultr/get_dns_domain.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_firewall_group.py` & `ediri_vultr-2.15.0/ediri_vultr/get_firewall_group.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_instance.py` & `ediri_vultr-2.15.0/ediri_vultr/get_instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_instance_ipv4.py` & `ediri_vultr-2.15.0/ediri_vultr/get_instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_iso_private.py` & `ediri_vultr-2.15.0/ediri_vultr/get_iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_iso_public.py` & `ediri_vultr-2.15.0/ediri_vultr/get_iso_public.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_kubernetes.py` & `ediri_vultr-2.15.0/ediri_vultr/get_kubernetes.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_load_balancer.py` & `ediri_vultr-2.15.0/ediri_vultr/get_load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_object_storage.py` & `ediri_vultr-2.15.0/ediri_vultr/get_object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_object_storage_cluster.py` & `ediri_vultr-2.15.0/ediri_vultr/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_os.py` & `ediri_vultr-2.15.0/ediri_vultr/get_os.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_plan.py` & `ediri_vultr-2.15.0/ediri_vultr/get_plan.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_private_network.py` & `ediri_vultr-2.15.0/ediri_vultr/get_private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_region.py` & `ediri_vultr-2.15.0/ediri_vultr/get_region.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_reserved_ip.py` & `ediri_vultr-2.15.0/ediri_vultr/get_reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv4.py` & `ediri_vultr-2.15.0/ediri_vultr/get_reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_reverse_ipv6.py` & `ediri_vultr-2.15.0/ediri_vultr/get_reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_snapshot.py` & `ediri_vultr-2.15.0/ediri_vultr/get_snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_ssh_key.py` & `ediri_vultr-2.15.0/ediri_vultr/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_startup_script.py` & `ediri_vultr-2.15.0/ediri_vultr/get_startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_user.py` & `ediri_vultr-2.15.0/ediri_vultr/get_user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/get_vpc.py` & `ediri_vultr-2.15.0/ediri_vultr/get_vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/instance.py` & `ediri_vultr-2.15.0/ediri_vultr/instance.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/instance_ipv4.py` & `ediri_vultr-2.15.0/ediri_vultr/instance_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/iso_private.py` & `ediri_vultr-2.15.0/ediri_vultr/iso_private.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/kubernetes.py` & `ediri_vultr-2.15.0/ediri_vultr/kubernetes.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/kubernetes_node_pools.py` & `ediri_vultr-2.15.0/ediri_vultr/kubernetes_node_pools.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/load_balancer.py` & `ediri_vultr-2.15.0/ediri_vultr/load_balancer.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/object_storage.py` & `ediri_vultr-2.15.0/ediri_vultr/object_storage.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/outputs.py` & `ediri_vultr-2.15.0/ediri_vultr/outputs.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,26 +7,29 @@
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
 from . import outputs
 
 __all__ = [
+    'DatabaseReadReplica',
     'InstanceBackupsSchedule',
     'KubernetesNodePools',
     'KubernetesNodePoolsNode',
     'LoadBalancerFirewallRule',
     'LoadBalancerForwardingRule',
     'LoadBalancerHealthCheck',
     'LoadBalancerSsl',
     'GetApplicationFilterResult',
     'GetBackupFilterResult',
     'GetBareMetalPlanFilterResult',
     'GetBareMetalServerFilterResult',
     'GetBlockStorageFilterResult',
+    'GetDatabaseFilterResult',
+    'GetDatabaseReadReplicaResult',
     'GetFirewallGroupFilterResult',
     'GetInstanceFilterResult',
     'GetInstanceIpv4FilterResult',
     'GetIsoPrivateFilterResult',
     'GetIsoPublicFilterResult',
     'GetKubernetesFilterResult',
     'GetKubernetesNodePoolResult',
@@ -45,14 +48,290 @@
     'GetSshKeyFilterResult',
     'GetStartupScriptFilterResult',
     'GetUserFilterResult',
     'GetVpcFilterResult',
 ]
 
 @pulumi.output_type
+class DatabaseReadReplica(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "clusterTimeZone":
+            suggest = "cluster_time_zone"
+        elif key == "databaseEngine":
+            suggest = "database_engine"
+        elif key == "databaseEngineVersion":
+            suggest = "database_engine_version"
+        elif key == "dateCreated":
+            suggest = "date_created"
+        elif key == "latestBackup":
+            suggest = "latest_backup"
+        elif key == "maintenanceDow":
+            suggest = "maintenance_dow"
+        elif key == "maintenanceTime":
+            suggest = "maintenance_time"
+        elif key == "mysqlLongQueryTime":
+            suggest = "mysql_long_query_time"
+        elif key == "mysqlRequirePrimaryKey":
+            suggest = "mysql_require_primary_key"
+        elif key == "mysqlSlowQueryLog":
+            suggest = "mysql_slow_query_log"
+        elif key == "mysqlSqlModes":
+            suggest = "mysql_sql_modes"
+        elif key == "planDisk":
+            suggest = "plan_disk"
+        elif key == "planRam":
+            suggest = "plan_ram"
+        elif key == "planReplicas":
+            suggest = "plan_replicas"
+        elif key == "planVcpus":
+            suggest = "plan_vcpus"
+        elif key == "redisEvictionPolicy":
+            suggest = "redis_eviction_policy"
+        elif key == "trustedIps":
+            suggest = "trusted_ips"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in DatabaseReadReplica. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        DatabaseReadReplica.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        DatabaseReadReplica.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 label: str,
+                 region: str,
+                 cluster_time_zone: Optional[str] = None,
+                 database_engine: Optional[str] = None,
+                 database_engine_version: Optional[str] = None,
+                 date_created: Optional[str] = None,
+                 dbname: Optional[str] = None,
+                 host: Optional[str] = None,
+                 id: Optional[str] = None,
+                 latest_backup: Optional[str] = None,
+                 maintenance_dow: Optional[str] = None,
+                 maintenance_time: Optional[str] = None,
+                 mysql_long_query_time: Optional[int] = None,
+                 mysql_require_primary_key: Optional[bool] = None,
+                 mysql_slow_query_log: Optional[bool] = None,
+                 mysql_sql_modes: Optional[Sequence[str]] = None,
+                 password: Optional[str] = None,
+                 plan: Optional[str] = None,
+                 plan_disk: Optional[int] = None,
+                 plan_ram: Optional[int] = None,
+                 plan_replicas: Optional[int] = None,
+                 plan_vcpus: Optional[int] = None,
+                 port: Optional[str] = None,
+                 redis_eviction_policy: Optional[str] = None,
+                 status: Optional[str] = None,
+                 tag: Optional[str] = None,
+                 trusted_ips: Optional[Sequence[str]] = None,
+                 user: Optional[str] = None):
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "region", region)
+        if cluster_time_zone is not None:
+            pulumi.set(__self__, "cluster_time_zone", cluster_time_zone)
+        if database_engine is not None:
+            pulumi.set(__self__, "database_engine", database_engine)
+        if database_engine_version is not None:
+            pulumi.set(__self__, "database_engine_version", database_engine_version)
+        if date_created is not None:
+            pulumi.set(__self__, "date_created", date_created)
+        if dbname is not None:
+            pulumi.set(__self__, "dbname", dbname)
+        if host is not None:
+            pulumi.set(__self__, "host", host)
+        if id is not None:
+            pulumi.set(__self__, "id", id)
+        if latest_backup is not None:
+            pulumi.set(__self__, "latest_backup", latest_backup)
+        if maintenance_dow is not None:
+            pulumi.set(__self__, "maintenance_dow", maintenance_dow)
+        if maintenance_time is not None:
+            pulumi.set(__self__, "maintenance_time", maintenance_time)
+        if mysql_long_query_time is not None:
+            pulumi.set(__self__, "mysql_long_query_time", mysql_long_query_time)
+        if mysql_require_primary_key is not None:
+            pulumi.set(__self__, "mysql_require_primary_key", mysql_require_primary_key)
+        if mysql_slow_query_log is not None:
+            pulumi.set(__self__, "mysql_slow_query_log", mysql_slow_query_log)
+        if mysql_sql_modes is not None:
+            pulumi.set(__self__, "mysql_sql_modes", mysql_sql_modes)
+        if password is not None:
+            pulumi.set(__self__, "password", password)
+        if plan is not None:
+            pulumi.set(__self__, "plan", plan)
+        if plan_disk is not None:
+            pulumi.set(__self__, "plan_disk", plan_disk)
+        if plan_ram is not None:
+            pulumi.set(__self__, "plan_ram", plan_ram)
+        if plan_replicas is not None:
+            pulumi.set(__self__, "plan_replicas", plan_replicas)
+        if plan_vcpus is not None:
+            pulumi.set(__self__, "plan_vcpus", plan_vcpus)
+        if port is not None:
+            pulumi.set(__self__, "port", port)
+        if redis_eviction_policy is not None:
+            pulumi.set(__self__, "redis_eviction_policy", redis_eviction_policy)
+        if status is not None:
+            pulumi.set(__self__, "status", status)
+        if tag is not None:
+            pulumi.set(__self__, "tag", tag)
+        if trusted_ips is not None:
+            pulumi.set(__self__, "trusted_ips", trusted_ips)
+        if user is not None:
+            pulumi.set(__self__, "user", user)
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter(name="clusterTimeZone")
+    def cluster_time_zone(self) -> Optional[str]:
+        return pulumi.get(self, "cluster_time_zone")
+
+    @property
+    @pulumi.getter(name="databaseEngine")
+    def database_engine(self) -> Optional[str]:
+        return pulumi.get(self, "database_engine")
+
+    @property
+    @pulumi.getter(name="databaseEngineVersion")
+    def database_engine_version(self) -> Optional[str]:
+        return pulumi.get(self, "database_engine_version")
+
+    @property
+    @pulumi.getter(name="dateCreated")
+    def date_created(self) -> Optional[str]:
+        return pulumi.get(self, "date_created")
+
+    @property
+    @pulumi.getter
+    def dbname(self) -> Optional[str]:
+        return pulumi.get(self, "dbname")
+
+    @property
+    @pulumi.getter
+    def host(self) -> Optional[str]:
+        return pulumi.get(self, "host")
+
+    @property
+    @pulumi.getter
+    def id(self) -> Optional[str]:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter(name="latestBackup")
+    def latest_backup(self) -> Optional[str]:
+        return pulumi.get(self, "latest_backup")
+
+    @property
+    @pulumi.getter(name="maintenanceDow")
+    def maintenance_dow(self) -> Optional[str]:
+        return pulumi.get(self, "maintenance_dow")
+
+    @property
+    @pulumi.getter(name="maintenanceTime")
+    def maintenance_time(self) -> Optional[str]:
+        return pulumi.get(self, "maintenance_time")
+
+    @property
+    @pulumi.getter(name="mysqlLongQueryTime")
+    def mysql_long_query_time(self) -> Optional[int]:
+        return pulumi.get(self, "mysql_long_query_time")
+
+    @property
+    @pulumi.getter(name="mysqlRequirePrimaryKey")
+    def mysql_require_primary_key(self) -> Optional[bool]:
+        return pulumi.get(self, "mysql_require_primary_key")
+
+    @property
+    @pulumi.getter(name="mysqlSlowQueryLog")
+    def mysql_slow_query_log(self) -> Optional[bool]:
+        return pulumi.get(self, "mysql_slow_query_log")
+
+    @property
+    @pulumi.getter(name="mysqlSqlModes")
+    def mysql_sql_modes(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "mysql_sql_modes")
+
+    @property
+    @pulumi.getter
+    def password(self) -> Optional[str]:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def plan(self) -> Optional[str]:
+        return pulumi.get(self, "plan")
+
+    @property
+    @pulumi.getter(name="planDisk")
+    def plan_disk(self) -> Optional[int]:
+        return pulumi.get(self, "plan_disk")
+
+    @property
+    @pulumi.getter(name="planRam")
+    def plan_ram(self) -> Optional[int]:
+        return pulumi.get(self, "plan_ram")
+
+    @property
+    @pulumi.getter(name="planReplicas")
+    def plan_replicas(self) -> Optional[int]:
+        return pulumi.get(self, "plan_replicas")
+
+    @property
+    @pulumi.getter(name="planVcpus")
+    def plan_vcpus(self) -> Optional[int]:
+        return pulumi.get(self, "plan_vcpus")
+
+    @property
+    @pulumi.getter
+    def port(self) -> Optional[str]:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="redisEvictionPolicy")
+    def redis_eviction_policy(self) -> Optional[str]:
+        return pulumi.get(self, "redis_eviction_policy")
+
+    @property
+    @pulumi.getter
+    def status(self) -> Optional[str]:
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
+    def tag(self) -> Optional[str]:
+        return pulumi.get(self, "tag")
+
+    @property
+    @pulumi.getter(name="trustedIps")
+    def trusted_ips(self) -> Optional[Sequence[str]]:
+        return pulumi.get(self, "trusted_ips")
+
+    @property
+    @pulumi.getter
+    def user(self) -> Optional[str]:
+        return pulumi.get(self, "user")
+
+
+@pulumi.output_type
 class InstanceBackupsSchedule(dict):
     def __init__(__self__, *,
                  type: str,
                  dom: Optional[int] = None,
                  dow: Optional[int] = None,
                  hour: Optional[int] = None):
         """
@@ -810,14 +1089,234 @@
         """
         One or more values filter with.
         """
         return pulumi.get(self, "values")
 
 
 @pulumi.output_type
+class GetDatabaseFilterResult(dict):
+    def __init__(__self__, *,
+                 name: str,
+                 values: Sequence[str]):
+        pulumi.set(__self__, "name", name)
+        pulumi.set(__self__, "values", values)
+
+    @property
+    @pulumi.getter
+    def name(self) -> str:
+        return pulumi.get(self, "name")
+
+    @property
+    @pulumi.getter
+    def values(self) -> Sequence[str]:
+        return pulumi.get(self, "values")
+
+
+@pulumi.output_type
+class GetDatabaseReadReplicaResult(dict):
+    def __init__(__self__, *,
+                 cluster_time_zone: str,
+                 database_engine: str,
+                 database_engine_version: str,
+                 date_created: str,
+                 dbname: str,
+                 host: str,
+                 id: str,
+                 label: str,
+                 latest_backup: str,
+                 maintenance_dow: str,
+                 maintenance_time: str,
+                 mysql_long_query_time: int,
+                 mysql_require_primary_key: bool,
+                 mysql_slow_query_log: bool,
+                 mysql_sql_modes: Sequence[str],
+                 password: str,
+                 plan: str,
+                 plan_disk: int,
+                 plan_ram: int,
+                 plan_replicas: int,
+                 plan_vcpus: int,
+                 port: str,
+                 redis_eviction_policy: str,
+                 region: str,
+                 status: str,
+                 tag: str,
+                 trusted_ips: Sequence[str],
+                 user: str):
+        pulumi.set(__self__, "cluster_time_zone", cluster_time_zone)
+        pulumi.set(__self__, "database_engine", database_engine)
+        pulumi.set(__self__, "database_engine_version", database_engine_version)
+        pulumi.set(__self__, "date_created", date_created)
+        pulumi.set(__self__, "dbname", dbname)
+        pulumi.set(__self__, "host", host)
+        pulumi.set(__self__, "id", id)
+        pulumi.set(__self__, "label", label)
+        pulumi.set(__self__, "latest_backup", latest_backup)
+        pulumi.set(__self__, "maintenance_dow", maintenance_dow)
+        pulumi.set(__self__, "maintenance_time", maintenance_time)
+        pulumi.set(__self__, "mysql_long_query_time", mysql_long_query_time)
+        pulumi.set(__self__, "mysql_require_primary_key", mysql_require_primary_key)
+        pulumi.set(__self__, "mysql_slow_query_log", mysql_slow_query_log)
+        pulumi.set(__self__, "mysql_sql_modes", mysql_sql_modes)
+        pulumi.set(__self__, "password", password)
+        pulumi.set(__self__, "plan", plan)
+        pulumi.set(__self__, "plan_disk", plan_disk)
+        pulumi.set(__self__, "plan_ram", plan_ram)
+        pulumi.set(__self__, "plan_replicas", plan_replicas)
+        pulumi.set(__self__, "plan_vcpus", plan_vcpus)
+        pulumi.set(__self__, "port", port)
+        pulumi.set(__self__, "redis_eviction_policy", redis_eviction_policy)
+        pulumi.set(__self__, "region", region)
+        pulumi.set(__self__, "status", status)
+        pulumi.set(__self__, "tag", tag)
+        pulumi.set(__self__, "trusted_ips", trusted_ips)
+        pulumi.set(__self__, "user", user)
+
+    @property
+    @pulumi.getter(name="clusterTimeZone")
+    def cluster_time_zone(self) -> str:
+        return pulumi.get(self, "cluster_time_zone")
+
+    @property
+    @pulumi.getter(name="databaseEngine")
+    def database_engine(self) -> str:
+        return pulumi.get(self, "database_engine")
+
+    @property
+    @pulumi.getter(name="databaseEngineVersion")
+    def database_engine_version(self) -> str:
+        return pulumi.get(self, "database_engine_version")
+
+    @property
+    @pulumi.getter(name="dateCreated")
+    def date_created(self) -> str:
+        return pulumi.get(self, "date_created")
+
+    @property
+    @pulumi.getter
+    def dbname(self) -> str:
+        return pulumi.get(self, "dbname")
+
+    @property
+    @pulumi.getter
+    def host(self) -> str:
+        return pulumi.get(self, "host")
+
+    @property
+    @pulumi.getter
+    def id(self) -> str:
+        return pulumi.get(self, "id")
+
+    @property
+    @pulumi.getter
+    def label(self) -> str:
+        return pulumi.get(self, "label")
+
+    @property
+    @pulumi.getter(name="latestBackup")
+    def latest_backup(self) -> str:
+        return pulumi.get(self, "latest_backup")
+
+    @property
+    @pulumi.getter(name="maintenanceDow")
+    def maintenance_dow(self) -> str:
+        return pulumi.get(self, "maintenance_dow")
+
+    @property
+    @pulumi.getter(name="maintenanceTime")
+    def maintenance_time(self) -> str:
+        return pulumi.get(self, "maintenance_time")
+
+    @property
+    @pulumi.getter(name="mysqlLongQueryTime")
+    def mysql_long_query_time(self) -> int:
+        return pulumi.get(self, "mysql_long_query_time")
+
+    @property
+    @pulumi.getter(name="mysqlRequirePrimaryKey")
+    def mysql_require_primary_key(self) -> bool:
+        return pulumi.get(self, "mysql_require_primary_key")
+
+    @property
+    @pulumi.getter(name="mysqlSlowQueryLog")
+    def mysql_slow_query_log(self) -> bool:
+        return pulumi.get(self, "mysql_slow_query_log")
+
+    @property
+    @pulumi.getter(name="mysqlSqlModes")
+    def mysql_sql_modes(self) -> Sequence[str]:
+        return pulumi.get(self, "mysql_sql_modes")
+
+    @property
+    @pulumi.getter
+    def password(self) -> str:
+        return pulumi.get(self, "password")
+
+    @property
+    @pulumi.getter
+    def plan(self) -> str:
+        return pulumi.get(self, "plan")
+
+    @property
+    @pulumi.getter(name="planDisk")
+    def plan_disk(self) -> int:
+        return pulumi.get(self, "plan_disk")
+
+    @property
+    @pulumi.getter(name="planRam")
+    def plan_ram(self) -> int:
+        return pulumi.get(self, "plan_ram")
+
+    @property
+    @pulumi.getter(name="planReplicas")
+    def plan_replicas(self) -> int:
+        return pulumi.get(self, "plan_replicas")
+
+    @property
+    @pulumi.getter(name="planVcpus")
+    def plan_vcpus(self) -> int:
+        return pulumi.get(self, "plan_vcpus")
+
+    @property
+    @pulumi.getter
+    def port(self) -> str:
+        return pulumi.get(self, "port")
+
+    @property
+    @pulumi.getter(name="redisEvictionPolicy")
+    def redis_eviction_policy(self) -> str:
+        return pulumi.get(self, "redis_eviction_policy")
+
+    @property
+    @pulumi.getter
+    def region(self) -> str:
+        return pulumi.get(self, "region")
+
+    @property
+    @pulumi.getter
+    def status(self) -> str:
+        return pulumi.get(self, "status")
+
+    @property
+    @pulumi.getter
+    def tag(self) -> str:
+        return pulumi.get(self, "tag")
+
+    @property
+    @pulumi.getter(name="trustedIps")
+    def trusted_ips(self) -> Sequence[str]:
+        return pulumi.get(self, "trusted_ips")
+
+    @property
+    @pulumi.getter
+    def user(self) -> str:
+        return pulumi.get(self, "user")
+
+
+@pulumi.output_type
 class GetFirewallGroupFilterResult(dict):
     def __init__(__self__, *,
                  name: str,
                  values: Sequence[str]):
         """
         :param str name: Attribute name to filter with.
         :param Sequence[str] values: One or more values filter with.
```

### Comparing `ediri_vultr-2.14.1/ediri_vultr/private_network.py` & `ediri_vultr-2.15.0/ediri_vultr/private_network.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/provider.py` & `ediri_vultr-2.15.0/ediri_vultr/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/reserved_ip.py` & `ediri_vultr-2.15.0/ediri_vultr/reserved_ip.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/reverse_ipv4.py` & `ediri_vultr-2.15.0/ediri_vultr/reverse_ipv4.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/reverse_ipv6.py` & `ediri_vultr-2.15.0/ediri_vultr/reverse_ipv6.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/snapshot.py` & `ediri_vultr-2.15.0/ediri_vultr/snapshot.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/snapshot_from_url.py` & `ediri_vultr-2.15.0/ediri_vultr/snapshot_from_url.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/ssh_key.py` & `ediri_vultr-2.15.0/ediri_vultr/ssh_key.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/startup_script.py` & `ediri_vultr-2.15.0/ediri_vultr/startup_script.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/user.py` & `ediri_vultr-2.15.0/ediri_vultr/user.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr/vpc.py` & `ediri_vultr-2.15.0/ediri_vultr/vpc.py`

 * *Files identical despite different names*

### Comparing `ediri_vultr-2.14.1/ediri_vultr.egg-info/PKG-INFO` & `ediri_vultr-2.15.0/ediri_vultr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ediri-vultr
-Version: 2.14.1
+Version: 2.15.0
 Summary: A Pulumi package for creating and managing Vultr cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-vultr
 Keywords: pulumi vultr category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `ediri_vultr-2.14.1/ediri_vultr.egg-info/SOURCES.txt` & `ediri_vultr-2.15.0/ediri_vultr.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 README.md
 setup.py
 ediri_vultr/__init__.py
 ediri_vultr/_inputs.py
 ediri_vultr/_utilities.py
 ediri_vultr/bare_metal_server.py
 ediri_vultr/block_storage.py
+ediri_vultr/database.py
+ediri_vultr/database_connection_pool.py
+ediri_vultr/database_db.py
+ediri_vultr/database_replica.py
+ediri_vultr/database_user.py
 ediri_vultr/dns_domain.py
 ediri_vultr/dns_record.py
 ediri_vultr/firewall_group.py
 ediri_vultr/firewall_rule.py
 ediri_vultr/get_account.py
 ediri_vultr/get_application.py
 ediri_vultr/get_backup.py
 ediri_vultr/get_bare_metal_plan.py
 ediri_vultr/get_bare_metal_server.py
 ediri_vultr/get_block_storage.py
+ediri_vultr/get_database.py
 ediri_vultr/get_dns_domain.py
 ediri_vultr/get_firewall_group.py
 ediri_vultr/get_instance.py
 ediri_vultr/get_instance_ipv4.py
 ediri_vultr/get_iso_private.py
 ediri_vultr/get_iso_public.py
 ediri_vultr/get_kubernetes.py
```

### Comparing `ediri_vultr-2.14.1/setup.py` & `ediri_vultr-2.15.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "2.14.1"
-PLUGIN_VERSION = "2.14.1"
+VERSION = "2.15.0"
+PLUGIN_VERSION = "2.15.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'vultr', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-vultr'])
         except OSError as error:
```

