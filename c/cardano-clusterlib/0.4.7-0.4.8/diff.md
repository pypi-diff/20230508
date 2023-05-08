# Comparing `tmp/cardano-clusterlib-0.4.7.tar.gz` & `tmp/cardano-clusterlib-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.7.tar", last modified: Wed May  3 11:50:55 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.8.tar", last modified: Mon May  8 12:51:50 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.7.tar` & `cardano-clusterlib-0.4.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.582057 cardano-clusterlib-0.4.7/.github/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.583057 cardano-clusterlib-0.4.7/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.7/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.7/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.7/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1347 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.7/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.7/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.7/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.7/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.7/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.7/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.585057 cardano-clusterlib-0.4.7/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/address_group.py
--rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    14563 2023-05-03 11:46:08.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18201 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    62487 2023-05-03 11:46:08.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.7/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-03 11:50:55.000000 cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.7/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.7/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.7/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.7/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.7/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.7/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.7/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.7/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.7/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.7/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)     1124 2023-05-03 11:50:55.587057 cardano-clusterlib-0.4.7/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.7/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-03 11:50:55.586058 cardano-clusterlib-0.4.7/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.7/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.174079 cardano-clusterlib-0.4.8/.github/
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.176079 cardano-clusterlib-0.4.8/.github/workflows/
+-rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.8/.github/workflows/repo_lint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.8/.gitignore
+-rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.8/.markdownlint.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     1224 2023-05-06 20:29:59.000000 cardano-clusterlib-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.8/.pylintrc
+-rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.8/.readthedocs.yaml
+-rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.8/CODE-OF-CONDUCT.md
+-rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.8/LICENSE
+-rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.8/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.8/README.md
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/cardano_clusterlib/
+-rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/__init__.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     8119 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/address_group.py
+-rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    15500 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/consts.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/coverage.py
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/helpers.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/key_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/node_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/py.typed
+-rw-r--r--   0 martink   (1000) martink   (1000)    18252 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/query_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)     6849 2023-04-17 13:43:55.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/structs.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    63362 2023-05-08 12:50:28.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/txtools.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.8/cardano_clusterlib/types.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 martink   (1000) martink   (1000)       15 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-05-08 12:51:50.000000 cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/docs/
+-rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.8/docs/Makefile
+-rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.8/docs/requirements.txt
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.178079 cardano-clusterlib-0.4.8/docs/source/
+-rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.8/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)     4112 2023-04-17 08:42:14.000000 cardano-clusterlib-0.4.8/docs/source/conf.py
+-rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.8/docs/source/index.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.8/docs/source/modules.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.8/docs/source/readme.rst
+-rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.8/mypy.ini
+-rw-r--r--   0 martink   (1000) martink   (1000)      610 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.8/pyproject.toml
+-rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.8/requirements-dev.txt
+-rw-r--r--   0 martink   (1000) martink   (1000)      776 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/setup.cfg
+-rw-r--r--   0 martink   (1000) martink   (1000)      202 2023-05-03 11:49:49.000000 cardano-clusterlib-0.4.8/setup.py
+drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-05-08 12:51:50.179079 cardano-clusterlib-0.4.8/upgrading/
+-rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.8/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.7/.gitignore` & `cardano-clusterlib-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/.markdownlint.yaml` & `cardano-clusterlib-0.4.8/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.8/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -22,30 +22,25 @@
     language_version: python3
     exclude_types: [html]
   - id: check-yaml
     language_version: python3
   - id: debug-statements
     language_version: python3
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.261
+  rev: v0.0.265
   hooks:
     - id: ruff
 - repo: https://github.com/shellcheck-py/shellcheck-py
   rev: v0.9.0.2
   hooks:
   - id: shellcheck
 - repo: https://github.com/igorshubovych/markdownlint-cli
-  rev: v0.33.0
+  rev: v0.34.0
   hooks:
   - id: markdownlint
-- repo: https://github.com/rstcheck/rstcheck
-  rev: v6.1.2
-  hooks:
-  - id: rstcheck
-    additional_dependencies: [sphinx]
 - repo: local
   hooks:
   - id: pylint
     name: pylint
     entry: pylint
     language: system
     types: [python]
```

### Comparing `cardano-clusterlib-0.4.7/.pylintrc` & `cardano-clusterlib-0.4.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.8/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/LICENSE` & `cardano-clusterlib-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/Makefile` & `cardano-clusterlib-0.4.8/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/PKG-INFO` & `cardano-clusterlib-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.7/README.md` & `cardano-clusterlib-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/clusterlib_klass.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,35 +33,43 @@
 
     Attributes:
         state_dir: A directory with cluster state files (keys, config files, logs, ...).
         protocol: A cluster protocol - full cardano mode by default.
         tx_era: An era used for transactions, by default same as network Era.
         slots_offset: Difference in slots between cluster's start era and current era
             (e.g. Byron->Mary)
+        socket_path: A path to socket file for communication with the node. This overrides the
+            `CARDANO_NODE_SOCKET_PATH` environment variable.
     """
 
     # pylint: disable=too-many-instance-attributes
 
     def __init__(
         self,
         state_dir: FileType,
         protocol: str = consts.Protocols.CARDANO,
         tx_era: str = "",
         slots_offset: int = 0,
+        socket_path: FileType = "",
     ):
         self.cluster_id = 0  # can be used for identifying cluster instance
         self.cli_coverage: dict = {}
         self._rand_str = helpers.get_rand_str(4)
         self._cli_log = ""
         self.protocol = protocol
 
         self.state_dir = Path(state_dir).expanduser().resolve()
         if not self.state_dir.exists():
             raise exceptions.CLIError(f"The state dir `{self.state_dir}` doesn't exist.")
 
+        self._init_socket_path = socket_path
+        self.socket_path: Optional[Path] = None
+        self.socket_args: List[str] = []
+        self.set_socket_path(socket_path=socket_path)
+
         self.pparams_file = self.state_dir / f"pparams-{self._rand_str}.json"
 
         self.genesis_json = clusterlib_helpers._find_genesis_json(clusterlib_obj=self)
         with open(self.genesis_json, encoding="utf-8") as in_json:
             self.genesis = json.load(in_json)
 
         self.slot_length = self.genesis["slotLength"]
@@ -97,14 +105,28 @@
         self._node_group: Optional[node_group.NodeGroup] = None
         self._key_group: Optional[key_group.KeyGroup] = None
         self._genesis_group: Optional[genesis_group.GenesisGroup] = None
         self._governance_group: Optional[governance_group.GovernanceGroup] = None
 
         clusterlib_helpers._check_protocol(clusterlib_obj=self)
 
+    def set_socket_path(self, socket_path: Optional[FileType]) -> None:
+        """Set a path to socket file for communication with the node."""
+        if not socket_path:
+            self.socket_path = None
+            self.socket_args = []
+            return
+
+        socket_path = Path(socket_path).expanduser().resolve()
+        if not socket_path.exists():
+            raise exceptions.CLIError(f"The socket `{socket_path}` doesn't exist.")
+
+        self.socket_path = socket_path
+        self.socket_args = ["--socket-path", str(self.socket_path)]
+
     @property
     def g_transaction(self) -> transaction_group.TransactionGroup:
         """Transaction group."""
         if not self._transaction_group:
             self._transaction_group = transaction_group.TransactionGroup(clusterlib_obj=self)
         return self._transaction_group
```

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/query_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     def query_cli(self, cli_args: UnpackableSequence, cli_sub_args: UnpackableSequence = ()) -> str:
         """Run the `cardano-cli query` command."""
         stdout = self._clusterlib_obj.cli(
             [
                 "query",
                 *cli_args,
                 *self._clusterlib_obj.magic_args,
+                *self._clusterlib_obj.socket_args,
                 f"--{self._clusterlib_obj.protocol}-mode",
                 *cli_sub_args,
             ]
         ).stdout
         stdout_dec = stdout.decode("utf-8") if stdout else ""
         return stdout_dec
```

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/structs.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/transaction_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -339,14 +339,15 @@
         return_collateral_txouts: structs.OptionalTxOuts = (),
         total_collateral_amount: Optional[int] = None,
         mint: structs.OptionalMint = (),
         tx_files: Optional[structs.TxFiles] = None,
         complex_certs: structs.OptionalScriptCerts = (),
         fee: int = 0,
         required_signers: OptionalFiles = (),
+        required_signer_hashes: Optional[List[str]] = None,
         ttl: Optional[int] = None,
         withdrawals: structs.OptionalTxOuts = (),
         script_withdrawals: structs.OptionalScriptWithdrawals = (),
         deposit: Optional[int] = None,
         invalid_hereafter: Optional[int] = None,
         invalid_before: Optional[int] = None,
         join_txouts: bool = True,
@@ -370,14 +371,16 @@
             tx_files: A `structs.TxFiles` tuple containing files needed for the transaction
                 (optional).
             complex_certs: An iterable of `ComplexCert`, specifying certificates script data
                 (optional).
             fee: A fee amount (optional).
             required_signers: An iterable of filepaths of the signing keys whose signatures
                 are required (optional).
+            required_signer_hashes: A list of hashes of the signing keys whose signatures
+                are required (optional).
             ttl: A last block when the transaction is still valid
                 (deprecated in favor of `invalid_hereafter`, optional).
             withdrawals: A list (iterable) of `TxOuts`, specifying reward withdrawals (optional).
             script_withdrawals: An iterable of `ScriptWithdrawal`, specifying withdrawal script
                 data (optional).
             deposit: A deposit amount needed by the transaction (optional).
             invalid_hereafter: A last block when the transaction is still valid (optional).
@@ -427,14 +430,15 @@
             readonly_reference_txins=readonly_reference_txins,
             script_txins=script_txins,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             mint=mint,
             complex_certs=complex_certs,
             required_signers=required_signers,
+            required_signer_hashes=required_signer_hashes,
             withdrawals=collected_data.withdrawals,
             script_withdrawals=collected_data.script_withdrawals,
             invalid_hereafter=invalid_hereafter or ttl,
             invalid_before=invalid_before,
             join_txouts=join_txouts,
         )
 
@@ -494,14 +498,16 @@
         readonly_reference_txins: structs.OptionalUTXOData = (),
         script_txins: structs.OptionalScriptTxIn = (),
         return_collateral_txouts: structs.OptionalTxOuts = (),
         total_collateral_amount: Optional[int] = None,
         mint: structs.OptionalMint = (),
         tx_files: Optional[structs.TxFiles] = None,
         complex_certs: structs.OptionalScriptCerts = (),
+        required_signers: OptionalFiles = (),
+        required_signer_hashes: Optional[List[str]] = None,
         ttl: Optional[int] = None,
         withdrawals: structs.OptionalTxOuts = (),
         script_withdrawals: structs.OptionalScriptWithdrawals = (),
         invalid_hereafter: Optional[int] = None,
         invalid_before: Optional[int] = None,
         witness_count_add: int = 0,
         join_txouts: bool = True,
@@ -523,14 +529,18 @@
             total_collateral_amount: An integer indicating the total amount of collateral
                 (optional).
             mint: An iterable of `Mint`, specifying script minting data (optional).
             tx_files: A `structs.TxFiles` tuple containing files needed for the transaction
                 (optional).
             complex_certs: An iterable of `ComplexCert`, specifying certificates script data
                 (optional).
+            required_signers: An iterable of filepaths of the signing keys whose signatures
+                are required (optional).
+            required_signer_hashes: A list of hashes of the signing keys whose signatures
+                are required (optional).
             ttl: A last block when the transaction is still valid
                 (deprecated in favor of `invalid_hereafter`, optional).
             withdrawals: A list (iterable) of `TxOuts`, specifying reward withdrawals (optional).
             script_withdrawals: An iterable of `ScriptWithdrawal`, specifying withdrawal script
                 data (optional).
             invalid_hereafter: A last block when the transaction is still valid (optional).
             invalid_before: A first block when the transaction is valid (optional).
@@ -564,14 +574,16 @@
             readonly_reference_txins=readonly_reference_txins,
             script_txins=script_txins,
             return_collateral_txouts=return_collateral_txouts,
             total_collateral_amount=total_collateral_amount,
             mint=mint,
             tx_files=tx_files,
             complex_certs=complex_certs,
+            required_signers=required_signers,
+            required_signer_hashes=required_signer_hashes,
             fee=0,
             withdrawals=withdrawals,
             script_withdrawals=script_withdrawals,
             invalid_hereafter=invalid_hereafter or ttl,
             invalid_before=invalid_before,
             deposit=0,
             join_txouts=join_txouts,
@@ -863,14 +875,15 @@
             *helpers._prepend_flag("--metadata-json-file", tx_files.metadata_json_files),
             *helpers._prepend_flag("--metadata-cbor-file", tx_files.metadata_cbor_files),
             *helpers._prepend_flag("--withdrawal", withdrawal_strings),
             *txtools._get_return_collateral_txout_args(txouts=return_collateral_txouts),
             *misc_args,
             *self.tx_era_arg,
             *self._clusterlib_obj.magic_args,
+            *self._clusterlib_obj.socket_args,
         ]
         stdout = self._clusterlib_obj.cli(cli_args).stdout
         stdout_dec = stdout.decode("utf-8") if stdout else ""
 
         # check for the presence of fee information so compatibility with older versions
         # of the `build` command is preserved
         estimated_fee = -1
@@ -1030,14 +1043,15 @@
             tx_file: A path to signed transaction file.
         """
         self._clusterlib_obj.cli(
             [
                 "transaction",
                 "submit",
                 *self._clusterlib_obj.magic_args,
+                *self._clusterlib_obj.socket_args,
                 "--tx-file",
                 str(tx_file),
                 f"--{self._clusterlib_obj.protocol}-mode",
             ]
         )
 
     def submit_tx(
@@ -1183,14 +1197,15 @@
                 readonly_reference_txins=readonly_reference_txins,
                 script_txins=script_txins,
                 return_collateral_txouts=return_collateral_txouts,
                 total_collateral_amount=total_collateral_amount,
                 mint=mint,
                 tx_files=tx_files,
                 complex_certs=complex_certs,
+                required_signers=required_signers,
                 withdrawals=withdrawals,
                 script_withdrawals=script_withdrawals,
                 invalid_hereafter=invalid_hereafter or ttl,
                 witness_count_add=witness_count_add,
                 join_txouts=join_txouts,
                 destination_dir=destination_dir,
             )
```

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.8/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.7
+Version: 0.4.8
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `cardano-clusterlib-0.4.7/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.8/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/docs/Makefile` & `cardano-clusterlib-0.4.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.8/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/docs/source/conf.py` & `cardano-clusterlib-0.4.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/pyproject.toml` & `cardano-clusterlib-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.7/setup.cfg` & `cardano-clusterlib-0.4.8/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-[flake8]
-ignore = E128,E811,W503,E203,PT001,PT004,PT007,PT012,PT018,PT023,PL123
-max_line_length = 100
-
-[pydocstyle]
-inherit = false
-ignore = D10,D203,D212,D213,D214,D215,D404,D405,D406,D407,D408,D409,D410,D411,D413
-match = .*\.py
-
-[rstcheck]
-ignore_directives = 
-	automodule,
-	mdinclude,
-ignore_messages = (Undefined substitution referenced: \":)
-
 [metadata]
 name = cardano-clusterlib
 url = https://github.com/input-output-hk/cardano-clusterlib-py
 maintainer = Martin Kourim
 maintainer_email = martin.kourim@iohk.io
 description = Python wrapper for cardano-cli for working with cardano cluster
 long_description = file: README.md
```

### Comparing `cardano-clusterlib-0.4.7/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.8/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

