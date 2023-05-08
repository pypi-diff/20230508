# Comparing `tmp/trilogy-public-models-0.0.6.tar.gz` & `tmp/trilogy-public-models-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trilogy-public-models-0.0.6.tar", last modified: Mon Apr 10 01:29:06 2023, max compression
+gzip compressed data, was "trilogy-public-models-0.0.8.tar", last modified: Mon May  8 14:05:18 2023, max compression
```

## Comparing `trilogy-public-models-0.0.6.tar` & `trilogy-public-models-0.0.8.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/commits.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/contents.preql
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/datasources.preql
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/files.preql
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/language.preql
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/licenses.preql
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/repo.preql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/trends.preql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/conference.preql
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/datasources.preql
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/division.preql
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game.preql
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game_event.preql
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/league.preql
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/player.preql
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/team.preql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/bikes.preql
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/riders.preql
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/stations.preql
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/trips.preql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.244178 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/answer.preql
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/badge.preql
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/question.preql
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/tag.preql
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/user.preql
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/inventory.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-10 01:28:53.000000 trilogy-public-models-0.0.6/trilogy_public_models/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 01:29:06.240178 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-10 01:29:06.000000 trilogy-public-models-0.0.6/trilogy_public_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.228150 trilogy-public-models-0.0.8/trilogy_public_models/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.228150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.228150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/commits.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/contents.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/datasources.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/files.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/language.preql
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/licenses.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/repo.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.228150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/google_search_trends/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/google_search_trends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/google_search_trends/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/google_search_trends/trends.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/conference.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/datasources.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/division.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/game.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/game_event.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/league.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/player.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/team.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/bikes.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/riders.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/stations.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/trips.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/answer.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/badge.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/question.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/tag.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/user.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.232150 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/usa_names/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/usa_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/bigquery/usa_names/entrypoint.preql
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-08 14:05:06.000000 trilogy-public-models-0.0.8/trilogy_public_models/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 14:05:18.228150 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-08 14:05:18.000000 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-08 14:05:18.000000 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 14:05:18.000000 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-08 14:05:18.000000 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-08 14:05:18.000000 trilogy-public-models-0.0.8/trilogy_public_models.egg-info/top_level.txt
```

### Comparing `trilogy-public-models-0.0.6/PKG-INFO` & `trilogy-public-models-0.0.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trilogy-public-models
-Version: 0.0.6
+Version: 0.0.8
 Summary: Public trilogy/preql models.
 Home-page: 
 Author: 
 Author-email: preql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # trilogy-public-models
 
 ## Overview
 
 This repository contains semantic models on public datasets for the Preql/Trilogy language.
```

### Comparing `trilogy-public-models-0.0.6/README.md` & `trilogy-public-models-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/setup.py` & `trilogy-public-models-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,11 +29,11 @@
     package_data={
         "": ["*.preql", "py.typed"],
     },
     install_requires=install_requires,
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
 )
```

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/__init__.py` & `trilogy-public-models-0.0.8/trilogy_public_models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from preql import Environment
 from typing import Dict
 from os.path import dirname
 import sys
 
 models: Dict["str", Environment] = {}
 
-__version__ = "0.0.6"
+__version__ = "0.0.8"
 
 for loader, module_name, is_pkg in pkgutil.walk_packages([dirname(__file__)]):
     module = loader.find_module(module_name)  # type: ignore
     if not module:
         continue
     _module = module.load_module(module_name)
     try:
```

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/github/datasources.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/github/datasources.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/google_search_trends/trends.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/google_search_trends/trends.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/datasources.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/datasources.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/game.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/game_event.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/game_event.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/ncaa_basketball/team.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/ncaa_basketball/team.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/stations.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/stations.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/new_york_citibike/trips.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/new_york_citibike/trips.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/answer.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/answer.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/bigquery/stack_overflow/question.preql` & `trilogy-public-models-0.0.8/trilogy_public_models/bigquery/stack_overflow/question.preql`

 * *Files identical despite different names*

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/inventory.py` & `trilogy-public-models-0.0.8/trilogy_public_models/inventory.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from os import listdir
 from os.path import dirname, join
-from pathlib import Path
 
 from preql import Environment
 from preql.parser import parse
 
 
 def parse_initial_models(fpath: str) -> Environment:
     files = listdir(dirname(fpath))
```

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models/validator.py` & `trilogy-public-models-0.0.8/trilogy_public_models/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from preql import Environment
-from preql.core.models import Grain, Concept, Datasource
+from preql.core.models import Concept, Datasource
 from preql.executor import Executor
 from preql.parser import parse_text
 from preql.core.processing.concept_strategies_v2 import source_concepts
 
 
 def validate_dataset(
     dataset: Datasource, environment: Environment, executor: Executor, dry_run_client
```

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models.egg-info/PKG-INFO` & `trilogy-public-models-0.0.8/trilogy_public_models.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: trilogy-public-models
-Version: 0.0.6
+Version: 0.0.8
 Summary: Public trilogy/preql models.
 Home-page: 
 Author: 
 Author-email: preql-community@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # trilogy-public-models
 
 ## Overview
 
 This repository contains semantic models on public datasets for the Preql/Trilogy language.
```

### Comparing `trilogy-public-models-0.0.6/trilogy_public_models.egg-info/SOURCES.txt` & `trilogy-public-models-0.0.8/trilogy_public_models.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -41,8 +41,10 @@
 trilogy_public_models/bigquery/stack_overflow/__init__.py
 trilogy_public_models/bigquery/stack_overflow/answer.preql
 trilogy_public_models/bigquery/stack_overflow/badge.preql
 trilogy_public_models/bigquery/stack_overflow/entrypoint.preql
 trilogy_public_models/bigquery/stack_overflow/question.preql
 trilogy_public_models/bigquery/stack_overflow/tag.preql
 trilogy_public_models/bigquery/stack_overflow/user.preql
-trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
+trilogy_public_models/bigquery/stack_overflow/user_metrics.preql
+trilogy_public_models/bigquery/usa_names/__init__.py
+trilogy_public_models/bigquery/usa_names/entrypoint.preql
```

