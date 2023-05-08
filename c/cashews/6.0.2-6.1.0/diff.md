# Comparing `tmp/cashews-6.0.2.tar.gz` & `tmp/cashews-6.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cashews-6.0.2.tar", last modified: Tue Apr  4 22:25:25 2023, max compression
+gzip compressed data, was "dist/cashews-6.1.0.tar", last modified: Mon May  8 17:09:35 2023, max compression
```

## Comparing `cashews-6.0.2.tar` & `cashews-6.1.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.303780 cashews-6.0.2/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-03-15 17:20:31.000000 cashews-6.0.2/LICENSE
--rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-04-04 22:25:25.304067 cashews-6.0.2/PKG-INFO
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.292097 cashews-6.0.2/cashews/
--rw-r--r--   0 pandadoc   (501) staff       (20)     1281 2023-04-01 17:20:20.000000 cashews-6.0.2/cashews/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1464 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/_typing.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.294932 cashews-6.0.2/cashews/backends/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.0.2/cashews/backends/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     9148 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/backends/diskcache.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     6438 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/backends/interface.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     8648 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/backends/memory.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.296187 cashews-6.0.2/cashews/backends/redis/
--rw-r--r--   0 pandadoc   (501) staff       (20)      213 2023-04-01 17:21:03.000000 cashews-6.0.2/cashews/backends/redis/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    10542 2023-03-31 23:54:32.000000 cashews-6.0.2/cashews/backends/redis/backend.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1881 2023-04-01 10:22:37.000000 cashews-6.0.2/cashews/backends/redis/client.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    12475 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/backends/redis/client_side.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    11670 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/backends/transaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      639 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/cache_condition.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      882 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/commands.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.296651 cashews-6.0.2/cashews/contrib/
--rw-r--r--   0 pandadoc   (501) staff       (20)       63 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/contrib/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1701 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/contrib/_starlette.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.298007 cashews-6.0.2/cashews/decorators/
--rw-r--r--   0 pandadoc   (501) staff       (20)      616 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     7303 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/bloom.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.299811 cashews-6.0.2/cashews/decorators/cache/
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.0.2/cashews/decorators/cache/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2000 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/defaults.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4006 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/early.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2732 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/fail.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3247 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/hit.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2408 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/iterator.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2324 2023-04-02 09:24:36.000000 cashews-6.0.2/cashews/decorators/cache/simple.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3531 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/cache/soft.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3004 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/circuit_breaker.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3505 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/locked.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2253 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/rate.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2234 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/decorators/rate_slide.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      961 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/exceptions.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     6968 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/formatter.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2372 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/helpers.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     5924 2023-04-02 08:52:05.000000 cashews-6.0.2/cashews/key.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1900 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/picklers.py
--rw-r--r--   0 pandadoc   (501) staff       (20)        0 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/py.typed
--rw-r--r--   0 pandadoc   (501) staff       (20)     8004 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/serialize.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1124 2023-04-01 18:49:21.000000 cashews-6.0.2/cashews/ttl.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.300977 cashews-6.0.2/cashews/utils/
--rw-r--r--   0 pandadoc   (501) staff       (20)      175 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/utils/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1415 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/utils/_bitarray.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1713 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/utils/_bitarray_lib.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      848 2022-11-14 08:28:19.000000 cashews-6.0.2/cashews/utils/object_size.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      862 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/utils/split_hash.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2795 2023-04-04 22:17:36.000000 cashews-6.0.2/cashews/validation.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.303357 cashews-6.0.2/cashews/wrapper/
--rw-r--r--   0 pandadoc   (501) staff       (20)      558 2023-04-01 17:20:44.000000 cashews-6.0.2/cashews/wrapper/__init__.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      623 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/wrapper/auto_init.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     2749 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/wrapper/backend_settings.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     6862 2023-04-04 22:17:36.000000 cashews-6.0.2/cashews/wrapper/commands.py
--rw-r--r--   0 pandadoc   (501) staff       (20)    11806 2023-04-04 22:21:42.000000 cashews-6.0.2/cashews/wrapper/decorators.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     1558 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/wrapper/disable_control.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4437 2023-04-04 22:17:36.000000 cashews-6.0.2/cashews/wrapper/tags.py
--rw-r--r--   0 pandadoc   (501) staff       (20)      820 2023-03-27 18:56:42.000000 cashews-6.0.2/cashews/wrapper/time_condition.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     4163 2023-04-04 22:17:36.000000 cashews-6.0.2/cashews/wrapper/transaction.py
--rw-r--r--   0 pandadoc   (501) staff       (20)     3026 2023-04-01 00:09:08.000000 cashews-6.0.2/cashews/wrapper/wrapper.py
-drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-04-04 22:25:25.293513 cashews-6.0.2/cashews.egg-info/
--rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-04-04 22:25:24.000000 cashews-6.0.2/cashews.egg-info/PKG-INFO
--rw-r--r--   0 pandadoc   (501) staff       (20)     1721 2023-04-04 22:25:25.000000 cashews-6.0.2/cashews.egg-info/SOURCES.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-04-04 22:25:24.000000 cashews-6.0.2/cashews.egg-info/dependency_links.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-04-04 22:25:24.000000 cashews-6.0.2/cashews.egg-info/not-zip-safe
--rw-r--r--   0 pandadoc   (501) staff       (20)      200 2023-04-04 22:25:25.000000 cashews-6.0.2/cashews.egg-info/requires.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)        8 2023-04-04 22:25:25.000000 cashews-6.0.2/cashews.egg-info/top_level.txt
--rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2023-04-04 22:25:25.304846 cashews-6.0.2/setup.cfg
--rw-r--r--   0 pandadoc   (501) staff       (20)       52 2022-03-15 17:20:32.000000 cashews-6.0.2/setup.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.236388 cashews-6.1.0/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1081 2022-03-15 17:20:31.000000 cashews-6.1.0/LICENSE
+-rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-05-08 17:09:35.236574 cashews-6.1.0/PKG-INFO
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.217746 cashews-6.1.0/cashews/
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1281 2023-04-01 17:20:20.000000 cashews-6.1.0/cashews/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1464 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/_typing.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.220555 cashews-6.1.0/cashews/backends/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.1.0/cashews/backends/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     9148 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/diskcache.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6438 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/interface.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8648 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/memory.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.221954 cashews-6.1.0/cashews/backends/redis/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      213 2023-04-01 17:21:03.000000 cashews-6.1.0/cashews/backends/redis/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    10542 2023-03-31 23:54:32.000000 cashews-6.1.0/cashews/backends/redis/backend.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1881 2023-04-01 10:22:37.000000 cashews-6.1.0/cashews/backends/redis/client.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    12475 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/redis/client_side.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    11670 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/backends/transaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      639 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/cache_condition.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      882 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/commands.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.222636 cashews-6.1.0/cashews/contrib/
+-rw-r--r--   0 pandadoc   (501) staff       (20)       63 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/contrib/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1701 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/contrib/_starlette.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.224148 cashews-6.1.0/cashews/decorators/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      616 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7303 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/bloom.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.226227 cashews-6.1.0/cashews/decorators/cache/
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2022-03-15 17:20:31.000000 cashews-6.1.0/cashews/decorators/cache/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2000 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/defaults.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4006 2023-05-08 07:21:58.000000 cashews-6.1.0/cashews/decorators/cache/early.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2732 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/cache/fail.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3247 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/hit.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2408 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/iterator.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2324 2023-04-02 09:24:36.000000 cashews-6.1.0/cashews/decorators/cache/simple.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3531 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/cache/soft.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3004 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/circuit_breaker.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3505 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/decorators/locked.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2253 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/rate.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2234 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/decorators/rate_slide.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      961 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/exceptions.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     7214 2023-05-08 17:06:55.000000 cashews-6.1.0/cashews/formatter.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2372 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/helpers.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     5924 2023-05-04 21:58:39.000000 cashews-6.1.0/cashews/key.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1900 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/picklers.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)        0 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/py.typed
+-rw-r--r--   0 pandadoc   (501) staff       (20)     8004 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/serialize.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1124 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/ttl.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.233228 cashews-6.1.0/cashews/utils/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      175 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1415 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/_bitarray.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1713 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/_bitarray_lib.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      848 2022-11-14 08:28:19.000000 cashews-6.1.0/cashews/utils/object_size.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      862 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/utils/split_hash.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2795 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/validation.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.236138 cashews-6.1.0/cashews/wrapper/
+-rw-r--r--   0 pandadoc   (501) staff       (20)      558 2023-04-01 17:20:44.000000 cashews-6.1.0/cashews/wrapper/__init__.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      623 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/wrapper/auto_init.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     2749 2023-04-05 06:41:56.000000 cashews-6.1.0/cashews/wrapper/backend_settings.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     6862 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/commands.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)    11806 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/decorators.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1558 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/disable_control.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4437 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/tags.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)      820 2023-03-27 18:56:42.000000 cashews-6.1.0/cashews/wrapper/time_condition.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     4163 2023-04-04 22:17:36.000000 cashews-6.1.0/cashews/wrapper/transaction.py
+-rw-r--r--   0 pandadoc   (501) staff       (20)     3026 2023-05-08 17:06:36.000000 cashews-6.1.0/cashews/wrapper/wrapper.py
+drwxr-xr-x   0 pandadoc   (501) staff       (20)        0 2023-05-08 17:09:35.219116 cashews-6.1.0/cashews.egg-info/
+-rw-r--r--   0 pandadoc   (501) staff       (20)    28062 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/PKG-INFO
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1721 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/SOURCES.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/dependency_links.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        1 2023-05-08 17:09:34.000000 cashews-6.1.0/cashews.egg-info/not-zip-safe
+-rw-r--r--   0 pandadoc   (501) staff       (20)      200 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/requires.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)        8 2023-05-08 17:09:35.000000 cashews-6.1.0/cashews.egg-info/top_level.txt
+-rw-r--r--   0 pandadoc   (501) staff       (20)     1452 2023-05-08 17:09:35.237156 cashews-6.1.0/setup.cfg
+-rw-r--r--   0 pandadoc   (501) staff       (20)       52 2022-03-15 17:20:32.000000 cashews-6.1.0/setup.py
```

### Comparing `cashews-6.0.2/LICENSE` & `cashews-6.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/PKG-INFO` & `cashews-6.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 6.0.2
+Version: 6.1.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
 Platform: UNKNOWN
```

### Comparing `cashews-6.0.2/cashews/__init__.py` & `cashews-6.1.0/cashews/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/_typing.py` & `cashews-6.1.0/cashews/_typing.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/diskcache.py` & `cashews-6.1.0/cashews/backends/diskcache.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/interface.py` & `cashews-6.1.0/cashews/backends/interface.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/memory.py` & `cashews-6.1.0/cashews/backends/memory.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/redis/backend.py` & `cashews-6.1.0/cashews/backends/redis/backend.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/redis/client.py` & `cashews-6.1.0/cashews/backends/redis/client.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/redis/client_side.py` & `cashews-6.1.0/cashews/backends/redis/client_side.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/backends/transaction.py` & `cashews-6.1.0/cashews/backends/transaction.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/cache_condition.py` & `cashews-6.1.0/cashews/cache_condition.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/commands.py` & `cashews-6.1.0/cashews/commands.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/contrib/_starlette.py` & `cashews-6.1.0/cashews/contrib/_starlette.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/__init__.py` & `cashews-6.1.0/cashews/decorators/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/bloom.py` & `cashews-6.1.0/cashews/decorators/bloom.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/defaults.py` & `cashews-6.1.0/cashews/decorators/cache/defaults.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/early.py` & `cashews-6.1.0/cashews/decorators/cache/early.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/fail.py` & `cashews-6.1.0/cashews/decorators/cache/fail.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/hit.py` & `cashews-6.1.0/cashews/decorators/cache/hit.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/iterator.py` & `cashews-6.1.0/cashews/decorators/cache/iterator.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/simple.py` & `cashews-6.1.0/cashews/decorators/cache/simple.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/cache/soft.py` & `cashews-6.1.0/cashews/decorators/cache/soft.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/circuit_breaker.py` & `cashews-6.1.0/cashews/decorators/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/locked.py` & `cashews-6.1.0/cashews/decorators/locked.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/rate.py` & `cashews-6.1.0/cashews/decorators/rate.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/decorators/rate_slide.py` & `cashews-6.1.0/cashews/decorators/rate_slide.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/exceptions.py` & `cashews-6.1.0/cashews/exceptions.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/formatter.py` & `cashews-6.1.0/cashews/formatter.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,44 +85,50 @@
 
     def format_field(self, value, format_spec):
         return format(self._format_field(value))
 
 
 class _FuncFormatter(_ReplaceFormatter):
     def __init__(self, *args: Any, **kwargs: Any) -> None:
-        self._functions = {}
+        self._functions: Dict[str, Tuple[Callable, bool]] = {}
         super().__init__(*args, **kwargs)
 
-    def _register(self, alias, function) -> None:
-        self._functions[alias] = function
+    def _register(self, alias: str, function: Callable, preformat: bool = True) -> None:
+        self._functions[alias] = (function, preformat)
 
-    def register(self, alias):
+    def register(self, alias: str, preformat: bool = True):
         def _decorator(func):
-            self._register(alias, func)
+            self._register(alias, func, preformat=preformat)
             return func
 
         return _decorator
 
-    def format_field(self, value, format_spec):
+    def format_field(self, value: Any, format_spec: str) -> TemplateValue:
         format_spec, args = self.parse_format_spec(format_spec)
-        value = super().format_field(value, format_spec if format_spec not in self._functions else "")
-        if format_spec in self._functions:
-            value = self._functions[format_spec](value, *args)
-        return value
+        if format_spec not in self._functions:
+            return super().format_field(value, format_spec)
+        func, preformat = self._functions[format_spec]
+        if preformat:
+            value = super().format_field(value, "")
+        return func(value, *args)
 
     @staticmethod
-    def parse_format_spec(format_spec):
+    def parse_format_spec(format_spec: str):
         if not format_spec or "(" not in format_spec:
             return format_spec, ()
         format_spec, args = format_spec.split("(", 1)
         return format_spec, args.replace(")", "").split(",")
 
 
 default_formatter = _FuncFormatter(lambda name: "")
-default_formatter._register("len", lambda x: str(len(x)))
+
+
+@default_formatter.register("len")
+def _len(value: TemplateValue):
+    return str(len(value))
 
 
 @default_formatter.register("jwt")
 def _jwt_func(jwt: TemplateValue, key: str) -> TemplateValue:
     _, payload, _ = jwt.split(".", 2)
     payload_dict = json.loads(base64.b64decode(payload))
     return payload_dict.get(key)
```

### Comparing `cashews-6.0.2/cashews/helpers.py` & `cashews-6.1.0/cashews/helpers.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/key.py` & `cashews-6.1.0/cashews/key.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/picklers.py` & `cashews-6.1.0/cashews/picklers.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/serialize.py` & `cashews-6.1.0/cashews/serialize.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/ttl.py` & `cashews-6.1.0/cashews/ttl.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/utils/_bitarray.py` & `cashews-6.1.0/cashews/utils/_bitarray.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/utils/_bitarray_lib.py` & `cashews-6.1.0/cashews/utils/_bitarray_lib.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/utils/object_size.py` & `cashews-6.1.0/cashews/utils/object_size.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/utils/split_hash.py` & `cashews-6.1.0/cashews/utils/split_hash.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/validation.py` & `cashews-6.1.0/cashews/validation.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/__init__.py` & `cashews-6.1.0/cashews/wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/auto_init.py` & `cashews-6.1.0/cashews/wrapper/auto_init.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/backend_settings.py` & `cashews-6.1.0/cashews/wrapper/backend_settings.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/commands.py` & `cashews-6.1.0/cashews/wrapper/commands.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/decorators.py` & `cashews-6.1.0/cashews/wrapper/decorators.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/disable_control.py` & `cashews-6.1.0/cashews/wrapper/disable_control.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/tags.py` & `cashews-6.1.0/cashews/wrapper/tags.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/time_condition.py` & `cashews-6.1.0/cashews/wrapper/time_condition.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/transaction.py` & `cashews-6.1.0/cashews/wrapper/transaction.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews/wrapper/wrapper.py` & `cashews-6.1.0/cashews/wrapper/wrapper.py`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/cashews.egg-info/PKG-INFO` & `cashews-6.1.0/cashews.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cashews
-Version: 6.0.2
+Version: 6.1.0
 Summary: cache tools with async power
 Home-page: https://github.com/Krukov/cashews/
 Author: Dmitry Kryukov
 Author-email: glebov.ru@gmail.com
 License: MIT
 Keywords: cache aio async multicache aiocache
 Platform: UNKNOWN
```

### Comparing `cashews-6.0.2/cashews.egg-info/SOURCES.txt` & `cashews-6.1.0/cashews.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cashews-6.0.2/setup.cfg` & `cashews-6.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cashews
-version = 6.0.2
+version = 6.1.0
 url = https://github.com/Krukov/cashews/
 author = Dmitry Kryukov
 author_email = glebov.ru@gmail.com
 description = cache tools with async power
 keywords = cache aio async multicache aiocache
 long_description = file: README.md
 long_description_content_type = text/markdown
```

