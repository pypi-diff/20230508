# Comparing `tmp/ml-starter-0.0.30.tar.gz` & `tmp/ml-starter-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.0.30.tar", last modified: Sun May  7 16:08:04 2023, max compression
+gzip compressed data, was "ml-starter-0.0.31.tar", last modified: Mon May  8 13:15:03 2023, max compression
```

## Comparing `ml-starter-0.0.30.tar` & `ml-starter-0.0.31.tar`

### file list

```diff
@@ -1,154 +1,154 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-07 16:07:51.000000 ml-starter-0.0.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-07 16:07:51.000000 ml-starter-0.0.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 16:08:04.549317 ml-starter-0.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-07 16:07:51.000000 ml-starter-0.0.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.533316 ml-starter-0.0.30/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    33142 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12378 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.537317 ml-starter-0.0.30/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/models/norms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adamw.py
--rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.541317 ml-starter-0.0.30/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/losses/reduce.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.545317 ml-starter-0.0.30/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/grad_clipping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)     8407 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/sl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/trainers/vanilla.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/call_train.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4840 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/torch_distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-07 16:07:51.000000 ml-starter-0.0.30/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 16:08:04.549317 ml-starter-0.0.30/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-07 16:08:04.000000 ml-starter-0.0.30/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-07 16:07:51.000000 ml-starter-0.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 16:07:51.000000 ml-starter-0.0.30/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-07 16:08:04.553317 ml-starter-0.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-07 16:07:51.000000 ml-starter-0.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-08 13:14:46.000000 ml-starter-0.0.31/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-08 13:14:46.000000 ml-starter-0.0.31/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 13:15:03.231423 ml-starter-0.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-08 13:14:46.000000 ml-starter-0.0.31/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.203423 ml-starter-0.0.31/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7423 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24979 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4777 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.207423 ml-starter-0.0.31/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6276 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32373 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12434 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1892 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3398 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11993 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/models/norms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.211423 ml-starter-0.0.31/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3382 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.215423 ml-starter-0.0.31/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.215423 ml-starter-0.0.31/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17884 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9774 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2345 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1431 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      931 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/losses/reduce.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17653 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.219423 ml-starter-0.0.31/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20195 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.223423 ml-starter-0.0.31/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8897 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8654 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/grad_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4419 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7713 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9857 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/sl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11038 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/trainers/vanilla.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.227423 ml-starter-0.0.31/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3295 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/call_train.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5127 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4585 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/torch_distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-05-08 13:14:46.000000 ml-starter-0.0.31/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:15:03.231423 ml-starter-0.0.31/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-08 13:15:03.000000 ml-starter-0.0.31/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-05-08 13:14:46.000000 ml-starter-0.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:14:46.000000 ml-starter-0.0.31/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-08 13:15:03.231423 ml-starter-0.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-08 13:14:46.000000 ml-starter-0.0.31/setup.py
```

### Comparing `ml-starter-0.0.30/LICENSE` & `ml-starter-0.0.31/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/PKG-INFO` & `ml-starter-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.30
+Version: 0.0.31
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.30/README.md` & `ml-starter-0.0.31/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/api.py` & `ml-starter-0.0.31/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/core/config.py` & `ml-starter-0.0.31/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/core/env.py` & `ml-starter-0.0.31/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/core/registry.py` & `ml-starter-0.0.31/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/core/state.py` & `ml-starter-0.0.31/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/launchers/base.py` & `ml-starter-0.0.31/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/launchers/ddp.py` & `ml-starter-0.0.31/ml/launchers/ddp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/launchers/slurm.py` & `ml-starter-0.0.31/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/launchers/torchrun.py` & `ml-starter-0.0.31/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/loggers/base.py` & `ml-starter-0.0.31/ml/loggers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         Args:
             key: The key to log
             value: The value to log
             state: The current log state
             namespace: The namespace to be logged
         """
 
-    def log_audio(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
+    def log_audio(self, key: str, value: Callable[[], tuple[Tensor, int]], state: State, namespace: str) -> None:
         """Logs a normalized audio, with shape (T,).
 
         Args:
             key: The key to log
             value: The value to log
             state: The current log state
             namespace: The namespace to be logged
```

### Comparing `ml-starter-0.0.30/ml/loggers/meter.py` & `ml-starter-0.0.31/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/loggers/multi.py` & `ml-starter-0.0.31/ml/loggers/multi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import functools
+import logging
 import math
 import re
-import warnings
 from collections import defaultdict
 from typing import Any, Callable, Iterator, Sequence, TypeVar
 
 import torch
 import torch.nn.functional as F
 import torchvision.transforms.functional as V
 from PIL import Image, ImageDraw, ImageFont
 from torch import Tensor
 from torchvision.transforms import InterpolationMode
 
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
+from ml.utils.logging import IntervalTicker
+
+logger = logging.getLogger(__name__)
 
 LogT = TypeVar("LogT")
 Number = int | float | Tensor
 
 VALID_VIDEO_CHANNEL_COUNTS = {1, 3}
 VALID_AUDIO_CHANNEL_COUNTS = {1, 2}
 TARGET_FPS = 12
-TARGET_SAMPLE_RATE = 22050
 DEFAULT_NAMESPACE = "value"
 
 
 def _aminmax(t: Tensor) -> tuple[Tensor, Tensor]:
     # `aminmax` isn't supported for MPS tensors, fall back to separate calls.
     minv, maxv = (t.min(), t.max()) if t.is_mps else tuple(t.aminmax())
     return minv, maxv
@@ -171,14 +173,19 @@
         raise ValueError(f"Invalid image shape{'' if log_key is None else f' for {log_key}'}: {images.shape}")
 
     if not keep_resolution:
         images = torch.stack([make_human_viewable_resolution(image) for image in images.unbind(0)], 0)
     return images
 
 
+@functools.lru_cache()
+def audio_warning_ticker() -> IntervalTicker:
+    return IntervalTicker(5.0)
+
+
 def standardize_audio(audio: Tensor, *, log_key: str | None = None) -> Tensor:
     """Converts an arbitrary audio tensor to shape (C, T).
 
     Args:
         audio: The audio tensor to log
         log_key: An optional logging key to use in the exception message
 
@@ -196,17 +203,19 @@
             pass
         elif audio.shape[1] in VALID_AUDIO_CHANNEL_COUNTS:
             audio = audio.permute(1, 0)
         else:
             raise ValueError(f"Invalid channel count{'' if log_key is None else f' for {log_key}'}: {audio.shape}")
     else:
         raise ValueError(f"Invalid audio shape{'' if log_key is None else f' for {log_key}'}: {audio.shape}")
-    if audio.max() > 1.0:
-        warnings.warn("Audio is outside the range [-1, 1]; clipping")
-        audio = audio / audio.max()
+    max_abs = audio.abs().max()
+    if max_abs > 1.0:
+        if audio_warning_ticker().tick():
+            logger.warning("Audio is outside the range [-1, 1]; clipping")
+        audio = audio.clamp_(-5e3, 5e3) / max_abs
     return audio
 
 
 def standardize_video(video: Tensor, *, log_key: str | None = None, normalize: bool = True) -> Tensor:
     """Converts an arbitrary video to shape (T, C, H, W).
 
     Args:
@@ -356,46 +365,14 @@
         frame_ids = torch.linspace(0, pre_frames - 1, post_frames).long()
         return torch.stack([video[i] for i in frame_ids], dim=stack_dim)
 
     frame_ids = torch.linspace(0, pre_frames - 1, post_frames, device=video.device).long()
     return video[frame_ids]
 
 
-def normalize_audio_sample_rate(
-    audio: Tensor,
-    sample_rate: int | None,
-    length: float | None,
-    target_sample_rate: int = TARGET_SAMPLE_RATE,
-) -> Tensor:
-    """Normalizes an audio signal to have a particular sample rate.
-
-    Args:
-        audio: The audio signal to normalize, with shape (T, C)
-        sample_rate: The desired sample rate
-        length: The desired audio length, in seconds, at the target sample rate
-        target_sample_rate: The target sample rate for the logger
-
-    Returns:
-        The normalized audio signal
-    """
-
-    if sample_rate is None and length is None:
-        return audio
-
-    pre_frames = audio.size(0)
-    if sample_rate is None:
-        assert length is not None  # Not used, just for type checker
-        sample_rate = int(pre_frames / length)
-
-    post_frames = int(pre_frames * (target_sample_rate / sample_rate))
-
-    frame_ids = torch.linspace(0, pre_frames - 1, post_frames, device=audio.device).long()
-    return audio[frame_ids]
-
-
 def standardize_point_cloud(value: Tensor, max_points: int, *, log_key: str | None) -> Tensor:
     for i in range(0, value.ndim - 1):
         if value.shape[i] == 3:
             value = value.transpose(i, -1)
             break
     if value.shape[-1] != 3:
         raise ValueError(f"Invalid point cloud shape{'' if log_key is None else f' for {log_key}'}: {value.shape}")
@@ -488,15 +465,15 @@
 class MultiLogger:
     """Defines an intermediate container which holds values to log somewhere else."""
 
     def __init__(self, default_namespace: str = DEFAULT_NAMESPACE) -> None:
         self.scalars: dict[str, dict[str, Callable[[], Number]]] = defaultdict(dict)
         self.strings: dict[str, dict[str, Callable[[], str]]] = defaultdict(dict)
         self.images: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
-        self.audio: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
+        self.audio: dict[str, dict[str, Callable[[], tuple[Tensor, int]]]] = defaultdict(dict)
         self.videos: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.histograms: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.point_clouds: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.poses: dict[str, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.default_namespace = default_namespace
 
     def resolve_namespace(self, namespace: str | None = None) -> str:
@@ -736,20 +713,20 @@
             sample_rate: The sample rate of the audio clip
             length: The maximum length of the audio clip, in seconds
         """
 
         namespace = self.resolve_namespace(namespace)
 
         @functools.lru_cache
-        def audio_future() -> Tensor:
+        def audio_future() -> tuple[Tensor, int]:
             value_concrete = value() if callable(value) else value
             assert isinstance(value_concrete, Tensor)
             audio = standardize_audio(value_concrete, log_key=f"{namespace}/{key}")
             audio = cast_fp32(audio)
-            return normalize_audio_sample_rate(audio, sample_rate, length)
+            return audio, sample_rate
 
         self.audio[namespace][key] = audio_future
 
     def log_video(
         self,
         key: str,
         value: Callable[[], Tensor] | Tensor,
```

### Comparing `ml-starter-0.0.30/ml/loggers/stdout.py` & `ml-starter-0.0.31/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/loggers/tensorboard.py` & `ml-starter-0.0.31/ml/loggers/tensorboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from torch.utils.tensorboard import SummaryWriter
 
 from ml.core.config import conf_field
 from ml.core.env import is_tensorboard_disabled
 from ml.core.registry import register_logger
 from ml.core.state import Phase, State
 from ml.loggers.base import BaseLogger, BaseLoggerConfig
-from ml.loggers.multi import TARGET_FPS, TARGET_SAMPLE_RATE
+from ml.loggers.multi import TARGET_FPS
 from ml.utils.distributed import is_distributed, is_master
 from ml.utils.networking import get_unused_port
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 WRITE_PROC_TEXT_EVERY_N_SECONDS: int = 60 * 2
 
@@ -120,15 +120,15 @@
 class TensorboardLogger(BaseLogger[TensorboardLoggerConfig]):
     def __init__(self, config: TensorboardLoggerConfig) -> None:
         super().__init__(config)
 
         self.scalars: dict[Phase, dict[str, Callable[[], int | float | Tensor]]] = defaultdict(dict)
         self.strings: dict[Phase, dict[str, Callable[[], str]]] = defaultdict(dict)
         self.images: dict[Phase, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
-        self.audio: dict[Phase, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
+        self.audio: dict[Phase, dict[str, Callable[[], tuple[Tensor, int]]]] = defaultdict(dict)
         self.videos: dict[Phase, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.histograms: dict[Phase, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
         self.point_clouds: dict[Phase, dict[str, Callable[[], Tensor]]] = defaultdict(dict)
 
         self.run_config: DictConfig | None = None
         self.logged_run_config = False
 
@@ -236,15 +236,15 @@
 
     def log_string(self, key: str, value: Callable[[], str], state: State, namespace: str) -> None:
         self.strings[state.phase][f"{namespace}/{key}"] = value
 
     def log_image(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
         self.images[state.phase][f"{namespace}/{key}"] = value
 
-    def log_audio(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
+    def log_audio(self, key: str, value: Callable[[], tuple[Tensor, int]], state: State, namespace: str) -> None:
         self.audio[state.phase][f"{namespace}/{key}"] = value
 
     def log_video(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
         self.videos[state.phase][f"{namespace}/{key}"] = value
 
     def log_histogram(self, key: str, value: Callable[[], Tensor], state: State, namespace: str) -> None:
         self.histograms[state.phase][f"{namespace}/{key}"] = value
@@ -265,15 +265,16 @@
         for scalar_key, scalar_value in self.scalars[state.phase].items():
             writer.add_scalar(scalar_key, scalar_value(), global_step=state.num_steps)
         for string_key, string_value in self.strings[state.phase].items():
             writer.add_text(string_key, string_value(), global_step=state.num_steps)
         for image_key, image_value in self.images[state.phase].items():
             writer.add_image(image_key, image_value(), global_step=state.num_steps)
         for audio_key, audio_value in self.audio[state.phase].items():
-            writer.add_audio(audio_key, audio_value(), global_step=state.num_steps, sample_rate=TARGET_SAMPLE_RATE)
+            audio_wav, audio_sample_rate = audio_value()
+            writer.add_audio(audio_key, audio_wav, global_step=state.num_steps, sample_rate=audio_sample_rate)
         for video_key, video_value in self.videos[state.phase].items():
             writer.add_video(video_key, video_value().unsqueeze(0), global_step=state.num_steps, fps=TARGET_FPS)
         for hist_key, hist_value in self.histograms[state.phase].items():
             writer.add_histogram(hist_key, hist_value(), global_step=state.num_steps)
         for pc_key, pc_value_func in self.point_clouds[state.phase].items():
             pc_value = pc_value_func()
             bsz, _, _ = pc_value.shape
```

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/base.py` & `ml-starter-0.0.31/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/cosine.py` & `ml-starter-0.0.31/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.0.31/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/linear.py` & `ml-starter-0.0.31/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.0.31/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.0.31/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/activations.py` & `ml-starter-0.0.31/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/base.py` & `ml-starter-0.0.31/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/embeddings.py` & `ml-starter-0.0.31/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/init.py` & `ml-starter-0.0.31/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/lora.py` & `ml-starter-0.0.31/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/models/norms.py` & `ml-starter-0.0.31/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/adam.py` & `ml-starter-0.0.31/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/adamw.py` & `ml-starter-0.0.31/ml/optimizers/adamw.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/adan.py` & `ml-starter-0.0.31/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/base.py` & `ml-starter-0.0.31/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/sgd.py` & `ml-starter-0.0.31/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/optimizers/shampoo.py` & `ml-starter-0.0.31/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/scripts/cli.py` & `ml-starter-0.0.31/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/scripts/stage.py` & `ml-starter-0.0.31/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/scripts/train.py` & `ml-starter-0.0.31/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/base.py` & `ml-starter-0.0.31/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.0.31/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/clippify.py` & `ml-starter-0.0.31/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/collate.py` & `ml-starter-0.0.31/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/error_handling.py` & `ml-starter-0.0.31/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.0.31/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/samplers.py` & `ml-starter-0.0.31/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/streaming.py` & `ml-starter-0.0.31/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/transforms.py` & `ml-starter-0.0.31/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/utils.py` & `ml-starter-0.0.31/ml/tasks/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/datasets/video_file.py` & `ml-starter-0.0.31/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/environments/base.py` & `ml-starter-0.0.31/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/environments/utils.py` & `ml-starter-0.0.31/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/environments/worker.py` & `ml-starter-0.0.31/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/losses/reduce.py` & `ml-starter-0.0.31/ml/tasks/losses/reduce.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/rl/base.py` & `ml-starter-0.0.31/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/rl/replay.py` & `ml-starter-0.0.31/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/tasks/sl/base.py` & `ml-starter-0.0.31/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/base.py` & `ml-starter-0.0.31/ml/trainers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.0.31/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.0.31/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/grad_clipping.py` & `ml-starter-0.0.31/ml/trainers/mixins/grad_clipping.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 @dataclass
 class GradientClipping:
     clip_grad_norm: float | None = conf_field(None, help="What to clip the gradient norm to")
     norm_type: Any = conf_field(2, help="Type of norm to use")
     clip_grad_value: float | None = conf_field(None, help="What to clip the gradient value to")
     clip_global_grad_norm: float | None = conf_field(None, help="What to clip global gradient norm to")
     global_norm_type: Any = conf_field(2, help="Type of global norm to use")
+    log_grad: bool = conf_field(False, help="Whether to log the gradient norm")
 
 
 @dataclass
 class GradientClippingConfig(MixedPrecisionTrainerConfig, BaseTrainerConfig):
     grad_clipping: GradientClipping = conf_field(GradientClipping(), help="Gradient clipping configuration")
 
 
@@ -69,7 +70,15 @@
             self.unscale_mixed_precision(optim)
             total_norm = nn.utils.clip_grad.clip_grad_norm_(
                 model.parameters(),
                 max_norm=clip_norm,
                 norm_type=self.config.grad_clipping.global_norm_type,
             )
             self.logger.log_scalar("total_norm", total_norm.item(), namespace="optim")
+        if self.config.grad_clipping.log_grad:
+            self.unscale_mixed_precision(optim)
+            total_grad = sum(
+                param.grad.norm(self.config.grad_clipping.norm_type) ** 2
+                for param in model.parameters()
+                if param.grad is not None
+            )
+            self.logger.log_scalar("total_grad", total_grad.item(), namespace="optim")
```

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.0.31/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.0.31/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.0.31/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/profiler.py` & `ml-starter-0.0.31/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.0.31/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/rl.py` & `ml-starter-0.0.31/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/trainers/sl.py` & `ml-starter-0.0.31/ml/trainers/sl.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 """Defines a trainer to use for supervised learning.
 
 This trainer is akin to PyTorch Lightning or Keras, in that it handles
 the training loop, logging, and checkpointing. We get a dataset and dataloader
 from the task, and then train the model on the dataset.
 """
 
+import bisect
 import contextlib
+import functools
+import itertools
 import logging
 import signal
 from dataclasses import dataclass
 from types import FrameType
 from typing import Generic, Iterator, TypeVar
 
+from omegaconf import MISSING
+
 from ml.core.common_types import Batch
 from ml.core.config import conf_field
 from ml.core.registry import register_trainer
+from ml.core.state import State
 from ml.lr_schedulers.base import BaseLRScheduler
 from ml.optimizers.base import BaseOptimizer
 from ml.tasks.sl.base import SupervisedLearningTask
 from ml.trainers.base import ModelT
 from ml.trainers.vanilla import TrainingFinishedException, VanillaTrainer, VanillaTrainerConfig
 from ml.utils.device.base import InfinitePrefetcher
 from ml.utils.timer import Timer
@@ -33,28 +39,55 @@
 @dataclass
 class ValidationConfig:
     valid_every_n_steps: int | None = conf_field(100, help="Number of training steps to run per test step")
     num_init_valid_steps: int | None = conf_field(1, help="Number of initial validation steps")
 
 
 @dataclass
+class BatchScheduleConfig:
+    num_steps: int = conf_field(MISSING, help="Number of steps to run for")
+    num_batches: int = conf_field(MISSING, help="Number of minibatches for a given step")
+
+
+@dataclass
 class SupervisedLearningTrainerConfig(VanillaTrainerConfig):
     validation: ValidationConfig = conf_field(ValidationConfig())
     batches_per_step: int = conf_field(1, help="Batches per training step, to simulate larger effective batch sizes")
+    batches_per_step_schedule: list[BatchScheduleConfig] | None = conf_field(
+        None,
+        help="A schedule for the number of minibatches per step, as a list of (step_count, num_batches) tuples.",
+    )
 
 
 SupervisedLearningTrainerConfigT = TypeVar("SupervisedLearningTrainerConfigT", bound=SupervisedLearningTrainerConfig)
 SupervisedLearningTaskT = TypeVar("SupervisedLearningTaskT", bound=SupervisedLearningTask)
 
 
 @register_trainer("sl", SupervisedLearningTrainerConfig)
 class SupervisedLearningTrainer(
     VanillaTrainer[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
     Generic[SupervisedLearningTrainerConfigT, ModelT, SupervisedLearningTaskT],
 ):
+    @functools.lru_cache()
+    def batches_per_step_schedule(self) -> list[tuple[int, int]] | None:
+        schedule = self.config.batches_per_step_schedule
+        if schedule is None:
+            return None
+        if any(s.num_steps <= 0 or s.num_batches <= 0 for s in schedule):
+            raise ValueError("steps and num_batches must be non-negative")
+        schedule_list = [(s.num_steps, s.num_batches) for s in schedule]
+        schedule_cumsum = list(itertools.accumulate([0] + [s[0] for s in schedule_list]))
+        return list(zip(schedule_cumsum[1:], [s[1] for s in schedule_list]))
+
+    def get_batches_per_step(self, state: State) -> int:
+        if (schedule := self.batches_per_step_schedule()) is not None:
+            i = bisect.bisect_left(schedule, (state.num_steps, 0))
+            return schedule[-1][1] if i == len(schedule) else schedule[i][1]
+        return self.config.batches_per_step
+
     def train(
         self,
         model: ModelT,
         task: SupervisedLearningTaskT,
         optimizer: BaseOptimizer,
         lr_scheduler: BaseLRScheduler,
     ) -> None:
@@ -151,15 +184,15 @@
 
                             def batch_iterator() -> Iterator[Batch]:
                                 try:
                                     yield next(train_pf_iter)
                                 except StopIteration:
                                     raise EpochDoneException
 
-                                for _ in range(self.config.batches_per_step - 1):
+                                for _ in range(self.get_batches_per_step(state) - 1):
                                     try:
                                         yield next(train_pf_iter)
                                     except StopIteration:
                                         pass
 
                             loss_dict = self.train_step(
                                 task_model=task_model,
```

### Comparing `ml-starter-0.0.30/ml/trainers/vanilla.py` & `ml-starter-0.0.31/ml/trainers/vanilla.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/argparse.py` & `ml-starter-0.0.31/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/atomic.py` & `ml-starter-0.0.31/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/augmentation.py` & `ml-starter-0.0.31/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/caching.py` & `ml-starter-0.0.31/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/call_train.py` & `ml-starter-0.0.31/ml/utils/call_train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/cli.py` & `ml-starter-0.0.31/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/colors.py` & `ml-starter-0.0.31/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/data.py` & `ml-starter-0.0.31/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/datetime.py` & `ml-starter-0.0.31/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/device/auto.py` & `ml-starter-0.0.31/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/device/base.py` & `ml-starter-0.0.31/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/device/cpu.py` & `ml-starter-0.0.31/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/device/gpu.py` & `ml-starter-0.0.31/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/device/metal.py` & `ml-starter-0.0.31/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/distributed.py` & `ml-starter-0.0.31/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/image.py` & `ml-starter-0.0.31/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/io.py` & `ml-starter-0.0.31/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/large_models.py` & `ml-starter-0.0.31/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/logging.py` & `ml-starter-0.0.31/ml/utils/logging.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 import math
 import sys
+import time
 
 from ml.core.env import is_debugging
 from ml.utils.colors import Color, colorize, get_colorize_parts
 
 # Logging level to show on all ranks.
 INFOALL: int = logging.INFO + 1
 
@@ -121,7 +122,20 @@
     handler.addFilter(RankFilter(rank=rank))
     root_logger.addHandler(handler)
     root_logger.setLevel(logging.DEBUG if is_debugging() else logging.INFO)
 
     # Avoid junk logs from other libraries.
     logging.getLogger("matplotlib").setLevel(logging.WARNING)
     logging.getLogger("PIL").setLevel(logging.WARNING)
+
+
+class IntervalTicker:
+    def __init__(self, interval: float) -> None:
+        self.interval = interval
+        self.last_tick_time: float | None = None
+
+    def tick(self) -> bool:
+        tick_time = time.time()
+        if self.last_tick_time is None or tick_time - self.last_tick_time > self.interval:
+            self.last_tick_time = tick_time
+            return True
+        return False
```

### Comparing `ml-starter-0.0.30/ml/utils/meter.py` & `ml-starter-0.0.31/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/staging.py` & `ml-starter-0.0.31/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/timer.py` & `ml-starter-0.0.31/ml/utils/timer.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,17 +63,17 @@
     def close(self) -> None:
         self.stop()
         self._spinner_close = True
         self._thread.join()
 
     def _spinner(self) -> None:
         chars = [colorize(c, "light-yellow") for c in ("|", "/", "-", "\\")]
+        max_line_len = 0
         while not self._spinner_close:
             self._flag.wait()
-            max_line_len = 0
             start_time = time.time()
             while not self._spinner_stop:
                 for char in chars:
                     elapsed_secs = time.time() - start_time
                     line = f"[ {char} {elapsed_secs:.1f} ] {self._text}\r"
                     max_line_len = max(max_line_len, len(line))
                     sys.stderr.write(line)
```

### Comparing `ml-starter-0.0.30/ml/utils/torch_distributed.py` & `ml-starter-0.0.31/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml/utils/video.py` & `ml-starter-0.0.31/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.0.31/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.0.30
+Version: 0.0.31
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.0.30/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.0.31/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/pyproject.toml` & `ml-starter-0.0.31/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.0.30/setup.py` & `ml-starter-0.0.31/setup.py`

 * *Files identical despite different names*

