# Comparing `tmp/phiterm-1.6.2.tar.gz` & `tmp/phiterm-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phiterm-1.6.2.tar", last modified: Wed May  3 15:16:00 2023, max compression
+gzip compressed data, was "phiterm-1.6.3.tar", last modified: Mon May  8 12:59:09 2023, max compression
```

## Comparing `phiterm-1.6.2.tar` & `phiterm-1.6.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.010510 phiterm-1.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-03 15:15:40.000000 phiterm-1.6.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 15:16:00.006509 phiterm-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 15:15:40.000000 phiterm-1.6.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/routes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/api/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/aws/aws_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/cli_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/cli_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/dx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/dx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/dx/dx_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gcp_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/gcp/gke/gke_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/k8s/k8s_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/wf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/wf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/wf/wf_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/cli/ws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/ws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35062 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/cli/ws/ws_app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.994509 phiterm-1.6.2/phiterm/conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/conf/phi_conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/databox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/databox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/databox/databox_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/docker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/docker/docker_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/enums/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/enums/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/enums/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/k8s_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_k8s_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/k8s/tbd_phi_k8s_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/local/local_operator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/release/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/release_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/release_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/release/ws_releases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.998509 phiterm-1.6.2/phiterm/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/user_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/schemas/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm/tbd/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/backend_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/api_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/auth_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/backend_api/workspace_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_zones.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/tbd/tbd_old_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/tbd/tbd_old_api/kubectl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.002509 phiterm-1.6.2/phiterm/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/types/run_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/cli_auth_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/cli_console.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/dttm.py
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/load_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/pyproject.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/utils/ws_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workflow/wf_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/phiterm/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/phi_ws_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)    40288 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-03 15:15:40.000000 phiterm-1.6.2/phiterm/workspace/ws_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:15:59.990508 phiterm-1.6.2/phiterm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-03 15:15:59.000000 phiterm-1.6.2/phiterm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-03 15:15:40.000000 phiterm-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 15:16:00.010510 phiterm-1.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-03 15:15:40.000000 phiterm-1.6.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 15:16:00.006509 phiterm-1.6.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-03 15:15:40.000000 phiterm-1.6.2/tests/test_backend_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.503415 phiterm-1.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     4001 2023-05-08 12:58:45.000000 phiterm-1.6.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 12:59:09.503415 phiterm-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-08 12:58:45.000000 phiterm-1.6.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/routes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/api/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/aws/aws_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/cli_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5700 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/cli_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/cli/dx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/dx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2847 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/dx/dx_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm/cli/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/gcp/gcp_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/cli/gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3196 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/gcp/gke/gke_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/cli/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8420 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/k8s/k8s_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/cli/wf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/wf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/wf/wf_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/cli/ws/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/ws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35062 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/cli/ws/ws_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/conf/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/conf/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/conf/phi_conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/databox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/databox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1930 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/databox/databox_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22147 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/docker/docker_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.491413 phiterm-1.6.3/phiterm/enums/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/enums/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/enums/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.495414 phiterm-1.6.3/phiterm/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/k8s_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12435 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/tbd_k8s_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/tbd_k8s_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/tbd_k8s_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/k8s/tbd_phi_k8s_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.495414 phiterm-1.6.3/phiterm/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/local/local_operator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.495414 phiterm-1.6.3/phiterm/release/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/release/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/release/release_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/release/release_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/release/ws_releases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.495414 phiterm-1.6.3/phiterm/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/schemas/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/schemas/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/schemas/user_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/schemas/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.483412 phiterm-1.6.3/phiterm/tbd/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.495414 phiterm-1.6.3/phiterm/tbd/backend_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/api_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/api_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5636 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/auth_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4595 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/backend_api/workspace_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.499414 phiterm-1.6.3/phiterm/tbd/tbd_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27690 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_zones.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.499414 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20042 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/gke_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/gke_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/phi_gcp_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.499414 phiterm-1.6.3/phiterm/tbd/tbd_old_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_old_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_old_api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10503 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_old_api/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7226 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/tbd/tbd_old_api/kubectl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.499414 phiterm-1.6.3/phiterm/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/types/run_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.499414 phiterm-1.6.3/phiterm/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/cli_auth_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/cli_console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/dttm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/load_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/pyproject.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/utils/ws_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.503415 phiterm-1.6.3/phiterm/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workflow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workflow/wf_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23048 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workflow/wf_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workflow/wf_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.503415 phiterm-1.6.3/phiterm/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/phi_ws_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/ws_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/ws_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40285 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/ws_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/ws_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-05-08 12:58:45.000000 phiterm-1.6.3/phiterm/workspace/ws_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.487413 phiterm-1.6.3/phiterm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-08 12:59:09.000000 phiterm-1.6.3/phiterm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-08 12:58:45.000000 phiterm-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 12:59:09.503415 phiterm-1.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-08 12:58:45.000000 phiterm-1.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 12:59:09.503415 phiterm-1.6.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-08 12:58:45.000000 phiterm-1.6.3/tests/test_backend_api.py
```

### Comparing `phiterm-1.6.2/LICENSE.md` & `phiterm-1.6.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/api/client.py` & `phiterm-1.6.3/phiterm/api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/api/routes.py` & `phiterm-1.6.3/phiterm/api/routes.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/api/user.py` & `phiterm-1.6.3/phiterm/api/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/api/workspace.py` & `phiterm-1.6.3/phiterm/api/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/aws/aws_operator.py` & `phiterm-1.6.3/phiterm/aws/aws_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/cli_app.py` & `phiterm-1.6.3/phiterm/cli/cli_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/cli_operator.py` & `phiterm-1.6.3/phiterm/cli/cli_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/dx/dx_app.py` & `phiterm-1.6.3/phiterm/cli/dx/dx_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/gcp/gcp_app.py` & `phiterm-1.6.3/phiterm/cli/gcp/gcp_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/gcp/gke/gke_app.py` & `phiterm-1.6.3/phiterm/cli/gcp/gke/gke_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/k8s/k8s_app.py` & `phiterm-1.6.3/phiterm/cli/k8s/k8s_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/wf/wf_app.py` & `phiterm-1.6.3/phiterm/cli/wf/wf_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/cli/ws/ws_app.py` & `phiterm-1.6.3/phiterm/cli/ws/ws_app.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/conf/auth.py` & `phiterm-1.6.3/phiterm/conf/auth.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/conf/constants.py` & `phiterm-1.6.3/phiterm/conf/constants.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/conf/phi_conf.py` & `phiterm-1.6.3/phiterm/conf/phi_conf.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/databox/databox_operator.py` & `phiterm-1.6.3/phiterm/databox/databox_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/docker/docker_operator.py` & `phiterm-1.6.3/phiterm/docker/docker_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/enums/user.py` & `phiterm-1.6.3/phiterm/enums/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/k8s/k8s_operator.py` & `phiterm-1.6.3/phiterm/k8s/k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/k8s/tbd_k8s_operator.py` & `phiterm-1.6.3/phiterm/k8s/tbd_k8s_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/k8s/tbd_k8s_ops.py` & `phiterm-1.6.3/phiterm/k8s/tbd_k8s_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/k8s/tbd_k8s_utils.py` & `phiterm-1.6.3/phiterm/k8s/tbd_k8s_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/k8s/tbd_phi_k8s_data.py` & `phiterm-1.6.3/phiterm/k8s/tbd_phi_k8s_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/local/local_operator.py` & `phiterm-1.6.3/phiterm/local/local_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/release/release_schemas.py` & `phiterm-1.6.3/phiterm/release/release_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/release/ws_releases.py` & `phiterm-1.6.3/phiterm/release/ws_releases.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/schemas/user.py` & `phiterm-1.6.3/phiterm/schemas/user.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/schemas/user_schemas.py` & `phiterm-1.6.3/phiterm/schemas/user_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/schemas/workspace.py` & `phiterm-1.6.3/phiterm/schemas/workspace.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/backend_api/api_client.py` & `phiterm-1.6.3/phiterm/tbd/backend_api/api_client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/backend_api/api_utils.py` & `phiterm-1.6.3/phiterm/tbd/backend_api/api_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/backend_api/auth_api.py` & `phiterm-1.6.3/phiterm/tbd/backend_api/auth_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/backend_api/workspace_api.py` & `phiterm-1.6.3/phiterm/tbd/backend_api/workspace_api.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_enums.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_operator.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_schemas.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_utils.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gcp_zones.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gcp_zones.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_operator.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/gke_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/gke/gke_utils.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/gke/gke_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/phi_gcp_data.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/phi_gcp_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py` & `phiterm-1.6.3/phiterm/tbd/tbd_gcp/tbd_gcp_ops.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_old_api/client.py` & `phiterm-1.6.3/phiterm/tbd/tbd_old_api/client.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_old_api/gcp.py` & `phiterm-1.6.3/phiterm/tbd/tbd_old_api/gcp.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/tbd/tbd_old_api/kubectl.py` & `phiterm-1.6.3/phiterm/tbd/tbd_old_api/kubectl.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/cli_auth_server.py` & `phiterm-1.6.3/phiterm/utils/cli_auth_server.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/cli_console.py` & `phiterm-1.6.3/phiterm/utils/cli_console.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/common.py` & `phiterm-1.6.3/phiterm/utils/common.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/dttm.py` & `phiterm-1.6.3/phiterm/utils/dttm.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/enums.py` & `phiterm-1.6.3/phiterm/utils/enums.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/filesystem.py` & `phiterm-1.6.3/phiterm/utils/filesystem.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/git.py` & `phiterm-1.6.3/phiterm/utils/git.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/load_env.py` & `phiterm-1.6.3/phiterm/utils/load_env.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/log.py` & `phiterm-1.6.3/phiterm/utils/log.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/pyproject.py` & `phiterm-1.6.3/phiterm/utils/pyproject.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/utils/ws_filter.py` & `phiterm-1.6.3/phiterm/utils/ws_filter.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/workflow/wf_operator.py` & `phiterm-1.6.3/phiterm/workflow/wf_operator.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/workflow/wf_utils.py` & `phiterm-1.6.3/phiterm/workflow/wf_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/workspace/phi_ws_data.py` & `phiterm-1.6.3/phiterm/workspace/phi_ws_data.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/workspace/ws_enums.py` & `phiterm-1.6.3/phiterm/workspace/ws_enums.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 
 class WorkspaceVisibilityEnum(ExtendedEnum):
     PRIVATE = "PRIVATE"
     PUBLIC = "PUBLIC"
 
 
 class WorkspaceStarterTemplate(ExtendedEnum):
+    api_app = "api-app"
     ml_app = "ml-app"
     ai_app = "ai-app"
-    duck_gpt = "duck-gpt"
     aws_dp = "data-platform"
     aws_spark_dp = "spark-data-platform"
     aws_snowflake_dp = "snowflake-data-platform"
 
 
 class WorkspaceEnv(ExtendedEnum):
     dev = "dev"
```

### Comparing `phiterm-1.6.2/phiterm/workspace/ws_loader.py` & `phiterm-1.6.3/phiterm/workspace/ws_loader.py`

 * *Files 5% similar despite different names*

```diff
@@ -54,15 +54,16 @@
         workspace_config_objects = {}
         config_files = config_dir_path.rglob("*.py")
         for _config_file in config_files:
             if _config_file.name == "__init__.py":
                 continue
             logger.debug(f"Reading file: {_config_file}")
             parent_dir = _config_file.parent.name
-            if parent_dir in ("resources", "tests"):
+            parent_parent_dir = _config_file.parent.parent.name
+            if parent_dir in ("resources", "tests") or parent_parent_dir in ("resources", "tests"):
                 logger.debug(f"Skipping file in {parent_dir}")
                 continue
             try:
                 python_objects = get_python_objects_from_module(_config_file)
                 for obj_name, obj in python_objects.items():
                     _type_name = obj.__class__.__name__
                     if _type_name in [
```

### Comparing `phiterm-1.6.2/phiterm/workspace/ws_operator.py` & `phiterm-1.6.3/phiterm/workspace/ws_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,25 +22,25 @@
     WorkspaceStarterTemplate,
 )
 from phiterm.workspace.exceptions import WorkspaceException
 
 # List of reserved workspace names
 RESERVED_WS_NAMES = ["root", "bedi", "ashpreet", "ashpreetbedi"]
 TEMPLATE_TO_NAME_MAP: Dict[WorkspaceStarterTemplate, str] = {
+    WorkspaceStarterTemplate.api_app: "api-app",
     WorkspaceStarterTemplate.ml_app: "ml-app",
     WorkspaceStarterTemplate.ai_app: "ai-app",
-    WorkspaceStarterTemplate.duck_gpt: "duck-gpt",
     WorkspaceStarterTemplate.aws_dp: "data-platform",
     WorkspaceStarterTemplate.aws_spark_dp: "spark-data-platform",
     WorkspaceStarterTemplate.aws_snowflake_dp: "snowflake-data-platform",
 }
 TEMPLATE_TO_REPO_MAP: Dict[WorkspaceStarterTemplate, str] = {
+    WorkspaceStarterTemplate.api_app: "https://github.com/phidatahq/api-app.git",
     WorkspaceStarterTemplate.ml_app: "https://github.com/phidatahq/ml-app.git",
     WorkspaceStarterTemplate.ai_app: "https://github.com/phidatahq/ai-app.git",
-    WorkspaceStarterTemplate.duck_gpt: "https://github.com/phidatahq/duck-gpt.git",
     WorkspaceStarterTemplate.aws_dp: "https://github.com/phidatahq/aws-dp-template.git",
     WorkspaceStarterTemplate.aws_spark_dp: "https://github.com/phidatahq/aws-spark-dp-template.git",
     WorkspaceStarterTemplate.aws_snowflake_dp: "https://github.com/phidatahq/aws-snowflake-dp-template.git",
 }
 
 
 def create_new_workspace(ws_name: str, template: WorkspaceStarterTemplate) -> bool:
@@ -158,15 +158,15 @@
     for idx, prvdr in enumerate(templates, start=1):
         print_info("  [{}] {}".format(idx, prvdr))
 
     # Get starter template from the user
     template_inp_raw = input(": ")
     # Convert input to int value.
     template_inp = str_to_int(template_inp_raw)
-    template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.ml_app
+    template: WorkspaceStarterTemplate = WorkspaceStarterTemplate.api_app
 
     if template_inp is not None:
         try:
             template = cast(
                 WorkspaceStarterTemplate,
                 WorkspaceStarterTemplate.from_str(templates[template_inp - 1]),
             )
```

### Comparing `phiterm-1.6.2/phiterm/workspace/ws_schemas.py` & `phiterm-1.6.3/phiterm/workspace/ws_schemas.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm/workspace/ws_utils.py` & `phiterm-1.6.3/phiterm/workspace/ws_utils.py`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/phiterm.egg-info/SOURCES.txt` & `phiterm-1.6.3/phiterm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phiterm-1.6.2/pyproject.toml` & `phiterm-1.6.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phiterm"
-version = "1.6.2"
+version = "1.6.3"
 requires-python = ">=3.7"
 readme = "README.md"
 authors = [
   {name = "Ashpreet Bedi", email = "ashpreet@phidata.com"}
 ]
 
 dependencies = [
```

