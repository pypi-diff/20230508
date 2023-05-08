# Comparing `tmp/accelerate-0.8.0.tar.gz` & `tmp/accelerate-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelerate-0.8.0.tar", last modified: Thu May 12 14:53:43 2022, max compression
+gzip compressed data, was "accelerate-0.9.0.tar", last modified: Fri May 20 17:47:23 2022, max compression
```

## Comparing `accelerate-0.8.0.tar` & `accelerate-0.9.0.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    11357 2022-02-04 16:53:57.000000 accelerate-0.8.0/LICENSE
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12592 2022-05-12 14:53:43.770580 accelerate-0.8.0/PKG-INFO
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    11587 2022-04-28 14:47:29.000000 accelerate-0.8.0/README.md
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)       57 2022-02-04 16:53:57.000000 accelerate-0.8.0/pyproject.toml
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      404 2022-05-12 14:53:43.770580 accelerate-0.8.0/setup.cfg
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     3515 2022-05-12 14:51:21.000000 accelerate-0.8.0/setup.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.766580 accelerate-0.8.0/src/
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      709 2022-05-12 14:51:28.000000 accelerate-0.8.0/src/accelerate/__init__.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    41643 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/accelerator.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12890 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/big_modeling.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7483 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/checkpointing.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate/commands/
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)        0 2022-02-04 16:53:57.000000 accelerate-0.8.0/src/accelerate/commands/__init__.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1492 2022-03-14 18:57:01.000000 accelerate-0.8.0/src/accelerate/commands/accelerate_cli.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate/commands/config/
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     2757 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/commands/config/__init__.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7085 2022-05-12 14:20:34.000000 accelerate-0.8.0/src/accelerate/commands/config/cluster.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6088 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/commands/config/config_args.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1694 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/commands/config/config_utils.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6265 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/commands/config/sagemaker.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2001 2022-03-14 18:57:01.000000 accelerate-0.8.0/src/accelerate/commands/env.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    19693 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/commands/launch.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     2106 2022-03-08 19:14:40.000000 accelerate-0.8.0/src/accelerate/commands/test.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    26126 2022-03-11 18:31:38.000000 accelerate-0.8.0/src/accelerate/data_loader.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    16234 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/hooks.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7706 2022-03-31 13:27:19.000000 accelerate-0.8.0/src/accelerate/launchers.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2267 2022-05-04 14:00:00.000000 accelerate-0.8.0/src/accelerate/logging.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1087 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/memory_utils.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     5917 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/optimizer.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     3381 2022-04-04 18:51:37.000000 accelerate-0.8.0/src/accelerate/scheduler.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    10000 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/state.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate/test_utils/
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      348 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/test_utils/__init__.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6975 2022-04-28 14:47:29.000000 accelerate-0.8.0/src/accelerate/test_utils/examples.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12993 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/test_utils/test_script.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     8470 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/test_utils/testing.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1610 2022-03-08 19:15:30.000000 accelerate-0.8.0/src/accelerate/test_utils/training.py
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12246 2022-05-04 14:00:00.000000 accelerate-0.8.0/src/accelerate/tracking.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate/utils/
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2101 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/utils/__init__.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)      753 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/constants.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9718 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/dataclasses.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3577 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/deepspeed.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1760 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/imports.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1987 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/launch.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3230 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/memory.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    28006 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/utils/modeling.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5250 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/utils/offload.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)    18444 2022-05-12 14:20:36.000000 accelerate-0.8.0/src/accelerate/utils/operations.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3273 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/other.py
--rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3335 2022-05-05 19:35:13.000000 accelerate-0.8.0/src/accelerate/utils/random.py
-drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-12 14:53:43.770580 accelerate-0.8.0/src/accelerate.egg-info/
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12592 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/PKG-INFO
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1628 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/SOURCES.txt
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)        1 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/dependency_links.txt
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      176 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/entry_points.txt
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      354 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/requires.txt
--rw-rw-r--   0 sgugger   (1000) sgugger   (1000)       11 2022-05-12 14:53:43.000000 accelerate-0.8.0/src/accelerate.egg-info/top_level.txt
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.233775 accelerate-0.9.0/
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    11357 2022-02-04 16:53:57.000000 accelerate-0.9.0/LICENSE
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12592 2022-05-20 17:47:23.233775 accelerate-0.9.0/PKG-INFO
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    11587 2022-04-28 14:47:29.000000 accelerate-0.9.0/README.md
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)       57 2022-02-04 16:53:57.000000 accelerate-0.9.0/pyproject.toml
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      404 2022-05-20 17:47:23.233775 accelerate-0.9.0/setup.cfg
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     3515 2022-05-20 17:45:43.000000 accelerate-0.9.0/setup.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.229775 accelerate-0.9.0/src/
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.229775 accelerate-0.9.0/src/accelerate/
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)      709 2022-05-20 17:45:55.000000 accelerate-0.9.0/src/accelerate/__init__.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    41691 2022-05-19 15:39:25.000000 accelerate-0.9.0/src/accelerate/accelerator.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)    12890 2022-05-12 14:20:36.000000 accelerate-0.9.0/src/accelerate/big_modeling.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7469 2022-05-19 15:39:25.000000 accelerate-0.9.0/src/accelerate/checkpointing.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.233775 accelerate-0.9.0/src/accelerate/commands/
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)        0 2022-02-04 16:53:57.000000 accelerate-0.9.0/src/accelerate/commands/__init__.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1492 2022-03-14 18:57:01.000000 accelerate-0.9.0/src/accelerate/commands/accelerate_cli.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.233775 accelerate-0.9.0/src/accelerate/commands/config/
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     2757 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/commands/config/__init__.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7085 2022-05-12 14:20:34.000000 accelerate-0.9.0/src/accelerate/commands/config/cluster.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6088 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/commands/config/config_args.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1694 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/commands/config/config_utils.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6265 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/commands/config/sagemaker.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2001 2022-03-14 18:57:01.000000 accelerate-0.9.0/src/accelerate/commands/env.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    20262 2022-05-20 14:33:53.000000 accelerate-0.9.0/src/accelerate/commands/launch.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     2106 2022-03-08 19:14:40.000000 accelerate-0.9.0/src/accelerate/commands/test.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    26602 2022-05-20 14:33:53.000000 accelerate-0.9.0/src/accelerate/data_loader.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)    16234 2022-05-12 14:20:36.000000 accelerate-0.9.0/src/accelerate/hooks.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     7708 2022-05-19 15:39:25.000000 accelerate-0.9.0/src/accelerate/launchers.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2267 2022-05-04 14:00:00.000000 accelerate-0.9.0/src/accelerate/logging.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1087 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/memory_utils.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     5917 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/optimizer.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     3381 2022-04-04 18:51:37.000000 accelerate-0.9.0/src/accelerate/scheduler.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    10000 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/state.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.233775 accelerate-0.9.0/src/accelerate/test_utils/
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      348 2022-05-12 14:20:36.000000 accelerate-0.9.0/src/accelerate/test_utils/__init__.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     6975 2022-04-28 14:47:29.000000 accelerate-0.9.0/src/accelerate/test_utils/examples.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12993 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/test_utils/test_script.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     8470 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/test_utils/testing.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     3521 2022-05-20 14:33:53.000000 accelerate-0.9.0/src/accelerate/test_utils/training.py
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12872 2022-05-19 15:39:25.000000 accelerate-0.9.0/src/accelerate/tracking.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.233775 accelerate-0.9.0/src/accelerate/utils/
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2243 2022-05-20 17:37:00.000000 accelerate-0.9.0/src/accelerate/utils/__init__.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)      753 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/constants.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     9718 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/dataclasses.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3577 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/deepspeed.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     2387 2022-05-20 15:10:06.000000 accelerate-0.9.0/src/accelerate/utils/imports.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     1987 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/launch.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3230 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/memory.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)    27108 2022-05-20 17:37:00.000000 accelerate-0.9.0/src/accelerate/utils/modeling.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     6216 2022-05-20 17:37:00.000000 accelerate-0.9.0/src/accelerate/utils/offload.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)    18444 2022-05-12 14:20:36.000000 accelerate-0.9.0/src/accelerate/utils/operations.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     5392 2022-05-19 15:39:25.000000 accelerate-0.9.0/src/accelerate/utils/other.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)     3335 2022-05-05 19:35:13.000000 accelerate-0.9.0/src/accelerate/utils/random.py
+-rw-r--r--   0 sgugger   (1000) sgugger   (1000)      835 2022-05-12 16:15:29.000000 accelerate-0.9.0/src/accelerate/utils/versions.py
+drwxrwxr-x   0 sgugger   (1000) sgugger   (1000)        0 2022-05-20 17:47:23.229775 accelerate-0.9.0/src/accelerate.egg-info/
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)    12592 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/PKG-INFO
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)     1661 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)        1 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      176 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/entry_points.txt
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)      354 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/requires.txt
+-rw-rw-r--   0 sgugger   (1000) sgugger   (1000)       11 2022-05-20 17:47:23.000000 accelerate-0.9.0/src/accelerate.egg-info/top_level.txt
```

### Comparing `accelerate-0.8.0/LICENSE` & `accelerate-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/PKG-INFO` & `accelerate-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelerate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Accelerate
 Home-page: https://github.com/huggingface/accelerate
 Author: The HuggingFace team
 Author-email: sylvain@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: accelerate Version: 0.8.0 Summary: Accelerate Home-
+Metadata-Version: 2.1 Name: accelerate Version: 0.9.0 Summary: Accelerate Home-
 page: https://github.com/huggingface/accelerate Author: The HuggingFace team
 Author-email: sylvain@huggingface.co License: Apache Keywords: deep learning
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `accelerate-0.8.0/README.md` & `accelerate-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/setup.py` & `accelerate-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 extras["sagemaker"] = [
     "sagemaker",  # boto3 is a required package in sagemaker
 ]
 
 setup(
     name="accelerate",
-    version="0.8.0",
+    version="0.9.0",
     description="Accelerate",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning",
     license="Apache",
     author="The HuggingFace team",
     author_email="sylvain@huggingface.co",
```

### Comparing `accelerate-0.8.0/src/accelerate/__init__.py` & `accelerate-0.9.0/src/accelerate/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # flake8: noqa
 # There's no way to ignore "F401 '...' imported but unused" warnings in this
 # module, but to preserve other warnings. So, don't check this module at all.
 
-__version__ = "0.8.0"
+__version__ = "0.9.0"
 
 from .accelerator import Accelerator
 from .big_modeling import cpu_offload, disk_offload, dispatch_model, init_empty_weights, load_checkpoint_and_dispatch
 from .launchers import debug_launcher, notebook_launcher
 from .utils import (
     DeepSpeedPlugin,
     DistributedDataParallelKwargs,
```

### Comparing `accelerate-0.8.0/src/accelerate/accelerator.py` & `accelerate-0.9.0/src/accelerate/accelerator.py`

 * *Files 0% similar despite different names*

```diff
@@ -877,22 +877,23 @@
     def get_state_dict(self, model):
         is_zero_3 = False
         if is_deepspeed_available():
             if isinstance(model, DeepSpeedEngineWrapper) and self.distributed_type == DistributedType.DEEPSPEED:
                 is_zero_3 = self.state.deepspeed_plugin.zero_stage == 3
 
         if is_zero_3:
-            state_dict = model._zero3_consolidated_fp16_state_dict()
+            state_dict = model._zero3_consolidated_16bit_state_dict()
         else:
             model = self.unwrap_model(model)
             state_dict = model.state_dict()
 
-        for k in state_dict:
-            if state_dict[k].dtype == torch.float16:
-                state_dict[k] = state_dict[k].float()
+        if state_dict is not None:
+            for k in state_dict:
+                if state_dict[k].dtype == torch.float16:
+                    state_dict[k] = state_dict[k].float()
 
         return state_dict
 
     def register_for_checkpointing(self, *objects):
         """
         Makes note of `objects` and will save or load them in during `save_state` or `load_state`.
```

### Comparing `accelerate-0.8.0/src/accelerate/big_modeling.py` & `accelerate-0.9.0/src/accelerate/big_modeling.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/checkpointing.py` & `accelerate-0.9.0/src/accelerate/checkpointing.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     states_name = f"{RNG_STATE_NAME}_{process_index}.pkl"
     states["random_state"] = random.getstate()
     states["numpy_random_seed"] = np.random.get_state()
     states["torch_manual_seed"] = torch.get_rng_state()
     states["torch_cuda_manual_seed"] = torch.cuda.get_rng_state_all()
     # ^^ safe to call this function even if cuda is not available
     if is_tpu_available():
-        states["xm_seed"] = torch.tensor(xm.get_rng_state())
+        states["xm_seed"] = xm.get_rng_state()
     output_states_file = os.path.join(output_dir, states_name)
     torch.save(states, output_states_file)
     logger.info(f"Random states saved in {output_states_file}")
     return output_dir
 
 
 def load_accelerator_state(input_dir, models, optimizers, schedulers, process_index, scaler=None):
```

### Comparing `accelerate-0.8.0/src/accelerate/commands/accelerate_cli.py` & `accelerate-0.9.0/src/accelerate/commands/accelerate_cli.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/config/__init__.py` & `accelerate-0.9.0/src/accelerate/commands/config/__init__.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/config/cluster.py` & `accelerate-0.9.0/src/accelerate/commands/config/cluster.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/config/config_args.py` & `accelerate-0.9.0/src/accelerate/commands/config/config_args.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/config/config_utils.py` & `accelerate-0.9.0/src/accelerate/commands/config/config_utils.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/config/sagemaker.py` & `accelerate-0.9.0/src/accelerate/commands/config/sagemaker.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/env.py` & `accelerate-0.9.0/src/accelerate/commands/env.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/commands/launch.py` & `accelerate-0.9.0/src/accelerate/commands/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 from accelerate.utils import (
     ComputeEnvironment,
     DistributedType,
     PrecisionType,
     PrepareForLaunch,
     is_sagemaker_available,
 )
+from accelerate.utils.versions import torch_version
+from packaging import version
 
 
 def launch_command_parser(subparsers=None):
     if subparsers is not None:
         parser = subparsers.add_parser("launch")
     else:
         parser = argparse.ArgumentParser("Accelerate launch command")
@@ -128,14 +130,20 @@
     )
     parser.add_argument(
         "--no_python",
         action="store_true",
         help="Skip prepending the training script with 'python' - just execute it directly. Useful when the script is not a Python script.",
     )
     parser.add_argument(
+        "--num_cpu_threads_per_process",
+        type=int,
+        default=1,
+        help="The number of CPU threads per process. Can be tuned for optimal performance.",
+    )
+    parser.add_argument(
         "--aws_access_key_id",
         type=str,
         default=None,
         help="The AWS_ACCESS_KEY_ID used to launch the Amazon SageMaker training job",
     )
     parser.add_argument(
         "--aws_secret_access_key",
@@ -207,15 +215,20 @@
     process = subprocess.Popen(cmd, env=current_env)
     process.wait()
     if process.returncode != 0:
         raise subprocess.CalledProcessError(returncode=process.returncode, cmd=cmd)
 
 
 def multi_gpu_launcher(args):
-    cmd = [sys.executable, "-m", "torch.distributed.launch", "--use_env"]
+    if torch_version >= version.parse("1.10.0"):
+        cmd = ["torchrun"]
+    elif torch_version >= version.parse("1.9.0"):
+        cmd = [sys.executable, "-m", "torch.distributed.run"]
+    else:
+        cmd = [sys.executable, "-m", "torch.distributed.launch", "--use_env"]
     if args.num_machines > 1:
         cmd.extend(
             [
                 "--nproc_per_node",
                 str(args.num_processes // args.num_machines),
                 "--nnodes",
                 str(args.num_machines),
@@ -255,14 +268,15 @@
 
     current_env["MIXED_PRECISION"] = str(mixed_precision)
     if args.use_fsdp:
         current_env["USE_FSDP"] = "true"
         current_env["FSDP_OFFLOAD_PARAMS"] = str(args.offload_params).lower()
         current_env["FSDP_MIN_NUM_PARAMS"] = str(args.min_num_params)
         current_env["FSDP_SHARDING_STRATEGY"] = str(args.sharding_strategy)
+    current_env["OMP_NUM_THREADS"] = str(args.num_cpu_threads_per_process)
     process = subprocess.Popen(cmd, env=current_env)
     process.wait()
     if process.returncode != 0:
         raise subprocess.CalledProcessError(returncode=process.returncode, cmd=cmd)
 
 
 def deepspeed_launcher(args):
@@ -306,15 +320,15 @@
         warnings.warn('--fp16 flag is deprecated. Use "--mixed_precision fp16" instead.', DeprecationWarning)
         mixed_precision = "fp16"
 
     current_env["MIXED_PRECISION"] = str(mixed_precision)
     current_env["USE_DEEPSPEED"] = "true"
     current_env["DEEPSPEED_ZERO_STAGE"] = str(args.zero_stage)
     current_env["GRADIENT_ACCUMULATION_STEPS"] = str(args.gradient_accumulation_steps)
-    current_env["DEEPSPEED_OFFLOAD_OPTIMIZER_DEVICE"] = str(args.offload_optimizer_device)
+    current_env["DEEPSPEED_OFFLOAD_OPTIMIZER_DEVICE"] = str(args.offload_optimizer_device).lower()
 
     process = subprocess.Popen(cmd, env=current_env)
     process.wait()
     if process.returncode != 0:
         raise subprocess.CalledProcessError(returncode=process.returncode, cmd=cmd)
```

### Comparing `accelerate-0.8.0/src/accelerate/commands/test.py` & `accelerate-0.9.0/src/accelerate/commands/test.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/data_loader.py` & `accelerate-0.9.0/src/accelerate/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,20 +322,29 @@
             otherwise.
 
             Setting this option to `True` requires that the batch size of the `dataloader` is a round multiple of
             `batch_size`.
     """
 
     def __init__(self, dataset, split_batches: bool = False, **kwargs):
+        shuffle = False
+        if version.parse(torch.__version__) >= version.parse("1.11.0"):
+            from torch.utils.data.datapipes.iter.combinatorics import ShufflerIterDataPipe
+
+            # We need to save the shuffling state of the DataPipe
+            if isinstance(dataset, ShufflerIterDataPipe):
+                shuffle = dataset._shuffle_enabled
         super().__init__(dataset, **kwargs)
         self.split_batches = split_batches
         if version.parse(torch.__version__) < version.parse("1.8.0"):
             raise ImportError(
                 "Using `DataLoaderDispatcher` requires PyTorch 1.8.0 minimum. You have {torch.__version__}."
             )
+        if shuffle:
+            torch.utils.data.graph_settings.apply_shuffle_settings(dataset, shuffle=shuffle)
 
     def __iter__(self):
         state = AcceleratorState()
         if state.process_index == 0:
             # We only iterate through the DataLoader on process 0.
             main_iterator = super().__iter__()
         stop_iteration = False
```

### Comparing `accelerate-0.8.0/src/accelerate/hooks.py` & `accelerate-0.9.0/src/accelerate/hooks.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/launchers.py` & `accelerate-0.9.0/src/accelerate/launchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,15 @@
             else:
                 print("Launching training on CPU.")
             function(*args)
 
     else:
         if num_processes is None:
             raise ValueError(
-                "You have to specify the number of GPUs you would like to use, add `num_process=...` to your call."
+                "You have to specify the number of GPUs you would like to use, add `num_processes=...` to your call."
             )
 
         if num_processes > 1:
             # Multi-GPU launch
             if version.parse(torch.__version__) < version.parse("1.5.0"):
                 raise ImportError(
                     "Using `notebook_launcher` for distributed training on GPUs require torch >= 1.5.0, got "
```

### Comparing `accelerate-0.8.0/src/accelerate/logging.py` & `accelerate-0.9.0/src/accelerate/logging.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/memory_utils.py` & `accelerate-0.9.0/src/accelerate/memory_utils.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/optimizer.py` & `accelerate-0.9.0/src/accelerate/optimizer.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/scheduler.py` & `accelerate-0.9.0/src/accelerate/scheduler.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/state.py` & `accelerate-0.9.0/src/accelerate/state.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/test_utils/examples.py` & `accelerate-0.9.0/src/accelerate/test_utils/examples.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/test_utils/test_script.py` & `accelerate-0.9.0/src/accelerate/test_utils/test_script.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/test_utils/testing.py` & `accelerate-0.9.0/src/accelerate/test_utils/testing.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/tracking.py` & `accelerate-0.9.0/src/accelerate/tracking.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,24 +132,27 @@
         logger.info("Stored initial configuration hyperparameters to TensorBoard")
 
     def log(self, values: dict, step: Optional[int] = None):
         """
         Logs `values` to the current run.
 
         Args:
-            values (Dictionary `str` to `str`, `float`, or `int`):
-                Values to be logged as key-value pairs. The values need to have type `str`, `float`, or `int`.
+            values (Dictionary `str` to `str`, `float`, `int` or `dict` of `str` to `float`/`int`):
+                Values to be logged as key-value pairs. The values need to have type `str`, `float`, `int` or `dict` of
+                `str` to `float`/`int`.
             step (`int`, *optional*):
                 The run step. If included, the log will be affiliated with this step.
         """
         for k, v in values.items():
             if isinstance(v, (int, float)):
                 self.writer.add_scalar(k, v, global_step=step)
             elif isinstance(v, str):
                 self.writer.add_text(k, v, global_step=step)
+            elif isinstance(v, dict):
+                self.writer.add_scalars(k, v, global_step=step)
         self.writer.flush()
         logger.info("Successfully logged to TensorBoard")
 
     def finish(self):
         """
         Closes `TensorBoard` writer
         """
@@ -166,15 +169,15 @@
             The name of the experiment run.
     """
 
     requires_logging_directory = False
 
     def __init__(self, run_name: str):
         self.run_name = run_name
-        self.run = wandb.init(self.run_name)
+        self.run = wandb.init(project=self.run_name)
         logger.info(f"Initialized WandB project {self.run_name}")
         logger.info(
             "Make sure to log any initial configurations with `self.store_init_configuration` before training!"
         )
 
     def store_init_configuration(self, values: dict):
         """
@@ -189,16 +192,17 @@
         logger.info("Stored initial configuration hyperparameters to WandB")
 
     def log(self, values: dict, step: Optional[int] = None):
         """
         Logs `values` to the current run.
 
         Args:
-            values (Dictionary `str` to `str`, `float`, or `int`):
-                Values to be logged as key-value pairs. The values need to have type `str`, `float`, or `int`.
+            values (Dictionary `str` to `str`, `float`, `int` or `dict` of `str` to `float`/`int`):
+                Values to be logged as key-value pairs. The values need to have type `str`, `float`, `int` or `dict` of
+                `str` to `float`/`int`.
             step (`int`, *optional*):
                 The run step. If included, the log will be affiliated with this step.
         """
         self.run.log(values, step=step)
         logger.info("Successfully logged to WandB")
 
     def finish(self):
@@ -243,22 +247,29 @@
         logger.info("Stored initial configuration hyperparameters to CometML")
 
     def log(self, values: dict, step: Optional[int] = None):
         """
         Logs `values` to the current run.
 
         Args:
-            values (Dictionary `str` to `str`, `float`, or `int`):
-                Values to be logged as key-value pairs. The values need to have type `str`, `float`, or `int`.
+            values (Dictionary `str` to `str`, `float`, `int` or `dict` of `str` to `float`/`int`):
+                Values to be logged as key-value pairs. The values need to have type `str`, `float`, `int` or `dict` of
+                `str` to `float`/`int`.
             step (`int`, *optional*):
                 The run step. If included, the log will be affiliated with this step.
         """
         if step is not None:
             self.writer.set_step(step)
-        self.writer.log_others(values)
+        for k, v in values.items():
+            if isinstance(v, (int, float)):
+                self.writer.log_metric(k, v, step=step)
+            elif isinstance(v, str):
+                self.writer.log_other(k, v)
+            elif isinstance(v, dict):
+                self.writer.log_metrics(v, step=step)
         logger.info("Successfully logged to CometML")
 
     def finish(self):
         """
         Closes `comet-ml` writer
         """
         self.writer.end()
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/__init__.py` & `accelerate-0.9.0/src/accelerate/utils/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,26 @@
     convert_file_size_to_int,
     dtype_byte_size,
     find_tied_parameters,
     get_max_layer_size,
     get_max_memory,
     infer_auto_device_map,
     load_checkpoint_in_model,
+    load_offloaded_weights,
     named_module_tensors,
     set_module_tensor_to_device,
 )
-from .offload import OffloadedWeightsLoader, PrefixedDataset, extract_submodules_state_dict, offload_state_dict
+from .offload import (
+    OffloadedWeightsLoader,
+    PrefixedDataset,
+    extract_submodules_state_dict,
+    offload_state_dict,
+    offload_weight,
+    save_offload_index,
+)
 from .operations import (
     broadcast,
     broadcast_object_list,
     concatenate,
     convert_outputs_to_fp32,
     convert_to_fp32,
     find_batch_size,
@@ -68,9 +76,16 @@
 
 
 if is_deepspeed_available():
     from .deepspeed import DeepSpeedEngineWrapper, DeepSpeedOptimizerWrapper
 
 from .launch import PrepareForLaunch
 from .memory import find_executable_batch_size
-from .other import extract_model_from_parallel, get_pretty_name, patch_environment, save, wait_for_everyone
+from .other import (
+    extract_model_from_parallel,
+    get_pretty_name,
+    patch_environment,
+    save,
+    wait_for_everyone,
+    write_basic_config,
+)
 from .random import set_seed, synchronize_rng_state, synchronize_rng_states
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/constants.py` & `accelerate-0.9.0/src/accelerate/utils/constants.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/dataclasses.py` & `accelerate-0.9.0/src/accelerate/utils/dataclasses.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/deepspeed.py` & `accelerate-0.9.0/src/accelerate/utils/deepspeed.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/imports.py` & `accelerate-0.9.0/src/accelerate/utils/imports.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,16 +8,23 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 import importlib
+import sys
+
+
+# The package importlib_metadata is in a different place, depending on the Python version.
+if sys.version_info < (3, 8):
+    import importlib_metadata
+else:
+    import importlib.metadata as importlib_metadata
 
 
 try:
     import torch_ccl  # noqa: F401
 
     _ccl_available = True
 except ImportError:
@@ -41,15 +48,23 @@
 
 
 def is_tpu_available():
     return _tpu_available
 
 
 def is_deepspeed_available():
-    return importlib.util.find_spec("deepspeed") is not None
+    package_exists = importlib.util.find_spec("deepspeed") is not None
+    # Check we're not importing a "deepspeed" directory somewhere but the actual library by trying to grab the version
+    # AND checking it has an author field in the metadata that is HuggingFace.
+    if package_exists:
+        try:
+            _ = importlib_metadata.metadata("deepspeed")
+            return True
+        except importlib_metadata.PackageNotFoundError:
+            return False
 
 
 def is_tensorflow_available():
     return importlib.util.find_spec("tensorflow") is not None
 
 
 def is_tensorboard_available():
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/launch.py` & `accelerate-0.9.0/src/accelerate/utils/launch.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/memory.py` & `accelerate-0.9.0/src/accelerate/utils/memory.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/modeling.py` & `accelerate-0.9.0/src/accelerate/utils/modeling.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from collections import defaultdict
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch
 import torch.nn as nn
 
+from .offload import offload_weight, save_offload_index
+
 
 WEIGHTS_INDEX_NAME = "pytorch_model.bin.index.json"
 
 
 def convert_file_size_to_int(size: Union[int, str]):
     """
     Converts a size expressed as a string with digits an unit (like `"5MB"`) to an integer (in bytes).
@@ -308,14 +310,26 @@
     children_modules = set(".".join(k.split(".")[:idx]) for k in children_modules)
     for child in children_modules:
         clean_device_map(device_map, module_name=child)
 
     return device_map
 
 
+def load_offloaded_weights(model, index, offload_folder):
+    if index is None or len(index) == 0:
+        # Nothing to do
+        return
+
+    for param_name, metadata in index.items():
+        tensor_file = os.path.join(offload_folder, f"{param_name}.dat")
+        shape = tuple(metadata["shape"])
+        weight = np.memmap(tensor_file, dtype=metadata["dtype"], mode="r", shape=shape)
+        set_module_tensor_to_device(model, param_name, "cpu", value=torch.tensor(weight))
+
+
 def infer_auto_device_map(
     model: nn.Module,
     max_memory: Optional[Dict[Union[int, str], Union[int, str]]] = None,
     no_split_module_classes: Optional[List[str]] = None,
     dtype: Optional[Union[str, torch.dtype]] = None,
 ):
     """
@@ -577,48 +591,24 @@
                 if module_name == "" and "" not in device_map:
                     # TODO: group all errors and raise at the end.
                     raise ValueError(f"{param_name} doesn't have any device set.")
                 param_device = device_map[module_name]
 
                 if param_device == "disk":
                     set_module_tensor_to_device(model, param_name, "meta")
-                    tensor_file = os.path.join(offload_folder, f"{param_name}.dat")
-                    array = param.numpy()
-                    offload_index[param_name] = {"dtype": str(array.dtype), "shape": list(array.shape)}
-                    file_array = np.memmap(tensor_file, dtype=array.dtype, mode="w+", shape=array.shape)
-                    file_array[:] = array[:]
-                    file_array.flush()
+                    offload_weight(param, param_name, offload_folder, index=offload_index)
                 elif param_device == "cpu" and offload_state_dict:
                     set_module_tensor_to_device(model, param_name, "meta")
-                    tensor_file = os.path.join(state_dict_folder, f"{param_name}.dat")
-                    array = param.numpy()
-                    state_dict_index[param_name] = {"dtype": str(array.dtype), "shape": list(array.shape)}
-                    file_array = np.memmap(tensor_file, dtype=array.dtype, mode="w+", shape=array.shape)
-                    file_array[:] = array[:]
-                    file_array.flush()
+                    offload_weight(param, param_name, state_dict_folder, index=state_dict_index)
                 else:
                     set_module_tensor_to_device(model, param_name, param_device, value=param)
 
         # Force Python to clean up.
         del checkpoint
         gc.collect()
 
-    if len(offload_index) > 0:
-        offload_index_file = os.path.join(offload_folder, "index.json")
-        if os.path.isfile(offload_index_file):
-            with open(offload_index_file, "r", encoding="utf-8") as f:
-                current_offload_index = json.load(f)
-        else:
-            current_offload_index = {}
-        current_offload_index.update(offload_index)
-
-        with open(offload_index_file, "w", encoding="utf-8") as f:
-            json.dump(current_offload_index, f, indent=2)
+    save_offload_index(offload_index, offload_folder)
 
     # Load back offloaded state dict on CPU
-    if offload_state_dict and len(state_dict_index) > 0:
-        for param_name, metadata in state_dict_index.items():
-            tensor_file = os.path.join(state_dict_folder, f"{param_name}.dat")
-            shape = tuple(metadata["shape"])
-            weight = np.memmap(tensor_file, dtype=metadata["dtype"], mode="r", shape=shape)
-            set_module_tensor_to_device(model, param_name, "cpu", value=torch.tensor(weight))
+    if offload_state_dict:
+        load_offloaded_weights(model, state_dict_index, state_dict_folder)
         shutil.rmtree(state_dict_folder)
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/offload.py` & `accelerate-0.9.0/src/accelerate/utils/offload.py`

 * *Files 12% similar despite different names*

```diff
@@ -50,14 +50,42 @@
         current_index = {}
     current_index.update(index)
 
     with open(index_file, "w", encoding="utf-8") as f:
         json.dump(current_index, f, indent=2)
 
 
+def offload_weight(weight, weight_name, offload_folder, index=None):
+    array = weight.numpy()
+    tensor_file = os.path.join(offload_folder, f"{weight_name}.dat")
+    if index is not None:
+        index[weight_name] = {"dtype": str(array.dtype), "shape": list(array.shape)}
+    file_array = np.memmap(tensor_file, dtype=array.dtype, mode="w+", shape=array.shape)
+    file_array[:] = array[:]
+    file_array.flush()
+    return index
+
+
+def save_offload_index(index, offload_folder):
+    if index is None or len(index) == 0:
+        # Nothing to save
+        return
+
+    offload_index_file = os.path.join(offload_folder, "index.json")
+    if os.path.isfile(offload_index_file):
+        with open(offload_index_file, "r", encoding="utf-8") as f:
+            current_index = json.load(f)
+    else:
+        current_index = {}
+    current_index.update(index)
+
+    with open(offload_index_file, "w", encoding="utf-8") as f:
+        json.dump(current_index, f, indent=2)
+
+
 class PrefixedDataset(Mapping):
     """
     Will access keys in a given dataset by adding a prefix.
 
     Args:
         dataset (`Mapping`): Any map with string keys.
         prefix (`str`): A prefix to add when trying to access any element in the underlying dataset.
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/operations.py` & `accelerate-0.9.0/src/accelerate/utils/operations.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate/utils/other.py` & `accelerate-0.9.0/src/accelerate/utils/other.py`

 * *Files 26% similar despite different names*

```diff
@@ -10,17 +10,20 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import os
 from contextlib import contextmanager
+from pathlib import Path
 
 import torch
 
+from ..commands.config.cluster import ClusterConfig
+from ..commands.config.config_args import default_json_config_file
 from ..state import AcceleratorState
 from .dataclasses import DistributedType
 from .imports import is_deepspeed_available, is_tpu_available
 
 
 if is_deepspeed_available():
     from deepspeed import DeepSpeedEngine
@@ -105,7 +108,49 @@
     if not hasattr(obj, "__qualname__") and not hasattr(obj, "__name__"):
         obj = getattr(obj, "__class__", obj)
     if hasattr(obj, "__qualname__"):
         return obj.__qualname__
     if hasattr(obj, "__name__"):
         return obj.__name__
     return str(obj)
+
+
+def write_basic_config(mixed_precision="no", save_location: str = default_json_config_file):
+    """
+    Creates and saves a basic cluster config to be used on a local machine with potentially multiple GPUs. Will also
+    set CPU if it is a CPU-only machine.
+
+    Args:
+        mixed_precision (`str`, *optional*, defaults to "no"):
+            Mixed Precision to use. Should be one of "no", "fp16", or "bf16"
+        save_location (`str`, *optional*, defaults to `default_json_config_file`):
+            Optional custom save location. Should be passed to `--config_file` when using `accelerate launch`. Default
+            location is inside the huggingface cache folder (`~/.cache/huggingface`) but can be overriden by setting
+            the `HF_HOME` environmental variable, followed by `accelerate/default_config.yaml`.
+    """
+    path = Path(save_location)
+    path.parent.mkdir(parents=True, exist_ok=True)
+    if path.exists():
+        print(
+            f"Configuration already exists at {save_location}, will not override. Run `accelerate config` manually or pass a different `save_location`."
+        )
+        return
+    mixed_precision = mixed_precision.lower()
+    if mixed_precision not in ["no", "fp16", "bf16"]:
+        raise ValueError(f"`mixed_precision` should be one of 'no', 'fp16', or 'bf16'. Received {mixed_precision}")
+    config = {"compute_environment": "LOCAL_MACHINE", "mixed_precision": mixed_precision}
+    if torch.cuda.is_available():
+        num_gpus = torch.cuda.device_count()
+        config["num_processes"] = num_gpus
+        config["use_cpu"] = False
+        if num_gpus > 1:
+            config["distributed_type"] = "MULTI_GPU"
+        else:
+            config["distributed_type"] = "NO"
+    else:
+        num_gpus = 0
+        config["use_cpu"] = True
+        config["num_processes"] = 1
+        config["distributed_type"] = "NO"
+    if not path.exists():
+        config = ClusterConfig(**config)
+        config.to_json_file(path)
```

### Comparing `accelerate-0.8.0/src/accelerate/utils/random.py` & `accelerate-0.9.0/src/accelerate/utils/random.py`

 * *Files identical despite different names*

### Comparing `accelerate-0.8.0/src/accelerate.egg-info/PKG-INFO` & `accelerate-0.9.0/src/accelerate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelerate
-Version: 0.8.0
+Version: 0.9.0
 Summary: Accelerate
 Home-page: https://github.com/huggingface/accelerate
 Author: The HuggingFace team
 Author-email: sylvain@huggingface.co
 License: Apache
 Keywords: deep learning
 Platform: UNKNOWN
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: accelerate Version: 0.8.0 Summary: Accelerate Home-
+Metadata-Version: 2.1 Name: accelerate Version: 0.9.0 Summary: Accelerate Home-
 page: https://github.com/huggingface/accelerate Author: The HuggingFace team
 Author-email: sylvain@huggingface.co License: Apache Keywords: deep learning
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers Classifier: Intended Audience ::
 Education Classifier: Intended Audience :: Science/Research Classifier: License
 :: OSI Approved :: Apache Software License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
```

### Comparing `accelerate-0.8.0/src/accelerate.egg-info/SOURCES.txt` & `accelerate-0.9.0/src/accelerate.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -44,8 +44,9 @@
 src/accelerate/utils/imports.py
 src/accelerate/utils/launch.py
 src/accelerate/utils/memory.py
 src/accelerate/utils/modeling.py
 src/accelerate/utils/offload.py
 src/accelerate/utils/operations.py
 src/accelerate/utils/other.py
-src/accelerate/utils/random.py
+src/accelerate/utils/random.py
+src/accelerate/utils/versions.py
```

