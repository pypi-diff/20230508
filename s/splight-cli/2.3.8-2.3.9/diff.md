# Comparing `tmp/splight-cli-2.3.8.tar.gz` & `tmp/splight-cli-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splight-cli-2.3.8.tar", last modified: Thu Mar 30 20:58:29 2023, max compression
+gzip compressed data, was "splight-cli-2.3.9.tar", last modified: Mon Apr  3 11:29:34 2023, max compression
```

## Comparing `splight-cli-2.3.8.tar` & `splight-cli-2.3.9.tar`

### file list

```diff
@@ -1,100 +1,100 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.208506 splight-cli-2.3.8/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-30 20:58:29.204506 splight-cli-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-03-30 20:58:28.000000 splight-cli-2.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.200506 splight-cli-2.3.8/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.200506 splight-cli-2.3.8/cli/component/
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.200506 splight-cli-2.3.8/cli/component/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/templates/Initialization
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/templates/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/templates/auto_readme.md
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/templates/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/templates/spec.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/component/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/tests/test_create.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/tests/test_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/component/tests/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/config/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/context/
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/context/framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/context/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/deployment/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/deployment/deployment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/alert/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/alert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/asset/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/asset/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/attribute/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/attribute/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/component/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/component/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/datalake/
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/datalake/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/datalake/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/datalake/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/datalake/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/datalake/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/datalake/tests/test_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/file/
--rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/manager/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/manager/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/query/
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/secret/
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/engine/setpoint/
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/engine/setpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/hub/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/hub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/hub/component/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/hub/component/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/hub/component/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/hub/component/hub_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/tests/TestHub/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/tests/TestHub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/tests/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/tests/test_generic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/api_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/headers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/input.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/utils/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/cli/workspace/
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-30 20:58:28.000000 splight-cli-2.3.8/cli/workspace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 20:58:29.208506 splight-cli-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-03-30 20:58:28.000000 splight-cli-2.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 20:58:29.204506 splight-cli-2.3.8/splight_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-30 20:58:29.000000 splight-cli-2.3.8/splight_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.772240 splight-cli-2.3.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 11:29:34.772240 splight-cli-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15178 2023-04-03 11:29:33.000000 splight-cli-2.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.764240 splight-cli-2.3.9/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5980 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7736 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/Initialization
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/auto_readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/templates/spec.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/component/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/component/tests/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/context/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/deployment/deployment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/alert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/asset/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/asset/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/attribute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/attribute/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/component/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/datalake/
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/datalake/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/datalake/tests/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/file/
+-rw-r--r--   0 runner    (1001) docker     (123)     2187 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8149 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/manager/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/secret/
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/engine/setpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/engine/setpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/hub/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/hub/component/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5957 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/hub/component/hub_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/tests/TestHub/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/TestHub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/test_configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/tests/test_generic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/api_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/utils/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.768240 splight-cli-2.3.9/cli/workspace/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-03 11:29:33.000000 splight-cli-2.3.9/cli/workspace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 11:29:34.772240 splight-cli-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-03 11:29:33.000000 splight-cli-2.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 11:29:34.772240 splight-cli-2.3.9/splight_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-03 11:29:34.000000 splight-cli-2.3.9/splight_cli.egg-info/top_level.txt
```

### Comparing `splight-cli-2.3.8/README.md` & `splight-cli-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/cli.py` & `splight-cli-2.3.9/cli/cli.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/__init__.py` & `splight-cli-2.3.9/cli/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/component.py` & `splight-cli-2.3.9/cli/component/component.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/exceptions.py` & `splight-cli-2.3.9/cli/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/loaders.py` & `splight-cli-2.3.9/cli/component/loaders.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/spec.py` & `splight-cli-2.3.9/cli/component/spec.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/templates/auto_readme.md` & `splight-cli-2.3.9/cli/component/templates/auto_readme.md`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/templates/component.py` & `splight-cli-2.3.9/cli/component/templates/component.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/templates/spec.json` & `splight-cli-2.3.9/cli/component/templates/spec.json`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/tests/test_create.py` & `splight-cli-2.3.9/cli/component/tests/test_create.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/tests/test_initialize.py` & `splight-cli-2.3.9/cli/component/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/component/tests/test_run.py` & `splight-cli-2.3.9/cli/component/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/config/__init__.py` & `splight-cli-2.3.9/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/constants.py` & `splight-cli-2.3.9/cli/constants.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/context/__init__.py` & `splight-cli-2.3.9/cli/context/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/context/framework.py` & `splight-cli-2.3.9/cli/context/framework.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/context/workspace.py` & `splight-cli-2.3.9/cli/context/workspace.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/deployment/__init__.py` & `splight-cli-2.3.9/cli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/deployment/deployment.py` & `splight-cli-2.3.9/cli/deployment/deployment.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/__init__.py` & `splight-cli-2.3.9/cli/engine/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/alert/__init__.py` & `splight-cli-2.3.9/cli/engine/alert/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/asset/__init__.py` & `splight-cli-2.3.9/cli/engine/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/attribute/__init__.py` & `splight-cli-2.3.9/cli/engine/attribute/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/component/__init__.py` & `splight-cli-2.3.9/cli/engine/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/datalake/__init__.py` & `splight-cli-2.3.9/cli/engine/datalake/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/datalake/tests/test_dump.py` & `splight-cli-2.3.9/cli/engine/datalake/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/datalake/tests/test_list.py` & `splight-cli-2.3.9/cli/engine/datalake/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/datalake/tests/test_load.py` & `splight-cli-2.3.9/cli/engine/datalake/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/file/__init__.py` & `splight-cli-2.3.9/cli/engine/file/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/graph/__init__.py` & `splight-cli-2.3.9/cli/engine/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/manager/manager.py` & `splight-cli-2.3.9/cli/engine/manager/manager.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/query/__init__.py` & `splight-cli-2.3.9/cli/engine/query/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/secret/__init__.py` & `splight-cli-2.3.9/cli/engine/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/engine/setpoint/__init__.py` & `splight-cli-2.3.9/cli/engine/setpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/hub/component/__init__.py` & `splight-cli-2.3.9/cli/hub/component/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/hub/component/exceptions.py` & `splight-cli-2.3.9/cli/hub/component/exceptions.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/hub/component/hub_manager.py` & `splight-cli-2.3.9/cli/hub/component/hub_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -89,45 +89,45 @@
         table = Table("Name", "Version", "Verification", "Privacy Policy")
         for item in components:
             table.add_row(
                 name, item.version, item.verification, item.privacy_policy
             )
         console.print(table)
 
+    def _get_ignore_pathspec(self, path):
+        try:
+            with open(os.path.join(path, SPLIGHT_IGNORE), "r") as splightignore:
+                return pathspec.PathSpec.from_lines(
+                    'gitwildmatch',
+                    splightignore
+                )
+        except FileNotFoundError:
+            return None
+
     def _upload_component(self, spec: Dict[str, Any], path: str):
         name = spec["name"]
         version = spec["version"]
 
         file_name = f"{name}-{version}.{COMPRESSION_TYPE}"
         versioned_name = f"{name}-{version}"
         readme_path = os.path.join(path, README_FILE_1)
         if not os.path.exists(readme_path):
             readme_path = os.path.join(path, README_FILE_2)
-        try:
-            with open(os.path.join(path, SPLIGHT_IGNORE), "r") as splightignore:
-                regexes = pathspec.PathSpec.from_lines(
-                    'gitwildmatch',
-                    splightignore
-                )
-            ignored_files = set(regexes.match_tree(path))
-        except FileNotFoundError:
-            ignored_files = set()
 
         try:
-            with py7zr.SevenZipFile(file_name, "w") as fid:
-                matched_files = filter(
-                    lambda f: f not in ignored_files,
-                    os.listdir(path)
-                )
-                for included_file in matched_files:
-                    fid.write(
-                        os.path.join(path, included_file),
-                        os.path.join(versioned_name, included_file)
-                    )
-
+            ignore_pathpec = self._get_ignore_pathspec(path)
+            with py7zr.SevenZipFile(file_name, "w") as archive:
+                for root, _, files in os.walk(path):
+                    if ignore_pathpec and ignore_pathpec.match_file(root):
+                        continue
+                    for file in files:
+                        if ignore_pathpec and ignore_pathpec.match_file(os.path.join(root, file)):
+                            continue
+                        filepath = os.path.join(root, file)
+                        archive.write(filepath, os.path.join(versioned_name, filepath))
             data = {
                 "name": name,
                 "version": version,
                 "splight_cli_version": spec["splight_cli_version"],
                 "privacy_policy": spec.get("privacy_policy", "private"),
                 "tags": spec.get("tags", []),
                 "custom_types": json.dumps(spec.get("custom_types", [])),
```

### Comparing `splight-cli-2.3.8/cli/settings.py` & `splight-cli-2.3.9/cli/settings.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/tests/test_configure.py` & `splight-cli-2.3.9/cli/tests/test_configure.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/tests/test_generic.py` & `splight-cli-2.3.9/cli/tests/test_generic.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/utils/api_requests.py` & `splight-cli-2.3.9/cli/utils/api_requests.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/utils/input.py` & `splight-cli-2.3.9/cli/utils/input.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/utils/loader.py` & `splight-cli-2.3.9/cli/utils/loader.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/utils/pprint.py` & `splight-cli-2.3.9/cli/utils/pprint.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/utils/yaml.py` & `splight-cli-2.3.9/cli/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/cli/workspace/__init__.py` & `splight-cli-2.3.9/cli/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/setup.py` & `splight-cli-2.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `splight-cli-2.3.8/splight_cli.egg-info/SOURCES.txt` & `splight-cli-2.3.9/splight_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

