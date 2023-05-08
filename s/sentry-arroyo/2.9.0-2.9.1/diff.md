# Comparing `tmp/sentry-arroyo-2.9.0.tar.gz` & `tmp/sentry-arroyo-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry-arroyo-2.9.0.tar", last modified: Wed Apr  5 23:45:18 2023, max compression
+gzip compressed data, was "sentry-arroyo-2.9.1.tar", last modified: Thu Apr  6 02:59:07 2023, max compression
```

## Comparing `sentry-arroyo-2.9.0.tar` & `sentry-arroyo-2.9.1.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.592254 sentry-arroyo-2.9.0/arroyo/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.592254 sentry-arroyo-2.9.0/arroyo/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/backends/kafka/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/kafka/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/kafka/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    26979 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/kafka/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/backends/local/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/local/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/backends/local/storages/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/local/storages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/local/storages/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/backends/local/storages/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/codecs/avro.py
--rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/codecs/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/codecs/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/dlq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/processing/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/processing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/batching.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/commit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.596254 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/dead_letter_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/invalid_messages.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/count.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/ignore.py
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/produce.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/raise_e.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/produce.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task_in_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task_with_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/processing/strategies/unfold.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/arroyo/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/codecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/arroyo/utils/retries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.592254 sentry-arroyo-2.9.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/examples/transform_and_produce/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/examples/transform_and_produce/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/examples/transform_and_produce/batched.py
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/examples/transform_and_produce/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/examples/transform_and_produce/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-05 23:45:18.000000 sentry-arroyo-2.9.0/sentry_arroyo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.592254 sentry-arroyo-2.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/backends/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/backends/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/backends/test_kafka.py
--rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/backends/test_local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.600254 sentry-arroyo-2.9.0/tests/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/codecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/codecs/test_codecs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/tests/processing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/tests/processing/strategies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_batching.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_commit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_dead_letter_queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_produce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task_in_threads.py
--rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task_with_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/strategies/test_unfold.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/processing/test_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:18.604254 sentry-arroyo-2.9.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/utils/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/utils/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-05 23:45:16.000000 sentry-arroyo-2.9.0/tests/utils/test_retries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.938567 sentry-arroyo-2.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10829 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-06 02:59:07.938567 sentry-arroyo-2.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/backends/kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/kafka/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3552 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/kafka/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26979 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/kafka/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/backends/local/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13799 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/local/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/backends/local/storages/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/local/storages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/local/storages/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/backends/local/storages/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/codecs/avro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/codecs/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/codecs/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6947 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/dlq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.930567 sentry-arroyo-2.9.1/arroyo/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12376 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/arroyo/processing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4578 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/commit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2216 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/dead_letter_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/invalid_messages.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/count.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/produce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/raise_e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/produce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task_in_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19487 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task_with_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/processing/strategies/unfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4545 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/arroyo/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3445 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/arroyo/utils/retries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.926567 sentry-arroyo-2.9.1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/examples/transform_and_produce/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/examples/transform_and_produce/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/examples/transform_and_produce/batched.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/examples/transform_and_produce/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/examples/transform_and_produce/simple.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-06 02:59:07.000000 sentry-arroyo-2.9.1/sentry_arroyo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 02:59:07.938567 sentry-arroyo-2.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.926567 sentry-arroyo-2.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/backends/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/backends/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8177 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/backends/test_kafka.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/backends/test_local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/tests/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/codecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/codecs/test_codecs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.934567 sentry-arroyo-2.9.1/tests/processing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.938567 sentry-arroyo-2.9.1/tests/processing/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_batching.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12245 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_dead_letter_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_produce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task_in_threads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11156 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task_with_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/strategies/test_unfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/processing/test_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:07.938567 sentry-arroyo-2.9.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/utils/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/utils/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-06 02:59:03.000000 sentry-arroyo-2.9.1/tests/utils/test_retries.py
```

### Comparing `sentry-arroyo-2.9.0/LICENSE` & `sentry-arroyo-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/PKG-INFO` & `sentry-arroyo-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-arroyo
-Version: 2.9.0
+Version: 2.9.1
 Summary: Arroyo is a Python library for working with streaming data.
 Home-page: https://github.com/getsentry/arroyo
 Author: Sentry
 Author-email: oss@sentry.io
 License: Apache-2.0
 Description: # Arroyo
```

### Comparing `sentry-arroyo-2.9.0/README.md` & `sentry-arroyo-2.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/abstract.py` & `sentry-arroyo-2.9.1/arroyo/backends/abstract.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/kafka/commit.py` & `sentry-arroyo-2.9.1/arroyo/backends/kafka/commit.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/kafka/configuration.py` & `sentry-arroyo-2.9.1/arroyo/backends/kafka/configuration.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/kafka/consumer.py` & `sentry-arroyo-2.9.1/arroyo/backends/kafka/consumer.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/local/backend.py` & `sentry-arroyo-2.9.1/arroyo/backends/local/backend.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/local/storages/abstract.py` & `sentry-arroyo-2.9.1/arroyo/backends/local/storages/abstract.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/backends/local/storages/memory.py` & `sentry-arroyo-2.9.1/arroyo/backends/local/storages/memory.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/codecs/__init__.py` & `sentry-arroyo-2.9.1/arroyo/codecs/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/codecs/avro.py` & `sentry-arroyo-2.9.1/arroyo/codecs/avro.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/codecs/json.py` & `sentry-arroyo-2.9.1/arroyo/codecs/json.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/codecs/msgpack.py` & `sentry-arroyo-2.9.1/arroyo/codecs/msgpack.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/commit.py` & `sentry-arroyo-2.9.1/arroyo/commit.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/dlq.py` & `sentry-arroyo-2.9.1/arroyo/dlq.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/errors.py` & `sentry-arroyo-2.9.1/arroyo/errors.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/processor.py` & `sentry-arroyo-2.9.1/arroyo/processing/processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -254,17 +254,15 @@
                     # accepted, at which point we can resume consuming.
                     if not message_carried_over:
                         logger.debug(
                             "Caught %r while submitting %r, pausing consumer...",
                             e,
                             self.__message,
                         )
-
-                        if self.__paused_timestamp is None:
-                            self.__consumer.pause([*self.__consumer.tell().keys()])
+                        self.__consumer.pause([*self.__consumer.tell().keys()])
 
                         self.__paused_timestamp = time.time()
                     else:
                         current_time = time.time()
                         if self.__paused_timestamp:
                             self.__metrics_buffer.increment(
                                 ConsumerTiming.CONSUMER_PAUSED_TIME,
```

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/__init__.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/abstract.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/abstract.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/batching.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/batching.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/commit.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/commit.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/__init__.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/dead_letter_queue.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/invalid_messages.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/invalid_messages.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/abstract.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/abstract.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/count.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/count.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/ignore.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/ignore.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/produce.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/produce.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/dead_letter_queue/policies/raise_e.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/dead_letter_queue/policies/raise_e.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/decoder.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/decoder.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/filter.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/filter.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/produce.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/produce.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/reduce.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/reduce.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task_in_threads.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task_in_threads.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/run_task_with_multiprocessing.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/run_task_with_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/transform.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/transform.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/processing/strategies/unfold.py` & `sentry-arroyo-2.9.1/arroyo/processing/strategies/unfold.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/types.py` & `sentry-arroyo-2.9.1/arroyo/types.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/clock.py` & `sentry-arroyo-2.9.1/arroyo/utils/clock.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/codecs.py` & `sentry-arroyo-2.9.1/arroyo/utils/codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/concurrent.py` & `sentry-arroyo-2.9.1/arroyo/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/metrics.py` & `sentry-arroyo-2.9.1/arroyo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/profiler.py` & `sentry-arroyo-2.9.1/arroyo/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/arroyo/utils/retries.py` & `sentry-arroyo-2.9.1/arroyo/utils/retries.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/examples/transform_and_produce/batched.py` & `sentry-arroyo-2.9.1/examples/transform_and_produce/batched.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/examples/transform_and_produce/script.py` & `sentry-arroyo-2.9.1/examples/transform_and_produce/script.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/examples/transform_and_produce/simple.py` & `sentry-arroyo-2.9.1/examples/transform_and_produce/simple.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/sentry_arroyo.egg-info/PKG-INFO` & `sentry-arroyo-2.9.1/sentry_arroyo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-arroyo
-Version: 2.9.0
+Version: 2.9.1
 Summary: Arroyo is a Python library for working with streaming data.
 Home-page: https://github.com/getsentry/arroyo
 Author: Sentry
 Author-email: oss@sentry.io
 License: Apache-2.0
 Description: # Arroyo
```

### Comparing `sentry-arroyo-2.9.0/sentry_arroyo.egg-info/SOURCES.txt` & `sentry-arroyo-2.9.1/sentry_arroyo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/setup.py` & `sentry-arroyo-2.9.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def get_requirements() -> Sequence[str]:
     with open("requirements.txt") as fp:
         return [x.strip() for x in fp if not x.startswith("#")]
 
 
 setup(
     name="sentry-arroyo",
-    version="2.9.0",
+    version="2.9.1",
     author="Sentry",
     author_email="oss@sentry.io",
     license="Apache-2.0",
     url="https://github.com/getsentry/arroyo",
     description="Arroyo is a Python library for working with streaming data.",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `sentry-arroyo-2.9.0/tests/backends/mixins.py` & `sentry-arroyo-2.9.1/tests/backends/mixins.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/backends/test_kafka.py` & `sentry-arroyo-2.9.1/tests/backends/test_kafka.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/backends/test_local.py` & `sentry-arroyo-2.9.1/tests/backends/test_local.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/codecs/test_codecs.py` & `sentry-arroyo-2.9.1/tests/codecs/test_codecs.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_batching.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_batching.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_dead_letter_queue.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_dead_letter_queue.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_decoder.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_decoder.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_filter.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_filter.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_produce.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_produce.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_reduce.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_reduce.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task_in_threads.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task_in_threads.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_run_task_with_multiprocessing.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_run_task_with_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_transform.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_transform.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/strategies/test_unfold.py` & `sentry-arroyo-2.9.1/tests/processing/strategies/test_unfold.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/processing/test_processor.py` & `sentry-arroyo-2.9.1/tests/processing/test_processor.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/utils/test_metrics.py` & `sentry-arroyo-2.9.1/tests/utils/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry-arroyo-2.9.0/tests/utils/test_retries.py` & `sentry-arroyo-2.9.1/tests/utils/test_retries.py`

 * *Files identical despite different names*

