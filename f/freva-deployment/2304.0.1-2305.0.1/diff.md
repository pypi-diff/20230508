# Comparing `tmp/freva_deployment-2304.0.1.tar.gz` & `tmp/freva_deployment-2305.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freva_deployment-2304.0.1.tar", last modified: Sat Apr 22 21:30:38 2023, max compression
+gzip compressed data, was "freva_deployment-2305.0.1.tar", last modified: Mon May  8 15:03:24 2023, max compression
```

## Comparing `freva_deployment-2304.0.1.tar` & `freva_deployment-2305.0.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.712277 freva_deployment-2304.0.1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/config/
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/config/create_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-22 21:30:29.000000 freva_deployment-2304.0.1/assets/config/evaluation_system.conf.tmpl
--rw-r--r--   0 runner    (1001) docker     (123)    10288 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/config/inventory.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/db_service/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/db_service/password_rotate.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/db_service/reset_root_pw.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/core-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/db-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/server-map-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/solr-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/vault-server-playbook.yml
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/playbooks/web-server-playbook.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.716277 freva_deployment-2304.0.1/assets/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/create_cron.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/create_systemd.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/docker-or-podman
--rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/scripts/dump_sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/servers/
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/servers/freva/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/freva/servers.toml
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/servers/restservice.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/vault/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/deploy_vault.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/policy-file.hcl
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/runserver.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/vault-server-no-tls.hcl
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/vault/vault-server-tls.hcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/assets/web/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/docker_cmd.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/assets/web/freva_web.conf
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.712277 freva_deployment-2304.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.720277 freva_deployment-2304.0.1/src/freva_deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_server_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/cli/_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/deploy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment/ui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.728277 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    33544 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-04-22 21:30:28.000000 freva_deployment-2304.0.1/src/freva_deployment/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:30:38.724277 freva_deployment-2304.0.1/src/freva_deployment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-22 21:30:38.000000 freva_deployment-2304.0.1/src/freva_deployment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.749595 freva_deployment-2305.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/create_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/evaluation_system.conf.tmpl
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/config/inventory.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/assets/db_service/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/db_service/password_rotate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/db_service/reset_root_pw.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     5278 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/core-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5643 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/db-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/server-map-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/solr-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/vault-server-playbook.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/playbooks/web-server-playbook.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      351 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/create_cron.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/create_systemd.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3293 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/docker-or-podman
+-rwxr-xr-x   0 runner    (1001) docker     (123)       66 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/scripts/dump_sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/servers/
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/servers/freva/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/freva/servers.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/servers/restservice.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/vault/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/deploy_vault.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/policy-file.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/runserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/vault-server-no-tls.hcl
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/vault/vault-server-tls.hcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.741595 freva_deployment-2305.0.1/assets/web/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2305 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)       38 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/docker_cmd.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       17 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)    15874 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/assets/web/freva_web.conf
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 15:03:24.749595 freva_deployment-2305.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.737595 freva_deployment-2305.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_server_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7201 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/cli/_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21996 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13252 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34020 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10320 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11596 2023-05-08 15:03:12.000000 freva_deployment-2305.0.1/src/freva_deployment/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 15:03:24.745595 freva_deployment-2305.0.1/src/freva_deployment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16382 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-08 15:03:24.000000 freva_deployment-2305.0.1/src/freva_deployment.egg-info/top_level.txt
```

### Comparing `freva_deployment-2304.0.1/PKG-INFO` & `freva_deployment-2305.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva_deployment
-Version: 2304.0.1
+Version: 2305.0.1
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2304.0.1/README.md` & `freva_deployment-2305.0.1/README.md`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/config/create_tables.sql` & `freva_deployment-2305.0.1/assets/config/create_tables.sql`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/config/evaluation_system.conf.tmpl` & `freva_deployment-2305.0.1/assets/config/evaluation_system.conf.tmpl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/config/inventory.toml` & `freva_deployment-2305.0.1/assets/config/inventory.toml`

 * *Files 1% similar despite different names*

```diff
@@ -280,15 +280,15 @@
 ldap_model = "MiklipUserInformation"
 
 ## set the passwd for the ldap user
 ldap_user_pw = ""
 
 #######
 ## Set the hosts that are allowed to execute wsgi code
-allowed_hosts = ["www.freva.dkrz.de", "localhost"]
+allowed_hosts = ["localhost"]
 
 ## Turn on/off debug mode on the website
 debug=false
 
 ## Which plugin id should be used for the web tour
 guest_tour_result = 105
```

### Comparing `freva_deployment-2304.0.1/assets/db_service/password_rotate.py` & `freva_deployment-2305.0.1/assets/db_service/password_rotate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/core-server-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/core-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/db-server-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/db-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/server-map-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/server-map-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/solr-server-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/solr-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/vault-server-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/vault-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/playbooks/web-server-playbook.yml` & `freva_deployment-2305.0.1/assets/playbooks/web-server-playbook.yml`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/scripts/create_systemd.py` & `freva_deployment-2305.0.1/assets/scripts/create_systemd.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/scripts/docker-or-podman` & `freva_deployment-2305.0.1/assets/scripts/docker-or-podman`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/servers/Dockerfile` & `freva_deployment-2305.0.1/assets/servers/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/servers/restservice.py` & `freva_deployment-2305.0.1/assets/servers/restservice.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/vault/Dockerfile` & `freva_deployment-2305.0.1/assets/vault/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/vault/deploy_vault.py` & `freva_deployment-2305.0.1/assets/vault/deploy_vault.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/vault/runserver.py` & `freva_deployment-2305.0.1/assets/vault/runserver.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/vault/vault-server-tls.hcl` & `freva_deployment-2305.0.1/assets/vault/vault-server-tls.hcl`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/web/Dockerfile` & `freva_deployment-2305.0.1/assets/web/Dockerfile`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/assets/web/freva_web.conf` & `freva_deployment-2305.0.1/assets/web/freva_web.conf`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/setup.py` & `freva_deployment-2305.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/cli/_deploy.py` & `freva_deployment-2305.0.1/src/freva_deployment/cli/_deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/cli/_migrate.py` & `freva_deployment-2305.0.1/src/freva_deployment/cli/_migrate.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/cli/_server_map.py` & `freva_deployment-2305.0.1/src/freva_deployment/cli/_server_map.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/cli/_service.py` & `freva_deployment-2305.0.1/src/freva_deployment/cli/_service.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/deploy.py` & `freva_deployment-2305.0.1/src/freva_deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/__init__.py` & `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/__init__.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/base.py` & `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/base.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py` & `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/deploy_forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -388,14 +388,27 @@
                             List[str],
                             cfg.get("scheduler_host", ["levante.dkrz.de"]),
                         )
                     ),
                 ),
                 True,
             ),
+            allowed_hosts=(
+                self.add_widget_intelligent(
+                    npyscreen.TitleText,
+                    name=f"{self.num}Set additional hostnames django can serve:",
+                    value=",".join(
+                        cast(
+                            List[str],
+                            cfg.get("allowed_hosts", ["localhost"]),
+                        ),
+                    ),
+                ),
+                True,
+            ),
             auth_ldap_server_uri=(
                 self.add_widget_intelligent(
                     npyscreen.TitleText,
                     name=(
                         f"{self.num}Ldap server name(s) used for authentication"
                         " - comma separated:"
                     ),
```

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/ui/deployment_tui/main_window.py` & `freva_deployment-2305.0.1/src/freva_deployment/ui/deployment_tui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,26 +198,33 @@
             "config": self.config,
         }
         with open(self.cache_dir / "freva_deployment.json", "w") as f:
             json.dump({k: v for (k, v) in config.items()}, f, indent=3)
         if write_toml_file is False:
             return None
         try:
+            with open(self.save_file) as f:
+                config_tmpl = cast(Dict[str, Any], tomlkit.load(f))
+        except FileNotFoundError:
             with open(asset_dir / "config" / "inventory.toml") as f:
                 config_tmpl = cast(Dict[str, Any], tomlkit.load(f))
         except Exception:
             config_tmpl = self.config
         config_tmpl["certificates"] = cert_files
         config_tmpl["project_name"] = project_name
         for step, settings in self.config.items():
             if step in ("certificates", "project_name"):
                 continue
             config_tmpl[step]["hosts"] = settings["hosts"]
             for key, config in settings["config"].items():
                 config_tmpl[step]["config"][key] = config
+                if key == "allowed_hosts" and step == "web":
+                    config_tmpl[step]["config"][key] = list(
+                        set(cast(str, config).split(","))
+                    )
         Path(self.save_file).parent.mkdir(exist_ok=True, parents=True)
         with open(self.save_file, "w") as f:
             toml_string = tomlkit.dumps(config_tmpl)
             f.write(toml_string)
         return Path(self.save_file)
 
     @property
```

### Comparing `freva_deployment-2304.0.1/src/freva_deployment/utils.py` & `freva_deployment-2305.0.1/src/freva_deployment/utils.py`

 * *Files identical despite different names*

### Comparing `freva_deployment-2304.0.1/src/freva_deployment.egg-info/PKG-INFO` & `freva_deployment-2305.0.1/src/freva_deployment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freva-deployment
-Version: 2304.0.1
+Version: 2305.0.1
 Summary: Deploy freva and its services on different machines.
 Home-page: https://github.com/FREVA-CLINT/freva.git
 Author: Martin Bergemann
 Author-email: martin.bergemann@dkrz.de
 Maintainer: Martin Bergemann
 License: GPLv3
 Project-URL: Documentation, https://freva-deployment.readthedocs.io/en/latest/
```

### Comparing `freva_deployment-2304.0.1/src/freva_deployment.egg-info/SOURCES.txt` & `freva_deployment-2305.0.1/src/freva_deployment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

