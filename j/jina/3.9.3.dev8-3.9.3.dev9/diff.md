# Comparing `tmp/jina-3.9.3.dev8.tar.gz` & `tmp/jina-3.9.3.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jina-3.9.3.dev8.tar", last modified: Tue Sep 20 11:01:59 2022, max compression
+gzip compressed data, was "dist/jina-3.9.3.dev9.tar", last modified: Wed Sep 21 11:14:05 2022, max compression
```

## Comparing `jina-3.9.3.dev8.tar` & `jina-3.9.3.dev9.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/
--rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    30942 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    24000 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/extra-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/fastentrypoints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/
--rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-09-20 11:01:58.000000 jina-3.9.3.dev8/jina/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/checker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/clients/
--rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/clients/base/
--rw-r--r--   0 runner    (1001) docker     (121)     5211 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/base/grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/base/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/base/http.py
--rw-r--r--   0 runner    (1001) docker     (121)     7844 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/base/websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/http.py
--rw-r--r--   0 runner    (1001) docker     (121)    13936 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/clients/request/
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/request/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/request/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     4283 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/excepts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/exporter.py
--rw-r--r--   0 runner    (1001) docker     (121)    47339 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/hubble/
--rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/hubble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19751 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/hubble/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7834 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/hubble/hubapi.py
--rw-r--r--   0 runner    (1001) docker     (121)    46871 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/hubble/hubio.py
--rw-r--r--   0 runner    (1001) docker     (121)     4565 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/hubble/requirements.py
--rw-r--r--   0 runner    (1001) docker     (121)     5898 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/jaml/
--rw-r--r--   0 runner    (1001) docker     (121)    29036 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9349 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/jaml/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/jaml/parsers/default/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/default/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/jaml/parsers/executor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5696 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/executor/legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/jaml/parsers/flow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4967 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/jaml/parsers/flow/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/logging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (121)     8394 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/logging/logger.py
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/logging/predefined.py
--rw-r--r--   0 runner    (1001) docker     (121)     8833 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/logging/profile.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/
--rw-r--r--   0 runner    (1001) docker     (121)    32110 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17199 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/docker_compose.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)    14581 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8s.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/kubernetes_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/flow/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/flow/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)   107080 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/flow/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/flow/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/orchestrate/pods/
--rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/pods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14774 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/pods/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/pods/container_helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/pods/factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/orchestrate/pods/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/parsers/
--rw-r--r--   0 runner    (1001) docker     (121)     8356 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/create.py
--rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/export.py
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/parsers/hubble/
--rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/hubble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/hubble/new.py
--rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/hubble/pull.py
--rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/hubble/push.py
--rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/hubble/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/pod.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/container.py
--rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/distributed.py
--rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/head.py
--rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/remote.py
--rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/worker.py
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/parsers/ping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/proto/
--rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/jina_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/jina_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/proto/pb/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6486 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb/jina_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14346 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb/jina_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/proto/pb2/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11562 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb2/jina_pb2.py
--rw-r--r--   0 runner    (1001) docker     (121)    14346 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/pb2/jina_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/proto/serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/Python.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/ci-vendors.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/completions/
--rw-r--r--   0 runner    (1001) docker     (121)      567 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/completions/jina.bash
--rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/completions/jina.fish
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/completions/jina.zsh
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/executor-template/
--rw-r--r--   0 runner    (1001) docker     (121)      333 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      163 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/jax.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/tf.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/executor-template/torch.Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-09-20 11:01:58.000000 jina-3.9.3.dev8/jina/resources/extra-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/health_check/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/health_check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/health_check/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/health_check/pod.py
--rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/jina.logo
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/k8s/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/k8s/template/
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/configmap.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-after.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-before-after.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-before.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/deployment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/namespace.yml
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/service.yml
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/service_monitor.yml
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/k8s/template/service_monitoring.yml
--rw-r--r--   0 runner    (1001) docker     (121)      885 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/logging.default.yml
--rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/logging.docker.yml
--rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/logging.profile.yml
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/logging.quiet.yml
--rw-r--r--   0 runner    (1001) docker     (121)      517 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/logging.remote.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/project-template/
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/project-template/client.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/resources/project-template/executor1/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/project-template/executor1/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/project-template/executor1/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/project-template/executor1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/resources/project-template/flow.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/schemas/
--rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/deployment.py
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/flow.py
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/schemas/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/executors/
--rw-r--r--   0 runner    (1001) docker     (121)    21021 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/executors/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/executors/metas.py
--rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    48095 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/
--rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7093 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (121)     5057 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/graph/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19383 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/graph/topology_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/grpc/
--rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/grpc/gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/
--rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14405 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/gateway.py
--rw-r--r--   0 runner    (1001) docker     (121)    10010 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/models.py
--rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/request_handling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10908 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/gateway.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/head/
--rw-r--r--   0 runner    (1001) docker     (121)    15227 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/head/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/monitoring.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/request_handlers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/request_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13660 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/request_handlers/data_request_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/runtimes/worker/
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/runtimes/worker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/serve/stream/
--rw-r--r--   0 runner    (1001) docker     (121)     8442 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/stream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2907 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/stream/helper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7094 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/serve/streamer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/types/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/types/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina/types/request/
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/types/request/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12347 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/types/request/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina/types/request/status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    30942 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/jina_cli/
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     9537 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/export.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/known_plugins.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/jina_cli/lookup.py
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-20 11:01:59.000000 jina-3.9.3.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-09-20 11:00:19.000000 jina-3.9.3.dev8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/
+-rw-r--r--   0 runner    (1001) docker     (121)    10826 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      177 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    30942 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    24000 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/extra-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4059 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/fastentrypoints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/
+-rw-r--r--   0 runner    (1001) docker     (121)     6261 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2010 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/checker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/clients/
+-rw-r--r--   0 runner    (1001) docker     (121)     4623 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (121)     5211 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5838 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/base/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7644 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/base/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6077 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/base/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7844 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/base/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2331 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2468 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/http.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13936 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/clients/request/
+-rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2431 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/request/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2349 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/request/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2443 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7080 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4283 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/excepts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1987 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (121)    47339 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/hubble/
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/hubble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19751 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/hubble/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7834 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/hubble/hubapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46871 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/hubble/hubio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4565 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/hubble/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5898 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/jaml/
+-rw-r--r--   0 runner    (1001) docker     (121)    29036 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9349 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/jaml/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/jaml/parsers/default/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1672 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/default/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/jaml/parsers/executor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5696 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/executor/legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/jaml/parsers/flow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4967 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/jaml/parsers/flow/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/logging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2356 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8394 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/logging/logger.py
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/logging/predefined.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8833 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/logging/profile.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/
+-rw-r--r--   0 runner    (1001) docker     (121)    32110 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17199 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/docker_compose.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14581 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8s.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7602 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/kubernetes_deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2306 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/kubernetes_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/flow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2175 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/flow/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)   107080 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/flow/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1684 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/flow/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/orchestrate/pods/
+-rw-r--r--   0 runner    (1001) docker     (121)    13102 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/pods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14774 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/pods/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2284 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/pods/container_helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/pods/factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2912 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/orchestrate/pods/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/parsers/
+-rw-r--r--   0 runner    (1001) docker     (121)     8356 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1320 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      833 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/create.py
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3965 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8540 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/parsers/hubble/
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/hubble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1307 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/hubble/new.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1160 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/hubble/pull.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2563 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/hubble/push.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1139 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/hubble/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3552 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2193 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3491 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/pod.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2368 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/container.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1311 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1490 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/head.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6177 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/remote.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4115 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/worker.py
+-rw-r--r--   0 runner    (1001) docker     (121)      986 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/parsers/ping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/proto/
+-rw-r--r--   0 runner    (1001) docker     (121)      231 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/jina_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/jina_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/proto/pb/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6486 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb/jina_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14346 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb/jina_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/proto/pb2/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11562 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb2/jina_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14346 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/pb2/jina_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4185 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/proto/serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/Python.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     4170 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/ci-vendors.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/completions/
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/completions/jina.bash
+-rw-r--r--   0 runner    (1001) docker     (121)      663 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/completions/jina.fish
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/completions/jina.zsh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/executor-template/
+-rw-r--r--   0 runner    (1001) docker     (121)      333 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      163 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      191 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/jax.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      468 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/tf.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/executor-template/torch.Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/extra-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/health_check/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/health_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1500 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/health_check/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/health_check/pod.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3922 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/jina.logo
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/k8s/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/k8s/template/
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/configmap.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1772 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-after.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-before-after.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1778 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-before.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1166 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/deployment.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      103 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/namespace.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      247 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/service.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      281 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/service_monitor.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/k8s/template/service_monitoring.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      885 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/logging.default.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      654 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/logging.docker.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      431 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/logging.profile.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/logging.quiet.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      517 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/logging.remote.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/project-template/
+-rw-r--r--   0 runner    (1001) docker     (121)      176 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/project-template/client.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/resources/project-template/executor1/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/project-template/executor1/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      225 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/project-template/executor1/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/project-template/executor1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/resources/project-template/flow.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/schemas/
+-rw-r--r--   0 runner    (1001) docker     (121)     1035 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1057 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1479 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/flow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2415 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/schemas/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/executors/
+-rw-r--r--   0 runner    (1001) docker     (121)    21021 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10792 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/executors/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/executors/metas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3254 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (121)    48095 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1292 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7093 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5057 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/graph/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19383 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/graph/topology_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/grpc/
+-rw-r--r--   0 runner    (1001) docker     (121)     1869 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5833 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/grpc/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/
+-rw-r--r--   0 runner    (1001) docker     (121)     2017 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14405 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6032 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10010 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12718 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/request_handling.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10908 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4137 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/gateway.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/head/
+-rw-r--r--   0 runner    (1001) docker     (121)    15227 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/head/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3779 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)      595 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/monitoring.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/request_handlers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/request_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13660 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/request_handlers/data_request_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/runtimes/worker/
+-rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/runtimes/worker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/serve/stream/
+-rw-r--r--   0 runner    (1001) docker     (121)     8442 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/stream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2907 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/stream/helper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7094 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/serve/streamer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/types/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3794 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/types/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina/types/request/
+-rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/types/request/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12347 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/types/request/data.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2189 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina/types/request/status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    30942 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6300 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     3671 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/jina_cli/
+-rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5267 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9537 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3773 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/known_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4719 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/jina_cli/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 11:14:05.000000 jina-3.9.3.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6636 2022-09-21 11:12:50.000000 jina-3.9.3.dev9/setup.py
```

### Comparing `jina-3.9.3.dev8/LICENSE` & `jina-3.9.3.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/PKG-INFO` & `jina-3.9.3.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a69 6e61  : 2.1.Name: jina
 00000020: 0a56 6572 7369 6f6e 3a20 332e 392e 332e  .Version: 3.9.3.
-00000030: 6465 7638 0a53 756d 6d61 7279 3a20 4275  dev8.Summary: Bu
+00000030: 6465 7639 0a53 756d 6d61 7279 3a20 4275  dev9.Summary: Bu
 00000040: 696c 6420 6372 6f73 732d 6d6f 6461 6c20  ild cross-modal 
 00000050: 616e 6420 6d75 6c74 692d 6d6f 6461 6c20  and multi-modal 
 00000060: 6170 706c 6963 6174 696f 6e73 206f 6e20  applications on 
 00000070: 7468 6520 636c 6f75 6420 c2b7 204e 6575  the cloud .. Neu
 00000080: 7261 6c20 5365 6172 6368 20c2 b720 4372  ral Search .. Cr
 00000090: 6561 7469 7665 2041 4920 c2b7 2043 6c6f  eative AI .. Clo
 000000a0: 7564 204e 6174 6976 6520 c2b7 204d 4c4f  ud Native .. MLO
@@ -1849,20 +1849,20 @@
 00007380: 6c0a 5072 6f76 6964 6573 2d45 7874 7261  l.Provides-Extra
 00007390: 3a20 7061 636b 6167 696e 670a 5072 6f76  : packaging.Prov
 000073a0: 6964 6573 2d45 7874 7261 3a20 646f 6361  ides-Extra: doca
 000073b0: 7272 6179 0a50 726f 7669 6465 732d 4578  rray.Provides-Ex
 000073c0: 7472 613a 206a 696e 612d 6875 6262 6c65  tra: jina-hubble
 000073d0: 2d73 646b 0a50 726f 7669 6465 732d 4578  -sdk.Provides-Ex
 000073e0: 7472 613a 206a 636c 6f75 640a 5072 6f76  tra: jcloud.Prov
-000073f0: 6964 6573 2d45 7874 7261 3a20 7576 6c6f  ides-Extra: uvlo
-00007400: 6f70 0a50 726f 7669 6465 732d 4578 7472  op.Provides-Extr
-00007410: 613a 2070 6572 660a 5072 6f76 6964 6573  a: perf.Provides
-00007420: 2d45 7874 7261 3a20 6465 7665 6c0a 5072  -Extra: devel.Pr
-00007430: 6f76 6964 6573 2d45 7874 7261 3a20 7374  ovides-Extra: st
-00007440: 616e 6461 7264 0a50 726f 7669 6465 732d  andard.Provides-
+000073f0: 6964 6573 2d45 7874 7261 3a20 7374 616e  ides-Extra: stan
+00007400: 6461 7264 0a50 726f 7669 6465 732d 4578  dard.Provides-Ex
+00007410: 7472 613a 2064 6576 656c 0a50 726f 7669  tra: devel.Provi
+00007420: 6465 732d 4578 7472 613a 2075 766c 6f6f  des-Extra: uvloo
+00007430: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
+00007440: 3a20 7065 7266 0a50 726f 7669 6465 732d  : perf.Provides-
 00007450: 4578 7472 613a 2070 726f 6d65 7468 6575  Extra: prometheu
 00007460: 735f 636c 6965 6e74 0a50 726f 7669 6465  s_client.Provide
 00007470: 732d 4578 7472 613a 2066 6173 7461 7069  s-Extra: fastapi
 00007480: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 00007490: 2075 7669 636f 726e 5b73 7461 6e64 6172   uvicorn[standar
 000074a0: 645d 0a50 726f 7669 6465 732d 4578 7472  d].Provides-Extr
 000074b0: 613a 2064 6f63 6172 7261 795b 636f 6d6d  a: docarray[comm
@@ -1881,16 +1881,16 @@
 00007580: 4578 7472 613a 2070 7974 686f 6e2d 6d75  Extra: python-mu
 00007590: 6c74 6970 6172 740a 5072 6f76 6964 6573  ltipart.Provides
 000075a0: 2d45 7874 7261 3a20 6169 6f66 696c 6573  -Extra: aiofiles
 000075b0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 000075c0: 2061 696f 6874 7470 0a50 726f 7669 6465   aiohttp.Provide
 000075d0: 732d 4578 7472 613a 2061 696f 7374 7265  s-Extra: aiostre
 000075e0: 616d 0a50 726f 7669 6465 732d 4578 7472  am.Provides-Extr
-000075f0: 613a 2074 6573 740a 5072 6f76 6964 6573  a: test.Provides
-00007600: 2d45 7874 7261 3a20 7363 6970 790a 5072  -Extra: scipy.Pr
+000075f0: 613a 2073 6369 7079 0a50 726f 7669 6465  a: scipy.Provide
+00007600: 732d 4578 7472 613a 2074 6573 740a 5072  s-Extra: test.Pr
 00007610: 6f76 6964 6573 2d45 7874 7261 3a20 5069  ovides-Extra: Pi
 00007620: 6c6c 6f77 0a50 726f 7669 6465 732d 4578  llow.Provides-Ex
 00007630: 7472 613a 2070 7974 6573 740a 5072 6f76  tra: pytest.Prov
 00007640: 6964 6573 2d45 7874 7261 3a20 7079 7465  ides-Extra: pyte
 00007650: 7374 2d74 696d 656f 7574 0a50 726f 7669  st-timeout.Provi
 00007660: 6465 732d 4578 7472 613a 2070 7974 6573  des-Extra: pytes
 00007670: 742d 6d6f 636b 0a50 726f 7669 6465 732d  t-mock.Provides-
```

### Comparing `jina-3.9.3.dev8/README.md` & `jina-3.9.3.dev9/README.md`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/extra-requirements.txt` & `jina-3.9.3.dev9/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/fastentrypoints.py` & `jina-3.9.3.dev9/fastentrypoints.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/__init__.py` & `jina-3.9.3.dev9/jina/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     _set_start_method('fork')
 
 # do not change this line manually
 # this is managed by git tag and updated on every release
 # NOTE: this represents the NEXT release version
 
-__version__ = '3.9.3.dev8'
+__version__ = '3.9.3.dev9'
 
 # do not change this line manually
 # this is managed by proto/build-proto.sh and updated on every execution
 __proto_version__ = '0.1.13'
 
 try:
     __docarray_version__ = _docarray.__version__
```

### Comparing `jina-3.9.3.dev8/jina/checker.py` & `jina-3.9.3.dev9/jina/checker.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/__init__.py` & `jina-3.9.3.dev9/jina/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/base/__init__.py` & `jina-3.9.3.dev9/jina/clients/base/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/base/grpc.py` & `jina-3.9.3.dev9/jina/clients/base/grpc.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/base/helper.py` & `jina-3.9.3.dev9/jina/clients/base/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/base/http.py` & `jina-3.9.3.dev9/jina/clients/base/http.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/base/websocket.py` & `jina-3.9.3.dev9/jina/clients/base/websocket.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/grpc.py` & `jina-3.9.3.dev9/jina/clients/grpc.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/helper.py` & `jina-3.9.3.dev9/jina/clients/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/http.py` & `jina-3.9.3.dev9/jina/clients/http.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/mixin.py` & `jina-3.9.3.dev9/jina/clients/mixin.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/request/__init__.py` & `jina-3.9.3.dev9/jina/clients/request/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/request/asyncio.py` & `jina-3.9.3.dev9/jina/clients/request/asyncio.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/request/helper.py` & `jina-3.9.3.dev9/jina/clients/request/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/clients/websocket.py` & `jina-3.9.3.dev9/jina/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/enums.py` & `jina-3.9.3.dev9/jina/enums.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/excepts.py` & `jina-3.9.3.dev9/jina/excepts.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/exporter.py` & `jina-3.9.3.dev9/jina/exporter.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/helper.py` & `jina-3.9.3.dev9/jina/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/hubble/helper.py` & `jina-3.9.3.dev9/jina/hubble/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/hubble/hubapi.py` & `jina-3.9.3.dev9/jina/hubble/hubapi.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/hubble/hubio.py` & `jina-3.9.3.dev9/jina/hubble/hubio.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/hubble/requirements.py` & `jina-3.9.3.dev9/jina/hubble/requirements.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/importer.py` & `jina-3.9.3.dev9/jina/importer.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/__init__.py` & `jina-3.9.3.dev9/jina/jaml/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/helper.py` & `jina-3.9.3.dev9/jina/jaml/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/parsers/__init__.py` & `jina-3.9.3.dev9/jina/jaml/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/parsers/base.py` & `jina-3.9.3.dev9/jina/jaml/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/parsers/default/v1.py` & `jina-3.9.3.dev9/jina/jaml/parsers/default/v1.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/parsers/executor/legacy.py` & `jina-3.9.3.dev9/jina/jaml/parsers/executor/legacy.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/jaml/parsers/flow/v1.py` & `jina-3.9.3.dev9/jina/jaml/parsers/flow/v1.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/logging/formatter.py` & `jina-3.9.3.dev9/jina/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/logging/logger.py` & `jina-3.9.3.dev9/jina/logging/logger.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/logging/profile.py` & `jina-3.9.3.dev9/jina/logging/profile.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/__init__.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/config/docker_compose.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/config/docker_compose.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/config/helper.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/config/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8s.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8s.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/kubernetes_deployment.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/kubernetes_deployment.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/deployments/config/k8slib/kubernetes_tools.py` & `jina-3.9.3.dev9/jina/orchestrate/deployments/config/k8slib/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/flow/asyncio.py` & `jina-3.9.3.dev9/jina/orchestrate/flow/asyncio.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/flow/base.py` & `jina-3.9.3.dev9/jina/orchestrate/flow/base.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/flow/builder.py` & `jina-3.9.3.dev9/jina/orchestrate/flow/builder.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/helper.py` & `jina-3.9.3.dev9/jina/orchestrate/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/pods/__init__.py` & `jina-3.9.3.dev9/jina/orchestrate/pods/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/pods/container.py` & `jina-3.9.3.dev9/jina/orchestrate/pods/container.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/pods/container_helper.py` & `jina-3.9.3.dev9/jina/orchestrate/pods/container_helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/pods/factory.py` & `jina-3.9.3.dev9/jina/orchestrate/pods/factory.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/orchestrate/pods/helper.py` & `jina-3.9.3.dev9/jina/orchestrate/pods/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/__init__.py` & `jina-3.9.3.dev9/jina/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/base.py` & `jina-3.9.3.dev9/jina/parsers/base.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/client.py` & `jina-3.9.3.dev9/jina/parsers/client.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/deprecated.py` & `jina-3.9.3.dev9/jina/parsers/deprecated.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/export.py` & `jina-3.9.3.dev9/jina/parsers/export.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/flow.py` & `jina-3.9.3.dev9/jina/parsers/flow.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/helper.py` & `jina-3.9.3.dev9/jina/parsers/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/hubble/__init__.py` & `jina-3.9.3.dev9/jina/parsers/hubble/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/hubble/new.py` & `jina-3.9.3.dev9/jina/parsers/hubble/new.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/hubble/pull.py` & `jina-3.9.3.dev9/jina/parsers/hubble/pull.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/hubble/push.py` & `jina-3.9.3.dev9/jina/parsers/hubble/push.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/hubble/status.py` & `jina-3.9.3.dev9/jina/parsers/hubble/status.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/base.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/base.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/deployment.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/deployment.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/pod.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/pod.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/container.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/container.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/distributed.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/distributed.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/head.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/head.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/remote.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/remote.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/orchestrate/runtimes/worker.py` & `jina-3.9.3.dev9/jina/parsers/orchestrate/runtimes/worker.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/parsers/ping.py` & `jina-3.9.3.dev9/jina/parsers/ping.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/proto/pb/jina_pb2.py` & `jina-3.9.3.dev9/jina/proto/pb/jina_pb2.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/proto/pb/jina_pb2_grpc.py` & `jina-3.9.3.dev9/jina/proto/pb/jina_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/proto/pb2/jina_pb2.py` & `jina-3.9.3.dev9/jina/proto/pb2/jina_pb2.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/proto/pb2/jina_pb2_grpc.py` & `jina-3.9.3.dev9/jina/proto/pb2/jina_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/proto/serializer.py` & `jina-3.9.3.dev9/jina/proto/serializer.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/Python.gitignore` & `jina-3.9.3.dev9/jina/resources/Python.gitignore`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/ci-vendors.json` & `jina-3.9.3.dev9/jina/resources/ci-vendors.json`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/completions/jina.bash` & `jina-3.9.3.dev9/jina/resources/completions/jina.bash`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/completions/jina.fish` & `jina-3.9.3.dev9/jina/resources/completions/jina.fish`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/executor-template/jax.Dockerfile` & `jina-3.9.3.dev9/jina/resources/executor-template/jax.Dockerfile`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/executor-template/torch.Dockerfile` & `jina-3.9.3.dev9/jina/resources/executor-template/torch.Dockerfile`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/extra-requirements.txt` & `jina-3.9.3.dev9/jina/resources/extra-requirements.txt`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/health_check/gateway.py` & `jina-3.9.3.dev9/jina/resources/health_check/gateway.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/health_check/pod.py` & `jina-3.9.3.dev9/jina/resources/health_check/pod.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/jina.logo` & `jina-3.9.3.dev9/jina/resources/jina.logo`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-after.yml` & `jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-after.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-before-after.yml` & `jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-before-after.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/k8s/template/deployment-uses-before.yml` & `jina-3.9.3.dev9/jina/resources/k8s/template/deployment-uses-before.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/k8s/template/deployment.yml` & `jina-3.9.3.dev9/jina/resources/k8s/template/deployment.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/logging.default.yml` & `jina-3.9.3.dev9/jina/resources/logging.default.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/logging.docker.yml` & `jina-3.9.3.dev9/jina/resources/logging.docker.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/logging.quiet.yml` & `jina-3.9.3.dev9/jina/resources/logging.quiet.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/resources/logging.remote.yml` & `jina-3.9.3.dev9/jina/resources/logging.remote.yml`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/schemas/__init__.py` & `jina-3.9.3.dev9/jina/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/schemas/deployment.py` & `jina-3.9.3.dev9/jina/schemas/deployment.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/schemas/flow.py` & `jina-3.9.3.dev9/jina/schemas/flow.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/schemas/helper.py` & `jina-3.9.3.dev9/jina/schemas/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/schemas/meta.py` & `jina-3.9.3.dev9/jina/schemas/meta.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/executors/__init__.py` & `jina-3.9.3.dev9/jina/serve/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/executors/decorators.py` & `jina-3.9.3.dev9/jina/serve/executors/decorators.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/executors/metas.py` & `jina-3.9.3.dev9/jina/serve/executors/metas.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/gateway.py` & `jina-3.9.3.dev9/jina/serve/gateway.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/networking.py` & `jina-3.9.3.dev9/jina/serve/networking.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/asyncio.py` & `jina-3.9.3.dev9/jina/serve/runtimes/asyncio.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/base.py` & `jina-3.9.3.dev9/jina/serve/runtimes/base.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/graph/topology_graph.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/graph/topology_graph.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/grpc/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/grpc/gateway.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/grpc/gateway.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/app.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/app.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/gateway.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/gateway.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/http/models.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/http/models.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/request_handling.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/request_handling.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/app.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/app.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/gateway/websocket/gateway.py` & `jina-3.9.3.dev9/jina/serve/runtimes/gateway/websocket/gateway.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/head/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/head/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/helper.py` & `jina-3.9.3.dev9/jina/serve/runtimes/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/monitoring.py` & `jina-3.9.3.dev9/jina/serve/runtimes/monitoring.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/request_handlers/data_request_handler.py` & `jina-3.9.3.dev9/jina/serve/runtimes/request_handlers/data_request_handler.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/runtimes/worker/__init__.py` & `jina-3.9.3.dev9/jina/serve/runtimes/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/stream/__init__.py` & `jina-3.9.3.dev9/jina/serve/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/stream/helper.py` & `jina-3.9.3.dev9/jina/serve/stream/helper.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/serve/streamer.py` & `jina-3.9.3.dev9/jina/serve/streamer.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/types/mixin.py` & `jina-3.9.3.dev9/jina/types/mixin.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/types/request/__init__.py` & `jina-3.9.3.dev9/jina/types/request/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/types/request/data.py` & `jina-3.9.3.dev9/jina/types/request/data.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina/types/request/status.py` & `jina-3.9.3.dev9/jina/types/request/status.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina.egg-info/PKG-INFO` & `jina-3.9.3.dev9/jina.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6a69 6e61  : 2.1.Name: jina
 00000020: 0a56 6572 7369 6f6e 3a20 332e 392e 332e  .Version: 3.9.3.
-00000030: 6465 7638 0a53 756d 6d61 7279 3a20 4275  dev8.Summary: Bu
+00000030: 6465 7639 0a53 756d 6d61 7279 3a20 4275  dev9.Summary: Bu
 00000040: 696c 6420 6372 6f73 732d 6d6f 6461 6c20  ild cross-modal 
 00000050: 616e 6420 6d75 6c74 692d 6d6f 6461 6c20  and multi-modal 
 00000060: 6170 706c 6963 6174 696f 6e73 206f 6e20  applications on 
 00000070: 7468 6520 636c 6f75 6420 c2b7 204e 6575  the cloud .. Neu
 00000080: 7261 6c20 5365 6172 6368 20c2 b720 4372  ral Search .. Cr
 00000090: 6561 7469 7665 2041 4920 c2b7 2043 6c6f  eative AI .. Clo
 000000a0: 7564 204e 6174 6976 6520 c2b7 204d 4c4f  ud Native .. MLO
@@ -1849,20 +1849,20 @@
 00007380: 6c0a 5072 6f76 6964 6573 2d45 7874 7261  l.Provides-Extra
 00007390: 3a20 7061 636b 6167 696e 670a 5072 6f76  : packaging.Prov
 000073a0: 6964 6573 2d45 7874 7261 3a20 646f 6361  ides-Extra: doca
 000073b0: 7272 6179 0a50 726f 7669 6465 732d 4578  rray.Provides-Ex
 000073c0: 7472 613a 206a 696e 612d 6875 6262 6c65  tra: jina-hubble
 000073d0: 2d73 646b 0a50 726f 7669 6465 732d 4578  -sdk.Provides-Ex
 000073e0: 7472 613a 206a 636c 6f75 640a 5072 6f76  tra: jcloud.Prov
-000073f0: 6964 6573 2d45 7874 7261 3a20 7576 6c6f  ides-Extra: uvlo
-00007400: 6f70 0a50 726f 7669 6465 732d 4578 7472  op.Provides-Extr
-00007410: 613a 2070 6572 660a 5072 6f76 6964 6573  a: perf.Provides
-00007420: 2d45 7874 7261 3a20 6465 7665 6c0a 5072  -Extra: devel.Pr
-00007430: 6f76 6964 6573 2d45 7874 7261 3a20 7374  ovides-Extra: st
-00007440: 616e 6461 7264 0a50 726f 7669 6465 732d  andard.Provides-
+000073f0: 6964 6573 2d45 7874 7261 3a20 7374 616e  ides-Extra: stan
+00007400: 6461 7264 0a50 726f 7669 6465 732d 4578  dard.Provides-Ex
+00007410: 7472 613a 2064 6576 656c 0a50 726f 7669  tra: devel.Provi
+00007420: 6465 732d 4578 7472 613a 2075 766c 6f6f  des-Extra: uvloo
+00007430: 700a 5072 6f76 6964 6573 2d45 7874 7261  p.Provides-Extra
+00007440: 3a20 7065 7266 0a50 726f 7669 6465 732d  : perf.Provides-
 00007450: 4578 7472 613a 2070 726f 6d65 7468 6575  Extra: prometheu
 00007460: 735f 636c 6965 6e74 0a50 726f 7669 6465  s_client.Provide
 00007470: 732d 4578 7472 613a 2066 6173 7461 7069  s-Extra: fastapi
 00007480: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 00007490: 2075 7669 636f 726e 5b73 7461 6e64 6172   uvicorn[standar
 000074a0: 645d 0a50 726f 7669 6465 732d 4578 7472  d].Provides-Extr
 000074b0: 613a 2064 6f63 6172 7261 795b 636f 6d6d  a: docarray[comm
@@ -1881,16 +1881,16 @@
 00007580: 4578 7472 613a 2070 7974 686f 6e2d 6d75  Extra: python-mu
 00007590: 6c74 6970 6172 740a 5072 6f76 6964 6573  ltipart.Provides
 000075a0: 2d45 7874 7261 3a20 6169 6f66 696c 6573  -Extra: aiofiles
 000075b0: 0a50 726f 7669 6465 732d 4578 7472 613a  .Provides-Extra:
 000075c0: 2061 696f 6874 7470 0a50 726f 7669 6465   aiohttp.Provide
 000075d0: 732d 4578 7472 613a 2061 696f 7374 7265  s-Extra: aiostre
 000075e0: 616d 0a50 726f 7669 6465 732d 4578 7472  am.Provides-Extr
-000075f0: 613a 2074 6573 740a 5072 6f76 6964 6573  a: test.Provides
-00007600: 2d45 7874 7261 3a20 7363 6970 790a 5072  -Extra: scipy.Pr
+000075f0: 613a 2073 6369 7079 0a50 726f 7669 6465  a: scipy.Provide
+00007600: 732d 4578 7472 613a 2074 6573 740a 5072  s-Extra: test.Pr
 00007610: 6f76 6964 6573 2d45 7874 7261 3a20 5069  ovides-Extra: Pi
 00007620: 6c6c 6f77 0a50 726f 7669 6465 732d 4578  llow.Provides-Ex
 00007630: 7472 613a 2070 7974 6573 740a 5072 6f76  tra: pytest.Prov
 00007640: 6964 6573 2d45 7874 7261 3a20 7079 7465  ides-Extra: pyte
 00007650: 7374 2d74 696d 656f 7574 0a50 726f 7669  st-timeout.Provi
 00007660: 6465 732d 4578 7472 613a 2070 7974 6573  des-Extra: pytes
 00007670: 742d 6d6f 636b 0a50 726f 7669 6465 732d  t-mock.Provides-
```

### Comparing `jina-3.9.3.dev8/jina.egg-info/SOURCES.txt` & `jina-3.9.3.dev9/jina.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina.egg-info/requires.txt` & `jina-3.9.3.dev9/jina.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 aiofiles
-fastapi>=0.76.0
+docarray[common]>=0.16.3
+requests
+grpcio-reflection<1.48.1,>=1.46.0
 pathspec
+python-multipart
+protobuf>=3.20.0
+fastapi>=0.76.0
+docarray>=0.16.4
+jcloud>=0.0.35
 aiohttp
+prometheus_client
 cryptography
-grpcio-health-checking<1.48.1,>=1.46.0
-numpy
-websockets
-docker
-python-multipart
-pyyaml>=5.3.1
 aiostream
-grpcio-reflection<1.48.1,>=1.46.0
 uvloop
-filelock
+jina-hubble-sdk>=0.16.1
+docker
+websockets
 packaging>=20.0
-prometheus_client
-jcloud>=0.0.35
+grpcio<1.48.1,>=1.46.0
 uvicorn[standard]
-docarray[common]>=0.16.3
-jina-hubble-sdk>=0.16.1
-docarray>=0.16.4
-requests
+grpcio-health-checking<1.48.1,>=1.46.0
+filelock
 pydantic
-protobuf>=3.20.0
-grpcio<1.48.1,>=1.46.0
+numpy
+pyyaml>=5.3.1
 
 [Pillow]
 Pillow
 
 [aiofiles]
 aiofiles
 
@@ -35,118 +35,118 @@
 aiohttp
 
 [aiostream]
 aiostream
 
 [all]
 aiofiles
-fastapi>=0.76.0
+strawberry-graphql>=0.96.0
+pytest-asyncio
+docarray[common]>=0.16.3
+requests
+torch
+grpcio-reflection<1.48.1,>=1.46.0
+flaky
+jsonschema
 pathspec
-aiohttp
-pytest-mock
+pytest-kind==21.1.3
+python-multipart
+protobuf>=3.20.0
+requests-mock
+fastapi>=0.76.0
+docarray>=0.16.4
 pytest-reraise
-pytest-lazy-fixture
-cryptography
-grpcio-health-checking<1.48.1,>=1.46.0
-pytest-custom_exit_code
-numpy
-pytest-asyncio
+pytest-timeout
+tensorflow>=2.0
+pytest
+jcloud>=0.0.35
 scipy>=1.6.1
-websockets
+pytest-custom_exit_code
 pytest-repeat
-kubernetes>=18.20.0
-flaky
-docker
-coverage==6.2
-pyyaml>=5.3.1
-python-multipart
+pytest-mock
+aiohttp
+prometheus_client
+cryptography
 aiostream
-pytest-timeout
-bs4
-pytest-cov
-psutil
-grpcio-reflection<1.48.1,>=1.46.0
 Pillow
-mock
-tensorflow>=2.0
-requests-mock
+coverage==6.2
+kubernetes>=18.20.0
+jina-hubble-sdk>=0.16.1
 uvloop
-portforward>=0.2.4
-filelock
-packaging>=20.0
-prometheus_client
-strawberry-graphql>=0.96.0
+pytest-cov
+black==22.3.0
 sgqlc
-torch
-pytest-kind==21.1.3
-jcloud>=0.0.35
+docker
+websockets
+bs4
+pytest-lazy-fixture
+packaging>=20.0
+grpcio<1.48.1,>=1.46.0
 uvicorn[standard]
-jsonschema
-docarray[common]>=0.16.3
-jina-hubble-sdk>=0.16.1
-docarray>=0.16.4
-requests
+portforward>=0.2.4
+grpcio-health-checking<1.48.1,>=1.46.0
+filelock
+psutil
 pydantic
-black==22.3.0
-protobuf>=3.20.0
-grpcio<1.48.1,>=1.46.0
-pytest
+numpy
+mock
+pyyaml>=5.3.1
 
 [black]
 black==22.3.0
 
 [bs4]
 bs4
 
 [cicd]
-portforward>=0.2.4
+jsonschema
 strawberry-graphql>=0.96.0
+portforward>=0.2.4
 torch
+tensorflow>=2.0
 sgqlc
 bs4
-tensorflow>=2.0
-jsonschema
 
 [core]
-grpcio-reflection<1.48.1,>=1.46.0
-jina-hubble-sdk>=0.16.1
-pyyaml>=5.3.1
-docarray>=0.16.4
-packaging>=20.0
-grpcio-health-checking<1.48.1,>=1.46.0
 protobuf>=3.20.0
-numpy
 grpcio<1.48.1,>=1.46.0
+packaging>=20.0
+docarray>=0.16.4
+grpcio-health-checking<1.48.1,>=1.46.0
+grpcio-reflection<1.48.1,>=1.46.0
+jina-hubble-sdk>=0.16.1
 jcloud>=0.0.35
+numpy
+pyyaml>=5.3.1
 
 [coverage]
 coverage==6.2
 
 [cryptography]
 cryptography
 
 [devel]
-docarray[common]>=0.16.3
-uvloop
-fastapi>=0.76.0
-pathspec
-python-multipart
 aiofiles
-requests
-pydantic
-filelock
-aiohttp
+python-multipart
 prometheus_client
-aiostream
+pathspec
+aiohttp
+uvicorn[standard]
+docarray[common]>=0.16.3
 cryptography
+fastapi>=0.76.0
 strawberry-graphql>=0.96.0
+requests
+filelock
+uvloop
+pydantic
 sgqlc
-websockets
-uvicorn[standard]
 docker
+aiostream
+websockets
 
 [docarray]
 docarray>=0.16.4
 
 [docarray[common]]
 docarray[common]>=0.16.3
 
@@ -192,16 +192,16 @@
 [packaging]
 packaging>=20.0
 
 [pathspec]
 pathspec
 
 [perf]
-uvloop
 prometheus_client
+uvloop
 
 [portforward]
 portforward>=0.2.4
 
 [prometheus_client]
 prometheus_client
 
@@ -259,57 +259,57 @@
 [scipy]
 scipy>=1.6.1
 
 [sgqlc]
 sgqlc
 
 [standard]
+aiofiles
+python-multipart
+prometheus_client
+pathspec
+aiohttp
+uvicorn[standard]
 docarray[common]>=0.16.3
-uvloop
+cryptography
 fastapi>=0.76.0
-pathspec
-python-multipart
-aiofiles
 requests
-pydantic
 filelock
-aiohttp
-prometheus_client
+uvloop
+pydantic
+docker
 aiostream
-cryptography
 websockets
-uvicorn[standard]
-docker
 
 [strawberry-graphql]
 strawberry-graphql>=0.96.0
 
 [tensorflow]
 tensorflow>=2.0
 
 [test]
-pytest-mock
+pytest-asyncio
+flaky
+pytest-kind==21.1.3
+requests-mock
 pytest-reraise
-pytest-lazy-fixture
+pytest-timeout
+pytest
 pytest-custom_exit_code
-pytest-asyncio
 scipy>=1.6.1
-pytest-repeat
-kubernetes>=18.20.0
-flaky
+pytest-mock
+Pillow
 coverage==6.2
-pytest-timeout
+kubernetes>=18.20.0
 pytest-cov
+black==22.3.0
+pytest-lazy-fixture
 psutil
-Pillow
+pytest-repeat
 mock
-requests-mock
-pytest-kind==21.1.3
-black==22.3.0
-pytest
 
 [torch]
 torch
 
 [uvicorn[standard]]
 uvicorn[standard]
```

### Comparing `jina-3.9.3.dev8/jina_cli/__init__.py` & `jina-3.9.3.dev9/jina_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina_cli/api.py` & `jina-3.9.3.dev9/jina_cli/api.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina_cli/autocomplete.py` & `jina-3.9.3.dev9/jina_cli/autocomplete.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina_cli/export.py` & `jina-3.9.3.dev9/jina_cli/export.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/jina_cli/lookup.py` & `jina-3.9.3.dev9/jina_cli/lookup.py`

 * *Files identical despite different names*

### Comparing `jina-3.9.3.dev8/setup.py` & `jina-3.9.3.dev9/setup.py`

 * *Files identical despite different names*

