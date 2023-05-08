# Comparing `tmp/nitric-0.9.2.dev3.tar.gz` & `tmp/nitric-0.9.2.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nitric-0.9.2.dev3.tar", last modified: Tue Apr 11 04:01:12 2023, max compression
+gzip compressed data, was "nitric-0.9.2.dev4.tar", last modified: Wed May  3 00:26:23 2023, max compression
```

## Comparing `nitric-0.9.2.dev3.tar` & `nitric-0.9.2.dev4.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/application.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/config/default_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    21168 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/faas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/proto/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric/proto/nitric/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/deploy/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/document/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/document/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/error/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/error/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/event/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/event/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/faas/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/faas/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/queue/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/queue/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/resource/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/secret/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/
--rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/proto/validate/
--rw-r--r--   0 runner    (1001) docker     (123)    37084 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/proto/validate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.862969 nitric-0.9.2.dev3/nitric/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/buckets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/queues.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/resources/topics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-04-11 04:01:09.000000 nitric-0.9.2.dev3/nitric/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 04:01:12.858970 nitric-0.9.2.dev3/nitric.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-11 04:01:12.000000 nitric-0.9.2.dev3/nitric.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 04:01:12.866970 nitric-0.9.2.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-04-11 04:00:31.000000 nitric-0.9.2.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.816513 nitric-0.9.2.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-03 00:25:23.000000 nitric-0.9.2.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-03 00:26:23.816513 nitric-0.9.2.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-03 00:25:23.000000 nitric-0.9.2.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.804513 nitric-0.9.2.dev4/nitric/
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20891 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5001 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8160 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3990 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/application.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/config/default_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21168 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/faas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/deploy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/deploy/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/deploy/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/document/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/document/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/document/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    12398 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/document/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/error/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.808513 nitric-0.9.2.dev4/nitric/proto/nitric/error/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1802 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/error/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/event/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/event/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5731 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/event/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/faas/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/faas/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/faas/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11014 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/faas/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/queue/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/queue/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/queue/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     9567 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/queue/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/resource/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/resource/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8295 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/resource/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/secret/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)     5355 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/secret/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/nitric/storage/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/nitric/storage/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.812513 nitric-0.9.2.dev4/nitric/proto/validate/
+-rw-r--r--   0 runner    (1001) docker     (123)    37084 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/proto/validate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.816513 nitric-0.9.2.dev4/nitric/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11839 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3715 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3151 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/buckets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/queues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/resources/topics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-03 00:26:17.000000 nitric-0.9.2.dev4/nitric/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:26:23.804513 nitric-0.9.2.dev4/nitric.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-03 00:26:23.000000 nitric-0.9.2.dev4/nitric.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-05-03 00:26:23.000000 nitric-0.9.2.dev4/nitric.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:26:23.000000 nitric-0.9.2.dev4/nitric.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-03 00:26:23.000000 nitric-0.9.2.dev4/nitric.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-03 00:26:23.000000 nitric-0.9.2.dev4/nitric.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-03 00:25:23.000000 nitric-0.9.2.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:26:23.816513 nitric-0.9.2.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-03 00:25:23.000000 nitric-0.9.2.dev4/setup.py
```

### Comparing `nitric-0.9.2.dev3/LICENSE` & `nitric-0.9.2.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/PKG-INFO` & `nitric-0.9.2.dev4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 0.9.2.dev3
+Version: 0.9.2.dev4
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://nitric.io">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev3 Summary: The Nitric SDK
+Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev4 Summary: The Nitric SDK
 for Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io License: UNKNOWN Description:
                                  [Nitric_Logo]
                ***** Build nitric applications with Python *****
          [Build_Status] [Codecov] [Version] [Downloads/week] [Discord]
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework
 with Python 3.10+. For more information check out the main [Nitric repo](https:
```

### Comparing `nitric-0.9.2.dev3/README.md` & `nitric-0.9.2.dev4/README.md`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/__init__.py` & `nitric-0.9.2.dev4/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/__init__.py` & `nitric-0.9.2.dev4/nitric/api/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/const.py` & `nitric-0.9.2.dev4/nitric/api/const.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/documents.py` & `nitric-0.9.2.dev4/nitric/api/documents.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/events.py` & `nitric-0.9.2.dev4/nitric/api/events.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/exception.py` & `nitric-0.9.2.dev4/nitric/api/exception.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/queues.py` & `nitric-0.9.2.dev4/nitric/api/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/secrets.py` & `nitric-0.9.2.dev4/nitric/api/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/api/storage.py` & `nitric-0.9.2.dev4/nitric/api/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,19 +128,19 @@
                 storage_delete_request=StorageDeleteRequest(bucket_name=self._bucket, key=self.key)
             )
         except GRPCError as grpc_err:
             raise exception_from_grpc_error(grpc_err)
 
     async def upload_url(self, expiry: int = 600):
         """Get a temporary writable URL to this file."""
-        await self.sign_url(mode=FileMode.WRITE, expiry=expiry)
+        return await self.sign_url(mode=FileMode.WRITE, expiry=expiry)
 
     async def download_url(self, expiry: int = 600):
         """Get a temporary readable URL to this file."""
-        await self.sign_url(mode=FileMode.READ, expiry=expiry)
+        return await self.sign_url(mode=FileMode.READ, expiry=expiry)
 
     async def sign_url(self, mode: FileMode = FileMode.READ, expiry: int = 3600):
         """Generate a signed URL for reading or writing to a file."""
         try:
             response = await self._storage._storage_stub.pre_sign_url(
                 storage_pre_sign_url_request=StoragePreSignUrlRequest(
                     bucket_name=self._bucket, key=self.key, operation=mode.to_request_operation(), expiry=expiry
```

### Comparing `nitric-0.9.2.dev3/nitric/application.py` & `nitric-0.9.2.dev4/nitric/application.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/config/__init__.py` & `nitric-0.9.2.dev4/nitric/config/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/config/default_settings.py` & `nitric-0.9.2.dev4/nitric/config/default_settings.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/faas.py` & `nitric-0.9.2.dev4/nitric/faas.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/deploy/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/deploy/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/deploy/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/document/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/document/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/document/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/document/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/error/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/error/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/error/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/error/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/event/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/event/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/event/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/event/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/faas/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/faas/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/faas/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/faas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/queue/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/queue/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/queue/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/resource/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/resource/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/resource/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/secret/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/secret/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/secret/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/storage/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/nitric/storage/v1/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/nitric/storage/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/proto/validate/__init__.py` & `nitric-0.9.2.dev4/nitric/proto/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/__init__.py` & `nitric-0.9.2.dev4/nitric/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/apis.py` & `nitric-0.9.2.dev4/nitric/resources/apis.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/base.py` & `nitric-0.9.2.dev4/nitric/resources/base.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/buckets.py` & `nitric-0.9.2.dev4/nitric/resources/buckets.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/collections.py` & `nitric-0.9.2.dev4/nitric/resources/collections.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/queues.py` & `nitric-0.9.2.dev4/nitric/resources/queues.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/schedules.py` & `nitric-0.9.2.dev4/nitric/resources/schedules.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/secrets.py` & `nitric-0.9.2.dev4/nitric/resources/secrets.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/resources/topics.py` & `nitric-0.9.2.dev4/nitric/resources/topics.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric/utils.py` & `nitric-0.9.2.dev4/nitric/utils.py`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/nitric.egg-info/PKG-INFO` & `nitric-0.9.2.dev4/nitric.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nitric
-Version: 0.9.2.dev3
+Version: 0.9.2.dev4
 Summary: The Nitric SDK for Python 3
 Home-page: https://github.com/nitrictech/python-sdk
 Author: Nitric
 Author-email: team@nitric.io
 License: UNKNOWN
 Description: <p align="center">
           <a href="https://nitric.io">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev3 Summary: The Nitric SDK
+Metadata-Version: 2.1 Name: nitric Version: 0.9.2.dev4 Summary: The Nitric SDK
 for Python 3 Home-page: https://github.com/nitrictech/python-sdk Author: Nitric
 Author-email: team@nitric.io License: UNKNOWN Description:
                                  [Nitric_Logo]
                ***** Build nitric applications with Python *****
          [Build_Status] [Codecov] [Version] [Downloads/week] [Discord]
 The Python SDK supports the use of the [Nitric](https://nitric.io) framework
 with Python 3.10+. For more information check out the main [Nitric repo](https:
```

### Comparing `nitric-0.9.2.dev3/nitric.egg-info/SOURCES.txt` & `nitric-0.9.2.dev4/nitric.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nitric-0.9.2.dev3/setup.py` & `nitric-0.9.2.dev4/setup.py`

 * *Files identical despite different names*

