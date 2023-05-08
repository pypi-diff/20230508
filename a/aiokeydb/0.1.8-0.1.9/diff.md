# Comparing `tmp/aiokeydb-0.1.8.tar.gz` & `tmp/aiokeydb-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiokeydb-0.1.8.tar", last modified: Tue Feb  7 15:52:21 2023, max compression
+gzip compressed data, was "aiokeydb-0.1.9.tar", last modified: Tue Feb  7 23:15:16 2023, max compression
```

## Comparing `aiokeydb-0.1.8.tar` & `aiokeydb-0.1.9.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.381413 aiokeydb-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.365412 aiokeydb-0.1.8/aiokeydb/
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.369413 aiokeydb-0.1.8/aiokeydb/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    56165 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    67205 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    53418 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/backoff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.369413 aiokeydb-0.1.8/aiokeydb/client/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15984 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)   108477 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.369413 aiokeydb-0.1.8/aiokeydb/client/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    98860 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/schemas/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.369413 aiokeydb-0.1.8/aiokeydb/client/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/serializers/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/serializers/_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/serializers/_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/client/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    83429 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.373413 aiokeydb-0.1.8/aiokeydb/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.373413 aiokeydb-0.1.8/aiokeydb/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   213069 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.373413 aiokeydb-0.1.8/aiokeydb/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.373413 aiokeydb-0.1.8/aiokeydb/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/aiokeydb/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35449 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/aiokeydb/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33444 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61725 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/connection.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57971 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/ocsp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/parsers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/aiokeydb/queues/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/aiokeydb/queues/imports/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/imports/cron.py
--rw-r--r--   0 runner    (1001) docker     (123)    39056 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/aiokeydb/queues/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27717 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/queues/worker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/aiokeydb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.369413 aiokeydb-0.1.8/aiokeydb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-02-07 15:52:21.000000 aiokeydb-0.1.8/aiokeydb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-02-07 15:52:21.000000 aiokeydb-0.1.8/aiokeydb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 15:52:21.000000 aiokeydb-0.1.8/aiokeydb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-07 15:52:21.000000 aiokeydb-0.1.8/aiokeydb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 15:52:21.000000 aiokeydb-0.1.8/aiokeydb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 15:52:21.381413 aiokeydb-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 15:52:21.377413 aiokeydb-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/tests/test_keydb.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/tests/test_multi_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/tests/test_suite.py
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-07 15:52:07.000000 aiokeydb-0.1.8/tests/test_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.717134 aiokeydb-0.1.9/aiokeydb/
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.721134 aiokeydb-0.1.9/aiokeydb/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56165 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67205 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53418 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11695 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/backoff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.721134 aiokeydb-0.1.9/aiokeydb/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16343 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)   108475 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.721134 aiokeydb-0.1.9/aiokeydb/client/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98860 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/schemas/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.721134 aiokeydb-0.1.9/aiokeydb/client/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3936 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/serializers/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/serializers/_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/serializers/_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13736 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83429 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.721134 aiokeydb-0.1.9/aiokeydb/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.725134 aiokeydb-0.1.9/aiokeydb/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18389 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   213069 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.725134 aiokeydb-0.1.9/aiokeydb/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17127 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.725134 aiokeydb-0.1.9/aiokeydb/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4443 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14110 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6525 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.725134 aiokeydb-0.1.9/aiokeydb/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9914 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35449 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10275 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/aiokeydb/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33444 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61725 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/connection.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57971 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11574 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11454 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20032 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/parsers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/aiokeydb/queues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/aiokeydb/queues/imports/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/imports/cron.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39056 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13313 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/aiokeydb/queues/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27717 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/queues/worker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/aiokeydb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.717134 aiokeydb-0.1.9/aiokeydb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11051 2023-02-07 23:15:16.000000 aiokeydb-0.1.9/aiokeydb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-02-07 23:15:16.000000 aiokeydb-0.1.9/aiokeydb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 23:15:16.000000 aiokeydb-0.1.9/aiokeydb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-02-07 23:15:16.000000 aiokeydb-0.1.9/aiokeydb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-07 23:15:16.000000 aiokeydb-0.1.9/aiokeydb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 23:15:16.729134 aiokeydb-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/tests/test_keydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/tests/test_multi_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4583 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/tests/test_suite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-02-07 23:15:06.000000 aiokeydb-0.1.9/tests/test_task_queue.py
```

### Comparing `aiokeydb-0.1.8/PKG-INFO` & `aiokeydb-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokeydb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for KeyDB database and key-value store
 Home-page: https://github.com/trisongz/aiokeydb-py
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiokeydb-0.1.8/README.md` & `aiokeydb-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/__init__.py` & `aiokeydb-0.1.9/aiokeydb/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/__init__.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/client.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/cluster.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/connection.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/connection.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/core.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/core.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/lock.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/parser.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/parser.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/retry.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/sentinel.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/asyncio/utils.py` & `aiokeydb-0.1.9/aiokeydb/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/backoff.py` & `aiokeydb-0.1.9/aiokeydb/backoff.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/__init__.py` & `aiokeydb-0.1.9/aiokeydb/client/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/config.py` & `aiokeydb-0.1.9/aiokeydb/client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -433,18 +433,18 @@
         ssl: Optional[bool] = None,
         cache_ttl: Optional[int] = None,
         cache_prefix: Optional[str] = None,
         cache_enabled: Optional[bool] = None,
         worker_enabled: Optional[bool] = None,
         serializer: Optional[SerializerType] = None,
         db_mapping: Optional[Union[str, Dict[str, int]]] = None,
-        socket_timeout: Optional[float] = None,
-        socket_connect_timeout: Optional[float] = None,
+        socket_timeout: Optional[float] = -1.0,
+        socket_connect_timeout: Optional[float] = -1.0,
+        connection_timeout: Optional[int] = -1,
         socket_keepalive: Optional[bool] = None,
-        connection_timeout: Optional[int] = None,
         encoding: Optional[str] = None,
         encoding_errors: Optional[str] = None,
         config_kwargs: Optional[Union[str, Dict[str, Any]]] = None,
         log_level: Optional[str] = None,
         debug_enabled: Optional[bool] = None,
         queue_db: Optional[int] = None,
         **kwargs,
@@ -461,18 +461,23 @@
         if ssl is not None: self.ssl = ssl
         if cache_ttl is not None: self.cache_ttl = cache_ttl
         if cache_prefix is not None: self.cache_prefix = cache_prefix
         if cache_enabled is not None: self.cache_enabled = cache_enabled
         if worker_enabled is not None: self.worker_enabled = worker_enabled
         if serializer is not None: self.serializer = serializer
         if db_mapping is not None: self.db_mapping = db_mapping
-        if socket_timeout is not None: self.socket_timeout = socket_timeout
-        if socket_connect_timeout is not None: self.socket_connect_timeout = socket_connect_timeout
+        # if socket_timeout is not None: self.socket_timeout = socket_timeout
+        # if socket_connect_timeout is not None: self.socket_connect_timeout = socket_connect_timeout
+        # if connection_timeout is not None: self.connection_timeout = connection_timeout
+        
+        if socket_timeout is None or socket_timeout >= 0.0: self.socket_timeout = socket_timeout
+        if socket_connect_timeout is None or socket_connect_timeout >= 0.0: self.socket_connect_timeout = socket_connect_timeout
+        if connection_timeout is None or connection_timeout >= 0: self.connection_timeout = connection_timeout
+        
         if socket_keepalive is not None: self.socket_keepalive = socket_keepalive
-        if connection_timeout is not None: self.connection_timeout = connection_timeout
         if encoding is not None: self.encoding = encoding
         if encoding_errors is not None: self.encoding_errors = encoding_errors
         if config_kwargs is not None: self.config_kwargs = config_kwargs
         if debug_enabled is not None: self.debug_enabled = debug_enabled
         if log_level is not None: self.log_level = log_level
 
         if kwargs or queue_db is not None:
```

### Comparing `aiokeydb-0.1.8/aiokeydb/client/core.py` & `aiokeydb-0.1.9/aiokeydb/client/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,18 +36,18 @@
         ssl: typing.Optional[bool] = None,
         cache_ttl: typing.Optional[int] = None,
         cache_prefix: typing.Optional[str] = None,
         cache_enabled: typing.Optional[bool] = None,
         worker_enabled: typing.Optional[bool] = None,
         serializer: typing.Optional[SerializerType] = None,
         db_mapping: typing.Optional[typing.Union[str, typing.Dict[str, int]]] = None,
-        socket_timeout: typing.Optional[float] = None,
-        socket_connect_timeout: typing.Optional[float] = None,
+        socket_timeout: typing.Optional[float] = -1.0,
+        socket_connect_timeout: typing.Optional[float] = -1.0,
+        connection_timeout: typing.Optional[int] = -1,
         socket_keepalive: typing.Optional[bool] = None,
-        connection_timeout: typing.Optional[int] = None,
         encoding: typing.Optional[str] = None,
         encoding_errors: typing.Optional[str] = None,
         config_kwargs: typing.Optional[typing.Union[str, typing.Dict[str, typing.Any]]] = None,
         debug_enabled: typing.Optional[bool] = None,
         log_level: typing.Optional[str] = None,
         queue_db: typing.Optional[int] = None,
         overwrite: typing.Optional[bool] = None,
```

### Comparing `aiokeydb-0.1.8/aiokeydb/client/schemas/session.py` & `aiokeydb-0.1.9/aiokeydb/client/schemas/session.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/serializers/__init__.py` & `aiokeydb-0.1.9/aiokeydb/client/serializers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/serializers/_json.py` & `aiokeydb-0.1.9/aiokeydb/client/serializers/_json.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/serializers/_msgpack.py` & `aiokeydb-0.1.9/aiokeydb/client/serializers/_msgpack.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/serializers/_pickle.py` & `aiokeydb-0.1.9/aiokeydb/client/serializers/_pickle.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/types.py` & `aiokeydb-0.1.9/aiokeydb/client/types.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/client/utils.py` & `aiokeydb-0.1.9/aiokeydb/client/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/cluster.py` & `aiokeydb-0.1.9/aiokeydb/cluster.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/bf/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/bf/commands.py` & `aiokeydb-0.1.9/aiokeydb/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/bf/info.py` & `aiokeydb-0.1.9/aiokeydb/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/cluster.py` & `aiokeydb-0.1.9/aiokeydb/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/core.py` & `aiokeydb-0.1.9/aiokeydb/commands/core.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/commands.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/edge.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/execution_plan.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/node.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/path.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/graph/query_result.py` & `aiokeydb-0.1.9/aiokeydb/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/helpers.py` & `aiokeydb-0.1.9/aiokeydb/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/json/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/json/commands.py` & `aiokeydb-0.1.9/aiokeydb/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/json/decoders.py` & `aiokeydb-0.1.9/aiokeydb/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/parser.py` & `aiokeydb-0.1.9/aiokeydb/commands/parser.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/redismodules.py` & `aiokeydb-0.1.9/aiokeydb/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/aggregation.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/commands.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/commands.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/field.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/indexDefinition.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/query.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/querystring.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/reducers.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/result.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/search/suggestion.py` & `aiokeydb-0.1.9/aiokeydb/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/sentinel.py` & `aiokeydb-0.1.9/aiokeydb/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/timeseries/__init__.py` & `aiokeydb-0.1.9/aiokeydb/commands/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/timeseries/commands.py` & `aiokeydb-0.1.9/aiokeydb/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/timeseries/info.py` & `aiokeydb-0.1.9/aiokeydb/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/commands/timeseries/utils.py` & `aiokeydb-0.1.9/aiokeydb/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/connection.py` & `aiokeydb-0.1.9/aiokeydb/connection.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/core.py` & `aiokeydb-0.1.9/aiokeydb/core.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/crc.py` & `aiokeydb-0.1.9/aiokeydb/crc.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/exceptions.py` & `aiokeydb-0.1.9/aiokeydb/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/lock.py` & `aiokeydb-0.1.9/aiokeydb/lock.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/ocsp.py` & `aiokeydb-0.1.9/aiokeydb/ocsp.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/parsers.py` & `aiokeydb-0.1.9/aiokeydb/parsers.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/README.md` & `aiokeydb-0.1.9/aiokeydb/queues/README.md`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/imports/cron.py` & `aiokeydb-0.1.9/aiokeydb/queues/imports/cron.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/queue.py` & `aiokeydb-0.1.9/aiokeydb/queues/queue.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/types.py` & `aiokeydb-0.1.9/aiokeydb/queues/types.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/utils.py` & `aiokeydb-0.1.9/aiokeydb/queues/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/queues/worker/base.py` & `aiokeydb-0.1.9/aiokeydb/queues/worker/base.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/retry.py` & `aiokeydb-0.1.9/aiokeydb/retry.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/sentinel.py` & `aiokeydb-0.1.9/aiokeydb/sentinel.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/typing.py` & `aiokeydb-0.1.9/aiokeydb/typing.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb/utils.py` & `aiokeydb-0.1.9/aiokeydb/utils.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/aiokeydb.egg-info/PKG-INFO` & `aiokeydb-0.1.9/aiokeydb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiokeydb
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python client for KeyDB database and key-value store
 Home-page: https://github.com/trisongz/aiokeydb-py
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aiokeydb-0.1.8/aiokeydb.egg-info/SOURCES.txt` & `aiokeydb-0.1.9/aiokeydb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/setup.py` & `aiokeydb-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/tests/test_client.py` & `aiokeydb-0.1.9/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/tests/test_multi_config.py` & `aiokeydb-0.1.9/tests/test_multi_config.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/tests/test_suite.py` & `aiokeydb-0.1.9/tests/test_suite.py`

 * *Files identical despite different names*

### Comparing `aiokeydb-0.1.8/tests/test_task_queue.py` & `aiokeydb-0.1.9/tests/test_task_queue.py`

 * *Files identical despite different names*

