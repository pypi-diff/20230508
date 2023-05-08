# Comparing `tmp/redis-5.0.0b2.tar.gz` & `tmp/redis-5.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redis-5.0.0b2.tar", last modified: Mon Apr 24 15:08:06 2023, max compression
+gzip compressed data, was "redis-5.0.0b3.tar", last modified: Thu May  4 09:43:28 2023, max compression
```

## Comparing `redis-5.0.0b2.tar` & `redis-5.0.0b3.tar`

### file list

```diff
@@ -1,158 +1,158 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.278016 redis-5.0.0b2/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-24 15:07:50.000000 redis-5.0.0b2/INSTALL
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-24 15:07:50.000000 redis-5.0.0b2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-24 15:07:50.000000 redis-5.0.0b2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-24 15:08:06.278016 redis-5.0.0b2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-04-24 15:07:50.000000 redis-5.0.0b2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.258016 redis-5.0.0b2/redis/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55388 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/asyncio/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/backoff.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    79861 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    86601 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/bf/
--rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/bf/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   216287 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/execution_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/path.py
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/graph/query_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis/commands/json/
--rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/json/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/redismodules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/commands/search/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/aggregation.py
--rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/indexDefinition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/querystring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/reducers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/search/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/sentinel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/commands/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/commands/timeseries/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/crc.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/ocsp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.266016 redis-5.0.0b2/redis/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/encoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/hiredis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/resp2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/resp3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/parsers/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/retry.py
--rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-04-24 15:07:50.000000 redis-5.0.0b2/redis/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.262016 redis-5.0.0b2/redis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-24 15:08:06.000000 redis-5.0.0b2/redis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 15:08:06.278016 redis-5.0.0b2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-04-24 15:07:50.000000 redis-5.0.0b2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.270016 redis-5.0.0b2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/asynctests
--rw-r--r--   0 runner    (1001) docker     (123)    15584 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/synctests
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    38371 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_sentinel_managed_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_asyncio/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_asyncio/testdata/will_play_text.csv.bz2
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_command_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_connection_pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.274016 redis-5.0.0b2/tests/test_graph_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_graph_utils/test_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_pubsub.py
--rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_retry.py
--rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_scripting.py
--rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_sentinel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/test_timeseries.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 15:08:06.278016 redis-5.0.0b2/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/jsontestdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/titles.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-04-24 15:07:50.000000 redis-5.0.0b2/tests/testdata/will_play_text.csv.bz2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.397854 redis-5.0.0b3/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-04 09:43:12.000000 redis-5.0.0b3/INSTALL
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 09:43:12.000000 redis-5.0.0b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-04 09:43:12.000000 redis-5.0.0b3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-04 09:43:28.397854 redis-5.0.0b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-04 09:43:12.000000 redis-5.0.0b3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55393 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61198 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51222 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13694 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/asyncio/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/backoff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80560 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86601 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis/commands/bf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6665 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21575 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/bf/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30844 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   216287 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     7009 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10379 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2460 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/execution_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/graph/query_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/json/
+-rw-r--r--   0 runner    (1001) docker     (123)     4331 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14216 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/json/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/redismodules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/search/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10232 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35597 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4519 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/indexDefinition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10522 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/reducers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/search/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4110 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/sentinel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/commands/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33438 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/commands/timeseries/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46593 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/crc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11451 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/ocsp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.385854 redis-5.0.0b3/redis/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9925 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/encoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/hiredis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/resp2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9308 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/resp3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/parsers/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1817 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12626 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-04 09:43:12.000000 redis-5.0.0b3/redis/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.381854 redis-5.0.0b3/redis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7907 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3850 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 09:43:28.000000 redis-5.0.0b3/redis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:43:28.397854 redis-5.0.0b3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-04 09:43:12.000000 redis-5.0.0b3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.389854 redis-5.0.0b3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/asynctests
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7822 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/synctests
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9434 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18706 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112337 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)   122627 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34475 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9314 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4222 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15811 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2672 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13965 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38371 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35180 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_sentinel_managed_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_asyncio/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)   118948 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_command_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)   180759 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30432 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_connection_pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7959 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18914 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/test_graph_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_graph_utils/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42822 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8824 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12616 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28906 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_pubsub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8207 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_retry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8795 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_scripting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53061 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7103 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_sentinel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24927 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/test_timeseries.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:43:28.393854 redis-5.0.0b3/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)    14095 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/jsontestdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98632 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/titles.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2069623 2023-05-04 09:43:12.000000 redis-5.0.0b3/tests/testdata/will_play_text.csv.bz2
```

### Comparing `redis-5.0.0b2/LICENSE` & `redis-5.0.0b3/LICENSE`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/PKG-INFO` & `redis-5.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b2
+Version: 5.0.0b3
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b2/README.md` & `redis-5.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/__init__.py` & `redis-5.0.0b3/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/__init__.py` & `redis-5.0.0b3/redis/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/client.py` & `redis-5.0.0b3/redis/asyncio/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,15 +251,15 @@
             connection_pool = ConnectionPool(**kwargs)
         self.connection_pool = connection_pool
         self.single_connection_client = single_connection_client
         self.connection: Optional[Connection] = None
 
         self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
 
-        if self.connection_pool.connection_kwargs.get("protocol") == "3":
+        if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
             self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
 
         # If using a single connection client, we need to lock creation-of and use-of
         # the client in order to avoid race conditions such as using asyncio.gather
         # on a set of redis commands
         self._single_conn_lock = asyncio.Lock()
```

### Comparing `redis-5.0.0b2/redis/asyncio/cluster.py` & `redis-5.0.0b3/redis/asyncio/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/connection.py` & `redis-5.0.0b3/redis/asyncio/connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/lock.py` & `redis-5.0.0b3/redis/asyncio/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/retry.py` & `redis-5.0.0b3/redis/asyncio/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/sentinel.py` & `redis-5.0.0b3/redis/asyncio/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/asyncio/utils.py` & `redis-5.0.0b3/redis/asyncio/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/backoff.py` & `redis-5.0.0b3/redis/backoff.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/client.py` & `redis-5.0.0b3/redis/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -570,14 +570,34 @@
             cmd_dict["tips"] = command[7]
             cmd_dict["key_specifications"] = command[8]
             cmd_dict["subcommands"] = command[9]
         commands[cmd_name] = cmd_dict
     return commands
 
 
+def parse_command_resp3(response, **options):
+    commands = {}
+    for command in response:
+        cmd_dict = {}
+        cmd_name = str_if_bytes(command[0])
+        cmd_dict["name"] = cmd_name
+        cmd_dict["arity"] = command[1]
+        cmd_dict["flags"] = command[2]
+        cmd_dict["first_key_pos"] = command[3]
+        cmd_dict["last_key_pos"] = command[4]
+        cmd_dict["step_count"] = command[5]
+        cmd_dict["acl_categories"] = command[6]
+        cmd_dict["tips"] = command[7]
+        cmd_dict["key_specifications"] = command[8]
+        cmd_dict["subcommands"] = command[9]
+
+        commands[cmd_name] = cmd_dict
+    return commands
+
+
 def parse_pubsub_numsub(response, **options):
     return list(zip(response[0::2], response[1::2]))
 
 
 def parse_client_kill(response, **options):
     if isinstance(response, int):
         return response
@@ -870,14 +890,15 @@
         "ACL LOG": lambda r: [
             {str_if_bytes(key): str_if_bytes(value) for key, value in x.items()}
             for x in r
         ]
         if isinstance(r, list)
         else bool_ok(r),
         **string_keys_to_dict("XREAD XREADGROUP", parse_xread_resp3),
+        "COMMAND": parse_command_resp3,
         "STRALGO": lambda r, **options: {
             str_if_bytes(key): str_if_bytes(value) for key, value in r.items()
         }
         if isinstance(r, dict)
         else str_if_bytes(r),
         "XINFO CONSUMERS": lambda r: [
             {str_if_bytes(key): value for key, value in x.items()} for x in r
@@ -1084,15 +1105,15 @@
         self.connection_pool = connection_pool
         self.connection = None
         if single_connection_client:
             self.connection = self.connection_pool.get_connection("_")
 
         self.response_callbacks = CaseInsensitiveDict(self.__class__.RESPONSE_CALLBACKS)
 
-        if self.connection_pool.connection_kwargs.get("protocol") == "3":
+        if self.connection_pool.connection_kwargs.get("protocol") in ["3", 3]:
             self.response_callbacks.update(self.__class__.RESP3_RESPONSE_CALLBACKS)
 
     def __repr__(self):
         return f"{type(self).__name__}<{repr(self.connection_pool)}>"
 
     def get_encoder(self):
         """Get the connection pool's encoder"""
```

### Comparing `redis-5.0.0b2/redis/cluster.py` & `redis-5.0.0b3/redis/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/__init__.py` & `redis-5.0.0b3/redis/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/bf/__init__.py` & `redis-5.0.0b3/redis/commands/bf/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/bf/commands.py` & `redis-5.0.0b3/redis/commands/bf/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/bf/info.py` & `redis-5.0.0b3/redis/commands/bf/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/cluster.py` & `redis-5.0.0b3/redis/commands/cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/core.py` & `redis-5.0.0b3/redis/commands/core.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/__init__.py` & `redis-5.0.0b3/redis/commands/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/commands.py` & `redis-5.0.0b3/redis/commands/graph/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/edge.py` & `redis-5.0.0b3/redis/commands/graph/edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/execution_plan.py` & `redis-5.0.0b3/redis/commands/graph/execution_plan.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/node.py` & `redis-5.0.0b3/redis/commands/graph/node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/path.py` & `redis-5.0.0b3/redis/commands/graph/path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/graph/query_result.py` & `redis-5.0.0b3/redis/commands/graph/query_result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/helpers.py` & `redis-5.0.0b3/redis/commands/helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/json/__init__.py` & `redis-5.0.0b3/redis/commands/json/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/json/commands.py` & `redis-5.0.0b3/redis/commands/json/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/json/decoders.py` & `redis-5.0.0b3/redis/commands/json/decoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/redismodules.py` & `redis-5.0.0b3/redis/commands/redismodules.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/__init__.py` & `redis-5.0.0b3/redis/commands/search/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/aggregation.py` & `redis-5.0.0b3/redis/commands/search/aggregation.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/commands.py` & `redis-5.0.0b3/redis/commands/search/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/field.py` & `redis-5.0.0b3/redis/commands/search/field.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/indexDefinition.py` & `redis-5.0.0b3/redis/commands/search/indexDefinition.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/query.py` & `redis-5.0.0b3/redis/commands/search/query.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/querystring.py` & `redis-5.0.0b3/redis/commands/search/querystring.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/reducers.py` & `redis-5.0.0b3/redis/commands/search/reducers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/result.py` & `redis-5.0.0b3/redis/commands/search/result.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/search/suggestion.py` & `redis-5.0.0b3/redis/commands/search/suggestion.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/sentinel.py` & `redis-5.0.0b3/redis/commands/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/timeseries/__init__.py` & `redis-5.0.0b3/redis/commands/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/timeseries/commands.py` & `redis-5.0.0b3/redis/commands/timeseries/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/timeseries/info.py` & `redis-5.0.0b3/redis/commands/timeseries/info.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/commands/timeseries/utils.py` & `redis-5.0.0b3/redis/commands/timeseries/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/connection.py` & `redis-5.0.0b3/redis/connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/crc.py` & `redis-5.0.0b3/redis/crc.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/credentials.py` & `redis-5.0.0b3/redis/credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/exceptions.py` & `redis-5.0.0b3/redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/lock.py` & `redis-5.0.0b3/redis/lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/ocsp.py` & `redis-5.0.0b3/redis/ocsp.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/__init__.py` & `redis-5.0.0b3/redis/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/base.py` & `redis-5.0.0b3/redis/parsers/base.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/commands.py` & `redis-5.0.0b3/redis/parsers/commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/encoders.py` & `redis-5.0.0b3/redis/parsers/encoders.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/hiredis.py` & `redis-5.0.0b3/redis/parsers/hiredis.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/resp2.py` & `redis-5.0.0b3/redis/parsers/resp2.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/parsers/resp3.py` & `redis-5.0.0b3/redis/parsers/resp3.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,18 +76,24 @@
         elif byte == b"*":
             response = [
                 self._read_response(disable_decoding=disable_decoding)
                 for _ in range(int(response))
             ]
         # set response
         elif byte == b"~":
-            response = {
+            # redis can return unhashable types (like dict) in a set,
+            # so we need to first convert to a list, and then try to convert it to a set
+            response = [
                 self._read_response(disable_decoding=disable_decoding)
                 for _ in range(int(response))
-            }
+            ]
+            try:
+                response = set(response)
+            except TypeError:
+                pass
         # map response
         elif byte == b"%":
             response = {
                 self._read_response(
                     disable_decoding=disable_decoding
                 ): self._read_response(
                     disable_decoding=disable_decoding, push_request=push_request
@@ -195,18 +201,24 @@
         elif byte == b"*":
             response = [
                 (await self._read_response(disable_decoding=disable_decoding))
                 for _ in range(int(response))
             ]
         # set response
         elif byte == b"~":
-            response = {
+            # redis can return unhashable types (like dict) in a set,
+            # so we need to first convert to a list, and then try to convert it to a set
+            response = [
                 (await self._read_response(disable_decoding=disable_decoding))
                 for _ in range(int(response))
-            }
+            ]
+            try:
+                response = set(response)
+            except TypeError:
+                pass
         # map response
         elif byte == b"%":
             response = {
                 (await self._read_response(disable_decoding=disable_decoding)): (
                     await self._read_response(disable_decoding=disable_decoding)
                 )
                 for _ in range(int(response))
```

### Comparing `redis-5.0.0b2/redis/parsers/socket.py` & `redis-5.0.0b3/redis/parsers/socket.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/retry.py` & `redis-5.0.0b3/redis/retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/sentinel.py` & `redis-5.0.0b3/redis/sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/typing.py` & `redis-5.0.0b3/redis/typing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis/utils.py` & `redis-5.0.0b3/redis/utils.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/redis.egg-info/PKG-INFO` & `redis-5.0.0b3/redis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redis
-Version: 5.0.0b2
+Version: 5.0.0b3
 Summary: Python client for Redis database and key-value store
 Home-page: https://github.com/redis/redis-py
 Author: Redis Inc.
 Author-email: oss@redis.com
 License: MIT
 Project-URL: Documentation, https://redis.readthedocs.io/en/latest/
 Project-URL: Changes, https://github.com/redis/redis-py/releases
```

### Comparing `redis-5.0.0b2/redis.egg-info/SOURCES.txt` & `redis-5.0.0b3/redis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/setup.py` & `redis-5.0.0b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="redis",
     description="Python client for Redis database and key-value store",
     long_description=open("README.md").read().strip(),
     long_description_content_type="text/markdown",
     keywords=["Redis", "key-value store", "database"],
     license="MIT",
-    version="5.0.0b2",
+    version="5.0.0b3",
     packages=find_packages(
         include=[
             "redis",
             "redis.asyncio",
             "redis.commands",
             "redis.commands.bf",
             "redis.commands.json",
```

### Comparing `redis-5.0.0b2/tests/asynctests` & `redis-5.0.0b3/tests/asynctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/conftest.py` & `redis-5.0.0b3/tests/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -475,8 +475,8 @@
 
 
 def is_resp2_connection(r):
     if isinstance(r, redis.Redis):
         protocol = r.connection_pool.connection_kwargs.get("protocol")
     elif isinstance(r, redis.RedisCluster):
         protocol = r.nodes_manager.connection_kwargs.get("protocol")
-    return protocol == "2" or protocol is None
+    return protocol in ["2", 2, None]
```

### Comparing `redis-5.0.0b2/tests/mocks.py` & `redis-5.0.0b3/tests/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/synctests` & `redis-5.0.0b3/tests/synctests`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/conftest.py` & `redis-5.0.0b3/tests/test_asyncio/conftest.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/mocks.py` & `redis-5.0.0b3/tests/test_asyncio/mocks.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_bloom.py` & `redis-5.0.0b3/tests/test_asyncio/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_cluster.py` & `redis-5.0.0b3/tests/test_asyncio/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_commands.py` & `redis-5.0.0b3/tests/test_asyncio/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_connection.py` & `redis-5.0.0b3/tests/test_asyncio/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_connection_pool.py` & `redis-5.0.0b3/tests/test_asyncio/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_credentials.py` & `redis-5.0.0b3/tests/test_asyncio/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_encoding.py` & `redis-5.0.0b3/tests/test_asyncio/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_graph.py` & `redis-5.0.0b3/tests/test_asyncio/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_json.py` & `redis-5.0.0b3/tests/test_asyncio/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_lock.py` & `redis-5.0.0b3/tests/test_asyncio/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_monitor.py` & `redis-5.0.0b3/tests/test_asyncio/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_pipeline.py` & `redis-5.0.0b3/tests/test_asyncio/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_pubsub.py` & `redis-5.0.0b3/tests/test_asyncio/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_retry.py` & `redis-5.0.0b3/tests/test_asyncio/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_scripting.py` & `redis-5.0.0b3/tests/test_asyncio/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_search.py` & `redis-5.0.0b3/tests/test_asyncio/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_sentinel.py` & `redis-5.0.0b3/tests/test_asyncio/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_sentinel_managed_connection.py` & `redis-5.0.0b3/tests/test_asyncio/test_sentinel_managed_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/test_timeseries.py` & `redis-5.0.0b3/tests/test_asyncio/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/testdata/jsontestdata.py` & `redis-5.0.0b3/tests/test_asyncio/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/testdata/titles.csv` & `redis-5.0.0b3/tests/test_asyncio/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_asyncio/testdata/will_play_text.csv.bz2` & `redis-5.0.0b3/tests/test_asyncio/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_bloom.py` & `redis-5.0.0b3/tests/test_bloom.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_cluster.py` & `redis-5.0.0b3/tests/test_cluster.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_command_parser.py` & `redis-5.0.0b3/tests/test_command_parser.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_commands.py` & `redis-5.0.0b3/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_connection.py` & `redis-5.0.0b3/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_connection_pool.py` & `redis-5.0.0b3/tests/test_connection_pool.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_credentials.py` & `redis-5.0.0b3/tests/test_credentials.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_encoding.py` & `redis-5.0.0b3/tests/test_encoding.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_function.py` & `redis-5.0.0b3/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_graph.py` & `redis-5.0.0b3/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_graph_utils/test_edge.py` & `redis-5.0.0b3/tests/test_graph_utils/test_edge.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_graph_utils/test_node.py` & `redis-5.0.0b3/tests/test_graph_utils/test_node.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_graph_utils/test_path.py` & `redis-5.0.0b3/tests/test_graph_utils/test_path.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_helpers.py` & `redis-5.0.0b3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_json.py` & `redis-5.0.0b3/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_lock.py` & `redis-5.0.0b3/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_monitor.py` & `redis-5.0.0b3/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_multiprocessing.py` & `redis-5.0.0b3/tests/test_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_pipeline.py` & `redis-5.0.0b3/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_pubsub.py` & `redis-5.0.0b3/tests/test_pubsub.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_retry.py` & `redis-5.0.0b3/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_scripting.py` & `redis-5.0.0b3/tests/test_scripting.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_search.py` & `redis-5.0.0b3/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_sentinel.py` & `redis-5.0.0b3/tests/test_sentinel.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_ssl.py` & `redis-5.0.0b3/tests/test_ssl.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/test_timeseries.py` & `redis-5.0.0b3/tests/test_timeseries.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/testdata/jsontestdata.py` & `redis-5.0.0b3/tests/testdata/jsontestdata.py`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/testdata/titles.csv` & `redis-5.0.0b3/tests/testdata/titles.csv`

 * *Files identical despite different names*

### Comparing `redis-5.0.0b2/tests/testdata/will_play_text.csv.bz2` & `redis-5.0.0b3/tests/testdata/will_play_text.csv.bz2`

 * *Files identical despite different names*

