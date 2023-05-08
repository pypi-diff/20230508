# Comparing `tmp/databricks-cli-0.9.0.tar.gz` & `tmp/databricks-cli-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/databricks-cli-0.9.0.tar", last modified: Wed Aug 28 21:59:15 2019, max compression
+gzip compressed data, was "dist/databricks-cli-0.9.1.tar", last modified: Thu Oct 31 23:45:09 2019, max compression
```

## Comparing `databricks-cli-0.9.0.tar` & `databricks-cli-0.9.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3652 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/PKG-INFO
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/integration/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1691 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/conftest.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/integration/workspace/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/workspace/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     5358 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/workspace/test_integration.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/__init__.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/integration/dbfs/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/dbfs/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     4566 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/integration/dbfs/test_integration.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli.egg-info/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3652 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/PKG-INFO
--rw-r--r--   0 andrew.chen   (502) staff       (20)        1 2019-01-31 23:33:16.000000 databricks-cli-0.9.0/databricks_cli.egg-info/not-zip-safe
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1956 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/SOURCES.txt
--rw-r--r--   0 andrew.chen   (502) staff       (20)      121 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/entry_points.txt
--rw-r--r--   0 andrew.chen   (502) staff       (20)       76 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/requires.txt
--rw-r--r--   0 andrew.chen   (502) staff       (20)       27 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/top_level.txt
--rw-r--r--   0 andrew.chen   (502) staff       (20)        1 2019-08-28 21:59:14.000000 databricks-cli-0.9.0/databricks_cli.egg-info/dependency_links.txt
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2241 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/setup.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)       38 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/setup.cfg
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1287 2019-08-28 21:34:06.000000 databricks-cli-0.9.0/databricks_cli/version.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/configure/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3738 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/configure/config.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    10513 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/configure/provider.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/configure/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3609 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/configure/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/secrets/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/secrets/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2225 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/secrets/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    13303 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/secrets/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/workspace/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/workspace/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3109 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/workspace/types.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     7718 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/workspace/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     8670 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/workspace/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/clusters/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/clusters/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2645 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/clusters/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    12878 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/clusters/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1514 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/__init__.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/libraries/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/libraries/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1682 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/libraries/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    12454 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/libraries/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/groups/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/groups/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3370 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/groups/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     6627 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/groups/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     4671 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/click_types.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2658 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     3561 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/utils.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/sdk/
--rw-r--r--   0 andrew.chen   (502) staff       (20)    35719 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/sdk/service.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1085 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/sdk/version.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1827 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/sdk/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     5343 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/sdk/api_client.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/dbfs/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/dbfs/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    11601 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/dbfs/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     5893 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/dbfs/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1122 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/dbfs/exceptions.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     4143 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/dbfs/dbfs_path.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/instance_pools/
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/instance_pools/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1832 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/instance_pools/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     6644 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/instance_pools/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/stack/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/stack/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)    27054 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/stack/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     6359 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/databricks_cli/stack/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1108 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/stack/exceptions.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/jobs/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/jobs/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2403 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/jobs/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     7898 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/jobs/cli.py
-drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-08-28 21:59:15.000000 databricks-cli-0.9.0/databricks_cli/runs/
--rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.0/databricks_cli/runs/__init__.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     1752 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/runs/api.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     6227 2019-08-28 21:33:17.000000 databricks-cli-0.9.0/databricks_cli/runs/cli.py
--rw-r--r--   0 andrew.chen   (502) staff       (20)     2601 2019-07-31 01:38:58.000000 databricks-cli-0.9.0/README.rst
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3652 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/PKG-INFO
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/integration/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1691 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/conftest.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/integration/workspace/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/workspace/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     5358 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/workspace/test_integration.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/__init__.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/integration/dbfs/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/dbfs/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     4566 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/integration/dbfs/test_integration.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3652 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/PKG-INFO
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        1 2019-01-31 23:33:16.000000 databricks-cli-0.9.1/databricks_cli.egg-info/not-zip-safe
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1956 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew.chen   (502) staff       (20)      121 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/entry_points.txt
+-rw-r--r--   0 andrew.chen   (502) staff       (20)       76 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/requires.txt
+-rw-r--r--   0 andrew.chen   (502) staff       (20)       27 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/top_level.txt
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        1 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2241 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/setup.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)       38 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/setup.cfg
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1287 2019-10-31 23:44:53.000000 databricks-cli-0.9.1/databricks_cli/version.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/configure/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3738 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/configure/config.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    10513 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/configure/provider.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/configure/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3609 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/configure/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/secrets/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/secrets/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2225 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/secrets/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    13511 2019-10-31 23:44:53.000000 databricks-cli-0.9.1/databricks_cli/secrets/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/workspace/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/workspace/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3195 2019-10-31 23:44:53.000000 databricks-cli-0.9.1/databricks_cli/workspace/types.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     7718 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/workspace/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     8670 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/workspace/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/clusters/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/clusters/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2645 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/clusters/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    12878 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/clusters/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1514 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/__init__.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/libraries/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/libraries/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1682 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/libraries/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    12454 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/libraries/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/groups/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/groups/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3370 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/groups/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     6627 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/groups/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     4671 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/click_types.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2658 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     3561 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/utils.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/sdk/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    35719 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/sdk/service.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1085 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/sdk/version.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1827 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/sdk/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     5343 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/sdk/api_client.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/dbfs/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/dbfs/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    11601 2019-10-31 23:44:36.000000 databricks-cli-0.9.1/databricks_cli/dbfs/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     5893 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/dbfs/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1122 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/dbfs/exceptions.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     4143 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/dbfs/dbfs_path.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/instance_pools/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1068 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/instance_pools/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1832 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/instance_pools/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     6644 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/instance_pools/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/stack/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/stack/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)    27054 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/stack/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     6359 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/databricks_cli/stack/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1108 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/stack/exceptions.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/jobs/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/jobs/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2403 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/jobs/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     7898 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/jobs/cli.py
+drwxr-xr-x   0 andrew.chen   (502) staff       (20)        0 2019-10-31 23:45:09.000000 databricks-cli-0.9.1/databricks_cli/runs/
+-rw-r--r--   0 andrew.chen   (502) staff       (20)        0 2019-01-31 23:21:21.000000 databricks-cli-0.9.1/databricks_cli/runs/__init__.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     1752 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/runs/api.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     6227 2019-08-28 21:33:17.000000 databricks-cli-0.9.1/databricks_cli/runs/cli.py
+-rw-r--r--   0 andrew.chen   (502) staff       (20)     2601 2019-07-31 01:38:58.000000 databricks-cli-0.9.1/README.rst
```

### Comparing `databricks-cli-0.9.0/PKG-INFO` & `databricks-cli-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: databricks-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: A command line interface for Databricks
 Home-page: https://github.com/databricks/databricks-cli
 Author: Andrew Chen
 Author-email: andrewchen@databricks.com
 License: Apache License 2.0
 Description: databricks-cli
         ==============
```

### Comparing `databricks-cli-0.9.0/integration/conftest.py` & `databricks-cli-0.9.1/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/integration/workspace/test_integration.py` & `databricks-cli-0.9.1/integration/workspace/test_integration.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/integration/__init__.py` & `databricks-cli-0.9.1/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/integration/dbfs/__init__.py` & `databricks-cli-0.9.1/integration/dbfs/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/integration/dbfs/test_integration.py` & `databricks-cli-0.9.1/integration/dbfs/test_integration.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli.egg-info/PKG-INFO` & `databricks-cli-0.9.1/databricks_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: databricks-cli
-Version: 0.9.0
+Version: 0.9.1
 Summary: A command line interface for Databricks
 Home-page: https://github.com/databricks/databricks-cli
 Author: Andrew Chen
 Author-email: andrewchen@databricks.com
 License: Apache License 2.0
 Description: databricks-cli
         ==============
```

### Comparing `databricks-cli-0.9.0/databricks_cli.egg-info/SOURCES.txt` & `databricks-cli-0.9.1/databricks_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/setup.py` & `databricks-cli-0.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/version.py` & `databricks-cli-0.9.1/databricks_cli/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-version = '0.9.0' #  NOQA
+version = '0.9.1' #  NOQA
 
 
 def print_version_callback(ctx, param, value): #  NOQA
     import click
     if not value or ctx.resilient_parsing:
         return
     click.echo('Version {}'.format(version))
```

### Comparing `databricks-cli-0.9.0/databricks_cli/configure/config.py` & `databricks-cli-0.9.1/databricks_cli/configure/config.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/configure/provider.py` & `databricks-cli-0.9.1/databricks_cli/configure/provider.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/configure/__init__.py` & `databricks-cli-0.9.1/databricks_cli/configure/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/configure/cli.py` & `databricks-cli-0.9.1/databricks_cli/configure/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/secrets/__init__.py` & `databricks-cli-0.9.1/databricks_cli/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/secrets/api.py` & `databricks-cli-0.9.1/databricks_cli/secrets/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/secrets/cli.py` & `databricks-cli-0.9.1/databricks_cli/secrets/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from databricks_cli.secrets.api import SecretApi
 from databricks_cli.utils import eat_exceptions, CONTEXT_SETTINGS, pretty_format, truncate_string, \
     error_and_quit
 from databricks_cli.configure.config import provide_api_client, profile_option, debug_option
 from databricks_cli.version import print_version_callback, version
 
 
-SCOPE_HEADER = ('Scope', 'Backend')
+SCOPE_HEADER = ('Scope', 'Backend', 'KeyVault URL')
 SECRET_HEADER = ('Key name', 'Last updated')
 ACL_HEADER = ('Principal', 'Permission')
 DASH_MARKER = '# ' + '-' * 70 + '\n'
 
 
 @click.command(context_settings=CONTEXT_SETTINGS,
                short_help="Creates a secret scope.")
@@ -60,15 +60,19 @@
     """
     SecretApi(api_client).create_scope(scope, initial_manage_principal)
 
 
 def _scopes_to_table(scopes_json):
     ret = []
     for s in scopes_json.get('scopes', []):
-        ret.append((truncate_string(s['name']), s['backend_type']))
+        if "keyvault_metadata" in s:
+            url = s["keyvault_metadata"]["dns_name"]
+            ret.append((truncate_string(s['name']), s['backend_type'], url))
+        else:
+            ret.append((truncate_string(s['name']), s['backend_type'], "N/A"))
     return ret
 
 
 @click.command(context_settings=CONTEXT_SETTINGS,
                short_help='Lists all secret scopes.')
 @click.option('--output', help=OutputClickType.help, type=OutputClickType())
 @debug_option
```

### Comparing `databricks-cli-0.9.0/databricks_cli/workspace/types.py` & `databricks-cli-0.9.1/databricks_cli/workspace/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,29 +26,31 @@
 
 class WorkspaceLanguage(object):
     SCALA = 'SCALA'
     PYTHON = 'PYTHON'
     SQL = 'SQL'
     R = 'R'
     ALL = [SCALA, PYTHON, SQL, R]
-    EXTENSIONS = ['.scala', '.py', '.sql', '.SQL', '.r', '.R', '.ipynb']
+    EXTENSIONS = ['.scala', '.py', '.sql', '.SQL', '.r', '.R', '.ipynb', '.html']
 
     @classmethod
     def to_language_and_format(cls, path):
         ext = cls.get_extension(path).lower()
         if ext == '.scala':
             return (cls.SCALA, WorkspaceFormat.SOURCE)
         elif ext == '.py':
             return (cls.PYTHON, WorkspaceFormat.SOURCE)
         elif ext == '.sql':
             return (cls.SQL, WorkspaceFormat.SOURCE)
         elif ext == '.r':
             return (cls.R, WorkspaceFormat.SOURCE)
         elif ext == '.ipynb':
             return (cls.PYTHON, WorkspaceFormat.JUPYTER)
+        elif ext == '.html':
+            return (None, WorkspaceFormat.HTML)
 
     @classmethod
     def to_extension(cls, language):
         if language == cls.SCALA:
             return '.scala'
         elif language == cls.PYTHON:
             return '.py'
```

### Comparing `databricks-cli-0.9.0/databricks_cli/workspace/api.py` & `databricks-cli-0.9.1/databricks_cli/workspace/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/workspace/cli.py` & `databricks-cli-0.9.1/databricks_cli/workspace/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/clusters/api.py` & `databricks-cli-0.9.1/databricks_cli/clusters/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/clusters/cli.py` & `databricks-cli-0.9.1/databricks_cli/clusters/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/__init__.py` & `databricks-cli-0.9.1/databricks_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/libraries/__init__.py` & `databricks-cli-0.9.1/databricks_cli/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/libraries/api.py` & `databricks-cli-0.9.1/databricks_cli/libraries/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/libraries/cli.py` & `databricks-cli-0.9.1/databricks_cli/libraries/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/groups/api.py` & `databricks-cli-0.9.1/databricks_cli/groups/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/groups/cli.py` & `databricks-cli-0.9.1/databricks_cli/groups/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/click_types.py` & `databricks-cli-0.9.1/databricks_cli/click_types.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/cli.py` & `databricks-cli-0.9.1/databricks_cli/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/utils.py` & `databricks-cli-0.9.1/databricks_cli/utils.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/sdk/service.py` & `databricks-cli-0.9.1/databricks_cli/sdk/service.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/sdk/version.py` & `databricks-cli-0.9.1/databricks_cli/sdk/version.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/sdk/__init__.py` & `databricks-cli-0.9.1/databricks_cli/sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/sdk/api_client.py` & `databricks-cli-0.9.1/databricks_cli/sdk/api_client.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/dbfs/__init__.py` & `databricks-cli-0.9.1/databricks_cli/dbfs/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/dbfs/api.py` & `databricks-cli-0.9.1/databricks_cli/dbfs/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/dbfs/cli.py` & `databricks-cli-0.9.1/databricks_cli/dbfs/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/dbfs/exceptions.py` & `databricks-cli-0.9.1/databricks_cli/dbfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/dbfs/dbfs_path.py` & `databricks-cli-0.9.1/databricks_cli/dbfs/dbfs_path.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/instance_pools/__init__.py` & `databricks-cli-0.9.1/databricks_cli/instance_pools/__init__.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/instance_pools/api.py` & `databricks-cli-0.9.1/databricks_cli/instance_pools/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/instance_pools/cli.py` & `databricks-cli-0.9.1/databricks_cli/instance_pools/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/stack/api.py` & `databricks-cli-0.9.1/databricks_cli/stack/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/stack/cli.py` & `databricks-cli-0.9.1/databricks_cli/stack/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/stack/exceptions.py` & `databricks-cli-0.9.1/databricks_cli/stack/exceptions.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/jobs/api.py` & `databricks-cli-0.9.1/databricks_cli/jobs/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/jobs/cli.py` & `databricks-cli-0.9.1/databricks_cli/jobs/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/runs/api.py` & `databricks-cli-0.9.1/databricks_cli/runs/api.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/databricks_cli/runs/cli.py` & `databricks-cli-0.9.1/databricks_cli/runs/cli.py`

 * *Files identical despite different names*

### Comparing `databricks-cli-0.9.0/README.rst` & `databricks-cli-0.9.1/README.rst`

 * *Files identical despite different names*

