# Comparing `tmp/aim-4.0.0.dev4.tar.gz` & `tmp/aim-4.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aim-4.0.0.dev4.tar", last modified: Sat Apr 29 15:33:52 2023, max compression
+gzip compressed data, was "aim-4.0.0.dev5.tar", last modified: Mon May  1 19:14:58 2023, max compression
```

## Comparing `aim-4.0.0.dev4.tar` & `aim-4.0.0.dev5.tar`

### file list

```diff
@@ -1,479 +1,479 @@
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.951090 aim-4.0.0.dev4/
--rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev4/LICENSE
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/MANIFEST.in
--rw-r--r--   0 github     (503) staff       (20)    38879 2023-04-29 15:33:52.951264 aim-4.0.0.dev4/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    38192 2023-04-28 20:15:40.000000 aim-4.0.0.dev4/README.md
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.868392 aim-4.0.0.dev4/aim/
--rw-r--r--   0 github     (503) staff       (20)        9 2023-04-29 15:33:43.000000 aim-4.0.0.dev4/aim/VERSION
--rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/__about__.py
--rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/__version__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/acme.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev4/aim/catboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.870341 aim-4.0.0.dev4/aim/cli/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/cli.py
--rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev4/aim/cli/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.870679 aim-4.0.0.dev4/aim/cli/convert/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/convert/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/cli/convert/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.871684 aim-4.0.0.dev4/aim/cli/convert/processors/
--rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/cli/convert/processors/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/aim/cli/convert/processors/mlflow.py
--rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev4/aim/cli/convert/processors/tensorboard.py
--rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/cli/convert/processors/wandb.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872020 aim-4.0.0.dev4/aim/cli/init/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/init/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/init/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872373 aim-4.0.0.dev4/aim/cli/manager/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/manager/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev4/aim/cli/manager/manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.872736 aim-4.0.0.dev4/aim/cli/reindex/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/reindex/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/cli/reindex/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.873365 aim-4.0.0.dev4/aim/cli/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/runs/commands.py
--rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/cli/runs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.873697 aim-4.0.0.dev4/aim/cli/server/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/server/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/server/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.874000 aim-4.0.0.dev4/aim/cli/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev4/aim/cli/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev4/aim/cli/storage/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.874345 aim-4.0.0.dev4/aim/cli/telemetry/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/telemetry/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/telemetry/commands.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.875058 aim-4.0.0.dev4/aim/cli/up/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/up/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/up/commands.py
--rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev4/aim/cli/up/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.875721 aim-4.0.0.dev4/aim/cli/upgrade/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.876494 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/
--rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/configs.py
--rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/metric_artifact.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877138 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877591 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.877984 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.878979 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/
--rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/metric.py
--rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/repo.py
--rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/run.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/trace.py
--rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/utils.py
--rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/upgrade/utils.py
--rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.879237 aim-4.0.0.dev4/aim/cli/version/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/version/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/cli/version/commands.py
--rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/cli/watcher_cli.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.879813 aim-4.0.0.dev4/aim/ext/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.880086 aim-4.0.0.dev4/aim/ext/cleanup/
--rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/ext/cleanup/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/ext/exception_resistant.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.880442 aim-4.0.0.dev4/aim/ext/notebook/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/notebook/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/notebook/notebook.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.882468 aim-4.0.0.dev4/aim/ext/notifier/
--rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/base_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/ext/notifier/config.py
--rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/config_default.json
--rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/config_empty.json
--rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/logging_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/notifier_builder.py
--rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/slack_notifier.py
--rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/utils.py
--rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/notifier/workplace_notifier.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.883736 aim-4.0.0.dev4/aim/ext/resource/
--rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/configs.py
--rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev4/aim/ext/resource/log.py
--rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/resource/stat.py
--rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/resource/tracker.py
--rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/resource/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.883998 aim-4.0.0.dev4/aim/ext/sshfs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/sshfs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/sshfs/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.884288 aim-4.0.0.dev4/aim/ext/task_queue/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/task_queue/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/task_queue/queue.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.884937 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/
--rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/run.py
--rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/ext/tensorboard_tracker/tracker.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.888986 aim-4.0.0.dev4/aim/ext/transport/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/transport/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    13282 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/ext/transport/client.py
--rw-r--r--   0 github     (503) staff       (20)      563 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/ext/transport/config.py
--rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/ext/transport/handlers.py
--rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/health.py
--rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/heartbeat.py
--rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/message_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.890766 aim-4.0.0.dev4/aim/ext/transport/proto/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2_grpc.py
--rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.891721 aim-4.0.0.dev4/aim/ext/transport/proto/v3/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_tracking_pb2.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.892484 aim-4.0.0.dev4/aim/ext/transport/proto/v4/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/health_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_router_pb2.py
--rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_tracking_pb2.py
--rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/ext/transport/remote_resource.py
--rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/ext/transport/remote_tracking.py
--rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/router.py
--rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev4/aim/ext/transport/rpc_queue.py
--rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/ext/transport/server.py
--rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/ext/transport/worker.py
--rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/ext/utils.py
--rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/aim/fastai.py
--rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/hf_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/keras.py
--rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev4/aim/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev4/aim/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev4/aim/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/optuna.py
--rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/paddle.py
--rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev4/aim/prophet.py
--rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/aim/sb3.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.899412 aim-4.0.0.dev4/aim/sdk/
--rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.903019 aim-4.0.0.dev4/aim/sdk/adapters/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/adapters/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3521 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/acme.py
--rw-r--r--   0 github     (503) staff       (20)     4648 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/catboost.py
--rw-r--r--   0 github     (503) staff       (20)     6461 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/fastai.py
--rw-r--r--   0 github     (503) staff       (20)     6610 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/hugging_face.py
--rw-r--r--   0 github     (503) staff       (20)     3438 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras.py
--rw-r--r--   0 github     (503) staff       (20)     1086 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras_mixins.py
--rw-r--r--   0 github     (503) staff       (20)     3718 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/keras_tuner.py
--rw-r--r--   0 github     (503) staff       (20)     3810 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/lightgbm.py
--rw-r--r--   0 github     (503) staff       (20)     9022 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/mxnet.py
--rw-r--r--   0 github     (503) staff       (20)     7300 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/optuna.py
--rw-r--r--   0 github     (503) staff       (20)     3576 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/paddle.py
--rw-r--r--   0 github     (503) staff       (20)     3772 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/prophet.py
--rw-r--r--   0 github     (503) staff       (20)     2436 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch.py
--rw-r--r--   0 github     (503) staff       (20)     9518 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch_ignite.py
--rw-r--r--   0 github     (503) staff       (20)     6871 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/pytorch_lightning.py
--rw-r--r--   0 github     (503) staff       (20)     4711 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/sb3.py
--rw-r--r--   0 github     (503) staff       (20)     3459 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/tensorflow.py
--rw-r--r--   0 github     (503) staff       (20)     3836 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/adapters/xgboost.py
--rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/base_run.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.903811 aim-4.0.0.dev4/aim/sdk/callbacks/
--rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/caller.py
--rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/events.py
--rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/callbacks/helpers.py
--rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev4/aim/sdk/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.905841 aim-4.0.0.dev4/aim/sdk/core/
--rw-r--r--   0 github     (503) staff       (20)      263 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     9802 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/collections.py
--rw-r--r--   0 github     (503) staff       (20)      519 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/constants.py
--rw-r--r--   0 github     (503) staff       (20)    10813 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/container.py
--rw-r--r--   0 github     (503) staff       (20)      561 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/exceptions.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.906253 aim-4.0.0.dev4/aim/sdk/core/interfaces/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1247 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/container.py
--rw-r--r--   0 github     (503) staff       (20)     2255 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/interfaces/sequence.py
--rw-r--r--   0 github     (503) staff       (20)      873 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/object.py
--rw-r--r--   0 github     (503) staff       (20)     2805 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)     5286 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/repo.py
--rw-r--r--   0 github     (503) staff       (20)     9304 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     3534 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/type_utils.py
--rw-r--r--   0 github     (503) staff       (20)      205 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/core/utils.py
--rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev4/aim/sdk/data_version.py
--rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/errors.py
--rw-r--r--   0 github     (503) staff       (20)     4994 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/index_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.907280 aim-4.0.0.dev4/aim/sdk/legacy/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/deprecation_warning.py
--rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/flush.py
--rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/init.py
--rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/select.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.907764 aim-4.0.0.dev4/aim/sdk/legacy/session/
--rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/__init__.py
--rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/configs.py
--rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/session/session.py
--rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/legacy/track.py
--rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/sdk/lock_manager.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.908081 aim-4.0.0.dev4/aim/sdk/logging/
--rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/logging/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev4/aim/sdk/logging/log_record.py
--rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/maintenance_run.py
--rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/num_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.909644 aim-4.0.0.dev4/aim/sdk/objects/
--rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev4/aim/sdk/objects/audio.py
--rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/sdk/objects/distribution.py
--rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev4/aim/sdk/objects/figure.py
--rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev4/aim/sdk/objects/image.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.910009 aim-4.0.0.dev4/aim/sdk/objects/io/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/io/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/io/wavfile.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.911089 aim-4.0.0.dev4/aim/sdk/objects/plugins/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/hf_datasets_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/plugins/hub_dataset.py
--rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/objects/text.py
--rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/aim/sdk/query_utils.py
--rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/remote_repo_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/remote_run_reporter.py
--rw-r--r--   0 github     (503) staff       (20)    34518 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/repo.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev4/aim/sdk/repo_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.911754 aim-4.0.0.dev4/aim/sdk/reporter/
--rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/sdk/reporter/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/aim/sdk/reporter/file_manager.py
--rw-r--r--   0 github     (503) staff       (20)    30870 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/run.py
--rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev4/aim/sdk/run_status_watcher.py
--rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequence.py
--rw-r--r--   0 github     (503) staff       (20)     9975 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/sdk/sequence_collection.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.913159 aim-4.0.0.dev4/aim/sdk/sequences/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/audio_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequences/distribution_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/sequences/figure_sequence.py
--rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/image_sequence.py
--rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev4/aim/sdk/sequences/metric.py
--rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/sequences/text_sequence.py
--rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/aim/sdk/tracker.py
--rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/sdk/training_flow.py
--rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/aim/sdk/types.py
--rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/sdk/uri_service.py
--rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.925774 aim-4.0.0.dev4/aim/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   439810 2023-04-29 15:33:49.000000 aim-4.0.0.dev4/aim/storage/arrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/arrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/arrayview.py
--rw-r--r--   0 github     (503) staff       (20)   844368 2023-04-29 15:33:49.000000 aim-4.0.0.dev4/aim/storage/container.cpp
--rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/container.pxd
--rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/container.py
--rw-r--r--   0 github     (503) staff       (20)   912217 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/containertreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/containertreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/containertreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1825 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/context.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.927198 aim-4.0.0.dev4/aim/storage/encoding/
--rw-r--r--   0 github     (503) staff       (20)   148655 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   378105 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.cpp
--rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.pxd
--rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding.pyx
--rw-r--r--   0 github     (503) staff       (20)   353597 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.cpp
--rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pxd
--rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pyx
--rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/env.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.928546 aim-4.0.0.dev4/aim/storage/hashing/
--rw-r--r--   0 github     (503) staff       (20)   141729 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.cpp
--rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.pxd
--rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/__init__.py
--rw-r--r--   0 github     (503) staff       (20)   205598 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.cpp
--rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.pxd
--rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/c_hash.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.928654 aim-4.0.0.dev4/aim/storage/hashing/hash/
--rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/hash/hash.h
--rw-r--r--   0 github     (503) staff       (20)   392224 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.cpp
--rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.pxd
--rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/hashing/hashing.py
--rw-r--r--   0 github     (503) staff       (20)   672756 2023-04-29 15:33:50.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/inmemorytreeview.py
--rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/lock_proxy.py
--rw-r--r--   0 github     (503) staff       (20)     6344 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/storage/locking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.930046 aim-4.0.0.dev4/aim/storage/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/README
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/script.py.mako
--rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.931198 aim-4.0.0.dev4/aim/storage/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
--rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
--rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/46b89d830ad8_.py
--rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/9ba30ab3b2b4_.py
--rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/b07e7b07c8ce_.py
--rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
--rw-r--r--   0 github     (503) staff       (20)     1657 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/object.py
--rw-r--r--   0 github     (503) staff       (20)   959785 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/prefixview.cpp
--rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/prefixview.pxd
--rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/prefixview.py
--rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/proxy.py
--rw-r--r--   0 github     (503) staff       (20)     4937 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/storage/query.py
--rw-r--r--   0 github     (503) staff       (20)  1056280 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/rockscontainer.cpp
--rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/storage/rockscontainer.pyx
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.931939 aim-4.0.0.dev4/aim/storage/structured/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/db.py
--rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/structured/entities.py
--rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev4/aim/storage/structured/proxy.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.933165 aim-4.0.0.dev4/aim/storage/structured/sql_engine/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/entities.py
--rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/factory.py
--rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/models.py
--rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/structured/sql_engine/utils.py
--rw-r--r--   0 github     (503) staff       (20)   697830 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treearrayview.cpp
--rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treearrayview.pxd
--rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev4/aim/storage/treearrayview.py
--rw-r--r--   0 github     (503) staff       (20)   722166 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treeutils.cpp
--rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev4/aim/storage/treeutils.pyx
--rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treeutils_non_native.py
--rw-r--r--   0 github     (503) staff       (20)   515752 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/treeview.cpp
--rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/treeview.pxd
--rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/storage/treeview.py
--rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev4/aim/storage/treeviewproxy.py
--rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/types.py
--rw-r--r--   0 github     (503) staff       (20)   812526 2023-04-29 15:33:51.000000 aim-4.0.0.dev4/aim/storage/union.cpp
--rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev4/aim/storage/union.pyx
--rw-r--r--   0 github     (503) staff       (20)   810540 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim/storage/utils.cpp
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/utils.pxd
--rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/tensorflow.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.933815 aim-4.0.0.dev4/aim/utils/
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/aim/utils/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev4/aim/utils/deprecation.py
--rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev4/aim/utils/tracking.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.934668 aim-4.0.0.dev4/aim/web/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.935577 aim-4.0.0.dev4/aim/web/api/
--rw-r--r--   0 github     (503) staff       (20)     3616 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.936488 aim-4.0.0.dev4/aim/web/api/dashboard_apps/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/models.py
--rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboard_apps/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.937349 aim-4.0.0.dev4/aim/web/api/dashboards/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/models.py
--rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/dashboards/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/dashboards/serializers.py
--rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/dashboards/views.py
--rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/db.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.937863 aim-4.0.0.dev4/aim/web/api/experiments/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/experiments/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev4/aim/web/api/experiments/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev4/aim/web/api/experiments/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.938676 aim-4.0.0.dev4/aim/web/api/projects/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/projects/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      740 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/projects/project.py
--rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev4/aim/web/api/projects/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev4/aim/web/api/projects/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.939011 aim-4.0.0.dev4/aim/web/api/queries/
--rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/queries/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2770 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/queries/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.940347 aim-4.0.0.dev4/aim/web/api/runs/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/runs/__init__.py
--rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev4/aim/web/api/runs/object_api_utils.py
--rw-r--r--   0 github     (503) staff       (20)     7642 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/runs/object_views.py
--rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev4/aim/web/api/runs/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)    16029 2023-04-06 20:09:56.000000 aim-4.0.0.dev4/aim/web/api/runs/utils.py
--rw-r--r--   0 github     (503) staff       (20)    13619 2023-04-27 20:14:52.000000 aim-4.0.0.dev4/aim/web/api/runs/views.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.940900 aim-4.0.0.dev4/aim/web/api/tags/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/pydantic_models.py
--rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/tags/views.py
--rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/api/utils.py
--rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev4/aim/web/api/views.py
--rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev4/aim/web/configs.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.941056 aim-4.0.0.dev4/aim/web/middlewares/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/__init__.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.941420 aim-4.0.0.dev4/aim/web/middlewares/profiler/
--rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/profiler/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/middlewares/profiler/profiler.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.942337 aim-4.0.0.dev4/aim/web/migrations/
--rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/README
--rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/alembic.ini
--rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/alembic_dev.ini
--rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/env.py
--rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/script.py.mako
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.943023 aim-4.0.0.dev4/aim/web/migrations/versions/
--rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/11672b13f92c_.py
--rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/517a45b2e62c_.py
--rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/5ae8371b7481_.py
--rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/migrations/versions/73a3d004c227_.py
--rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/run.py
--rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/web/utils.py
--rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/aim/xgboost.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.869331 aim-4.0.0.dev4/aim.egg-info/
--rw-r--r--   0 github     (503) staff       (20)    38879 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/PKG-INFO
--rw-r--r--   0 github     (503) staff       (20)    12349 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/SOURCES.txt
--rw-r--r--   0 github     (503) staff       (20)        1 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/dependency_links.txt
--rw-r--r--   0 github     (503) staff       (20)      102 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/entry_points.txt
--rw-r--r--   0 github     (503) staff       (20)      422 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/requires.txt
--rw-r--r--   0 github     (503) staff       (20)       28 2023-04-29 15:33:52.000000 aim-4.0.0.dev4/aim.egg-info/top_level.txt
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.860730 aim-4.0.0.dev4/performance_tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.943993 aim-4.0.0.dev4/performance_tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/queries.py
--rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/test_data_collection.py
--rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/sdk/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/performance_tests/sdk/utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.944874 aim-4.0.0.dev4/performance_tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_container_open.py
--rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_iterative_access.py
--rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/performance_tests/storage/test_random_access.py
--rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/performance_tests/storage/utils.py
--rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/pyproject.toml
--rw-r--r--   0 github     (503) staff       (20)      336 2023-04-29 15:33:52.951584 aim-4.0.0.dev4/setup.cfg
--rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev4/setup.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.861007 aim-4.0.0.dev4/tests/
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.947152 aim-4.0.0.dev4/tests/api/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/api/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/api/test_dashboards_api.py
--rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/api/test_project_api.py
--rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_run_api.py
--rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_run_images_api.py
--rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev4/tests/api/test_structured_data_api.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.948024 aim-4.0.0.dev4/tests/integrations/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/test_dvc_metadata.py
--rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev4/tests/integrations/test_hf_datasets.py
--rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/integrations/test_hub_dataset.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.950228 aim-4.0.0.dev4/tests/sdk/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/test_image_construction.py
--rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_resource_tracker.py
--rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev4/tests/sdk/test_run_apis.py
--rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev4/tests/sdk/test_run_creation_checks.py
--rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/sdk/test_run_finalization_time.py
--rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev4/tests/sdk/test_run_metric_types.py
--rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_run_track_type_checking.py
--rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/sdk/test_run_write_container_data.py
--rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev4/tests/sdk/test_utils.py
-drwxr-xr-x   0 github     (503) staff       (20)        0 2023-04-29 15:33:52.950944 aim-4.0.0.dev4/tests/storage/
--rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev4/tests/storage/__init__.py
--rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/storage/test_query.py
--rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev4/tests/storage/test_query_with_epoch_none.py
--rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev4/tests/storage/test_structured_db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.287487 aim-4.0.0.dev5/
+-rw-r--r--   0 github     (503) staff       (20)    11347 2022-08-06 00:13:01.000000 aim-4.0.0.dev5/LICENSE
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/MANIFEST.in
+-rw-r--r--   0 github     (503) staff       (20)    38879 2023-05-01 19:14:58.287640 aim-4.0.0.dev5/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    38192 2023-04-28 20:15:40.000000 aim-4.0.0.dev5/README.md
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.205849 aim-4.0.0.dev5/aim/
+-rw-r--r--   0 github     (503) staff       (20)       10 2023-05-01 19:14:49.000000 aim-4.0.0.dev5/aim/VERSION
+-rw-r--r--   0 github     (503) staff       (20)      825 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/__about__.py
+-rw-r--r--   0 github     (503) staff       (20)      377 2023-02-01 20:08:30.000000 aim-4.0.0.dev5/aim/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      183 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/__version__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/acme.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-05-06 13:59:46.000000 aim-4.0.0.dev5/aim/catboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.207582 aim-4.0.0.dev5/aim/cli/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1323 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/cli/cli.py
+-rw-r--r--   0 github     (503) staff       (20)      166 2022-06-17 00:13:19.000000 aim-4.0.0.dev5/aim/cli/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.207832 aim-4.0.0.dev5/aim/cli/convert/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/convert/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2998 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/cli/convert/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.208863 aim-4.0.0.dev5/aim/cli/convert/processors/
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/cli/convert/processors/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5914 2022-09-01 19:23:53.000000 aim-4.0.0.dev5/aim/cli/convert/processors/mlflow.py
+-rw-r--r--   0 github     (503) staff       (20)    10372 2022-08-06 00:13:01.000000 aim-4.0.0.dev5/aim/cli/convert/processors/tensorboard.py
+-rw-r--r--   0 github     (503) staff       (20)     6816 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/cli/convert/processors/wandb.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.209288 aim-4.0.0.dev5/aim/cli/init/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/init/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1592 2023-03-24 14:18:45.000000 aim-4.0.0.dev5/aim/cli/init/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.209647 aim-4.0.0.dev5/aim/cli/manager/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/manager/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3382 2022-08-11 13:58:02.000000 aim-4.0.0.dev5/aim/cli/manager/manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.210081 aim-4.0.0.dev5/aim/cli/reindex/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/reindex/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      736 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/cli/reindex/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.210873 aim-4.0.0.dev5/aim/cli/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6621 2023-03-24 14:18:45.000000 aim-4.0.0.dev5/aim/cli/runs/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     2570 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/cli/runs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.211215 aim-4.0.0.dev5/aim/cli/server/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/server/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3709 2023-03-24 14:18:45.000000 aim-4.0.0.dev5/aim/cli/server/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.211515 aim-4.0.0.dev5/aim/cli/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-06-17 00:13:19.000000 aim-4.0.0.dev5/aim/cli/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7537 2023-03-24 14:18:45.000000 aim-4.0.0.dev5/aim/cli/storage/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.211927 aim-4.0.0.dev5/aim/cli/telemetry/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/cli/telemetry/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/cli/telemetry/commands.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.212355 aim-4.0.0.dev5/aim/cli/up/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/up/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5953 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/cli/up/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     1446 2022-06-21 18:01:08.000000 aim-4.0.0.dev5/aim/cli/up/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.213051 aim-4.0.0.dev5/aim/cli/upgrade/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.214497 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/
+-rw-r--r--   0 github     (503) staff       (20)      258 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      734 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      448 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/metric_artifact.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.215148 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      267 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.215628 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3396 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     1919 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.216035 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1111 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      969 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.217051 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/
+-rw-r--r--   0 github     (503) staff       (20)        1 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1722 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/metric.py
+-rw-r--r--   0 github     (503) staff       (20)     3722 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     4062 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/run.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/trace.py
+-rw-r--r--   0 github     (503) staff       (20)     1211 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     6635 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/upgrade/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      370 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.217314 aim-4.0.0.dev5/aim/cli/version/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/version/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      149 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/cli/version/commands.py
+-rw-r--r--   0 github     (503) staff       (20)     9960 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/cli/watcher_cli.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.217868 aim-4.0.0.dev5/aim/ext/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.218156 aim-4.0.0.dev5/aim/ext/cleanup/
+-rw-r--r--   0 github     (503) staff       (20)     3579 2022-11-12 00:14:35.000000 aim-4.0.0.dev5/aim/ext/cleanup/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2021 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/ext/exception_resistant.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.218529 aim-4.0.0.dev5/aim/ext/notebook/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/notebook/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7314 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/notebook/notebook.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.220765 aim-4.0.0.dev5/aim/ext/notifier/
+-rw-r--r--   0 github     (503) staff       (20)      589 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      305 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/base_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1858 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/ext/notifier/config.py
+-rw-r--r--   0 github     (503) staff       (20)      361 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/config_default.json
+-rw-r--r--   0 github     (503) staff       (20)       70 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/config_empty.json
+-rw-r--r--   0 github     (503) staff       (20)      522 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/logging_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1428 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1158 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/notifier_builder.py
+-rw-r--r--   0 github     (503) staff       (20)      524 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/slack_notifier.py
+-rw-r--r--   0 github     (503) staff       (20)     1034 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      862 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/notifier/workplace_notifier.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.222162 aim-4.0.0.dev5/aim/ext/resource/
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/resource/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      100 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/resource/configs.py
+-rw-r--r--   0 github     (503) staff       (20)      726 2022-05-16 21:25:24.000000 aim-4.0.0.dev5/aim/ext/resource/log.py
+-rw-r--r--   0 github     (503) staff       (20)     6700 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/ext/resource/stat.py
+-rw-r--r--   0 github     (503) staff       (20)     7511 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/ext/resource/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)       56 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/resource/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.222523 aim-4.0.0.dev5/aim/ext/sshfs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/sshfs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     7768 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/sshfs/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.222815 aim-4.0.0.dev5/aim/ext/task_queue/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/task_queue/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2069 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/task_queue/queue.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.223480 aim-4.0.0.dev5/aim/ext/tensorboard_tracker/
+-rw-r--r--   0 github     (503) staff       (20)       48 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/ext/tensorboard_tracker/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      919 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/ext/tensorboard_tracker/run.py
+-rw-r--r--   0 github     (503) staff       (20)     7201 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/ext/tensorboard_tracker/tracker.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.226787 aim-4.0.0.dev5/aim/ext/transport/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/transport/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    13282 2023-04-06 20:09:56.000000 aim-4.0.0.dev5/aim/ext/transport/client.py
+-rw-r--r--   0 github     (503) staff       (20)      563 2023-04-06 20:09:56.000000 aim-4.0.0.dev5/aim/ext/transport/config.py
+-rw-r--r--   0 github     (503) staff       (20)     3298 2023-01-23 20:08:00.000000 aim-4.0.0.dev5/aim/ext/transport/handlers.py
+-rw-r--r--   0 github     (503) staff       (20)     5555 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/health.py
+-rw-r--r--   0 github     (503) staff       (20)     5616 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/heartbeat.py
+-rw-r--r--   0 github     (503) staff       (20)     3347 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/message_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.228001 aim-4.0.0.dev5/aim/ext/transport/proto/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      245 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     3991 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/health_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      259 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     8855 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/remote_router_pb2_grpc.py
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     9444 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/remote_tracking_pb2_grpc.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.228828 aim-4.0.0.dev5/aim/ext/transport/proto/v3/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v3/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     6195 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v3/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    25245 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v3/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)    37567 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v3/remote_tracking_pb2.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.229531 aim-4.0.0.dev5/aim/ext/transport/proto/v4/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v4/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1749 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v4/health_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     4280 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v4/remote_router_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)     5662 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/proto/v4/remote_tracking_pb2.py
+-rw-r--r--   0 github     (503) staff       (20)      428 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/ext/transport/remote_resource.py
+-rw-r--r--   0 github     (503) staff       (20)     8078 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/aim/ext/transport/remote_tracking.py
+-rw-r--r--   0 github     (503) staff       (20)     3637 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/router.py
+-rw-r--r--   0 github     (503) staff       (20)     3728 2022-11-18 00:13:03.000000 aim-4.0.0.dev5/aim/ext/transport/rpc_queue.py
+-rw-r--r--   0 github     (503) staff       (20)     4609 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/aim/ext/transport/server.py
+-rw-r--r--   0 github     (503) staff       (20)     3419 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/ext/transport/worker.py
+-rw-r--r--   0 github     (503) staff       (20)     2103 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/ext/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       92 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/aim/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)      127 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/hf_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      105 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/keras.py
+-rw-r--r--   0 github     (503) staff       (20)      103 2022-08-20 12:34:00.000000 aim-4.0.0.dev5/aim/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-05-06 13:59:46.000000 aim-4.0.0.dev5/aim/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)       97 2022-10-04 00:16:28.000000 aim-4.0.0.dev5/aim/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)       98 2022-11-12 00:14:35.000000 aim-4.0.0.dev5/aim/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)       99 2022-11-12 00:14:35.000000 aim-4.0.0.dev5/aim/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)       93 2023-01-31 20:08:25.000000 aim-4.0.0.dev5/aim/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)      115 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)      107 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)      113 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)       87 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/aim/sb3.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.236142 aim-4.0.0.dev5/aim/sdk/
+-rw-r--r--   0 github     (503) staff       (20)      915 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.239786 aim-4.0.0.dev5/aim/sdk/adapters/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/adapters/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3521 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/acme.py
+-rw-r--r--   0 github     (503) staff       (20)     4648 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/catboost.py
+-rw-r--r--   0 github     (503) staff       (20)     6461 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/fastai.py
+-rw-r--r--   0 github     (503) staff       (20)     6610 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/hugging_face.py
+-rw-r--r--   0 github     (503) staff       (20)     3438 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/keras.py
+-rw-r--r--   0 github     (503) staff       (20)     1086 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/keras_mixins.py
+-rw-r--r--   0 github     (503) staff       (20)     3718 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/keras_tuner.py
+-rw-r--r--   0 github     (503) staff       (20)     3810 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/lightgbm.py
+-rw-r--r--   0 github     (503) staff       (20)     9022 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/mxnet.py
+-rw-r--r--   0 github     (503) staff       (20)     7300 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/optuna.py
+-rw-r--r--   0 github     (503) staff       (20)     3576 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/paddle.py
+-rw-r--r--   0 github     (503) staff       (20)     3772 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/prophet.py
+-rw-r--r--   0 github     (503) staff       (20)     2436 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/pytorch.py
+-rw-r--r--   0 github     (503) staff       (20)     9518 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/pytorch_ignite.py
+-rw-r--r--   0 github     (503) staff       (20)     6871 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/pytorch_lightning.py
+-rw-r--r--   0 github     (503) staff       (20)     4711 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/sb3.py
+-rw-r--r--   0 github     (503) staff       (20)     3459 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/tensorflow.py
+-rw-r--r--   0 github     (503) staff       (20)     3836 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/adapters/xgboost.py
+-rw-r--r--   0 github     (503) staff       (20)     5138 2023-03-16 00:07:12.000000 aim-4.0.0.dev5/aim/sdk/base_run.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.240571 aim-4.0.0.dev5/aim/sdk/callbacks/
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/callbacks/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1493 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/callbacks/caller.py
+-rw-r--r--   0 github     (503) staff       (20)      495 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/callbacks/events.py
+-rw-r--r--   0 github     (503) staff       (20)     1416 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/callbacks/helpers.py
+-rw-r--r--   0 github     (503) staff       (20)      253 2022-09-26 00:13:35.000000 aim-4.0.0.dev5/aim/sdk/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.242550 aim-4.0.0.dev5/aim/sdk/core/
+-rw-r--r--   0 github     (503) staff       (20)      263 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     9802 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/collections.py
+-rw-r--r--   0 github     (503) staff       (20)      519 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/constants.py
+-rw-r--r--   0 github     (503) staff       (20)    10813 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/container.py
+-rw-r--r--   0 github     (503) staff       (20)      561 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/exceptions.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.242955 aim-4.0.0.dev5/aim/sdk/core/interfaces/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/interfaces/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1247 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/interfaces/container.py
+-rw-r--r--   0 github     (503) staff       (20)     2255 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/interfaces/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      873 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/object.py
+-rw-r--r--   0 github     (503) staff       (20)     2805 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     5286 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     9304 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3534 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/type_utils.py
+-rw-r--r--   0 github     (503) staff       (20)      205 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/core/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       22 2022-11-24 20:09:30.000000 aim-4.0.0.dev5/aim/sdk/data_version.py
+-rw-r--r--   0 github     (503) staff       (20)      145 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/errors.py
+-rw-r--r--   0 github     (503) staff       (20)     4994 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/index_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.244062 aim-4.0.0.dev5/aim/sdk/legacy/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      288 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/deprecation_warning.py
+-rw-r--r--   0 github     (503) staff       (20)       94 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/flush.py
+-rw-r--r--   0 github     (503) staff       (20)      185 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/init.py
+-rw-r--r--   0 github     (503) staff       (20)      702 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/select.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.244604 aim-4.0.0.dev5/aim/sdk/legacy/session/
+-rw-r--r--   0 github     (503) staff       (20)       67 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/session/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)       30 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/session/configs.py
+-rw-r--r--   0 github     (503) staff       (20)     4277 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/session/session.py
+-rw-r--r--   0 github     (503) staff       (20)      410 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/legacy/track.py
+-rw-r--r--   0 github     (503) staff       (20)     6513 2023-02-01 20:08:30.000000 aim-4.0.0.dev5/aim/sdk/lock_manager.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.244938 aim-4.0.0.dev5/aim/sdk/logging/
+-rw-r--r--   0 github     (503) staff       (20)       61 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/logging/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1863 2023-02-03 15:21:38.000000 aim-4.0.0.dev5/aim/sdk/logging/log_record.py
+-rw-r--r--   0 github     (503) staff       (20)      954 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/maintenance_run.py
+-rw-r--r--   0 github     (503) staff       (20)     3397 2023-03-16 00:07:12.000000 aim-4.0.0.dev5/aim/sdk/num_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.246354 aim-4.0.0.dev5/aim/sdk/objects/
+-rw-r--r--   0 github     (503) staff       (20)      214 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3264 2022-11-11 08:24:45.000000 aim-4.0.0.dev5/aim/sdk/objects/audio.py
+-rw-r--r--   0 github     (503) staff       (20)     4232 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/sdk/objects/distribution.py
+-rw-r--r--   0 github     (503) staff       (20)     2885 2023-01-04 20:08:59.000000 aim-4.0.0.dev5/aim/sdk/objects/figure.py
+-rw-r--r--   0 github     (503) staff       (20)     9914 2023-03-03 20:09:01.000000 aim-4.0.0.dev5/aim/sdk/objects/image.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.246680 aim-4.0.0.dev5/aim/sdk/objects/io/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/io/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    21094 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/io/wavfile.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.247803 aim-4.0.0.dev5/aim/sdk/objects/plugins/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/plugins/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1983 2023-01-23 20:08:00.000000 aim-4.0.0.dev5/aim/sdk/objects/plugins/dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     3648 2023-02-02 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/objects/plugins/hf_datasets_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1272 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/plugins/hub_dataset.py
+-rw-r--r--   0 github     (503) staff       (20)      694 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/objects/text.py
+-rw-r--r--   0 github     (503) staff       (20)     6048 2022-09-01 19:23:53.000000 aim-4.0.0.dev5/aim/sdk/query_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1050 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/aim/sdk/remote_repo_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     2171 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/aim/sdk/remote_run_reporter.py
+-rw-r--r--   0 github     (503) staff       (20)    34518 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/repo.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2023-03-16 00:07:12.000000 aim-4.0.0.dev5/aim/sdk/repo_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.248451 aim-4.0.0.dev5/aim/sdk/reporter/
+-rw-r--r--   0 github     (503) staff       (20)    31012 2023-01-23 20:08:00.000000 aim-4.0.0.dev5/aim/sdk/reporter/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1832 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/aim/sdk/reporter/file_manager.py
+-rw-r--r--   0 github     (503) staff       (20)    30870 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/run.py
+-rw-r--r--   0 github     (503) staff       (20)    13171 2023-02-03 15:21:38.000000 aim-4.0.0.dev5/aim/sdk/run_status_watcher.py
+-rw-r--r--   0 github     (503) staff       (20)    12970 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/sdk/sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     9975 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/sdk/sequence_collection.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.250283 aim-4.0.0.dev5/aim/sdk/sequences/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/sequences/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/sequences/audio_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      408 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/sdk/sequences/distribution_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      452 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/sdk/sequences/figure_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)      482 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/sequences/image_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)     3936 2022-07-09 00:13:12.000000 aim-4.0.0.dev5/aim/sdk/sequences/metric.py
+-rw-r--r--   0 github     (503) staff       (20)      458 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/sequences/text_sequence.py
+-rw-r--r--   0 github     (503) staff       (20)    10545 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/aim/sdk/tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     2202 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/sdk/training_flow.py
+-rw-r--r--   0 github     (503) staff       (20)      159 2022-06-18 00:13:24.000000 aim-4.0.0.dev5/aim/sdk/types.py
+-rw-r--r--   0 github     (503) staff       (20)     2940 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/sdk/uri_service.py
+-rw-r--r--   0 github     (503) staff       (20)     4046 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.262186 aim-4.0.0.dev5/aim/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   439810 2023-05-01 19:14:54.000000 aim-4.0.0.dev5/aim/storage/arrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      278 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/arrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2649 2022-06-15 14:05:59.000000 aim-4.0.0.dev5/aim/storage/arrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   844368 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/container.cpp
+-rw-r--r--   0 github     (503) staff       (20)      951 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/container.pxd
+-rw-r--r--   0 github     (503) staff       (20)    10477 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/container.py
+-rw-r--r--   0 github     (503) staff       (20)   912217 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/containertreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      313 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/containertreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     6026 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/storage/containertreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1825 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/storage/context.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.263666 aim-4.0.0.dev5/aim/storage/encoding/
+-rw-r--r--   0 github     (503) staff       (20)   148655 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/encoding/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)      155 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       95 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   378105 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding.cpp
+-rw-r--r--   0 github     (503) staff       (20)      507 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding.pxd
+-rw-r--r--   0 github     (503) staff       (20)     7373 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding.pyx
+-rw-r--r--   0 github     (503) staff       (20)   353597 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding_native.cpp
+-rw-r--r--   0 github     (503) staff       (20)      930 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding_native.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5974 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/encoding/encoding_native.pyx
+-rw-r--r--   0 github     (503) staff       (20)      337 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/env.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.265040 aim-4.0.0.dev5/aim/storage/hashing/
+-rw-r--r--   0 github     (503) staff       (20)   141729 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/hashing/__init__.cpp
+-rw-r--r--   0 github     (503) staff       (20)       85 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/__init__.pxd
+-rw-r--r--   0 github     (503) staff       (20)       50 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)   205598 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/hashing/c_hash.cpp
+-rw-r--r--   0 github     (503) staff       (20)      151 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/c_hash.pxd
+-rw-r--r--   0 github     (503) staff       (20)     1077 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/c_hash.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.265149 aim-4.0.0.dev5/aim/storage/hashing/hash/
+-rw-r--r--   0 github     (503) staff       (20)     1412 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/hash/hash.h
+-rw-r--r--   0 github     (503) staff       (20)   392224 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/hashing/hashing.cpp
+-rw-r--r--   0 github     (503) staff       (20)     1009 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/hashing/hashing.pxd
+-rw-r--r--   0 github     (503) staff       (20)     5562 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/storage/hashing/hashing.py
+-rw-r--r--   0 github     (503) staff       (20)   672756 2023-05-01 19:14:55.000000 aim-4.0.0.dev5/aim/storage/inmemorytreeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      196 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/inmemorytreeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     4341 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/storage/inmemorytreeview.py
+-rw-r--r--   0 github     (503) staff       (20)     1322 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/storage/lock_proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     6344 2023-04-06 20:09:56.000000 aim-4.0.0.dev5/aim/storage/locking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.266537 aim-4.0.0.dev5/aim/storage/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2218 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)     2215 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2339 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/script.py.mako
+-rw-r--r--   0 github     (503) staff       (20)      965 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.267676 aim-4.0.0.dev5/aim/storage/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2841 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py
+-rw-r--r--   0 github     (503) staff       (20)      658 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1475 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/46b89d830ad8_.py
+-rw-r--r--   0 github     (503) staff       (20)      653 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/9ba30ab3b2b4_.py
+-rw-r--r--   0 github     (503) staff       (20)     1516 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/b07e7b07c8ce_.py
+-rw-r--r--   0 github     (503) staff       (20)      789 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py
+-rw-r--r--   0 github     (503) staff       (20)     1657 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/storage/object.py
+-rw-r--r--   0 github     (503) staff       (20)   959785 2023-05-01 19:14:56.000000 aim-4.0.0.dev5/aim/storage/prefixview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      770 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/prefixview.pxd
+-rw-r--r--   0 github     (503) staff       (20)    11248 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/prefixview.py
+-rw-r--r--   0 github     (503) staff       (20)    11648 2022-06-15 14:05:59.000000 aim-4.0.0.dev5/aim/storage/proxy.py
+-rw-r--r--   0 github     (503) staff       (20)     4937 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/storage/query.py
+-rw-r--r--   0 github     (503) staff       (20)  1056280 2023-05-01 19:14:56.000000 aim-4.0.0.dev5/aim/storage/rockscontainer.cpp
+-rw-r--r--   0 github     (503) staff       (20)    18514 2023-01-23 20:08:00.000000 aim-4.0.0.dev5/aim/storage/rockscontainer.pyx
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.268452 aim-4.0.0.dev5/aim/storage/structured/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/structured/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3183 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/structured/db.py
+-rw-r--r--   0 github     (503) staff       (20)     5355 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/storage/structured/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     2959 2022-11-12 00:14:35.000000 aim-4.0.0.dev5/aim/storage/structured/proxy.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.269655 aim-4.0.0.dev5/aim/storage/structured/sql_engine/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/structured/sql_engine/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    19882 2023-01-25 20:08:55.000000 aim-4.0.0.dev5/aim/storage/structured/sql_engine/entities.py
+-rw-r--r--   0 github     (503) staff       (20)     3484 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/structured/sql_engine/factory.py
+-rw-r--r--   0 github     (503) staff       (20)     4888 2022-11-25 20:09:54.000000 aim-4.0.0.dev5/aim/storage/structured/sql_engine/models.py
+-rw-r--r--   0 github     (503) staff       (20)     4811 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/structured/sql_engine/utils.py
+-rw-r--r--   0 github     (503) staff       (20)   697830 2023-05-01 19:14:56.000000 aim-4.0.0.dev5/aim/storage/treearrayview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      251 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/treearrayview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     3033 2022-08-02 09:43:44.000000 aim-4.0.0.dev5/aim/storage/treearrayview.py
+-rw-r--r--   0 github     (503) staff       (20)   722166 2023-05-01 19:14:56.000000 aim-4.0.0.dev5/aim/storage/treeutils.cpp
+-rw-r--r--   0 github     (503) staff       (20)     8365 2022-06-15 14:05:59.000000 aim-4.0.0.dev5/aim/storage/treeutils.pyx
+-rw-r--r--   0 github     (503) staff       (20)      707 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/treeutils_non_native.py
+-rw-r--r--   0 github     (503) staff       (20)   515752 2023-05-01 19:14:56.000000 aim-4.0.0.dev5/aim/storage/treeview.cpp
+-rw-r--r--   0 github     (503) staff       (20)      311 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/treeview.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2765 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/storage/treeview.py
+-rw-r--r--   0 github     (503) staff       (20)     8241 2023-02-27 08:16:06.000000 aim-4.0.0.dev5/aim/storage/treeviewproxy.py
+-rw-r--r--   0 github     (503) staff       (20)     1357 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/types.py
+-rw-r--r--   0 github     (503) staff       (20)   812526 2023-05-01 19:14:57.000000 aim-4.0.0.dev5/aim/storage/union.cpp
+-rw-r--r--   0 github     (503) staff       (20)     7919 2023-01-23 20:08:00.000000 aim-4.0.0.dev5/aim/storage/union.pyx
+-rw-r--r--   0 github     (503) staff       (20)   810540 2023-05-01 19:14:57.000000 aim-4.0.0.dev5/aim/storage/utils.cpp
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/utils.pxd
+-rw-r--r--   0 github     (503) staff       (20)     2102 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)      119 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/tensorflow.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.270321 aim-4.0.0.dev5/aim/utils/
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/aim/utils/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1209 2023-02-01 20:08:30.000000 aim-4.0.0.dev5/aim/utils/deprecation.py
+-rw-r--r--   0 github     (503) staff       (20)     4728 2023-02-27 08:16:06.000000 aim-4.0.0.dev5/aim/utils/tracking.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.271192 aim-4.0.0.dev5/aim/web/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.272177 aim-4.0.0.dev5/aim/web/api/
+-rw-r--r--   0 github     (503) staff       (20)     3616 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.273101 aim-4.0.0.dev5/aim/web/api/dashboard_apps/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboard_apps/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      939 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboard_apps/models.py
+-rw-r--r--   0 github     (503) staff       (20)      542 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboard_apps/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      445 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboard_apps/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     2974 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboard_apps/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.274005 aim-4.0.0.dev5/aim/web/api/dashboards/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboards/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      667 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboards/models.py
+-rw-r--r--   0 github     (503) staff       (20)      652 2022-10-06 00:17:33.000000 aim-4.0.0.dev5/aim/web/api/dashboards/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)      775 2022-10-06 00:17:33.000000 aim-4.0.0.dev5/aim/web/api/dashboards/serializers.py
+-rw-r--r--   0 github     (503) staff       (20)     3341 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/dashboards/views.py
+-rw-r--r--   0 github     (503) staff       (20)      820 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/db.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.274525 aim-4.0.0.dev5/aim/web/api/experiments/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/experiments/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      974 2022-11-24 20:09:30.000000 aim-4.0.0.dev5/aim/web/api/experiments/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     8931 2023-01-19 20:08:35.000000 aim-4.0.0.dev5/aim/web/api/experiments/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.275362 aim-4.0.0.dev5/aim/web/api/projects/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/projects/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      740 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/projects/project.py
+-rw-r--r--   0 github     (503) staff       (20)      943 2022-10-06 00:17:33.000000 aim-4.0.0.dev5/aim/web/api/projects/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     5200 2023-01-24 20:09:40.000000 aim-4.0.0.dev5/aim/web/api/projects/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.275714 aim-4.0.0.dev5/aim/web/api/queries/
+-rw-r--r--   0 github     (503) staff       (20)        0 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/queries/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2770 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/queries/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.277091 aim-4.0.0.dev5/aim/web/api/runs/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/runs/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)    12969 2022-07-21 10:42:47.000000 aim-4.0.0.dev5/aim/web/api/runs/object_api_utils.py
+-rw-r--r--   0 github     (503) staff       (20)     7642 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/runs/object_views.py
+-rw-r--r--   0 github     (503) staff       (20)     4420 2022-12-23 10:19:51.000000 aim-4.0.0.dev5/aim/web/api/runs/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)    16029 2023-04-06 20:09:56.000000 aim-4.0.0.dev5/aim/web/api/runs/utils.py
+-rw-r--r--   0 github     (503) staff       (20)    13619 2023-04-27 20:14:52.000000 aim-4.0.0.dev5/aim/web/api/runs/views.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.277630 aim-4.0.0.dev5/aim/web/api/tags/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/tags/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      871 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/tags/pydantic_models.py
+-rw-r--r--   0 github     (503) staff       (20)     4272 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/tags/views.py
+-rw-r--r--   0 github     (503) staff       (20)     1169 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/api/utils.py
+-rw-r--r--   0 github     (503) staff       (20)     1589 2022-05-16 21:25:24.000000 aim-4.0.0.dev5/aim/web/api/views.py
+-rw-r--r--   0 github     (503) staff       (20)      508 2022-08-11 13:58:02.000000 aim-4.0.0.dev5/aim/web/configs.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.277791 aim-4.0.0.dev5/aim/web/middlewares/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/middlewares/__init__.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.278156 aim-4.0.0.dev5/aim/web/middlewares/profiler/
+-rw-r--r--   0 github     (503) staff       (20)       81 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/middlewares/profiler/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     3654 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/middlewares/profiler/profiler.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.279137 aim-4.0.0.dev5/aim/web/migrations/
+-rw-r--r--   0 github     (503) staff       (20)       38 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/README
+-rw-r--r--   0 github     (503) staff       (20)      810 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/alembic.ini
+-rw-r--r--   0 github     (503) staff       (20)      807 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/alembic_dev.ini
+-rw-r--r--   0 github     (503) staff       (20)     2792 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/env.py
+-rw-r--r--   0 github     (503) staff       (20)      494 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/script.py.mako
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.279879 aim-4.0.0.dev5/aim/web/migrations/versions/
+-rw-r--r--   0 github     (503) staff       (20)     2183 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/versions/11672b13f92c_.py
+-rw-r--r--   0 github     (503) staff       (20)     1545 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/versions/517a45b2e62c_.py
+-rw-r--r--   0 github     (503) staff       (20)     5592 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/versions/5ae8371b7481_.py
+-rw-r--r--   0 github     (503) staff       (20)     7262 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/migrations/versions/73a3d004c227_.py
+-rw-r--r--   0 github     (503) staff       (20)       55 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/run.py
+-rw-r--r--   0 github     (503) staff       (20)     3055 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/web/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       96 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/aim/xgboost.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.206687 aim-4.0.0.dev5/aim.egg-info/
+-rw-r--r--   0 github     (503) staff       (20)    38879 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/PKG-INFO
+-rw-r--r--   0 github     (503) staff       (20)    12349 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/SOURCES.txt
+-rw-r--r--   0 github     (503) staff       (20)        1 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/dependency_links.txt
+-rw-r--r--   0 github     (503) staff       (20)      102 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/entry_points.txt
+-rw-r--r--   0 github     (503) staff       (20)      423 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/requires.txt
+-rw-r--r--   0 github     (503) staff       (20)       28 2023-05-01 19:14:58.000000 aim-4.0.0.dev5/aim.egg-info/top_level.txt
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.198393 aim-4.0.0.dev5/performance_tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.280836 aim-4.0.0.dev5/performance_tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      469 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/sdk/queries.py
+-rw-r--r--   0 github     (503) staff       (20)     1199 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/sdk/test_data_collection.py
+-rw-r--r--   0 github     (503) staff       (20)     1134 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/sdk/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1881 2022-06-18 00:13:24.000000 aim-4.0.0.dev5/performance_tests/sdk/utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.281744 aim-4.0.0.dev5/performance_tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)      678 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/storage/test_container_open.py
+-rw-r--r--   0 github     (503) staff       (20)      690 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/storage/test_iterative_access.py
+-rw-r--r--   0 github     (503) staff       (20)      802 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/performance_tests/storage/test_random_access.py
+-rw-r--r--   0 github     (503) staff       (20)     1262 2022-06-18 00:13:24.000000 aim-4.0.0.dev5/performance_tests/storage/utils.py
+-rw-r--r--   0 github     (503) staff       (20)       84 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/pyproject.toml
+-rw-r--r--   0 github     (503) staff       (20)      336 2023-05-01 19:14:58.287937 aim-4.0.0.dev5/setup.cfg
+-rw-r--r--   0 github     (503) staff       (20)     6716 2023-03-02 20:49:40.000000 aim-4.0.0.dev5/setup.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.198702 aim-4.0.0.dev5/tests/
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.283469 aim-4.0.0.dev5/tests/api/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/api/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5155 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/api/test_dashboards_api.py
+-rw-r--r--   0 github     (503) staff       (20)     4335 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/api/test_project_api.py
+-rw-r--r--   0 github     (503) staff       (20)    10653 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/tests/api/test_run_api.py
+-rw-r--r--   0 github     (503) staff       (20)    21533 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/tests/api/test_run_images_api.py
+-rw-r--r--   0 github     (503) staff       (20)    12787 2023-01-23 10:30:27.000000 aim-4.0.0.dev5/tests/api/test_structured_data_api.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.284260 aim-4.0.0.dev5/tests/integrations/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/integrations/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     1167 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/integrations/test_dvc_metadata.py
+-rw-r--r--   0 github     (503) staff       (20)     1093 2023-01-13 20:10:23.000000 aim-4.0.0.dev5/tests/integrations/test_hf_datasets.py
+-rw-r--r--   0 github     (503) staff       (20)      961 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/integrations/test_hub_dataset.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.286519 aim-4.0.0.dev5/tests/sdk/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/sdk/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     2312 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/sdk/test_image_construction.py
+-rw-r--r--   0 github     (503) staff       (20)     2665 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/sdk/test_resource_tracker.py
+-rw-r--r--   0 github     (503) staff       (20)     1022 2022-11-01 00:13:35.000000 aim-4.0.0.dev5/tests/sdk/test_run_apis.py
+-rw-r--r--   0 github     (503) staff       (20)     1147 2022-09-01 19:23:53.000000 aim-4.0.0.dev5/tests/sdk/test_run_creation_checks.py
+-rw-r--r--   0 github     (503) staff       (20)     1661 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/sdk/test_run_finalization_time.py
+-rw-r--r--   0 github     (503) staff       (20)     1214 2022-11-01 00:13:35.000000 aim-4.0.0.dev5/tests/sdk/test_run_metric_types.py
+-rw-r--r--   0 github     (503) staff       (20)     4631 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/sdk/test_run_track_type_checking.py
+-rw-r--r--   0 github     (503) staff       (20)    10444 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/sdk/test_run_write_container_data.py
+-rw-r--r--   0 github     (503) staff       (20)     4517 2022-06-01 01:05:15.000000 aim-4.0.0.dev5/tests/sdk/test_utils.py
+drwxr-xr-x   0 github     (503) staff       (20)        0 2023-05-01 19:14:58.287310 aim-4.0.0.dev5/tests/storage/
+-rw-r--r--   0 github     (503) staff       (20)        0 2022-04-19 22:29:06.000000 aim-4.0.0.dev5/tests/storage/__init__.py
+-rw-r--r--   0 github     (503) staff       (20)     5677 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/storage/test_query.py
+-rw-r--r--   0 github     (503) staff       (20)     1482 2022-06-18 00:13:24.000000 aim-4.0.0.dev5/tests/storage/test_query_with_epoch_none.py
+-rw-r--r--   0 github     (503) staff       (20)     1342 2022-09-25 12:02:15.000000 aim-4.0.0.dev5/tests/storage/test_structured_db.py
```

### Comparing `aim-4.0.0.dev4/LICENSE` & `aim-4.0.0.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/PKG-INFO` & `aim-4.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0.dev4
+Version: 4.0.0.dev5
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev4 Summary: A super-easy way
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev5 Summary: A super-easy way
 to record, search and compare AI experiments. Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `aim-4.0.0.dev4/README.md` & `aim-4.0.0.dev5/README.md`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/__about__.py` & `aim-4.0.0.dev5/aim/__about__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/cli.py` & `aim-4.0.0.dev5/aim/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/convert/commands.py` & `aim-4.0.0.dev5/aim/cli/convert/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/convert/processors/mlflow.py` & `aim-4.0.0.dev5/aim/cli/convert/processors/mlflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/convert/processors/tensorboard.py` & `aim-4.0.0.dev5/aim/cli/convert/processors/tensorboard.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/convert/processors/wandb.py` & `aim-4.0.0.dev5/aim/cli/convert/processors/wandb.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/init/commands.py` & `aim-4.0.0.dev5/aim/cli/init/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/manager/manager.py` & `aim-4.0.0.dev5/aim/cli/manager/manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/reindex/commands.py` & `aim-4.0.0.dev5/aim/cli/reindex/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/runs/commands.py` & `aim-4.0.0.dev5/aim/cli/runs/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/runs/utils.py` & `aim-4.0.0.dev5/aim/cli/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/server/commands.py` & `aim-4.0.0.dev5/aim/cli/server/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/storage/commands.py` & `aim-4.0.0.dev5/aim/cli/storage/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/up/commands.py` & `aim-4.0.0.dev5/aim/cli/up/commands.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/up/utils.py` & `aim-4.0.0.dev5/aim/cli/up/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/configs.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/configs.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v3/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/base_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/proto/v4/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/metric.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/repo.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/run.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/trace.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/trace.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/_legacy_repo/repo/utils.py` & `aim-4.0.0.dev5/aim/cli/upgrade/_legacy_repo/repo/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/upgrade/utils.py` & `aim-4.0.0.dev5/aim/cli/upgrade/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/cli/watcher_cli.py` & `aim-4.0.0.dev5/aim/cli/watcher_cli.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/cleanup/__init__.py` & `aim-4.0.0.dev5/aim/ext/cleanup/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/exception_resistant.py` & `aim-4.0.0.dev5/aim/ext/exception_resistant.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notebook/notebook.py` & `aim-4.0.0.dev5/aim/ext/notebook/notebook.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/__init__.py` & `aim-4.0.0.dev5/aim/ext/notifier/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/config.py` & `aim-4.0.0.dev5/aim/ext/notifier/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/logging_notifier.py` & `aim-4.0.0.dev5/aim/ext/notifier/logging_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/notifier.py` & `aim-4.0.0.dev5/aim/ext/notifier/notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/notifier_builder.py` & `aim-4.0.0.dev5/aim/ext/notifier/notifier_builder.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/slack_notifier.py` & `aim-4.0.0.dev5/aim/ext/notifier/slack_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/utils.py` & `aim-4.0.0.dev5/aim/ext/notifier/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/notifier/workplace_notifier.py` & `aim-4.0.0.dev5/aim/ext/notifier/workplace_notifier.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/resource/log.py` & `aim-4.0.0.dev5/aim/ext/resource/log.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/resource/stat.py` & `aim-4.0.0.dev5/aim/ext/resource/stat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/resource/tracker.py` & `aim-4.0.0.dev5/aim/ext/resource/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/sshfs/utils.py` & `aim-4.0.0.dev5/aim/ext/sshfs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/task_queue/queue.py` & `aim-4.0.0.dev5/aim/ext/task_queue/queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/tensorboard_tracker/run.py` & `aim-4.0.0.dev5/aim/ext/tensorboard_tracker/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/tensorboard_tracker/tracker.py` & `aim-4.0.0.dev5/aim/ext/tensorboard_tracker/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/client.py` & `aim-4.0.0.dev5/aim/ext/transport/client.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/config.py` & `aim-4.0.0.dev5/aim/ext/transport/config.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/handlers.py` & `aim-4.0.0.dev5/aim/ext/transport/handlers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/health.py` & `aim-4.0.0.dev5/aim/ext/transport/health.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/heartbeat.py` & `aim-4.0.0.dev5/aim/ext/transport/heartbeat.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/message_utils.py` & `aim-4.0.0.dev5/aim/ext/transport/message_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/health_pb2_grpc.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/health_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/remote_router_pb2_grpc.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/remote_router_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/remote_tracking_pb2_grpc.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/remote_tracking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v3/health_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v3/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_router_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v3/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v3/remote_tracking_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v3/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v4/health_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v4/health_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_router_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v4/remote_router_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/proto/v4/remote_tracking_pb2.py` & `aim-4.0.0.dev5/aim/ext/transport/proto/v4/remote_tracking_pb2.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/remote_tracking.py` & `aim-4.0.0.dev5/aim/ext/transport/remote_tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/router.py` & `aim-4.0.0.dev5/aim/ext/transport/router.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/rpc_queue.py` & `aim-4.0.0.dev5/aim/ext/transport/rpc_queue.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/server.py` & `aim-4.0.0.dev5/aim/ext/transport/server.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/transport/worker.py` & `aim-4.0.0.dev5/aim/ext/transport/worker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/ext/utils.py` & `aim-4.0.0.dev5/aim/ext/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/__init__.py` & `aim-4.0.0.dev5/aim/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/acme.py` & `aim-4.0.0.dev5/aim/sdk/adapters/acme.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/catboost.py` & `aim-4.0.0.dev5/aim/sdk/adapters/catboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/fastai.py` & `aim-4.0.0.dev5/aim/sdk/adapters/fastai.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/hugging_face.py` & `aim-4.0.0.dev5/aim/sdk/adapters/hugging_face.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/keras.py` & `aim-4.0.0.dev5/aim/sdk/adapters/keras.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/keras_mixins.py` & `aim-4.0.0.dev5/aim/sdk/adapters/keras_mixins.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/keras_tuner.py` & `aim-4.0.0.dev5/aim/sdk/adapters/keras_tuner.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/lightgbm.py` & `aim-4.0.0.dev5/aim/sdk/adapters/lightgbm.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/mxnet.py` & `aim-4.0.0.dev5/aim/sdk/adapters/mxnet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/optuna.py` & `aim-4.0.0.dev5/aim/sdk/adapters/optuna.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/paddle.py` & `aim-4.0.0.dev5/aim/sdk/adapters/paddle.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/prophet.py` & `aim-4.0.0.dev5/aim/sdk/adapters/prophet.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/pytorch.py` & `aim-4.0.0.dev5/aim/sdk/adapters/pytorch.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/pytorch_ignite.py` & `aim-4.0.0.dev5/aim/sdk/adapters/pytorch_ignite.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/pytorch_lightning.py` & `aim-4.0.0.dev5/aim/sdk/adapters/pytorch_lightning.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/sb3.py` & `aim-4.0.0.dev5/aim/sdk/adapters/sb3.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/tensorflow.py` & `aim-4.0.0.dev5/aim/sdk/adapters/tensorflow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/adapters/xgboost.py` & `aim-4.0.0.dev5/aim/sdk/adapters/xgboost.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/base_run.py` & `aim-4.0.0.dev5/aim/sdk/base_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/callbacks/caller.py` & `aim-4.0.0.dev5/aim/sdk/callbacks/caller.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/callbacks/helpers.py` & `aim-4.0.0.dev5/aim/sdk/callbacks/helpers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/collections.py` & `aim-4.0.0.dev5/aim/sdk/core/collections.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/constants.py` & `aim-4.0.0.dev5/aim/sdk/core/constants.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/container.py` & `aim-4.0.0.dev5/aim/sdk/core/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/exceptions.py` & `aim-4.0.0.dev5/aim/sdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/interfaces/container.py` & `aim-4.0.0.dev5/aim/sdk/core/interfaces/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/interfaces/sequence.py` & `aim-4.0.0.dev5/aim/sdk/core/interfaces/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/object.py` & `aim-4.0.0.dev5/aim/sdk/core/object.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/query_utils.py` & `aim-4.0.0.dev5/aim/sdk/core/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/repo.py` & `aim-4.0.0.dev5/aim/sdk/core/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/sequence.py` & `aim-4.0.0.dev5/aim/sdk/core/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/core/type_utils.py` & `aim-4.0.0.dev5/aim/sdk/core/type_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/index_manager.py` & `aim-4.0.0.dev5/aim/sdk/index_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/legacy/select.py` & `aim-4.0.0.dev5/aim/sdk/legacy/select.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/legacy/session/session.py` & `aim-4.0.0.dev5/aim/sdk/legacy/session/session.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/lock_manager.py` & `aim-4.0.0.dev5/aim/sdk/lock_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/logging/log_record.py` & `aim-4.0.0.dev5/aim/sdk/logging/log_record.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/maintenance_run.py` & `aim-4.0.0.dev5/aim/sdk/maintenance_run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/num_utils.py` & `aim-4.0.0.dev5/aim/sdk/num_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/audio.py` & `aim-4.0.0.dev5/aim/sdk/objects/audio.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/distribution.py` & `aim-4.0.0.dev5/aim/sdk/objects/distribution.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/figure.py` & `aim-4.0.0.dev5/aim/sdk/objects/figure.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/image.py` & `aim-4.0.0.dev5/aim/sdk/objects/image.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/io/wavfile.py` & `aim-4.0.0.dev5/aim/sdk/objects/io/wavfile.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/plugins/dvc_metadata.py` & `aim-4.0.0.dev5/aim/sdk/objects/plugins/dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/plugins/hf_datasets_metadata.py` & `aim-4.0.0.dev5/aim/sdk/objects/plugins/hf_datasets_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/plugins/hub_dataset.py` & `aim-4.0.0.dev5/aim/sdk/objects/plugins/hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/objects/text.py` & `aim-4.0.0.dev5/aim/sdk/objects/text.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/query_utils.py` & `aim-4.0.0.dev5/aim/sdk/query_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/remote_repo_proxy.py` & `aim-4.0.0.dev5/aim/sdk/remote_repo_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/remote_run_reporter.py` & `aim-4.0.0.dev5/aim/sdk/remote_run_reporter.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/repo.py` & `aim-4.0.0.dev5/aim/sdk/repo.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/repo_utils.py` & `aim-4.0.0.dev5/aim/sdk/repo_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/reporter/__init__.py` & `aim-4.0.0.dev5/aim/sdk/reporter/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/reporter/file_manager.py` & `aim-4.0.0.dev5/aim/sdk/reporter/file_manager.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/run.py` & `aim-4.0.0.dev5/aim/sdk/run.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/run_status_watcher.py` & `aim-4.0.0.dev5/aim/sdk/run_status_watcher.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/sequence.py` & `aim-4.0.0.dev5/aim/sdk/sequence.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/sequence_collection.py` & `aim-4.0.0.dev5/aim/sdk/sequence_collection.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/sequences/metric.py` & `aim-4.0.0.dev5/aim/sdk/sequences/metric.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/tracker.py` & `aim-4.0.0.dev5/aim/sdk/tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/training_flow.py` & `aim-4.0.0.dev5/aim/sdk/training_flow.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/uri_service.py` & `aim-4.0.0.dev5/aim/sdk/uri_service.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/sdk/utils.py` & `aim-4.0.0.dev5/aim/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/arrayview.cpp` & `aim-4.0.0.dev5/aim/storage/arrayview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.arrayview",
         "sources": [
             "aim/storage/arrayview.py"
         ]
     },
     "module_name": "aim.storage.arrayview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/arrayview.py` & `aim-4.0.0.dev5/aim/storage/arrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/container.cpp` & `aim-4.0.0.dev5/aim/storage/container.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.container",
         "sources": [
             "aim/storage/container.py"
         ]
     },
     "module_name": "aim.storage.container"
```

### Comparing `aim-4.0.0.dev4/aim/storage/container.pxd` & `aim-4.0.0.dev5/aim/storage/container.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/container.py` & `aim-4.0.0.dev5/aim/storage/container.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/containertreeview.cpp` & `aim-4.0.0.dev5/aim/storage/containertreeview.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.containertreeview",
         "sources": [
             "aim/storage/containertreeview.py"
         ]
     },
     "module_name": "aim.storage.containertreeview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/containertreeview.py` & `aim-4.0.0.dev5/aim/storage/containertreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/context.py` & `aim-4.0.0.dev5/aim/storage/context.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/__init__.cpp` & `aim-4.0.0.dev5/aim/storage/encoding/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding",
         "sources": [
             "aim/storage/encoding/__init__.py"
         ]
     },
     "module_name": "aim.storage.encoding"
```

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/encoding.cpp` & `aim-4.0.0.dev5/aim/storage/encoding/encoding.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding",
         "sources": [
             "aim/storage/encoding/encoding.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding"
```

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/encoding.pyx` & `aim-4.0.0.dev5/aim/storage/encoding/encoding.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.cpp` & `aim-4.0.0.dev5/aim/storage/encoding/encoding_native.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.encoding.encoding_native",
         "sources": [
             "aim/storage/encoding/encoding_native.pyx"
         ]
     },
     "module_name": "aim.storage.encoding.encoding_native"
```

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pxd` & `aim-4.0.0.dev5/aim/storage/encoding/encoding_native.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/encoding/encoding_native.pyx` & `aim-4.0.0.dev5/aim/storage/encoding/encoding_native.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/__init__.cpp` & `aim-4.0.0.dev5/aim/storage/hashing/__init__.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing",
         "sources": [
             "aim/storage/hashing/__init__.py"
         ]
     },
     "module_name": "aim.storage.hashing"
```

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/c_hash.cpp` & `aim-4.0.0.dev5/aim/storage/hashing/c_hash.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,23 +14,23 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "language_level": "3",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.c_hash",
         "sources": [
             "aim/storage/hashing/c_hash.pyx"
         ]
     },
     "module_name": "aim.storage.hashing.c_hash"
```

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/c_hash.pyx` & `aim-4.0.0.dev5/aim/storage/hashing/c_hash.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/hash/hash.h` & `aim-4.0.0.dev5/aim/storage/hashing/hash/hash.h`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/hashing.cpp` & `aim-4.0.0.dev5/aim/storage/hashing/hashing.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -14,22 +14,22 @@
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
             "aim/storage/hashing",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.hashing.hashing",
         "sources": [
             "aim/storage/hashing/hashing.py"
         ]
     },
     "module_name": "aim.storage.hashing.hashing"
```

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/hashing.pxd` & `aim-4.0.0.dev5/aim/storage/hashing/hashing.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/hashing/hashing.py` & `aim-4.0.0.dev5/aim/storage/hashing/hashing.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/inmemorytreeview.cpp` & `aim-4.0.0.dev5/aim/storage/inmemorytreeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.inmemorytreeview",
         "sources": [
             "aim/storage/inmemorytreeview.py"
         ]
     },
     "module_name": "aim.storage.inmemorytreeview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/inmemorytreeview.py` & `aim-4.0.0.dev5/aim/storage/inmemorytreeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/lock_proxy.py` & `aim-4.0.0.dev5/aim/storage/lock_proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/locking.py` & `aim-4.0.0.dev5/aim/storage/locking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/alembic.ini` & `aim-4.0.0.dev5/aim/storage/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/alembic_dev.ini` & `aim-4.0.0.dev5/aim/storage/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/env.py` & `aim-4.0.0.dev5/aim/storage/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/utils.py` & `aim-4.0.0.dev5/aim/storage/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/1ecf8222220d_initial_schema.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/3c4f22db7a46_run_end_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/46b89d830ad8_.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/46b89d830ad8_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/9ba30ab3b2b4_.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/9ba30ab3b2b4_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/b07e7b07c8ce_.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/b07e7b07c8ce_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py` & `aim-4.0.0.dev5/aim/storage/migrations/versions/fbfe5c4702fb_soft_delete.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/object.py` & `aim-4.0.0.dev5/aim/storage/object.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/prefixview.cpp` & `aim-4.0.0.dev5/aim/storage/prefixview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.prefixview",
         "sources": [
             "aim/storage/prefixview.py"
         ]
     },
     "module_name": "aim.storage.prefixview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/prefixview.pxd` & `aim-4.0.0.dev5/aim/storage/prefixview.pxd`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/prefixview.py` & `aim-4.0.0.dev5/aim/storage/prefixview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/proxy.py` & `aim-4.0.0.dev5/aim/storage/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/query.py` & `aim-4.0.0.dev5/aim/storage/query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/rockscontainer.cpp` & `aim-4.0.0.dev5/aim/storage/rockscontainer.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.rockscontainer",
         "sources": [
             "aim/storage/rockscontainer.pyx"
         ]
     },
     "module_name": "aim.storage.rockscontainer"
```

### Comparing `aim-4.0.0.dev4/aim/storage/rockscontainer.pyx` & `aim-4.0.0.dev5/aim/storage/rockscontainer.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/db.py` & `aim-4.0.0.dev5/aim/storage/structured/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/entities.py` & `aim-4.0.0.dev5/aim/storage/structured/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/proxy.py` & `aim-4.0.0.dev5/aim/storage/structured/proxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/sql_engine/entities.py` & `aim-4.0.0.dev5/aim/storage/structured/sql_engine/entities.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/sql_engine/factory.py` & `aim-4.0.0.dev5/aim/storage/structured/sql_engine/factory.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/sql_engine/models.py` & `aim-4.0.0.dev5/aim/storage/structured/sql_engine/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/structured/sql_engine/utils.py` & `aim-4.0.0.dev5/aim/storage/structured/sql_engine/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/treearrayview.cpp` & `aim-4.0.0.dev5/aim/storage/treearrayview.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treearrayview",
         "sources": [
             "aim/storage/treearrayview.py"
         ]
     },
     "module_name": "aim.storage.treearrayview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/treearrayview.py` & `aim-4.0.0.dev5/aim/storage/treearrayview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/treeutils.cpp` & `aim-4.0.0.dev5/aim/storage/treeutils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -11,22 +11,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeutils",
         "sources": [
             "aim/storage/treeutils.pyx"
         ]
     },
     "module_name": "aim.storage.treeutils"
```

### Comparing `aim-4.0.0.dev4/aim/storage/treeutils.pyx` & `aim-4.0.0.dev5/aim/storage/treeutils.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/treeutils_non_native.py` & `aim-4.0.0.dev5/aim/storage/treeutils_non_native.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/treeview.cpp` & `aim-4.0.0.dev5/aim/storage/treeview.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.treeview",
         "sources": [
             "aim/storage/treeview.py"
         ]
     },
     "module_name": "aim.storage.treeview"
```

### Comparing `aim-4.0.0.dev4/aim/storage/treeview.py` & `aim-4.0.0.dev5/aim/storage/treeview.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/treeviewproxy.py` & `aim-4.0.0.dev5/aim/storage/treeviewproxy.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/types.py` & `aim-4.0.0.dev5/aim/storage/types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/union.cpp` & `aim-4.0.0.dev5/aim/storage/union.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -10,22 +10,22 @@
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.union",
         "sources": [
             "aim/storage/union.pyx"
         ]
     },
     "module_name": "aim.storage.union"
```

### Comparing `aim-4.0.0.dev4/aim/storage/union.pyx` & `aim-4.0.0.dev5/aim/storage/union.pyx`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/storage/utils.cpp` & `aim-4.0.0.dev5/aim/storage/utils.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 /* Generated by Cython 3.0.0a11 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/comparator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/filter_policy_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/memtable_factories.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/merge_operator_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/slice_transform_wrapper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/utils.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rdb_include/write_batch_iter_helper.hpp",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/cache.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/comparator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/db.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/env.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/filter_policy.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/iterator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/memtablerep.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/merge_operator.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/options.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/slice_transform.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/status.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/table.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/universal_compaction.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/utilities/backup_engine.h",
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include/rocksdb/write_batch.h"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-Wall",
             "-Wextra",
             "-Wconversion",
             "-fno-strict-aliasing",
             "-fno-rtti",
             "-fPIC"
         ],
         "include_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks/include"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks/include"
         ],
         "language": "c++",
         "libraries": [
             "rocksdb"
         ],
         "library_dirs": [
-            "/tmp/build-env-nta0804i/lib/python3.10/site-packages/aimrocks"
+            "/tmp/build-env-gyox9tax/lib/python3.10/site-packages/aimrocks"
         ],
         "name": "aim.storage.utils",
         "sources": [
             "aim/storage/utils.py"
         ]
     },
     "module_name": "aim.storage.utils"
```

### Comparing `aim-4.0.0.dev4/aim/storage/utils.py` & `aim-4.0.0.dev5/aim/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/utils/deprecation.py` & `aim-4.0.0.dev5/aim/utils/deprecation.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/utils/tracking.py` & `aim-4.0.0.dev5/aim/utils/tracking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/__init__.py` & `aim-4.0.0.dev5/aim/web/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboard_apps/models.py` & `aim-4.0.0.dev5/aim/web/api/dashboard_apps/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboard_apps/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/dashboard_apps/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboard_apps/views.py` & `aim-4.0.0.dev5/aim/web/api/dashboard_apps/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboards/models.py` & `aim-4.0.0.dev5/aim/web/api/dashboards/models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboards/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/dashboards/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboards/serializers.py` & `aim-4.0.0.dev5/aim/web/api/dashboards/serializers.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/dashboards/views.py` & `aim-4.0.0.dev5/aim/web/api/dashboards/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/db.py` & `aim-4.0.0.dev5/aim/web/api/db.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/experiments/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/experiments/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/experiments/views.py` & `aim-4.0.0.dev5/aim/web/api/experiments/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/projects/project.py` & `aim-4.0.0.dev5/aim/web/api/projects/project.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/projects/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/projects/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/projects/views.py` & `aim-4.0.0.dev5/aim/web/api/projects/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/queries/views.py` & `aim-4.0.0.dev5/aim/web/api/queries/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/runs/object_api_utils.py` & `aim-4.0.0.dev5/aim/web/api/runs/object_api_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/runs/object_views.py` & `aim-4.0.0.dev5/aim/web/api/runs/object_views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/runs/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/runs/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/runs/utils.py` & `aim-4.0.0.dev5/aim/web/api/runs/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/runs/views.py` & `aim-4.0.0.dev5/aim/web/api/runs/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/tags/pydantic_models.py` & `aim-4.0.0.dev5/aim/web/api/tags/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/tags/views.py` & `aim-4.0.0.dev5/aim/web/api/tags/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/utils.py` & `aim-4.0.0.dev5/aim/web/api/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/api/views.py` & `aim-4.0.0.dev5/aim/web/api/views.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/middlewares/profiler/profiler.py` & `aim-4.0.0.dev5/aim/web/middlewares/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/alembic.ini` & `aim-4.0.0.dev5/aim/web/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/alembic_dev.ini` & `aim-4.0.0.dev5/aim/web/migrations/alembic_dev.ini`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/env.py` & `aim-4.0.0.dev5/aim/web/migrations/env.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/versions/11672b13f92c_.py` & `aim-4.0.0.dev5/aim/web/migrations/versions/11672b13f92c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/versions/517a45b2e62c_.py` & `aim-4.0.0.dev5/aim/web/migrations/versions/517a45b2e62c_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/versions/5ae8371b7481_.py` & `aim-4.0.0.dev5/aim/web/migrations/versions/5ae8371b7481_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/migrations/versions/73a3d004c227_.py` & `aim-4.0.0.dev5/aim/web/migrations/versions/73a3d004c227_.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim/web/utils.py` & `aim-4.0.0.dev5/aim/web/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/aim.egg-info/PKG-INFO` & `aim-4.0.0.dev5/aim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aim
-Version: 4.0.0.dev4
+Version: 4.0.0.dev5
 Summary: A super-easy way to record, search and compare AI experiments.
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev4 Summary: A super-easy way
+Metadata-Version: 2.1 Name: aim Version: 4.0.0.dev5 Summary: A super-easy way
 to record, search and compare AI experiments. Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy Requires-
```

### Comparing `aim-4.0.0.dev4/aim.egg-info/SOURCES.txt` & `aim-4.0.0.dev5/aim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/sdk/test_data_collection.py` & `aim-4.0.0.dev5/performance_tests/sdk/test_data_collection.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/sdk/test_query.py` & `aim-4.0.0.dev5/performance_tests/sdk/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/sdk/utils.py` & `aim-4.0.0.dev5/performance_tests/sdk/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/storage/test_container_open.py` & `aim-4.0.0.dev5/performance_tests/storage/test_container_open.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/storage/test_iterative_access.py` & `aim-4.0.0.dev5/performance_tests/storage/test_iterative_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/storage/test_random_access.py` & `aim-4.0.0.dev5/performance_tests/storage/test_random_access.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/performance_tests/storage/utils.py` & `aim-4.0.0.dev5/performance_tests/storage/utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/setup.py` & `aim-4.0.0.dev5/setup.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/api/test_dashboards_api.py` & `aim-4.0.0.dev5/tests/api/test_dashboards_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/api/test_project_api.py` & `aim-4.0.0.dev5/tests/api/test_project_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/api/test_run_api.py` & `aim-4.0.0.dev5/tests/api/test_run_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/api/test_run_images_api.py` & `aim-4.0.0.dev5/tests/api/test_run_images_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/api/test_structured_data_api.py` & `aim-4.0.0.dev5/tests/api/test_structured_data_api.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/integrations/test_dvc_metadata.py` & `aim-4.0.0.dev5/tests/integrations/test_dvc_metadata.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/integrations/test_hf_datasets.py` & `aim-4.0.0.dev5/tests/integrations/test_hf_datasets.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/integrations/test_hub_dataset.py` & `aim-4.0.0.dev5/tests/integrations/test_hub_dataset.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_image_construction.py` & `aim-4.0.0.dev5/tests/sdk/test_image_construction.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_resource_tracker.py` & `aim-4.0.0.dev5/tests/sdk/test_resource_tracker.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_apis.py` & `aim-4.0.0.dev5/tests/sdk/test_run_apis.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_creation_checks.py` & `aim-4.0.0.dev5/tests/sdk/test_run_creation_checks.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_finalization_time.py` & `aim-4.0.0.dev5/tests/sdk/test_run_finalization_time.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_metric_types.py` & `aim-4.0.0.dev5/tests/sdk/test_run_metric_types.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_track_type_checking.py` & `aim-4.0.0.dev5/tests/sdk/test_run_track_type_checking.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_run_write_container_data.py` & `aim-4.0.0.dev5/tests/sdk/test_run_write_container_data.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/sdk/test_utils.py` & `aim-4.0.0.dev5/tests/sdk/test_utils.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/storage/test_query.py` & `aim-4.0.0.dev5/tests/storage/test_query.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/storage/test_query_with_epoch_none.py` & `aim-4.0.0.dev5/tests/storage/test_query_with_epoch_none.py`

 * *Files identical despite different names*

### Comparing `aim-4.0.0.dev4/tests/storage/test_structured_db.py` & `aim-4.0.0.dev5/tests/storage/test_structured_db.py`

 * *Files identical despite different names*

