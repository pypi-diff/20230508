# Comparing `tmp/nanomock-0.0.8.tar.gz` & `tmp/nanomock-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanomock-0.0.8.tar", last modified: Sat May  6 19:55:19 2023, max compression
+gzip compressed data, was "nanomock-0.0.9.tar", last modified: Sun May  7 20:58:50 2023, max compression
```

## Comparing `nanomock-0.0.8.tar` & `nanomock-0.0.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.431336 nanomock-0.0.8/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-06 19:55:19.431336 nanomock-0.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/
--rw-r--r--   0 root         (0) root         (0)       22 2023-05-06 15:00:39.000000 nanomock-0.0.8/nanomock/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/docker/
--rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.8/nanomock/docker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.8/nanomock/docker/autoheal.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.8/nanomock/docker/interface.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.8/nanomock/docker/linux.py
--rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.8/nanomock/docker/macos.py
--rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.8/nanomock/docker/mixin.py
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.8/nanomock/docker/windows.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.8/nanomock/internal/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.8/nanomock/internal/data/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.8/nanomock/internal/data/services/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/custom_Dockerfile
--rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/default_config-node.toml
--rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/default_config-node_voting-disabled.toml
--rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/default_config-rpc.toml
--rw-r--r--   0 root         (0) root         (0)     1822 2023-05-04 22:06:12.000000 nanomock-0.0.8/nanomock/internal/data/services/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/nanolooker/
--rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/nanolooker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.8/nanomock/internal/data/services/nanolooker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.8/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/nanomonitor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.8/nanomock/internal/data/services/nanomonitor/__init__.py
--rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/nanomonitor/default_config.php
--rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.8/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/nanoticker/
--rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/nanoticker/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.8/nanomock/internal/data/services/nanoticker/__init__.py
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.8/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/
--rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/__init__.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/promexporter/
--rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.423336 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
--rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
--rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
--rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/promexporter/prometheus.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/internal/data/services/tcpdump/
--rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/tcpdump/Dockerfile
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.8/nanomock/internal/data/services/tcpdump/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.8/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
--rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.8/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.8/nanomock/internal/dependency_checker.py
--rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.8/nanomock/internal/feature_toggle.py
--rw-r--r--   0 root         (0) root         (0)    26984 2023-05-02 13:32:24.000000 nanomock-0.0.8/nanomock/internal/nl_block_tools.py
--rw-r--r--   0 root         (0) root         (0)     7743 2023-05-06 14:53:34.000000 nanomock-0.0.8/nanomock/internal/nl_initialise.py
--rw-r--r--   0 root         (0) root         (0)     5695 2023-05-05 21:23:17.000000 nanomock-0.0.8/nanomock/internal/utils.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-05-05 13:17:03.000000 nanomock-0.0.8/nanomock/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock/modules/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.8/nanomock/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.8/nanomock/modules/nl_nanolib.py
--rw-rw-r--   0 root         (0) root         (0)    44037 2023-05-06 19:47:19.000000 nanomock-0.0.8/nanomock/modules/nl_parse_config.py
--rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.8/nanomock/modules/nl_rpc.py
--rw-rw-r--   0 root         (0) root         (0)    18011 2023-05-06 19:35:05.000000 nanomock-0.0.8/nanomock/nanomock_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.431336 nanomock-0.0.8/nanomock/os_operations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.8/nanomock/os_operations/__init__.py
--rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.8/nanomock/os_operations/interface.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.8/nanomock/os_operations/linux.py
--rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.8/nanomock/os_operations/macos.py
--rw-r--r--   0 root         (0) root         (0)      825 2023-05-04 19:05:01.000000 nanomock-0.0.8/nanomock/os_operations/mixin.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 19:55:19.427336 nanomock-0.0.8/nanomock.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2959 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2989 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       48 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       54 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-05-06 19:55:19.000000 nanomock-0.0.8/nanomock.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 19:55:19.431336 nanomock-0.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      784 2023-05-06 19:55:07.000000 nanomock-0.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-02 13:35:20.000000 nanomock-0.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-07 20:58:50.376045 nanomock-0.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2743 2023-05-02 22:46:21.000000 nanomock-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.372045 nanomock-0.0.9/nanomock/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-05-06 19:55:19.000000 nanomock-0.0.9/nanomock/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/docker/
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-05-04 20:29:22.000000 nanomock-0.0.9/nanomock/docker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-05-04 18:55:41.000000 nanomock-0.0.9/nanomock/docker/autoheal.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-05-04 20:35:54.000000 nanomock-0.0.9/nanomock/docker/interface.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-05-04 20:29:56.000000 nanomock-0.0.9/nanomock/docker/linux.py
+-rw-r--r--   0 root         (0) root         (0)      389 2023-05-04 20:30:32.000000 nanomock-0.0.9/nanomock/docker/macos.py
+-rw-r--r--   0 root         (0) root         (0)     3170 2023-05-04 18:48:04.000000 nanomock-0.0.9/nanomock/docker/mixin.py
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-04 20:30:11.000000 nanomock-0.0.9/nanomock/docker/windows.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 11:22:58.000000 nanomock-0.0.9/nanomock/internal/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:05.000000 nanomock-0.0.9/nanomock/internal/data/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-01 19:50:25.000000 nanomock-0.0.9/nanomock/internal/data/services/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      432 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/custom_Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/default_config-node.toml
+-rw-r--r--   0 root         (0) root         (0)      298 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/default_config-node_voting-disabled.toml
+-rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/default_config-rpc.toml
+-rw-r--r--   0 root         (0) root         (0)     1822 2023-05-04 22:06:12.000000 nanomock-0.0.9/nanomock/internal/data/services/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/nanolooker/
+-rw-r--r--   0 root         (0) root         (0)      960 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/nanolooker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:55.000000 nanomock-0.0.9/nanomock/internal/data/services/nanolooker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1211 2023-05-03 12:43:38.000000 nanomock-0.0.9/nanomock/internal/data/services/nanolooker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/nanomonitor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:41:59.000000 nanomock-0.0.9/nanomock/internal/data/services/nanomonitor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      659 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/nanomonitor/default_config.php
+-rw-r--r--   0 root         (0) root         (0)      354 2023-05-03 09:06:45.000000 nanomock-0.0.9/nanomock/internal/data/services/nanomonitor/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/nanoticker/
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/nanoticker/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:02.000000 nanomock-0.0.9/nanomock/internal/data/services/nanoticker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      466 2023-05-03 12:43:51.000000 nanomock-0.0.9/nanomock/internal/data/services/nanoticker/default_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/
+-rw-r--r--   0 root         (0) root         (0)      768 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:05.000000 nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-05-03 12:43:54.000000 nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      325 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/environment.prod.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/promexporter/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:14.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1555 2023-05-04 19:53:21.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      420 2023-05-04 19:54:54.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/default_exporter_docker-compose.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.372045 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.372045 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/
+-rw-r--r--   0 root         (0) root         (0)    78536 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json
+-rw-r--r--   0 root         (0) root         (0)      132 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml
+-rw-r--r--   0 root         (0) root         (0)      515 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/promexporter/prometheus.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/internal/data/services/tcpdump/
+-rw-r--r--   0 root         (0) root         (0)      119 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/tcpdump/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-02 08:42:10.000000 nanomock-0.0.9/nanomock/internal/data/services/tcpdump/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      221 2023-05-03 21:35:04.000000 nanomock-0.0.9/nanomock/internal/data/services/tcpdump/default_docker-compose.yml
+-rw-r--r--   0 root         (0) root         (0)      685 2023-04-27 20:34:19.000000 nanomock-0.0.9/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-01 12:06:33.000000 nanomock-0.0.9/nanomock/internal/dependency_checker.py
+-rw-rw-r--   0 root         (0) root         (0)      806 2023-05-03 21:35:04.000000 nanomock-0.0.9/nanomock/internal/feature_toggle.py
+-rw-r--r--   0 root         (0) root         (0)    26958 2023-05-07 06:48:09.000000 nanomock-0.0.9/nanomock/internal/nl_block_tools.py
+-rw-r--r--   0 root         (0) root         (0)     7743 2023-05-06 14:53:34.000000 nanomock-0.0.9/nanomock/internal/nl_initialise.py
+-rw-r--r--   0 root         (0) root         (0)     5730 2023-05-07 20:55:43.000000 nanomock-0.0.9/nanomock/internal/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-05-05 13:17:03.000000 nanomock-0.0.9/nanomock/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-27 15:36:50.000000 nanomock-0.0.9/nanomock/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2415 2023-04-27 18:47:46.000000 nanomock-0.0.9/nanomock/modules/nl_nanolib.py
+-rw-rw-r--   0 root         (0) root         (0)    43790 2023-05-07 06:48:15.000000 nanomock-0.0.9/nanomock/modules/nl_parse_config.py
+-rw-r--r--   0 root         (0) root         (0)    27670 2023-05-02 13:32:25.000000 nanomock-0.0.9/nanomock/modules/nl_rpc.py
+-rw-rw-r--   0 root         (0) root         (0)    18106 2023-05-07 20:55:59.000000 nanomock-0.0.9/nanomock/nanomock_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.376045 nanomock-0.0.9/nanomock/os_operations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-04 18:54:54.000000 nanomock-0.0.9/nanomock/os_operations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      250 2023-05-04 18:54:54.000000 nanomock-0.0.9/nanomock/os_operations/interface.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.9/nanomock/os_operations/linux.py
+-rw-r--r--   0 root         (0) root         (0)      159 2023-05-04 18:54:54.000000 nanomock-0.0.9/nanomock/os_operations/macos.py
+-rw-r--r--   0 root         (0) root         (0)      819 2023-05-07 20:24:10.000000 nanomock-0.0.9/nanomock/os_operations/mixin.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-07 20:58:50.372045 nanomock-0.0.9/nanomock.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2959 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2989 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       54 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-07 20:58:50.000000 nanomock-0.0.9/nanomock.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-07 20:58:50.376045 nanomock-0.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      784 2023-05-06 20:17:29.000000 nanomock-0.0.9/setup.py
```

### Comparing `nanomock-0.0.8/PKG-INFO` & `nanomock-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.8/README.md` & `nanomock-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/docker/__init__.py` & `nanomock-0.0.9/nanomock/docker/__init__.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/docker/autoheal.py` & `nanomock-0.0.9/nanomock/docker/autoheal.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/docker/interface.py` & `nanomock-0.0.9/nanomock/docker/interface.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/docker/mixin.py` & `nanomock-0.0.9/nanomock/docker/mixin.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/default_docker-compose.yml` & `nanomock-0.0.9/nanomock/internal/data/services/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/nanolooker/Dockerfile` & `nanomock-0.0.9/nanomock/internal/data/services/nanolooker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/nanolooker/default_docker-compose.yml` & `nanomock-0.0.9/nanomock/internal/data/services/nanolooker/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/nanomonitor/default_config.php` & `nanomock-0.0.9/nanomock/internal/data/services/nanomonitor/default_config.php`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/nanoticker/Dockerfile` & `nanomock-0.0.9/nanomock/internal/data/services/nanoticker/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/nanovotevisu/Dockerfile` & `nanomock-0.0.9/nanomock/internal/data/services/nanovotevisu/Dockerfile`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/promexporter/default_docker-compose.yml` & `nanomock-0.0.9/nanomock/internal/data/services/promexporter/default_docker-compose.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json` & `nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/dashboards/dashboard.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml` & `nanomock-0.0.9/nanomock/internal/data/services/promexporter/grafana/provisioning/datasources/datasource.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/promexporter/prometheus.yml` & `nanomock-0.0.9/nanomock/internal/data/services/promexporter/prometheus.yml`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json` & `nanomock-0.0.9/nanomock/internal/data/services/tcpdump/tcp_analyzer_config.example.json`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/dependency_checker.py` & `nanomock-0.0.9/nanomock/internal/dependency_checker.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/feature_toggle.py` & `nanomock-0.0.9/nanomock/internal/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/nl_block_tools.py` & `nanomock-0.0.9/nanomock/internal/nl_block_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -575,16 +575,16 @@
                 bc["cemented"], bc["count"]) for bc in nodes_block_count
         ]
         return '\n' + '\n'.join(report)
 
 
 class BlockReadWrite():
 
-    def __init__(self, nl_conf_path):
-        self.conf_rw = ConfigReadWrite(nl_conf_path)
+    def __init__(self):
+        self.conf_rw = ConfigReadWrite()
 
     def read_blocks_from_disk(self,
                               path,
                               seeds=False,
                               hashes=False,
                               blocks=False):
         res = self.conf_rw.read_json(path)
```

### Comparing `nanomock-0.0.8/nanomock/internal/nl_initialise.py` & `nanomock-0.0.9/nanomock/internal/nl_initialise.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/internal/utils.py` & `nanomock-0.0.9/nanomock/internal/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,14 +63,15 @@
             value, log_message = result
             logger.success(log_message)
             return value
         elif result is None:
             logger.success(func.__name__)
             return None
         else:
+            logger.success(result)
             return result
 
     return wrapper
 
 
 def is_packaged_version():
     is_packaged = None
```

### Comparing `nanomock-0.0.8/nanomock/main.py` & `nanomock-0.0.9/nanomock/main.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/modules/nl_nanolib.py` & `nanomock-0.0.9/nanomock/modules/nl_nanolib.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/modules/nl_parse_config.py` & `nanomock-0.0.9/nanomock/modules/nl_parse_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,20 +23,14 @@
 
 def str2bool(v):
     return str(v).lower() in ("yes", "true", "t", "1")
 
 
 class ConfigReadWrite:
 
-    def __init__(self, config_path, logger=None):
-        if logger is None:
-            self.logger = NanoLocalLogger.get_logger(__name__)
-        if not os.path.exists(config_path):
-            raise FileExistsError(config_path)
-
     @read_from_package_if_needed
     def read_json(self, path, is_packaged=False):
         with open(path, "r") as f:
             return json.load(f)
 
     @read_from_package_if_needed
     def read_file(self, path, is_packaged=False):
@@ -46,15 +40,15 @@
     @read_from_package_if_needed
     def read_toml(self, path, is_packaged=False):
         try:
             with open(path, "rb") as f:
                 toml_dict = tomli.load(f)
                 return toml_dict
         except tomli.TOMLDecodeError as e:
-            self.logger.error("Invalid config file! \n {}".format(str(e)))
+            raise FileExistsError("Invalid config file! \n {}".format(str(e)))
 
     @read_from_package_if_needed
     def read_yaml(self, path, is_packaged=False):
         with open(path, 'r') as f:
             return yaml.safe_load(f)
 
     def write_json(self, path, json_dict):
@@ -90,15 +84,15 @@
     preconfigured_peers = []
 
     def __init__(self, app_dir, config_file, logger=None):
         self.logger = logger or NanoLocalLogger.get_logger(__name__)
 
         self.enabled_services = []
         self._set_path_variables(app_dir, config_file)
-        self.conf_rw = ConfigReadWrite(self.nl_config_path)
+        self.conf_rw = ConfigReadWrite()
         self.nano_lib = NanoLibTools()
         self.config_dict = self.conf_rw.read_toml(self.nl_config_path)
         self.compose_dict = self.conf_rw.read_yaml(self.default_compose_path,
                                                    is_packaged=True)
         self.__config_dict_add_genesis_to_nodes()
         self.__config_dict_set_node_variables()  #modifies config_dict
         self.__config_dict_set_default_values()  #modifies config_dict
```

### Comparing `nanomock-0.0.8/nanomock/modules/nl_rpc.py` & `nanomock-0.0.9/nanomock/modules/nl_rpc.py`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/nanomock/nanomock_manager.py` & `nanomock-0.0.9/nanomock/nanomock_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import os
-import re
-import subprocess
+from pathlib import Path
 import logging
 from typing import List, Optional
 from .internal.dependency_checker import DependencyChecker
 from .modules.nl_parse_config import ConfigParser, ConfigReadWrite
 from .internal.nl_initialise import InitialBlocks
 from .docker import create_docker_interface
 from .modules.nl_rpc import NanoRpc
 from .internal.utils import log_on_success, NanoLocalLogger, shutil_rmtree, extract_packaged_services_to_disk, subprocess_run_capture_output
 from typing import List, Dict, Optional, Tuple, Union
 import concurrent.futures
 from math import floor
-import yaml
 import json
 import time
 import inspect
 
 logger = NanoLocalLogger.get_logger(__name__)
 
 
 class NanoLocalManager:
 
     def __init__(self, dir_path, project_name, config_file="nl_config.toml"):
         self.command_mapping = self._initialize_command_mapping()
         self.conf_p = ConfigParser(dir_path,
                                    config_file=config_file,
                                    logger=logger)
-        self.conf_rw = ConfigReadWrite(dir_path)
+        self.conf_rw = ConfigReadWrite()
         self.dependency_checker = DependencyChecker()
         self.dependency_checker.check_dependencies()
 
         self.dir_path = dir_path
         self.nano_nodes_path = self.conf_p.nano_nodes_path
         self.compose_yml_path = self.conf_p.compose_out_path
         self.compose_env_path = os.path.join(self.nano_nodes_path,
@@ -283,15 +281,14 @@
         online_count = len(online_containers)
         if online_count == total_nodes:
             return f"All {online_count} containers online"
         else:
             return f"{online_count}/{total_nodes} containers online"
 
     def conf_edit(self, payload):
-        print(payload)
         self.conf_p.modify_nanolocal_config(payload["path"], payload["value"])
         return True
 
     @log_on_success
     def network_status(self, nodes_name: Optional[List[str]] = None) -> str:
         if nodes_name == []:
             return ""
@@ -311,24 +308,23 @@
     def create_docker_compose_file(self):
         extract_packaged_services_to_disk(self.nano_nodes_path)
         self._prepare_nodes()
         self._generate_docker_compose_env_file()
         self._generate_docker_compose_yml_file()
         logger.success(
             f"Docker Compose file created at {self.compose_yml_path}")
-        return "\n".join(self.conf_p.get_enabled_services())
+        return None, "\n".join(self.conf_p.get_enabled_services())
 
     def _validator_rpc(self, nodes=None, payload=None):
         if not payload:
             raise ValueError(
                 "The --payload argument is required for the 'rpc' command.")
         return nodes, payload
 
     def _validator_conf_edit(self, nodes=None, payload=None):
-        print("_validator_conf_edit", payload)
         if payload is None:
             raise ValueError(
                 "payload must be provided '{\"path\" : ... , \"value\": ...}'")
         if "path" not in payload:
             raise ValueError("key \"path\" must be provided")
         if "value" not in payload:
             raise ValueError("key \"value\" must be provided")
@@ -342,15 +338,15 @@
             nodes = self.conf_p.get_nodes_name()
 
         for node in nodes:
             node_rpc = NanoRpc(self.conf_p.get_node_rpc(node))
             response = node_rpc.post_with_auth(payload)
             responses.append(response)
 
-        return json.dumps(responses, indent=2)
+        return None, json.dumps(responses, indent=2)
 
     @log_on_success
     def init_wallets(self):
         #self.start_nodes('all')  #fixes a bug on mac m1
         init_blocks = InitialBlocks(self.conf_p,
                                     self.conf_p.get_nodes_rpc()[0])
         for node_name in self.conf_p.get_nodes_name():
@@ -361,31 +357,38 @@
                     self.conf_p.get_genesis_node_name(),
                     private_key=self.conf_p.config_dict["genesis_key"])
             else:
                 init_blocks.create_node_wallet(
                     self.conf_p.get_node_config(node_name)["rpc_url"],
                     node_name,
                     seed=self.conf_p.get_node_config(node_name)["seed"])
+
+        #return without logging for unit tests
         return init_blocks.logger.pop("InitialBlocks")
 
     @log_on_success
     def init_nodes(self):
         self.init_wallets()
         init_blocks = InitialBlocks(self.conf_p,
                                     self.conf_p.get_nodes_rpc()[0])
         return init_blocks.publish_initial_blocks()
 
     @log_on_success
     def reset_nodes_data(self, nodes: Optional[List[str]] = None):
         self.stop_containers(nodes)
         nodes_to_process = nodes or ['.']
+
         for node in nodes_to_process:
-            node_path = f'{self.nano_nodes_path}/{node}' if nodes else self.nano_nodes_path
-            cmd = 'rm -f $(find . -name "*.ldb")'
-            subprocess_run_capture_output(cmd, node_path)
+            node_path = Path(self.nano_nodes_path) / node if nodes else Path(
+                self.nano_nodes_path)
+            files_to_remove = ['data.ldb', 'wallets.ldb']
+
+            for file_pattern in files_to_remove:
+                for file_path in node_path.rglob(file_pattern):
+                    file_path.unlink()
 
     def init_containers(self):
         self.create_docker_compose_file()
         self.build_containers()
 
     @log_on_success
     def restart_containers(self, nodes: Optional[List[str]] = None):
```

### Comparing `nanomock-0.0.8/nanomock/os_operations/mixin.py` & `nanomock-0.0.9/nanomock/os_operations/mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,9 +19,9 @@
                                       recursive=True):
                 try:
                     os.remove(filename)
                 except OSError as err:
                     logger.error("Error removing file %s\n%s", filename, err)
 
     @staticmethod
-    def makedirs(self, path):
+    def makedirs(path):
         os.makedirs(path, exist_ok=True)
```

### Comparing `nanomock-0.0.8/nanomock.egg-info/PKG-INFO` & `nanomock-0.0.9/nanomock.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanomock
-Version: 0.0.8
+Version: 0.0.9
 Summary: Create local dockerized nano-currency networks
 Home-page: https://github.com/gr0vity-dev/nanomock
 Author: gr0vity
 Description-Content-Type: text/markdown
 
 # nano-local
```

### Comparing `nanomock-0.0.8/nanomock.egg-info/SOURCES.txt` & `nanomock-0.0.9/nanomock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanomock-0.0.8/setup.py` & `nanomock-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name="nanomock",
-      version="0.0.8",
+      version="0.0.9",
       author="gr0vity",
       description="Create local dockerized nano-currency networks",
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/gr0vity-dev/nanomock",
       packages=find_packages(exclude=["unit_tests"]),
       include_package_data=True,
```

